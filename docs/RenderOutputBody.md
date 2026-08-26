# RenderOutputBody

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**LabelCount** | **int64** |  | 
**Labels** | [**[]RenderedLabel**](RenderedLabel.md) |  | 

## Methods

### NewRenderOutputBody

`func NewRenderOutputBody(labelCount int64, labels []RenderedLabel, ) *RenderOutputBody`

NewRenderOutputBody instantiates a new RenderOutputBody object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRenderOutputBodyWithDefaults

`func NewRenderOutputBodyWithDefaults() *RenderOutputBody`

NewRenderOutputBodyWithDefaults instantiates a new RenderOutputBody object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetLabelCount

`func (o *RenderOutputBody) GetLabelCount() int64`

GetLabelCount returns the LabelCount field if non-nil, zero value otherwise.

### GetLabelCountOk

`func (o *RenderOutputBody) GetLabelCountOk() (*int64, bool)`

GetLabelCountOk returns a tuple with the LabelCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLabelCount

`func (o *RenderOutputBody) SetLabelCount(v int64)`

SetLabelCount sets LabelCount field to given value.


### GetLabels

`func (o *RenderOutputBody) GetLabels() []RenderedLabel`

GetLabels returns the Labels field if non-nil, zero value otherwise.

### GetLabelsOk

`func (o *RenderOutputBody) GetLabelsOk() (*[]RenderedLabel, bool)`

GetLabelsOk returns a tuple with the Labels field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLabels

`func (o *RenderOutputBody) SetLabels(v []RenderedLabel)`

SetLabels sets Labels field to given value.


### SetLabelsNil

`func (o *RenderOutputBody) SetLabelsNil(b bool)`

 SetLabelsNil sets the value for Labels to be an explicit nil

### UnsetLabels
`func (o *RenderOutputBody) UnsetLabels()`

UnsetLabels ensures that no value is present for Labels, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


