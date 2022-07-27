[@dev/core](../README.md) / [Exports](../modules.md) / FollowBehavior

# Class: FollowBehavior

A behavior that when attached to a mesh will follow a camera

**`Since`**

5.0.0

## Implements

- [`Behavior`](../interfaces/Behavior.md)[`TransformNode`](TransformNode.md)

## Table of contents

### Constructors

- [constructor](FollowBehavior.md#constructor)

### Properties

- [\_followedCamera](FollowBehavior.md#_followedcamera)
- [\_lastTick](FollowBehavior.md#_lasttick)
- [\_onBeforeRender](FollowBehavior.md#_onbeforerender)
- [\_recenterNextUpdate](FollowBehavior.md#_recenternextupdate)
- [\_scene](FollowBehavior.md#_scene)
- [\_tmpForward](FollowBehavior.md#_tmpforward)
- [\_tmpInvertView](FollowBehavior.md#_tmpinvertview)
- [\_tmpMatrix](FollowBehavior.md#_tmpmatrix)
- [\_tmpNodeForward](FollowBehavior.md#_tmpnodeforward)
- [\_tmpPosition](FollowBehavior.md#_tmpposition)
- [\_tmpQuaternion](FollowBehavior.md#_tmpquaternion)
- [\_tmpVectors](FollowBehavior.md#_tmpvectors)
- [\_workingPosition](FollowBehavior.md#_workingposition)
- [\_workingQuaternion](FollowBehavior.md#_workingquaternion)
- [attachedNode](FollowBehavior.md#attachednode)
- [defaultDistance](FollowBehavior.md#defaultdistance)
- [fixedVerticalOffset](FollowBehavior.md#fixedverticaloffset)
- [ignoreAngleClamp](FollowBehavior.md#ignoreangleclamp)
- [ignoreCameraPitchAndRoll](FollowBehavior.md#ignorecamerapitchandroll)
- [ignoreDistanceClamp](FollowBehavior.md#ignoredistanceclamp)
- [interpolatePose](FollowBehavior.md#interpolatepose)
- [lerpTime](FollowBehavior.md#lerptime)
- [maxViewHorizontalDegrees](FollowBehavior.md#maxviewhorizontaldegrees)
- [maxViewVerticalDegrees](FollowBehavior.md#maxviewverticaldegrees)
- [maximumDistance](FollowBehavior.md#maximumdistance)
- [minimumDistance](FollowBehavior.md#minimumdistance)
- [orientToCameraDeadzoneDegrees](FollowBehavior.md#orienttocameradeadzonedegrees)
- [pitchOffset](FollowBehavior.md#pitchoffset)
- [useFixedVerticalOffset](FollowBehavior.md#usefixedverticaloffset)
- [verticalMaxDistance](FollowBehavior.md#verticalmaxdistance)

### Accessors

- [followedCamera](FollowBehavior.md#followedcamera)
- [name](FollowBehavior.md#name)

### Methods

- [\_addObservables](FollowBehavior.md#_addobservables)
- [\_angleBetweenVectorAndPlane](FollowBehavior.md#_anglebetweenvectorandplane)
- [\_angularClamp](FollowBehavior.md#_angularclamp)
- [\_applyPitchOffset](FollowBehavior.md#_applypitchoffset)
- [\_applyVerticalClamp](FollowBehavior.md#_applyverticalclamp)
- [\_distanceClamp](FollowBehavior.md#_distanceclamp)
- [\_length2D](FollowBehavior.md#_length2d)
- [\_orientationClamp](FollowBehavior.md#_orientationclamp)
- [\_passedOrientationDeadzone](FollowBehavior.md#_passedorientationdeadzone)
- [\_removeObservables](FollowBehavior.md#_removeobservables)
- [\_toOrientationQuatToRef](FollowBehavior.md#_toorientationquattoref)
- [\_updateLeashing](FollowBehavior.md#_updateleashing)
- [\_updateTransformToGoal](FollowBehavior.md#_updatetransformtogoal)
- [attach](FollowBehavior.md#attach)
- [detach](FollowBehavior.md#detach)
- [init](FollowBehavior.md#init)
- [recenter](FollowBehavior.md#recenter)

## Constructors

### constructor

• **new FollowBehavior**()

## Properties

### \_followedCamera

• `Private` **\_followedCamera**: [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:27

___

### \_lastTick

• `Private` **\_lastTick**: `number` = `-1`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:32

___

### \_onBeforeRender

• `Private` **\_onBeforeRender**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:28

___

### \_recenterNextUpdate

• `Private` **\_recenterNextUpdate**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:33

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:16

___

### \_tmpForward

• `Private` **\_tmpForward**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:23

___

### \_tmpInvertView

• `Private` **\_tmpInvertView**: [`Matrix`](Matrix.md)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:22

___

### \_tmpMatrix

• `Private` **\_tmpMatrix**: [`Matrix`](Matrix.md)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:21

___

### \_tmpNodeForward

• `Private` **\_tmpNodeForward**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:24

___

### \_tmpPosition

• `Private` **\_tmpPosition**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:25

___

### \_tmpQuaternion

• `Private` **\_tmpQuaternion**: [`Quaternion`](Quaternion.md)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:19

___

### \_tmpVectors

• `Private` **\_tmpVectors**: [`Vector3`](Vector3.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:20

___

### \_workingPosition

• `Private` **\_workingPosition**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:30

___

### \_workingQuaternion

• `Private` **\_workingQuaternion**: [`Quaternion`](Quaternion.md)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:31

___

### attachedNode

• **attachedNode**: [`Nullable`](../modules.md#nullable)[`TransformNode`](TransformNode.md)

Attached node of this behavior

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:38

___

### defaultDistance

• **defaultDistance**: `number` = `0.8`

Default distance from eye to attached node, i.e. the sphere radius

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:90

___

### fixedVerticalOffset

• **fixedVerticalOffset**: `number` = `0`

Fixed vertical position offset distance.

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:108

___

### ignoreAngleClamp

• **ignoreAngleClamp**: `boolean` = `false`

Option to ignore angle clamping

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:82

___

### ignoreCameraPitchAndRoll

• **ignoreCameraPitchAndRoll**: `boolean` = `false`

If the behavior should ignore the pitch and roll of the camera.

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:54

___

### ignoreDistanceClamp

• **ignoreDistanceClamp**: `boolean` = `false`

Option to ignore distance clamping

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:78

___

### interpolatePose

• **interpolatePose**: `boolean` = `true`

Set to false if the node should strictly follow the camera without any interpolation time

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:43

___

### lerpTime

• **lerpTime**: `number` = `500`

Rate of interpolation of position and rotation of the attached node.
Higher values will give a slower interpolation.

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:49

___

### maxViewHorizontalDegrees

• **maxViewHorizontalDegrees**: `number` = `30`

The horizontal angle from the camera forward axis to the owner will not exceed this value

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:70

___

### maxViewVerticalDegrees

• **maxViewVerticalDegrees**: `number` = `30`

The vertical angle from the camera forward axis to the owner will not exceed this value

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:65

___

### maximumDistance

• **maximumDistance**: `number` = `2`

Max distance from eye to attached node, i.e. the sphere radius

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:94

___

### minimumDistance

• **minimumDistance**: `number` = `0.3`

Min distance from eye to attached node, i.e. the sphere radius

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:98

___

### orientToCameraDeadzoneDegrees

• **orientToCameraDeadzoneDegrees**: `number` = `60`

The attached node will not reorient until the angle between its forward vector and the vector to the camera is greater than this value

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:74

___

### pitchOffset

• **pitchOffset**: `number` = `15`

Pitch offset from camera (relative to Max Distance)
Is only effective if `ignoreCameraPitchAndRoll` is set to `true`.

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:60

___

### useFixedVerticalOffset

• **useFixedVerticalOffset**: `boolean` = `false`

Ignore vertical movement and lock the Y position of the object.

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:103

___

### verticalMaxDistance

• **verticalMaxDistance**: `number` = `0`

Max vertical distance between the attachedNode and camera

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:86

## Accessors

### followedCamera

• `get` **followedCamera**(): [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md)

The camera that should be followed by this behavior

#### Returns

[`Nullable`](../modules.md#nullable)[`Camera`](Camera.md)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:119

• `set` **followedCamera**(`camera`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `camera` | [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:123

___

### name

• `get` **name**(): `string`

The name of the behavior

#### Returns

`string`

#### Implementation of

[Behavior](../interfaces/Behavior.md).[name](../interfaces/Behavior.md#name)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:130

## Methods

### \_addObservables

▸ `Private` **_addObservables**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:444

___

### \_angleBetweenVectorAndPlane

▸ `Private` **_angleBetweenVectorAndPlane**(`vector`, `normal`): `number`

#### Parameters

| Name | Type |
| :------ | :------ |
| `vector` | [`Vector3`](Vector3.md) |
| `normal` | [`Vector3`](Vector3.md) |

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:170

___

### \_angularClamp

▸ `Private` **_angularClamp**(`invertView`, `currentToTarget`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `invertView` | [`Matrix`](Matrix.md) |
| `currentToTarget` | [`Vector3`](Vector3.md) |

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:252

___

### \_applyPitchOffset

▸ `Private` **_applyPitchOffset**(`invertView`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `invertView` | [`Matrix`](Matrix.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:232

___

### \_applyVerticalClamp

▸ `Private` **_applyVerticalClamp**(`currentToTarget`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `currentToTarget` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:222

___

### \_distanceClamp

▸ `Private` **_distanceClamp**(`currentToTarget`, `moveToDefault?`): `boolean`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `currentToTarget` | [`Vector3`](Vector3.md) | `undefined` |
| `moveToDefault` | `boolean` | `false` |

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:187

___

### \_length2D

▸ `Private` **_length2D**(`vector`): `number`

#### Parameters

| Name | Type |
| :------ | :------ |
| `vector` | [`Vector3`](Vector3.md) |

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:183

___

### \_orientationClamp

▸ `Private` **_orientationClamp**(`currentToTarget`, `rotationQuaternion`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `currentToTarget` | [`Vector3`](Vector3.md) |
| `rotationQuaternion` | [`Quaternion`](Quaternion.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:309

___

### \_passedOrientationDeadzone

▸ `Private` **_passedOrientationDeadzone**(`currentToTarget`, `forward`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `currentToTarget` | [`Vector3`](Vector3.md) |
| `forward` | [`Vector3`](Vector3.md) |

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:337

___

### \_removeObservables

▸ `Private` **_removeObservables**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:458

___

### \_toOrientationQuatToRef

▸ `Private` **_toOrientationQuatToRef**(`vector`, `quaternion`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `vector` | [`Vector3`](Vector3.md) |
| `quaternion` | [`Quaternion`](Quaternion.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:228

___

### \_updateLeashing

▸ `Private` **_updateLeashing**(`camera`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `camera` | [`Camera`](Camera.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:346

___

### \_updateTransformToGoal

▸ `Private` **_updateTransformToGoal**(`elapsed`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `elapsed` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:411

___

### attach

▸ **attach**(`ownerNode`, `followedCamera?`): `void`

Attaches the follow behavior

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ownerNode` | [`TransformNode`](TransformNode.md) | The mesh that will be following once attached |
| `followedCamera?` | [`Camera`](Camera.md) | The camera that should be followed by the node |

#### Returns

`void`

#### Implementation of

[Behavior](../interfaces/Behavior.md).[attach](../interfaces/Behavior.md#attach)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:144

___

### detach

▸ **detach**(): `void`

Detaches the behavior from the mesh

#### Returns

`void`

#### Implementation of

[Behavior](../interfaces/Behavior.md).[detach](../interfaces/Behavior.md#detach)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:158

___

### init

▸ **init**(): `void`

Initializes the behavior

#### Returns

`void`

#### Implementation of

[Behavior](../interfaces/Behavior.md).[init](../interfaces/Behavior.md#init)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:137

___

### recenter

▸ **recenter**(): `void`

Recenters the attached node in front of the camera on the next update

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Meshes/followBehavior.ts:166
