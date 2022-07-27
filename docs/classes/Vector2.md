[@dev/core](../README.md) / [Exports](../modules.md) / Vector2

# Class: Vector2

Class representing a vector containing 2 coordinates

## Table of contents

### Constructors

- [constructor](Vector2.md#constructor)

### Properties

- [x](Vector2.md#x)
- [y](Vector2.md#y)

### Methods

- [add](Vector2.md#add)
- [addInPlace](Vector2.md#addinplace)
- [addToRef](Vector2.md#addtoref)
- [addVector3](Vector2.md#addvector3)
- [asArray](Vector2.md#asarray)
- [clone](Vector2.md#clone)
- [copyFrom](Vector2.md#copyfrom)
- [copyFromFloats](Vector2.md#copyfromfloats)
- [divide](Vector2.md#divide)
- [divideInPlace](Vector2.md#divideinplace)
- [divideToRef](Vector2.md#dividetoref)
- [equals](Vector2.md#equals)
- [equalsWithEpsilon](Vector2.md#equalswithepsilon)
- [floor](Vector2.md#floor)
- [fract](Vector2.md#fract)
- [fromArray](Vector2.md#fromarray)
- [getClassName](Vector2.md#getclassname)
- [getHashCode](Vector2.md#gethashcode)
- [length](Vector2.md#length)
- [lengthSquared](Vector2.md#lengthsquared)
- [multiply](Vector2.md#multiply)
- [multiplyByFloats](Vector2.md#multiplybyfloats)
- [multiplyInPlace](Vector2.md#multiplyinplace)
- [multiplyToRef](Vector2.md#multiplytoref)
- [negate](Vector2.md#negate)
- [negateInPlace](Vector2.md#negateinplace)
- [negateToRef](Vector2.md#negatetoref)
- [normalize](Vector2.md#normalize)
- [rotateToRef](Vector2.md#rotatetoref)
- [scale](Vector2.md#scale)
- [scaleAndAddToRef](Vector2.md#scaleandaddtoref)
- [scaleInPlace](Vector2.md#scaleinplace)
- [scaleToRef](Vector2.md#scaletoref)
- [set](Vector2.md#set)
- [subtract](Vector2.md#subtract)
- [subtractInPlace](Vector2.md#subtractinplace)
- [subtractToRef](Vector2.md#subtracttoref)
- [toArray](Vector2.md#toarray)
- [toString](Vector2.md#tostring)
- [CatmullRom](Vector2.md#catmullrom)
- [Center](Vector2.md#center)
- [CenterToRef](Vector2.md#centertoref)
- [Clamp](Vector2.md#clamp)
- [Distance](Vector2.md#distance)
- [DistanceOfPointFromSegment](Vector2.md#distanceofpointfromsegment)
- [DistanceSquared](Vector2.md#distancesquared)
- [Dot](Vector2.md#dot)
- [FromArray](Vector2.md#fromarray-1)
- [FromArrayToRef](Vector2.md#fromarraytoref)
- [Hermite](Vector2.md#hermite)
- [Hermite1stDerivative](Vector2.md#hermite1stderivative)
- [Hermite1stDerivativeToRef](Vector2.md#hermite1stderivativetoref)
- [Lerp](Vector2.md#lerp)
- [Maximize](Vector2.md#maximize)
- [Minimize](Vector2.md#minimize)
- [Normalize](Vector2.md#normalize-1)
- [NormalizeToRef](Vector2.md#normalizetoref)
- [One](Vector2.md#one)
- [PointInTriangle](Vector2.md#pointintriangle)
- [Transform](Vector2.md#transform)
- [TransformToRef](Vector2.md#transformtoref)
- [Zero](Vector2.md#zero)

## Constructors

### constructor

• **new Vector2**(`x?`, `y?`)

Creates a new Vector2 from the given x and y coordinates

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `x` | `number` | `0` | defines the first coordinate |
| `y` | `number` | `0` | defines the second coordinate |

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:29

## Properties

### x

• **x**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:31

___

### y

• **y**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:33

## Methods

### add

▸ **add**(`otherVector`): [`Vector2`](Vector2.md)

Add another vector with the current one

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherVector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines the other vector |

#### Returns

[`Vector2`](Vector2.md)

a new Vector2 set with the addition of the current Vector2 and the given one coordinates

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:136

___

### addInPlace

▸ **addInPlace**(`otherVector`): [`Vector2`](Vector2.md)

Set the Vector2 coordinates by adding the given Vector2 coordinates

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherVector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines the other vector |

#### Returns

[`Vector2`](Vector2.md)

the current updated Vector2

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:157

___

### addToRef

▸ **addToRef**(`otherVector`, `result`): [`Vector2`](Vector2.md)

Sets the "result" coordinates with the addition of the current Vector2 and the given one coordinates

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherVector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines the other vector |
| `result` | [`Vector2`](Vector2.md) | defines the target vector |

#### Returns

[`Vector2`](Vector2.md)

the unmodified current Vector2

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:146

___

### addVector3

▸ **addVector3**(`otherVector`): [`Vector2`](Vector2.md)

Gets a new Vector2 by adding the current Vector2 coordinates to the given Vector3 x, y coordinates

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherVector` | [`Vector3`](Vector3.md) | defines the other vector |

#### Returns

[`Vector2`](Vector2.md)

a new Vector2

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:168

___

### asArray

▸ **asArray**(): `number`[]

Copy the current vector to an array

#### Returns

`number`[]

a new array with 2 elements: the Vector2 coordinates.

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:93

___

### clone

▸ **clone**(): [`Vector2`](Vector2.md)

Gets a new Vector2 copied from the Vector2

#### Returns

[`Vector2`](Vector2.md)

a new Vector2

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:433

___

### copyFrom

▸ **copyFrom**(`source`): [`Vector2`](Vector2.md)

Sets the Vector2 coordinates with the given Vector2 coordinates

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines the source Vector2 |

#### Returns

[`Vector2`](Vector2.md)

the current updated Vector2

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:104

___

### copyFromFloats

▸ **copyFromFloats**(`x`, `y`): [`Vector2`](Vector2.md)

Sets the Vector2 coordinates with the given floats

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | defines the first coordinate |
| `y` | `number` | defines the second coordinate |

#### Returns

[`Vector2`](Vector2.md)

the current updated Vector2

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:116

___

### divide

▸ **divide**(`otherVector`): [`Vector2`](Vector2.md)

Returns a new Vector2 set with the Vector2 coordinates divided by the given one coordinates

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherVector` | [`Vector2`](Vector2.md) | defines the other vector |

#### Returns

[`Vector2`](Vector2.md)

a new Vector2

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:250

___

### divideInPlace

▸ **divideInPlace**(`otherVector`): [`Vector2`](Vector2.md)

Divides the current Vector2 coordinates by the given ones

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherVector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines the other vector |

#### Returns

[`Vector2`](Vector2.md)

the current updated Vector2

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:271

___

### divideToRef

▸ **divideToRef**(`otherVector`, `result`): [`Vector2`](Vector2.md)

Sets the "result" coordinates with the Vector2 divided by the given one coordinates

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherVector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines the other vector |
| `result` | [`Vector2`](Vector2.md) | defines the target vector |

#### Returns

[`Vector2`](Vector2.md)

the unmodified current Vector2

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:260

___

### equals

▸ **equals**(`otherVector`): `boolean`

Gets a boolean if two vectors are equals

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherVector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines the other vector |

#### Returns

`boolean`

true if the given vector coordinates strictly equal the current Vector2 ones

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:353

___

### equalsWithEpsilon

▸ **equalsWithEpsilon**(`otherVector`, `epsilon?`): `boolean`

Gets a boolean if two vectors are equals (using an epsilon value)

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `otherVector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | `undefined` | defines the other vector |
| `epsilon` | `number` | `Epsilon` | defines the minimal distance to consider equality |

#### Returns

`boolean`

true if the given vector coordinates are close to the current ones by a distance of epsilon.

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:363

___

### floor

▸ **floor**(): [`Vector2`](Vector2.md)

Gets a new Vector2 from current Vector2 floored values
eg (1.2, 2.31) returns (1, 2)

#### Returns

[`Vector2`](Vector2.md)

a new Vector2

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:372

___

### fract

▸ **fract**(): [`Vector2`](Vector2.md)

Gets a new Vector2 from current Vector2 fractional values
eg (1.2, 2.31) returns (0.2, 0.31)

#### Returns

[`Vector2`](Vector2.md)

a new Vector2

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:381

___

### fromArray

▸ **fromArray**(`array`, `index?`): [`Vector2`](Vector2.md)

Update the current vector from an array

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `array` | [`FloatArray`](../modules.md#floatarray) | `undefined` | defines the destination array |
| `index` | `number` | `0` | defines the offset in the destination array |

#### Returns

[`Vector2`](Vector2.md)

the current Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:84

___

### getClassName

▸ **getClassName**(): `string`

Gets class name

#### Returns

`string`

the string "Vector2"

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:48

___

### getHashCode

▸ **getHashCode**(): `number`

Gets current vector hash code

#### Returns

`number`

the Vector2 hash code as a number

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:56

___

### length

▸ **length**(): `number`

Gets the length of the vector

#### Returns

`number`

the vector length (float)

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:406

___

### lengthSquared

▸ **lengthSquared**(): `number`

Gets the vector squared length

#### Returns

`number`

the vector squared length (float)

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:414

___

### multiply

▸ **multiply**(`otherVector`): [`Vector2`](Vector2.md)

Returns a new Vector2 set with the multiplication of the current Vector2 and the given one coordinates

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherVector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines the other vector |

#### Returns

[`Vector2`](Vector2.md)

a new Vector2

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:219

___

### multiplyByFloats

▸ **multiplyByFloats**(`x`, `y`): [`Vector2`](Vector2.md)

Gets a new Vector2 set with the Vector2 coordinates multiplied by the given floats

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | defines the first coordinate |
| `y` | `number` | defines the second coordinate |

#### Returns

[`Vector2`](Vector2.md)

a new Vector2

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:241

___

### multiplyInPlace

▸ **multiplyInPlace**(`otherVector`): [`Vector2`](Vector2.md)

Multiplies in place the current Vector2 coordinates by the given ones

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherVector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines the other vector |

#### Returns

[`Vector2`](Vector2.md)

the current updated Vector2

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:208

___

### multiplyToRef

▸ **multiplyToRef**(`otherVector`, `result`): [`Vector2`](Vector2.md)

Sets "result" coordinates with the multiplication of the current Vector2 and the given one coordinates

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherVector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines the other vector |
| `result` | [`Vector2`](Vector2.md) | defines the target vector |

#### Returns

[`Vector2`](Vector2.md)

the unmodified current Vector2

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:229

___

### negate

▸ **negate**(): [`Vector2`](Vector2.md)

Gets a new Vector2 with current Vector2 negated coordinates

#### Returns

[`Vector2`](Vector2.md)

a new Vector2

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:279

___

### negateInPlace

▸ **negateInPlace**(): [`Vector2`](Vector2.md)

Negate this vector in place

#### Returns

[`Vector2`](Vector2.md)

this

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:287

___

### negateToRef

▸ **negateToRef**(`result`): [`Vector2`](Vector2.md)

Negate the current Vector2 and stores the result in the given vector "result" coordinates

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `result` | [`Vector2`](Vector2.md) | defines the Vector3 object where to store the result |

#### Returns

[`Vector2`](Vector2.md)

the current Vector2

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:298

___

### normalize

▸ **normalize**(): [`Vector2`](Vector2.md)

Normalize the vector

#### Returns

[`Vector2`](Vector2.md)

the current updated Vector2

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:424

___

### rotateToRef

▸ **rotateToRef**(`angle`, `result`): [`Vector2`](Vector2.md)

Rotate the current vector into a given result vector

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `angle` | `number` | defines the rotation angle |
| `result` | [`Vector2`](Vector2.md) | defines the result vector where to store the rotated vector |

#### Returns

[`Vector2`](Vector2.md)

the current vector

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:391

___

### scale

▸ **scale**(`scale`): [`Vector2`](Vector2.md)

Returns a new Vector2 scaled by "scale" from the current Vector2

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scale` | `number` | defines the scaling factor |

#### Returns

[`Vector2`](Vector2.md)

a new Vector2

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:318

___

### scaleAndAddToRef

▸ **scaleAndAddToRef**(`scale`, `result`): [`Vector2`](Vector2.md)

Scale the current Vector2 values by a factor and add the result to a given Vector2

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scale` | `number` | defines the scale factor |
| `result` | [`Vector2`](Vector2.md) | defines the Vector2 object where to store the result |

#### Returns

[`Vector2`](Vector2.md)

the unmodified current Vector2

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:342

___

### scaleInPlace

▸ **scaleInPlace**(`scale`): [`Vector2`](Vector2.md)

Multiply the Vector2 coordinates by scale

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scale` | `number` | defines the scaling factor |

#### Returns

[`Vector2`](Vector2.md)

the current updated Vector2

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:307

___

### scaleToRef

▸ **scaleToRef**(`scale`, `result`): [`Vector2`](Vector2.md)

Scale the current Vector2 values by a factor to a given Vector2

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scale` | `number` | defines the scale factor |
| `result` | [`Vector2`](Vector2.md) | defines the Vector2 object where to store the result |

#### Returns

[`Vector2`](Vector2.md)

the unmodified current Vector2

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:330

___

### set

▸ **set**(`x`, `y`): [`Vector2`](Vector2.md)

Sets the Vector2 coordinates with the given floats

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | defines the first coordinate |
| `y` | `number` | defines the second coordinate |

#### Returns

[`Vector2`](Vector2.md)

the current updated Vector2

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:128

___

### subtract

▸ **subtract**(`otherVector`): [`Vector2`](Vector2.md)

Gets a new Vector2 set with the subtracted coordinates of the given one from the current Vector2

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherVector` | [`Vector2`](Vector2.md) | defines the other vector |

#### Returns

[`Vector2`](Vector2.md)

a new Vector2

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:177

___

### subtractInPlace

▸ **subtractInPlace**(`otherVector`): [`Vector2`](Vector2.md)

Sets the current Vector2 coordinates by subtracting from it the given one coordinates

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherVector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines the other vector |

#### Returns

[`Vector2`](Vector2.md)

the current updated Vector2

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:197

___

### subtractToRef

▸ **subtractToRef**(`otherVector`, `result`): [`Vector2`](Vector2.md)

Sets the "result" coordinates with the subtraction of the given one from the current Vector2 coordinates.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherVector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines the other vector |
| `result` | [`Vector2`](Vector2.md) | defines the target vector |

#### Returns

[`Vector2`](Vector2.md)

the unmodified current Vector2

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:187

___

### toArray

▸ **toArray**(`array`, `index?`): [`Vector2`](Vector2.md)

Sets the Vector2 coordinates in the given array or Float32Array from the given index.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `array` | [`FloatArray`](../modules.md#floatarray) | `undefined` | defines the source array |
| `index` | `number` | `0` | defines the offset in source array |

#### Returns

[`Vector2`](Vector2.md)

the current Vector2

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:72

___

### toString

▸ **toString**(): `string`

Gets a string with the Vector2 coordinates

#### Returns

`string`

a string with the Vector2 coordinates

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:40

___

### CatmullRom

▸ `Static` **CatmullRom**(`value1`, `value2`, `value3`, `value4`, `amount`): [`Vector2`](Vector2.md)

Gets a new Vector2 located for "amount" (float) on the CatmullRom spline defined by the given four Vector2

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines 1st point of control |
| `value2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines 2nd point of control |
| `value3` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines 3rd point of control |
| `value4` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines 4th point of control |
| `amount` | `number` | defines the interpolation factor |

#### Returns

[`Vector2`](Vector2.md)

a new Vector2

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:485

___

### Center

▸ `Static` **Center**(`value1`, `value2`): [`Vector2`](Vector2.md)

Gets a new Vector2 located at the center of the vectors "value1" and "value2"

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines first vector |
| `value2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines second vector |

#### Returns

[`Vector2`](Vector2.md)

a new Vector2

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:753

___

### CenterToRef

▸ `Static` **CenterToRef**(`value1`, `value2`, `ref`): [`Vector2`](Vector2.md)

Gets the center of the vectors "value1" and "value2" and stores the result in the vector "ref"

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines first vector |
| `value2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines second vector |
| `ref` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines third vector |

#### Returns

[`Vector2`](Vector2.md)

ref

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:764

___

### Clamp

▸ `Static` **Clamp**(`value`, `min`, `max`): [`Vector2`](Vector2.md)

Returns a new Vector2 set with same the coordinates than "value" ones if the vector "value" is in the square defined by "min" and "max".
If a coordinate of "value" is lower than "min" coordinates, the returned Vector2 is given this "min" coordinate.
If a coordinate of "value" is greater than "max" coordinates, the returned Vector2 is given this "max" coordinate

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines the value to clamp |
| `min` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines the lower limit |
| `max` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines the upper limit |

#### Returns

[`Vector2`](Vector2.md)

a new Vector2

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:521

___

### Distance

▸ `Static` **Distance**(`value1`, `value2`): `number`

Gets the distance between the vectors "value1" and "value2"

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines first vector |
| `value2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines second vector |

#### Returns

`number`

the distance between vectors

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:731

___

### DistanceOfPointFromSegment

▸ `Static` **DistanceOfPointFromSegment**(`p`, `segA`, `segB`): `number`

Gets the shortest distance (float) between the point "p" and the segment defined by the two points "segA" and "segB".

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `p` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines the middle point |
| `segA` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines one point of the segment |
| `segB` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines the other point of the segment |

#### Returns

`number`

the shortest distance

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:775

___

### DistanceSquared

▸ `Static` **DistanceSquared**(`value1`, `value2`): `number`

Returns the squared distance between the vectors "value1" and "value2"

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines first vector |
| `value2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines second vector |

#### Returns

`number`

the squared distance between vectors

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:741

___

### Dot

▸ `Static` **Dot**(`left`, `right`): `number`

Gets the dot product of the vector "left" and the vector "right"

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `left` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines first vector |
| `right` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines second vector |

#### Returns

`number`

the dot product (float)

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:627

___

### FromArray

▸ `Static` **FromArray**(`array`, `offset?`): [`Vector2`](Vector2.md)

Gets a new Vector2 set from the given index element of the given array

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `array` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)`ArrayLike``number` | `undefined` | defines the data source |
| `offset` | `number` | `0` | defines the offset in the data source |

#### Returns

[`Vector2`](Vector2.md)

a new Vector2

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:461

___

### FromArrayToRef

▸ `Static` **FromArrayToRef**(`array`, `offset`, `result`): `void`

Sets "result" from the given index element of the given array

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `array` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)`ArrayLike``number` | defines the data source |
| `offset` | `number` | defines the offset in the data source |
| `result` | [`Vector2`](Vector2.md) | defines the target vector |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:471

___

### Hermite

▸ `Static` **Hermite**(`value1`, `tangent1`, `value2`, `tangent2`, `amount`): [`Vector2`](Vector2.md)

Returns a new Vector2 located for "amount" (float) on the Hermite spline defined by the vectors "value1", "value2", "tangent1", "tangent2"

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines the 1st control point |
| `tangent1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines the outgoing tangent |
| `value2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines the 2nd control point |
| `tangent2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines the incoming tangent |
| `amount` | `number` | defines the interpolation factor |

#### Returns

[`Vector2`](Vector2.md)

a new Vector2

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:542

___

### Hermite1stDerivative

▸ `Static` **Hermite1stDerivative**(`value1`, `tangent1`, `value2`, `tangent2`, `time`): [`Vector2`](Vector2.md)

Returns a new Vector2 which is the 1st derivative of the Hermite spline defined by the vectors "value1", "value2", "tangent1", "tangent2".

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines the first control point |
| `tangent1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines the first tangent |
| `value2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines the second control point |
| `tangent2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines the second tangent |
| `time` | `number` | define where the derivative must be done |

#### Returns

[`Vector2`](Vector2.md)

1st derivative

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:571

___

### Hermite1stDerivativeToRef

▸ `Static` **Hermite1stDerivativeToRef**(`value1`, `tangent1`, `value2`, `tangent2`, `time`, `result`): `void`

Returns a new Vector2 which is the 1st derivative of the Hermite spline defined by the vectors "value1", "value2", "tangent1", "tangent2".

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines the first control point |
| `tangent1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines the first tangent |
| `value2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines the second control point |
| `tangent2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines the second tangent |
| `time` | `number` | define where the derivative must be done |
| `result` | [`Vector2`](Vector2.md) | define where the derivative will be stored |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:594

___

### Lerp

▸ `Static` **Lerp**(`start`, `end`, `amount`): [`Vector2`](Vector2.md)

Returns a new Vector2 located for "amount" (float) on the linear interpolation between the vector "start" adn the vector "end".

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `start` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines the start vector |
| `end` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines the end vector |
| `amount` | `number` | defines the interpolation factor |

#### Returns

[`Vector2`](Vector2.md)

a new Vector2

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:615

___

### Maximize

▸ `Static` **Maximize**(`left`, `right`): [`Vector2`](Vector2.md)

Gets a new Vector2 set with the maximal coordinate values from the "left" and "right" vectors

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `left` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines 1st vector |
| `right` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines 2nd vector |

#### Returns

[`Vector2`](Vector2.md)

a new Vector2

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:676

___

### Minimize

▸ `Static` **Minimize**(`left`, `right`): [`Vector2`](Vector2.md)

Gets a new Vector2 set with the minimal coordinate values from the "left" and "right" vectors

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `left` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines 1st vector |
| `right` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines 2nd vector |

#### Returns

[`Vector2`](Vector2.md)

a new Vector2

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:664

___

### Normalize

▸ `Static` **Normalize**(`vector`): [`Vector2`](Vector2.md)

Returns a new Vector2 equal to the normalized given vector

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines the vector to normalize |

#### Returns

[`Vector2`](Vector2.md)

a new Vector2

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:636

___

### NormalizeToRef

▸ `Static` **NormalizeToRef**(`vector`, `result`): `void`

Normalize a given vector into a second one

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines the vector to normalize |
| `result` | [`Vector2`](Vector2.md) | defines the vector where to store the result |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:647

___

### One

▸ `Static` **One**(): [`Vector2`](Vector2.md)

Gets a new Vector2(1, 1)

#### Returns

[`Vector2`](Vector2.md)

a new Vector2

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:451

___

### PointInTriangle

▸ `Static` **PointInTriangle**(`p`, `p0`, `p1`, `p2`): `boolean`

Determines if a given vector is included in a triangle

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `p` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines the vector to test |
| `p0` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines 1st triangle point |
| `p1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines 2nd triangle point |
| `p2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines 3rd triangle point |

#### Returns

`boolean`

true if the point "p" is in the triangle defined by the vectors "p0", "p1", "p2"

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:716

___

### Transform

▸ `Static` **Transform**(`vector`, `transformation`): [`Vector2`](Vector2.md)

Gets a new Vector2 set with the transformed coordinates of the given vector by the given transformation matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines the vector to transform |
| `transformation` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the matrix to apply |

#### Returns

[`Vector2`](Vector2.md)

a new Vector2

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:688

___

### TransformToRef

▸ `Static` **TransformToRef**(`vector`, `transformation`, `result`): `void`

Transforms the given vector coordinates by the given transformation matrix and stores the result in the vector "result" coordinates

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines the vector to transform |
| `transformation` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the matrix to apply |
| `result` | [`Vector2`](Vector2.md) | defines the target vector |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:700

___

### Zero

▸ `Static` **Zero**(): [`Vector2`](Vector2.md)

Gets a new Vector2(0, 0)

#### Returns

[`Vector2`](Vector2.md)

a new Vector2

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:443
