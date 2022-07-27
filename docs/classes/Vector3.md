[@dev/core](../README.md) / [Exports](../modules.md) / Vector3

# Class: Vector3

Class used to store (x,y,z) vector representation
A Vector3 is the main object used in 3D geometry
It can represent either the coordinates of a point the space, either a direction
Reminder: js uses a left handed forward facing system

## Table of contents

### Constructors

- [constructor](Vector3.md#constructor)

### Properties

- [\_LeftHandedForwardReadOnly](Vector3.md#_lefthandedforwardreadonly)
- [\_LeftReadOnly](Vector3.md#_leftreadonly)
- [\_RightHandedForwardReadOnly](Vector3.md#_righthandedforwardreadonly)
- [\_RightReadOnly](Vector3.md#_rightreadonly)
- [\_UpReadOnly](Vector3.md#_upreadonly)
- [\_ZeroReadOnly](Vector3.md#_zeroreadonly)

### Accessors

- [hasAZeroComponent](Vector3.md#hasazerocomponent)
- [isNonUniform](Vector3.md#isnonuniform)
- [x](Vector3.md#x)
- [y](Vector3.md#y)
- [z](Vector3.md#z)
- [LeftHandedForwardReadOnly](Vector3.md#lefthandedforwardreadonly)
- [LeftReadOnly](Vector3.md#leftreadonly)
- [RightHandedForwardReadOnly](Vector3.md#righthandedforwardreadonly)
- [RightReadOnly](Vector3.md#rightreadonly)
- [UpReadOnly](Vector3.md#upreadonly)
- [ZeroReadOnly](Vector3.md#zeroreadonly)

### Methods

- [add](Vector3.md#add)
- [addInPlace](Vector3.md#addinplace)
- [addInPlaceFromFloats](Vector3.md#addinplacefromfloats)
- [addToRef](Vector3.md#addtoref)
- [applyRotationQuaternion](Vector3.md#applyrotationquaternion)
- [applyRotationQuaternionInPlace](Vector3.md#applyrotationquaternioninplace)
- [applyRotationQuaternionToRef](Vector3.md#applyrotationquaterniontoref)
- [asArray](Vector3.md#asarray)
- [clone](Vector3.md#clone)
- [copyFrom](Vector3.md#copyfrom)
- [copyFromFloats](Vector3.md#copyfromfloats)
- [cross](Vector3.md#cross)
- [divide](Vector3.md#divide)
- [divideInPlace](Vector3.md#divideinplace)
- [divideToRef](Vector3.md#dividetoref)
- [equals](Vector3.md#equals)
- [equalsToFloats](Vector3.md#equalstofloats)
- [equalsWithEpsilon](Vector3.md#equalswithepsilon)
- [floor](Vector3.md#floor)
- [fract](Vector3.md#fract)
- [fromArray](Vector3.md#fromarray)
- [getClassName](Vector3.md#getclassname)
- [getHashCode](Vector3.md#gethashcode)
- [isNonUniformWithinEpsilon](Vector3.md#isnonuniformwithinepsilon)
- [length](Vector3.md#length)
- [lengthSquared](Vector3.md#lengthsquared)
- [maximizeInPlace](Vector3.md#maximizeinplace)
- [maximizeInPlaceFromFloats](Vector3.md#maximizeinplacefromfloats)
- [minimizeInPlace](Vector3.md#minimizeinplace)
- [minimizeInPlaceFromFloats](Vector3.md#minimizeinplacefromfloats)
- [multiply](Vector3.md#multiply)
- [multiplyByFloats](Vector3.md#multiplybyfloats)
- [multiplyInPlace](Vector3.md#multiplyinplace)
- [multiplyToRef](Vector3.md#multiplytoref)
- [negate](Vector3.md#negate)
- [negateInPlace](Vector3.md#negateinplace)
- [negateToRef](Vector3.md#negatetoref)
- [normalize](Vector3.md#normalize)
- [normalizeFromLength](Vector3.md#normalizefromlength)
- [normalizeToNew](Vector3.md#normalizetonew)
- [normalizeToRef](Vector3.md#normalizetoref)
- [projectOnPlane](Vector3.md#projectonplane)
- [projectOnPlaneToRef](Vector3.md#projectonplanetoref)
- [reorderInPlace](Vector3.md#reorderinplace)
- [rotateByQuaternionAroundPointToRef](Vector3.md#rotatebyquaternionaroundpointtoref)
- [rotateByQuaternionToRef](Vector3.md#rotatebyquaterniontoref)
- [scale](Vector3.md#scale)
- [scaleAndAddToRef](Vector3.md#scaleandaddtoref)
- [scaleInPlace](Vector3.md#scaleinplace)
- [scaleToRef](Vector3.md#scaletoref)
- [set](Vector3.md#set)
- [setAll](Vector3.md#setall)
- [subtract](Vector3.md#subtract)
- [subtractFromFloats](Vector3.md#subtractfromfloats)
- [subtractFromFloatsToRef](Vector3.md#subtractfromfloatstoref)
- [subtractInPlace](Vector3.md#subtractinplace)
- [subtractToRef](Vector3.md#subtracttoref)
- [toArray](Vector3.md#toarray)
- [toQuaternion](Vector3.md#toquaternion)
- [toString](Vector3.md#tostring)
- [Backward](Vector3.md#backward)
- [CatmullRom](Vector3.md#catmullrom)
- [Center](Vector3.md#center)
- [CenterToRef](Vector3.md#centertoref)
- [CheckExtends](Vector3.md#checkextends)
- [Clamp](Vector3.md#clamp)
- [ClampToRef](Vector3.md#clamptoref)
- [Cross](Vector3.md#cross-1)
- [CrossToRef](Vector3.md#crosstoref)
- [Distance](Vector3.md#distance)
- [DistanceSquared](Vector3.md#distancesquared)
- [Dot](Vector3.md#dot)
- [Down](Vector3.md#down)
- [Forward](Vector3.md#forward)
- [FromArray](Vector3.md#fromarray-1)
- [FromArrayToRef](Vector3.md#fromarraytoref)
- [FromFloatArray](Vector3.md#fromfloatarray)
- [FromFloatArrayToRef](Vector3.md#fromfloatarraytoref)
- [FromFloatsToRef](Vector3.md#fromfloatstoref)
- [GetAngleBetweenVectors](Vector3.md#getanglebetweenvectors)
- [GetAngleBetweenVectorsOnPlane](Vector3.md#getanglebetweenvectorsonplane)
- [GetClipFactor](Vector3.md#getclipfactor)
- [Hermite](Vector3.md#hermite)
- [Hermite1stDerivative](Vector3.md#hermite1stderivative)
- [Hermite1stDerivativeToRef](Vector3.md#hermite1stderivativetoref)
- [Left](Vector3.md#left)
- [Lerp](Vector3.md#lerp)
- [LerpToRef](Vector3.md#lerptoref)
- [Maximize](Vector3.md#maximize)
- [Minimize](Vector3.md#minimize)
- [Normalize](Vector3.md#normalize-1)
- [NormalizeToRef](Vector3.md#normalizetoref-1)
- [One](Vector3.md#one)
- [Project](Vector3.md#project)
- [ProjectOnTriangleToRef](Vector3.md#projectontriangletoref)
- [ProjectToRef](Vector3.md#projecttoref)
- [Right](Vector3.md#right)
- [RotationFromAxis](Vector3.md#rotationfromaxis)
- [RotationFromAxisToRef](Vector3.md#rotationfromaxistoref)
- [SlerpToRef](Vector3.md#slerptoref)
- [SmoothToRef](Vector3.md#smoothtoref)
- [TransformCoordinates](Vector3.md#transformcoordinates)
- [TransformCoordinatesFromFloatsToRef](Vector3.md#transformcoordinatesfromfloatstoref)
- [TransformCoordinatesToRef](Vector3.md#transformcoordinatestoref)
- [TransformNormal](Vector3.md#transformnormal)
- [TransformNormalFromFloatsToRef](Vector3.md#transformnormalfromfloatstoref)
- [TransformNormalToRef](Vector3.md#transformnormaltoref)
- [Unproject](Vector3.md#unproject)
- [UnprojectFloatsToRef](Vector3.md#unprojectfloatstoref)
- [UnprojectFromTransform](Vector3.md#unprojectfromtransform)
- [UnprojectToRef](Vector3.md#unprojecttoref)
- [Up](Vector3.md#up)
- [Zero](Vector3.md#zero)

## Constructors

### constructor

• **new Vector3**(`x?`, `y?`, `z?`)

Creates a new Vector3 object from the given x, y, z (floats) coordinates.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `x` | `number` | `0` | defines the first coordinates (on X axis) |
| `y` | `number` | `0` | defines the second coordinates (on Y axis) |
| `z` | `number` | `0` | defines the third coordinates (on Z axis) |

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:849

## Properties

### \_LeftHandedForwardReadOnly

▪ `Static` `Private` **\_LeftHandedForwardReadOnly**: [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:795

___

### \_LeftReadOnly

▪ `Static` `Private` **\_LeftReadOnly**: [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:798

___

### \_RightHandedForwardReadOnly

▪ `Static` `Private` **\_RightHandedForwardReadOnly**: [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:796

___

### \_RightReadOnly

▪ `Static` `Private` **\_RightReadOnly**: [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:797

___

### \_UpReadOnly

▪ `Static` `Private` **\_UpReadOnly**: [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:794

___

### \_ZeroReadOnly

▪ `Static` `Private` **\_ZeroReadOnly**: [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:799

## Accessors

### hasAZeroComponent

• `get` **hasAZeroComponent**(): `boolean`

Gets a boolean indicating if the vector contains a zero in one of its components

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1433

___

### isNonUniform

• `get` **isNonUniform**(): `boolean`

Gets a boolean indicating that the vector is non uniform meaning x, y or z are not all the same

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1382

___

### x

• `get` **x**(): `number`

Gets or sets the x coordinate

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:814

• `set` **x**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:818

___

### y

• `get` **y**(): `number`

Gets or sets the y coordinate

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:824

• `set` **y**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:828

___

### z

• `get` **z**(): `number`

Gets or sets the z coordinate

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:834

• `set` **z**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:838

___

### LeftHandedForwardReadOnly

• `Static` `get` **LeftHandedForwardReadOnly**(): [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md)

Gets a forward Vector3 that must not be updated

#### Returns

[`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1815

___

### LeftReadOnly

• `Static` `get` **LeftReadOnly**(): [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md)

Gets a left Vector3 that must not be updated

#### Returns

[`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1808

___

### RightHandedForwardReadOnly

• `Static` `get` **RightHandedForwardReadOnly**(): [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md)

Gets a forward Vector3 that must not be updated

#### Returns

[`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1822

___

### RightReadOnly

• `Static` `get` **RightReadOnly**(): [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md)

Gets a right Vector3 that must not be updated

#### Returns

[`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1801

___

### UpReadOnly

• `Static` `get` **UpReadOnly**(): [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md)

Gets a up Vector3 that must not be updated

#### Returns

[`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1794

___

### ZeroReadOnly

• `Static` `get` **ZeroReadOnly**(): [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md)

Gets a zero Vector3 that must not be updated

#### Returns

[`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1829

## Methods

### add

▸ **add**(`otherVector`): [`Vector3`](Vector3.md)

Gets a new Vector3, result of the addition the current Vector3 and the given vector

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherVector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the second operand |

#### Returns

[`Vector3`](Vector3.md)

the resulting Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:958

___

### addInPlace

▸ **addInPlace**(`otherVector`): [`Vector3`](Vector3.md)

Adds the given vector to the current Vector3

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherVector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the second operand |

#### Returns

[`Vector3`](Vector3.md)

the current updated Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:935

___

### addInPlaceFromFloats

▸ **addInPlaceFromFloats**(`x`, `y`, `z`): [`Vector3`](Vector3.md)

Adds the given coordinates to the current Vector3

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | defines the x coordinate of the operand |
| `y` | `number` | defines the y coordinate of the operand |
| `z` | `number` | defines the z coordinate of the operand |

#### Returns

[`Vector3`](Vector3.md)

the current updated Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:946

___

### addToRef

▸ **addToRef**(`otherVector`, `result`): [`Vector3`](Vector3.md)

Adds the current Vector3 to the given one and stores the result in the vector "result"

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherVector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the second operand |
| `result` | [`Vector3`](Vector3.md) | defines the Vector3 object where to store the result |

#### Returns

[`Vector3`](Vector3.md)

the current Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:968

___

### applyRotationQuaternion

▸ **applyRotationQuaternion**(`q`): [`Vector3`](Vector3.md)

Rotates the vector using the given unit quaternion and returns the new vector

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `q` | [`Quaternion`](Quaternion.md) | the unit quaternion representing the rotation |

#### Returns

[`Vector3`](Vector3.md)

a new Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1118

___

### applyRotationQuaternionInPlace

▸ **applyRotationQuaternionInPlace**(`q`): [`Vector3`](Vector3.md)

Rotates the vector in place using the given unit quaternion

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `q` | [`Quaternion`](Quaternion.md) | the unit quaternion representing the rotation |

#### Returns

[`Vector3`](Vector3.md)

the current updated Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1109

___

### applyRotationQuaternionToRef

▸ **applyRotationQuaternionToRef**(`q`, `result`): [`Vector3`](Vector3.md)

Rotates the vector using the given unit quaternion and stores the new vector in result

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `q` | [`Quaternion`](Quaternion.md) | the unit quaternion representing the rotation |
| `result` | [`Vector3`](Vector3.md) | the output vector |

#### Returns

[`Vector3`](Vector3.md)

the current Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1091

___

### asArray

▸ **asArray**(): `number`[]

Creates an array containing three elements : the coordinates of the Vector3

#### Returns

`number`[]

a new array of numbers

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:892

___

### clone

▸ **clone**(): [`Vector3`](Vector3.md)

Creates a new Vector3 copied from the current Vector3

#### Returns

[`Vector3`](Vector3.md)

the new Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1541

___

### copyFrom

▸ **copyFrom**(`source`): [`Vector3`](Vector3.md)

Copies the given vector coordinates to the current Vector3 ones

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the source Vector3 |

#### Returns

[`Vector3`](Vector3.md)

the current updated Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1550

___

### copyFromFloats

▸ **copyFromFloats**(`x`, `y`, `z`): [`Vector3`](Vector3.md)

Copies the given floats to the current Vector3 coordinates

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | defines the x coordinate of the operand |
| `y` | `number` | defines the y coordinate of the operand |
| `z` | `number` | defines the z coordinate of the operand |

#### Returns

[`Vector3`](Vector3.md)

the current updated Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1561

___

### cross

▸ **cross**(`other`): [`Vector3`](Vector3.md)

Returns a new Vector3 as the cross product of the current vector and the "other" one
The cross product is then orthogonal to both current and "other"

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`Vector3`](Vector3.md) | defines the right operand |

#### Returns

[`Vector3`](Vector3.md)

the cross product

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1495

___

### divide

▸ **divide**(`otherVector`): [`Vector3`](Vector3.md)

Returns a new Vector3 set with the result of the division of the current Vector3 coordinates by the given ones

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherVector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the second operand |

#### Returns

[`Vector3`](Vector3.md)

the new Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1273

___

### divideInPlace

▸ **divideInPlace**(`otherVector`): [`Vector3`](Vector3.md)

Divides the current Vector3 coordinates by the given ones.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherVector` | [`Vector3`](Vector3.md) | defines the second operand |

#### Returns

[`Vector3`](Vector3.md)

the current updated Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1292

___

### divideToRef

▸ **divideToRef**(`otherVector`, `result`): [`Vector3`](Vector3.md)

Divides the current Vector3 coordinates by the given ones and stores the result in the given vector "result"

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherVector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the second operand |
| `result` | [`Vector3`](Vector3.md) | defines the Vector3 object where to store the result |

#### Returns

[`Vector3`](Vector3.md)

the current Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1283

___

### equals

▸ **equals**(`otherVector`): `boolean`

Returns true if the current Vector3 and the given vector coordinates are strictly equal

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherVector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the second operand |

#### Returns

`boolean`

true if both vectors are equals

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1196

___

### equalsToFloats

▸ **equalsToFloats**(`x`, `y`, `z`): `boolean`

Returns true if the current Vector3 coordinates equals the given floats

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | defines the x coordinate of the operand |
| `y` | `number` | defines the y coordinate of the operand |
| `z` | `number` | defines the z coordinate of the operand |

#### Returns

`boolean`

true if both vectors are equals

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1222

___

### equalsWithEpsilon

▸ **equalsWithEpsilon**(`otherVector`, `epsilon?`): `boolean`

Returns true if the current Vector3 and the given vector coordinates are distant less than epsilon

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `otherVector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | `undefined` | defines the second operand |
| `epsilon` | `number` | `Epsilon` | defines the minimal distance to define values as equals |

#### Returns

`boolean`

true if both vectors are distant less than epsilon

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1206

___

### floor

▸ **floor**(): [`Vector3`](Vector3.md)

Gets a new Vector3 from current Vector3 floored values

#### Returns

[`Vector3`](Vector3.md)

a new Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1401

___

### fract

▸ **fract**(): [`Vector3`](Vector3.md)

Gets a new Vector3 from current Vector3 floored values

#### Returns

[`Vector3`](Vector3.md)

a new Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1409

___

### fromArray

▸ **fromArray**(`array`, `index?`): [`Vector3`](Vector3.md)

Update the current vector from an array

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `array` | [`FloatArray`](../modules.md#floatarray) | `undefined` | defines the destination array |
| `index` | `number` | `0` | defines the offset in the destination array |

#### Returns

[`Vector3`](Vector3.md)

the current Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:917

___

### getClassName

▸ **getClassName**(): `string`

Gets the class name

#### Returns

`string`

the string "Vector3"

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:867

___

### getHashCode

▸ **getHashCode**(): `number`

Creates the Vector3 hash code

#### Returns

`number`

a number which tends to be unique between Vector3 instances

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:875

___

### isNonUniformWithinEpsilon

▸ **isNonUniformWithinEpsilon**(`epsilon`): `boolean`

Due to float precision, scale of a mesh could be uniform but float values are off by a small fraction
Check if is non uniform within a certain amount of decimal places to account for this

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `epsilon` | `number` | the amount the values can differ |

#### Returns

`boolean`

if the the vector is non uniform to a certain number of decimal places

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1360

___

### length

▸ **length**(): `number`

Gets the length of the Vector3

#### Returns

`number`

the length of the Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1418

___

### lengthSquared

▸ **lengthSquared**(): `number`

Gets the squared length of the Vector3

#### Returns

`number`

squared length of the Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1426

___

### maximizeInPlace

▸ **maximizeInPlace**(`other`): [`Vector3`](Vector3.md)

Updates the current Vector3 with the maximal coordinate values between its and the given vector ones.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the second operand |

#### Returns

[`Vector3`](Vector3.md)

the current updated Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1310

___

### maximizeInPlaceFromFloats

▸ **maximizeInPlaceFromFloats**(`x`, `y`, `z`): [`Vector3`](Vector3.md)

Updates the current Vector3 with the maximal coordinate values between its and the given coordinates.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | defines the x coordinate of the operand |
| `y` | `number` | defines the y coordinate of the operand |
| `z` | `number` | defines the z coordinate of the operand |

#### Returns

[`Vector3`](Vector3.md)

the current updated Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1341

___

### minimizeInPlace

▸ **minimizeInPlace**(`other`): [`Vector3`](Vector3.md)

Updates the current Vector3 with the minimal coordinate values between its and the given vector ones

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the second operand |

#### Returns

[`Vector3`](Vector3.md)

the current updated Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1301

___

### minimizeInPlaceFromFloats

▸ **minimizeInPlaceFromFloats**(`x`, `y`, `z`): [`Vector3`](Vector3.md)

Updates the current Vector3 with the minimal coordinate values between its and the given coordinates

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | defines the x coordinate of the operand |
| `y` | `number` | defines the y coordinate of the operand |
| `z` | `number` | defines the z coordinate of the operand |

#### Returns

[`Vector3`](Vector3.md)

the current updated Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1321

___

### multiply

▸ **multiply**(`otherVector`): [`Vector3`](Vector3.md)

Returns a new Vector3, result of the multiplication of the current Vector3 by the given vector

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherVector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the second operand |

#### Returns

[`Vector3`](Vector3.md)

the new Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1243

___

### multiplyByFloats

▸ **multiplyByFloats**(`x`, `y`, `z`): [`Vector3`](Vector3.md)

Returns a new Vector3 set with the result of the multiplication of the current Vector3 coordinates by the given floats

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | defines the x coordinate of the operand |
| `y` | `number` | defines the y coordinate of the operand |
| `z` | `number` | defines the z coordinate of the operand |

#### Returns

[`Vector3`](Vector3.md)

the new Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1264

___

### multiplyInPlace

▸ **multiplyInPlace**(`otherVector`): [`Vector3`](Vector3.md)

Multiplies the current Vector3 coordinates by the given ones

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherVector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the second operand |

#### Returns

[`Vector3`](Vector3.md)

the current updated Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1231

___

### multiplyToRef

▸ **multiplyToRef**(`otherVector`, `result`): [`Vector3`](Vector3.md)

Multiplies the current Vector3 by the given one and stores the result in the given vector "result"

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherVector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the second operand |
| `result` | [`Vector3`](Vector3.md) | defines the Vector3 object where to store the result |

#### Returns

[`Vector3`](Vector3.md)

the current Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1253

___

### negate

▸ **negate**(): [`Vector3`](Vector3.md)

Gets a new Vector3 set with the current Vector3 negated coordinates

#### Returns

[`Vector3`](Vector3.md)

a new Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1030

___

### negateInPlace

▸ **negateInPlace**(): [`Vector3`](Vector3.md)

Negate this vector in place

#### Returns

[`Vector3`](Vector3.md)

this

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1038

___

### negateToRef

▸ **negateToRef**(`result`): [`Vector3`](Vector3.md)

Negate the current Vector3 and stores the result in the given vector "result" coordinates

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `result` | [`Vector3`](Vector3.md) | defines the Vector3 object where to store the result |

#### Returns

[`Vector3`](Vector3.md)

the current Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1050

___

### normalize

▸ **normalize**(): [`Vector3`](Vector3.md)

Normalize the current Vector3.
Please note that this is an in place operation.

#### Returns

[`Vector3`](Vector3.md)

the current updated Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1442

___

### normalizeFromLength

▸ **normalizeFromLength**(`len`): [`Vector3`](Vector3.md)

Normalize the current Vector3 with the given input length.
Please note that this is an in place operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `len` | `number` | the length of the vector |

#### Returns

[`Vector3`](Vector3.md)

the current updated Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1505

___

### normalizeToNew

▸ **normalizeToNew**(): [`Vector3`](Vector3.md)

Normalize the current Vector3 to a new vector

#### Returns

[`Vector3`](Vector3.md)

the new Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1517

___

### normalizeToRef

▸ **normalizeToRef**(`reference`): [`Vector3`](Vector3.md)

Normalize the current Vector3 to the reference

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `reference` | [`Vector3`](Vector3.md) | define the Vector3 to update |

#### Returns

[`Vector3`](Vector3.md)

the updated Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1528

___

### projectOnPlane

▸ **projectOnPlane**(`plane`, `origin`): [`Vector3`](Vector3.md)

Projects the current vector3 to a plane along a ray starting from a specified origin and directed towards the point.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `plane` | [`Plane`](Plane.md) | defines the plane to project to |
| `origin` | [`Vector3`](Vector3.md) | defines the origin of the projection ray |

#### Returns

[`Vector3`](Vector3.md)

the projected vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1138

___

### projectOnPlaneToRef

▸ **projectOnPlaneToRef**(`plane`, `origin`, `result`): `void`

Projects the current vector3 to a plane along a ray starting from a specified origin and directed towards the point.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `plane` | [`Plane`](Plane.md) | defines the plane to project to |
| `origin` | [`Vector3`](Vector3.md) | defines the origin of the projection ray |
| `result` | [`Vector3`](Vector3.md) | defines the Vector3 where to store the result |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1152

___

### reorderInPlace

▸ **reorderInPlace**(`order`): [`Vector3`](Vector3.md)

Reorders the x y z properties of the vector in place

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `order` | `string` | new ordering of the properties (eg. for vector 1,2,3 with "ZYX" will produce 3,2,1) |

#### Returns

[`Vector3`](Vector3.md)

the current updated vector

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1451

___

### rotateByQuaternionAroundPointToRef

▸ **rotateByQuaternionAroundPointToRef**(`quaternion`, `point`, `result`): [`Vector3`](Vector3.md)

Rotates a vector around a given point

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `quaternion` | [`Quaternion`](Quaternion.md) | the rotation quaternion |
| `point` | [`Vector3`](Vector3.md) | the point to rotate around |
| `result` | [`Vector3`](Vector3.md) | vector to store the result |

#### Returns

[`Vector3`](Vector3.md)

the resulting vector

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1482

___

### rotateByQuaternionToRef

▸ **rotateByQuaternionToRef**(`quaternion`, `result`): [`Vector3`](Vector3.md)

Rotates the vector around 0,0,0 by a quaternion

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `quaternion` | [`Quaternion`](Quaternion.md) | the rotation quaternion |
| `result` | [`Vector3`](Vector3.md) | vector to store the result |

#### Returns

[`Vector3`](Vector3.md)

the resulting vector

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1469

___

### scale

▸ **scale**(`scale`): [`Vector3`](Vector3.md)

Returns a new Vector3 set with the current Vector3 coordinates multiplied by the float "scale"

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scale` | `number` | defines the multiplier factor |

#### Returns

[`Vector3`](Vector3.md)

a new Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1071

___

### scaleAndAddToRef

▸ **scaleAndAddToRef**(`scale`, `result`): [`Vector3`](Vector3.md)

Scale the current Vector3 values by a factor and add the result to a given Vector3

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scale` | `number` | defines the scale factor |
| `result` | [`Vector3`](Vector3.md) | defines the Vector3 object where to store the result |

#### Returns

[`Vector3`](Vector3.md)

the unmodified current Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1128

___

### scaleInPlace

▸ **scaleInPlace**(`scale`): [`Vector3`](Vector3.md)

Multiplies the Vector3 coordinates by the float "scale"

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scale` | `number` | defines the multiplier factor |

#### Returns

[`Vector3`](Vector3.md)

the current updated Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1059

___

### scaleToRef

▸ **scaleToRef**(`scale`, `result`): [`Vector3`](Vector3.md)

Multiplies the current Vector3 coordinates by the float "scale" and stores the result in the given vector "result" coordinates

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scale` | `number` | defines the multiplier factor |
| `result` | [`Vector3`](Vector3.md) | defines the Vector3 object where to store the result |

#### Returns

[`Vector3`](Vector3.md)

the current Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1081

___

### set

▸ **set**(`x`, `y`, `z`): [`Vector3`](Vector3.md)

Copies the given floats to the current Vector3 coordinates

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | defines the x coordinate of the operand |
| `y` | `number` | defines the y coordinate of the operand |
| `z` | `number` | defines the z coordinate of the operand |

#### Returns

[`Vector3`](Vector3.md)

the current updated Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1575

___

### setAll

▸ **setAll**(`v`): [`Vector3`](Vector3.md)

Copies the given float to the current Vector3 coordinates

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `v` | `number` | defines the x, y and z coordinates of the operand |

#### Returns

[`Vector3`](Vector3.md)

the current updated Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1584

___

### subtract

▸ **subtract**(`otherVector`): [`Vector3`](Vector3.md)

Returns a new Vector3, result of the subtraction of the given vector from the current Vector3

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherVector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the second operand |

#### Returns

[`Vector3`](Vector3.md)

the resulting Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:989

___

### subtractFromFloats

▸ **subtractFromFloats**(`x`, `y`, `z`): [`Vector3`](Vector3.md)

Returns a new Vector3 set with the subtraction of the given floats from the current Vector3 coordinates

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | defines the x coordinate of the operand |
| `y` | `number` | defines the y coordinate of the operand |
| `z` | `number` | defines the z coordinate of the operand |

#### Returns

[`Vector3`](Vector3.md)

the resulting Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1010

___

### subtractFromFloatsToRef

▸ **subtractFromFloatsToRef**(`x`, `y`, `z`, `result`): [`Vector3`](Vector3.md)

Subtracts the given floats from the current Vector3 coordinates and set the given vector "result" with this result

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | defines the x coordinate of the operand |
| `y` | `number` | defines the y coordinate of the operand |
| `z` | `number` | defines the z coordinate of the operand |
| `result` | [`Vector3`](Vector3.md) | defines the Vector3 object where to store the result |

#### Returns

[`Vector3`](Vector3.md)

the current Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1022

___

### subtractInPlace

▸ **subtractInPlace**(`otherVector`): [`Vector3`](Vector3.md)

Subtract the given vector from the current Vector3

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherVector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the second operand |

#### Returns

[`Vector3`](Vector3.md)

the current updated Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:977

___

### subtractToRef

▸ **subtractToRef**(`otherVector`, `result`): [`Vector3`](Vector3.md)

Subtracts the given vector from the current Vector3 and stores the result in the vector "result".

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherVector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the second operand |
| `result` | [`Vector3`](Vector3.md) | defines the Vector3 object where to store the result |

#### Returns

[`Vector3`](Vector3.md)

the current Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:999

___

### toArray

▸ **toArray**(`array`, `index?`): [`Vector3`](Vector3.md)

Populates the given array or Float32Array from the given index with the successive coordinates of the Vector3

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `array` | [`FloatArray`](../modules.md#floatarray) | `undefined` | defines the destination array |
| `index` | `number` | `0` | defines the offset in the destination array |

#### Returns

[`Vector3`](Vector3.md)

the current Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:904

___

### toQuaternion

▸ **toQuaternion**(): [`Quaternion`](Quaternion.md)

Converts the current Vector3 into a quaternion (considering that the Vector3 contains Euler angles representation of a rotation)

#### Returns

[`Quaternion`](Quaternion.md)

a new Quaternion object, computed from the Vector3 coordinates

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:926

___

### toString

▸ **toString**(): `string`

Creates a string representation of the Vector3

#### Returns

`string`

a string with the Vector3 coordinates.

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:859

___

### Backward

▸ `Static` **Backward**(`rightHandedSystem?`): [`Vector3`](Vector3.md)

Returns a new Vector3 set to (0.0, 0.0, -1.0)

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `rightHandedSystem` | `boolean` | `false` | is the scene right-handed (negative-z) |

#### Returns

[`Vector3`](Vector3.md)

a new forward Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1853

___

### CatmullRom

▸ `Static` **CatmullRom**(`value1`, `value2`, `value3`, `value4`, `amount`): [`Vector3`](Vector3.md)

Returns a new Vector3 located for "amount" on the CatmullRom interpolation spline defined by the vectors "value1", "value2", "value3", "value4"

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the first control point |
| `value2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the second control point |
| `value3` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the third control point |
| `value4` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the fourth control point |
| `amount` | `number` | defines the amount on the spline to use |

#### Returns

[`Vector3`](Vector3.md)

the new Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1965

___

### Center

▸ `Static` **Center**(`value1`, `value2`): [`Vector3`](Vector3.md)

Returns a new Vector3 located at the center between "value1" and "value2"

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the first operand |
| `value2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the second operand |

#### Returns

[`Vector3`](Vector3.md)

the new Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:2580

___

### CenterToRef

▸ `Static` **CenterToRef**(`value1`, `value2`, `ref`): [`Vector3`](Vector3.md)

Gets the center of the vectors "value1" and "value2" and stores the result in the vector "ref"

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines first vector |
| `value2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines second vector |
| `ref` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines third vector |

#### Returns

[`Vector3`](Vector3.md)

ref

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:2591

___

### CheckExtends

▸ `Static` **CheckExtends**(`v`, `min`, `max`): `void`

Checks if a given vector is inside a specific range

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `v` | [`Vector3`](Vector3.md) | defines the vector to test |
| `min` | [`Vector3`](Vector3.md) | defines the minimum range |
| `max` | [`Vector3`](Vector3.md) | defines the maximum range |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:2044

___

### Clamp

▸ `Static` **Clamp**(`value`, `min`, `max`): [`Vector3`](Vector3.md)

Returns a new Vector3 set with the coordinates of "value", if the vector "value" is in the cube defined by the vectors "min" and "max"
If a coordinate value of "value" is lower than one of the "min" coordinate, then this "value" coordinate is set with the "min" one
If a coordinate value of "value" is greater than one of the "max" coordinate, then this "value" coordinate is set with the "max" one

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the current value |
| `min` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the lower range value |
| `max` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the upper range value |

#### Returns

[`Vector3`](Vector3.md)

the new Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:2008

___

### ClampToRef

▸ `Static` **ClampToRef**(`value`, `min`, `max`, `result`): `void`

Sets the given vector "result" with the coordinates of "value", if the vector "value" is in the cube defined by the vectors "min" and "max"
If a coordinate value of "value" is lower than one of the "min" coordinate, then this "value" coordinate is set with the "min" one
If a coordinate value of "value" is greater than one of the "max" coordinate, then this "value" coordinate is set with the "max" one

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the current value |
| `min` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the lower range value |
| `max` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the upper range value |
| `result` | [`Vector3`](Vector3.md) | defines the Vector3 where to store the result |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:2022

___

### Cross

▸ `Static` **Cross**(`left`, `right`): [`Vector3`](Vector3.md)

Returns a new Vector3 as the cross product of the vectors "left" and "right"
The cross product is then orthogonal to both "left" and "right"

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `left` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the left operand |
| `right` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the right operand |

#### Returns

[`Vector3`](Vector3.md)

the cross product

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:2168

___

### CrossToRef

▸ `Static` **CrossToRef**(`left`, `right`, `result`): `void`

Sets the given vector "result" with the cross product of "left" and "right"
The cross product is then orthogonal to both "left" and "right"

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `left` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the left operand |
| `right` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the right operand |
| `result` | [`Vector3`](Vector3.md) | defines the Vector3 where to store the result |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:2181

___

### Distance

▸ `Static` **Distance**(`value1`, `value2`): `number`

Returns the distance between the vectors "value1" and "value2"

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the first operand |
| `value2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the second operand |

#### Returns

`number`

the distance

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:2400

___

### DistanceSquared

▸ `Static` **DistanceSquared**(`value1`, `value2`): `number`

Returns the squared distance between the vectors "value1" and "value2"

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the first operand |
| `value2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the second operand |

#### Returns

`number`

the squared distance

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:2410

___

### Dot

▸ `Static` **Dot**(`left`, `right`): `number`

Returns the dot product (float) between the vectors "left" and "right"

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `left` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the left operand |
| `right` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the right operand |

#### Returns

`number`

the dot product

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:2157

___

### Down

▸ `Static` **Down**(): [`Vector3`](Vector3.md)

Returns a new Vector3 set to (0.0, -1.0, 0.0)

#### Returns

[`Vector3`](Vector3.md)

a new down Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1837

___

### Forward

▸ `Static` **Forward**(`rightHandedSystem?`): [`Vector3`](Vector3.md)

Returns a new Vector3 set to (0.0, 0.0, 1.0)

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `rightHandedSystem` | `boolean` | `false` | is the scene right-handed (negative z) |

#### Returns

[`Vector3`](Vector3.md)

a new forward Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1845

___

### FromArray

▸ `Static` **FromArray**(`array`, `offset?`): [`Vector3`](Vector3.md)

Returns a new Vector3 set from the index "offset" of the given array

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `array` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)`ArrayLike``number` | `undefined` | defines the source array |
| `offset` | `number` | `0` | defines the offset in the source array |

#### Returns

[`Vector3`](Vector3.md)

the new Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1720

___

### FromArrayToRef

▸ `Static` **FromArrayToRef**(`array`, `offset`, `result`): `void`

Sets the given vector "result" with the element values from the index "offset" of the given array

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `array` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)`ArrayLike``number` | defines the source array |
| `offset` | `number` | defines the offset in the source array |
| `result` | [`Vector3`](Vector3.md) | defines the Vector3 where to store the result |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1741

___

### FromFloatArray

▸ `Static` **FromFloatArray**(`array`, `offset?`): [`Vector3`](Vector3.md)

Returns a new Vector3 set from the index "offset" of the given Float32Array

**`Deprecated`**

Please use FromArray instead.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `array` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)`Float32Array` | defines the source array |
| `offset?` | `number` | defines the offset in the source array |

#### Returns

[`Vector3`](Vector3.md)

the new Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1731

___

### FromFloatArrayToRef

▸ `Static` **FromFloatArrayToRef**(`array`, `offset`, `result`): `void`

Sets the given vector "result" with the element values from the index "offset" of the given Float32Array

**`Deprecated`**

Please use FromArrayToRef instead.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `array` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)`Float32Array` | defines the source array |
| `offset` | `number` | defines the offset in the source array |
| `result` | [`Vector3`](Vector3.md) | defines the Vector3 where to store the result |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1754

___

### FromFloatsToRef

▸ `Static` **FromFloatsToRef**(`x`, `y`, `z`, `result`): `void`

Sets the given vector "result" with the given floats.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | defines the x coordinate of the source |
| `y` | `number` | defines the y coordinate of the source |
| `z` | `number` | defines the z coordinate of the source |
| `result` | [`Vector3`](Vector3.md) | defines the Vector3 where to store the result |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1765

___

### GetAngleBetweenVectors

▸ `Static` **GetAngleBetweenVectors**(`vector0`, `vector1`, `normal`): `number`

Get angle between two vectors

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vector0` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | angle between vector0 and vector1 |
| `vector1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | angle between vector0 and vector1 |
| `normal` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | direction of the normal |

#### Returns

`number`

the angle between vector0 and vector1

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1615

___

### GetAngleBetweenVectorsOnPlane

▸ `Static` **GetAngleBetweenVectorsOnPlane**(`vector0`, `vector1`, `normal`): `number`

Get angle between two vectors projected on a plane

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vector0` | [`Vector3`](Vector3.md) | angle between vector0 and vector1 |
| `vector1` | [`Vector3`](Vector3.md) | angle between vector0 and vector1 |
| `normal` | [`Vector3`](Vector3.md) | Normal of the projection plane |

#### Returns

`number`

the angle between vector0 and vector1 projected on the plane with the specified normal

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1638

___

### GetClipFactor

▸ `Static` **GetClipFactor**(`vector0`, `vector1`, `axis`, `size`): `number`

Get the clip factor between two vectors

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vector0` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the first operand |
| `vector1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the second operand |
| `axis` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the axis to use |
| `size` | `number` | defines the size along the axis |

#### Returns

`number`

the clip factor

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1599

___

### Hermite

▸ `Static` **Hermite**(`value1`, `tangent1`, `value2`, `tangent2`, `amount`): [`Vector3`](Vector3.md)

Returns a new Vector3 located for "amount" (float) on the Hermite interpolation spline defined by the vectors "value1", "tangent1", "value2", "tangent2"

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the first control point |
| `tangent1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the first tangent vector |
| `value2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the second control point |
| `tangent2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the second tangent vector |
| `amount` | `number` | defines the amount on the interpolation spline (between 0 and 1) |

#### Returns

[`Vector3`](Vector3.md)

the new Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:2058

___

### Hermite1stDerivative

▸ `Static` **Hermite1stDerivative**(`value1`, `tangent1`, `value2`, `tangent2`, `time`): [`Vector3`](Vector3.md)

Returns a new Vector3 which is the 1st derivative of the Hermite spline defined by the vectors "value1", "value2", "tangent1", "tangent2".

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the first control point |
| `tangent1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the first tangent |
| `value2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the second control point |
| `tangent2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the second tangent |
| `time` | `number` | define where the derivative must be done |

#### Returns

[`Vector3`](Vector3.md)

1st derivative

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:2087

___

### Hermite1stDerivativeToRef

▸ `Static` **Hermite1stDerivativeToRef**(`value1`, `tangent1`, `value2`, `tangent2`, `time`, `result`): `void`

Update a Vector3 with the 1st derivative of the Hermite spline defined by the vectors "value1", "value2", "tangent1", "tangent2".

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the first control point |
| `tangent1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the first tangent |
| `value2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the second control point |
| `tangent2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the second tangent |
| `time` | `number` | define where the derivative must be done |
| `result` | [`Vector3`](Vector3.md) | define where to store the derivative |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:2110

___

### Left

▸ `Static` **Left**(): [`Vector3`](Vector3.md)

Returns a new Vector3 set to (-1.0, 0.0, 0.0)

#### Returns

[`Vector3`](Vector3.md)

a new left Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1867

___

### Lerp

▸ `Static` **Lerp**(`start`, `end`, `amount`): [`Vector3`](Vector3.md)

Returns a new Vector3 located for "amount" (float) on the linear interpolation between the vectors "start" and "end"

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `start` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the start value |
| `end` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the end value |
| `amount` | `number` | max defines amount between both (between 0 and 1) |

#### Returns

[`Vector3`](Vector3.md)

the new Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:2132

___

### LerpToRef

▸ `Static` **LerpToRef**(`start`, `end`, `amount`, `result`): `void`

Sets the given vector "result" with the result of the linear interpolation from the vector "start" for "amount" to the vector "end"

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `start` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the start value |
| `end` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the end value |
| `amount` | `number` | max defines amount between both (between 0 and 1) |
| `result` | [`Vector3`](Vector3.md) | defines the Vector3 where to store the result |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:2145

___

### Maximize

▸ `Static` **Maximize**(`left`, `right`): [`Vector3`](Vector3.md)

Gets the maximal coordinate values between two Vector3

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `left` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the first operand |
| `right` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the second operand |

#### Returns

[`Vector3`](Vector3.md)

the new Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:2388

___

### Minimize

▸ `Static` **Minimize**(`left`, `right`): [`Vector3`](Vector3.md)

Gets the minimal coordinate values between two Vector3

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `left` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the first operand |
| `right` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the second operand |

#### Returns

[`Vector3`](Vector3.md)

the new Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:2376

___

### Normalize

▸ `Static` **Normalize**(`vector`): [`Vector3`](Vector3.md)

Returns a new Vector3 as the normalization of the given vector

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the Vector3 to normalize |

#### Returns

[`Vector3`](Vector3.md)

the new Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:2193

___

### NormalizeToRef

▸ `Static` **NormalizeToRef**(`vector`, `result`): `void`

Sets the given vector "result" with the normalization of the given first vector

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the Vector3 to normalize |
| `result` | [`Vector3`](Vector3.md) | defines the Vector3 where to store the result |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:2204

___

### One

▸ `Static` **One**(): [`Vector3`](Vector3.md)

Returns a new Vector3 set to (1.0, 1.0, 1.0)

#### Returns

[`Vector3`](Vector3.md)

a new unit Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1780

___

### Project

▸ `Static` **Project**(`vector`, `world`, `transform`, `viewport`): [`Vector3`](Vector3.md)

Project a Vector3 onto screen space

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the Vector3 to project |
| `world` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the world matrix to use |
| `transform` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the transform (view x projection) matrix to use |
| `viewport` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Viewport`](Viewport.md) | defines the screen viewport to use |

#### Returns

[`Vector3`](Vector3.md)

the new Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:2216

___

### ProjectOnTriangleToRef

▸ `Static` **ProjectOnTriangleToRef**(`vector`, `p0`, `p1`, `p2`, `ref`): `number`

Projects "vector" on the triangle determined by its extremities "p0", "p1" and "p2", stores the result in "ref"
and returns the distance to the projected point.
From http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.104.4264&rep=rep1&type=pdf

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | the vector to get distance from |
| `p0` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | extremity of the triangle |
| `p1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | extremity of the triangle |
| `p2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | extremity of the triangle |
| `ref` | [`Vector3`](Vector3.md) | variable to store the result to |

#### Returns

`number`

The distance between "ref" and "vector"

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:2430

___

### ProjectToRef

▸ `Static` **ProjectToRef**(`vector`, `world`, `transform`, `viewport`, `result`): [`Vector3`](Vector3.md)

Project a Vector3 onto screen space to reference

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the Vector3 to project |
| `world` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the world matrix to use |
| `transform` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the transform (view x projection) matrix to use |
| `viewport` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Viewport`](Viewport.md) | defines the screen viewport to use |
| `result` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | the vector in which the screen space will be stored |

#### Returns

[`Vector3`](Vector3.md)

the new Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:2231

___

### Right

▸ `Static` **Right**(): [`Vector3`](Vector3.md)

Returns a new Vector3 set to (1.0, 0.0, 0.0)

#### Returns

[`Vector3`](Vector3.md)

a new right Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1860

___

### RotationFromAxis

▸ `Static` **RotationFromAxis**(`axis1`, `axis2`, `axis3`): [`Vector3`](Vector3.md)

Given three orthogonal normalized left-handed oriented Vector3 axis in space (target system),
RotationFromAxis() returns the rotation Euler angles (ex : rotation.x, rotation.y, rotation.z) to apply
to something in order to rotate it from its local system to the given target system
Note: axis1, axis2 and axis3 are normalized during this operation

**`See`**

https://doc.babylonjs.com/divingDeeper/mesh/transforms/center_origin/target_align

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `axis1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the first axis |
| `axis2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the second axis |
| `axis3` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the third axis |

#### Returns

[`Vector3`](Vector3.md)

a new Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:2606

___

### RotationFromAxisToRef

▸ `Static` **RotationFromAxisToRef**(`axis1`, `axis2`, `axis3`, `ref`): `void`

The same than RotationFromAxis but updates the given ref Vector3 parameter instead of returning a new Vector3

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `axis1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the first axis |
| `axis2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the second axis |
| `axis3` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the third axis |
| `ref` | [`Vector3`](Vector3.md) | defines the Vector3 where to store the result |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:2619

___

### SlerpToRef

▸ `Static` **SlerpToRef**(`vector0`, `vector1`, `slerp`, `result`): `void`

Slerp between two vectors. See also `SmoothToRef`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vector0` | [`Vector3`](Vector3.md) | Start vector |
| `vector1` | [`Vector3`](Vector3.md) | End vector |
| `slerp` | `number` | amount (will be clamped between 0 and 1) |
| `result` | [`Vector3`](Vector3.md) | The slerped vector |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1667

___

### SmoothToRef

▸ `Static` **SmoothToRef**(`source`, `goal`, `deltaTime`, `lerpTime`, `result`): `void`

Smooth interpolation between two vectors using Slerp

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | [`Vector3`](Vector3.md) | source vector |
| `goal` | [`Vector3`](Vector3.md) | goal vector |
| `deltaTime` | `number` | current interpolation frame |
| `lerpTime` | `number` | total interpolation time |
| `result` | [`Vector3`](Vector3.md) | the smoothed vector |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1710

___

### TransformCoordinates

▸ `Static` **TransformCoordinates**(`vector`, `transformation`): [`Vector3`](Vector3.md)

Returns a new Vector3 set with the result of the transformation by the given matrix of the given vector.
This method computes transformed coordinates only, not transformed direction vectors (ie. it takes translation in account)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the Vector3 to transform |
| `transformation` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the transformation matrix |

#### Returns

[`Vector3`](Vector3.md)

the transformed Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1878

___

### TransformCoordinatesFromFloatsToRef

▸ `Static` **TransformCoordinatesFromFloatsToRef**(`x`, `y`, `z`, `transformation`, `result`): `void`

Sets the given vector "result" coordinates with the result of the transformation by the given matrix of the given floats (x, y, z)
This method computes transformed coordinates only, not transformed direction vectors

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | define the x coordinate of the source vector |
| `y` | `number` | define the y coordinate of the source vector |
| `z` | `number` | define the z coordinate of the source vector |
| `transformation` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the transformation matrix |
| `result` | [`Vector3`](Vector3.md) | defines the Vector3 where to store the result |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1904

___

### TransformCoordinatesToRef

▸ `Static` **TransformCoordinatesToRef**(`vector`, `transformation`, `result`): `void`

Sets the given vector "result" coordinates with the result of the transformation by the given matrix of the given vector
This method computes transformed coordinates only, not transformed direction vectors (ie. it takes translation in account)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the Vector3 to transform |
| `transformation` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the transformation matrix |
| `result` | [`Vector3`](Vector3.md) | defines the Vector3 where to store the result |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1891

___

### TransformNormal

▸ `Static` **TransformNormal**(`vector`, `transformation`): [`Vector3`](Vector3.md)

Returns a new Vector3 set with the result of the normal transformation by the given matrix of the given vector
This methods computes transformed normalized direction vectors only (ie. it does not apply translation)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the Vector3 to transform |
| `transformation` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the transformation matrix |

#### Returns

[`Vector3`](Vector3.md)

the new Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1923

___

### TransformNormalFromFloatsToRef

▸ `Static` **TransformNormalFromFloatsToRef**(`x`, `y`, `z`, `transformation`, `result`): `void`

Sets the given vector "result" with the result of the normal transformation by the given matrix of the given floats (x, y, z)
This methods computes transformed normalized direction vectors only (ie. it does not apply translation)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | define the x coordinate of the source vector |
| `y` | `number` | define the y coordinate of the source vector |
| `z` | `number` | define the z coordinate of the source vector |
| `transformation` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the transformation matrix |
| `result` | [`Vector3`](Vector3.md) | defines the Vector3 where to store the result |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1949

___

### TransformNormalToRef

▸ `Static` **TransformNormalToRef**(`vector`, `transformation`, `result`): `void`

Sets the given vector "result" with the result of the normal transformation by the given matrix of the given vector
This methods computes transformed normalized direction vectors only (ie. it does not apply translation)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vector` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the Vector3 to transform |
| `transformation` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the transformation matrix |
| `result` | [`Vector3`](Vector3.md) | defines the Vector3 where to store the result |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1936

___

### Unproject

▸ `Static` **Unproject**(`source`, `viewportWidth`, `viewportHeight`, `world`, `view`, `projection`): [`Vector3`](Vector3.md)

Unproject from screen space to object space

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the screen space Vector3 to use |
| `viewportWidth` | `number` | defines the current width of the viewport |
| `viewportHeight` | `number` | defines the current height of the viewport |
| `world` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the world matrix to use (can be set to Identity to go to world space) |
| `view` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the view matrix to use |
| `projection` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the projection matrix to use |

#### Returns

[`Vector3`](Vector3.md)

the new Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:2293

___

### UnprojectFloatsToRef

▸ `Static` **UnprojectFloatsToRef**(`sourceX`, `sourceY`, `sourceZ`, `viewportWidth`, `viewportHeight`, `world`, `view`, `projection`, `result`): `void`

Unproject from screen space to object space

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sourceX` | `number` | defines the screen space x coordinate to use |
| `sourceY` | `number` | defines the screen space y coordinate to use |
| `sourceZ` | `number` | defines the screen space z coordinate to use |
| `viewportWidth` | `number` | defines the current width of the viewport |
| `viewportHeight` | `number` | defines the current height of the viewport |
| `world` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the world matrix to use (can be set to Identity to go to world space) |
| `view` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the view matrix to use |
| `projection` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the projection matrix to use |
| `result` | [`Vector3`](Vector3.md) | defines the Vector3 where to store the result |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:2342

___

### UnprojectFromTransform

▸ `Static` **UnprojectFromTransform**(`source`, `viewportWidth`, `viewportHeight`, `world`, `transform`): [`Vector3`](Vector3.md)

Unproject from screen space to object space

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | [`Vector3`](Vector3.md) | defines the screen space Vector3 to use |
| `viewportWidth` | `number` | defines the current width of the viewport |
| `viewportHeight` | `number` | defines the current height of the viewport |
| `world` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the world matrix to use (can be set to Identity to go to world space) |
| `transform` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the transform (view x projection) matrix to use |

#### Returns

[`Vector3`](Vector3.md)

the new Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:2279

___

### UnprojectToRef

▸ `Static` **UnprojectToRef**(`source`, `viewportWidth`, `viewportHeight`, `world`, `view`, `projection`, `result`): `void`

Unproject from screen space to object space

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the screen space Vector3 to use |
| `viewportWidth` | `number` | defines the current width of the viewport |
| `viewportHeight` | `number` | defines the current height of the viewport |
| `world` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the world matrix to use (can be set to Identity to go to world space) |
| `view` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the view matrix to use |
| `projection` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the projection matrix to use |
| `result` | [`Vector3`](Vector3.md) | defines the Vector3 where to store the result |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:2318

___

### Up

▸ `Static` **Up**(): [`Vector3`](Vector3.md)

Returns a new Vector3 set to (0.0, 1.0, 0.0)

#### Returns

[`Vector3`](Vector3.md)

a new up Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1787

___

### Zero

▸ `Static` **Zero**(): [`Vector3`](Vector3.md)

Returns a new Vector3 set to (0.0, 0.0, 0.0)

#### Returns

[`Vector3`](Vector3.md)

a new empty Vector3

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:1773
