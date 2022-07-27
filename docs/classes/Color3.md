[@dev/core](../README.md) / [Exports](../modules.md) / Color3

# Class: Color3

Class used to hold a RGB color

## Table of contents

### Constructors

- [constructor](Color3.md#constructor)

### Properties

- [b](Color3.md#b)
- [g](Color3.md#g)
- [r](Color3.md#r)
- [\_BlackReadOnly](Color3.md#_blackreadonly)

### Accessors

- [BlackReadOnly](Color3.md#blackreadonly)

### Methods

- [add](Color3.md#add)
- [addToRef](Color3.md#addtoref)
- [asArray](Color3.md#asarray)
- [clampToRef](Color3.md#clamptoref)
- [clone](Color3.md#clone)
- [copyFrom](Color3.md#copyfrom)
- [copyFromFloats](Color3.md#copyfromfloats)
- [equals](Color3.md#equals)
- [equalsFloats](Color3.md#equalsfloats)
- [fromArray](Color3.md#fromarray)
- [getClassName](Color3.md#getclassname)
- [getHashCode](Color3.md#gethashcode)
- [multiply](Color3.md#multiply)
- [multiplyToRef](Color3.md#multiplytoref)
- [scale](Color3.md#scale)
- [scaleAndAddToRef](Color3.md#scaleandaddtoref)
- [scaleInPlace](Color3.md#scaleinplace)
- [scaleToRef](Color3.md#scaletoref)
- [set](Color3.md#set)
- [subtract](Color3.md#subtract)
- [subtractToRef](Color3.md#subtracttoref)
- [toArray](Color3.md#toarray)
- [toColor4](Color3.md#tocolor4)
- [toGammaSpace](Color3.md#togammaspace)
- [toGammaSpaceToRef](Color3.md#togammaspacetoref)
- [toHSV](Color3.md#tohsv)
- [toHSVToRef](Color3.md#tohsvtoref)
- [toHexString](Color3.md#tohexstring)
- [toLinearSpace](Color3.md#tolinearspace)
- [toLinearSpaceToRef](Color3.md#tolinearspacetoref)
- [toLuminance](Color3.md#toluminance)
- [toString](Color3.md#tostring)
- [Black](Color3.md#black)
- [Blue](Color3.md#blue)
- [FromArray](Color3.md#fromarray-1)
- [FromArrayToRef](Color3.md#fromarraytoref)
- [FromHSV](Color3.md#fromhsv)
- [FromHexString](Color3.md#fromhexstring)
- [FromInts](Color3.md#fromints)
- [Gray](Color3.md#gray)
- [Green](Color3.md#green)
- [HSVtoRGBToRef](Color3.md#hsvtorgbtoref)
- [Hermite](Color3.md#hermite)
- [Hermite1stDerivative](Color3.md#hermite1stderivative)
- [Hermite1stDerivativeToRef](Color3.md#hermite1stderivativetoref)
- [Lerp](Color3.md#lerp)
- [LerpToRef](Color3.md#lerptoref)
- [Magenta](Color3.md#magenta)
- [Purple](Color3.md#purple)
- [Random](Color3.md#random)
- [Red](Color3.md#red)
- [Teal](Color3.md#teal)
- [White](Color3.md#white)
- [Yellow](Color3.md#yellow)

## Constructors

### constructor

• **new Color3**(`r?`, `g?`, `b?`)

Creates a new Color3 object from red, green, blue values, all between 0 and 1

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `r` | `number` | `0` | defines the red component (between 0 and 1, default is 0) |
| `g` | `number` | `0` | defines the green component (between 0 and 1, default is 0) |
| `b` | `number` | `0` | defines the blue component (between 0 and 1, default is 0) |

#### Defined in

packages/dev/core/src/Maths/math.color.ts:17

## Properties

### b

• **b**: `number` = `0`

#### Defined in

packages/dev/core/src/Maths/math.color.ts:29

___

### g

• **g**: `number` = `0`

#### Defined in

packages/dev/core/src/Maths/math.color.ts:25

___

### r

• **r**: `number` = `0`

#### Defined in

packages/dev/core/src/Maths/math.color.ts:21

___

### \_BlackReadOnly

▪ `Static` `Private` **\_BlackReadOnly**: [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Color3`](Color3.md)

#### Defined in

packages/dev/core/src/Maths/math.color.ts:412

## Accessors

### BlackReadOnly

• `Static` `get` **BlackReadOnly**(): [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Color3`](Color3.md)

Gets a Color3 value containing a black color that must not be updated

#### Returns

[`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Color3`](Color3.md)

#### Defined in

packages/dev/core/src/Maths/math.color.ts:644

## Methods

### add

▸ **add**(`otherColor`): [`Color3`](Color3.md)

Creates a new Color3 set with the added values of the current Color3 and of the given one

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherColor` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Color3`](Color3.md) | defines the second operand |

#### Returns

[`Color3`](Color3.md)

the new Color3

#### Defined in

packages/dev/core/src/Maths/math.color.ts:219

___

### addToRef

▸ **addToRef**(`otherColor`, `result`): [`Color3`](Color3.md)

Stores the result of the addition of the current Color3 and given one rgb values into "result"

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherColor` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Color3`](Color3.md) | defines the second operand |
| `result` | [`Color3`](Color3.md) | defines Color3 object to store the result into |

#### Returns

[`Color3`](Color3.md)

the unmodified current Color3

#### Defined in

packages/dev/core/src/Maths/math.color.ts:229

___

### asArray

▸ **asArray**(): `number`[]

Returns a new array populated with 3 numeric elements : red, green and blue values

#### Returns

`number`[]

the new array

#### Defined in

packages/dev/core/src/Maths/math.color.ts:99

___

### clampToRef

▸ **clampToRef**(`min?`, `max?`, `result`): [`Color3`](Color3.md)

Clamps the rgb values by the min and max values and stores the result into "result"

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `min` | `number` | `0` | defines minimum clamping value (default is 0) |
| `max` | `number` | `1` | defines maximum clamping value (default is 1) |
| `result` | [`Color3`](Color3.md) | `undefined` | defines color to store the result into |

#### Returns

[`Color3`](Color3.md)

the original Color3

#### Defined in

packages/dev/core/src/Maths/math.color.ts:207

___

### clone

▸ **clone**(): [`Color3`](Color3.md)

Copy the current object

#### Returns

[`Color3`](Color3.md)

a new Color3 copied the current one

#### Defined in

packages/dev/core/src/Maths/math.color.ts:262

___

### copyFrom

▸ **copyFrom**(`source`): [`Color3`](Color3.md)

Copies the rgb values from the source in the current Color3

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Color3`](Color3.md) | defines the source Color3 object |

#### Returns

[`Color3`](Color3.md)

the updated Color3 object

#### Defined in

packages/dev/core/src/Maths/math.color.ts:271

___

### copyFromFloats

▸ **copyFromFloats**(`r`, `g`, `b`): [`Color3`](Color3.md)

Updates the Color3 rgb values from the given floats

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `r` | `number` | defines the red component to read from |
| `g` | `number` | defines the green component to read from |
| `b` | `number` | defines the blue component to read from |

#### Returns

[`Color3`](Color3.md)

the current Color3 object

#### Defined in

packages/dev/core/src/Maths/math.color.ts:285

___

### equals

▸ **equals**(`otherColor`): `boolean`

Determines equality between Color3 objects

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherColor` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Color3`](Color3.md) | defines the second operand |

#### Returns

`boolean`

true if the rgb values are equal to the given ones

#### Defined in

packages/dev/core/src/Maths/math.color.ts:138

___

### equalsFloats

▸ **equalsFloats**(`r`, `g`, `b`): `boolean`

Determines equality between the current Color3 object and a set of r,b,g values

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `r` | `number` | defines the red component to check |
| `g` | `number` | defines the green component to check |
| `b` | `number` | defines the blue component to check |

#### Returns

`boolean`

true if the rgb values are equal to the given ones

#### Defined in

packages/dev/core/src/Maths/math.color.ts:149

___

### fromArray

▸ **fromArray**(`array`, `offset?`): [`Color3`](Color3.md)

Update the current color with values stored in an array from the starting index of the given array

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `array` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)`ArrayLike``number` | `undefined` | defines the source array |
| `offset` | `number` | `0` | defines an offset in the source array |

#### Returns

[`Color3`](Color3.md)

the current Color3 object

#### Defined in

packages/dev/core/src/Maths/math.color.ts:81

___

### getClassName

▸ **getClassName**(): `string`

Returns the string "Color3"

#### Returns

`string`

"Color3"

#### Defined in

packages/dev/core/src/Maths/math.color.ts:44

___

### getHashCode

▸ **getHashCode**(): `number`

Compute the Color3 hash code

#### Returns

`number`

an unique number that can be used to hash Color3 objects

#### Defined in

packages/dev/core/src/Maths/math.color.ts:52

___

### multiply

▸ **multiply**(`otherColor`): [`Color3`](Color3.md)

Multiply each Color3 rgb values by the given Color3 rgb values in a new Color3 object

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherColor` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Color3`](Color3.md) | defines the second operand |

#### Returns

[`Color3`](Color3.md)

the new Color3 object

#### Defined in

packages/dev/core/src/Maths/math.color.ts:116

___

### multiplyToRef

▸ **multiplyToRef**(`otherColor`, `result`): [`Color3`](Color3.md)

Multiply the rgb values of the Color3 and the given Color3 and stores the result in the object "result"

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherColor` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Color3`](Color3.md) | defines the second operand |
| `result` | [`Color3`](Color3.md) | defines the Color3 object where to store the result |

#### Returns

[`Color3`](Color3.md)

the current Color3

#### Defined in

packages/dev/core/src/Maths/math.color.ts:126

___

### scale

▸ **scale**(`scale`): [`Color3`](Color3.md)

Creates a new Color3 with the current Color3 values multiplied by scale

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scale` | `number` | defines the scaling factor to apply |

#### Returns

[`Color3`](Color3.md)

a new Color3 object

#### Defined in

packages/dev/core/src/Maths/math.color.ts:158

___

### scaleAndAddToRef

▸ **scaleAndAddToRef**(`scale`, `result`): [`Color3`](Color3.md)

Scale the current Color3 values by a factor and add the result to a given Color3

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scale` | `number` | defines the scale factor |
| `result` | [`Color3`](Color3.md) | defines color to store the result into |

#### Returns

[`Color3`](Color3.md)

the unmodified current Color3

#### Defined in

packages/dev/core/src/Maths/math.color.ts:193

___

### scaleInPlace

▸ **scaleInPlace**(`scale`): [`Color3`](Color3.md)

Multiplies the Color3 values by the float "scale"

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scale` | `number` | defines the scaling factor to apply |

#### Returns

[`Color3`](Color3.md)

the current updated Color3

#### Defined in

packages/dev/core/src/Maths/math.color.ts:167

___

### scaleToRef

▸ **scaleToRef**(`scale`, `result`): [`Color3`](Color3.md)

Multiplies the rgb values by scale and stores the result into "result"

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scale` | `number` | defines the scaling factor |
| `result` | [`Color3`](Color3.md) | defines the Color3 object where to store the result |

#### Returns

[`Color3`](Color3.md)

the unmodified current Color3

#### Defined in

packages/dev/core/src/Maths/math.color.ts:180

___

### set

▸ **set**(`r`, `g`, `b`): [`Color3`](Color3.md)

Updates the Color3 rgb values from the given floats

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `r` | `number` | defines the red component to read from |
| `g` | `number` | defines the green component to read from |
| `b` | `number` | defines the blue component to read from |

#### Returns

[`Color3`](Color3.md)

the current Color3 object

#### Defined in

packages/dev/core/src/Maths/math.color.ts:299

___

### subtract

▸ **subtract**(`otherColor`): [`Color3`](Color3.md)

Returns a new Color3 set with the subtracted values of the given one from the current Color3

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherColor` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Color3`](Color3.md) | defines the second operand |

#### Returns

[`Color3`](Color3.md)

the new Color3

#### Defined in

packages/dev/core/src/Maths/math.color.ts:241

___

### subtractToRef

▸ **subtractToRef**(`otherColor`, `result`): [`Color3`](Color3.md)

Stores the result of the subtraction of given one from the current Color3 rgb values into "result"

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherColor` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Color3`](Color3.md) | defines the second operand |
| `result` | [`Color3`](Color3.md) | defines Color3 object to store the result into |

#### Returns

[`Color3`](Color3.md)

the unmodified current Color3

#### Defined in

packages/dev/core/src/Maths/math.color.ts:251

___

### toArray

▸ **toArray**(`array`, `index?`): [`Color3`](Color3.md)

Stores in the given array from the given starting index the red, green, blue values as successive elements

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `array` | [`FloatArray`](../modules.md#floatarray) | `undefined` | defines the array where to store the r,g,b components |
| `index` | `number` | `0` | defines an optional index in the target array to define where to start storing values |

#### Returns

[`Color3`](Color3.md)

the current Color3 object

#### Defined in

packages/dev/core/src/Maths/math.color.ts:67

___

### toColor4

▸ **toColor4**(`alpha?`): [`Color4`](Color4.md)

Returns a new Color4 object from the current Color3 and the given alpha

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `alpha` | `number` | `1` | defines the alpha component on the new Color4 object (default is 1) |

#### Returns

[`Color4`](Color4.md)

a new Color4 object

#### Defined in

packages/dev/core/src/Maths/math.color.ts:91

___

### toGammaSpace

▸ **toGammaSpace**(): [`Color3`](Color3.md)

Computes a new Color3 converted from the current one to gamma space

#### Returns

[`Color3`](Color3.md)

a new Color3 object

#### Defined in

packages/dev/core/src/Maths/math.color.ts:392

___

### toGammaSpaceToRef

▸ **toGammaSpaceToRef**(`convertedColor`): [`Color3`](Color3.md)

Converts the Color3 values to gamma space and stores the result in "convertedColor"

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `convertedColor` | [`Color3`](Color3.md) | defines the Color3 object where to store the gamma space version |

#### Returns

[`Color3`](Color3.md)

the unmodified Color3

#### Defined in

packages/dev/core/src/Maths/math.color.ts:403

___

### toHSV

▸ **toHSV**(): [`Color3`](Color3.md)

Converts current color in rgb space to HSV values

#### Returns

[`Color3`](Color3.md)

a new color3 representing the HSV values

#### Defined in

packages/dev/core/src/Maths/math.color.ts:328

___

### toHSVToRef

▸ **toHSVToRef**(`result`): `void`

Converts current color in rgb space to HSV values

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `result` | [`Color3`](Color3.md) | defines the Color3 where to store the HSV values |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Maths/math.color.ts:340

___

### toHexString

▸ **toHexString**(): `string`

Compute the Color3 hexadecimal code as a string

#### Returns

`string`

a string containing the hexadecimal representation of the Color3 object

#### Defined in

packages/dev/core/src/Maths/math.color.ts:307

___

### toLinearSpace

▸ **toLinearSpace**(): [`Color3`](Color3.md)

Computes a new Color3 converted from the current one to linear space

#### Returns

[`Color3`](Color3.md)

a new Color3 object

#### Defined in

packages/dev/core/src/Maths/math.color.ts:318

___

### toLinearSpaceToRef

▸ **toLinearSpaceToRef**(`convertedColor`): [`Color3`](Color3.md)

Converts the Color3 values to linear space and stores the result in "convertedColor"

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `convertedColor` | [`Color3`](Color3.md) | defines the Color3 object where to store the linear space version |

#### Returns

[`Color3`](Color3.md)

the unmodified Color3

#### Defined in

packages/dev/core/src/Maths/math.color.ts:381

___

### toLuminance

▸ **toLuminance**(): `number`

Returns the luminance value

#### Returns

`number`

a float value

#### Defined in

packages/dev/core/src/Maths/math.color.ts:107

___

### toString

▸ **toString**(): `string`

Creates a string with the Color3 current values

#### Returns

`string`

the string representation of the Color3 object

#### Defined in

packages/dev/core/src/Maths/math.color.ts:36

___

### Black

▸ `Static` **Black**(): [`Color3`](Color3.md)

Returns a Color3 value containing a black color

#### Returns

[`Color3`](Color3.md)

a new Color3 object

#### Defined in

packages/dev/core/src/Maths/math.color.ts:637

___

### Blue

▸ `Static` **Blue**(): [`Color3`](Color3.md)

Returns a Color3 value containing a blue color

#### Returns

[`Color3`](Color3.md)

a new Color3 object

#### Defined in

packages/dev/core/src/Maths/math.color.ts:630

___

### FromArray

▸ `Static` **FromArray**(`array`, `offset?`): [`Color3`](Color3.md)

Creates a new Color3 from the starting index of the given array

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `array` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)`ArrayLike``number` | `undefined` | defines the source array |
| `offset` | `number` | `0` | defines an offset in the source array |

#### Returns

[`Color3`](Color3.md)

a new Color3 object

#### Defined in

packages/dev/core/src/Maths/math.color.ts:489

___

### FromArrayToRef

▸ `Static` **FromArrayToRef**(`array`, `offset?`, `result`): `void`

Creates a new Color3 from the starting index element of the given array

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `array` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)`ArrayLike``number` | `undefined` | defines the source array to read from |
| `offset` | `number` | `0` | defines the offset in the source array |
| `result` | [`Color3`](Color3.md) | `undefined` | defines the target Color3 object |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Maths/math.color.ts:499

___

### FromHSV

▸ `Static` **FromHSV**(`hue`, `saturation`, `value`): [`Color3`](Color3.md)

Converts Hue, saturation and value to a new Color3 (RGB)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `hue` | `number` | defines the hue |
| `saturation` | `number` | defines the saturation |
| `value` | `number` | defines the value |

#### Returns

[`Color3`](Color3.md)

a new Color3 object

#### Defined in

packages/dev/core/src/Maths/math.color.ts:460

___

### FromHexString

▸ `Static` **FromHexString**(`hex`): [`Color3`](Color3.md)

Creates a new Color3 from the string containing valid hexadecimal values

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `hex` | `string` | defines a string containing valid hexadecimal values |

#### Returns

[`Color3`](Color3.md)

a new Color3 object

#### Defined in

packages/dev/core/src/Maths/math.color.ts:471

___

### FromInts

▸ `Static` **FromInts**(`r`, `g`, `b`): [`Color3`](Color3.md)

Creates a new Color3 from integer values ( 256)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `r` | `number` | defines the red component to read from (value between 0 and 255) |
| `g` | `number` | defines the green component to read from (value between 0 and 255) |
| `b` | `number` | defines the blue component to read from (value between 0 and 255) |

#### Returns

[`Color3`](Color3.md)

a new Color3 object

#### Defined in

packages/dev/core/src/Maths/math.color.ts:512

___

### Gray

▸ `Static` **Gray**(): [`Color3`](Color3.md)

Returns a Color3 value containing a gray color

#### Returns

[`Color3`](Color3.md)

a new Color3 object

#### Defined in

packages/dev/core/src/Maths/math.color.ts:680

___

### Green

▸ `Static` **Green**(): [`Color3`](Color3.md)

Returns a Color3 value containing a green color

#### Returns

[`Color3`](Color3.md)

a new Color3 object

#### Defined in

packages/dev/core/src/Maths/math.color.ts:623

___

### HSVtoRGBToRef

▸ `Static` **HSVtoRGBToRef**(`hue`, `saturation`, `value`, `result`): `void`

Converts Hue, saturation and value to a Color3 (RGB)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `hue` | `number` | defines the hue |
| `saturation` | `number` | defines the saturation |
| `value` | `number` | defines the value |
| `result` | [`Color3`](Color3.md) | defines the Color3 where to store the RGB values |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Maths/math.color.ts:421

___

### Hermite

▸ `Static` **Hermite**(`value1`, `tangent1`, `value2`, `tangent2`, `amount`): [`Color3`](Color3.md)

Returns a new Color3 located for "amount" (float) on the Hermite interpolation spline defined by the vectors "value1", "tangent1", "value2", "tangent2"

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Color3`](Color3.md) | defines the first control point |
| `tangent1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Color3`](Color3.md) | defines the first tangent Color3 |
| `value2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Color3`](Color3.md) | defines the second control point |
| `tangent2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Color3`](Color3.md) | defines the second tangent Color3 |
| `amount` | `number` | defines the amount on the interpolation spline (between 0 and 1) |

#### Returns

[`Color3`](Color3.md)

the new Color3

#### Defined in

packages/dev/core/src/Maths/math.color.ts:551

___

### Hermite1stDerivative

▸ `Static` **Hermite1stDerivative**(`value1`, `tangent1`, `value2`, `tangent2`, `time`): [`Color3`](Color3.md)

Returns a new Color3 which is the 1st derivative of the Hermite spline defined by the colors "value1", "value2", "tangent1", "tangent2".

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Color3`](Color3.md) | defines the first control point |
| `tangent1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Color3`](Color3.md) | defines the first tangent |
| `value2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Color3`](Color3.md) | defines the second control point |
| `tangent2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Color3`](Color3.md) | defines the second tangent |
| `time` | `number` | define where the derivative must be done |

#### Returns

[`Color3`](Color3.md)

1st derivative

#### Defined in

packages/dev/core/src/Maths/math.color.ts:574

___

### Hermite1stDerivativeToRef

▸ `Static` **Hermite1stDerivativeToRef**(`value1`, `tangent1`, `value2`, `tangent2`, `time`, `result`): `void`

Returns a new Color3 which is the 1st derivative of the Hermite spline defined by the colors "value1", "value2", "tangent1", "tangent2".

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Color3`](Color3.md) | defines the first control point |
| `tangent1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Color3`](Color3.md) | defines the first tangent |
| `value2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Color3`](Color3.md) | defines the second control point |
| `tangent2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Color3`](Color3.md) | defines the second tangent |
| `time` | `number` | define where the derivative must be done |
| `result` | [`Color3`](Color3.md) | define where to store the derivative |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Maths/math.color.ts:597

___

### Lerp

▸ `Static` **Lerp**(`start`, `end`, `amount`): [`Color3`](Color3.md)

Creates a new Color3 with values linearly interpolated of "amount" between the start Color3 and the end Color3

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `start` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Color3`](Color3.md) | defines the start Color3 value |
| `end` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Color3`](Color3.md) | defines the end Color3 value |
| `amount` | `number` | defines the gradient value between start and end |

#### Returns

[`Color3`](Color3.md)

a new Color3 object

#### Defined in

packages/dev/core/src/Maths/math.color.ts:523

___

### LerpToRef

▸ `Static` **LerpToRef**(`left`, `right`, `amount`, `result`): `void`

Creates a new Color3 with values linearly interpolated of "amount" between the start Color3 and the end Color3

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `left` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Color3`](Color3.md) | defines the start value |
| `right` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Color3`](Color3.md) | defines the end value |
| `amount` | `number` | defines the gradient factor |
| `result` | [`Color3`](Color3.md) | defines the Color3 object where to store the result |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Maths/math.color.ts:536

___

### Magenta

▸ `Static` **Magenta**(): [`Color3`](Color3.md)

Returns a Color3 value containing a magenta color

#### Returns

[`Color3`](Color3.md)

a new Color3 object

#### Defined in

packages/dev/core/src/Maths/math.color.ts:666

___

### Purple

▸ `Static` **Purple**(): [`Color3`](Color3.md)

Returns a Color3 value containing a purple color

#### Returns

[`Color3`](Color3.md)

a new Color3 object

#### Defined in

packages/dev/core/src/Maths/math.color.ts:659

___

### Random

▸ `Static` **Random**(): [`Color3`](Color3.md)

Returns a Color3 value containing a random color

#### Returns

[`Color3`](Color3.md)

a new Color3 object

#### Defined in

packages/dev/core/src/Maths/math.color.ts:694

___

### Red

▸ `Static` **Red**(): [`Color3`](Color3.md)

Returns a Color3 value containing a red color

#### Returns

[`Color3`](Color3.md)

a new Color3 object

#### Defined in

packages/dev/core/src/Maths/math.color.ts:616

___

### Teal

▸ `Static` **Teal**(): [`Color3`](Color3.md)

Returns a Color3 value containing a teal color

#### Returns

[`Color3`](Color3.md)

a new Color3 object

#### Defined in

packages/dev/core/src/Maths/math.color.ts:687

___

### White

▸ `Static` **White**(): [`Color3`](Color3.md)

Returns a Color3 value containing a white color

#### Returns

[`Color3`](Color3.md)

a new Color3 object

#### Defined in

packages/dev/core/src/Maths/math.color.ts:652

___

### Yellow

▸ `Static` **Yellow**(): [`Color3`](Color3.md)

Returns a Color3 value containing a yellow color

#### Returns

[`Color3`](Color3.md)

a new Color3 object

#### Defined in

packages/dev/core/src/Maths/math.color.ts:673
