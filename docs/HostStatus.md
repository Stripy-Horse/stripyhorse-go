# HostStatus

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Blocking** | **bool** | True when any condition stops printing | 
**BufferFull** | **bool** |  | 
**CommSettings** | **string** | Raw communication-settings code | 
**CorruptRam** | **bool** |  | 
**DiagnosticMode** | **bool** |  | 
**FormatsInBuffer** | **int64** | Jobs waiting in the receive buffer | 
**FunctionSettings** | **string** | Raw function-settings code | 
**GraphicsStored** | **int64** |  | 
**HeadUp** | **bool** |  | 
**LabelLengthDots** | **int64** |  | 
**LabelsRemaining** | **int64** |  | 
**OverTemp** | **bool** |  | 
**PaperOut** | **bool** |  | 
**PartialFormat** | **bool** |  | 
**Password** | **string** |  | 
**Paused** | **bool** |  | 
**PrintMode** | **string** | rewind, peel-off, tear-off, cutter or applicator | 
**RibbonOut** | **bool** |  | 
**StaticRam** | **bool** |  | 
**ThermalTransfer** | **bool** |  | 
**UnderTemp** | **bool** |  | 

## Methods

### NewHostStatus

`func NewHostStatus(blocking bool, bufferFull bool, commSettings string, corruptRam bool, diagnosticMode bool, formatsInBuffer int64, functionSettings string, graphicsStored int64, headUp bool, labelLengthDots int64, labelsRemaining int64, overTemp bool, paperOut bool, partialFormat bool, password string, paused bool, printMode string, ribbonOut bool, staticRam bool, thermalTransfer bool, underTemp bool, ) *HostStatus`

NewHostStatus instantiates a new HostStatus object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewHostStatusWithDefaults

`func NewHostStatusWithDefaults() *HostStatus`

NewHostStatusWithDefaults instantiates a new HostStatus object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetBlocking

`func (o *HostStatus) GetBlocking() bool`

GetBlocking returns the Blocking field if non-nil, zero value otherwise.

### GetBlockingOk

`func (o *HostStatus) GetBlockingOk() (*bool, bool)`

GetBlockingOk returns a tuple with the Blocking field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBlocking

`func (o *HostStatus) SetBlocking(v bool)`

SetBlocking sets Blocking field to given value.


### GetBufferFull

`func (o *HostStatus) GetBufferFull() bool`

GetBufferFull returns the BufferFull field if non-nil, zero value otherwise.

### GetBufferFullOk

`func (o *HostStatus) GetBufferFullOk() (*bool, bool)`

GetBufferFullOk returns a tuple with the BufferFull field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBufferFull

`func (o *HostStatus) SetBufferFull(v bool)`

SetBufferFull sets BufferFull field to given value.


### GetCommSettings

`func (o *HostStatus) GetCommSettings() string`

GetCommSettings returns the CommSettings field if non-nil, zero value otherwise.

### GetCommSettingsOk

`func (o *HostStatus) GetCommSettingsOk() (*string, bool)`

GetCommSettingsOk returns a tuple with the CommSettings field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCommSettings

`func (o *HostStatus) SetCommSettings(v string)`

SetCommSettings sets CommSettings field to given value.


### GetCorruptRam

`func (o *HostStatus) GetCorruptRam() bool`

GetCorruptRam returns the CorruptRam field if non-nil, zero value otherwise.

### GetCorruptRamOk

`func (o *HostStatus) GetCorruptRamOk() (*bool, bool)`

GetCorruptRamOk returns a tuple with the CorruptRam field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCorruptRam

`func (o *HostStatus) SetCorruptRam(v bool)`

SetCorruptRam sets CorruptRam field to given value.


### GetDiagnosticMode

`func (o *HostStatus) GetDiagnosticMode() bool`

GetDiagnosticMode returns the DiagnosticMode field if non-nil, zero value otherwise.

### GetDiagnosticModeOk

`func (o *HostStatus) GetDiagnosticModeOk() (*bool, bool)`

