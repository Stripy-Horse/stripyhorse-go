# RenderInputBody

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Dpmm** | Pointer to **int64** | Print density in dots/mm (152/203/300/600 dpi); default 8 | [optional] 
**HeightMm** | Pointer to **float64** |  | [optional] 
**Preset** | Pointer to **string** | Named label size in inches; alternative to widthMm/heightMm | [optional] 
**Rotation** | Pointer to **int64** |  | [optional] 
**WidthMm** | Pointer to **float64** |  | [optional] 
**Zpl** | **string** |  | 

## Methods

### NewRenderInputBody

`func NewRenderInputBody(zpl string, ) *RenderInputBody`

NewRenderInputBody instantiates a new RenderInputBody object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRenderInputBodyWithDefaults

`func NewRenderInputBodyWithDefaults() *RenderInputBody`

NewRenderInputBodyWithDefaults instantiates a new RenderInputBody object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDpmm

`func (o *RenderInputBody) GetDpmm() int64`

GetDpmm returns the Dpmm field if non-nil, zero value otherwise.

### GetDpmmOk

`func (o *RenderInputBody) GetDpmmOk() (*int64, bool)`

GetDpmmOk returns a tuple with the Dpmm field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDpmm

`func (o *RenderInputBody) SetDpmm(v int64)`

SetDpmm sets Dpmm field to given value.

### HasDpmm

`func (o *RenderInputBody) HasDpmm() bool`

HasDpmm returns a boolean if a field has been set.

### GetHeightMm

`func (o *RenderInputBody) GetHeightMm() float64`

GetHeightMm returns the HeightMm field if non-nil, zero value otherwise.

### GetHeightMmOk

`func (o *RenderInputBody) GetHeightMmOk() (*float64, bool)`

GetHeightMmOk returns a tuple with the HeightMm field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHeightMm

`func (o *RenderInputBody) SetHeightMm(v float64)`

SetHeightMm sets HeightMm field to given value.

### HasHeightMm

`func (o *RenderInputBody) HasHeightMm() bool`

HasHeightMm returns a boolean if a field has been set.

### GetPreset

`func (o *RenderInputBody) GetPreset() string`

GetPreset returns the Preset field if non-nil, zero value otherwise.

### GetPresetOk

`func (o *RenderInputBody) GetPresetOk() (*string, bool)`

GetPresetOk returns a tuple with the Preset field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPreset

`func (o *RenderInputBody) SetPreset(v string)`

SetPreset sets Preset field to given value.

### HasPreset

`func (o *RenderInputBody) HasPreset() bool`

HasPreset returns a boolean if a field has been set.

### GetRotation

`func (o *RenderInputBody) GetRotation() int64`

GetRotation returns the Rotation field if non-nil, zero value otherwise.

### GetRotationOk

`func (o *RenderInputBody) GetRotationOk() (*int64, bool)`

GetRotationOk returns a tuple with the Rotation field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRotation

`func (o *RenderInputBody) SetRotation(v int64)`

SetRotation sets Rotation field to given value.

### HasRotation

`func (o *RenderInputBody) HasRotation() bool`

HasRotation returns a boolean if a field has been set.

### GetWidthMm

`func (o *RenderInputBody) GetWidthMm() float64`

GetWidthMm returns the WidthMm field if non-nil, zero value otherwise.

### GetWidthMmOk

`func (o *RenderInputBody) GetWidthMmOk() (*float64, bool)`

GetWidthMmOk returns a tuple with the WidthMm field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWidthMm

`func (o *RenderInputBody) SetWidthMm(v float64)`

SetWidthMm sets WidthMm field to given value.

### HasWidthMm

`func (o *RenderInputBody) HasWidthMm() bool`

HasWidthMm returns a boolean if a field has been set.

### GetZpl

`func (o *RenderInputBody) GetZpl() string`

GetZpl returns the Zpl field if non-nil, zero value otherwise.

### GetZplOk

`func (o *RenderInputBody) GetZplOk() (*string, bool)`

GetZplOk returns a tuple with the Zpl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetZpl

`func (o *RenderInputBody) SetZpl(v string)`

SetZpl sets Zpl field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


