# JobOutputBody

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Labels** | **[]string** | URLs of the rendered label PNGs | 
**Zpl** | **string** | The raw ZPL as received | 

## Methods

### NewJobOutputBody

`func NewJobOutputBody(labels []string, zpl string, ) *JobOutputBody`

NewJobOutputBody instantiates a new JobOutputBody object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewJobOutputBodyWithDefaults

`func NewJobOutputBodyWithDefaults() *JobOutputBody`

NewJobOutputBodyWithDefaults instantiates a new JobOutputBody object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetLabels

`func (o *JobOutputBody) GetLabels() []string`

GetLabels returns the Labels field if non-nil, zero value otherwise.

### GetLabelsOk

`func (o *JobOutputBody) GetLabelsOk() (*[]string, bool)`

GetLabelsOk returns a tuple with the Labels field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLabels

`func (o *JobOutputBody) SetLabels(v []string)`

SetLabels sets Labels field to given value.


### SetLabelsNil

`func (o *JobOutputBody) SetLabelsNil(b bool)`

 SetLabelsNil sets the value for Labels to be an explicit nil

### UnsetLabels
`func (o *JobOutputBody) UnsetLabels()`

UnsetLabels ensures that no value is present for Labels, not even an explicit nil
### GetZpl

`func (o *JobOutputBody) GetZpl() string`

GetZpl returns the Zpl field if non-nil, zero value otherwise.

### GetZplOk

`func (o *JobOutputBody) GetZplOk() (*string, bool)`

GetZplOk returns a tuple with the Zpl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetZpl

`func (o *JobOutputBody) SetZpl(v string)`

SetZpl sets Zpl field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