GetDiagnosticModeOk returns a tuple with the DiagnosticMode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDiagnosticMode

`func (o *HostStatus) SetDiagnosticMode(v bool)`

SetDiagnosticMode sets DiagnosticMode field to given value.


### GetFormatsInBuffer

`func (o *HostStatus) GetFormatsInBuffer() int64`

GetFormatsInBuffer returns the FormatsInBuffer field if non-nil, zero value otherwise.

### GetFormatsInBufferOk

`func (o *HostStatus) GetFormatsInBufferOk() (*int64, bool)`

GetFormatsInBufferOk returns a tuple with the FormatsInBuffer field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFormatsInBuffer

`func (o *HostStatus) SetFormatsInBuffer(v int64)`

SetFormatsInBuffer sets FormatsInBuffer field to given value.


### GetFunctionSettings

`func (o *HostStatus) GetFunctionSettings() string`

GetFunctionSettings returns the FunctionSettings field if non-nil, zero value otherwise.

### GetFunctionSettingsOk

`func (o *HostStatus) GetFunctionSettingsOk() (*string, bool)`

GetFunctionSettingsOk returns a tuple with the FunctionSettings field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFunctionSettings

`func (o *HostStatus) SetFunctionSettings(v string)`

SetFunctionSettings sets FunctionSettings field to given value.


### GetGraphicsStored

`func (o *HostStatus) GetGraphicsStored() int64`

GetGraphicsStored returns the GraphicsStored field if non-nil, zero value otherwise.

### GetGraphicsStoredOk

`func (o *HostStatus) GetGraphicsStoredOk() (*int64, bool)`

GetGraphicsStoredOk returns a tuple with the GraphicsStored field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGraphicsStored

`func (o *HostStatus) SetGraphicsStored(v int64)`

SetGraphicsStored sets GraphicsStored field to given value.


### GetHeadUp

`func (o *HostStatus) GetHeadUp() bool`

GetHeadUp returns the HeadUp field if non-nil, zero value otherwise.

### GetHeadUpOk

`func (o *HostStatus) GetHeadUpOk() (*bool, bool)`

GetHeadUpOk returns a tuple with the HeadUp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHeadUp

`func (o *HostStatus) SetHeadUp(v bool)`

SetHeadUp sets HeadUp field to given value.


### GetLabelLengthDots

`func (o *HostStatus) GetLabelLengthDots() int64`

GetLabelLengthDots returns the LabelLengthDots field if non-nil, zero value otherwise.

### GetLabelLengthDotsOk

`func (o *HostStatus) GetLabelLengthDotsOk() (*int64, bool)`

GetLabelLengthDotsOk returns a tuple with the LabelLengthDots field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLabelLengthDots

`func (o *HostStatus) SetLabelLengthDots(v int64)`

SetLabelLengthDots sets LabelLengthDots field to given value.


### GetLabelsRemaining

`func (o *HostStatus) GetLabelsRemaining() int64`

GetLabelsRemaining returns the LabelsRemaining field if non-nil, zero value otherwise.

### GetLabelsRemainingOk

`func (o *HostStatus) GetLabelsRemainingOk() (*int64, bool)`

GetLabelsRemainingOk returns a tuple with the LabelsRemaining field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLabelsRemaining

`func (o *HostStatus) SetLabelsRemaining(v int64)`

SetLabelsRemaining sets LabelsRemaining field to given value.


### GetOverTemp

`func (o *HostStatus) GetOverTemp() bool`

GetOverTemp returns the OverTemp field if non-nil, zero value otherwise.

### GetOverTempOk

`func (o *HostStatus) GetOverTempOk() (*bool, bool)`

GetOverTempOk returns a tuple with the OverTemp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOverTemp

`func (o *HostStatus) SetOverTemp(v bool)`

SetOverTemp sets OverTemp field to given value.


### GetPaperOut

`func (o *HostStatus) GetPaperOut() bool`

