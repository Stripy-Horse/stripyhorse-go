# Element

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Align** | Pointer to **string** | Alignment when wrapping | [optional] 
**CornerRadius** | Pointer to **int64** | Box corner rounding 0-8 | [optional] 
**Data** | Pointer to **string** | Barcode payload; {{name}} interpolates | [optional] 
**Diameter** | Pointer to **int64** | Circle diameter in dots | [optional] 
**ErrorCorrection** | Pointer to **string** | QR error correction (default M) | [optional] 
**Font** | Pointer to **string** | Printer font: 0 (scalable, default) or A-Z | [optional] 
**FontHeight** | Pointer to **int64** | Character height in dots (text) | [optional] 
**FontWidth** | Pointer to **int64** | Character width in dots; 0 follows fontHeight | [optional] 
**Height** | Pointer to **int64** | Bar height in dots (1D) / box height in dots (box) | [optional] 
**Length** | Pointer to **int64** | Line length in dots | [optional] 
**Lines** | Pointer to **int64** | Max lines when wrapping (default 1) | [optional] 
**Magnification** | Pointer to **int64** | QR module magnification (default 3) | [optional] 
**MaxWidth** | Pointer to **int64** | Wrap text into a block this many dots wide | [optional] 
**ModuleSize** | Pointer to **int64** | DataMatrix module size in dots (default 4) | [optional] 
**ModuleWidth** | Pointer to **int64** | Narrow element width in dots (1D; default 3) | [optional] 
**Orientation** | Pointer to **string** | Line direction | [optional] 
**Png** | Pointer to **string** | PNG/GIF/JPEG, base64-encoded | [optional] 
**PrintText** | Pointer to **bool** | Print the human-readable line under 1D barcodes (default true) | [optional] 
**Rotation** | Pointer to **int64** |  | [optional] 
**Text** | Pointer to **string** | Text content; {{name}} interpolates from variables | [optional] 
**Thickness** | Pointer to **int64** | Stroke thickness in dots (default 1) | [optional] 
**Threshold** | Pointer to **int64** | Bitonal threshold (default 128) | [optional] 
**Type** | **string** | What to place | 
**Width** | Pointer to **int64** | Box/image width in dots | [optional] 
**X** | Pointer to **int64** | Left edge in dots | [optional] 
**Y** | Pointer to **int64** | Top edge in dots | [optional] 
**Zpl** | Pointer to **string** | Verbatim ZPL commands (raw only) - the escape hatch | [optional] 

## Methods

### NewElement

`func NewElement(type_ string, ) *Element`

NewElement instantiates a new Element object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewElementWithDefaults

`func NewElementWithDefaults() *Element`

NewElementWithDefaults instantiates a new Element object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAlign

`func (o *Element) GetAlign() string`

GetAlign returns the Align field if non-nil, zero value otherwise.

### GetAlignOk

`func (o *Element) GetAlignOk() (*string, bool)`

GetAlignOk returns a tuple with the Align field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAlign

`func (o *Element) SetAlign(v string)`

SetAlign sets Align field to given value.

### HasAlign

`func (o *Element) HasAlign() bool`

HasAlign returns a boolean if a field has been set.

### GetCornerRadius

`func (o *Element) GetCornerRadius() int64`

GetCornerRadius returns the CornerRadius field if non-nil, zero value otherwise.

### GetCornerRadiusOk

`func (o *Element) GetCornerRadiusOk() (*int64, bool)`

GetCornerRadiusOk returns a tuple with the CornerRadius field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCornerRadius

`func (o *Element) SetCornerRadius(v int64)`

SetCornerRadius sets CornerRadius field to given value.

### HasCornerRadius

`func (o *Element) HasCornerRadius() bool`

HasCornerRadius returns a boolean if a field has been set.

### GetData

