[@dev/core](../README.md) / [Exports](../modules.md) / HandConstraintBehavior

# Class: HandConstraintBehavior

Hand constraint behavior that makes the attached `TransformNode` follow hands in XR experiences.

**`Since`**

5.0.0

## Implements

- [`Behavior`](../interfaces/Behavior.md)[`TransformNode`](TransformNode.md)

## Table of contents

### Constructors

- [constructor](HandConstraintBehavior.md#constructor)

### Properties

- [\_eyeTracking](HandConstraintBehavior.md#_eyetracking)
- [\_handTracking](HandConstraintBehavior.md#_handtracking)
- [\_node](HandConstraintBehavior.md#_node)
- [\_scene](HandConstraintBehavior.md#_scene)
- [\_sceneRenderObserver](HandConstraintBehavior.md#_scenerenderobserver)
- [\_zoneAxis](HandConstraintBehavior.md#_zoneaxis)
- [gazeProximityRadius](HandConstraintBehavior.md#gazeproximityradius)
- [handConstraintVisibility](HandConstraintBehavior.md#handconstraintvisibility)
- [handedness](HandConstraintBehavior.md#handedness)
- [lerpTime](HandConstraintBehavior.md#lerptime)
- [nodeOrientationMode](HandConstraintBehavior.md#nodeorientationmode)
- [palmUpStrictness](HandConstraintBehavior.md#palmupstrictness)
- [targetOffset](HandConstraintBehavior.md#targetoffset)
- [targetZone](HandConstraintBehavior.md#targetzone)
- [zoneOrientationMode](HandConstraintBehavior.md#zoneorientationmode)

### Accessors

- [name](HandConstraintBehavior.md#name)

### Methods

- [\_getHandPose](HandConstraintBehavior.md#_gethandpose)
- [\_setVisibility](HandConstraintBehavior.md#_setvisibility)
- [attach](HandConstraintBehavior.md#attach)
- [detach](HandConstraintBehavior.md#detach)
- [disable](HandConstraintBehavior.md#disable)
- [enable](HandConstraintBehavior.md#enable)
- [init](HandConstraintBehavior.md#init)
- [linkToXRExperience](HandConstraintBehavior.md#linktoxrexperience)

## Constructors

### constructor

• **new HandConstraintBehavior**()

Builds a hand constraint behavior

#### Defined in

packages/dev/core/src/Behaviors/Meshes/handConstraintBehavior.ts:142

## Properties

### \_eyeTracking

• `Private` **\_eyeTracking**: [`Nullable`](../modules.md#nullable)[`WebXREyeTracking`](WebXREyeTracking.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/handConstraintBehavior.ts:86

___

### \_handTracking

• `Private` **\_handTracking**: [`Nullable`](../modules.md#nullable)[`WebXRHandTracking`](WebXRHandTracking.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/handConstraintBehavior.ts:87

___

### \_node

• `Private` **\_node**: [`TransformNode`](TransformNode.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/handConstraintBehavior.ts:85

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/handConstraintBehavior.ts:84

___

### \_sceneRenderObserver

• `Private` **\_sceneRenderObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Scene`](Scene.md) = `null`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/handConstraintBehavior.ts:88

___

### \_zoneAxis

• `Private` **\_zoneAxis**: `Object` = `{}`

#### Index signature

▪ [id: `number`]: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/handConstraintBehavior.ts:89

___

### gazeProximityRadius

• **gazeProximityRadius**: `number` = `0.15`

The radius in meters around the center of the hand that the user must gaze inside for the attached node to be enabled and appear.
Used with HandConstraintVisibility.GAZE_FOCUS

#### Defined in

packages/dev/core/src/Behaviors/Meshes/handConstraintBehavior.ts:107

___

### handConstraintVisibility

• **handConstraintVisibility**: [`HandConstraintVisibility`](../enums/HandConstraintVisibility.md) = `HandConstraintVisibility.PALM_AND_GAZE`

Sets the HandConstraintVisibility level for the hand constraint

#### Defined in

packages/dev/core/src/Behaviors/Meshes/handConstraintBehavior.ts:94

___

### handedness

• **handedness**: `XRHandedness` = `"none"`

Set the hand this behavior should follow. If set to "none", it will follow any visible hand (prioritising the left one).

#### Defined in

packages/dev/core/src/Behaviors/Meshes/handConstraintBehavior.ts:131

___

### lerpTime

• **lerpTime**: `number` = `100`

Rate of interpolation of position and rotation of the attached node.
Higher values will give a slower interpolation.

#### Defined in

packages/dev/core/src/Behaviors/Meshes/handConstraintBehavior.ts:137

___

### nodeOrientationMode

• **nodeOrientationMode**: [`HandConstraintOrientation`](../enums/HandConstraintOrientation.md) = `HandConstraintOrientation.HAND_ROTATION`

Orientation mode of the node attached to this behavior

#### Defined in

packages/dev/core/src/Behaviors/Meshes/handConstraintBehavior.ts:126

___

### palmUpStrictness

• **palmUpStrictness**: `number` = `0.95`

A number from 0.0 to 1.0, marking how restricted the direction the palm faces is for the attached node to be enabled.
A 1 means the palm must be directly facing the user before the node is enabled, a 0 means it is always enabled.
Used with HandConstraintVisibility.PALM_UP

#### Defined in

packages/dev/core/src/Behaviors/Meshes/handConstraintBehavior.ts:101

___

### targetOffset

• **targetOffset**: `number` = `0.1`

Offset distance from the hand in meters

#### Defined in

packages/dev/core/src/Behaviors/Meshes/handConstraintBehavior.ts:112

___

### targetZone

• **targetZone**: [`HandConstraintZone`](../enums/HandConstraintZone.md) = `HandConstraintZone.ULNAR_SIDE`

Where to place the node regarding the center of the hand.

#### Defined in

packages/dev/core/src/Behaviors/Meshes/handConstraintBehavior.ts:117

___

### zoneOrientationMode

• **zoneOrientationMode**: [`HandConstraintOrientation`](../enums/HandConstraintOrientation.md) = `HandConstraintOrientation.HAND_ROTATION`

Orientation mode of the 4 zones around the hand

#### Defined in

packages/dev/core/src/Behaviors/Meshes/handConstraintBehavior.ts:122

## Accessors

### name

• `get` **name**(): `string`

gets or sets behavior's name

#### Returns

`string`

#### Implementation of

[Behavior](../interfaces/Behavior.md).[name](../interfaces/Behavior.md#name)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/handConstraintBehavior.ts:151

## Methods

### \_getHandPose

▸ `Private` **_getHandPose**(): [`Nullable`](../modules.md#nullable)`HandPoseInfo`

#### Returns

[`Nullable`](../modules.md#nullable)`HandPoseInfo`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/handConstraintBehavior.ts:165

___

### \_setVisibility

▸ `Private` **_setVisibility**(`pose`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `pose` | [`Nullable`](../modules.md#nullable)`HandPoseInfo` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/handConstraintBehavior.ts:281

___

### attach

▸ **attach**(`node`): `void`

Attaches the hand constraint to a `TransformNode`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `node` | [`TransformNode`](TransformNode.md) | defines the node to attach the behavior to |

#### Returns

`void`

#### Implementation of

[Behavior](../interfaces/Behavior.md).[attach](../interfaces/Behavior.md#attach)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/handConstraintBehavior.ts:215

___

### detach

▸ **detach**(): `void`

Detaches the behavior from the `TransformNode`

#### Returns

`void`

#### Implementation of

[Behavior](../interfaces/Behavior.md).[detach](../interfaces/Behavior.md#detach)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/handConstraintBehavior.ts:336

___

### disable

▸ **disable**(): `void`

Disable the behavior

#### Returns

`void`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/handConstraintBehavior.ts:161

___

### enable

▸ **enable**(): `void`

Enable the behavior

#### Returns

`void`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/handConstraintBehavior.ts:156

___

### init

▸ **init**(): `void`

Initializes the hand constraint behavior

#### Returns

`void`

#### Implementation of

[Behavior](../interfaces/Behavior.md).[init](../interfaces/Behavior.md#init)

#### Defined in

packages/dev/core/src/Behaviors/Meshes/handConstraintBehavior.ts:209

___

### linkToXRExperience

▸ **linkToXRExperience**(`xr`): `void`

Links the behavior to the XR experience in which to retrieve hand transform information.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `xr` | [`WebXRExperienceHelper`](WebXRExperienceHelper.md) | xr experience |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Behaviors/Meshes/handConstraintBehavior.ts:344
