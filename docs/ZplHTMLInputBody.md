# ZplHTMLInputBody

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Dpmm** | Pointer to **int64** | Print density in dots/mm (152/203/300/600 dpi); default 8 | [optional] 
**HeightMm** | Pointer to **float64** |  | [optional] 
**Preset** | Pointer to **string** | Named label size in inches; alternative to widthMm/heightMm | [optional] 
**WidthMm** | Pointer to **float64** |  | [optional] 
**Zpl** | **string** |  | 

## Methods

### NewZplHTMLInputBody

`func NewZplHTMLInputBody(zpl string, ) *ZplHTMLInputBody`

NewZplHTMLInputBody instantiates a new ZplHTMLInputBody object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewZplHTMLInputBodyWithDefaults

`func NewZplHTMLInputBodyWithDefaults() *ZplHTMLInputBody`

NewZplHTMLInputBodyWithDefaults instantiates a new ZplHTMLInputBody object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDpmm

`func (o *ZplHTMLInputBody) GetDpmm() int64`

GetDpmm returns the Dpmm field if non-nil, zero value otherwise.

### GetDpmmOk

`func (o *ZplHTMLInputBody) GetDpmmOk() (*int64, bool)`

GetDpmmOk returns a tuple with the Dpmm field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDpmm

`func (o *ZplHTMLInputBody) SetDpmm(v int64)`

SetDpmm sets Dpmm field to given value.

### HasDpmm

`func (o *ZplHTMLInputBody) HasDpmm() bool`

HasDpmm returns a boolean if a field has been set.

### GetHeightMm

`func (o *ZplHTMLInputBody) GetHeightMm() float64`

GetHeightMm returns the HeightMm field if non-nil, zero value otherwise.

### GetHeightMmOk

`func (o *ZplHTMLInputBody) GetHeightMmOk() (*float64, bool)`

GetHeightMmOk returns a tuple with the HeightMm field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHeightMm

`func (o *ZplHTMLInputBody) SetHeightMm(v float64)`

SetHeightMm sets HeightMm field to given value.

### HasHeightMm

`func (o *ZplHTMLInputBody) HasHeightMm() bool`

HasHeightMm returns a boolean if a field has been set.

### GetPreset

`func (o *ZplHTMLInputBody) GetPreset() string`

GetPreset returns the Preset field if non-nil, zero value otherwise.

### GetPresetOk

`func (o *ZplHTMLInputBody) GetPresetOk() (*string, bool)`

GetPresetOk returns a tuple with the Preset field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPreset

`func (o *ZplHTMLInputBody) SetPreset(v string)`

SetPreset sets Preset field to given value.

### HasPreset

`func (o *ZplHTMLInputBody) HasPreset() bool`

HasPreset returns a boolean if a field has been set.

### GetWidthMm

`func (o *ZplHTMLInputBody) GetWidthMm() float64`

GetWidthMm returns the WidthMm field if non-nil, zero value otherwise.

### GetWidthMmOk

`func (o *ZplHTMLInputBody) GetWidthMmOk() (*float64, bool)`

GetWidthMmOk returns a tuple with the WidthMm field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWidthMm

`func (o *ZplHTMLInputBody) SetWidthMm(v float64)`

SetWidthMm sets WidthMm field to given value.

### HasWidthMm

`func (o *ZplHTMLInputBody) HasWidthMm() bool`

HasWidthMm returns a boolean if a field has been set.

### GetZpl

`func (o *ZplHTMLInputBody) GetZpl() string`

GetZpl returns the Zpl field if non-nil, zero value otherwise.

### GetZplOk

`func (o *ZplHTMLInputBody) GetZplOk() (*string, bool)`

GetZplOk returns a tuple with the Zpl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetZpl

`func (o *ZplHTMLInputBody) SetZpl(v string)`

SetZpl sets Zpl field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


