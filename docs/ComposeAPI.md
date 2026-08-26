# \ComposeAPI

All URIs are relative to *https://api.stripyhorse.io*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ComposeLabel**](ComposeAPI.md#ComposeLabel) | **Post** /v1/labels/compose | Compose ZPL from typed JSON elements



## ComposeLabel

> ComposeOutputBody ComposeLabel(ctx).ComposeInputBody(composeInputBody).Execute()

Compose ZPL from typed JSON elements



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
	composeInputBody := *openapiclient.NewComposeInputBody([]openapiclient.Element{*openapiclient.NewElement("Type_example")}) // ComposeInputBody | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ComposeAPI.ComposeLabel(context.Background()).ComposeInputBody(composeInputBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ComposeAPI.ComposeLabel``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ComposeLabel`: ComposeOutputBody
	fmt.Fprintf(os.Stdout, "Response from `ComposeAPI.ComposeLabel`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiComposeLabelRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **composeInputBody** | [**ComposeInputBody**](ComposeInputBody.md) |  | 

### Return type

[**ComposeOutputBody**](ComposeOutputBody.md)

### Authorization

[headerKey](../README.md#headerKey), [bearerKey](../README.md#bearerKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

