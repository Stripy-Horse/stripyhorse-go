# CreatePrinterInputBody

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AccessMode** | Pointer to **string** | Who may print to the TCP port; default open. Use token from CI, where the source address is different every run. | [optional] 
**Anonymize** | Pointer to **bool** | Mask PII and strip graphics from every captured frame | [optional] 
**Dpmm** | Pointer to **int64** | Print density in dots/mm (152/203/300/600 dpi); default 8 | [optional] 
**HeightMm** | Pointer to **float64** |  | [optional] 
**Mode** | Pointer to **string** |  | [optional] 
**Name** | **string** |  | 
**Preset** | Pointer to **string** | Named label size in inches; alternative to widthMm/heightMm | [optional] 
**SharedPort** | Pointer to **bool** | Put this printer on the shared router port instead of spending one of the plan&#39;s dedicated ports. It is then reached by naming it in the stream, a ZPL comment carrying the ingest token, which suits CI. | [optional] 
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

### GetAccessMode

`func (o *CreatePrinterInputBody) GetAccessMode() string`

GetAccessMode returns the AccessMode field if non-nil, zero value otherwise.

### GetAccessModeOk

`func (o *CreatePrinterInputBody) GetAccessModeOk() (*string, bool)`

GetAccessModeOk returns a tuple with the AccessMode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccessMode

`func (o *CreatePrinterInputBody) SetAccessMode(v string)`

SetAccessMode sets AccessMode field to given value.

### HasAccessMode

`func (o *CreatePrinterInputBody) HasAccessMode() bool`

HasAccessMode returns a boolean if a field has been set.

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

### GetSharedPort

`func (o *CreatePrinterInputBody) GetSharedPort() bool`

GetSharedPort returns the SharedPort field if non-nil, zero value otherwise.

### GetSharedPortOk

`func (o *CreatePrinterInputBody) GetSharedPortOk() (*bool, bool)`

GetSharedPortOk returns a tuple with the SharedPort field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSharedPort

`func (o *CreatePrinterInputBody) SetSharedPort(v bool)`

SetSharedPort sets SharedPort field to given value.

### HasSharedPort

`func (o *CreatePrinterInputBody) HasSharedPort() bool`

HasSharedPort returns a boolean if a field has been set.

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


