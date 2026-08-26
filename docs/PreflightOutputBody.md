# PreflightOutputBody

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Labels** | [**[]Report**](Report.md) | One report per rendered label | 
**Lint** | [**[]Finding**](Finding.md) | Static ZPL findings: structure, encoding, bounds | 

## Methods

### NewPreflightOutputBody

`func NewPreflightOutputBody(labels []Report, lint []Finding, ) *PreflightOutputBody`

NewPreflightOutputBody instantiates a new PreflightOutputBody object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPreflightOutputBodyWithDefaults

`func NewPreflightOutputBodyWithDefaults() *PreflightOutputBody`

NewPreflightOutputBodyWithDefaults instantiates a new PreflightOutputBody object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetLabels

`func (o *PreflightOutputBody) GetLabels() []Report`

GetLabels returns the Labels field if non-nil, zero value otherwise.

### GetLabelsOk

`func (o *PreflightOutputBody) GetLabelsOk() (*[]Report, bool)`

GetLabelsOk returns a tuple with the Labels field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLabels

`func (o *PreflightOutputBody) SetLabels(v []Report)`

SetLabels sets Labels field to given value.


### SetLabelsNil

`func (o *PreflightOutputBody) SetLabelsNil(b bool)`

 SetLabelsNil sets the value for Labels to be an explicit nil

### UnsetLabels
`func (o *PreflightOutputBody) UnsetLabels()`

UnsetLabels ensures that no value is present for Labels, not even an explicit nil
### GetLint

`func (o *PreflightOutputBody) GetLint() []Finding`

GetLint returns the Lint field if non-nil, zero value otherwise.

### GetLintOk

`func (o *PreflightOutputBody) GetLintOk() (*[]Finding, bool)`

GetLintOk returns a tuple with the Lint field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLint

`func (o *PreflightOutputBody) SetLint(v []Finding)`

SetLint sets Lint field to given value.


### SetLintNil

`func (o *PreflightOutputBody) SetLintNil(b bool)`

 SetLintNil sets the value for Lint to be an explicit nil

### UnsetLint
`func (o *PreflightOutputBody) UnsetLint()`

UnsetLint ensures that no value is present for Lint, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


