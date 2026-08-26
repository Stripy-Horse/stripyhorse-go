# ComposeOutputBody

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Labels** | Pointer to [**[]RenderedLabel**](RenderedLabel.md) | Rendered previews when preview&#x3D;true | [optional] 
**Warnings** | **[]string** |  | 
**Zpl** | **string** |  | 

## Methods

### NewComposeOutputBody

`func NewComposeOutputBody(warnings []string, zpl string, ) *ComposeOutputBody`

NewComposeOutputBody instantiates a new ComposeOutputBody object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewComposeOutputBodyWithDefaults

`func NewComposeOutputBodyWithDefaults() *ComposeOutputBody`

NewComposeOutputBodyWithDefaults instantiates a new ComposeOutputBody object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetLabels

`func (o *ComposeOutputBody) GetLabels() []RenderedLabel`

GetLabels returns the Labels field if non-nil, zero value otherwise.

### GetLabelsOk

`func (o *ComposeOutputBody) GetLabelsOk() (*[]RenderedLabel, bool)`

GetLabelsOk returns a tuple with the Labels field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLabels

`func (o *ComposeOutputBody) SetLabels(v []RenderedLabel)`

SetLabels sets Labels field to given value.

### HasLabels

`func (o *ComposeOutputBody) HasLabels() bool`

HasLabels returns a boolean if a field has been set.

### SetLabelsNil

`func (o *ComposeOutputBody) SetLabelsNil(b bool)`

 SetLabelsNil sets the value for Labels to be an explicit nil

### UnsetLabels
`func (o *ComposeOutputBody) UnsetLabels()`

UnsetLabels ensures that no value is present for Labels, not even an explicit nil
### GetWarnings

`func (o *ComposeOutputBody) GetWarnings() []string`

GetWarnings returns the Warnings field if non-nil, zero value otherwise.

### GetWarningsOk

`func (o *ComposeOutputBody) GetWarningsOk() (*[]string, bool)`

GetWarningsOk returns a tuple with the Warnings field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWarnings

`func (o *ComposeOutputBody) SetWarnings(v []string)`

SetWarnings sets Warnings field to given value.


### SetWarningsNil

`func (o *ComposeOutputBody) SetWarningsNil(b bool)`

 SetWarningsNil sets the value for Warnings to be an explicit nil

### UnsetWarnings
`func (o *ComposeOutputBody) UnsetWarnings()`

UnsetWarnings ensures that no value is present for Warnings, not even an explicit nil
### GetZpl

`func (o *ComposeOutputBody) GetZpl() string`

GetZpl returns the Zpl field if non-nil, zero value otherwise.

### GetZplOk

`func (o *ComposeOutputBody) GetZplOk() (*string, bool)`

GetZplOk returns a tuple with the Zpl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetZpl

`func (o *ComposeOutputBody) SetZpl(v string)`

SetZpl sets Zpl field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


