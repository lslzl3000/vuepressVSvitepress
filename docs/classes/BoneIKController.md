[@dev/core](../README.md) / [Exports](../modules.md) / BoneIKController

# Class: BoneIKController

Class used to apply inverse kinematics to bones

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_bones_and_skeletons#boneikcontroller

## Table of contents

### Constructors

- [constructor](BoneIKController.md#constructor)

### Properties

- [\_adjustRoll](BoneIKController.md#_adjustroll)
- [\_bendAxis](BoneIKController.md#_bendaxis)
- [\_bone1](BoneIKController.md#_bone1)
- [\_bone1Length](BoneIKController.md#_bone1length)
- [\_bone1Mat](BoneIKController.md#_bone1mat)
- [\_bone1Quat](BoneIKController.md#_bone1quat)
- [\_bone2](BoneIKController.md#_bone2)
- [\_bone2Ang](BoneIKController.md#_bone2ang)
- [\_bone2Length](BoneIKController.md#_bone2length)
- [\_maxAngle](BoneIKController.md#_maxangle)
- [\_maxReach](BoneIKController.md#_maxreach)
- [\_rightHandedSystem](BoneIKController.md#_righthandedsystem)
- [\_slerping](BoneIKController.md#_slerping)
- [mesh](BoneIKController.md#mesh)
- [poleAngle](BoneIKController.md#poleangle)
- [poleTargetBone](BoneIKController.md#poletargetbone)
- [poleTargetLocalOffset](BoneIKController.md#poletargetlocaloffset)
- [poleTargetMesh](BoneIKController.md#poletargetmesh)
- [poleTargetPosition](BoneIKController.md#poletargetposition)
- [slerpAmount](BoneIKController.md#slerpamount)
- [targetMesh](BoneIKController.md#targetmesh)
- [targetPosition](BoneIKController.md#targetposition)
- [\_TmpMats](BoneIKController.md#_tmpmats)
- [\_TmpQuat](BoneIKController.md#_tmpquat)
- [\_TmpVecs](BoneIKController.md#_tmpvecs)

### Accessors

- [maxAngle](BoneIKController.md#maxangle)

### Methods

- [\_setMaxAngle](BoneIKController.md#_setmaxangle)
- [\_updateLinkedTransformRotation](BoneIKController.md#_updatelinkedtransformrotation)
- [update](BoneIKController.md#update)

## Constructors

### constructor

• **new BoneIKController**(`mesh`, `bone`, `options?`)

Creates a new BoneIKController

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`TransformNode`](TransformNode.md) | defines the TransformNode to control |
| `bone` | [`Bone`](Bone.md) | defines the bone to control |
| `options?` | `Object` | defines options to set up the controller |
| `options.bendAxis?` | [`Vector3`](Vector3.md) |  |
| `options.maxAngle?` | `number` |  |
| `options.poleAngle?` | `number` |  |
| `options.poleTargetBone?` | [`Bone`](Bone.md) |  |
| `options.poleTargetLocalOffset?` | [`Vector3`](Vector3.md) |  |
| `options.poleTargetMesh?` | [`TransformNode`](TransformNode.md) |  |
| `options.slerpAmount?` | `number` |  |
| `options.targetMesh?` | [`TransformNode`](TransformNode.md) |  |

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneIKController.ts:104

## Properties

### \_adjustRoll

• `Private` **\_adjustRoll**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneIKController.ts:77

___

### \_bendAxis

• `Private` **\_bendAxis**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneIKController.ts:74

___

### \_bone1

• `Private` **\_bone1**: [`Nullable`](../modules.md#nullable)[`Bone`](Bone.md)

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneIKController.ts:65

___

### \_bone1Length

• `Private` **\_bone1Length**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneIKController.ts:67

___

### \_bone1Mat

• `Private` **\_bone1Mat**: [`Matrix`](Matrix.md)

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneIKController.ts:62

___

### \_bone1Quat

• `Private` **\_bone1Quat**: [`Quaternion`](Quaternion.md)

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneIKController.ts:61

___

### \_bone2

• `Private` **\_bone2**: [`Bone`](Bone.md)

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneIKController.ts:66

___

### \_bone2Ang

• `Private` **\_bone2Ang**: `number` = `Math.PI`

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneIKController.ts:63

___

### \_bone2Length

• `Private` **\_bone2Length**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneIKController.ts:68

___

### \_maxAngle

• `Private` **\_maxAngle**: `number` = `Math.PI`

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneIKController.ts:69

___

### \_maxReach

• `Private` **\_maxReach**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneIKController.ts:70

___

### \_rightHandedSystem

• `Private` **\_rightHandedSystem**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneIKController.ts:72

___

### \_slerping

• `Private` **\_slerping**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneIKController.ts:75

___

### mesh

• **mesh**: [`TransformNode`](TransformNode.md)

Gets or sets the TransformNode associated with the controller
Name kept as mesh for back compatibility

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneIKController.ts:54

___

### poleAngle

• **poleAngle**: `number` = `0`

Gets or sets the pole angle

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneIKController.ts:48

___

### poleTargetBone

• **poleTargetBone**: [`Nullable`](../modules.md#nullable)[`Bone`](Bone.md)

Gets or sets the bone used as pole

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneIKController.ts:28

___

### poleTargetLocalOffset

• **poleTargetLocalOffset**: [`Vector3`](Vector3.md)

Gets or sets the pole target local offset

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneIKController.ts:43

___

### poleTargetMesh

• **poleTargetMesh**: [`TransformNode`](TransformNode.md)

Gets or sets the mesh used as pole

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneIKController.ts:23

___

### poleTargetPosition

• **poleTargetPosition**: [`Vector3`](Vector3.md)

Gets or sets the pole target position

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneIKController.ts:38

___

### slerpAmount

• **slerpAmount**: `number` = `1`

The amount to slerp (spherical linear interpolation) to the target.  Set this to a value between 0 and 1 (a value of 1 disables slerp)

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneIKController.ts:59

___

### targetMesh

• **targetMesh**: [`TransformNode`](TransformNode.md)

Gets or sets the target TransformNode
Name kept as mesh for back compatibility

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneIKController.ts:20

___

### targetPosition

• **targetPosition**: [`Vector3`](Vector3.md)

Gets or sets the target position

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneIKController.ts:33

___

### \_TmpMats

▪ `Static` `Private` **\_TmpMats**: [`Matrix`](Matrix.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneIKController.ts:14

___

### \_TmpQuat

▪ `Static` `Private` **\_TmpQuat**: [`Quaternion`](Quaternion.md)

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneIKController.ts:13

___

### \_TmpVecs

▪ `Static` `Private` **\_TmpVecs**: [`Vector3`](Vector3.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneIKController.ts:12

## Accessors

### maxAngle

• `get` **maxAngle**(): `number`

Gets or sets maximum allowed angle

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneIKController.ts:82

• `set` **maxAngle**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneIKController.ts:86

## Methods

### \_setMaxAngle

▸ `Private` **_setMaxAngle**(`ang`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `ang` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneIKController.ts:198

___

### \_updateLinkedTransformRotation

▸ `Private` **_updateLinkedTransformRotation**(`bone`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `bone` | [`Bone`](Bone.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneIKController.ts:348

___

### update

▸ **update**(): `void`

Force the controller to update the bones

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneIKController.ts:218
