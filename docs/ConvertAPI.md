# \ConvertAPI

All URIs are relative to *https://api.stripyhorse.io*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ConvertBatch**](ConvertAPI.md#ConvertBatch) | **Post** /v1/convert/batch | Convert many documents in one request, results streamed
[**ConvertDocument**](ConvertAPI.md#ConvertDocument) | **Post** /v1/convert | Convert a PDF or image to ZPL
[**ConvertHtml**](ConvertAPI.md#ConvertHtml) | **Post** /v1/convert/html | Convert an HTML label design to ZPL
[**ConvertZplToHtml**](ConvertAPI.md#ConvertZplToHtml) | **Post** /v1/convert/zpl-html | Decompile ZPL into editable HTML
[**RasterizeUnicode**](ConvertAPI.md#RasterizeUnicode) | **Post** /v1/unicode | Make Unicode ZPL printable on any Zebra
[**StampZpl**](ConvertAPI.md#StampZpl) | **Post** /v1/stamp | Stamp an image onto ZPL labels
[**VoidZpl**](ConvertAPI.md#VoidZpl) | **Post** /v1/void | Stamp ZPL as void / do-not-ship



## ConvertBatch

> ConvertBatch(ctx).Files(files).BarcodeAware(barcodeAware).Compression(compression).Dpmm(dpmm).HeightMm(heightMm).Preset(preset).Rotation(rotation).Scale(scale).Threshold(threshold).WidthMm(widthMm).Execute()

Convert many documents in one request, results streamed



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/Stripy-Horse/stripyhorse-go"
)

func main() {
	files := []*os.File{"TODO"} // []*os.File | 
	barcodeAware := true // bool |  (optional)
	compression := "compression_example" // string |  (optional)
	dpmm := int64(789) // int64 |  (optional)
	heightMm := float64(1.2) // float64 |  (optional)
	preset := "preset_example" // string |  (optional)
	rotation := int64(789) // int64 |  (optional)
	scale := "scale_example" // string |  (optional)
	threshold := int64(789) // int64 |  (optional)
	widthMm := float64(1.2) // float64 |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.ConvertAPI.ConvertBatch(context.Background()).Files(files).BarcodeAware(barcodeAware).Compression(compression).Dpmm(dpmm).HeightMm(heightMm).Preset(preset).Rotation(rotation).Scale(scale).Threshold(threshold).WidthMm(widthMm).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ConvertAPI.ConvertBatch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiConvertBatchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **files** | **[]*os.File** |  | 
 **barcodeAware** | **bool** |  | 
 **compression** | **string** |  | 
 **dpmm** | **int64** |  | 
 **heightMm** | **float64** |  | 
 **preset** | **string** |  | 
 **rotation** | **int64** |  | 
 **scale** | **string** |  | 
 **threshold** | **int64** |  | 
 **widthMm** | **float64** |  | 

### Return type

 (empty response body)

### Authorization

[headerKey](../README.md#headerKey), [bearerKey](../README.md#bearerKey)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ConvertDocument

> ConvertOutputBody ConvertDocument(ctx).File(file).BarcodeAware(barcodeAware).Compression(compression).Dpmm(dpmm).HeightMm(heightMm).Preset(preset).Rotation(rotation).Scale(scale).Threshold(threshold).WidthMm(widthMm).Execute()

Convert a PDF or image to ZPL



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/Stripy-Horse/stripyhorse-go"
)

func main() {
	file := os.NewFile(1234, "some_file") // *os.File | PDF, PNG, GIF or JPEG
	barcodeAware := true // bool | EXPERIMENTAL: re-emit decodable barcodes as native ^BC/^BQ fields, verified by a decode round trip with automatic fallback to plain rasterization (optional)
	compression := "compression_example" // string | acs (default) or z64 (zlib+base64, smaller payloads) (optional)
	dpmm := int64(789) // int64 |  (optional)
	heightMm := float64(1.2) // float64 |  (optional)
	preset := "preset_example" // string |  (optional)
	rotation := int64(789) // int64 |  (optional)
	scale := "scale_example" // string | cover (fit), fill (stretch) or none (optional)
	threshold := int64(789) // int64 |  (optional)
	widthMm := float64(1.2) // float64 |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ConvertAPI.ConvertDocument(context.Background()).File(file).BarcodeAware(barcodeAware).Compression(compression).Dpmm(dpmm).HeightMm(heightMm).Preset(preset).Rotation(rotation).Scale(scale).Threshold(threshold).WidthMm(widthMm).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ConvertAPI.ConvertDocument``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ConvertDocument`: ConvertOutputBody
	fmt.Fprintf(os.Stdout, "Response from `ConvertAPI.ConvertDocument`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiConvertDocumentRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **file** | ***os.File** | PDF, PNG, GIF or JPEG | 
 **barcodeAware** | **bool** | EXPERIMENTAL: re-emit decodable barcodes as native ^BC/^BQ fields, verified by a decode round trip with automatic fallback to plain rasterization | 
 **compression** | **string** | acs (default) or z64 (zlib+base64, smaller payloads) | 
 **dpmm** | **int64** |  | 
 **heightMm** | **float64** |  | 
 **preset** | **string** |  | 
 **rotation** | **int64** |  | 
 **scale** | **string** | cover (fit), fill (stretch) or none | 
 **threshold** | **int64** |  | 
 **widthMm** | **float64** |  | 

### Return type

[**ConvertOutputBody**](ConvertOutputBody.md)

### Authorization

[headerKey](../README.md#headerKey), [bearerKey](../README.md#bearerKey)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ConvertHtml

> HtmlOutputBody ConvertHtml(ctx).HtmlInputBody(htmlInputBody).Execute()

Convert an HTML label design to ZPL



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/Stripy-Horse/stripyhorse-go"
)

func main() {
	htmlInputBody := *openapiclient.NewHtmlInputBody("Html_example") // HtmlInputBody | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ConvertAPI.ConvertHtml(context.Background()).HtmlInputBody(htmlInputBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ConvertAPI.ConvertHtml``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ConvertHtml`: HtmlOutputBody
	fmt.Fprintf(os.Stdout, "Response from `ConvertAPI.ConvertHtml`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiConvertHtmlRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **htmlInputBody** | [**HtmlInputBody**](HtmlInputBody.md) |  | 

### Return type

[**HtmlOutputBody**](HtmlOutputBody.md)

### Authorization

[headerKey](../README.md#headerKey), [bearerKey](../README.md#bearerKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ConvertZplToHtml

> ZplHTMLOutputBody ConvertZplToHtml(ctx).ZplHTMLInputBody(zplHTMLInputBody).Execute()

Decompile ZPL into editable HTML



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/Stripy-Horse/stripyhorse-go"
)

func main() {
	zplHTMLInputBody := *openapiclient.NewZplHTMLInputBody("Zpl_example") // ZplHTMLInputBody | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ConvertAPI.ConvertZplToHtml(context.Background()).ZplHTMLInputBody(zplHTMLInputBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ConvertAPI.ConvertZplToHtml``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ConvertZplToHtml`: ZplHTMLOutputBody
	fmt.Fprintf(os.Stdout, "Response from `ConvertAPI.ConvertZplToHtml`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiConvertZplToHtmlRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **zplHTMLInputBody** | [**ZplHTMLInputBody**](ZplHTMLInputBody.md) |  | 

### Return type

[**ZplHTMLOutputBody**](ZplHTMLOutputBody.md)

### Authorization

[headerKey](../README.md#headerKey), [bearerKey](../README.md#bearerKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RasterizeUnicode

> UnicodeOutputBody RasterizeUnicode(ctx).UnicodeInputBody(unicodeInputBody).Execute()

Make Unicode ZPL printable on any Zebra



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/Stripy-Horse/stripyhorse-go"
)

func main() {
	unicodeInputBody := *openapiclient.NewUnicodeInputBody("Zpl_example") // UnicodeInputBody | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ConvertAPI.RasterizeUnicode(context.Background()).UnicodeInputBody(unicodeInputBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ConvertAPI.RasterizeUnicode``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RasterizeUnicode`: UnicodeOutputBody
	fmt.Fprintf(os.Stdout, "Response from `ConvertAPI.RasterizeUnicode`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiRasterizeUnicodeRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **unicodeInputBody** | [**UnicodeInputBody**](UnicodeInputBody.md) |  | 

### Return type

[**UnicodeOutputBody**](UnicodeOutputBody.md)

### Authorization

[headerKey](../README.md#headerKey), [bearerKey](../README.md#bearerKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## StampZpl

> StampOutputBody StampZpl(ctx).StampInputBody(stampInputBody).Execute()

Stamp an image onto ZPL labels



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/Stripy-Horse/stripyhorse-go"
)

func main() {
	stampInputBody := *openapiclient.NewStampInputBody("Image_example", "Zpl_example") // StampInputBody | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ConvertAPI.StampZpl(context.Background()).StampInputBody(stampInputBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ConvertAPI.StampZpl``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `StampZpl`: StampOutputBody
	fmt.Fprintf(os.Stdout, "Response from `ConvertAPI.StampZpl`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiStampZplRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **stampInputBody** | [**StampInputBody**](StampInputBody.md) |  | 

### Return type

[**StampOutputBody**](StampOutputBody.md)

### Authorization

[headerKey](../README.md#headerKey), [bearerKey](../README.md#bearerKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## VoidZpl

> VoidOutputBody VoidZpl(ctx).VoidInputBody(voidInputBody).Execute()

Stamp ZPL as void / do-not-ship



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/Stripy-Horse/stripyhorse-go"
)

func main() {
	voidInputBody := *openapiclient.NewVoidInputBody("Zpl_example") // VoidInputBody | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ConvertAPI.VoidZpl(context.Background()).VoidInputBody(voidInputBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ConvertAPI.VoidZpl``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `VoidZpl`: VoidOutputBody
	fmt.Fprintf(os.Stdout, "Response from `ConvertAPI.VoidZpl`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiVoidZplRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **voidInputBody** | [**VoidInputBody**](VoidInputBody.md) |  | 

### Return type

[**VoidOutputBody**](VoidOutputBody.md)

### Authorization

[headerKey](../README.md#headerKey), [bearerKey](../README.md#bearerKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

