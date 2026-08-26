# \PrintersAPI

All URIs are relative to *https://api.stripyhorse.io*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ParseHostStatus**](PrintersAPI.md#ParseHostStatus) | **Post** /v1/host-status/parse | Decode a Zebra ~HS host status response



## ParseHostStatus

> HostStatusOutputBody ParseHostStatus(ctx).HostStatusInputBody(hostStatusInputBody).Execute()

Decode a Zebra ~HS host status response



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
	hostStatusInputBody := *openapiclient.NewHostStatusInputBody("Response_example") // HostStatusInputBody | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PrintersAPI.ParseHostStatus(context.Background()).HostStatusInputBody(hostStatusInputBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PrintersAPI.ParseHostStatus``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ParseHostStatus`: HostStatusOutputBody
	fmt.Fprintf(os.Stdout, "Response from `PrintersAPI.ParseHostStatus`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiParseHostStatusRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **hostStatusInputBody** | [**HostStatusInputBody**](HostStatusInputBody.md) |  | 

### Return type

[**HostStatusOutputBody**](HostStatusOutputBody.md)

### Authorization

[headerKey](../README.md#headerKey), [bearerKey](../README.md#bearerKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, application/problem+json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