GetPaperOut returns the PaperOut field if non-nil, zero value otherwise.

### GetPaperOutOk

`func (o *HostStatus) GetPaperOutOk() (*bool, bool)`

GetPaperOutOk returns a tuple with the PaperOut field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPaperOut

`func (o *HostStatus) SetPaperOut(v bool)`

SetPaperOut sets PaperOut field to given value.


### GetPartialFormat

`func (o *HostStatus) GetPartialFormat() bool`

GetPartialFormat returns the PartialFormat field if non-nil, zero value otherwise.

### GetPartialFormatOk

`func (o *HostStatus) GetPartialFormatOk() (*bool, bool)`

GetPartialFormatOk returns a tuple with the PartialFormat field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPartialFormat

`func (o *HostStatus) SetPartialFormat(v bool)`

SetPartialFormat sets PartialFormat field to given value.


### GetPassword

`func (o *HostStatus) GetPassword() string`

GetPassword returns the Password field if non-nil, zero value otherwise.

### GetPasswordOk

`func (o *HostStatus) GetPasswordOk() (*string, bool)`

GetPasswordOk returns a tuple with the Password field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPassword

`func (o *HostStatus) SetPassword(v string)`

SetPassword sets Password field to given value.


### GetPaused

`func (o *HostStatus) GetPaused() bool`

GetPaused returns the Paused field if non-nil, zero value otherwise.

### GetPausedOk

`func (o *HostStatus) GetPausedOk() (*bool, bool)`

GetPausedOk returns a tuple with the Paused field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPaused

`func (o *HostStatus) SetPaused(v bool)`

SetPaused sets Paused field to given value.


### GetPrintMode

`func (o *HostStatus) GetPrintMode() string`

GetPrintMode returns the PrintMode field if non-nil, zero value otherwise.

### GetPrintModeOk

`func (o *HostStatus) GetPrintModeOk() (*string, bool)`

GetPrintModeOk returns a tuple with the PrintMode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrintMode

`func (o *HostStatus) SetPrintMode(v string)`

SetPrintMode sets PrintMode field to given value.


### GetRibbonOut

`func (o *HostStatus) GetRibbonOut() bool`

GetRibbonOut returns the RibbonOut field if non-nil, zero value otherwise.

### GetRibbonOutOk

`func (o *HostStatus) GetRibbonOutOk() (*bool, bool)`

GetRibbonOutOk returns a tuple with the RibbonOut field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRibbonOut

`func (o *HostStatus) SetRibbonOut(v bool)`

SetRibbonOut sets RibbonOut field to given value.


### GetStaticRam

`func (o *HostStatus) GetStaticRam() bool`

GetStaticRam returns the StaticRam field if non-nil, zero value otherwise.

### GetStaticRamOk

`func (o *HostStatus) GetStaticRamOk() (*bool, bool)`

GetStaticRamOk returns a tuple with the StaticRam field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStaticRam

`func (o *HostStatus) SetStaticRam(v bool)`

SetStaticRam sets StaticRam field to given value.


### GetThermalTransfer

`func (o *HostStatus) GetThermalTransfer() bool`

GetThermalTransfer returns the ThermalTransfer field if non-nil, zero value otherwise.

### GetThermalTransferOk

`func (o *HostStatus) GetThermalTransferOk() (*bool, bool)`

GetThermalTransferOk returns a tuple with the ThermalTransfer field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetThermalTransfer

`func (o *HostStatus) SetThermalTransfer(v bool)`

SetThermalTransfer sets ThermalTransfer field to given value.


### GetUnderTemp

`func (o *HostStatus) GetUnderTemp() bool`

GetUnderTemp returns the UnderTemp field if non-nil, zero value otherwise.

### GetUnderTempOk

`func (o *HostStatus) GetUnderTempOk() (*bool, bool)`

GetUnderTempOk returns a tuple with the UnderTemp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUnderTemp

`func (o *HostStatus) SetUnderTemp(v bool)`

SetUnderTemp sets UnderTemp field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


