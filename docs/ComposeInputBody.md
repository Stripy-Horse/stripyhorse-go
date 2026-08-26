# ComposeInputBody

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Dpmm** | Pointer to **int64** |  | [optional] 
**Elements** | [**[]Element**](Element.md) |  | 
**HeightMm** | Pointer to **float64** |  | [optional] 
**Preset** | Pointer to **string** | Named label size; alternative to widthMm/heightMm | [optional] 
**Preview** | Pointer to **bool** | Also render the composed label to PNG | [optional] 
**Variables** | Pointer to **map[string]string** | Values for {{name}} references | [optional] 
**WidthMm** | Pointer to **float64** |  | [optional] 

## Methods

### NewComposeInputBody

`func NewComposeInputBody(elements []Element, ) *ComposeInputBody`

NewComposeInputBody instantiates a new ComposeInputBody object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewComposeInputBodyWithDefaults

`func NewComposeInputBodyWithDefaults() *ComposeInputBody`

NewComposeInputBodyWithDefaults instantiates a new ComposeInputBody object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDpmm

`func (o *ComposeInputBody) GetDpmm() int64`

GetDpmm returns the Dpmm field if non-nil, zero value otherwise.

### GetDpmmOk

`func (o *ComposeInputBody) GetDpmmOk() (*int64, bool)`

GetDpmmOk returns a tuple with the Dpmm field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDpmm

`func (o *ComposeInputBody) SetDpmm(v int64)`

SetDpmm sets Dpmm field to given value.

### HasDpmm

`func (o *ComposeInputBody) HasDpmm() bool`

HasDpmm returns a boolean if a field has been set.

### GetElements

`func (o *ComposeInputBody) GetElements() []Element`

GetElements returns the Elements field if non-nil, zero value otherwise.

### GetElementsOk

`func (o *ComposeInputBody) GetElementsOk() (*[]Element, bool)`

GetElementsOk returns a tuple with the Elements field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetElements

`func (o *ComposeInputBody) SetElements(v []Element)`

SetElements sets Elements field to given value.


### SetElementsNil

`func (o *ComposeInputBody) SetElementsNil(b bool)`

 SetElementsNil sets the value for Elements to be an explicit nil

### UnsetElements
`func (o *ComposeInputBody) UnsetElements()`

UnsetElements ensures that no value is present for Elements, not even an explicit nil
### GetHeightMm

`func (o *ComposeInputBody) GetHeightMm() float64`

GetHeightMm returns the HeightMm field if non-nil, zero value otherwise.

### GetHeightMmOk

`func (o *ComposeInputBody) GetHeightMmOk() (*float64, bool)`

GetHeightMmOk returns a tuple with the HeightMm field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHeightMm

`func (o *ComposeInputBody) SetHeightMm(v float64)`

SetHeightMm sets HeightMm field to given value.

### HasHeightMm

`func (o *ComposeInputBody) HasHeightMm() bool`

HasHeightMm returns a boolean if a field has been set.

### GetPreset

`func (o *ComposeInputBody) GetPreset() string`

GetPreset returns the Preset field if non-nil, zero value otherwise.

### GetPresetOk

`func (o *ComposeInputBody) GetPresetOk() (*string, bool)`

GetPresetOk returns a tuple with the Preset field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPreset

`func (o *ComposeInputBody) SetPreset(v string)`

SetPreset sets Preset field to given value.

### HasPreset

`func (o *ComposeInputBody) HasPreset() bool`

HasPreset returns a boolean if a field has been set.

### GetPreview

`func (o *ComposeInputBody) GetPreview() bool`

GetPreview returns the Preview field if non-nil, zero value otherwise.

### GetPreviewOk

`func (o *ComposeInputBody) GetPreviewOk() (*bool, bool)`

GetPreviewOk returns a tuple with the Preview field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPreview

`func (o *ComposeInputBody) SetPreview(v bool)`

SetPreview sets Preview field to given value.

### HasPreview

`func (o *ComposeInputBody) HasPreview() bool`

HasPreview returns a boolean if a field has been set.

### GetVariables

`func (o *ComposeInputBody) GetVariables() map[string]string`

GetVariables returns the Variables field if non-nil, zero value otherwise.

### GetVariablesOk

`func (o *ComposeInputBody) GetVariablesOk() (*map[string]string, bool)`

GetVariablesOk returns a tuple with the Variables field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVariables

`func (o *ComposeInputBody) SetVariables(v map[string]string)`

SetVariables sets Variables field to given value.

### HasVariables

`func (o *ComposeInputBody) HasVariables() bool`

HasVariables returns a boolean if a field has been set.

### GetWidthMm

`func (o *ComposeInputBody) GetWidthMm() float64`

GetWidthMm returns the WidthMm field if non-nil, zero value otherwise.

### GetWidthMmOk

`func (o *ComposeInputBody) GetWidthMmOk() (*float64, bool)`

GetWidthMmOk returns a tuple with the WidthMm field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWidthMm

`func (o *ComposeInputBody) SetWidthMm(v float64)`

SetWidthMm sets WidthMm field to given value.

### HasWidthMm

`func (o *ComposeInputBody) HasWidthMm() bool`

HasWidthMm returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


