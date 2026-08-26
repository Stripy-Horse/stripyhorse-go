# StampInputBody

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Image** | **string** | PNG/GIF/JPEG, base64-encoded | 
**WidthDots** | Pointer to **int64** | Stamp width in dots; 0 keeps the image&#39;s natural size | [optional] 
**X** | Pointer to **int64** | Left edge in dots | [optional] 
**Y** | Pointer to **int64** | Top edge in dots | [optional] 
**Zpl** | **string** |  | 

## Methods

### NewStampInputBody

`func NewStampInputBody(image string, zpl string, ) *StampInputBody`

NewStampInputBody instantiates a new StampInputBody object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewStampInputBodyWithDefaults

`func NewStampInputBodyWithDefaults() *StampInputBody`

NewStampInputBodyWithDefaults instantiates a new StampInputBody object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetImage

`func (o *StampInputBody) GetImage() string`

GetImage returns the Image field if non-nil, zero value otherwise.

### GetImageOk

`func (o *StampInputBody) GetImageOk() (*string, bool)`

GetImageOk returns a tuple with the Image field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetImage

`func (o *StampInputBody) SetImage(v string)`

SetImage sets Image field to given value.


### GetWidthDots

`func (o *StampInputBody) GetWidthDots() int64`

GetWidthDots returns the WidthDots field if non-nil, zero value otherwise.

### GetWidthDotsOk

`func (o *StampInputBody) GetWidthDotsOk() (*int64, bool)`

GetWidthDotsOk returns a tuple with the WidthDots field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWidthDots

`func (o *StampInputBody) SetWidthDots(v int64)`

SetWidthDots sets WidthDots field to given value.

### HasWidthDots

`func (o *StampInputBody) HasWidthDots() bool`

HasWidthDots returns a boolean if a field has been set.

### GetX

`func (o *StampInputBody) GetX() int64`

GetX returns the X field if non-nil, zero value otherwise.

### GetXOk

`func (o *StampInputBody) GetXOk() (*int64, bool)`

GetXOk returns a tuple with the X field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetX

`func (o *StampInputBody) SetX(v int64)`

SetX sets X field to given value.

### HasX

`func (o *StampInputBody) HasX() bool`

HasX returns a boolean if a field has been set.

### GetY

`func (o *StampInputBody) GetY() int64`

GetY returns the Y field if non-nil, zero value otherwise.

### GetYOk

`func (o *StampInputBody) GetYOk() (*int64, bool)`

GetYOk returns a tuple with the Y field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetY

`func (o *StampInputBody) SetY(v int64)`

SetY sets Y field to given value.

### HasY

`func (o *StampInputBody) HasY() bool`

HasY returns a boolean if a field has been set.

### GetZpl

`func (o *StampInputBody) GetZpl() string`

GetZpl returns the Zpl field if non-nil, zero value otherwise.

### GetZplOk

`func (o *StampInputBody) GetZplOk() (*string, bool)`

GetZplOk returns a tuple with the Zpl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetZpl

`func (o *StampInputBody) SetZpl(v string)`

SetZpl sets Zpl field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


