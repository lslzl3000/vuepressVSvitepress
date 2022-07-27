[@dev/core](../README.md) / [Exports](../modules.md) / BouncingBehavior

# Class: BouncingBehavior

Add a bouncing effect to an ArcRotateCamera when reaching a specified minimum and maximum radius

**`See`**

https://doc.babylonjs.com/how_to/camera_behaviors#bouncing-behavior

## Implements

- [`Behavior`](../interfaces/Behavior.md)[`ArcRotateCamera`](ArcRotateCamera.md)

## Table of contents

### Constructors

- [constructor](BouncingBehavior.md#constructor)

### Properties

- [\_animatables](BouncingBehavior.md#_animatables)
- [\_attachedCamera](BouncingBehavior.md#_attachedcamera)
- [\_autoTransitionRange](BouncingBehavior.md#_autotransitionrange)
- [\_cachedWheelPrecision](BouncingBehavior.md#_cachedwheelprecision)
- [\_onAfterCheckInputsObserver](BouncingBehavior.md#_onaftercheckinputsobserver)
- [\_onMeshTargetChangedObserver](BouncingBehavior.md#_onmeshtargetchangedobserver)
- [\_radiusBounceTransition](BouncingBehavior.md#_radiusbouncetransition)
- [\_radiusIsAnimating](BouncingBehavior.md#_radiusisanimating)
- [lowerRadiusTransitionRange](BouncingBehavior.md#lowerradiustransitionrange)
- [transitionDuration](BouncingBehavior.md#transitionduration)
- [upperRadiusTransitionRange](BouncingBehavior.md#upperradiustransitionrange)
- [EasingFunction](BouncingBehavior.md#easingfunction)
- [EasingMode](BouncingBehavior.md#easingmode)

### Accessors

- [autoTransitionRange](BouncingBehavior.md#autotransitionrange)
- [name](BouncingBehavior.md#name)

### Methods

- [\_applyBoundRadiusAnimation](BouncingBehavior.md#_applyboundradiusanimation)
- [\_clearAnimationLocks](BouncingBehavior.md#_clearanimationlocks)
- [\_isRadiusAtLimit](BouncingBehavior.md#_isradiusatlimit)
- [attach](BouncingBehavior.md#attach)
- [detach](BouncingBehavior.md#detach)
- [init](BouncingBehavior.md#init)
- [stopAllAnimations](BouncingBehavior.md#stopallanimations)

## Constructors

### constructor

• **new BouncingBehavior**()

## Properties

### \_animatables

• `Private` **\_animatables**: [`Animatable`](Animatable.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/bouncingBehavior.ts:144

___

### \_attachedCamera

• `Private` **\_attachedCamera**: [`Nullable`](../modules.md#nullable)[`ArcRotateCamera`](ArcRotateCamera.md)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/bouncingBehavior.ts:91

___

### \_autoTransitionRange

• `Private` **\_autoTransitionRange**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/bouncingBehavior.ts:48

___

### \_cachedWheelPrecision

• `Private` **\_cachedWheelPrecision**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/bouncingBehavior.ts:145

___

### \_onAfterCheckInputsObserver

• `Private` **\_onAfterCheckInputsObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Camera`](Camera.md)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/bouncingBehavior.ts:92

___

### \_onMeshTargetChangedObserver

• `Private` **\_onMeshTargetChangedObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/bouncingBehavior.ts:93

___

### \_radiusBounceTransition

• `Private` **\_radiusBounceTransition**: [`Nullable`](../modules.md#nullable)[`Animation`](Animation.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/bouncingBehavior.ts:143

___

### \_radiusIsAnimating

• `Private` **\_radiusIsAnimating**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/bouncingBehavior.ts:142

___

### lowerRadiusTransitionRange

• **lowerRadiusTransitionRange**: `number` = `2`

Length of the distance animated by the transition when lower radius is reached

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/bouncingBehavior.ts:41

___

### transitionDuration

• **transitionDuration**: `number` = `450`

The duration of the animation, in milliseconds

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/bouncingBehavior.ts:36

___

### upperRadiusTransitionRange

• **upperRadiusTransitionRange**: `number` = `-2`

Length of the distance animated by the transition when upper radius is reached

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/bouncingBehavior.ts:46

___

### EasingFunction

▪ `Static` **EasingFunction**: [`BackEase`](BackEase.md)

The easing function used by animations

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/bouncingBehavior.ts:26

___

### EasingMode

▪ `Static` **EasingMode**: `number` = `EasingFunction.EASINGMODE_EASEOUT`

The easing mode used by animations

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/bouncingBehavior.ts:31

## Accessors

### autoTransitionRange

• `get` **autoTransitionRange**(): `boolean`

Gets a value indicating if the lowerRadiusTransitionRange and upperRadiusTransitionRange are defined automatically

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/bouncingBehavior.ts:53

• `set` **autoTransitionRange**(`value`): `void`

Sets a value indicating if the lowerRadiusTransitionRange and upperRadiusTransitionRange are defined automatically
Transition ranges will be set to 5% of the bounding box diagonal in world space

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/bouncingBehavior.ts:61

___

### name

• `get` **name**(): `string`

Gets the name of the behavior.

#### Returns

`string`

#### Implementation of

[Behavior](../interfaces/Behavior.md).[name](../interfaces/Behavior.md#name)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/bouncingBehavior.ts:19

## Methods

### \_applyBoundRadiusAnimation

▸ `Private` **_applyBoundRadiusAnimation**(`radiusDelta`): `void`

Applies an animation to the radius of the camera, extending by the radiusDelta.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `radiusDelta` | `number` | The delta by which to animate to. Can be negative. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/bouncingBehavior.ts:167

___

### \_clearAnimationLocks

▸ `Protected` **_clearAnimationLocks**(): `void`

Removes all animation locks. Allows new animations to be added to any of the camera properties.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/bouncingBehavior.ts:203

___

### \_isRadiusAtLimit

▸ `Private` **_isRadiusAtLimit**(`radiusLimit`): `boolean`

Checks if the camera radius is at the specified limit. Takes into account animation locks.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `radiusLimit` | [`Nullable`](../modules.md#nullable)`number` | The limit to check against. |

#### Returns

`boolean`

Bool to indicate if at limit.

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/bouncingBehavior.ts:152

___

### attach

▸ **attach**(`camera`): `void`

Attaches the behavior to its arc rotate camera.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `camera` | [`ArcRotateCamera`](ArcRotateCamera.md) | Defines the camera to attach the behavior to |

#### Returns

`void`

#### Implementation of

[Behavior](../interfaces/Behavior.md).[attach](../interfaces/Behavior.md#attach)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/bouncingBehavior.ts:106

___

### detach

▸ **detach**(): `void`

Detaches the behavior from its current arc rotate camera.

#### Returns

`void`

#### Implementation of

[Behavior](../interfaces/Behavior.md).[detach](../interfaces/Behavior.md#detach)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/bouncingBehavior.ts:128

___

### init

▸ **init**(): `void`

Initializes the behavior.

#### Returns

`void`

#### Implementation of

[Behavior](../interfaces/Behavior.md).[init](../interfaces/Behavior.md#init)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/bouncingBehavior.ts:98

___

### stopAllAnimations

▸ **stopAllAnimations**(): `void`

Stops and removes all animations that have been applied to the camera

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/bouncingBehavior.ts:214
