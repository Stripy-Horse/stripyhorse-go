# \SimulatorAPI

All URIs are relative to *https://api.stripyhorse.io*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ClearJobs**](SimulatorAPI.md#ClearJobs) | **Delete** /v1/printers/{printerId}/jobs | Delete all captured jobs
[**CreatePrinter**](SimulatorAPI.md#CreatePrinter) | **Post** /v1/printers | Create a virtual printer
[**DeletePrinter**](SimulatorAPI.md#DeletePrinter) | **Delete** /v1/printers/{printerId} | Delete a printer and its captured jobs
[**GetJob**](SimulatorAPI.md#GetJob) | **Get** /v1/printers/{printerId}/jobs/{jobId} | Get one job including its raw ZPL
[**GetJobLabel**](SimulatorAPI.md#GetJobLabel) | **Get** /v1/printers/{printerId}/jobs/{jobId}/labels/{index}.png | Get one rendered label as a PNG
[**GetPrinter**](SimulatorAPI.md#GetPrinter) | **Get** /v1/printers/{printerId} | Get a printer with live state
[**ListJobs**](SimulatorAPI.md#ListJobs) | **Get** /v1/printers/{printerId}/jobs | List captured jobs, newest first
[**ListPrinters**](SimulatorAPI.md#ListPrinters) | **Get** /v1/printers | List your printers
[**ResetPrinter**](SimulatorAPI.md#ResetPrinter) | **Post** /v1/printers/{printerId}/reset | Clear all faults and flush held jobs
[**SetPrinterFaults**](SimulatorAPI.md#SetPrinterFaults) | **Post** /v1/printers/{printerId}/faults | Inject or clear fault conditions
[**UpdatePrinter**](SimulatorAPI.md#UpdatePrinter) | **Patch** /v1/printers/{printerId} | Rename a printer or set its webhook URL



## ClearJobs

> ClearJobs(ctx, printerId).Execute()

Delete all captured jobs

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
	printerId := "printerId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.SimulatorAPI.ClearJobs(context.Background(), printerId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SimulatorAPI.ClearJobs``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**printerId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiClearJobsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

 (empty response body)

### Authorization

[headerKey](../README.md#headerKey), [bearerKey](../README.md#bearerKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreatePrinter

> PrinterBody CreatePrinter(ctx).CreatePrinterInputBody(createPrinterInputBody).Execute()

Create a virtual printer



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
	createPrinterInputBody := *openapiclient.NewCreatePrinterInputBody("Name_example") // CreatePrinterInputBody | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SimulatorAPI.CreatePrinter(context.Background()).CreatePrinterInputBody(createPrinterInputBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SimulatorAPI.CreatePrinter``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreatePrinter`: PrinterBody
	fmt.Fprintf(os.Stdout, "Response from `SimulatorAPI.CreatePrinter`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreatePrinterRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createPrinterInputBody** | [**CreatePrinterInputBody**](CreatePrinterInputBody.md) |  | 

### Return type

[**PrinterBody**](PrinterBody.md)

### Authorization

[headerKey](../README.md#headerKey), [bearerKey](../README.md#bearerKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeletePrinter

> DeletePrinter(ctx, printerId).Execute()

Delete a printer and its captured jobs

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
	printerId := "printerId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.SimulatorAPI.DeletePrinter(context.Background(), printerId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SimulatorAPI.DeletePrinter``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**printerId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeletePrinterRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

 (empty response body)

### Authorization

[headerKey](../README.md#headerKey), [bearerKey](../README.md#bearerKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetJob

> JobOutputBody GetJob(ctx, printerId, jobId).Execute()

Get one job including its raw ZPL

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
	printerId := "printerId_example" // string | 
	jobId := int64(789) // int64 | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SimulatorAPI.GetJob(context.Background(), printerId, jobId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SimulatorAPI.GetJob``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetJob`: JobOutputBody
	fmt.Fprintf(os.Stdout, "Response from `SimulatorAPI.GetJob`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**printerId** | **string** |  | 
**jobId** | **int64** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetJobRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**JobOutputBody**](JobOutputBody.md)

### Authorization

[headerKey](../README.md#headerKey), [bearerKey](../README.md#bearerKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetJobLabel

> string GetJobLabel(ctx, printerId, jobId, index).Execute()

Get one rendered label as a PNG

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
	printerId := "printerId_example" // string | 
	jobId := int64(789) // int64 | 
	index := int64(789) // int64 | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SimulatorAPI.GetJobLabel(context.Background(), printerId, jobId, index).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SimulatorAPI.GetJobLabel``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetJobLabel`: string
	fmt.Fprintf(os.Stdout, "Response from `SimulatorAPI.GetJobLabel`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**printerId** | **string** |  | 
**jobId** | **int64** |  | 
**index** | **int64** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetJobLabelRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




### Return type

**string**

### Authorization

[headerKey](../README.md#headerKey), [bearerKey](../README.md#bearerKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetPrinter

> PrinterBody GetPrinter(ctx, printerId).Execute()

Get a printer with live state

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
	printerId := "printerId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SimulatorAPI.GetPrinter(context.Background(), printerId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SimulatorAPI.GetPrinter``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetPrinter`: PrinterBody
	fmt.Fprintf(os.Stdout, "Response from `SimulatorAPI.GetPrinter`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**printerId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetPrinterRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**PrinterBody**](PrinterBody.md)

### Authorization

[headerKey](../README.md#headerKey), [bearerKey](../README.md#bearerKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListJobs

> ListJobsOutputBody ListJobs(ctx, printerId).Limit(limit).Before(before).Execute()

List captured jobs, newest first



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
	printerId := "printerId_example" // string | 
	limit := int64(789) // int64 |  (optional) (default to 50)
	before := int64(789) // int64 | Return jobs with id lower than this cursor (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SimulatorAPI.ListJobs(context.Background(), printerId).Limit(limit).Before(before).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SimulatorAPI.ListJobs``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListJobs`: ListJobsOutputBody
	fmt.Fprintf(os.Stdout, "Response from `SimulatorAPI.ListJobs`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**printerId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListJobsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **limit** | **int64** |  | [default to 50]
 **before** | **int64** | Return jobs with id lower than this cursor | 

### Return type

[**ListJobsOutputBody**](ListJobsOutputBody.md)

### Authorization

[headerKey](../README.md#headerKey), [bearerKey](../README.md#bearerKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListPrinters

> ListPrintersOutputBody ListPrinters(ctx).Execute()

List your printers

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SimulatorAPI.ListPrinters(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SimulatorAPI.ListPrinters``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListPrinters`: ListPrintersOutputBody
	fmt.Fprintf(os.Stdout, "Response from `SimulatorAPI.ListPrinters`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiListPrintersRequest struct via the builder pattern


### Return type

[**ListPrintersOutputBody**](ListPrintersOutputBody.md)

### Authorization

[headerKey](../README.md#headerKey), [bearerKey](../README.md#bearerKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ResetPrinter

> StateOutputBody ResetPrinter(ctx, printerId).Execute()

Clear all faults and flush held jobs

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
	printerId := "printerId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SimulatorAPI.ResetPrinter(context.Background(), printerId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SimulatorAPI.ResetPrinter``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ResetPrinter`: StateOutputBody
	fmt.Fprintf(os.Stdout, "Response from `SimulatorAPI.ResetPrinter`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**printerId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiResetPrinterRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**StateOutputBody**](StateOutputBody.md)

### Authorization

[headerKey](../README.md#headerKey), [bearerKey](../README.md#bearerKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SetPrinterFaults

> StateOutputBody SetPrinterFaults(ctx, printerId).Faults(faults).Execute()

Inject or clear fault conditions



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
	printerId := "printerId_example" // string | 
	faults := *openapiclient.NewFaults() // Faults | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SimulatorAPI.SetPrinterFaults(context.Background(), printerId).Faults(faults).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SimulatorAPI.SetPrinterFaults``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SetPrinterFaults`: StateOutputBody
	fmt.Fprintf(os.Stdout, "Response from `SimulatorAPI.SetPrinterFaults`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**printerId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiSetPrinterFaultsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **faults** | [**Faults**](Faults.md) |  | 

### Return type

[**StateOutputBody**](StateOutputBody.md)

### Authorization

[headerKey](../README.md#headerKey), [bearerKey](../README.md#bearerKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdatePrinter

> PrinterBody UpdatePrinter(ctx, printerId).UpdatePrinterInputBody(updatePrinterInputBody).Execute()

Rename a printer or set its webhook URL

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
	printerId := "printerId_example" // string | 
	updatePrinterInputBody := *openapiclient.NewUpdatePrinterInputBody() // UpdatePrinterInputBody | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SimulatorAPI.UpdatePrinter(context.Background(), printerId).UpdatePrinterInputBody(updatePrinterInputBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SimulatorAPI.UpdatePrinter``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdatePrinter`: PrinterBody
	fmt.Fprintf(os.Stdout, "Response from `SimulatorAPI.UpdatePrinter`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**printerId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdatePrinterRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **updatePrinterInputBody** | [**UpdatePrinterInputBody**](UpdatePrinterInputBody.md) |  | 

### Return type

[**PrinterBody**](PrinterBody.md)

### Authorization

[headerKey](../README.md#headerKey), [bearerKey](../README.md#bearerKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

