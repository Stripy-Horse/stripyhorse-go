# \RenderAPI

All URIs are relative to *https://api.stripyhorse.io*

Method | HTTP request | Description
------------- | ------------- | -------------
[**PreflightLabel**](RenderAPI.md#PreflightLabel) | **Post** /v1/preflight | Grade a label&#39;s barcodes before they ship
[**RenderZpl**](RenderAPI.md#RenderZpl) | **Post** /v1/render | Render ZPL to PNG images
[**RenderZplPng**](RenderAPI.md#RenderZplPng) | **Post** /v1/render.png | Render ZPL and return the first label as a raw PNG



## PreflightLabel

> PreflightOutputBody PreflightLabel(ctx).PreflightInputBody(preflightInputBody).Execute()

Grade a label's barcodes before they ship



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
	preflightInputBody := *openapiclient.NewPreflightInputBody("Zpl_example") // PreflightInputBody | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RenderAPI.PreflightLabel(context.Background()).PreflightInputBody(preflightInputBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RenderAPI.PreflightLabel``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PreflightLabel`: PreflightOutputBody
	fmt.Fprintf(os.Stdout, "Response from `RenderAPI.PreflightLabel`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiPreflightLabelRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **preflightInputBody** | [**PreflightInputBody**](PreflightInputBody.md) |  | 

### Return type

[**PreflightOutputBody**](PreflightOutputBody.md)

### Authorization

[headerKey](../README.md#headerKey), [bearerKey](../README.md#bearerKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RenderZpl

> RenderOutputBody RenderZpl(ctx).RenderInputBody(renderInputBody).Execute()

Render ZPL to PNG images



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
	renderInputBody := *openapiclient.NewRenderInputBody("Zpl_example") // RenderInputBody | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RenderAPI.RenderZpl(context.Background()).RenderInputBody(renderInputBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RenderAPI.RenderZpl``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RenderZpl`: RenderOutputBody
	fmt.Fprintf(os.Stdout, "Response from `RenderAPI.RenderZpl`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiRenderZplRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **renderInputBody** | [**RenderInputBody**](RenderInputBody.md) |  | 

### Return type

[**RenderOutputBody**](RenderOutputBody.md)

### Authorization

[headerKey](../README.md#headerKey), [bearerKey](../README.md#bearerKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RenderZplPng

> string RenderZplPng(ctx).RenderInputBody(renderInputBody).Execute()

Render ZPL and return the first label as a raw PNG



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
	renderInputBody := *openapiclient.NewRenderInputBody("Zpl_example") // RenderInputBody | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RenderAPI.RenderZplPng(context.Background()).RenderInputBody(renderInputBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RenderAPI.RenderZplPng``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RenderZplPng`: string
	fmt.Fprintf(os.Stdout, "Response from `RenderAPI.RenderZplPng`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiRenderZplPngRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **renderInputBody** | [**RenderInputBody**](RenderInputBody.md) |  | 

### Return type

**string**

### Authorization

[headerKey](../README.md#headerKey), [bearerKey](../README.md#bearerKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

