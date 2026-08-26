# StateOutputBody

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**State** | [**StatusSnapshot**](StatusSnapshot.md) |  | 

## Methods

### NewStateOutputBody

`func NewStateOutputBody(state StatusSnapshot, ) *StateOutputBody`

NewStateOutputBody instantiates a new StateOutputBody object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewStateOutputBodyWithDefaults

`func NewStateOutputBodyWithDefaults() *StateOutputBody`

NewStateOutputBodyWithDefaults instantiates a new StateOutputBody object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetState

`func (o *StateOutputBody) GetState() StatusSnapshot`

GetState returns the State field if non-nil, zero value otherwise.

### GetStateOk

`func (o *StateOutputBody) GetStateOk() (*StatusSnapshot, bool)`

GetStateOk returns a tuple with the State field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetState

`func (o *StateOutputBody) SetState(v StatusSnapshot)`

SetState sets State field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


