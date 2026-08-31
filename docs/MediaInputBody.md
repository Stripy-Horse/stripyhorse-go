# MediaInputBody

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Labels** | Pointer to **int64** | Labels on the roll; 0 for an endless roll | [optional] 
**RibbonMetres** | Pointer to **float64** | Ribbon on the spool in metres; 0 for endless, which is also what direct thermal looks like | [optional] 

## Methods

### NewMediaInputBody

`func NewMediaInputBody() *MediaInputBody`

NewMediaInputBody instantiates a new MediaInputBody object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewMediaInputBodyWithDefaults

`func NewMediaInputBodyWithDefaults() *MediaInputBody`

NewMediaInputBodyWithDefaults instantiates a new MediaInputBody object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetLabels

`func (o *MediaInputBody) GetLabels() int64`

GetLabels returns the Labels field if non-nil, zero value otherwise.

### GetLabelsOk

`func (o *MediaInputBody) GetLabelsOk() (*int64, bool)`

GetLabelsOk returns a tuple with the Labels field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLabels

`func (o *MediaInputBody) SetLabels(v int64)`

SetLabels sets Labels field to given value.

### HasLabels

`func (o *MediaInputBody) HasLabels() bool`

HasLabels returns a boolean if a field has been set.

### GetRibbonMetres

`func (o *MediaInputBody) GetRibbonMetres() float64`

GetRibbonMetres returns the RibbonMetres field if non-nil, zero value otherwise.

### GetRibbonMetresOk

`func (o *MediaInputBody) GetRibbonMetresOk() (*float64, bool)`

GetRibbonMetresOk returns a tuple with the RibbonMetres field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRibbonMetres

`func (o *MediaInputBody) SetRibbonMetres(v float64)`

SetRibbonMetres sets RibbonMetres field to given value.

### HasRibbonMetres

`func (o *MediaInputBody) HasRibbonMetres() bool`

HasRibbonMetres returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


