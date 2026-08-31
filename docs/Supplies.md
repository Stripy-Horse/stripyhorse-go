# Supplies

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**LabelsLeft** | Pointer to **int64** | Labels left on the roll | [optional] 
**LabelsLoaded** | Pointer to **int64** | Labels the roll held when it was fitted; 0 means an endless roll | [optional] 
**RibbonMmLeft** | Pointer to **int64** | Millimetres of ribbon left | [optional] 
**RibbonMmLoaded** | Pointer to **int64** | Millimetres of ribbon fitted; 0 means endless, which is also what direct thermal looks like | [optional] 

## Methods

### NewSupplies

`func NewSupplies() *Supplies`

NewSupplies instantiates a new Supplies object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSuppliesWithDefaults

`func NewSuppliesWithDefaults() *Supplies`

NewSuppliesWithDefaults instantiates a new Supplies object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetLabelsLeft

`func (o *Supplies) GetLabelsLeft() int64`

GetLabelsLeft returns the LabelsLeft field if non-nil, zero value otherwise.

### GetLabelsLeftOk

`func (o *Supplies) GetLabelsLeftOk() (*int64, bool)`

GetLabelsLeftOk returns a tuple with the LabelsLeft field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLabelsLeft

`func (o *Supplies) SetLabelsLeft(v int64)`

SetLabelsLeft sets LabelsLeft field to given value.

### HasLabelsLeft

`func (o *Supplies) HasLabelsLeft() bool`

HasLabelsLeft returns a boolean if a field has been set.

### GetLabelsLoaded

`func (o *Supplies) GetLabelsLoaded() int64`

GetLabelsLoaded returns the LabelsLoaded field if non-nil, zero value otherwise.

### GetLabelsLoadedOk

`func (o *Supplies) GetLabelsLoadedOk() (*int64, bool)`

GetLabelsLoadedOk returns a tuple with the LabelsLoaded field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLabelsLoaded

`func (o *Supplies) SetLabelsLoaded(v int64)`

SetLabelsLoaded sets LabelsLoaded field to given value.

### HasLabelsLoaded

`func (o *Supplies) HasLabelsLoaded() bool`

HasLabelsLoaded returns a boolean if a field has been set.

### GetRibbonMmLeft

`func (o *Supplies) GetRibbonMmLeft() int64`

GetRibbonMmLeft returns the RibbonMmLeft field if non-nil, zero value otherwise.

### GetRibbonMmLeftOk

`func (o *Supplies) GetRibbonMmLeftOk() (*int64, bool)`

GetRibbonMmLeftOk returns a tuple with the RibbonMmLeft field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRibbonMmLeft

`func (o *Supplies) SetRibbonMmLeft(v int64)`

SetRibbonMmLeft sets RibbonMmLeft field to given value.

### HasRibbonMmLeft

`func (o *Supplies) HasRibbonMmLeft() bool`

HasRibbonMmLeft returns a boolean if a field has been set.

### GetRibbonMmLoaded

`func (o *Supplies) GetRibbonMmLoaded() int64`

GetRibbonMmLoaded returns the RibbonMmLoaded field if non-nil, zero value otherwise.

### GetRibbonMmLoadedOk

`func (o *Supplies) GetRibbonMmLoadedOk() (*int64, bool)`

GetRibbonMmLoadedOk returns a tuple with the RibbonMmLoaded field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRibbonMmLoaded

`func (o *Supplies) SetRibbonMmLoaded(v int64)`

SetRibbonMmLoaded sets RibbonMmLoaded field to given value.

### HasRibbonMmLoaded

`func (o *Supplies) HasRibbonMmLoaded() bool`

HasRibbonMmLoaded returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


