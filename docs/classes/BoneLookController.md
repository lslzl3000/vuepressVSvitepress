[@dev/core](../README.md) / [Exports](../modules.md) / BoneLookController

# Class: BoneLookController

Class used to make a bone look toward a point in space

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_bones_and_skeletons#bonelookcontroller

## Table of contents

### Constructors

- [constructor](BoneLookController.md#constructor)

### Properties

- [\_boneQuat](BoneLookController.md#_bonequat)
- [\_firstFrameSkipped](BoneLookController.md#_firstframeskipped)
- [\_fowardAxis](BoneLookController.md#_fowardaxis)
- [\_maxPitch](BoneLookController.md#_maxpitch)
- [\_maxPitchTan](BoneLookController.md#_maxpitchtan)
- [\_maxYaw](BoneLookController.md#_maxyaw)
- [\_maxYawCos](BoneLookController.md#_maxyawcos)
- [\_maxYawSin](BoneLookController.md#_maxyawsin)
- [\_midYawConstraint](BoneLookController.md#_midyawconstraint)
- [\_minPitch](BoneLookController.md#_minpitch)
- [\_minPitchTan](BoneLookController.md#_minpitchtan)
- [\_minYaw](BoneLookController.md#_minyaw)
- [\_minYawCos](BoneLookController.md#_minyawcos)
- [\_minYawSin](BoneLookController.md#_minyawsin)
- [\_slerping](BoneLookController.md#_slerping)
- [\_transformYawPitch](BoneLookController.md#_transformyawpitch)
- [\_transformYawPitchInv](BoneLookController.md#_transformyawpitchinv)
- [\_yawRange](BoneLookController.md#_yawrange)
- [adjustPitch](BoneLookController.md#adjustpitch)
- [adjustRoll](BoneLookController.md#adjustroll)
- [adjustYaw](BoneLookController.md#adjustyaw)
- [bone](BoneLookController.md#bone)
- [mesh](BoneLookController.md#mesh)
- [slerpAmount](BoneLookController.md#slerpamount)
- [target](BoneLookController.md#target)
- [upAxis](BoneLookController.md#upaxis)
- [upAxisSpace](BoneLookController.md#upaxisspace)
- [\_TmpMats](BoneLookController.md#_tmpmats)
- [\_TmpQuat](BoneLookController.md#_tmpquat)
- [\_TmpVecs](BoneLookController.md#_tmpvecs)

### Accessors

- [maxPitch](BoneLookController.md#maxpitch)
- [maxYaw](BoneLookController.md#maxyaw)
- [minPitch](BoneLookController.md#minpitch)
- [minYaw](BoneLookController.md#minyaw)

### Methods

- [\_getAngleBetween](BoneLookController.md#_getanglebetween)
- [\_getAngleDiff](BoneLookController.md#_getanglediff)
- [\_isAngleBetween](BoneLookController.md#_isanglebetween)
- [\_updateLinkedTransformRotation](BoneLookController.md#_updatelinkedtransformrotation)
- [update](BoneLookController.md#update)

## Constructors

### constructor

• **new BoneLookController**(`mesh`, `bone`, `target`, `options?`)

Create a BoneLookController

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`TransformNode`](TransformNode.md) | the TransformNode that the bone belongs to |
| `bone` | [`Bone`](Bone.md) | the bone that will be looking to the target |
| `target` | [`Vector3`](Vector3.md) | the target Vector3 to look at |
| `options?` | `Object` | optional settings:  * maxYaw: the maximum angle the bone will yaw to  * minYaw: the minimum angle the bone will yaw to  * maxPitch: the maximum angle the bone will pitch to  * minPitch: the minimum angle the bone will yaw to  * slerpAmount: set the between 0 and 1 to make the bone slerp to the target.  * upAxis: the up axis of the coordinate system  * upAxisSpace: the space that the up axis is in - Space.BONE, Space.LOCAL (default), or Space.WORLD.  * yawAxis: set yawAxis if the bone does not yaw on the y axis  * pitchAxis: set pitchAxis if the bone does not pitch on the x axis  * adjustYaw: used to make an adjustment to the yaw of the bone  * adjustPitch: used to make an adjustment to the pitch of the bone  * adjustRoll: used to make an adjustment to the roll of the bone |
| `options.adjustPitch?` | `number` |  |
| `options.adjustRoll?` | `number` |  |
| `options.adjustYaw?` | `number` |  |
| `options.maxPitch?` | `number` |  |
| `options.maxYaw?` | `number` |  |
| `options.minPitch?` | `number` |  |
| `options.minYaw?` | `number` |  |
| `options.pitchAxis?` | [`Vector3`](Vector3.md) |  |
| `options.slerpAmount?` | `number` |  |
| `options.upAxis?` | [`Vector3`](Vector3.md) |  |
| `options.upAxisSpace?` | [`Space`](../enums/Space.md) |  |
| `options.yawAxis?` | [`Vector3`](Vector3.md) |  |

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:172

## Properties

### \_boneQuat

• `Private` **\_boneQuat**: [`Quaternion`](Quaternion.md)

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:75

___

### \_firstFrameSkipped

• `Private` **\_firstFrameSkipped**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:79

___

### \_fowardAxis

• `Private` **\_fowardAxis**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:81

___

### \_maxPitch

• `Private` **\_maxPitch**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:66

___

### \_maxPitchTan

• `Private` **\_maxPitchTan**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:73

___

### \_maxYaw

• `Private` **\_maxYaw**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:64

___

### \_maxYawCos

• `Private` **\_maxYawCos**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:70

___

### \_maxYawSin

• `Private` **\_maxYawSin**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:69

___

### \_midYawConstraint

• `Private` **\_midYawConstraint**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:71

___

### \_minPitch

• `Private` **\_minPitch**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:65

___

### \_minPitchTan

• `Private` **\_minPitchTan**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:72

___

### \_minYaw

• `Private` **\_minYaw**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:63

___

### \_minYawCos

• `Private` **\_minYawCos**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:68

___

### \_minYawSin

• `Private` **\_minYawSin**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:67

___

### \_slerping

• `Private` **\_slerping**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:76

___

### \_transformYawPitch

• `Private` **\_transformYawPitch**: [`Matrix`](Matrix.md)

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:77

___

### \_transformYawPitchInv

• `Private` **\_transformYawPitchInv**: [`Matrix`](Matrix.md)

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:78

___

### \_yawRange

• `Private` **\_yawRange**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:80

___

### adjustPitch

• **adjustPitch**: `number` = `0`

Used to make an adjustment to the pitch of the bone

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:51

___

### adjustRoll

• **adjustRoll**: `number` = `0`

Used to make an adjustment to the roll of the bone

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:56

___

### adjustYaw

• **adjustYaw**: `number` = `0`

Used to make an adjustment to the yaw of the bone

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:46

___

### bone

• **bone**: [`Bone`](Bone.md)

The bone that will be looking to the target

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:31

___

### mesh

• **mesh**: [`TransformNode`](TransformNode.md)

The TransformNode that the bone is attached to
Name kept as mesh for back compatibility

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:26

___

### slerpAmount

• **slerpAmount**: `number` = `1`

The amount to slerp (spherical linear interpolation) to the target.  Set this to a value between 0 and 1 (a value of 1 disables slerp)

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:61

___

### target

• **target**: [`Vector3`](Vector3.md)

The target Vector3 that the bone will look at

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:20

___

### upAxis

• **upAxis**: [`Vector3`](Vector3.md)

The up axis of the coordinate system that is used when the bone is rotated

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:36

___

### upAxisSpace

• **upAxisSpace**: [`Space`](../enums/Space.md) = `Space.LOCAL`

The space that the up axis is in - Space.BONE, Space.LOCAL (default), or Space.WORLD

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:41

___

### \_TmpMats

▪ `Static` `Private` **\_TmpMats**: [`Matrix`](Matrix.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:15

___

### \_TmpQuat

▪ `Static` `Private` **\_TmpQuat**: [`Quaternion`](Quaternion.md)

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:14

___

### \_TmpVecs

▪ `Static` `Private` **\_TmpVecs**: [`Vector3`](Vector3.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:13

## Accessors

### maxPitch

• `get` **maxPitch**(): `number`

Gets or sets the maximum pitch angle that the bone can look to

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:132

• `set` **maxPitch**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:136

___

### maxYaw

• `get` **maxYaw**(): `number`

Gets or sets the maximum yaw angle that the bone can look to

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:103

• `set` **maxYaw**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:107

___

### minPitch

• `get` **minPitch**(): `number`

Gets or sets the minimum pitch angle that the bone can look to

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:120

• `set` **minPitch**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:124

___

### minYaw

• `get` **minYaw**(): `number`

Gets or sets the minimum yaw angle that the bone can look to

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:86

• `set` **minYaw**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:90

## Methods

### \_getAngleBetween

▸ `Private` **_getAngleBetween**(`ang1`, `ang2`): `number`

#### Parameters

| Name | Type |
| :------ | :------ |
| `ang1` | `number` |
| `ang2` | `number` |

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:524

___

### \_getAngleDiff

▸ `Private` **_getAngleDiff**(`ang1`, `ang2`): `number`

#### Parameters

| Name | Type |
| :------ | :------ |
| `ang1` | `number` |
| `ang2` | `number` |

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:511

___

### \_isAngleBetween

▸ `Private` **_isAngleBetween**(`ang`, `ang1`, `ang2`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `ang` | `number` |
| `ang1` | `number` |
| `ang2` | `number` |

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:546

___

### \_updateLinkedTransformRotation

▸ `Private` **_updateLinkedTransformRotation**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:566

___

### update

▸ **update**(): `void`

Update the bone to look at the target.  This should be called before the scene is rendered (use scene.registerBeforeRender())

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Bones/boneLookController.ts:276
