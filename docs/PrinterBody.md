# PrinterBody

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AccessMode** | **string** | Who may print to the TCP port: open (anyone), token (the stream must open with ~SH plus the ingest token), ip (only addresses the org has claimed) | 
**Anonymize** | **bool** | When true, PII is masked and graphics stripped from every captured frame | 
**CreatedAt** | **time.Time** |  | 
**Dpmm** | **int64** |  | 
**ExpiresAt** | Pointer to **time.Time** |  | [optional] 
**HeightMm** | **float64** |  | 
**Id** | **string** |  | 
**IngestUrl** | Pointer to **string** | HTTPS print capability URL. Only returned on creation. | [optional] 
**Mode** | **string** |  | 
**Name** | **string** |  | 
**State** | Pointer to [**StatusSnapshot**](StatusSnapshot.md) |  | [optional] 
**Tcp** | [**PrinterBodyTCPStruct**](PrinterBodyTCPStruct.md) |  | 
**WebhookSecret** | Pointer to **string** | HMAC-SHA256 key for X-Stripy-Horse-Signature. Only returned on creation. | [optional] 
**WebhookUrl** | Pointer to **string** |  | [optional] 
**WidthMm** | **float64** |  | 

## Methods

### NewPrinterBody

`func NewPrinterBody(accessMode string, anonymize bool, createdAt time.Time, dpmm int64, heightMm float64, id string, mode string, name string, tcp PrinterBodyTCPStruct, widthMm float64, ) *PrinterBody`

NewPrinterBody instantiates a new PrinterBody object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPrinterBodyWithDefaults

`func NewPrinterBodyWithDefaults() *PrinterBody`

NewPrinterBodyWithDefaults instantiates a new PrinterBody object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAccessMode

`func (o *PrinterBody) GetAccessMode() string`

GetAccessMode returns the AccessMode field if non-nil, zero value otherwise.

### GetAccessModeOk

`func (o *PrinterBody) GetAccessModeOk() (*string, bool)`

GetAccessModeOk returns a tuple with the AccessMode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccessMode

`func (o *PrinterBody) SetAccessMode(v string)`

SetAccessMode sets AccessMode field to given value.


### GetAnonymize

`func (o *PrinterBody) GetAnonymize() bool`

GetAnonymize returns the Anonymize field if non-nil, zero value otherwise.

### GetAnonymizeOk

`func (o *PrinterBody) GetAnonymizeOk() (*bool, bool)`

GetAnonymizeOk returns a tuple with the Anonymize field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAnonymize

`func (o *PrinterBody) SetAnonymize(v bool)`

SetAnonymize sets Anonymize field to given value.


### GetCreatedAt

