# StatusSnapshot

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Darkness** | **string** | print.tone setting, e.g. 20.0 | 
**Faults** | [**Faults**](Faults.md) |  | 
**FormatsInBuffer** | **int64** |  | 
**FriendlyName** | **string** | device.friendly_name override; empty means unset | 
**LabelLengthDots** | **int64** |  | 
**Odometer** | **int64** |  | 
**SpeedIps** | **string** | media.speed setting, inches/second | 
**WidthDots** | **int64** |  | 

## Methods

### NewStatusSnapshot

`func NewStatusSnapshot(darkness string, faults Faults, formatsInBuffer int64, friendlyName string, labelLengthDots int64, odometer int64, speedIps string, widthDots int64, ) *StatusSnapshot`

NewStatusSnapshot instantiates a new StatusSnapshot object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewStatusSnapshotWithDefaults

`func NewStatusSnapshotWithDefaults() *StatusSnapshot`

NewStatusSnapshotWithDefaults instantiates a new StatusSnapshot object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDarkness

`func (o *StatusSnapshot) GetDarkness() string`

GetDarkness returns the Darkness field if non-nil, zero value otherwise.

### GetDarknessOk

`func (o *StatusSnapshot) GetDarknessOk() (*string, bool)`

GetDarknessOk returns a tuple with the Darkness field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDarkness

`func (o *StatusSnapshot) SetDarkness(v string)`

SetDarkness sets Darkness field to given value.


### GetFaults

`func (o *StatusSnapshot) GetFaults() Faults`

GetFaults returns the Faults field if non-nil, zero value otherwise.

### GetFaultsOk

`func (o *StatusSnapshot) GetFaultsOk() (*Faults, bool)`

GetFaultsOk returns a tuple with the Faults field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFaults

`func (o *StatusSnapshot) SetFaults(v Faults)`

SetFaults sets Faults field to given value.


### GetFormatsInBuffer

`func (o *StatusSnapshot) GetFormatsInBuffer() int64`

GetFormatsInBuffer returns the FormatsInBuffer field if non-nil, zero value otherwise.

### GetFormatsInBufferOk

`func (o *StatusSnapshot) GetFormatsInBufferOk() (*int64, bool)`

GetFormatsInBufferOk returns a tuple with the FormatsInBuffer field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFormatsInBuffer

`func (o *StatusSnapshot) SetFormatsInBuffer(v int64)`

SetFormatsInBuffer sets FormatsInBuffer field to given value.


### GetFriendlyName

`func (o *StatusSnapshot) GetFriendlyName() string`

GetFriendlyName returns the FriendlyName field if non-nil, zero value otherwise.

### GetFriendlyNameOk

`func (o *StatusSnapshot) GetFriendlyNameOk() (*string, bool)`

GetFriendlyNameOk returns a tuple with the FriendlyName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFriendlyName

`func (o *StatusSnapshot) SetFriendlyName(v string)`

SetFriendlyName sets FriendlyName field to given value.


### GetLabelLengthDots

`func (o *StatusSnapshot) GetLabelLengthDots() int64`

GetLabelLengthDots returns the LabelLengthDots field if non-nil, zero value otherwise.

### GetLabelLengthDotsOk

`func (o *StatusSnapshot) GetLabelLengthDotsOk() (*int64, bool)`

GetLabelLengthDotsOk returns a tuple with the LabelLengthDots field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLabelLengthDots

`func (o *StatusSnapshot) SetLabelLengthDots(v int64)`

SetLabelLengthDots sets LabelLengthDots field to given value.


### GetOdometer

`func (o *StatusSnapshot) GetOdometer() int64`

GetOdometer returns the Odometer field if non-nil, zero value otherwise.

### GetOdometerOk

`func (o *StatusSnapshot) GetOdometerOk() (*int64, bool)`

GetOdometerOk returns a tuple with the Odometer field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOdometer

`func (o *StatusSnapshot) SetOdometer(v int64)`

SetOdometer sets Odometer field to given value.


### GetSpeedIps

`func (o *StatusSnapshot) GetSpeedIps() string`

GetSpeedIps returns the SpeedIps field if non-nil, zero value otherwise.

### GetSpeedIpsOk

`func (o *StatusSnapshot) GetSpeedIpsOk() (*string, bool)`

GetSpeedIpsOk returns a tuple with the SpeedIps field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSpeedIps

`func (o *StatusSnapshot) SetSpeedIps(v string)`

SetSpeedIps sets SpeedIps field to given value.


### GetWidthDots

`func (o *StatusSnapshot) GetWidthDots() int64`

GetWidthDots returns the WidthDots field if non-nil, zero value otherwise.

### GetWidthDotsOk

`func (o *StatusSnapshot) GetWidthDotsOk() (*int64, bool)`

GetWidthDotsOk returns a tuple with the WidthDots field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWidthDots

`func (o *StatusSnapshot) SetWidthDots(v int64)`

SetWidthDots sets WidthDots field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


