[@dev/core](../README.md) / [Exports](../modules.md) / Vector4

# Class: Vector4

Vector4 class created for EulerAngle class conversion to Quaternion

## Table of contents

### Constructors

- [constructor](Vector4.md#constructor)

### Properties

- [w](Vector4.md#w)
- [x](Vector4.md#x)
- [y](Vector4.md#y)
- [z](Vector4.md#z)

### Methods

- [add](Vector4.md#add)
- [addInPlace](Vector4.md#addinplace)
- [addToRef](Vector4.md#addtoref)
- [asArray](Vector4.md#asarray)
- [clone](Vector4.md#clone)
- [copyFrom](Vector4.md#copyfrom)
- [copyFromFloats](Vector4.md#copyfromfloats)
- [divide](Vector4.md#divide)
- [divideInPlace](Vector4.md#divideinplace)
- [divideToRef](Vector4.md#dividetoref)
- [equals](Vector4.md#equals)
- [equalsToFloats](Vector4.md#equalstofloats)
- [equalsWithEpsilon](Vector4.md#equalswithepsilon)
- [floor](Vector4.md#floor)
- [fract](Vector4.md#fract)
- [fromArray](Vector4.md#fromarray)
- [getClassName](Vector4.md#getclassname)
- [getHashCode](Vector4.md#gethashcode)
- [length](Vector4.md#length)
- [lengthSquared](Vector4.md#lengthsquared)
- [maximizeInPlace](Vector4.md#maximizeinplace)
- [minimizeInPlace](Vector4.md#minimizeinplace)
- [multiply](Vector4.md#multiply)
- [multiplyByFloats](Vector4.md#multiplybyfloats)
- [multiplyInPlace](Vector4.md#multiplyinplace)
- [multiplyToRef](Vector4.md#multiplytoref)
- [negate](Vector4.md#negate)
- [negateInPlace](Vector4.md#negateinplace)
- [negateToRef](Vector4.md#negatetoref)
- [normalize](Vector4.md#normalize)
- [scale](Vector4.md#scale)
- [scaleAndAddToRef](Vector4.md#scaleandaddtoref)
- [scaleInPlace](Vector4.md#scaleinplace)
- [scaleToRef](Vector4.md#scaletoref)
- [set](Vector4.md#set)
- [setAll](Vector4.md#setall)
- [subtract](Vector4.md#subtract)
- [subtractFromFloats](Vector4.md#subtractfromfloats)
- [subtractFromFloatsToRef](Vector4.md#subtractfromfloatstoref)
- [subtractInPlace](Vector4.md#subtractinplace)
- [subtractToRef](Vector4.md#subtracttoref)
- [toArray](Vector4.md#toarray)
- [toString](Vector4.md#tostring)
- [toVector3](Vector4.md#tovector3)
- [Center](Vector4.md#center)
- [CenterToRef](Vector4.md#centertoref)
- [Distance](Vector4.md#distance)
- [DistanceSquared](Vector4.md#distancesquared)
- [FromArray](Vector4.md#fromarray-1)
- [FromArrayToRef](Vector4.md#fromarraytoref)
- [FromFloatArrayToRef](Vector4.md#fromfloatarraytoref)
- [FromFloatsToRef](Vector4.md#fromfloatstoref)
- [FromVector3](Vector4.md#fromvector3)
- [Maximize](Vector4.md#maximize)
- [Minimize](Vector4.md#minimize)
- [Normalize](Vector4.md#normalize-1)
- [NormalizeToRef](Vector4.md#normalizetoref)
- [One](Vector4.md#one)
- [TransformCoordinates](Vector4.md#transformcoordinates)
- [TransformCoordinatesFromFloatsToRef](Vector4.md#transformcoordinatesfromfloatstoref)
- [TransformCoordinatesToRef](Vector4.md#transformcoordinatestoref)
- [TransformNormal](Vector4.md#transformnormal)
- [TransformNormalFromFloatsToRef](Vector4.md#transformnormalfromfloatstoref)
- [TransformNormalToRef](Vector4.md#transformnormaltoref)
- [Zero](Vector4.md#zero)

## Constructors

### constructor

• **new Vector4**(`x`, `y`, `z`, `w`)

Creates a Vector4 object from the given floats.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | x value of the vector |
| `y` | `number` | y value of the vector |
| `z` | `number` | z value of the vector |
| `w` | `number` | w value of the vector |

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:2637

## Properties

### w

• **w**: `number`

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:2645

___

### x

• **x**: `number`

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:2639

___

### y

• **y**: `number`

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:2641

___

### z

• **z**: `number`

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:2643

## Methods

### add

▸ **add**(`otherVector`): [`Vector4`](Vector4.md)

Returns a new Vector4 as the result of the addition of the current Vector4 and the given one.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherVector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector4`](Vector4.md) | the vector to add |

#### Returns

[`Vector4`](Vector4.md)

the resulting vector

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:2740

___

### addInPlace

▸ **addInPlace**(`otherVector`): [`Vector4`](Vector4.md)

Adds the given vector to the current Vector4.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherVector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector4`](Vector4.md) | the vector to add |

#### Returns

[`Vector4`](Vector4.md)

the updated Vector4.

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:2727

___

### addToRef

▸ **addToRef**(`otherVector`, `result`): [`Vector4`](Vector4.md)

Updates the given vector "result" with the result of the addition of the current Vector4 and the given one.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherVector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector4`](Vector4.md) | the vector to add |
| `result` | [`Vector4`](Vector4.md) | the vector to store the result |

#### Returns

[`Vector4`](Vector4.md)

the current Vector4.

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:2750

___

### asArray

▸ **asArray**(): `number`[]

Returns a new array populated with 4 elements : the Vector4 coordinates.

#### Returns

`number`[]

the resulting array

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:2686

___

### clone

▸ **clone**(): [`Vector4`](Vector4.md)

Returns a new Vector4 copied from the current one.

#### Returns

[`Vector4`](Vector4.md)

the new cloned vector

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:3117

___

### copyFrom

▸ **copyFrom**(`source`): [`Vector4`](Vector4.md)

Updates the current Vector4 with the given one coordinates.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector4`](Vector4.md) | the source vector to copy from |

#### Returns

[`Vector4`](Vector4.md)

the updated Vector4.

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:3125

___

### copyFromFloats

▸ **copyFromFloats**(`x`, `y`, `z`, `w`): [`Vector4`](Vector4.md)

Updates the current Vector4 coordinates with the given floats.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | float to copy from |
| `y` | `number` | float to copy from |
| `z` | `number` | float to copy from |
| `w` | `number` | float to copy from |

#### Returns

[`Vector4`](Vector4.md)

the updated Vector4.

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:3140

___

### divide

▸ **divide**(`otherVector`): [`Vector4`](Vector4.md)

Returns a new Vector4 set with the division result of the current Vector4 by the given one.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherVector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector4`](Vector4.md) | vector to devide with |

#### Returns

[`Vector4`](Vector4.md)

resulting new vector

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:2992

___

### divideInPlace

▸ **divideInPlace**(`otherVector`): [`Vector4`](Vector4.md)

Divides the current Vector3 coordinates by the given ones.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherVector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector4`](Vector4.md) | vector to devide with |

#### Returns

[`Vector4`](Vector4.md)

the updated Vector3.

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:3014

___

### divideToRef

▸ **divideToRef**(`otherVector`, `result`): [`Vector4`](Vector4.md)

Updates the given vector "result" with the division result of the current Vector4 by the given one.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherVector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector4`](Vector4.md) | vector to devide with |
| `result` | [`Vector4`](Vector4.md) | vector to store the result |

#### Returns

[`Vector4`](Vector4.md)

the current Vector4.

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:3001

___

### equals

▸ **equals**(`otherVector`): `boolean`

Boolean : True if the current Vector4 coordinates are stricly equal to the given ones.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherVector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector4`](Vector4.md) | the vector to compare against |

#### Returns

`boolean`

true if they are equal

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:2910

___

### equalsToFloats

▸ **equalsToFloats**(`x`, `y`, `z`, `w`): `boolean`

Boolean : True if the given floats are strictly equal to the current Vector4 coordinates.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | x value to compare against |
| `y` | `number` | y value to compare against |
| `z` | `number` | z value to compare against |
| `w` | `number` | w value to compare against |

#### Returns

`boolean`

true if equal

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:2938

___

### equalsWithEpsilon

▸ **equalsWithEpsilon**(`otherVector`, `epsilon?`): `boolean`

Boolean : True if the current Vector4 coordinates are each beneath the distance "epsilon" from the given vector ones.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `otherVector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector4`](Vector4.md) | `undefined` | vector to compare against |
| `epsilon` | `number` | `Epsilon` | (Default: very small number) |

#### Returns

`boolean`

true if they are equal

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:2920

___

### floor

▸ **floor**(): [`Vector4`](Vector4.md)

Gets a new Vector4 from current Vector4 floored values

#### Returns

[`Vector4`](Vector4.md)

a new Vector4

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:3063

___

### fract

▸ **fract**(): [`Vector4`](Vector4.md)

Gets a new Vector4 from current Vector3 floored values

#### Returns

[`Vector4`](Vector4.md)

a new Vector4

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:3071

___

### fromArray

▸ **fromArray**(`array`, `index?`): [`Vector4`](Vector4.md)

Update the current vector from an array

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `array` | [`FloatArray`](../modules.md#floatarray) | `undefined` | defines the destination array |
| `index` | `number` | `0` | defines the offset in the destination array |

#### Returns

[`Vector4`](Vector4.md)

the current Vector3

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:2717

___

### getClassName

▸ **getClassName**(): `string`

Returns the string "Vector4".

#### Returns

`string`

"Vector4"

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:2660

___

### getHashCode

▸ **getHashCode**(): `number`

Returns the Vector4 hash code.

#### Returns

`number`

a unique hash code

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:2668

___

### length

▸ **length**(): `number`

Returns the Vector4 length (float).

#### Returns

`number`

the length

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:3080

___

### lengthSquared

▸ **lengthSquared**(): `number`

Returns the Vector4 squared length (float).

#### Returns

`number`

the length squared

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:3087

___

### maximizeInPlace

▸ **maximizeInPlace**(`other`): [`Vector4`](Vector4.md)

Updates the Vector4 coordinates with the maximum values between its own and the given vector ones

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector4`](Vector4.md) | defines the second operand |

#### Returns

[`Vector4`](Vector4.md)

the current updated Vector4

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:3043

___

### minimizeInPlace

▸ **minimizeInPlace**(`other`): [`Vector4`](Vector4.md)

Updates the Vector4 coordinates with the minimum values between its own and the given vector ones

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector4`](Vector4.md) | defines the second operand |

#### Returns

[`Vector4`](Vector4.md)

the current updated Vector4

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:3023

___

### multiply

▸ **multiply**(`otherVector`): [`Vector4`](Vector4.md)

Returns a new Vector4 set with the multiplication result of the current Vector4 and the given one.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherVector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector4`](Vector4.md) | vector to multiple with |

#### Returns

[`Vector4`](Vector4.md)

resulting new vector

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:2960

___

### multiplyByFloats

▸ **multiplyByFloats**(`x`, `y`, `z`, `w`): [`Vector4`](Vector4.md)

Returns a new Vector4 set with the multiplication result of the given floats and the current Vector4 coordinates.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | x value multiply with |
| `y` | `number` | y value multiply with |
| `z` | `number` | z value multiply with |
| `w` | `number` | w value multiply with |

#### Returns

[`Vector4`](Vector4.md)

resulting new vector

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:2984

___

### multiplyInPlace

▸ **multiplyInPlace**(`otherVector`): [`Vector4`](Vector4.md)

Multiplies in place the current Vector4 by the given one.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherVector` | [`Vector4`](Vector4.md) | vector to multiple with |

#### Returns

[`Vector4`](Vector4.md)

the updated Vector4.

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:2947

___

### multiplyToRef

▸ **multiplyToRef**(`otherVector`, `result`): [`Vector4`](Vector4.md)

Updates the given vector "result" with the multiplication result of the current Vector4 and the given one.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherVector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector4`](Vector4.md) | vector to multiple with |
| `result` | [`Vector4`](Vector4.md) | vector to store the result |

#### Returns

[`Vector4`](Vector4.md)

the current Vector4.

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:2969

___

### negate

▸ **negate**(): [`Vector4`](Vector4.md)

Returns a new Vector4 set with the current Vector4 negated coordinates.

#### Returns

[`Vector4`](Vector4.md)

a new vector with the negated values

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:2830

___

### negateInPlace

▸ **negateInPlace**(): [`Vector4`](Vector4.md)

Negate this vector in place

#### Returns

[`Vector4`](Vector4.md)

this

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:2838

___

### negateToRef

▸ **negateToRef**(`result`): [`Vector4`](Vector4.md)

Negate the current Vector4 and stores the result in the given vector "result" coordinates

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `result` | [`Vector4`](Vector4.md) | defines the Vector3 object where to store the result |

#### Returns

[`Vector4`](Vector4.md)

the current Vector4

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:2851

___

### normalize

▸ **normalize**(): [`Vector4`](Vector4.md)

Normalizes in place the Vector4.

#### Returns

[`Vector4`](Vector4.md)

the updated Vector4.

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:3096

___

### scale

▸ **scale**(`scale`): [`Vector4`](Vector4.md)

Returns a new Vector4 set with the current Vector4 coordinates multiplied by scale (float).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scale` | `number` | the number to scale with |

#### Returns

[`Vector4`](Vector4.md)

a new vector with the result

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:2873

___

### scaleAndAddToRef

▸ **scaleAndAddToRef**(`scale`, `result`): [`Vector4`](Vector4.md)

Scale the current Vector4 values by a factor and add the result to a given Vector4

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scale` | `number` | defines the scale factor |
| `result` | [`Vector4`](Vector4.md) | defines the Vector4 object where to store the result |

#### Returns

[`Vector4`](Vector4.md)

the unmodified current Vector4

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:2897

___

### scaleInPlace

▸ **scaleInPlace**(`scale`): [`Vector4`](Vector4.md)

Multiplies the current Vector4 coordinates by scale (float).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scale` | `number` | the number to scale with |

#### Returns

[`Vector4`](Vector4.md)

the updated Vector4.

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:2860

___

### scaleToRef

▸ **scaleToRef**(`scale`, `result`): [`Vector4`](Vector4.md)

Sets the given vector "result" with the current Vector4 coordinates multiplied by scale (float).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scale` | `number` | the number to scale with |
| `result` | [`Vector4`](Vector4.md) | a vector to store the result in |

#### Returns

[`Vector4`](Vector4.md)

the current Vector4.

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:2883

___

### set

▸ **set**(`x`, `y`, `z`, `w`): [`Vector4`](Vector4.md)

Updates the current Vector4 coordinates with the given floats.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | float to set from |
| `y` | `number` | float to set from |
| `z` | `number` | float to set from |
| `w` | `number` | float to set from |

#### Returns

[`Vector4`](Vector4.md)

the updated Vector4.

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:3155

___

### setAll

▸ **setAll**(`v`): [`Vector4`](Vector4.md)

Copies the given float to the current Vector3 coordinates

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `v` | `number` | defines the x, y, z and w coordinates of the operand |

#### Returns

[`Vector4`](Vector4.md)

the current updated Vector3

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:3164

___

### subtract

▸ **subtract**(`otherVector`): [`Vector4`](Vector4.md)

Returns a new Vector4 with the result of the subtraction of the given vector from the current Vector4.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherVector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector4`](Vector4.md) | the vector to add |

#### Returns

[`Vector4`](Vector4.md)

the new vector with the result

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:2776

___

### subtractFromFloats

▸ **subtractFromFloats**(`x`, `y`, `z`, `w`): [`Vector4`](Vector4.md)

Returns a new Vector4 set with the result of the subtraction of the given floats from the current Vector4 coordinates.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | value to subtract |
| `y` | `number` | value to subtract |
| `z` | `number` | value to subtract |
| `w` | `number` | value to subtract |

#### Returns

[`Vector4`](Vector4.md)

new vector containing the result

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:2805

___

### subtractFromFloatsToRef

▸ **subtractFromFloatsToRef**(`x`, `y`, `z`, `w`, `result`): [`Vector4`](Vector4.md)

Sets the given vector "result" set with the result of the subtraction of the given floats from the current Vector4 coordinates.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | value to subtract |
| `y` | `number` | value to subtract |
| `z` | `number` | value to subtract |
| `w` | `number` | value to subtract |
| `result` | [`Vector4`](Vector4.md) | the vector to store the result in |

#### Returns

[`Vector4`](Vector4.md)

the current Vector4.

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:2818

___

### subtractInPlace

▸ **subtractInPlace**(`otherVector`): [`Vector4`](Vector4.md)

Subtract in place the given vector from the current Vector4.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherVector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector4`](Vector4.md) | the vector to subtract |

#### Returns

[`Vector4`](Vector4.md)

the updated Vector4.

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:2763

___

### subtractToRef

▸ **subtractToRef**(`otherVector`, `result`): [`Vector4`](Vector4.md)

Sets the given vector "result" with the result of the subtraction of the given vector from the current Vector4.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherVector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector4`](Vector4.md) | the vector to subtract |
| `result` | [`Vector4`](Vector4.md) | the vector to store the result |

#### Returns

[`Vector4`](Vector4.md)

the current Vector4.

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:2786

___

### toArray

▸ **toArray**(`array`, `index?`): [`Vector4`](Vector4.md)

Populates the given array from the given index with the Vector4 coordinates.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `array` | [`FloatArray`](../modules.md#floatarray) | array to populate |
| `index?` | `number` | index of the array to start at (default: 0) |

#### Returns

[`Vector4`](Vector4.md)

the Vector4.

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:2700

___

### toString

▸ **toString**(): `string`

Returns the string with the Vector4 coordinates.

#### Returns

`string`

a string containing all the vector values

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:2652

___

### toVector3

▸ **toVector3**(): [`Vector3`](Vector3.md)

Returns a new Vector3 from the Vector4 (x, y, z) coordinates.

#### Returns

[`Vector3`](Vector3.md)

this converted to a new vector3

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:3110

___

### Center

▸ `Static` **Center**(`value1`, `value2`): [`Vector4`](Vector4.md)

Returns a new Vector4 located at the center between the vectors "value1" and "value2".

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector4`](Vector4.md) | value to calulate the center between |
| `value2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector4`](Vector4.md) | value to calulate the center between |

#### Returns

[`Vector4`](Vector4.md)

the center between the two vectors

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:3303

___

### CenterToRef

▸ `Static` **CenterToRef**(`value1`, `value2`, `ref`): [`Vector4`](Vector4.md)

Gets the center of the vectors "value1" and "value2" and stores the result in the vector "ref"

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector4`](Vector4.md) | defines first vector |
| `value2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector4`](Vector4.md) | defines second vector |
| `ref` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector4`](Vector4.md) | defines third vector |

#### Returns

[`Vector4`](Vector4.md)

ref

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:3314

___

### Distance

▸ `Static` **Distance**(`value1`, `value2`): `number`

Returns the distance (float) between the vectors "value1" and "value2".

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector4`](Vector4.md) | value to calulate the distance between |
| `value2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector4`](Vector4.md) | value to calulate the distance between |

#### Returns

`number`

the distance between the two vectors

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:3280

___

### DistanceSquared

▸ `Static` **DistanceSquared**(`value1`, `value2`): `number`

Returns the squared distance (float) between the vectors "value1" and "value2".

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector4`](Vector4.md) | value to calulate the distance between |
| `value2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector4`](Vector4.md) | value to calulate the distance between |

#### Returns

`number`

the distance between the two vectors squared

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:3289

___

### FromArray

▸ `Static` **FromArray**(`array`, `offset?`): [`Vector4`](Vector4.md)

Returns a new Vector4 set from the starting index of the given array.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `array` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)`ArrayLike``number` | the array to pull values from |
| `offset?` | `number` | the offset into the array to start at |

#### Returns

[`Vector4`](Vector4.md)

the new vector

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:3176

___

### FromArrayToRef

▸ `Static` **FromArrayToRef**(`array`, `offset`, `result`): `void`

Updates the given vector "result" from the starting index of the given array.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `array` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)`ArrayLike``number` | the array to pull values from |
| `offset` | `number` | the offset into the array to start at |
| `result` | [`Vector4`](Vector4.md) | the vector to store the result in |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:3188

___

### FromFloatArrayToRef

▸ `Static` **FromFloatArrayToRef**(`array`, `offset`, `result`): `void`

Updates the given vector "result" from the starting index of the given Float32Array.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `array` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)`Float32Array` | the array to pull values from |
| `offset` | `number` | the offset into the array to start at |
| `result` | [`Vector4`](Vector4.md) | the vector to store the result in |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:3200

___

### FromFloatsToRef

▸ `Static` **FromFloatsToRef**(`x`, `y`, `z`, `w`, `result`): `void`

Updates the given vector "result" coordinates from the given floats.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | float to set from |
| `y` | `number` | float to set from |
| `z` | `number` | float to set from |
| `w` | `number` | float to set from |
| `result` | [`Vector4`](Vector4.md) | the vector to the floats in |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:3211

___

### FromVector3

▸ `Static` **FromVector3**(`source`, `w?`): [`Vector4`](Vector4.md)

Creates a new Vector4 from a Vector3

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `source` | [`Vector3`](Vector3.md) | `undefined` | defines the source data |
| `w` | `number` | `0` | defines the 4th component (default is 0) |

#### Returns

[`Vector4`](Vector4.md)

a new Vector4

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:3422

___

### Maximize

▸ `Static` **Maximize**(`left`, `right`): [`Vector4`](Vector4.md)

Returns a vector with the maximum values from the left and right vectors

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `left` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector4`](Vector4.md) | left vector to maximize |
| `right` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector4`](Vector4.md) | right vector to maximize |

#### Returns

[`Vector4`](Vector4.md)

a new vector with the maximum of the left and right vector values

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:3269

___

### Minimize

▸ `Static` **Minimize**(`left`, `right`): [`Vector4`](Vector4.md)

Returns a vector with the minimum values from the left and right vectors

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `left` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector4`](Vector4.md) | left vector to minimize |
| `right` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector4`](Vector4.md) | right vector to minimize |

#### Returns

[`Vector4`](Vector4.md)

a new vector with the minimum of the left and right vector values

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:3257

___

### Normalize

▸ `Static` **Normalize**(`vector`): [`Vector4`](Vector4.md)

Returns a new normalized Vector4 from the given one.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector4`](Vector4.md) | the vector to normalize |

#### Returns

[`Vector4`](Vector4.md)

the vector

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:3236

___

### NormalizeToRef

▸ `Static` **NormalizeToRef**(`vector`, `result`): `void`

Updates the given vector "result" from the normalization of the given one.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector4`](Vector4.md) | the vector to normalize |
| `result` | [`Vector4`](Vector4.md) | the vector to store the result in |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:3246

___

### One

▸ `Static` **One**(): [`Vector4`](Vector4.md)

Returns a new Vector4 set to (1.0, 1.0, 1.0, 1.0)

#### Returns

[`Vector4`](Vector4.md)

the new vector

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:3228

___

### TransformCoordinates

▸ `Static` **TransformCoordinates**(`vector`, `transformation`): [`Vector4`](Vector4.md)

Returns a new Vector4 set with the result of the transformation by the given matrix of the given vector.
This method computes tranformed coordinates only, not transformed direction vectors (ie. it takes translation in account)
The difference with Vector3.TransformCoordinates is that the w component is not used to divide the other coordinates but is returned in the w coordinate instead

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the Vector3 to transform |
| `transformation` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the transformation matrix |

#### Returns

[`Vector4`](Vector4.md)

the transformed Vector4

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:3326

___

### TransformCoordinatesFromFloatsToRef

▸ `Static` **TransformCoordinatesFromFloatsToRef**(`x`, `y`, `z`, `transformation`, `result`): `void`

Sets the given vector "result" coordinates with the result of the transformation by the given matrix of the given floats (x, y, z)
This method computes tranformed coordinates only, not transformed direction vectors
The difference with Vector3.TransformCoordinatesFromFloatsToRef is that the w component is not used to divide the other coordinates but is returned in the w coordinate instead

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | define the x coordinate of the source vector |
| `y` | `number` | define the y coordinate of the source vector |
| `z` | `number` | define the z coordinate of the source vector |
| `transformation` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the transformation matrix |
| `result` | [`Vector4`](Vector4.md) | defines the Vector4 where to store the result |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:3354

___

### TransformCoordinatesToRef

▸ `Static` **TransformCoordinatesToRef**(`vector`, `transformation`, `result`): `void`

Sets the given vector "result" coordinates with the result of the transformation by the given matrix of the given vector
This method computes tranformed coordinates only, not transformed direction vectors (ie. it takes translation in account)
The difference with Vector3.TransformCoordinatesToRef is that the w component is not used to divide the other coordinates but is returned in the w coordinate instead

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the Vector3 to transform |
| `transformation` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the transformation matrix |
| `result` | [`Vector4`](Vector4.md) | defines the Vector4 where to store the result |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:3340

___

### TransformNormal

▸ `Static` **TransformNormal**(`vector`, `transformation`): [`Vector4`](Vector4.md)

Returns a new Vector4 set with the result of the normal transformation by the given matrix of the given vector.
This methods computes transformed normalized direction vectors only.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector4`](Vector4.md) | the vector to transform |
| `transformation` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | the transformation matrix to apply |

#### Returns

[`Vector4`](Vector4.md)

the new vector

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:3374

___

### TransformNormalFromFloatsToRef

▸ `Static` **TransformNormalFromFloatsToRef**(`x`, `y`, `z`, `w`, `transformation`, `result`): `void`

Sets the given vector "result" with the result of the normal transformation by the given matrix of the given floats (x, y, z, w).
This methods computes transformed normalized direction vectors only.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | value to transform |
| `y` | `number` | value to transform |
| `z` | `number` | value to transform |
| `w` | `number` | value to transform |
| `transformation` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | the transformation matrix to apply |
| `result` | [`Vector4`](Vector4.md) | the vector to store the results in |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:3408

___

### TransformNormalToRef

▸ `Static` **TransformNormalToRef**(`vector`, `transformation`, `result`): `void`

Sets the given vector "result" with the result of the normal transformation by the given matrix of the given vector.
This methods computes transformed normalized direction vectors only.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector4`](Vector4.md) | the vector to transform |
| `transformation` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | the transformation matrix to apply |
| `result` | [`Vector4`](Vector4.md) | the vector to store the result in |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:3387

___

### Zero

▸ `Static` **Zero**(): [`Vector4`](Vector4.md)

Returns a new Vector4 set to (0.0, 0.0, 0.0, 0.0)

#### Returns

[`Vector4`](Vector4.md)

the new vector

#### Defined in

packages/dev/core/src/Maths/math.vector.ts:3221
