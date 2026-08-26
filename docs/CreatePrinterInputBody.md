# CreatePrinterInputBody

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Anonymize** | Pointer to **bool** | Mask PII and strip graphics from every captured frame | [optional] 
**Dpmm** | Pointer to **int64** | Print density in dots/mm (152/203/300/600 dpi); default 8 | [optional] 
**HeightMm** | Pointer to **float64** |  | [optional] 
**Mode** | Pointer to **string** |  | [optional] 
**Name** | **string** |  | 
**Preset** | Pointer to **string** | Named label size in inches; alternative to widthMm/heightMm | [optional] 
**WebhookUrl** | Pointer to **string** |  | [optional] 
**WidthMm** | Pointer to **float64** |  | [optional] 

## Methods

### NewCreatePrinterInputBody

`func NewCreatePrinterInputBody(name string, ) *CreatePrinterInputBody`

NewCreatePrinterInputBody instantiates a new CreatePrinterInputBody object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreatePrinterInputBodyWithDefaults

`func NewCreatePrinterInputBodyWithDefaults() *CreatePrinterInputBody`

NewCreatePrinterInputBodyWithDefaults instantiates a new CreatePrinterInputBody object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAnonymize

`func (o *CreatePrinterInputBody) GetAnonymize() bool`

GetAnonymize returns the Anonymize field if non-nil, zero value otherwise.

### GetAnonymizeOk

`func (o *CreatePrinterInputBody) GetAnonymizeOk() (*bool, bool)`

GetAnonymizeOk returns a tuple with the Anonymize field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAnonymize

`func (o *CreatePrinterInputBody) SetAnonymize(v bool)`

SetAnonymize sets Anonymize field to given value.

### HasAnonymize

`func (o *CreatePrinterInputBody) HasAnonymize() bool`

HasAnonymize returns a boolean if a field has been set.

### GetDpmm

`func (o *CreatePrinterInputBody) GetDpmm() int64`

GetDpmm returns the Dpmm field if non-nil, zero value otherwise.

### GetDpmmOk

`func (o *CreatePrinterInputBody) GetDpmmOk() (*int64, bool)`

GetDpmmOk returns a tuple with the Dpmm field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDpmm

`func (o *CreatePrinterInputBody) SetDpmm(v int64)`

SetDpmm sets Dpmm field to given value.

### HasDpmm

`func (o *CreatePrinterInputBody) HasDpmm() bool`

HasDpmm returns a boolean if a field has been set.

### GetHeightMm

`func (o *CreatePrinterInputBody) GetHeightMm() float64`

GetHeightMm returns the HeightMm field if non-nil, zero value otherwise.

### GetHeightMmOk

`func (o *CreatePrinterInputBody) GetHeightMmOk() (*float64, bool)`

GetHeightMmOk returns a tuple with the HeightMm field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHeightMm

`func (o *CreatePrinterInputBody) SetHeightMm(v float64)`

SetHeightMm sets HeightMm field to given value.

### HasHeightMm

`func (o *CreatePrinterInputBody) HasHeightMm() bool`

HasHeightMm returns a boolean if a field has been set.

### GetMode

`func (o *CreatePrinterInputBody) GetMode() string`

GetMode returns the Mode field if non-nil, zero value otherwise.

### GetModeOk

`func (o *CreatePrinterInputBody) GetModeOk() (*string, bool)`

GetModeOk returns a tuple with the Mode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMode

`func (o *CreatePrinterInputBody) SetMode(v string)`

SetMode sets Mode field to given value.

### HasMode

`func (o *CreatePrinterInputBody) HasMode() bool`

HasMode returns a boolean if a field has been set.

### GetName

`func (o *CreatePrinterInputBody) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CreatePrinterInputBody) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CreatePrinterInputBody) SetName(v string)`

SetName sets Name field to given value.


### GetPreset

`func (o *CreatePrinterInputBody) GetPreset() string`

GetPreset returns the Preset field if non-nil, zero value otherwise.

### GetPresetOk

`func (o *CreatePrinterInputBody) GetPresetOk() (*string, bool)`

GetPresetOk returns a tuple with the Preset field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPreset

`func (o *CreatePrinterInputBody) SetPreset(v string)`

SetPreset sets Preset field to given value.

### HasPreset

`func (o *CreatePrinterInputBody) HasPreset() bool`

HasPreset returns a boolean if a field has been set.

### GetWebhookUrl

`func (o *CreatePrinterInputBody) GetWebhookUrl() string`

GetWebhookUrl returns the WebhookUrl field if non-nil, zero value otherwise.

### GetWebhookUrlOk

`func (o *CreatePrinterInputBody) GetWebhookUrlOk() (*string, bool)`

GetWebhookUrlOk returns a tuple with the WebhookUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWebhookUrl

`func (o *CreatePrinterInputBody) SetWebhookUrl(v string)`

SetWebhookUrl sets WebhookUrl field to given value.

### HasWebhookUrl

`func (o *CreatePrinterInputBody) HasWebhookUrl() bool`

HasWebhookUrl returns a boolean if a field has been set.

### GetWidthMm

`func (o *CreatePrinterInputBody) GetWidthMm() float64`

GetWidthMm returns the WidthMm field if non-nil, zero value otherwise.

### GetWidthMmOk

`func (o *CreatePrinterInputBody) GetWidthMmOk() (*float64, bool)`

GetWidthMmOk returns a tuple with the WidthMm field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWidthMm

`func (o *CreatePrinterInputBody) SetWidthMm(v float64)`

SetWidthMm sets WidthMm field to given value.

### HasWidthMm

`func (o *CreatePrinterInputBody) HasWidthMm() bool`

HasWidthMm returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


