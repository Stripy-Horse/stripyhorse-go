# ListJobsOutputBody

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Jobs** | [**[]JobSummary**](JobSummary.md) |  | 

## Methods

### NewListJobsOutputBody

`func NewListJobsOutputBody(jobs []JobSummary, ) *ListJobsOutputBody`

NewListJobsOutputBody instantiates a new ListJobsOutputBody object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewListJobsOutputBodyWithDefaults

`func NewListJobsOutputBodyWithDefaults() *ListJobsOutputBody`

NewListJobsOutputBodyWithDefaults instantiates a new ListJobsOutputBody object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetJobs

`func (o *ListJobsOutputBody) GetJobs() []JobSummary`

GetJobs returns the Jobs field if non-nil, zero value otherwise.

### GetJobsOk

`func (o *ListJobsOutputBody) GetJobsOk() (*[]JobSummary, bool)`

GetJobsOk returns a tuple with the Jobs field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetJobs

`func (o *ListJobsOutputBody) SetJobs(v []JobSummary)`

SetJobs sets Jobs field to given value.


### SetJobsNil

`func (o *ListJobsOutputBody) SetJobsNil(b bool)`

 SetJobsNil sets the value for Jobs to be an explicit nil

### UnsetJobs
`func (o *ListJobsOutputBody) UnsetJobs()`

UnsetJobs ensures that no value is present for Jobs, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


