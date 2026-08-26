# Finding

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Code** | **string** |  | 
**Label** | **int64** | 1-based label index; 0 &#x3D; whole stream | 
**Message** | **string** |  | 
**Severity** | **string** |  | 

## Methods

### NewFinding

`func NewFinding(code string, label int64, message string, severity string, ) *Finding`

NewFinding instantiates a new Finding object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewFindingWithDefaults

`func NewFindingWithDefaults() *Finding`

NewFindingWithDefaults instantiates a new Finding object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCode

`func (o *Finding) GetCode() string`

GetCode returns the Code field if non-nil, zero value otherwise.

### GetCodeOk

`func (o *Finding) GetCodeOk() (*string, bool)`

GetCodeOk returns a tuple with the Code field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCode

`func (o *Finding) SetCode(v string)`

SetCode sets Code field to given value.


### GetLabel

`func (o *Finding) GetLabel() int64`

GetLabel returns the Label field if non-nil, zero value otherwise.

### GetLabelOk

`func (o *Finding) GetLabelOk() (*int64, bool)`

GetLabelOk returns a tuple with the Label field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLabel

`func (o *Finding) SetLabel(v int64)`

SetLabel sets Label field to given value.


### GetMessage

`func (o *Finding) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *Finding) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *Finding) SetMessage(v string)`

SetMessage sets Message field to given value.


### GetSeverity

`func (o *Finding) GetSeverity() string`

GetSeverity returns the Severity field if non-nil, zero value otherwise.

### GetSeverityOk

`func (o *Finding) GetSeverityOk() (*string, bool)`

GetSeverityOk returns a tuple with the Severity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSeverity

`func (o *Finding) SetSeverity(v string)`

SetSeverity sets Severity field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


