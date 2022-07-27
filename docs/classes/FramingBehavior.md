[@dev/core](../README.md) / [Exports](../modules.md) / FramingBehavior

# Class: FramingBehavior

The framing behavior (FramingBehavior) is designed to automatically position an ArcRotateCamera when its target is set to a mesh. It is also useful if you want to prevent the camera to go under a virtual horizontal plane.

**`See`**

https://doc.babylonjs.com/how_to/camera_behaviors#framing-behavior

## Implements

- [`Behavior`](../interfaces/Behavior.md)[`ArcRotateCamera`](ArcRotateCamera.md)

## Table of contents

### Constructors

- [constructor](FramingBehavior.md#constructor)

### Properties

- [\_animatables](FramingBehavior.md#_animatables)
- [\_attachedCamera](FramingBehavior.md#_attachedcamera)
- [\_betaIsAnimating](FramingBehavior.md#_betaisanimating)
- [\_betaTransition](FramingBehavior.md#_betatransition)
- [\_defaultElevation](FramingBehavior.md#_defaultelevation)
- [\_elevationReturnTime](FramingBehavior.md#_elevationreturntime)
- [\_elevationReturnWaitTime](FramingBehavior.md#_elevationreturnwaittime)
- [\_framingTime](FramingBehavior.md#_framingtime)
- [\_isPointerDown](FramingBehavior.md#_ispointerdown)
- [\_lastInteractionTime](FramingBehavior.md#_lastinteractiontime)
- [\_mode](FramingBehavior.md#_mode)
- [\_onAfterCheckInputsObserver](FramingBehavior.md#_onaftercheckinputsobserver)
- [\_onMeshTargetChangedObserver](FramingBehavior.md#_onmeshtargetchangedobserver)
- [\_onPrePointerObservableObserver](FramingBehavior.md#_onprepointerobservableobserver)
- [\_positionScale](FramingBehavior.md#_positionscale)
- [\_radiusScale](FramingBehavior.md#_radiusscale)
- [\_radiusTransition](FramingBehavior.md#_radiustransition)
- [\_vectorTransition](FramingBehavior.md#_vectortransition)
- [\_zoomStopsAnimation](FramingBehavior.md#_zoomstopsanimation)
- [autoCorrectCameraLimitsAndSensibility](FramingBehavior.md#autocorrectcameralimitsandsensibility)
- [onTargetFramingAnimationEndObservable](FramingBehavior.md#ontargetframinganimationendobservable)
- [EasingFunction](FramingBehavior.md#easingfunction)
- [EasingMode](FramingBehavior.md#easingmode)
- [FitFrustumSidesMode](FramingBehavior.md#fitfrustumsidesmode)
- [IgnoreBoundsSizeMode](FramingBehavior.md#ignoreboundssizemode)

### Accessors

- [defaultElevation](FramingBehavior.md#defaultelevation)
- [elevationReturnTime](FramingBehavior.md#elevationreturntime)
- [elevationReturnWaitTime](FramingBehavior.md#elevationreturnwaittime)
- [framingTime](FramingBehavior.md#framingtime)
- [isUserIsMoving](FramingBehavior.md#isuserismoving)
- [mode](FramingBehavior.md#mode)
- [name](FramingBehavior.md#name)
- [positionScale](FramingBehavior.md#positionscale)
- [radiusScale](FramingBehavior.md#radiusscale)
- [zoomStopsAnimation](FramingBehavior.md#zoomstopsanimation)

### Methods

- [\_applyUserInteraction](FramingBehavior.md#_applyuserinteraction)
- [\_calculateLowerRadiusFromModelBoundingSphere](FramingBehavior.md#_calculatelowerradiusfrommodelboundingsphere)
- [\_clearAnimationLocks](FramingBehavior.md#_clearanimationlocks)
- [\_getFrustumSlope](FramingBehavior.md#_getfrustumslope)
- [\_maintainCameraAboveGround](FramingBehavior.md#_maintaincameraaboveground)
- [attach](FramingBehavior.md#attach)
- [detach](FramingBehavior.md#detach)
- [init](FramingBehavior.md#init)
- [stopAllAnimations](FramingBehavior.md#stopallanimations)
- [zoomOnBoundingInfo](FramingBehavior.md#zoomonboundinginfo)
- [zoomOnMesh](FramingBehavior.md#zoomonmesh)
- [zoomOnMeshHierarchy](FramingBehavior.md#zoomonmeshhierarchy)
- [zoomOnMeshesHierarchy](FramingBehavior.md#zoomonmesheshierarchy)

## Constructors

### constructor

• **new FramingBehavior**()

## Properties

### \_animatables

• `Private` **\_animatables**: [`Animatable`](Animatable.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:255

___

### \_attachedCamera

• `Private` **\_attachedCamera**: [`Nullable`](../modules.md#nullable)[`ArcRotateCamera`](ArcRotateCamera.md)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:179

___

### \_betaIsAnimating

• `Private` **\_betaIsAnimating**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:256

___

### \_betaTransition

• `Private` **\_betaTransition**: [`Animation`](Animation.md)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:257

___

### \_defaultElevation

• `Private` **\_defaultElevation**: `number` = `0.3`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:37

___

### \_elevationReturnTime

• `Private` **\_elevationReturnTime**: `number` = `1500`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:38

___

### \_elevationReturnWaitTime

• `Private` **\_elevationReturnWaitTime**: `number` = `1000`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:39

___

### \_framingTime

• `Private` **\_framingTime**: `number` = `1500`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:41

___

### \_isPointerDown

• `Private` **\_isPointerDown**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:180

___

### \_lastInteractionTime

• `Private` **\_lastInteractionTime**: `number` = `-Infinity`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:181

___

### \_mode

• `Private` **\_mode**: `number` = `FramingBehavior.FitFrustumSidesMode`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:34

___

### \_onAfterCheckInputsObserver

• `Private` **\_onAfterCheckInputsObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Camera`](Camera.md)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:177

___

### \_onMeshTargetChangedObserver

• `Private` **\_onMeshTargetChangedObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:178

___

### \_onPrePointerObservableObserver

• `Private` **\_onPrePointerObservableObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`PointerInfoPre`](PointerInfoPre.md)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:176

___

### \_positionScale

• `Private` **\_positionScale**: `number` = `0.5`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:36

___

### \_radiusScale

• `Private` **\_radiusScale**: `number` = `1.0`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:35

___

### \_radiusTransition

• `Private` **\_radiusTransition**: [`Animation`](Animation.md)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:258

___

### \_vectorTransition

• `Private` **\_vectorTransition**: [`Animation`](Animation.md)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:259

___

### \_zoomStopsAnimation

• `Private` **\_zoomStopsAnimation**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:40

___

### autoCorrectCameraLimitsAndSensibility

• **autoCorrectCameraLimitsAndSensibility**: `boolean` = `true`

Define if the behavior should automatically change the configured
camera limits and sensibilities.

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:173

___

### onTargetFramingAnimationEndObservable

• **onTargetFramingAnimationEndObservable**: [`Observable`](Observable.md)`void`

An event triggered when the animation to zoom on target mesh has ended

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:32

___

### EasingFunction

▪ `Static` **EasingFunction**: [`ExponentialEase`](ExponentialEase.md)

The easing function used by animations

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:46

___

### EasingMode

▪ `Static` **EasingMode**: `number` = `EasingFunction.EASINGMODE_EASEINOUT`

The easing mode used by animations

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:51

___

### FitFrustumSidesMode

▪ `Static` **FitFrustumSidesMode**: `number` = `1`

The camera is not allowed to zoom closer to the mesh than the point at which the adjusted bounding sphere touches the frustum sides

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:562

___

### IgnoreBoundsSizeMode

▪ `Static` **IgnoreBoundsSizeMode**: `number` = `0`

The camera can move all the way towards the mesh.

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:557

## Accessors

### defaultElevation

• `get` **defaultElevation**(): `number`

Gets the angle above/below the horizontal plane to return to when the return to default elevation idle
behaviour is triggered, in radians.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:107

• `set` **defaultElevation**(`elevation`): `void`

Sets the angle above/below the horizontal plane to return to when the return to default elevation idle
behaviour is triggered, in radians.

#### Parameters

| Name | Type |
| :------ | :------ |
| `elevation` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:99

___

### elevationReturnTime

• `get` **elevationReturnTime**(): `number`

Gets the time (in milliseconds) taken to return to the default beta position.
Negative value indicates camera should not return to default.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:123

• `set` **elevationReturnTime**(`speed`): `void`

Sets the time (in milliseconds) taken to return to the default beta position.
Negative value indicates camera should not return to default.

#### Parameters

| Name | Type |
| :------ | :------ |
| `speed` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:115

___

### elevationReturnWaitTime

• `get` **elevationReturnWaitTime**(): `number`

Gets the delay (in milliseconds) taken before the camera returns to the default beta position.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:137

• `set` **elevationReturnWaitTime**(`time`): `void`

Sets the delay (in milliseconds) taken before the camera returns to the default beta position.

#### Parameters

| Name | Type |
| :------ | :------ |
| `time` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:130

___

### framingTime

• `get` **framingTime**(): `number`

Gets the transition time when framing the mesh, in milliseconds

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:165

• `set` **framingTime**(`time`): `void`

Sets the transition time when framing the mesh, in milliseconds

#### Parameters

| Name | Type |
| :------ | :------ |
| `time` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:158

___

### isUserIsMoving

• `get` **isUserIsMoving**(): `boolean`

Gets a value indicating if the user is moving the camera

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:537

___

### mode

• `get` **mode**(): `number`

Gets current mode used by the behavior.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:63

• `set` **mode**(`mode`): `void`

Sets the current mode used by the behavior

#### Parameters

| Name | Type |
| :------ | :------ |
| `mode` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:56

___

### name

• `get` **name**(): `string`

Gets the name of the behavior.

#### Returns

`string`

#### Implementation of

[Behavior](../interfaces/Behavior.md).[name](../interfaces/Behavior.md#name)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:25

___

### positionScale

• `get` **positionScale**(): `number`

Gets the scale to apply on Y axis to position camera focus. 0.5 by default which means the center of the bounding box.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:91

• `set` **positionScale**(`scale`): `void`

Sets the scale to apply on Y axis to position camera focus. 0.5 by default which means the center of the bounding box.

#### Parameters

| Name | Type |
| :------ | :------ |
| `scale` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:84

___

### radiusScale

• `get` **radiusScale**(): `number`

Gets the scale applied to the radius

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:77

• `set` **radiusScale**(`radius`): `void`

Sets the scale applied to the radius (1 by default)

#### Parameters

| Name | Type |
| :------ | :------ |
| `radius` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:70

___

### zoomStopsAnimation

• `get` **zoomStopsAnimation**(): `boolean`

Gets the flag that indicates if user zooming should stop animation.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:151

• `set` **zoomStopsAnimation**(`flag`): `void`

Sets the flag that indicates if user zooming should stop animation.

#### Parameters

| Name | Type |
| :------ | :------ |
| `flag` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:144

## Methods

### \_applyUserInteraction

▸ `Private` **_applyUserInteraction**(): `void`

Applies any current user interaction to the camera. Takes into account maximum alpha rotation.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:509

___

### \_calculateLowerRadiusFromModelBoundingSphere

▸ `Protected` **_calculateLowerRadiusFromModelBoundingSphere**(`minimumWorld`, `maximumWorld`): `number`

Calculates the lowest radius for the camera based on the bounding box of the mesh.

#### Parameters

| Name | Type |
| :------ | :------ |
| `minimumWorld` | [`Vector3`](Vector3.md) |
| `maximumWorld` | [`Vector3`](Vector3.md) |

#### Returns

`number`

The minimum distance from the primary mesh's center point at which the camera must be kept in order
		 to fully enclose the mesh in the viewing frustum.

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:394

___

### \_clearAnimationLocks

▸ `Private` **_clearAnimationLocks**(): `void`

Removes all animation locks. Allows new animations to be added to any of the arcCamera properties.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:502

___

### \_getFrustumSlope

▸ `Private` **_getFrustumSlope**(): [`Vector2`](Vector2.md)

Returns the frustum slope based on the canvas ratio and camera FOV

#### Returns

[`Vector2`](Vector2.md)

The frustum slope represented as a Vector2 with X and Y slopes

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:475

___

### \_maintainCameraAboveGround

▸ `Private` **_maintainCameraAboveGround**(): `void`

Keeps the camera above the ground plane. If the user pulls the camera below the ground plane, the camera
is automatically returned to its default position (expected to be above ground plane).

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:431

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

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:194

___

### detach

▸ **detach**(): `void`

Detaches the behavior from its current arc rotate camera.

#### Returns

`void`

#### Implementation of

[Behavior](../interfaces/Behavior.md).[detach](../interfaces/Behavior.md#detach)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:232

___

### init

▸ **init**(): `void`

Initializes the behavior.

#### Returns

`void`

#### Implementation of

[Behavior](../interfaces/Behavior.md).[init](../interfaces/Behavior.md#init)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:186

___

### stopAllAnimations

▸ **stopAllAnimations**(): `void`

Stops and removes all animations that have been applied to the camera

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:520

___

### zoomOnBoundingInfo

▸ **zoomOnBoundingInfo**(`minimumWorld`, `maximumWorld`, `focusOnOriginXZ?`, `onAnimationEnd?`): `void`

Targets the bounding box info defined by its extends and updates zoom level accordingly.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `minimumWorld` | [`Vector3`](Vector3.md) | `undefined` | Determines the smaller position of the bounding box extend |
| `maximumWorld` | [`Vector3`](Vector3.md) | `undefined` | Determines the bigger position of the bounding box extend |
| `focusOnOriginXZ` | `boolean` | `false` | Determines if the camera should focus on 0 in the X and Z axis instead of the mesh |
| `onAnimationEnd` | [`Nullable`](../modules.md#nullable)() => `void` | `null` | Callback triggered at the end of the framing animation |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:313

___

### zoomOnMesh

▸ **zoomOnMesh**(`mesh`, `focusOnOriginXZ?`, `onAnimationEnd?`): `void`

Targets the given mesh and updates zoom level accordingly.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | `undefined` | The mesh to target. |
| `focusOnOriginXZ` | `boolean` | `false` | Determines if the camera should focus on 0 in the X and Z axis instead of the mesh |
| `onAnimationEnd` | [`Nullable`](../modules.md#nullable)() => `void` | `null` | Callback triggered at the end of the framing animation |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:267

___

### zoomOnMeshHierarchy

▸ **zoomOnMeshHierarchy**(`mesh`, `focusOnOriginXZ?`, `onAnimationEnd?`): `void`

Targets the given mesh with its children and updates zoom level accordingly.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | `undefined` | The mesh to target. |
| `focusOnOriginXZ` | `boolean` | `false` | Determines if the camera should focus on 0 in the X and Z axis instead of the mesh |
| `onAnimationEnd` | [`Nullable`](../modules.md#nullable)() => `void` | `null` | Callback triggered at the end of the framing animation |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:280

___

### zoomOnMeshesHierarchy

▸ **zoomOnMeshesHierarchy**(`meshes`, `focusOnOriginXZ?`, `onAnimationEnd?`): `void`

Targets the given meshes with their children and updates zoom level accordingly.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `meshes` | [`AbstractMesh`](AbstractMesh.md)[] | `undefined` | The mesh to target. |
| `focusOnOriginXZ` | `boolean` | `false` | Determines if the camera should focus on 0 in the X and Z axis instead of the mesh |
| `onAnimationEnd` | [`Nullable`](../modules.md#nullable)() => `void` | `null` | Callback triggered at the end of the framing animation |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/framingBehavior.ts:293
