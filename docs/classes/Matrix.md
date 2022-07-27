[@dev/core](../README.md) / [Exports](../modules.md) / Matrix

# Class: Matrix

Class used to store matrix data (4x4)

## Table of contents

### Constructors

- [constructor](Matrix.md#constructor)

### Properties

- [\_isIdentity](Matrix.md#_isidentity)
- [\_isIdentity3x2](Matrix.md#_isidentity3x2)
- [\_isIdentity3x2Dirty](Matrix.md#_isidentity3x2dirty)
- [\_isIdentityDirty](Matrix.md#_isidentitydirty)
- [\_m](Matrix.md#_m)
- [updateFlag](Matrix.md#updateflag)
- [\_IdentityReadOnly](Matrix.md#_identityreadonly)
- [\_UpdateFlagSeed](Matrix.md#_updateflagseed)

### Accessors

- [m](Matrix.md#m)
- [IdentityReadOnly](Matrix.md#identityreadonly)
- [Use64Bits](Matrix.md#use64bits)

### Methods

- [\_updateIdentityStatus](Matrix.md#_updateidentitystatus)
- [add](Matrix.md#add)
- [addAtIndex](Matrix.md#addatindex)
- [addToRef](Matrix.md#addtoref)
- [addToSelf](Matrix.md#addtoself)
- [addTranslationFromFloats](Matrix.md#addtranslationfromfloats)
- [asArray](Matrix.md#asarray)
- [clone](Matrix.md#clone)
- [copyFrom](Matrix.md#copyfrom)
- [copyToArray](Matrix.md#copytoarray)
- [decompose](Matrix.md#decompose)
- [decomposeToTransformNode](Matrix.md#decomposetotransformnode)
- [determinant](Matrix.md#determinant)
- [equals](Matrix.md#equals)
- [getClassName](Matrix.md#getclassname)
- [getHashCode](Matrix.md#gethashcode)
- [getRotationMatrix](Matrix.md#getrotationmatrix)
- [getRotationMatrixToRef](Matrix.md#getrotationmatrixtoref)
- [getRow](Matrix.md#getrow)
- [getTranslation](Matrix.md#gettranslation)
- [getTranslationToRef](Matrix.md#gettranslationtoref)
- [invert](Matrix.md#invert)
- [invertToRef](Matrix.md#inverttoref)
- [isIdentity](Matrix.md#isidentity)
- [isIdentityAs3x2](Matrix.md#isidentityas3x2)
- [markAsUpdated](Matrix.md#markasupdated)
- [multiply](Matrix.md#multiply)
- [multiplyAtIndex](Matrix.md#multiplyatindex)
- [multiplyToArray](Matrix.md#multiplytoarray)
- [multiplyToRef](Matrix.md#multiplytoref)
- [removeRotationAndScaling](Matrix.md#removerotationandscaling)
- [reset](Matrix.md#reset)
- [scale](Matrix.md#scale)
- [scaleAndAddToRef](Matrix.md#scaleandaddtoref)
- [scaleToRef](Matrix.md#scaletoref)
- [setRow](Matrix.md#setrow)
- [setRowFromFloats](Matrix.md#setrowfromfloats)
- [setTranslation](Matrix.md#settranslation)
- [setTranslationFromFloats](Matrix.md#settranslationfromfloats)
- [toArray](Matrix.md#toarray)
- [toNormalMatrix](Matrix.md#tonormalmatrix)
- [toggleModelMatrixHandInPlace](Matrix.md#togglemodelmatrixhandinplace)
- [toggleProjectionMatrixHandInPlace](Matrix.md#toggleprojectionmatrixhandinplace)
- [transpose](Matrix.md#transpose)
- [transposeToRef](Matrix.md#transposetoref)
- [Compose](Matrix.md#compose)
- [ComposeToRef](Matrix.md#composetoref)
- [DecomposeLerp](Matrix.md#decomposelerp)
- [DecomposeLerpToRef](Matrix.md#decomposelerptoref)
- [FromArray](Matrix.md#fromarray)
- [FromArrayToRef](Matrix.md#fromarraytoref)
- [FromFloat32ArrayToRefScaled](Matrix.md#fromfloat32arraytorefscaled)
- [FromQuaternionToRef](Matrix.md#fromquaterniontoref)
- [FromValues](Matrix.md#fromvalues)
- [FromValuesToRef](Matrix.md#fromvaluestoref)
- [FromXYZAxesToRef](Matrix.md#fromxyzaxestoref)
- [GetAsMatrix2x2](Matrix.md#getasmatrix2x2)
- [GetAsMatrix3x3](Matrix.md#getasmatrix3x3)
- [GetFinalMatrix](Matrix.md#getfinalmatrix)
- [Identity](Matrix.md#identity)
- [IdentityToRef](Matrix.md#identitytoref)
- [Invert](Matrix.md#invert-1)
- [Lerp](Matrix.md#lerp)
- [LerpToRef](Matrix.md#lerptoref)
- [LookAtLH](Matrix.md#lookatlh)
- [LookAtLHToRef](Matrix.md#lookatlhtoref)
- [LookAtRH](Matrix.md#lookatrh)
- [LookAtRHToRef](Matrix.md#lookatrhtoref)
- [LookDirectionLH](Matrix.md#lookdirectionlh)
- [LookDirectionLHToRef](Matrix.md#lookdirectionlhtoref)
- [LookDirectionRH](Matrix.md#lookdirectionrh)
- [LookDirectionRHToRef](Matrix.md#lookdirectionrhtoref)
- [OrthoLH](Matrix.md#ortholh)
- [OrthoLHToRef](Matrix.md#ortholhtoref)
- [OrthoOffCenterLH](Matrix.md#orthooffcenterlh)
- [OrthoOffCenterLHToRef](Matrix.md#orthooffcenterlhtoref)
- [OrthoOffCenterRH](Matrix.md#orthooffcenterrh)
- [OrthoOffCenterRHToRef](Matrix.md#orthooffcenterrhtoref)
- [PerspectiveFovLH](Matrix.md#perspectivefovlh)
- [PerspectiveFovLHToRef](Matrix.md#perspectivefovlhtoref)
- [PerspectiveFovRH](Matrix.md#perspectivefovrh)
- [PerspectiveFovRHToRef](Matrix.md#perspectivefovrhtoref)
- [PerspectiveFovReverseLHToRef](Matrix.md#perspectivefovreverselhtoref)
- [PerspectiveFovReverseRHToRef](Matrix.md#perspectivefovreverserhtoref)
- [PerspectiveFovWebVRToRef](Matrix.md#perspectivefovwebvrtoref)
- [PerspectiveLH](Matrix.md#perspectivelh)
- [Reflection](Matrix.md#reflection)
- [ReflectionToRef](Matrix.md#reflectiontoref)
- [RotationAlignToRef](Matrix.md#rotationaligntoref)
- [RotationAxis](Matrix.md#rotationaxis)
- [RotationAxisToRef](Matrix.md#rotationaxistoref)
- [RotationX](Matrix.md#rotationx)
- [RotationXToRef](Matrix.md#rotationxtoref)
- [RotationY](Matrix.md#rotationy)
- [RotationYToRef](Matrix.md#rotationytoref)
- [RotationYawPitchRoll](Matrix.md#rotationyawpitchroll)
- [RotationYawPitchRollToRef](Matrix.md#rotationyawpitchrolltoref)
- [RotationZ](Matrix.md#rotationz)
- [RotationZToRef](Matrix.md#rotationztoref)
- [Scaling](Matrix.md#scaling)
- [ScalingToRef](Matrix.md#scalingtoref)
- [Translation](Matrix.md#translation)
- [TranslationToRef](Matrix.md#translationtoref)
- [Transpose](Matrix.md#transpose-1)
- [TransposeToRef](Matrix.md#transposetoref-1)
- [Zero](Matrix.md#zero)

## Constructors

### constructor

• **new Matrix**()

Creates an empty matrix (filled with zeros)

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4533

## Properties

### \_isIdentity

• `Private` **\_isIdentity**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4492

___

### \_isIdentity3x2

• `Private` **\_isIdentity3x2**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4494

___

### \_isIdentity3x2Dirty

• `Private` **\_isIdentity3x2Dirty**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4495

___

### \_isIdentityDirty

• `Private` **\_isIdentityDirty**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4493

___

### \_m

• `Private` `Readonly` **\_m**: `number`[] \| `Float32Array`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4503

___

### updateFlag

• **updateFlag**: `number` = `-1`

Gets the update flag of the matrix which is an unique number for the matrix.
It will be incremented every time the matrix data change.
You can use it to speed the comparison between two versions of the same matrix.

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4501

___

### \_IdentityReadOnly

▪ `Static` `Private` **\_IdentityReadOnly**: [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md)

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4490

___

### \_UpdateFlagSeed

▪ `Static` `Private` **\_UpdateFlagSeed**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4489

## Accessors

### m

• `get` **m**(): [`DeepImmutableObject`](../modules.md#deepimmutableobject)`Float32Array` \| `DeepImmutableArray``number`

Gets the internal data of the matrix

#### Returns

[`DeepImmutableObject`](../modules.md#deepimmutableobject)`Float32Array` \| `DeepImmutableArray``number`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4508

___

### IdentityReadOnly

• `Static` `get` **IdentityReadOnly**(): [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md)

Gets an identity matrix that must not be updated

#### Returns

[`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md)

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5446

___

### Use64Bits

• `Static` `get` **Use64Bits**(): `boolean`

Gets the precision of matrix computations

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4485

## Methods

### \_updateIdentityStatus

▸ `Private` **_updateIdentityStatus**(`isIdentity`, `isIdentityDirty?`, `isIdentity3x2?`, `isIdentity3x2Dirty?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `isIdentity` | `boolean` | `undefined` |
| `isIdentityDirty` | `boolean` | `false` |
| `isIdentity3x2` | `boolean` | `false` |
| `isIdentity3x2Dirty` | `boolean` | `true` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4523

___

### add

▸ **add**(`other`): [`Matrix`](Matrix.md)

Adds the current matrix with a second one

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the matrix to add |

#### Returns

[`Matrix`](Matrix.md)

a new matrix as the addition of the current matrix and the given one

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4697

___

### addAtIndex

▸ **addAtIndex**(`index`, `value`): [`Matrix`](Matrix.md)

add a value at the specified position in the current Matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | the index of the value within the matrix. between 0 and 15. |
| `value` | `number` | the value to be added |

#### Returns

[`Matrix`](Matrix.md)

the current updated matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4843

___

### addToRef

▸ **addToRef**(`other`, `result`): [`Matrix`](Matrix.md)

Sets the given matrix "result" to the addition of the current matrix and the given one

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the matrix to add |
| `result` | [`Matrix`](Matrix.md) | defines the target matrix |

#### Returns

[`Matrix`](Matrix.md)

the current matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4709

___

### addToSelf

▸ **addToSelf**(`other`): [`Matrix`](Matrix.md)

Adds in place the given matrix to the current matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the second operand |

#### Returns

[`Matrix`](Matrix.md)

the current updated matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4725

___

### addTranslationFromFloats

▸ **addTranslationFromFloats**(`x`, `y`, `z`): [`Matrix`](Matrix.md)

Adds the translation vector (using 3 floats) in the current matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | defines the 1st component of the translation |
| `y` | `number` | defines the 2nd component of the translation |
| `z` | `number` | defines the 3rd component of the translation |

#### Returns

[`Matrix`](Matrix.md)

the current updated matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4883

___

### asArray

▸ **asArray**(): [`DeepImmutableObject`](../modules.md#deepimmutableobject)`Float32Array` \| `DeepImmutableArray``number`

Returns the matrix as a Float32Array or Array

#### Returns

[`DeepImmutableObject`](../modules.md#deepimmutableobject)`Float32Array` \| `DeepImmutableArray``number`

the matrix underlying array.

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4670

___

### clone

▸ **clone**(): [`Matrix`](Matrix.md)

Clone the current matrix

#### Returns

[`Matrix`](Matrix.md)

a new matrix from the current matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5113

___

### copyFrom

▸ **copyFrom**(`other`): [`Matrix`](Matrix.md)

Copy the current matrix from the given one

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the source matrix |

#### Returns

[`Matrix`](Matrix.md)

the current updated matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4947

___

### copyToArray

▸ **copyToArray**(`array`, `offset?`): [`Matrix`](Matrix.md)

Populates the given array from the starting index with the current matrix values

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `array` | `number`[] \| `Float32Array` | `undefined` | defines the target array |
| `offset` | `number` | `0` | defines the offset in the target array where to start storing values |

#### Returns

[`Matrix`](Matrix.md)

the current matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4961

___

### decompose

▸ **decompose**(`scale?`, `rotation?`, `translation?`, `preserveScalingNode?`): `boolean`

Decomposes the current Matrix into a translation, rotation and scaling components

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scale?` | [`Vector3`](Vector3.md) | defines the scale vector3 given as a reference to update |
| `rotation?` | [`Quaternion`](Quaternion.md) | defines the rotation quaternion given as a reference to update |
| `translation?` | [`Vector3`](Vector3.md) | defines the translation vector3 given as a reference to update |
| `preserveScalingNode?` | [`TransformNode`](TransformNode.md) | Use scaling sign coming from this node. Otherwise scaling sign might change. |

#### Returns

`boolean`

true if operation was successful

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5157

___

### decomposeToTransformNode

▸ **decomposeToTransformNode**(`node`): `boolean`

Decomposes the current Matrix into a translation, rotation and scaling components of the provided node

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `node` | [`TransformNode`](TransformNode.md) | the node to decompose the matrix to |

#### Returns

`boolean`

true if operation was successful

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5144

___

### determinant

▸ **determinant**(): `number`

Gets the determinant of the matrix

#### Returns

`number`

the matrix determinant

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4612

___

### equals

▸ **equals**(`value`): `boolean`

Check equality between this matrix and a second one

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the second matrix to compare |

#### Returns

`boolean`

true is the current matrix and the given one values are strictly equal

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5075

___

### getClassName

▸ **getClassName**(): `string`

Returns the name of the current matrix class

#### Returns

`string`

the string "Matrix"

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5123

___

### getHashCode

▸ **getHashCode**(): `number`

Gets the hash code of the current matrix

#### Returns

`number`

the hash code

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5131

___

### getRotationMatrix

▸ **getRotationMatrix**(): [`Matrix`](Matrix.md)

Gets only rotation part of the current matrix

#### Returns

[`Matrix`](Matrix.md)

a new matrix sets to the extracted rotation matrix from the current one

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5352

___

### getRotationMatrixToRef

▸ **getRotationMatrixToRef**(`result`): [`Matrix`](Matrix.md)

Extracts the rotation matrix from the current one and sets it as the given "result"

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `result` | [`Matrix`](Matrix.md) | defines the target matrix to store data to |

#### Returns

[`Matrix`](Matrix.md)

the current matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5363

___

### getRow

▸ **getRow**(`index`): [`Nullable`](../modules.md#nullable)[`Vector4`](Vector4.md)

Gets specific row of the matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | defines the number of the row to get |

#### Returns

[`Nullable`](../modules.md#nullable)[`Vector4`](Vector4.md)

the index-th row of the current matrix as a new Vector4

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5238

___

### getTranslation

▸ **getTranslation**(): [`Vector3`](Vector3.md)

Gets the translation value of the current matrix

#### Returns

[`Vector3`](Vector3.md)

a new Vector3 as the extracted translation from the matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4904

___

### getTranslationToRef

▸ **getTranslationToRef**(`result`): [`Matrix`](Matrix.md)

Fill a Vector3 with the extracted translation from the matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `result` | [`Vector3`](Vector3.md) | defines the Vector3 where to store the translation |

#### Returns

[`Matrix`](Matrix.md)

the current matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4913

___

### invert

▸ **invert**(): [`Matrix`](Matrix.md)

Inverts the current matrix in place

#### Returns

[`Matrix`](Matrix.md)

the current inverted matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4678

___

### invertToRef

▸ **invertToRef**(`other`): [`Matrix`](Matrix.md)

Sets the given matrix to the current inverted Matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`Matrix`](Matrix.md) | defines the target matrix |

#### Returns

[`Matrix`](Matrix.md)

the unmodified current matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4740

___

### isIdentity

▸ **isIdentity**(): `boolean`

Check if the current matrix is identity

#### Returns

`boolean`

true is the matrix is the identity matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4549

___

### isIdentityAs3x2

▸ **isIdentityAs3x2**(): `boolean`

Check if the current matrix is identity as a texture matrix (3x2 store in 4x4)

#### Returns

`boolean`

true is the matrix is the identity matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4579

___

### markAsUpdated

▸ **markAsUpdated**(): `void`

Update the updateFlag to indicate that the matrix has been updated

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4515

___

### multiply

▸ **multiply**(`other`): [`Matrix`](Matrix.md)

Multiply two matrices

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the second operand |

#### Returns

[`Matrix`](Matrix.md)

a new matrix set with the multiplication result of the current Matrix and the given one

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4936

___

### multiplyAtIndex

▸ **multiplyAtIndex**(`index`, `value`): [`Matrix`](Matrix.md)

mutiply the specified position in the current Matrix by a value

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | the index of the value within the matrix. between 0 and 15. |
| `value` | `number` | the value to be added |

#### Returns

[`Matrix`](Matrix.md)

the current updated matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4855

___

### multiplyToArray

▸ **multiplyToArray**(`other`, `result`, `offset`): [`Matrix`](Matrix.md)

Sets the Float32Array "result" from the given index "offset" with the multiplication of the current matrix and the given one

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the second operand |
| `result` | `number`[] \| `Float32Array` | defines the array where to store the multiplication |
| `offset` | `number` | defines the offset in the target array where to start storing values |

#### Returns

[`Matrix`](Matrix.md)

the current matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5011

___

### multiplyToRef

▸ **multiplyToRef**(`other`, `result`): [`Matrix`](Matrix.md)

Sets the given matrix "result" with the multiplication result of the current Matrix and the given one

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the second operand |
| `result` | [`Matrix`](Matrix.md) | defines the matrix where to store the multiplication |

#### Returns

[`Matrix`](Matrix.md)

the current matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4989

___

### removeRotationAndScaling

▸ **removeRotationAndScaling**(): [`Matrix`](Matrix.md)

Remove rotation and scaling part from the matrix

#### Returns

[`Matrix`](Matrix.md)

the updated matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4924

___

### reset

▸ **reset**(): [`Matrix`](Matrix.md)

Sets all the matrix elements to zero

#### Returns

[`Matrix`](Matrix.md)

the current matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4686

___

### scale

▸ **scale**(`scale`): [`Matrix`](Matrix.md)

Compute a new matrix set with the current matrix values multiplied by scale (float)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scale` | `number` | defines the scale factor |

#### Returns

[`Matrix`](Matrix.md)

a new matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5302

___

### scaleAndAddToRef

▸ **scaleAndAddToRef**(`scale`, `result`): [`Matrix`](Matrix.md)

Scale the current matrix values by a factor and add the result to a given matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scale` | `number` | defines the scale factor |
| `result` | [`Matrix`](Matrix.md) | defines the Matrix to store the result |

#### Returns

[`Matrix`](Matrix.md)

the current matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5328

___

### scaleToRef

▸ **scaleToRef**(`scale`, `result`): [`Matrix`](Matrix.md)

Scale the current matrix values by a factor to a given result matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scale` | `number` | defines the scale factor |
| `result` | [`Matrix`](Matrix.md) | defines the matrix to store the result |

#### Returns

[`Matrix`](Matrix.md)

the current matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5314

___

### setRow

▸ **setRow**(`index`, `row`): [`Matrix`](Matrix.md)

Sets the index-th row of the current matrix to the vector4 values

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | defines the number of the row to set |
| `row` | [`Vector4`](Vector4.md) | defines the target vector4 |

#### Returns

[`Matrix`](Matrix.md)

the updated current matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5252

___

### setRowFromFloats

▸ **setRowFromFloats**(`index`, `x`, `y`, `z`, `w`): [`Matrix`](Matrix.md)

Sets the index-th row of the current matrix with the given 4 x float values

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | defines the row index |
| `x` | `number` | defines the x component to set |
| `y` | `number` | defines the y component to set |
| `z` | `number` | defines the z component to set |
| `w` | `number` | defines the w component to set |

#### Returns

[`Matrix`](Matrix.md)

the updated current matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5283

___

### setTranslation

▸ **setTranslation**(`vector3`): [`Matrix`](Matrix.md)

Inserts the translation vector in the current matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vector3` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the translation to insert |

#### Returns

[`Matrix`](Matrix.md)

the current updated matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4896

___

### setTranslationFromFloats

▸ **setTranslationFromFloats**(`x`, `y`, `z`): [`Matrix`](Matrix.md)

Inserts the translation vector (using 3 floats) in the current matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | defines the 1st component of the translation |
| `y` | `number` | defines the 2nd component of the translation |
| `z` | `number` | defines the 3rd component of the translation |

#### Returns

[`Matrix`](Matrix.md)

the current updated matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4868

___

### toArray

▸ **toArray**(): [`DeepImmutableObject`](../modules.md#deepimmutableobject)`Float32Array` \| `DeepImmutableArray``number`

Returns the matrix as a Float32Array or Array

#### Returns

[`DeepImmutableObject`](../modules.md#deepimmutableobject)`Float32Array` \| `DeepImmutableArray``number`

the matrix underlying array

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:4663

___

### toNormalMatrix

▸ **toNormalMatrix**(`ref`): `void`

Writes to the given matrix a normal matrix, computed from this one (using values from identity matrix for fourth row and column).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ref` | [`Matrix`](Matrix.md) | matrix to store the result |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5340

___

### toggleModelMatrixHandInPlace

▸ **toggleModelMatrixHandInPlace**(): `void`

Toggles model matrix from being right handed to left handed in place and vice versa

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5381

___

### toggleProjectionMatrixHandInPlace

▸ **toggleProjectionMatrixHandInPlace**(): `void`

Toggles projection matrix from being right handed to left handed in place and vice versa

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5394

___

### transpose

▸ **transpose**(): [`Matrix`](Matrix.md)

Compute the transpose of the matrix

#### Returns

[`Matrix`](Matrix.md)

the new transposed matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5260

___

### transposeToRef

▸ **transposeToRef**(`result`): [`Matrix`](Matrix.md)

Compute the transpose of the matrix and store it in a given matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `result` | [`Matrix`](Matrix.md) | defines the target matrix |

#### Returns

[`Matrix`](Matrix.md)

the current matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5269

___

### Compose

▸ `Static` **Compose**(`scale`, `rotation`, `translation`): [`Matrix`](Matrix.md)

Creates a new matrix composed by merging scale (vector3), rotation (quaternion) and translation (vector3)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scale` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the scale vector3 |
| `rotation` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Quaternion`](Quaternion.md) | defines the rotation quaternion |
| `translation` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the translation vector3 |

#### Returns

[`Matrix`](Matrix.md)

a new matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5577

___

### ComposeToRef

▸ `Static` **ComposeToRef**(`scale`, `rotation`, `translation`, `result`): `void`

Sets a matrix to a value composed by merging scale (vector3), rotation (quaternion) and translation (vector3)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scale` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the scale vector3 |
| `rotation` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Quaternion`](Quaternion.md) | defines the rotation quaternion |
| `translation` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the translation vector3 |
| `result` | [`Matrix`](Matrix.md) | defines the target matrix |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5590

___

### DecomposeLerp

▸ `Static` **DecomposeLerp**(`startValue`, `endValue`, `gradient`): [`Matrix`](Matrix.md)

Builds a new matrix whose values are computed by:
* decomposing the the "startValue" and "endValue" matrices into their respective scale, rotation and translation matrices
* interpolating for "gradient" (float) the values between each of these decomposed matrices between the start and the end
* recomposing a new matrix from these 3 interpolated scale, rotation and translation matrices

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `startValue` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the first matrix |
| `endValue` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the second matrix |
| `gradient` | `number` | defines the gradient between the two matrices |

#### Returns

[`Matrix`](Matrix.md)

the new matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5961

___

### DecomposeLerpToRef

▸ `Static` **DecomposeLerpToRef**(`startValue`, `endValue`, `gradient`, `result`): `void`

Update a matrix to values which are computed by:
* decomposing the the "startValue" and "endValue" matrices into their respective scale, rotation and translation matrices
* interpolating for "gradient" (float) the values between each of these decomposed matrices between the start and the end
* recomposing a new matrix from these 3 interpolated scale, rotation and translation matrices

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `startValue` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the first matrix |
| `endValue` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the second matrix |
| `gradient` | `number` | defines the gradient between the two matrices |
| `result` | [`Matrix`](Matrix.md) | defines the target matrix |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5977

___

### FromArray

▸ `Static` **FromArray**(`array`, `offset?`): [`Matrix`](Matrix.md)

Creates a matrix from an array

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `array` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)`ArrayLike``number` | `undefined` | defines the source array |
| `offset` | `number` | `0` | defines an offset in the source array |

#### Returns

[`Matrix`](Matrix.md)

a new Matrix set from the starting index of the given array

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5410

___

### FromArrayToRef

▸ `Static` **FromArrayToRef**(`array`, `offset`, `result`): `void`

Copy the content of an array into a given matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `array` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)`ArrayLike``number` | defines the source array |
| `offset` | `number` | defines an offset in the source array |
| `result` | [`Matrix`](Matrix.md) | defines the target matrix |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5422

___

### FromFloat32ArrayToRefScaled

▸ `Static` **FromFloat32ArrayToRefScaled**(`array`, `offset`, `scale`, `result`): `void`

Stores an array into a matrix after having multiplied each component by a given factor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `array` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)`Float32Array` \| `DeepImmutableArray``number` | defines the source array |
| `offset` | `number` | defines the offset in the source array |
| `scale` | `number` | defines the scaling factor |
| `result` | [`Matrix`](Matrix.md) | defines the target matrix |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5436

___

### FromQuaternionToRef

▸ `Static` **FromQuaternionToRef**(`quat`, `result`): `void`

Creates a rotation matrix from a quaternion and stores it in a target matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `quat` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Quaternion`](Quaternion.md) | defines the quaternion to use |
| `result` | [`Matrix`](Matrix.md) | defines the target matrix |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:6737

___

### FromValues

▸ `Static` **FromValues**(`initialM11`, `initialM12`, `initialM13`, `initialM14`, `initialM21`, `initialM22`, `initialM23`, `initialM24`, `initialM31`, `initialM32`, `initialM33`, `initialM34`, `initialM41`, `initialM42`, `initialM43`, `initialM44`): [`Matrix`](Matrix.md)

Creates new matrix from a list of values (16)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `initialM11` | `number` | defines 1st value of 1st row |
| `initialM12` | `number` | defines 2nd value of 1st row |
| `initialM13` | `number` | defines 3rd value of 1st row |
| `initialM14` | `number` | defines 4th value of 1st row |
| `initialM21` | `number` | defines 1st value of 2nd row |
| `initialM22` | `number` | defines 2nd value of 2nd row |
| `initialM23` | `number` | defines 3rd value of 2nd row |
| `initialM24` | `number` | defines 4th value of 2nd row |
| `initialM31` | `number` | defines 1st value of 3rd row |
| `initialM32` | `number` | defines 2nd value of 3rd row |
| `initialM33` | `number` | defines 3rd value of 3rd row |
| `initialM34` | `number` | defines 4th value of 3rd row |
| `initialM41` | `number` | defines 1st value of 4th row |
| `initialM42` | `number` | defines 2nd value of 4th row |
| `initialM43` | `number` | defines 3rd value of 4th row |
| `initialM44` | `number` | defines 4th value of 4th row |

#### Returns

[`Matrix`](Matrix.md)

the new matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5530

___

### FromValuesToRef

▸ `Static` **FromValuesToRef**(`initialM11`, `initialM12`, `initialM13`, `initialM14`, `initialM21`, `initialM22`, `initialM23`, `initialM24`, `initialM31`, `initialM32`, `initialM33`, `initialM34`, `initialM41`, `initialM42`, `initialM43`, `initialM44`, `result`): `void`

Stores a list of values (16) inside a given matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `initialM11` | `number` | defines 1st value of 1st row |
| `initialM12` | `number` | defines 2nd value of 1st row |
| `initialM13` | `number` | defines 3rd value of 1st row |
| `initialM14` | `number` | defines 4th value of 1st row |
| `initialM21` | `number` | defines 1st value of 2nd row |
| `initialM22` | `number` | defines 2nd value of 2nd row |
| `initialM23` | `number` | defines 3rd value of 2nd row |
| `initialM24` | `number` | defines 4th value of 2nd row |
| `initialM31` | `number` | defines 1st value of 3rd row |
| `initialM32` | `number` | defines 2nd value of 3rd row |
| `initialM33` | `number` | defines 3rd value of 3rd row |
| `initialM34` | `number` | defines 4th value of 3rd row |
| `initialM41` | `number` | defines 1st value of 4th row |
| `initialM42` | `number` | defines 2nd value of 4th row |
| `initialM43` | `number` | defines 3rd value of 4th row |
| `initialM44` | `number` | defines 4th value of 4th row |
| `result` | [`Matrix`](Matrix.md) | defines the target matrix |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5470

___

### FromXYZAxesToRef

▸ `Static` **FromXYZAxesToRef**(`xaxis`, `yaxis`, `zaxis`, `result`): `void`

Sets the given matrix as a rotation matrix composed from the 3 left handed axes

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `xaxis` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the value of the 1st axis |
| `yaxis` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the value of the 2nd axis |
| `zaxis` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the value of the 3rd axis |
| `result` | [`Matrix`](Matrix.md) | defines the target matrix |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:6728

___

### GetAsMatrix2x2

▸ `Static` **GetAsMatrix2x2**(`matrix`): `number`[] \| `Float32Array`

Extracts a 2x2 matrix from a given matrix and store the result in a Float32Array

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `matrix` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the matrix to use |

#### Returns

`number`[] \| `Float32Array`

a new Float32Array array with 4 elements : the 2x2 matrix extracted from the given matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:6615

___

### GetAsMatrix3x3

▸ `Static` **GetAsMatrix3x3**(`matrix`): `number`[] \| `Float32Array`

Extracts a 3x3 matrix from a given matrix and store the result in a Float32Array

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `matrix` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the matrix to use |

#### Returns

`number`[] \| `Float32Array`

a new Float32Array array with 9 elements : the 3x3 matrix extracted from the given matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:6625

___

### GetFinalMatrix

▸ `Static` **GetFinalMatrix**(`viewport`, `world`, `view`, `projection`, `zmin`, `zmax`): [`Matrix`](Matrix.md)

Computes a complete transformation matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `viewport` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Viewport`](Viewport.md) | defines the viewport to use |
| `world` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the world matrix |
| `view` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the view matrix |
| `projection` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the projection matrix |
| `zmin` | `number` | defines the near clip plane |
| `zmax` | `number` | defines the far clip plane |

#### Returns

[`Matrix`](Matrix.md)

the transformation matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:6589

___

### Identity

▸ `Static` **Identity**(): [`Matrix`](Matrix.md)

Creates a new identity matrix

#### Returns

[`Matrix`](Matrix.md)

a new identity matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5640

___

### IdentityToRef

▸ `Static` **IdentityToRef**(`result`): `void`

Creates a new identity matrix and stores the result in a given matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `result` | [`Matrix`](Matrix.md) | defines the target matrix |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5650

___

### Invert

▸ `Static` **Invert**(`source`): [`Matrix`](Matrix.md)

Creates a new matrix as the invert of a given matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the source matrix |

#### Returns

[`Matrix`](Matrix.md)

the new matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5681

___

### Lerp

▸ `Static` **Lerp**(`startValue`, `endValue`, `gradient`): [`Matrix`](Matrix.md)

Returns a new Matrix whose values are the interpolated values for "gradient" (float) between the ones of the matrices "startValue" and "endValue".

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `startValue` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the start value |
| `endValue` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the end value |
| `gradient` | `number` | defines the gradient factor |

#### Returns

[`Matrix`](Matrix.md)

the new matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5928

___

### LerpToRef

▸ `Static` **LerpToRef**(`startValue`, `endValue`, `gradient`, `result`): `void`

Set the given matrix "result" as the interpolated values for "gradient" (float) between the ones of the matrices "startValue" and "endValue".

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `startValue` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the start value |
| `endValue` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the end value |
| `gradient` | `number` | defines the gradient factor |
| `result` | [`Matrix`](Matrix.md) | defines the Matrix object where to store data |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5941

___

### LookAtLH

▸ `Static` **LookAtLH**(`eye`, `target`, `up`): [`Matrix`](Matrix.md)

Gets a new rotation matrix used to rotate an entity so as it looks at the target vector3, from the eye vector3 position, the up vector3 being oriented like "up"
This function works in left handed mode

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `eye` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the final position of the entity |
| `target` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines where the entity should look at |
| `up` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the up vector for the entity |

#### Returns

[`Matrix`](Matrix.md)

the new matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:6007

___

### LookAtLHToRef

▸ `Static` **LookAtLHToRef**(`eye`, `target`, `up`, `result`): `void`

Sets the given "result" Matrix to a rotation matrix used to rotate an entity so that it looks at the target vector3, from the eye vector3 position, the up vector3 being oriented like "up".
This function works in left handed mode

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `eye` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the final position of the entity |
| `target` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines where the entity should look at |
| `up` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the up vector for the entity |
| `result` | [`Matrix`](Matrix.md) | defines the target matrix |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:6021

___

### LookAtRH

▸ `Static` **LookAtRH**(`eye`, `target`, `up`): [`Matrix`](Matrix.md)

Gets a new rotation matrix used to rotate an entity so as it looks at the target vector3, from the eye vector3 position, the up vector3 being oriented like "up"
This function works in right handed mode

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `eye` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the final position of the entity |
| `target` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines where the entity should look at |
| `up` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the up vector for the entity |

#### Returns

[`Matrix`](Matrix.md)

the new matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:6060

___

### LookAtRHToRef

▸ `Static` **LookAtRHToRef**(`eye`, `target`, `up`, `result`): `void`

Sets the given "result" Matrix to a rotation matrix used to rotate an entity so that it looks at the target vector3, from the eye vector3 position, the up vector3 being oriented like "up".
This function works in right handed mode

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `eye` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the final position of the entity |
| `target` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines where the entity should look at |
| `up` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the up vector for the entity |
| `result` | [`Matrix`](Matrix.md) | defines the target matrix |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:6074

___

### LookDirectionLH

▸ `Static` **LookDirectionLH**(`forward`, `up`): [`Matrix`](Matrix.md)

Gets a new rotation matrix used to rotate an entity so as it looks in the direction specified by forward from the eye position, the up direction being oriented like "up".
This function works in left handed mode

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `forward` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the forward direction - Must be normalized and orthogonal to up. |
| `up` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the up vector for the entity - Must be normalized and orthogonal to forward. |

#### Returns

[`Matrix`](Matrix.md)

the new matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:6112

___

### LookDirectionLHToRef

▸ `Static` **LookDirectionLHToRef**(`forward`, `up`, `result`): `void`

Sets the given "result" Matrix to a rotation matrix used to rotate an entity so that it looks in the direction of forward, the up direction being oriented like "up".
This function works in left handed mode

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `forward` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the forward direction - Must be normalized and orthogonal to up. |
| `up` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the up vector for the entity - Must be normalized and orthogonal to forward. |
| `result` | [`Matrix`](Matrix.md) | defines the target matrix |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:6125

___

### LookDirectionRH

▸ `Static` **LookDirectionRH**(`forward`, `up`): [`Matrix`](Matrix.md)

Gets a new rotation matrix used to rotate an entity so as it looks in the direction specified by forward from the eye position, the up Vector3 being oriented like "up".
This function works in right handed mode

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `forward` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the forward direction - Must be normalized and orthogonal to up. |
| `up` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the up vector for the entity - Must be normalized and orthogonal to forward. |

#### Returns

[`Matrix`](Matrix.md)

the new matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:6143

___

### LookDirectionRHToRef

▸ `Static` **LookDirectionRHToRef**(`forward`, `up`, `result`): `void`

Sets the given "result" Matrix to a rotation matrix used to rotate an entity so that it looks in the direction of forward, the up vector3 being oriented like "up".
This function works in right handed mode

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `forward` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the forward direction - Must be normalized and orthogonal to up. |
| `up` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the up vector for the entity - Must be normalized and orthogonal to forward. |
| `result` | [`Matrix`](Matrix.md) | defines the target matrix |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:6156

___

### OrthoLH

▸ `Static` **OrthoLH**(`width`, `height`, `znear`, `zfar`, `halfZRange?`): [`Matrix`](Matrix.md)

Create a left-handed orthographic projection matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `width` | `number` | defines the viewport width |
| `height` | `number` | defines the viewport height |
| `znear` | `number` | defines the near clip plane |
| `zfar` | `number` | defines the far clip plane |
| `halfZRange?` | `boolean` | true to generate NDC coordinates between 0 and 1 instead of -1 and 1 (default: false) |

#### Returns

[`Matrix`](Matrix.md)

a new matrix as a left-handed orthographic projection matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:6173

___

### OrthoLHToRef

▸ `Static` **OrthoLHToRef**(`width`, `height`, `znear`, `zfar`, `result`, `halfZRange?`): `void`

Store a left-handed orthographic projection to a given matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `width` | `number` | defines the viewport width |
| `height` | `number` | defines the viewport height |
| `znear` | `number` | defines the near clip plane |
| `zfar` | `number` | defines the far clip plane |
| `result` | [`Matrix`](Matrix.md) | defines the target matrix |
| `halfZRange?` | `boolean` | true to generate NDC coordinates between 0 and 1 instead of -1 and 1 (default: false) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:6188

___

### OrthoOffCenterLH

▸ `Static` **OrthoOffCenterLH**(`left`, `right`, `bottom`, `top`, `znear`, `zfar`, `halfZRange?`): [`Matrix`](Matrix.md)

Create a left-handed orthographic projection matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `left` | `number` | defines the viewport left coordinate |
| `right` | `number` | defines the viewport right coordinate |
| `bottom` | `number` | defines the viewport bottom coordinate |
| `top` | `number` | defines the viewport top coordinate |
| `znear` | `number` | defines the near clip plane |
| `zfar` | `number` | defines the far clip plane |
| `halfZRange?` | `boolean` | true to generate NDC coordinates between 0 and 1 instead of -1 and 1 (default: false) |

#### Returns

[`Matrix`](Matrix.md)

a new matrix as a left-handed orthographic projection matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:6217

___

### OrthoOffCenterLHToRef

▸ `Static` **OrthoOffCenterLHToRef**(`left`, `right`, `bottom`, `top`, `znear`, `zfar`, `result`, `halfZRange?`): `void`

Stores a left-handed orthographic projection into a given matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `left` | `number` | defines the viewport left coordinate |
| `right` | `number` | defines the viewport right coordinate |
| `bottom` | `number` | defines the viewport bottom coordinate |
| `top` | `number` | defines the viewport top coordinate |
| `znear` | `number` | defines the near clip plane |
| `zfar` | `number` | defines the far clip plane |
| `result` | [`Matrix`](Matrix.md) | defines the target matrix |
| `halfZRange?` | `boolean` | true to generate NDC coordinates between 0 and 1 instead of -1 and 1 (default: false) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:6234

___

### OrthoOffCenterRH

▸ `Static` **OrthoOffCenterRH**(`left`, `right`, `bottom`, `top`, `znear`, `zfar`, `halfZRange?`): [`Matrix`](Matrix.md)

Creates a right-handed orthographic projection matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `left` | `number` | defines the viewport left coordinate |
| `right` | `number` | defines the viewport right coordinate |
| `bottom` | `number` | defines the viewport bottom coordinate |
| `top` | `number` | defines the viewport top coordinate |
| `znear` | `number` | defines the near clip plane |
| `zfar` | `number` | defines the far clip plane |
| `halfZRange?` | `boolean` | true to generate NDC coordinates between 0 and 1 instead of -1 and 1 (default: false) |

#### Returns

[`Matrix`](Matrix.md)

a new matrix as a right-handed orthographic projection matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:6265

___

### OrthoOffCenterRHToRef

▸ `Static` **OrthoOffCenterRHToRef**(`left`, `right`, `bottom`, `top`, `znear`, `zfar`, `result`, `halfZRange?`): `void`

Stores a right-handed orthographic projection into a given matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `left` | `number` | defines the viewport left coordinate |
| `right` | `number` | defines the viewport right coordinate |
| `bottom` | `number` | defines the viewport bottom coordinate |
| `top` | `number` | defines the viewport top coordinate |
| `znear` | `number` | defines the near clip plane |
| `zfar` | `number` | defines the far clip plane |
| `result` | [`Matrix`](Matrix.md) | defines the target matrix |
| `halfZRange?` | `boolean` | true to generate NDC coordinates between 0 and 1 instead of -1 and 1 (default: false) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:6282

___

### PerspectiveFovLH

▸ `Static` **PerspectiveFovLH**(`fov`, `aspect`, `znear`, `zfar`, `halfZRange?`, `projectionPlaneTilt?`, `reverseDepthBufferMode?`): [`Matrix`](Matrix.md)

Creates a left-handed perspective projection matrix

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `fov` | `number` | `undefined` | defines the horizontal field of view |
| `aspect` | `number` | `undefined` | defines the aspect ratio |
| `znear` | `number` | `undefined` | defines the near clip plane |
| `zfar` | `number` | `undefined` | defines the far clip plane. If 0, assume we are in "infinite zfar" mode |
| `halfZRange?` | `boolean` | `undefined` | true to generate NDC coordinates between 0 and 1 instead of -1 and 1 (default: false) |
| `projectionPlaneTilt` | `number` | `0` | optional tilt angle of the projection plane around the X axis (horizontal) |
| `reverseDepthBufferMode` | `boolean` | `false` | true to indicate that we are in a reverse depth buffer mode (meaning znear and zfar have been inverted when calling the function) |

#### Returns

[`Matrix`](Matrix.md)

a new matrix as a left-handed perspective projection matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:6330

___

### PerspectiveFovLHToRef

▸ `Static` **PerspectiveFovLHToRef**(`fov`, `aspect`, `znear`, `zfar`, `result`, `isVerticalFovFixed?`, `halfZRange?`, `projectionPlaneTilt?`, `reverseDepthBufferMode?`): `void`

Stores a left-handed perspective projection into a given matrix

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `fov` | `number` | `undefined` | defines the horizontal field of view |
| `aspect` | `number` | `undefined` | defines the aspect ratio |
| `znear` | `number` | `undefined` | defines the near clip plane |
| `zfar` | `number` | `undefined` | defines the far clip plane. If 0, assume we are in "infinite zfar" mode |
| `result` | [`Matrix`](Matrix.md) | `undefined` | defines the target matrix |
| `isVerticalFovFixed` | `boolean` | `true` | defines it the fov is vertically fixed (default) or horizontally |
| `halfZRange?` | `boolean` | `undefined` | true to generate NDC coordinates between 0 and 1 instead of -1 and 1 (default: false) |
| `projectionPlaneTilt` | `number` | `0` | optional tilt angle of the projection plane around the X axis (horizontal) |
| `reverseDepthBufferMode` | `boolean` | `false` | true to indicate that we are in a reverse depth buffer mode (meaning znear and zfar have been inverted when calling the function) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:6356

___

### PerspectiveFovRH

▸ `Static` **PerspectiveFovRH**(`fov`, `aspect`, `znear`, `zfar`, `halfZRange?`, `projectionPlaneTilt?`, `reverseDepthBufferMode?`): [`Matrix`](Matrix.md)

Creates a right-handed perspective projection matrix

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `fov` | `number` | `undefined` | defines the horizontal field of view |
| `aspect` | `number` | `undefined` | defines the aspect ratio |
| `znear` | `number` | `undefined` | defines the near clip plane |
| `zfar` | `number` | `undefined` | defines the far clip plane. If 0, assume we are in "infinite zfar" mode |
| `halfZRange?` | `boolean` | `undefined` | true to generate NDC coordinates between 0 and 1 instead of -1 and 1 (default: false) |
| `projectionPlaneTilt` | `number` | `0` | optional tilt angle of the projection plane around the X axis (horizontal) |
| `reverseDepthBufferMode` | `boolean` | `false` | true to indicate that we are in a reverse depth buffer mode (meaning znear and zfar have been inverted when calling the function) |

#### Returns

[`Matrix`](Matrix.md)

a new matrix as a right-handed perspective projection matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:6430

___

### PerspectiveFovRHToRef

▸ `Static` **PerspectiveFovRHToRef**(`fov`, `aspect`, `znear`, `zfar`, `result`, `isVerticalFovFixed?`, `halfZRange?`, `projectionPlaneTilt?`, `reverseDepthBufferMode?`): `void`

Stores a right-handed perspective projection into a given matrix

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `fov` | `number` | `undefined` | defines the horizontal field of view |
| `aspect` | `number` | `undefined` | defines the aspect ratio |
| `znear` | `number` | `undefined` | defines the near clip plane |
| `zfar` | `number` | `undefined` | defines the far clip plane. If 0, assume we are in "infinite zfar" mode |
| `result` | [`Matrix`](Matrix.md) | `undefined` | defines the target matrix |
| `isVerticalFovFixed` | `boolean` | `true` | defines it the fov is vertically fixed (default) or horizontally |
| `halfZRange?` | `boolean` | `undefined` | true to generate NDC coordinates between 0 and 1 instead of -1 and 1 (default: false) |
| `projectionPlaneTilt` | `number` | `0` | optional tilt angle of the projection plane around the X axis (horizontal) |
| `reverseDepthBufferMode` | `boolean` | `false` | true to indicate that we are in a reverse depth buffer mode (meaning znear and zfar have been inverted when calling the function) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:6456

___

### PerspectiveFovReverseLHToRef

▸ `Static` **PerspectiveFovReverseLHToRef**(`fov`, `aspect`, `znear`, `zfar`, `result`, `isVerticalFovFixed?`, `halfZRange?`, `projectionPlaneTilt?`): `void`

Stores a left-handed perspective projection into a given matrix with depth reversed

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `fov` | `number` | `undefined` | defines the horizontal field of view |
| `aspect` | `number` | `undefined` | defines the aspect ratio |
| `znear` | `number` | `undefined` | defines the near clip plane |
| `zfar` | `number` | `undefined` | not used as infinity is used as far clip |
| `result` | [`Matrix`](Matrix.md) | `undefined` | defines the target matrix |
| `isVerticalFovFixed` | `boolean` | `true` | defines it the fov is vertically fixed (default) or horizontally |
| `halfZRange?` | `boolean` | `undefined` | true to generate NDC coordinates between 0 and 1 instead of -1 and 1 (default: false) |
| `projectionPlaneTilt` | `number` | `0` | optional tilt angle of the projection plane around the X axis (horizontal) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:6397

___

### PerspectiveFovReverseRHToRef

▸ `Static` **PerspectiveFovReverseRHToRef**(`fov`, `aspect`, `znear`, `zfar`, `result`, `isVerticalFovFixed?`, `halfZRange?`, `projectionPlaneTilt?`): `void`

Stores a right-handed perspective projection into a given matrix

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `fov` | `number` | `undefined` | defines the horizontal field of view |
| `aspect` | `number` | `undefined` | defines the aspect ratio |
| `znear` | `number` | `undefined` | defines the near clip plane |
| `zfar` | `number` | `undefined` | not used as infinity is used as far clip |
| `result` | [`Matrix`](Matrix.md) | `undefined` | defines the target matrix |
| `isVerticalFovFixed` | `boolean` | `true` | defines it the fov is vertically fixed (default) or horizontally |
| `halfZRange?` | `boolean` | `undefined` | true to generate NDC coordinates between 0 and 1 instead of -1 and 1 (default: false) |
| `projectionPlaneTilt` | `number` | `0` | optional tilt angle of the projection plane around the X axis (horizontal) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:6502

___

### PerspectiveFovWebVRToRef

▸ `Static` **PerspectiveFovWebVRToRef**(`fov`, `znear`, `zfar`, `result`, `rightHanded?`, `halfZRange?`, `projectionPlaneTilt?`): `void`

Stores a perspective projection for WebVR info a given matrix

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `fov` | `Object` | `undefined` | defines the field of view |
| `fov.downDegrees` | `number` | `undefined` |  |
| `fov.leftDegrees` | `number` | `undefined` |  |
| `fov.rightDegrees` | `number` | `undefined` |  |
| `fov.upDegrees` | `number` | `undefined` |  |
| `znear` | `number` | `undefined` | defines the near clip plane |
| `zfar` | `number` | `undefined` | defines the far clip plane |
| `result` | [`Matrix`](Matrix.md) | `undefined` | defines the target matrix |
| `rightHanded` | `boolean` | `false` | defines if the matrix must be in right-handed mode (false by default) |
| `halfZRange?` | `boolean` | `undefined` | true to generate NDC coordinates between 0 and 1 instead of -1 and 1 (default: false) |
| `projectionPlaneTilt` | `number` | `0` | optional tilt angle of the projection plane around the X axis (horizontal) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:6540

___

### PerspectiveLH

▸ `Static` **PerspectiveLH**(`width`, `height`, `znear`, `zfar`, `halfZRange?`, `projectionPlaneTilt?`): [`Matrix`](Matrix.md)

Creates a left-handed perspective projection matrix

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `width` | `number` | `undefined` | defines the viewport width |
| `height` | `number` | `undefined` | defines the viewport height |
| `znear` | `number` | `undefined` | defines the near clip plane |
| `zfar` | `number` | `undefined` | defines the far clip plane |
| `halfZRange?` | `boolean` | `undefined` | true to generate NDC coordinates between 0 and 1 instead of -1 and 1 (default: false) |
| `projectionPlaneTilt` | `number` | `0` | optional tilt angle of the projection plane around the X axis (horizontal) |

#### Returns

[`Matrix`](Matrix.md)

a new matrix as a left-handed perspective projection matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:6297

___

### Reflection

▸ `Static` **Reflection**(`plane`): [`Matrix`](Matrix.md)

Computes a reflection matrix from a plane

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `plane` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)`IPlaneLike` | defines the reflection plane |

#### Returns

[`Matrix`](Matrix.md)

a new matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:6681

___

### ReflectionToRef

▸ `Static` **ReflectionToRef**(`plane`, `result`): `void`

Computes a reflection matrix from a plane

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `plane` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)`IPlaneLike` | defines the reflection plane |
| `result` | [`Matrix`](Matrix.md) | defines the target matrix |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:6692

___

### RotationAlignToRef

▸ `Static` **RotationAlignToRef**(`from`, `to`, `result`): `void`

Takes normalised vectors and returns a rotation matrix to align "from" with "to".
Taken from http://www.iquilezles.org/www/articles/noacos/noacos.htm

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `from` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the vector to align |
| `to` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the vector to align to |
| `result` | [`Matrix`](Matrix.md) | defines the target matrix |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5803

___

### RotationAxis

▸ `Static` **RotationAxis**(`axis`, `angle`): [`Matrix`](Matrix.md)

Creates a new rotation matrix for "angle" radians around the given axis

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `axis` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the axis to use |
| `angle` | `number` | defines the angle (in radians) to use |

#### Returns

[`Matrix`](Matrix.md)

the new matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5754

___

### RotationAxisToRef

▸ `Static` **RotationAxisToRef**(`axis`, `angle`, `result`): `void`

Creates a new rotation matrix for "angle" radians around the given axis and stores it in a given matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `axis` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | defines the axis to use |
| `angle` | `number` | defines the angle (in radians) to use |
| `result` | [`Matrix`](Matrix.md) | defines the target matrix |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5766

___

### RotationX

▸ `Static` **RotationX**(`angle`): [`Matrix`](Matrix.md)

Creates a new rotation matrix for "angle" radians around the X axis

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `angle` | `number` | defines the angle (in radians) to use |

#### Returns

[`Matrix`](Matrix.md)

the new matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5670

___

### RotationXToRef

▸ `Static` **RotationXToRef**(`angle`, `result`): `void`

Creates a new rotation matrix for "angle" radians around the X axis and stores it in a given matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `angle` | `number` | defines the angle (in radians) to use |
| `result` | [`Matrix`](Matrix.md) | defines the target matrix |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5692

___

### RotationY

▸ `Static` **RotationY**(`angle`): [`Matrix`](Matrix.md)

Creates a new rotation matrix for "angle" radians around the Y axis

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `angle` | `number` | defines the angle (in radians) to use |

#### Returns

[`Matrix`](Matrix.md)

the new matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5705

___

### RotationYToRef

▸ `Static` **RotationYToRef**(`angle`, `result`): `void`

Creates a new rotation matrix for "angle" radians around the Y axis and stores it in a given matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `angle` | `number` | defines the angle (in radians) to use |
| `result` | [`Matrix`](Matrix.md) | defines the target matrix |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5716

___

### RotationYawPitchRoll

▸ `Static` **RotationYawPitchRoll**(`yaw`, `pitch`, `roll`): [`Matrix`](Matrix.md)

Creates a rotation matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `yaw` | `number` | defines the yaw angle in radians (Y axis) |
| `pitch` | `number` | defines the pitch angle in radians (X axis) |
| `roll` | `number` | defines the roll angle in radians (Z axis) |

#### Returns

[`Matrix`](Matrix.md)

the new rotation matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5852

___

### RotationYawPitchRollToRef

▸ `Static` **RotationYawPitchRollToRef**(`yaw`, `pitch`, `roll`, `result`): `void`

Creates a rotation matrix and stores it in a given matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `yaw` | `number` | defines the yaw angle in radians (Y axis) |
| `pitch` | `number` | defines the pitch angle in radians (X axis) |
| `roll` | `number` | defines the roll angle in radians (Z axis) |
| `result` | [`Matrix`](Matrix.md) | defines the target matrix |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5865

___

### RotationZ

▸ `Static` **RotationZ**(`angle`): [`Matrix`](Matrix.md)

Creates a new rotation matrix for "angle" radians around the Z axis

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `angle` | `number` | defines the angle (in radians) to use |

#### Returns

[`Matrix`](Matrix.md)

the new matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5729

___

### RotationZToRef

▸ `Static` **RotationZToRef**(`angle`, `result`): `void`

Creates a new rotation matrix for "angle" radians around the Z axis and stores it in a given matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `angle` | `number` | defines the angle (in radians) to use |
| `result` | [`Matrix`](Matrix.md) | defines the target matrix |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5740

___

### Scaling

▸ `Static` **Scaling**(`x`, `y`, `z`): [`Matrix`](Matrix.md)

Creates a scaling matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | defines the scale factor on X axis |
| `y` | `number` | defines the scale factor on Y axis |
| `z` | `number` | defines the scale factor on Z axis |

#### Returns

[`Matrix`](Matrix.md)

the new matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5877

___

### ScalingToRef

▸ `Static` **ScalingToRef**(`x`, `y`, `z`, `result`): `void`

Creates a scaling matrix and stores it in a given matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | defines the scale factor on X axis |
| `y` | `number` | defines the scale factor on Y axis |
| `z` | `number` | defines the scale factor on Z axis |
| `result` | [`Matrix`](Matrix.md) | defines the target matrix |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5890

___

### Translation

▸ `Static` **Translation**(`x`, `y`, `z`): [`Matrix`](Matrix.md)

Creates a translation matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | defines the translation on X axis |
| `y` | `number` | defines the translation on Y axis |
| `z` | `number` | defines the translationon Z axis |

#### Returns

[`Matrix`](Matrix.md)

the new matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5903

___

### TranslationToRef

▸ `Static` **TranslationToRef**(`x`, `y`, `z`, `result`): `void`

Creates a translation matrix and stores it in a given matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | defines the translation on X axis |
| `y` | `number` | defines the translation on Y axis |
| `z` | `number` | defines the translationon Z axis |
| `result` | [`Matrix`](Matrix.md) | defines the target matrix |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5916

___

### Transpose

▸ `Static` **Transpose**(`matrix`): [`Matrix`](Matrix.md)

Compute the transpose of a given matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `matrix` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the matrix to transpose |

#### Returns

[`Matrix`](Matrix.md)

the new matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:6636

___

### TransposeToRef

▸ `Static` **TransposeToRef**(`matrix`, `result`): `void`

Compute the transpose of a matrix and store it in a target matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `matrix` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the matrix to transpose |
| `result` | [`Matrix`](Matrix.md) | defines the target matrix |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:6647

___

### Zero

▸ `Static` **Zero**(): [`Matrix`](Matrix.md)

Creates a new zero matrix

#### Returns

[`Matrix`](Matrix.md)

a new zero matrix

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vector.ts:5659
