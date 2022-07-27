[@dev/core](../README.md) / [Exports](../modules.md) / Quaternion

# Class: Quaternion

Class used to store quaternion data

**`See`**

 - https://en.wikipedia.org/wiki/Quaternion
 - https://doc.babylonjs.com/features/position,_rotation,_scaling

## Table of contents

### Constructors

- [constructor](Quaternion.md#constructor)

### Accessors

- [w](Quaternion.md#w)
- [x](Quaternion.md#x)
- [y](Quaternion.md#y)
- [z](Quaternion.md#z)

### Methods

- [add](Quaternion.md#add)
- [addInPlace](Quaternion.md#addinplace)
- [asArray](Quaternion.md#asarray)
- [clone](Quaternion.md#clone)
- [conjugate](Quaternion.md#conjugate)
- [conjugateInPlace](Quaternion.md#conjugateinplace)
- [conjugateToRef](Quaternion.md#conjugatetoref)
- [copyFrom](Quaternion.md#copyfrom)
- [copyFromFloats](Quaternion.md#copyfromfloats)
- [equals](Quaternion.md#equals)
- [equalsWithEpsilon](Quaternion.md#equalswithepsilon)
- [fromRotationMatrix](Quaternion.md#fromrotationmatrix)
- [getClassName](Quaternion.md#getclassname)
- [getHashCode](Quaternion.md#gethashcode)
- [invert](Quaternion.md#invert)
- [invertInPlace](Quaternion.md#invertinplace)
- [length](Quaternion.md#length)
- [lengthSquared](Quaternion.md#lengthsquared)
- [multiply](Quaternion.md#multiply)
- [multiplyInPlace](Quaternion.md#multiplyinplace)
- [multiplyToRef](Quaternion.md#multiplytoref)
- [normalize](Quaternion.md#normalize)
- [normalizeToNew](Quaternion.md#normalizetonew)
- [scale](Quaternion.md#scale)
- [scaleAndAddToRef](Quaternion.md#scaleandaddtoref)
- [scaleInPlace](Quaternion.md#scaleinplace)
- [scaleToRef](Quaternion.md#scaletoref)
- [set](Quaternion.md#set)
- [subtract](Quaternion.md#subtract)
- [subtractInPlace](Quaternion.md#subtractinplace)
- [toArray](Quaternion.md#toarray)
- [toEulerAngles](Quaternion.md#toeulerangles)
- [toEulerAnglesToRef](Quaternion.md#toeuleranglestoref)
- [toRotationMatrix](Quaternion.md#torotationmatrix)
- [toString](Quaternion.md#tostring)
- [AreClose](Quaternion.md#areclose)
- [Dot](Quaternion.md#dot)
- [FromArray](Quaternion.md#fromarray)
- [FromArrayToRef](Quaternion.md#fromarraytoref)
- [FromEulerAngles](Quaternion.md#fromeulerangles)
- [FromEulerAnglesToRef](Quaternion.md#fromeuleranglestoref)
- [FromEulerVector](Quaternion.md#fromeulervector)
- [FromEulerVectorToRef](Quaternion.md#fromeulervectortoref)
- [FromLookDirectionLH](Quaternion.md#fromlookdirectionlh)
- [FromLookDirectionLHToRef](Quaternion.md#fromlookdirectionlhtoref)
- [FromLookDirectionRH](Quaternion.md#fromlookdirectionrh)
- [FromLookDirectionRHToRef](Quaternion.md#fromlookdirectionrhtoref)
- [FromRotationMatrix](Quaternion.md#fromrotationmatrix-1)
- [FromRotationMatrixToRef](Quaternion.md#fromrotationmatrixtoref)
- [FromUnitVectorsToRef](Quaternion.md#fromunitvectorstoref)
- [Hermite](Quaternion.md#hermite)
- [Hermite1stDerivative](Quaternion.md#hermite1stderivative)
- [Hermite1stDerivativeToRef](Quaternion.md#hermite1stderivativetoref)
- [Identity](Quaternion.md#identity)
- [Inverse](Quaternion.md#inverse)
- [InverseToRef](Quaternion.md#inversetoref)
- [IsIdentity](Quaternion.md#isidentity)
- [RotationAlphaBetaGamma](Quaternion.md#rotationalphabetagamma)
- [RotationAlphaBetaGammaToRef](Quaternion.md#rotationalphabetagammatoref)
- [RotationAxis](Quaternion.md#rotationaxis)
- [RotationAxisToRef](Quaternion.md#rotationaxistoref)
- [RotationQuaternionFromAxis](Quaternion.md#rotationquaternionfromaxis)
- [RotationQuaternionFromAxisToRef](Quaternion.md#rotationquaternionfromaxistoref)
- [RotationYawPitchRoll](Quaternion.md#rotationyawpitchroll)
- [RotationYawPitchRollToRef](Quaternion.md#rotationyawpitchrolltoref)
- [Slerp](Quaternion.md#slerp)
- [SlerpToRef](Quaternion.md#slerptoref)
- [SmoothToRef](Quaternion.md#smoothtoref)
- [Zero](Quaternion.md#zero)

## Constructors

### constructor

• **new Quaternion**(`x?`, `y?`, `z?`, `w?`)

Creates a new Quaternion from the given floats

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `x` | `number` | `0.0` | defines the first component (0 by default) |
| `y` | `number` | `0.0` | defines the second component (0 by default) |
| `z` | `number` | `0.0` | defines the third component (0 by default) |
| `w` | `number` | `1.0` | defines the fourth component (1.0 by default) |

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3494

## Accessors

### w

• `get` **w**(): `number`

Gets or sets the w coordinate

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3479

• `set` **w**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3483

___

### x

• `get` **x**(): `number`

Gets or sets the x coordinate

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3449

• `set` **x**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3453

___

### y

• `get` **y**(): `number`

Gets or sets the y coordinate

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3459

• `set` **y**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3463

___

### z

• `get` **z**(): `number`

Gets or sets the z coordinate

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3469

• `set` **z**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3473

## Methods

### add

▸ **add**(`other`): [`Quaternion`](Quaternion.md)

Adds two quaternions

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Quaternion`](Quaternion.md) | defines the second operand |

#### Returns

[`Quaternion`](Quaternion.md)

a new quaternion as the addition result of the given one and the current quaternion

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3635

___

### addInPlace

▸ **addInPlace**(`other`): [`Quaternion`](Quaternion.md)

Add a quaternion to the current one

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Quaternion`](Quaternion.md) | defines the quaternion to add |

#### Returns

[`Quaternion`](Quaternion.md)

the current quaternion

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3644

___

### asArray

▸ **asArray**(): `number`[]

Copy the quaternion to an array

#### Returns

`number`[]

a new array populated with 4 elements from the quaternion coordinates

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3538

___

### clone

▸ **clone**(): [`Quaternion`](Quaternion.md)

Clone the current quaternion

#### Returns

[`Quaternion`](Quaternion.md)

a new quaternion copied from the current one

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3585

___

### conjugate

▸ **conjugate**(): [`Quaternion`](Quaternion.md)

Conjugates in place (1-q) the current quaternion

#### Returns

[`Quaternion`](Quaternion.md)

a new quaternion

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3786

___

### conjugateInPlace

▸ **conjugateInPlace**(): [`Quaternion`](Quaternion.md)

Conjugates in place (1-q) the current quaternion

#### Returns

[`Quaternion`](Quaternion.md)

the current updated quaternion

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3775

___

### conjugateToRef

▸ **conjugateToRef**(`ref`): [`Quaternion`](Quaternion.md)

Conjugates (1-q) the current quaternion and stores the result in the given quaternion

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ref` | [`Quaternion`](Quaternion.md) | defines the target quaternion |

#### Returns

[`Quaternion`](Quaternion.md)

the current quaternion

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3766

___

### copyFrom

▸ **copyFrom**(`other`): [`Quaternion`](Quaternion.md)

Copy a quaternion to the current one

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Quaternion`](Quaternion.md) | defines the other quaternion |

#### Returns

[`Quaternion`](Quaternion.md)

the updated current quaternion

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3594

___

### copyFromFloats

▸ **copyFromFloats**(`x`, `y`, `z`, `w`): [`Quaternion`](Quaternion.md)

Updates the current quaternion with the given float coordinates

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | defines the x coordinate |
| `y` | `number` | defines the y coordinate |
| `z` | `number` | defines the z coordinate |
| `w` | `number` | defines the w coordinate |

#### Returns

[`Quaternion`](Quaternion.md)

the updated current quaternion

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3610

___

### equals

▸ **equals**(`otherQuaternion`): `boolean`

Check if two quaternions are equals

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherQuaternion` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Quaternion`](Quaternion.md) | defines the second operand |

#### Returns

`boolean`

true if the current quaternion and the given one coordinates are strictly equals

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3561

___

### equalsWithEpsilon

▸ **equalsWithEpsilon**(`otherQuaternion`, `epsilon?`): `boolean`

Gets a boolean if two quaternions are equals (using an epsilon value)

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `otherQuaternion` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Quaternion`](Quaternion.md) | `undefined` | defines the other quaternion |
| `epsilon` | `number` | `Epsilon` | defines the minimal distance to consider equality |

#### Returns

`boolean`

true if the given quaternion coordinates are close to the current ones by a distance of epsilon.

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3571

___

### fromRotationMatrix

▸ **fromRotationMatrix**(`matrix`): [`Quaternion`](Quaternion.md)

Updates the current quaternion from the given rotation matrix values

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `matrix` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the source matrix |

#### Returns

[`Quaternion`](Quaternion.md)

the current updated quaternion

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3925

___

### getClassName

▸ **getClassName**(): `string`

Gets the class name of the quaternion

#### Returns

`string`

the string "Quaternion"

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3513

___

### getHashCode

▸ **getHashCode**(): `number`

Gets a hash code for this quaternion

#### Returns

`number`

the quaternion hash code

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3521

___

### invert

▸ **invert**(): [`Quaternion`](Quaternion.md)

Returns the inverse of the current quaternion

#### Returns

[`Quaternion`](Quaternion.md)

a new quaternion

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3794

___

### invertInPlace

▸ **invertInPlace**(): [`Quaternion`](Quaternion.md)

Invert in place the current quaternion

#### Returns

[`Quaternion`](Quaternion.md)

this quaternion

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3808

___

### length

▸ **length**(): `number`

Gets length of current quaternion

#### Returns

`number`

the quaternion length (float)

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3830

___

### lengthSquared

▸ **lengthSquared**(): `number`

Gets squared length of current quaternion

#### Returns

`number`

the quaternion length (float)

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3822

___

### multiply

▸ **multiply**(`q1`): [`Quaternion`](Quaternion.md)

Multiplies two quaternions

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `q1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Quaternion`](Quaternion.md) | defines the second operand |

#### Returns

[`Quaternion`](Quaternion.md)

a new quaternion set as the multiplication result of the current one with the given one "q1"

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3730

___

### multiplyInPlace

▸ **multiplyInPlace**(`q1`): [`Quaternion`](Quaternion.md)

Updates the current quaternion with the multiplication of itself with the given one "q1"

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `q1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Quaternion`](Quaternion.md) | defines the second operand |

#### Returns

[`Quaternion`](Quaternion.md)

the currentupdated quaternion

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3756

___

### multiplyToRef

▸ **multiplyToRef**(`q1`, `result`): [`Quaternion`](Quaternion.md)

Sets the given "result" as the the multiplication result of the current one with the given one "q1"

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `q1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Quaternion`](Quaternion.md) | defines the second operand |
| `result` | [`Quaternion`](Quaternion.md) | defines the target quaternion |

#### Returns

[`Quaternion`](Quaternion.md)

the current quaternion

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3742

___

### normalize

▸ **normalize**(): [`Quaternion`](Quaternion.md)

Normalize in place the current quaternion

#### Returns

[`Quaternion`](Quaternion.md)

the current updated quaternion

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3838

___

### normalizeToNew

▸ **normalizeToNew**(): [`Quaternion`](Quaternion.md)

Normalize a copy of the current quaternion

#### Returns

[`Quaternion`](Quaternion.md)

the normalized quaternion

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3853

___

### scale

▸ **scale**(`value`): [`Quaternion`](Quaternion.md)

Multiplies the current quaternion by a scale factor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `number` | defines the scale factor |

#### Returns

[`Quaternion`](Quaternion.md)

a new quaternion set by multiplying the current quaternion coordinates by the float "scale"

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3679

___

### scaleAndAddToRef

▸ **scaleAndAddToRef**(`scale`, `result`): [`Quaternion`](Quaternion.md)

Scale the current quaternion values by a factor and add the result to a given quaternion

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scale` | `number` | defines the scale factor |
| `result` | [`Quaternion`](Quaternion.md) | defines the Quaternion object where to store the result |

#### Returns

[`Quaternion`](Quaternion.md)

the unmodified current quaternion

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3717

___

### scaleInPlace

▸ **scaleInPlace**(`value`): [`Quaternion`](Quaternion.md)

Multiplies in place the current quaternion by a scale factor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `number` | defines the scale factor |

#### Returns

[`Quaternion`](Quaternion.md)

the current modified quaternion

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3702

___

### scaleToRef

▸ **scaleToRef**(`scale`, `result`): [`Quaternion`](Quaternion.md)

Scale the current quaternion values by a factor and stores the result to a given quaternion

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scale` | `number` | defines the scale factor |
| `result` | [`Quaternion`](Quaternion.md) | defines the Quaternion object where to store the result |

#### Returns

[`Quaternion`](Quaternion.md)

the unmodified current quaternion

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3689

___

### set

▸ **set**(`x`, `y`, `z`, `w`): [`Quaternion`](Quaternion.md)

Updates the current quaternion from the given float coordinates

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | defines the x coordinate |
| `y` | `number` | defines the y coordinate |
| `z` | `number` | defines the z coordinate |
| `w` | `number` | defines the w coordinate |

#### Returns

[`Quaternion`](Quaternion.md)

the updated current quaternion

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3626

___

### subtract

▸ **subtract**(`other`): [`Quaternion`](Quaternion.md)

Subtract two quaternions

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`Quaternion`](Quaternion.md) | defines the second operand |

#### Returns

[`Quaternion`](Quaternion.md)

a new quaternion as the subtraction result of the given one from the current one

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3657

___

### subtractInPlace

▸ **subtractInPlace**(`other`): [`Quaternion`](Quaternion.md)

Subtract a quaternion to the current one

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Quaternion`](Quaternion.md) | defines the quaternion to subtract |

#### Returns

[`Quaternion`](Quaternion.md)

the current quaternion

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3666

___

### toArray

▸ **toArray**(`array`, `index?`): [`Quaternion`](Quaternion.md)

Stores from the starting index in the given array the Quaternion successive values

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `array` | [`FloatArray`](../modules.md#floatarray) | `undefined` | defines the array where to store the x,y,z,w components |
| `index` | `number` | `0` | defines an optional index in the target array to define where to start storing values |

#### Returns

[`Quaternion`](Quaternion.md)

the current Quaternion object

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3548

___

### toEulerAngles

▸ **toEulerAngles**(): [`Vector3`](Vector3.md)

Returns a new Vector3 set with the Euler angles translated from the current quaternion

**`See`**

https://doc.babylonjs.com/divingDeeper/mesh/transforms/center_origin/rotation_conventions

#### Returns

[`Vector3`](Vector3.md)

a new Vector3 containing the Euler angles

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3868

___

### toEulerAnglesToRef

▸ **toEulerAnglesToRef**(`result`): [`Quaternion`](Quaternion.md)

Sets the given vector3 "result" with the Euler angles translated from the current quaternion

**`See`**

https://doc.babylonjs.com/divingDeeper/mesh/transforms/center_origin/rotation_conventions

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `result` | [`Vector3`](Vector3.md) | defines the vector which will be filled with the Euler angles |

#### Returns

[`Quaternion`](Quaternion.md)

the current unchanged quaternion

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3880

___

### toRotationMatrix

▸ **toRotationMatrix**(`result`): [`Quaternion`](Quaternion.md)

Updates the given rotation matrix with the current quaternion values

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `result` | [`Matrix`](Matrix.md) | defines the target matrix |

#### Returns

[`Quaternion`](Quaternion.md)

the current unchanged quaternion

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3915

___

### toString

▸ **toString**(): `string`

Gets a string representation for the current quaternion

#### Returns

`string`

a string with the Quaternion coordinates

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3505

___

### AreClose

▸ `Static` **AreClose**(`quat0`, `quat1`): `boolean`

Checks if the two quaternions are close to each other

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `quat0` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Quaternion`](Quaternion.md) | defines the first quaternion to check |
| `quat1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Quaternion`](Quaternion.md) | defines the second quaternion to check |

#### Returns

`boolean`

true if the two quaternions are close to each other

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4009

___

### Dot

▸ `Static` **Dot**(`left`, `right`): `number`

Returns the dot product (float) between the quaternions "left" and "right"

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `left` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Quaternion`](Quaternion.md) | defines the left operand |
| `right` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Quaternion`](Quaternion.md) | defines the right operand |

#### Returns

`number`

the dot product

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3999

___

### FromArray

▸ `Static` **FromArray**(`array`, `offset?`): [`Quaternion`](Quaternion.md)

Creates a new quaternion from data stored into an array

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `array` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)`ArrayLike``number` | defines the data source |
| `offset?` | `number` | defines the offset in the source array where the data starts |

#### Returns

[`Quaternion`](Quaternion.md)

a new quaternion

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4109

___

### FromArrayToRef

▸ `Static` **FromArrayToRef**(`array`, `offset`, `result`): `void`

Updates the given quaternion "result" from the starting index of the given array.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `array` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)`ArrayLike``number` | the array to pull values from |
| `offset` | `number` | the offset into the array to start at |
| `result` | [`Quaternion`](Quaternion.md) | the quaternion to store the result in |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4122

___

### FromEulerAngles

▸ `Static` **FromEulerAngles**(`x`, `y`, `z`): [`Quaternion`](Quaternion.md)

Create a quaternion from Euler rotation angles

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | Pitch |
| `y` | `number` | Yaw |
| `z` | `number` | Roll |

#### Returns

[`Quaternion`](Quaternion.md)

the new Quaternion

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4136

___

### FromEulerAnglesToRef

▸ `Static` **FromEulerAnglesToRef**(`x`, `y`, `z`, `result`): [`Quaternion`](Quaternion.md)

Updates a quaternion from Euler rotation angles

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | Pitch |
| `y` | `number` | Yaw |
| `z` | `number` | Roll |
| `result` | [`Quaternion`](Quaternion.md) | the quaternion to store the result |

#### Returns

[`Quaternion`](Quaternion.md)

the updated quaternion

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4150

___

### FromEulerVector

▸ `Static` **FromEulerVector**(`vec`): [`Quaternion`](Quaternion.md)

Create a quaternion from Euler rotation vector

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vec` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | the Euler vector (x Pitch, y Yaw, z Roll) |

#### Returns

[`Quaternion`](Quaternion.md)

the new Quaternion

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4160

___

### FromEulerVectorToRef

▸ `Static` **FromEulerVectorToRef**(`vec`, `result`): [`Quaternion`](Quaternion.md)

Updates a quaternion from Euler rotation vector

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vec` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | the Euler vector (x Pitch, y Yaw, z Roll) |
| `result` | [`Quaternion`](Quaternion.md) | the quaternion to store the result |

#### Returns

[`Quaternion`](Quaternion.md)

the updated quaternion

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4172

___

### FromLookDirectionLH

▸ `Static` **FromLookDirectionLH**(`forward`, `up`): [`Quaternion`](Quaternion.md)

Creates a new rotation value to orient an object to look towards the given forward direction, the up direction being oriented like "up".
This function works in left handed mode

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `forward` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the forward direction - Must be normalized and orthogonal to up. |
| `up` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the up vector for the entity - Must be normalized and orthogonal to forward. |

#### Returns

[`Quaternion`](Quaternion.md)

A new quaternion oriented toward the specified forward and up.

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4305

___

### FromLookDirectionLHToRef

▸ `Static` **FromLookDirectionLHToRef**(`forward`, `up`, `ref`): `void`

Creates a new rotation value to orient an object to look towards the given forward direction with the up direction being oriented like "up", and stores it in the target quaternion.
This function works in left handed mode

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `forward` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the forward direction - Must be normalized and orthogonal to up. |
| `up` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the up vector for the entity - Must be normalized and orthogonal to forward. |
| `ref` | [`Quaternion`](Quaternion.md) | defines the target quaternion. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4318

___

### FromLookDirectionRH

▸ `Static` **FromLookDirectionRH**(`forward`, `up`): [`Quaternion`](Quaternion.md)

Creates a new rotation value to orient an object to look towards the given forward direction, the up direction being oriented like "up".
This function works in right handed mode

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `forward` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the forward direction - Must be normalized and orthogonal to up. |
| `up` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the up vector for the entity - Must be normalized and orthogonal to forward. |

#### Returns

[`Quaternion`](Quaternion.md)

A new quaternion oriented toward the specified forward and up.

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4331

___

### FromLookDirectionRHToRef

▸ `Static` **FromLookDirectionRHToRef**(`forward`, `up`, `ref`): `void`

Creates a new rotation value to orient an object to look towards the given forward direction with the up direction being oriented like "up", and stores it in the target quaternion.
This function works in right handed mode

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `forward` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the forward direction - Must be normalized and orthogonal to up. |
| `up` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the up vector for the entity - Must be normalized and orthogonal to forward. |
| `ref` | [`Quaternion`](Quaternion.md) | defines the target quaternion. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4344

___

### FromRotationMatrix

▸ `Static` **FromRotationMatrix**(`matrix`): [`Quaternion`](Quaternion.md)

Creates a new quaternion from a rotation matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `matrix` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the source matrix |

#### Returns

[`Quaternion`](Quaternion.md)

a new quaternion created from the given rotation matrix values

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3937

___

### FromRotationMatrixToRef

▸ `Static` **FromRotationMatrixToRef**(`matrix`, `result`): `void`

Updates the given quaternion with the given rotation matrix values

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `matrix` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the source matrix |
| `result` | [`Quaternion`](Quaternion.md) | defines the target quaternion |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:3948

___

### FromUnitVectorsToRef

▸ `Static` **FromUnitVectorsToRef**(`vecFrom`, `vecTo`, `result`): [`Quaternion`](Quaternion.md)

Updates a quaternion so that it rotates vector vecFrom to vector vecTo

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vecFrom` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the direction vector from which to rotate |
| `vecTo` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the direction vector to which to rotate |
| `result` | [`Quaternion`](Quaternion.md) | the quaternion to store the result |

#### Returns

[`Quaternion`](Quaternion.md)

the updated quaternion

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4184

___

### Hermite

▸ `Static` **Hermite**(`value1`, `tangent1`, `value2`, `tangent2`, `amount`): [`Quaternion`](Quaternion.md)

Interpolate between two quaternions using Hermite interpolation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Quaternion`](Quaternion.md) | defines first quaternion |
| `tangent1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Quaternion`](Quaternion.md) | defines the incoming tangent |
| `value2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Quaternion`](Quaternion.md) | defines second quaternion |
| `tangent2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Quaternion`](Quaternion.md) | defines the outgoing tangent |
| `amount` | `number` | defines the target quaternion |

#### Returns

[`Quaternion`](Quaternion.md)

the new interpolated quaternion

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4408

___

### Hermite1stDerivative

▸ `Static` **Hermite1stDerivative**(`value1`, `tangent1`, `value2`, `tangent2`, `time`): [`Quaternion`](Quaternion.md)

Returns a new Quaternion which is the 1st derivative of the Hermite spline defined by the quaternions "value1", "value2", "tangent1", "tangent2".

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Quaternion`](Quaternion.md) | defines the first control point |
| `tangent1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Quaternion`](Quaternion.md) | defines the first tangent |
| `value2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Quaternion`](Quaternion.md) | defines the second control point |
| `tangent2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Quaternion`](Quaternion.md) | defines the second tangent |
| `time` | `number` | define where the derivative must be done |

#### Returns

[`Quaternion`](Quaternion.md)

1st derivative

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4438

___

### Hermite1stDerivativeToRef

▸ `Static` **Hermite1stDerivativeToRef**(`value1`, `tangent1`, `value2`, `tangent2`, `time`, `result`): `void`

Update a Quaternion with the 1st derivative of the Hermite spline defined by the quaternions "value1", "value2", "tangent1", "tangent2".

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Quaternion`](Quaternion.md) | defines the first control point |
| `tangent1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Quaternion`](Quaternion.md) | defines the first tangent |
| `value2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Quaternion`](Quaternion.md) | defines the second control point |
| `tangent2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Quaternion`](Quaternion.md) | defines the second tangent |
| `time` | `number` | define where the derivative must be done |
| `result` | [`Quaternion`](Quaternion.md) | define where to store the derivative |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4461

___

### Identity

▸ `Static` **Identity**(): [`Quaternion`](Quaternion.md)

Creates an identity quaternion

#### Returns

[`Quaternion`](Quaternion.md)

the identity quaternion

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4063

___

### Inverse

▸ `Static` **Inverse**(`q`): [`Quaternion`](Quaternion.md)

Inverse a given quaternion

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `q` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Quaternion`](Quaternion.md) | defines the source quaternion |

#### Returns

[`Quaternion`](Quaternion.md)

a new quaternion as the inverted current quaternion

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4044

___

### InverseToRef

▸ `Static` **InverseToRef**(`q`, `result`): [`Quaternion`](Quaternion.md)

Inverse a given quaternion

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `q` | [`Quaternion`](Quaternion.md) | defines the source quaternion |
| `result` | [`Quaternion`](Quaternion.md) | the quaternion the result will be stored in |

#### Returns

[`Quaternion`](Quaternion.md)

the result quaternion

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4054

___

### IsIdentity

▸ `Static` **IsIdentity**(`quaternion`): `boolean`

Gets a boolean indicating if the given quaternion is identity

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `quaternion` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Quaternion`](Quaternion.md) | defines the quaternion to check |

#### Returns

`boolean`

true if the quaternion is identity

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4072

___

### RotationAlphaBetaGamma

▸ `Static` **RotationAlphaBetaGamma**(`alpha`, `beta`, `gamma`): [`Quaternion`](Quaternion.md)

Creates a new quaternion from the given Euler float angles expressed in z-x-z orientation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `alpha` | `number` | defines the rotation around first axis |
| `beta` | `number` | defines the rotation around second axis |
| `gamma` | `number` | defines the rotation around third axis |

#### Returns

[`Quaternion`](Quaternion.md)

the new quaternion

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4247

___

### RotationAlphaBetaGammaToRef

▸ `Static` **RotationAlphaBetaGammaToRef**(`alpha`, `beta`, `gamma`, `result`): `void`

Creates a new quaternion from the given Euler float angles expressed in z-x-z orientation and stores it in the target quaternion

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `alpha` | `number` | defines the rotation around first axis |
| `beta` | `number` | defines the rotation around second axis |
| `gamma` | `number` | defines the rotation around third axis |
| `result` | [`Quaternion`](Quaternion.md) | defines the target quaternion |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4260

___

### RotationAxis

▸ `Static` **RotationAxis**(`axis`, `angle`): [`Quaternion`](Quaternion.md)

Creates a quaternion from a rotation around an axis

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `axis` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the axis to use |
| `angle` | `number` | defines the angle to use |

#### Returns

[`Quaternion`](Quaternion.md)

a new quaternion created from the given axis (Vector3) and angle in radians (float)

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4082

___

### RotationAxisToRef

▸ `Static` **RotationAxisToRef**(`axis`, `angle`, `result`): [`Quaternion`](Quaternion.md)

Creates a rotation around an axis and stores it into the given quaternion

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `axis` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the axis to use |
| `angle` | `number` | defines the angle to use |
| `result` | [`Quaternion`](Quaternion.md) | defines the target quaternion |

#### Returns

[`Quaternion`](Quaternion.md)

the target quaternion

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4093

___

### RotationQuaternionFromAxis

▸ `Static` **RotationQuaternionFromAxis**(`axis1`, `axis2`, `axis3`): [`Quaternion`](Quaternion.md)

Creates a new quaternion containing the rotation value to reach the target (axis1, axis2, axis3) orientation as a rotated XYZ system (axis1, axis2 and axis3 are normalized during this operation)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `axis1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the first axis |
| `axis2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the second axis |
| `axis3` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the third axis |

#### Returns

[`Quaternion`](Quaternion.md)

the new quaternion

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4279

___

### RotationQuaternionFromAxisToRef

▸ `Static` **RotationQuaternionFromAxisToRef**(`axis1`, `axis2`, `axis3`, `ref`): `void`

Creates a rotation value to reach the target (axis1, axis2, axis3) orientation as a rotated XYZ system (axis1, axis2 and axis3 are normalized during this operation) and stores it in the target quaternion

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `axis1` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the first axis |
| `axis2` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the second axis |
| `axis3` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the third axis |
| `ref` | [`Quaternion`](Quaternion.md) | defines the target quaternion |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4292

___

### RotationYawPitchRoll

▸ `Static` **RotationYawPitchRoll**(`yaw`, `pitch`, `roll`): [`Quaternion`](Quaternion.md)

Creates a new quaternion from the given Euler float angles (y, x, z)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `yaw` | `number` | defines the rotation around Y axis |
| `pitch` | `number` | defines the rotation around X axis |
| `roll` | `number` | defines the rotation around Z axis |

#### Returns

[`Quaternion`](Quaternion.md)

the new quaternion

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4208

___

### RotationYawPitchRollToRef

▸ `Static` **RotationYawPitchRollToRef**(`yaw`, `pitch`, `roll`, `result`): `void`

Creates a new rotation from the given Euler float angles (y, x, z) and stores it in the target quaternion

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `yaw` | `number` | defines the rotation around Y axis |
| `pitch` | `number` | defines the rotation around X axis |
| `roll` | `number` | defines the rotation around Z axis |
| `result` | [`Quaternion`](Quaternion.md) | defines the target quaternion |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4221

___

### Slerp

▸ `Static` **Slerp**(`left`, `right`, `amount`): [`Quaternion`](Quaternion.md)

Interpolates between two quaternions

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `left` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Quaternion`](Quaternion.md) | defines first quaternion |
| `right` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Quaternion`](Quaternion.md) | defines second quaternion |
| `amount` | `number` | defines the gradient to use |

#### Returns

[`Quaternion`](Quaternion.md)

the new interpolated quaternion

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4357

___

### SlerpToRef

▸ `Static` **SlerpToRef**(`left`, `right`, `amount`, `result`): `void`

Interpolates between two quaternions and stores it into a target quaternion

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `left` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Quaternion`](Quaternion.md) | defines first quaternion |
| `right` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Quaternion`](Quaternion.md) | defines second quaternion |
| `amount` | `number` | defines the gradient to use |
| `result` | [`Quaternion`](Quaternion.md) | defines the target quaternion |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4372

___

### SmoothToRef

▸ `Static` **SmoothToRef**(`source`, `goal`, `deltaTime`, `lerpTime`, `result`): `void`

Smooth interpolation between two quaternions using Slerp

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | [`Quaternion`](Quaternion.md) | source quaternion |
| `goal` | [`Quaternion`](Quaternion.md) | goal quaternion |
| `deltaTime` | `number` | current interpolation frame |
| `lerpTime` | `number` | total interpolation time |
| `result` | [`Quaternion`](Quaternion.md) | the smoothed quaternion |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4024

___

### Zero

▸ `Static` **Zero**(): [`Quaternion`](Quaternion.md)

Creates an empty quaternion

#### Returns

[`Quaternion`](Quaternion.md)

a new quaternion set to (0.0, 0.0, 0.0)

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4035
