# Stripy Horse Go SDK

Official Go client for the [Stripy Horse](https://stripyhorse.io) API - Zebra/ZPL
developer tools: render ZPL to PNG, convert PDFs/images/HTML to print-ready ZPL,
and drive hosted virtual Zebra printers from your tests.

Generated from the live [OpenAPI spec](https://stripyhorse.io/openapi.yaml), which is
itself emitted from the server's handler code, so the SDK can never drift from the API.

Requires Go 1.23+.

## Install

```bash
go get github.com/Stripy-Horse/stripyhorse-go
```

## Setup

```go
import (
	"context"

	stripyhorse "github.com/Stripy-Horse/stripyhorse-go"
)

client := stripyhorse.NewAPIClient(stripyhorse.NewConfiguration())
ctx := context.WithValue(context.Background(),
	stripyhorse.ContextAccessToken, "sh_live_YOUR_KEY")
```

Every call takes that `ctx`; the key rides on it as a bearer token.

## Render ZPL to PNG

```go
body := *stripyhorse.NewRenderInputBody("^XA^FO50,50^A0N,45,45^FDHello^FS^XZ")
body.SetPreset("4x6")

out, _, err := client.RenderAPI.RenderZpl(ctx).RenderInputBody(body).Execute()
if err != nil {
	return err
}
png, err := base64.StdEncoding.DecodeString(out.Labels[0].Png)
if err != nil {
	return err
}
os.WriteFile("label.png", png, 0o644)
```

## Convert a PDF (or PNG/GIF/JPEG) to ZPL

```go
f, err := os.Open("shipping-label.pdf")
if err != nil {
	return err
}
defer f.Close()

result, _, err := client.ConvertAPI.ConvertDocument(ctx).File(f).Preset("4x6").Execute()
if err != nil {
	return err
}
for _, page := range result.Pages {
	sendToPrinter(page.Zpl)
}
```

## Design a label in HTML, get ZPL

```go
html := *stripyhorse.NewHtmlInputBody(
	`<div style="position:absolute;left:40px;top:40px;font-size:50px">Hello</div>`)
html.SetPreset("4x6")

out, _, err := client.ConvertAPI.ConvertHtml(ctx).HtmlInputBody(html).Execute()
if err != nil {
	return err
}
fmt.Println(out.Zpl)
```

## Test label printing in CI with a virtual printer

```go
create := *stripyhorse.NewCreatePrinterInputBody("ci-run-42")
create.SetPreset("4x6")

printer, _, err := client.SimulatorAPI.CreatePrinter(ctx).
	CreatePrinterInputBody(create).Execute()
if err != nil {
	return err
}

// Point the system under test at the printer, exactly like hardware:
addr := fmt.Sprintf("%s:%d", printer.Tcp.Host, printer.Tcp.Port)

// ... run your fulfillment code against addr ...

// Then assert on what it printed:
jobs, _, err := client.SimulatorAPI.ListJobs(ctx, printer.Id).Execute()
if err != nil {
	return err
}
if len(jobs.Jobs) != 1 {
	t.Fatalf("printed %d jobs, want 1", len(jobs.Jobs))
}

// Reproduce a paper-out jam and watch jobs hold in the buffer:
faults := *stripyhorse.NewFaults()
faults.SetPaperOut(true)
_, _, err = client.SimulatorAPI.SetPrinterFaults(ctx, printer.Id).Faults(faults).Execute()
```

## Errors

Every call returns `(value, *http.Response, error)`. An API error is a
`*stripyhorse.GenericOpenAPIError`; `err.Body()` carries the JSON error envelope
and `err.Model()` the decoded one. HTTP 429 includes a `Retry-After` header.

## Regenerating

Every file here is generated from the [OpenAPI spec](https://stripyhorse.io/openapi.yaml),
which is emitted from the server's own handler code. Hand edits are overwritten by the
next spec change, so report a problem with the SDK as a problem with the API:
[stripyhorse.io/contact](https://stripyhorse.io/contact).
