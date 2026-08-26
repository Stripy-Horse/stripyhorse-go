# JobSummary

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Error** | Pointer to **string** |  | [optional] 
**Id** | **int64** |  | 
**LabelCount** | **int64** |  | 
**ReceivedAt** | **time.Time** |  | 
**Source** | **string** |  | 
**Status** | **string** |  | 
**ZplBytes** | **int64** |  | 

## Methods

### NewJobSummary

`func NewJobSummary(id int64, labelCount int64, receivedAt time.Time, source string, status string, zplBytes int64, ) *JobSummary`

NewJobSummary instantiates a new JobSummary object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewJobSummaryWithDefaults

`func NewJobSummaryWithDefaults() *JobSummary`

NewJobSummaryWithDefaults instantiates a new JobSummary object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetError

`func (o *JobSummary) GetError() string`

GetError returns the Error field if non-nil, zero value otherwise.

### GetErrorOk

`func (o *JobSummary) GetErrorOk() (*string, bool)`

GetErrorOk returns a tuple with the Error field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetError

`func (o *JobSummary) SetError(v string)`

SetError sets Error field to given value.

### HasError

`func (o *JobSummary) HasError() bool`

HasError returns a boolean if a field has been set.

### GetId

`func (o *JobSummary) GetId() int64`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *JobSummary) GetIdOk() (*int64, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *JobSummary) SetId(v int64)`

SetId sets Id field to given value.


### GetLabelCount

`func (o *JobSummary) GetLabelCount() int64`

GetLabelCount returns the LabelCount field if non-nil, zero value otherwise.

### GetLabelCountOk

`func (o *JobSummary) GetLabelCountOk() (*int64, bool)`

GetLabelCountOk returns a tuple with the LabelCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLabelCount

`func (o *JobSummary) SetLabelCount(v int64)`

SetLabelCount sets LabelCount field to given value.


### GetReceivedAt

`func (o *JobSummary) GetReceivedAt() time.Time`

GetReceivedAt returns the ReceivedAt field if non-nil, zero value otherwise.

### GetReceivedAtOk

`func (o *JobSummary) GetReceivedAtOk() (*time.Time, bool)`

GetReceivedAtOk returns a tuple with the ReceivedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReceivedAt

`func (o *JobSummary) SetReceivedAt(v time.Time)`

SetReceivedAt sets ReceivedAt field to given value.


### GetSource

`func (o *JobSummary) GetSource() string`

GetSource returns the Source field if non-nil, zero value otherwise.

### GetSourceOk

`func (o *JobSummary) GetSourceOk() (*string, bool)`

GetSourceOk returns a tuple with the Source field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSource

`func (o *JobSummary) SetSource(v string)`

SetSource sets Source field to given value.


### GetStatus

`func (o *JobSummary) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *JobSummary) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *JobSummary) SetStatus(v string)`

SetStatus sets Status field to given value.


### GetZplBytes

`func (o *JobSummary) GetZplBytes() int64`

GetZplBytes returns the ZplBytes field if non-nil, zero value otherwise.

### GetZplBytesOk

`func (o *JobSummary) GetZplBytesOk() (*int64, bool)`

GetZplBytesOk returns a tuple with the ZplBytes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetZplBytes

`func (o *JobSummary) SetZplBytes(v int64)`

SetZplBytes sets ZplBytes field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