`func (o *PrinterBody) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *PrinterBody) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *PrinterBody) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.


### GetDpmm

`func (o *PrinterBody) GetDpmm() int64`

GetDpmm returns the Dpmm field if non-nil, zero value otherwise.

### GetDpmmOk

`func (o *PrinterBody) GetDpmmOk() (*int64, bool)`

GetDpmmOk returns a tuple with the Dpmm field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDpmm

`func (o *PrinterBody) SetDpmm(v int64)`

SetDpmm sets Dpmm field to given value.


### GetExpiresAt

`func (o *PrinterBody) GetExpiresAt() time.Time`

GetExpiresAt returns the ExpiresAt field if non-nil, zero value otherwise.

### GetExpiresAtOk

`func (o *PrinterBody) GetExpiresAtOk() (*time.Time, bool)`

GetExpiresAtOk returns a tuple with the ExpiresAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiresAt

`func (o *PrinterBody) SetExpiresAt(v time.Time)`

SetExpiresAt sets ExpiresAt field to given value.

### HasExpiresAt

`func (o *PrinterBody) HasExpiresAt() bool`

HasExpiresAt returns a boolean if a field has been set.

### GetHeightMm

`func (o *PrinterBody) GetHeightMm() float64`

GetHeightMm returns the HeightMm field if non-nil, zero value otherwise.

### GetHeightMmOk

`func (o *PrinterBody) GetHeightMmOk() (*float64, bool)`

GetHeightMmOk returns a tuple with the HeightMm field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHeightMm

`func (o *PrinterBody) SetHeightMm(v float64)`

SetHeightMm sets HeightMm field to given value.


### GetId

`func (o *PrinterBody) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *PrinterBody) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *PrinterBody) SetId(v string)`

SetId sets Id field to given value.


### GetIngestUrl

`func (o *PrinterBody) GetIngestUrl() string`

GetIngestUrl returns the IngestUrl field if non-nil, zero value otherwise.

### GetIngestUrlOk

`func (o *PrinterBody) GetIngestUrlOk() (*string, bool)`

GetIngestUrlOk returns a tuple with the IngestUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIngestUrl

`func (o *PrinterBody) SetIngestUrl(v string)`

SetIngestUrl sets IngestUrl field to given value.

### HasIngestUrl

`func (o *PrinterBody) HasIngestUrl() bool`

HasIngestUrl returns a boolean if a field has been set.

### GetMode

`func (o *PrinterBody) GetMode() string`

GetMode returns the Mode field if non-nil, zero value otherwise.

### GetModeOk

`func (o *PrinterBody) GetModeOk() (*string, bool)`

GetModeOk returns a tuple with the Mode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMode

`func (o *PrinterBody) SetMode(v string)`

SetMode sets Mode field to given value.


### GetName

`func (o *PrinterBody) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *PrinterBody) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *PrinterBody) SetName(v string)`

SetName sets Name field to given value.


### GetState

`func (o *PrinterBody) GetState() StatusSnapshot`

GetState returns the State field if non-nil, zero value otherwise.

### GetStateOk

`func (o *PrinterBody) GetStateOk() (*StatusSnapshot, bool)`

GetStateOk returns a tuple with the State field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetState

`func (o *PrinterBody) SetState(v StatusSnapshot)`

SetState sets State field to given value.

### HasState

`func (o *PrinterBody) HasState() bool`

HasState returns a boolean if a field has been set.

### GetTcp

`func (o *PrinterBody) GetTcp() PrinterBodyTCPStruct`

GetTcp returns the Tcp field if non-nil, zero value otherwise.

### GetTcpOk

`func (o *PrinterBody) GetTcpOk() (*PrinterBodyTCPStruct, bool)`

GetTcpOk returns a tuple with the Tcp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTcp

`func (o *PrinterBody) SetTcp(v PrinterBodyTCPStruct)`

SetTcp sets Tcp field to given value.


### GetWebhookSecret

`func (o *PrinterBody) GetWebhookSecret() string`

GetWebhookSecret returns the WebhookSecret field if non-nil, zero value otherwise.

### GetWebhookSecretOk

`func (o *PrinterBody) GetWebhookSecretOk() (*string, bool)`

GetWebhookSecretOk returns a tuple with the WebhookSecret field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWebhookSecret

`func (o *PrinterBody) SetWebhookSecret(v string)`

SetWebhookSecret sets WebhookSecret field to given value.

### HasWebhookSecret

`func (o *PrinterBody) HasWebhookSecret() bool`

HasWebhookSecret returns a boolean if a field has been set.

### GetWebhookUrl

`func (o *PrinterBody) GetWebhookUrl() string`

GetWebhookUrl returns the WebhookUrl field if non-nil, zero value otherwise.

### GetWebhookUrlOk

`func (o *PrinterBody) GetWebhookUrlOk() (*string, bool)`

GetWebhookUrlOk returns a tuple with the WebhookUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWebhookUrl

`func (o *PrinterBody) SetWebhookUrl(v string)`

SetWebhookUrl sets WebhookUrl field to given value.

### HasWebhookUrl

`func (o *PrinterBody) HasWebhookUrl() bool`

HasWebhookUrl returns a boolean if a field has been set.

### GetWidthMm

`func (o *PrinterBody) GetWidthMm() float64`

GetWidthMm returns the WidthMm field if non-nil, zero value otherwise.

### GetWidthMmOk

`func (o *PrinterBody) GetWidthMmOk() (*float64, bool)`

GetWidthMmOk returns a tuple with the WidthMm field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWidthMm

`func (o *PrinterBody) SetWidthMm(v float64)`

SetWidthMm sets WidthMm field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


