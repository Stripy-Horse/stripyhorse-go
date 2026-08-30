# HeldJob

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Bytes** | **int64** | Size of the held frame | 
**ReceivedAt** | **time.Time** |  | 
**Source** | **string** | How it arrived: tcp or https | 

## Methods

### NewHeldJob

`func NewHeldJob(bytes int64, receivedAt time.Time, source string, ) *HeldJob`

NewHeldJob instantiates a new HeldJob object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewHeldJobWithDefaults

`func NewHeldJobWithDefaults() *HeldJob`

NewHeldJobWithDefaults instantiates a new HeldJob object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetBytes

`func (o *HeldJob) GetBytes() int64`

GetBytes returns the Bytes field if non-nil, zero value otherwise.

### GetBytesOk

`func (o *HeldJob) GetBytesOk() (*int64, bool)`

GetBytesOk returns a tuple with the Bytes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBytes

`func (o *HeldJob) SetBytes(v int64)`

SetBytes sets Bytes field to given value.


### GetReceivedAt

`func (o *HeldJob) GetReceivedAt() time.Time`

GetReceivedAt returns the ReceivedAt field if non-nil, zero value otherwise.

### GetReceivedAtOk

`func (o *HeldJob) GetReceivedAtOk() (*time.Time, bool)`

GetReceivedAtOk returns a tuple with the ReceivedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReceivedAt

`func (o *HeldJob) SetReceivedAt(v time.Time)`

SetReceivedAt sets ReceivedAt field to given value.


### GetSource

`func (o *HeldJob) GetSource() string`

GetSource returns the Source field if non-nil, zero value otherwise.

### GetSourceOk

`func (o *HeldJob) GetSourceOk() (*string, bool)`

GetSourceOk returns a tuple with the Source field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSource

`func (o *HeldJob) SetSource(v string)`

SetSource sets Source field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


