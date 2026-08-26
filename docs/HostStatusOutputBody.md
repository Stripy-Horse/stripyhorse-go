# HostStatusOutputBody

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Fields** | [**[]StatusField**](StatusField.md) | Every field with its documented meaning and raw token | 
**Status** | [**HostStatus**](HostStatus.md) |  | 

## Methods

### NewHostStatusOutputBody

`func NewHostStatusOutputBody(fields []StatusField, status HostStatus, ) *HostStatusOutputBody`

NewHostStatusOutputBody instantiates a new HostStatusOutputBody object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewHostStatusOutputBodyWithDefaults

`func NewHostStatusOutputBodyWithDefaults() *HostStatusOutputBody`

NewHostStatusOutputBodyWithDefaults instantiates a new HostStatusOutputBody object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetFields

`func (o *HostStatusOutputBody) GetFields() []StatusField`

GetFields returns the Fields field if non-nil, zero value otherwise.

### GetFieldsOk

`func (o *HostStatusOutputBody) GetFieldsOk() (*[]StatusField, bool)`

GetFieldsOk returns a tuple with the Fields field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFields

`func (o *HostStatusOutputBody) SetFields(v []StatusField)`

SetFields sets Fields field to given value.


### SetFieldsNil

`func (o *HostStatusOutputBody) SetFieldsNil(b bool)`

 SetFieldsNil sets the value for Fields to be an explicit nil

### UnsetFields
`func (o *HostStatusOutputBody) UnsetFields()`

UnsetFields ensures that no value is present for Fields, not even an explicit nil
### GetStatus

`func (o *HostStatusOutputBody) GetStatus() HostStatus`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *HostStatusOutputBody) GetStatusOk() (*HostStatus, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *HostStatusOutputBody) SetStatus(v HostStatus)`

SetStatus sets Status field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