`func (o *Element) GetData() string`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *Element) GetDataOk() (*string, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *Element) SetData(v string)`

SetData sets Data field to given value.

### HasData

`func (o *Element) HasData() bool`

HasData returns a boolean if a field has been set.

### GetDiameter

`func (o *Element) GetDiameter() int64`

GetDiameter returns the Diameter field if non-nil, zero value otherwise.

### GetDiameterOk

`func (o *Element) GetDiameterOk() (*int64, bool)`

GetDiameterOk returns a tuple with the Diameter field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDiameter

`func (o *Element) SetDiameter(v int64)`

SetDiameter sets Diameter field to given value.

### HasDiameter

`func (o *Element) HasDiameter() bool`

HasDiameter returns a boolean if a field has been set.

### GetErrorCorrection

`func (o *Element) GetErrorCorrection() string`

GetErrorCorrection returns the ErrorCorrection field if non-nil, zero value otherwise.

### GetErrorCorrectionOk

`func (o *Element) GetErrorCorrectionOk() (*string, bool)`

GetErrorCorrectionOk returns a tuple with the ErrorCorrection field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrorCorrection

`func (o *Element) SetErrorCorrection(v string)`

SetErrorCorrection sets ErrorCorrection field to given value.

### HasErrorCorrection

`func (o *Element) HasErrorCorrection() bool`

HasErrorCorrection returns a boolean if a field has been set.

### GetFont

`func (o *Element) GetFont() string`

GetFont returns the Font field if non-nil, zero value otherwise.

### GetFontOk

`func (o *Element) GetFontOk() (*string, bool)`

GetFontOk returns a tuple with the Font field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFont

`func (o *Element) SetFont(v string)`

SetFont sets Font field to given value.

### HasFont

`func (o *Element) HasFont() bool`

HasFont returns a boolean if a field has been set.

### GetFontHeight

`func (o *Element) GetFontHeight() int64`

GetFontHeight returns the FontHeight field if non-nil, zero value otherwise.

### GetFontHeightOk

`func (o *Element) GetFontHeightOk() (*int64, bool)`

GetFontHeightOk returns a tuple with the FontHeight field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFontHeight

`func (o *Element) SetFontHeight(v int64)`

SetFontHeight sets FontHeight field to given value.

### HasFontHeight

`func (o *Element) HasFontHeight() bool`

HasFontHeight returns a boolean if a field has been set.

### GetFontWidth

`func (o *Element) GetFontWidth() int64`

GetFontWidth returns the FontWidth field if non-nil, zero value otherwise.

### GetFontWidthOk

`func (o *Element) GetFontWidthOk() (*int64, bool)`

GetFontWidthOk returns a tuple with the FontWidth field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFontWidth

`func (o *Element) SetFontWidth(v int64)`

SetFontWidth sets FontWidth field to given value.

### HasFontWidth

`func (o *Element) HasFontWidth() bool`

HasFontWidth returns a boolean if a field has been set.

### GetHeight

`func (o *Element) GetHeight() int64`

GetHeight returns the Height field if non-nil, zero value otherwise.

### GetHeightOk

`func (o *Element) GetHeightOk() (*int64, bool)`

GetHeightOk returns a tuple with the Height field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHeight

`func (o *Element) SetHeight(v int64)`

SetHeight sets Height field to given value.

### HasHeight

`func (o *Element) HasHeight() bool`

HasHeight returns a boolean if a field has been set.

### GetLength

`func (o *Element) GetLength() int64`

GetLength returns the Length field if non-nil, zero value otherwise.

### GetLengthOk

`func (o *Element) GetLengthOk() (*int64, bool)`

GetLengthOk returns a tuple with the Length field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLength

`func (o *Element) SetLength(v int64)`

SetLength sets Length field to given value.

### HasLength

`func (o *Element) HasLength() bool`

HasLength returns a boolean if a field has been set.

### GetLines

`func (o *Element) GetLines() int64`

GetLines returns the Lines field if non-nil, zero value otherwise.

### GetLinesOk

`func (o *Element) GetLinesOk() (*int64, bool)`

GetLinesOk returns a tuple with the Lines field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLines

`func (o *Element) SetLines(v int64)`

SetLines sets Lines field to given value.

### HasLines

`func (o *Element) HasLines() bool`

HasLines returns a boolean if a field has been set.

### GetMagnification

`func (o *Element) GetMagnification() int64`

GetMagnification returns the Magnification field if non-nil, zero value otherwise.

### GetMagnificationOk

`func (o *Element) GetMagnificationOk() (*int64, bool)`

GetMagnificationOk returns a tuple with the Magnification field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMagnification

`func (o *Element) SetMagnification(v int64)`

SetMagnification sets Magnification field to given value.

### HasMagnification

`func (o *Element) HasMagnification() bool`

HasMagnification returns a boolean if a field has been set.

### GetMaxWidth

`func (o *Element) GetMaxWidth() int64`

GetMaxWidth returns the MaxWidth field if non-nil, zero value otherwise.

### GetMaxWidthOk

`func (o *Element) GetMaxWidthOk() (*int64, bool)`

GetMaxWidthOk returns a tuple with the MaxWidth field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxWidth

`func (o *Element) SetMaxWidth(v int64)`

SetMaxWidth sets MaxWidth field to given value.

### HasMaxWidth

`func (o *Element) HasMaxWidth() bool`

HasMaxWidth returns a boolean if a field has been set.

### GetModuleSize

`func (o *Element) GetModuleSize() int64`

GetModuleSize returns the ModuleSize field if non-nil, zero value otherwise.

### GetModuleSizeOk

`func (o *Element) GetModuleSizeOk() (*int64, bool)`

GetModuleSizeOk returns a tuple with the ModuleSize field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetModuleSize

`func (o *Element) SetModuleSize(v int64)`

SetModuleSize sets ModuleSize field to given value.

### HasModuleSize

`func (o *Element) HasModuleSize() bool`

HasModuleSize returns a boolean if a field has been set.

### GetModuleWidth

`func (o *Element) GetModuleWidth() int64`

GetModuleWidth returns the ModuleWidth field if non-nil, zero value otherwise.

### GetModuleWidthOk

`func (o *Element) GetModuleWidthOk() (*int64, bool)`

GetModuleWidthOk returns a tuple with the ModuleWidth field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetModuleWidth

`func (o *Element) SetModuleWidth(v int64)`

SetModuleWidth sets ModuleWidth field to given value.

### HasModuleWidth

`func (o *Element) HasModuleWidth() bool`

HasModuleWidth returns a boolean if a field has been set.

### GetOrientation

`func (o *Element) GetOrientation() string`

GetOrientation returns the Orientation field if non-nil, zero value otherwise.

### GetOrientationOk

`func (o *Element) GetOrientationOk() (*string, bool)`

GetOrientationOk returns a tuple with the Orientation field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOrientation

`func (o *Element) SetOrientation(v string)`

SetOrientation sets Orientation field to given value.

### HasOrientation

`func (o *Element) HasOrientation() bool`

HasOrientation returns a boolean if a field has been set.

### GetPng

`func (o *Element) GetPng() string`

GetPng returns the Png field if non-nil, zero value otherwise.

### GetPngOk

`func (o *Element) GetPngOk() (*string, bool)`

GetPngOk returns a tuple with the Png field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPng

`func (o *Element) SetPng(v string)`

SetPng sets Png field to given value.

### HasPng

`func (o *Element) HasPng() bool`

HasPng returns a boolean if a field has been set.

### GetPrintText

`func (o *Element) GetPrintText() bool`

GetPrintText returns the PrintText field if non-nil, zero value otherwise.

### GetPrintTextOk

`func (o *Element) GetPrintTextOk() (*bool, bool)`

GetPrintTextOk returns a tuple with the PrintText field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrintText

`func (o *Element) SetPrintText(v bool)`

SetPrintText sets PrintText field to given value.

### HasPrintText

`func (o *Element) HasPrintText() bool`

HasPrintText returns a boolean if a field has been set.

### GetRotation

`func (o *Element) GetRotation() int64`

GetRotation returns the Rotation field if non-nil, zero value otherwise.

### GetRotationOk

`func (o *Element) GetRotationOk() (*int64, bool)`

GetRotationOk returns a tuple with the Rotation field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRotation

`func (o *Element) SetRotation(v int64)`

SetRotation sets Rotation field to given value.

### HasRotation

`func (o *Element) HasRotation() bool`

HasRotation returns a boolean if a field has been set.

### GetText

`func (o *Element) GetText() string`

GetText returns the Text field if non-nil, zero value otherwise.

### GetTextOk

`func (o *Element) GetTextOk() (*string, bool)`

GetTextOk returns a tuple with the Text field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetText

`func (o *Element) SetText(v string)`

SetText sets Text field to given value.

### HasText

`func (o *Element) HasText() bool`

HasText returns a boolean if a field has been set.

### GetThickness

`func (o *Element) GetThickness() int64`

GetThickness returns the Thickness field if non-nil, zero value otherwise.

### GetThicknessOk

`func (o *Element) GetThicknessOk() (*int64, bool)`

GetThicknessOk returns a tuple with the Thickness field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetThickness

`func (o *Element) SetThickness(v int64)`

SetThickness sets Thickness field to given value.

### HasThickness

`func (o *Element) HasThickness() bool`

HasThickness returns a boolean if a field has been set.

### GetThreshold

`func (o *Element) GetThreshold() int64`

GetThreshold returns the Threshold field if non-nil, zero value otherwise.

### GetThresholdOk

`func (o *Element) GetThresholdOk() (*int64, bool)`

GetThresholdOk returns a tuple with the Threshold field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetThreshold

`func (o *Element) SetThreshold(v int64)`

SetThreshold sets Threshold field to given value.

### HasThreshold

`func (o *Element) HasThreshold() bool`

HasThreshold returns a boolean if a field has been set.

### GetType

`func (o *Element) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *Element) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *Element) SetType(v string)`

SetType sets Type field to given value.


### GetWidth

`func (o *Element) GetWidth() int64`

GetWidth returns the Width field if non-nil, zero value otherwise.

### GetWidthOk

`func (o *Element) GetWidthOk() (*int64, bool)`

GetWidthOk returns a tuple with the Width field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWidth

`func (o *Element) SetWidth(v int64)`

SetWidth sets Width field to given value.

### HasWidth

`func (o *Element) HasWidth() bool`

HasWidth returns a boolean if a field has been set.

### GetX

`func (o *Element) GetX() int64`

GetX returns the X field if non-nil, zero value otherwise.

### GetXOk

`func (o *Element) GetXOk() (*int64, bool)`

GetXOk returns a tuple with the X field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetX

`func (o *Element) SetX(v int64)`

SetX sets X field to given value.

### HasX

`func (o *Element) HasX() bool`

HasX returns a boolean if a field has been set.

### GetY

`func (o *Element) GetY() int64`

GetY returns the Y field if non-nil, zero value otherwise.

### GetYOk

`func (o *Element) GetYOk() (*int64, bool)`

GetYOk returns a tuple with the Y field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetY

`func (o *Element) SetY(v int64)`

SetY sets Y field to given value.

### HasY

`func (o *Element) HasY() bool`

HasY returns a boolean if a field has been set.

### GetZpl

`func (o *Element) GetZpl() string`

GetZpl returns the Zpl field if non-nil, zero value otherwise.

### GetZplOk

`func (o *Element) GetZplOk() (*string, bool)`

GetZplOk returns a tuple with the Zpl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetZpl

`func (o *Element) SetZpl(v string)`

SetZpl sets Zpl field to given value.

### HasZpl

`func (o *Element) HasZpl() bool`

HasZpl returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


