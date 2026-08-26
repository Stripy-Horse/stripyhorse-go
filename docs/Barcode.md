# Barcode

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**BlurMarginDots** | **int64** | Largest blur radius the symbol survives; 0 &#x3D; no margin | 
**Checks** | [**[]Check**](Check.md) |  | 
**CrossDpi** | Pointer to [**[]DPIVerdict**](DPIVerdict.md) | X-dimension at other print densities, same dot counts | [optional] 
**Format** | **string** | CODE_128, CODE_39, ITF, QR_CODE, DATA_MATRIX | 
**ModuleDots** | Pointer to **float64** | Measured narrow-element width in printer dots (1D only) | [optional] 
**QuietLeftModules** | Pointer to **float64** |  | [optional] 
**QuietRightModules** | Pointer to **float64** |  | [optional] 
**Value** | **string** |  | 
**XDimensionMm** | Pointer to **float64** | Physical narrow-element width at the analyzed density | [optional] 

## Methods

### NewBarcode

`func NewBarcode(blurMarginDots int64, checks []Check, format string, value string, ) *Barcode`

NewBarcode instantiates a new Barcode object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBarcodeWithDefaults

`func NewBarcodeWithDefaults() *Barcode`

NewBarcodeWithDefaults instantiates a new Barcode object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetBlurMarginDots

`func (o *Barcode) GetBlurMarginDots() int64`

GetBlurMarginDots returns the BlurMarginDots field if non-nil, zero value otherwise.

### GetBlurMarginDotsOk

`func (o *Barcode) GetBlurMarginDotsOk() (*int64, bool)`

GetBlurMarginDotsOk returns a tuple with the BlurMarginDots field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBlurMarginDots

`func (o *Barcode) SetBlurMarginDots(v int64)`

SetBlurMarginDots sets BlurMarginDots field to given value.


### GetChecks

`func (o *Barcode) GetChecks() []Check`

GetChecks returns the Checks field if non-nil, zero value otherwise.

### GetChecksOk

`func (o *Barcode) GetChecksOk() (*[]Check, bool)`

GetChecksOk returns a tuple with the Checks field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChecks

`func (o *Barcode) SetChecks(v []Check)`

SetChecks sets Checks field to given value.


### SetChecksNil

`func (o *Barcode) SetChecksNil(b bool)`

 SetChecksNil sets the value for Checks to be an explicit nil

### UnsetChecks
`func (o *Barcode) UnsetChecks()`

UnsetChecks ensures that no value is present for Checks, not even an explicit nil
### GetCrossDpi

`func (o *Barcode) GetCrossDpi() []DPIVerdict`

GetCrossDpi returns the CrossDpi field if non-nil, zero value otherwise.

### GetCrossDpiOk

`func (o *Barcode) GetCrossDpiOk() (*[]DPIVerdict, bool)`

GetCrossDpiOk returns a tuple with the CrossDpi field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCrossDpi

`func (o *Barcode) SetCrossDpi(v []DPIVerdict)`

SetCrossDpi sets CrossDpi field to given value.

### HasCrossDpi

`func (o *Barcode) HasCrossDpi() bool`

HasCrossDpi returns a boolean if a field has been set.

### SetCrossDpiNil

`func (o *Barcode) SetCrossDpiNil(b bool)`

 SetCrossDpiNil sets the value for CrossDpi to be an explicit nil

### UnsetCrossDpi
`func (o *Barcode) UnsetCrossDpi()`

UnsetCrossDpi ensures that no value is present for CrossDpi, not even an explicit nil
### GetFormat

`func (o *Barcode) GetFormat() string`

GetFormat returns the Format field if non-nil, zero value otherwise.

### GetFormatOk

`func (o *Barcode) GetFormatOk() (*string, bool)`

GetFormatOk returns a tuple with the Format field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFormat

`func (o *Barcode) SetFormat(v string)`

SetFormat sets Format field to given value.


### GetModuleDots

`func (o *Barcode) GetModuleDots() float64`

GetModuleDots returns the ModuleDots field if non-nil, zero value otherwise.

### GetModuleDotsOk

`func (o *Barcode) GetModuleDotsOk() (*float64, bool)`

GetModuleDotsOk returns a tuple with the ModuleDots field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetModuleDots

`func (o *Barcode) SetModuleDots(v float64)`

SetModuleDots sets ModuleDots field to given value.

### HasModuleDots

`func (o *Barcode) HasModuleDots() bool`

HasModuleDots returns a boolean if a field has been set.

### GetQuietLeftModules

`func (o *Barcode) GetQuietLeftModules() float64`

GetQuietLeftModules returns the QuietLeftModules field if non-nil, zero value otherwise.

### GetQuietLeftModulesOk

`func (o *Barcode) GetQuietLeftModulesOk() (*float64, bool)`

GetQuietLeftModulesOk returns a tuple with the QuietLeftModules field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQuietLeftModules

`func (o *Barcode) SetQuietLeftModules(v float64)`

SetQuietLeftModules sets QuietLeftModules field to given value.

### HasQuietLeftModules

`func (o *Barcode) HasQuietLeftModules() bool`

HasQuietLeftModules returns a boolean if a field has been set.

### GetQuietRightModules

`func (o *Barcode) GetQuietRightModules() float64`

GetQuietRightModules returns the QuietRightModules field if non-nil, zero value otherwise.

### GetQuietRightModulesOk

`func (o *Barcode) GetQuietRightModulesOk() (*float64, bool)`

GetQuietRightModulesOk returns a tuple with the QuietRightModules field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQuietRightModules

`func (o *Barcode) SetQuietRightModules(v float64)`

SetQuietRightModules sets QuietRightModules field to given value.

### HasQuietRightModules

`func (o *Barcode) HasQuietRightModules() bool`

HasQuietRightModules returns a boolean if a field has been set.

### GetValue

`func (o *Barcode) GetValue() string`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *Barcode) GetValueOk() (*string, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *Barcode) SetValue(v string)`

SetValue sets Value field to given value.


### GetXDimensionMm

`func (o *Barcode) GetXDimensionMm() float64`

GetXDimensionMm returns the XDimensionMm field if non-nil, zero value otherwise.

### GetXDimensionMmOk

`func (o *Barcode) GetXDimensionMmOk() (*float64, bool)`

GetXDimensionMmOk returns a tuple with the XDimensionMm field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetXDimensionMm

`func (o *Barcode) SetXDimensionMm(v float64)`

SetXDimensionMm sets XDimensionMm field to given value.

### HasXDimensionMm

`func (o *Barcode) HasXDimensionMm() bool`

HasXDimensionMm returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


