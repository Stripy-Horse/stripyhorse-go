# VoidInputBody

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Dpmm** | Pointer to **int64** |  | [optional] 
**HeightMm** | Pointer to **float64** |  | [optional] 
**Preset** | Pointer to **string** | Named label size in inches; alternative to widthMm/heightMm | [optional] 
**Stamp** | Pointer to **string** | Attribution stamp, e.g. VOID: bfaerber | [optional] 
**Text** | Pointer to **string** | Warning text; default VOID - DO NOT MAIL | [optional] 
**WidthMm** | Pointer to **float64** |  | [optional] 
**Zpl** | **string** |  | 

## Methods

### NewVoidInputBody

`func NewVoidInputBody(zpl string, ) *VoidInputBody`

NewVoidInputBody instantiates a new VoidInputBody object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewVoidInputBodyWithDefaults

`func NewVoidInputBodyWithDefaults() *VoidInputBody`

NewVoidInputBodyWithDefaults instantiates a new VoidInputBody object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDpmm

`func (o *VoidInputBody) GetDpmm() int64`

GetDpmm returns the Dpmm field if non-nil, zero value otherwise.

### GetDpmmOk

`func (o *VoidInputBody) GetDpmmOk() (*int64, bool)`

GetDpmmOk returns a tuple with the Dpmm field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDpmm

`func (o *VoidInputBody) SetDpmm(v int64)`

SetDpmm sets Dpmm field to given value.

### HasDpmm

`func (o *VoidInputBody) HasDpmm() bool`

HasDpmm returns a boolean if a field has been set.

### GetHeightMm

`func (o *VoidInputBody) GetHeightMm() float64`

GetHeightMm returns the HeightMm field if non-nil, zero value otherwise.

### GetHeightMmOk

`func (o *VoidInputBody) GetHeightMmOk() (*float64, bool)`

GetHeightMmOk returns a tuple with the HeightMm field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHeightMm

`func (o *VoidInputBody) SetHeightMm(v float64)`

SetHeightMm sets HeightMm field to given value.

### HasHeightMm

`func (o *VoidInputBody) HasHeightMm() bool`

HasHeightMm returns a boolean if a field has been set.

### GetPreset

`func (o *VoidInputBody) GetPreset() string`

GetPreset returns the Preset field if non-nil, zero value otherwise.

### GetPresetOk

`func (o *VoidInputBody) GetPresetOk() (*string, bool)`

GetPresetOk returns a tuple with the Preset field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPreset

`func (o *VoidInputBody) SetPreset(v string)`

SetPreset sets Preset field to given value.

### HasPreset

`func (o *VoidInputBody) HasPreset() bool`

HasPreset returns a boolean if a field has been set.

### GetStamp

`func (o *VoidInputBody) GetStamp() string`

GetStamp returns the Stamp field if non-nil, zero value otherwise.

### GetStampOk

`func (o *VoidInputBody) GetStampOk() (*string, bool)`

GetStampOk returns a tuple with the Stamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStamp

`func (o *VoidInputBody) SetStamp(v string)`

SetStamp sets Stamp field to given value.

### HasStamp

`func (o *VoidInputBody) HasStamp() bool`

HasStamp returns a boolean if a field has been set.

### GetText

`func (o *VoidInputBody) GetText() string`

GetText returns the Text field if non-nil, zero value otherwise.

### GetTextOk

`func (o *VoidInputBody) GetTextOk() (*string, bool)`

GetTextOk returns a tuple with the Text field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetText

`func (o *VoidInputBody) SetText(v string)`

SetText sets Text field to given value.

### HasText

`func (o *VoidInputBody) HasText() bool`

HasText returns a boolean if a field has been set.

### GetWidthMm

`func (o *VoidInputBody) GetWidthMm() float64`

GetWidthMm returns the WidthMm field if non-nil, zero value otherwise.

### GetWidthMmOk

`func (o *VoidInputBody) GetWidthMmOk() (*float64, bool)`

GetWidthMmOk returns a tuple with the WidthMm field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWidthMm

`func (o *VoidInputBody) SetWidthMm(v float64)`

SetWidthMm sets WidthMm field to given value.

### HasWidthMm

`func (o *VoidInputBody) HasWidthMm() bool`

HasWidthMm returns a boolean if a field has been set.

### GetZpl

`func (o *VoidInputBody) GetZpl() string`

GetZpl returns the Zpl field if non-nil, zero value otherwise.

### GetZplOk

`func (o *VoidInputBody) GetZplOk() (*string, bool)`

GetZplOk returns a tuple with the Zpl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetZpl

`func (o *VoidInputBody) SetZpl(v string)`

SetZpl sets Zpl field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


