[@dev/core](../README.md) / [Exports](../modules.md) / AutoRotationBehavior

# Class: AutoRotationBehavior

The autoRotation behavior (AutoRotationBehavior) is designed to create a smooth rotation of an ArcRotateCamera when there is no user interaction.

**`See`**

https://doc.babylonjs.com/how_to/camera_behaviors#autorotation-behavior

## Implements

- [`Behavior`](../interfaces/Behavior.md)[`ArcRotateCamera`](ArcRotateCamera.md)

## Table of contents

### Constructors

- [constructor](AutoRotationBehavior.md#constructor)

### Properties

- [\_attachedCamera](AutoRotationBehavior.md#_attachedcamera)
- [\_cameraRotationSpeed](AutoRotationBehavior.md#_camerarotationspeed)
- [\_idleRotationSpeed](AutoRotationBehavior.md#_idlerotationspeed)
- [\_idleRotationSpinupTime](AutoRotationBehavior.md#_idlerotationspinuptime)
- [\_idleRotationWaitTime](AutoRotationBehavior.md#_idlerotationwaittime)
- [\_isPointerDown](AutoRotationBehavior.md#_ispointerdown)
- [\_lastFrameRadius](AutoRotationBehavior.md#_lastframeradius)
- [\_lastFrameTime](AutoRotationBehavior.md#_lastframetime)
- [\_lastInteractionTime](AutoRotationBehavior.md#_lastinteractiontime)
- [\_onAfterCheckInputsObserver](AutoRotationBehavior.md#_onaftercheckinputsobserver)
- [\_onPrePointerObservableObserver](AutoRotationBehavior.md#_onprepointerobservableobserver)
- [\_zoomStopsAnimation](AutoRotationBehavior.md#_zoomstopsanimation)
- [targetAlpha](AutoRotationBehavior.md#targetalpha)

### Accessors

- [idleRotationSpeed](AutoRotationBehavior.md#idlerotationspeed)
- [idleRotationSpinupTime](AutoRotationBehavior.md#idlerotationspinuptime)
- [idleRotationWaitTime](AutoRotationBehavior.md#idlerotationwaittime)
- [name](AutoRotationBehavior.md#name)
- [rotationInProgress](AutoRotationBehavior.md#rotationinprogress)
- [zoomStopsAnimation](AutoRotationBehavior.md#zoomstopsanimation)

### Methods

- [\_applyUserInteraction](AutoRotationBehavior.md#_applyuserinteraction)
- [\_reachTargetAlpha](AutoRotationBehavior.md#_reachtargetalpha)
- [\_shouldAnimationStopForInteraction](AutoRotationBehavior.md#_shouldanimationstopforinteraction)
- [\_userIsMoving](AutoRotationBehavior.md#_userismoving)
- [\_userIsZooming](AutoRotationBehavior.md#_useriszooming)
- [attach](AutoRotationBehavior.md#attach)
- [detach](AutoRotationBehavior.md#detach)
- [init](AutoRotationBehavior.md#init)
- [resetLastInteractionTime](AutoRotationBehavior.md#resetlastinteractiontime)

## Constructors

### constructor

• **new AutoRotationBehavior**()

## Properties

### \_attachedCamera

• `Private` **\_attachedCamera**: [`Nullable`](../modules.md#nullable)[`ArcRotateCamera`](ArcRotateCamera.md)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/autoRotationBehavior.ts:96

___

### \_cameraRotationSpeed

• `Private` **\_cameraRotationSpeed**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/autoRotationBehavior.ts:100

___

### \_idleRotationSpeed

• `Private` **\_idleRotationSpeed**: `number` = `0.05`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/autoRotationBehavior.ts:24

___

### \_idleRotationSpinupTime

• `Private` **\_idleRotationSpinupTime**: `number` = `2000`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/autoRotationBehavior.ts:26

___

### \_idleRotationWaitTime

• `Private` **\_idleRotationWaitTime**: `number` = `2000`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/autoRotationBehavior.ts:25

___

### \_isPointerDown

• `Private` **\_isPointerDown**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/autoRotationBehavior.ts:97

___

### \_lastFrameRadius

• `Private` **\_lastFrameRadius**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/autoRotationBehavior.ts:200

___

### \_lastFrameTime

• `Private` **\_lastFrameTime**: [`Nullable`](../modules.md#nullable)`number` = `null`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/autoRotationBehavior.ts:98

___

### \_lastInteractionTime

• `Private` **\_lastInteractionTime**: `number` = `-Infinity`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/autoRotationBehavior.ts:99

___

### \_onAfterCheckInputsObserver

• `Private` **\_onAfterCheckInputsObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Camera`](Camera.md)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/autoRotationBehavior.ts:95

___

### \_onPrePointerObservableObserver

• `Private` **\_onPrePointerObservableObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`PointerInfoPre`](PointerInfoPre.md)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/autoRotationBehavior.ts:94

___

### \_zoomStopsAnimation

• `Private` **\_zoomStopsAnimation**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/autoRotationBehavior.ts:23

___

### targetAlpha

• **targetAlpha**: [`Nullable`](../modules.md#nullable)`number` = `null`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/autoRotationBehavior.ts:28

## Accessors

### idleRotationSpeed

• `get` **idleRotationSpeed**(): `number`

Gets the default speed at which the camera rotates around the model.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/autoRotationBehavior.ts:54

• `set` **idleRotationSpeed**(`speed`): `void`

Sets the default speed at which the camera rotates around the model.

#### Parameters

| Name | Type |
| :------ | :------ |
| `speed` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/autoRotationBehavior.ts:47

___

### idleRotationSpinupTime

• `get` **idleRotationSpinupTime**(): `number`

Gets the time (milliseconds) to take to spin up to the full idle rotation speed.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/autoRotationBehavior.ts:82

• `set` **idleRotationSpinupTime**(`time`): `void`

Sets the time (milliseconds) to take to spin up to the full idle rotation speed.

#### Parameters

| Name | Type |
| :------ | :------ |
| `time` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/autoRotationBehavior.ts:75

___

### idleRotationWaitTime

• `get` **idleRotationWaitTime**(): `number`

Gets the time (milliseconds) to wait after user interaction before the camera starts rotating.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/autoRotationBehavior.ts:68

• `set` **idleRotationWaitTime**(`time`): `void`

Sets the time (in milliseconds) to wait after user interaction before the camera starts rotating.

#### Parameters

| Name | Type |
| :------ | :------ |
| `time` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/autoRotationBehavior.ts:61

___

### name

• `get` **name**(): `string`

Gets the name of the behavior.

#### Returns

`string`

#### Implementation of

[Behavior](../interfaces/Behavior.md).[name](../interfaces/Behavior.md#name)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/autoRotationBehavior.ts:19

___

### rotationInProgress

• `get` **rotationInProgress**(): `boolean`

Gets a value indicating if the camera is currently rotating because of this behavior

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/autoRotationBehavior.ts:89

___

### zoomStopsAnimation

• `get` **zoomStopsAnimation**(): `boolean`

Gets the flag that indicates if user zooming should stop animation.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/autoRotationBehavior.ts:40

• `set` **zoomStopsAnimation**(`flag`): `void`

Sets the flag that indicates if user zooming should stop animation.

#### Parameters

| Name | Type |
| :------ | :------ |
| `flag` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/autoRotationBehavior.ts:33

## Methods

### \_applyUserInteraction

▸ `Private` **_applyUserInteraction**(): `void`

Applies any current user interaction to the camera. Takes into account maximum alpha rotation.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/autoRotationBehavior.ts:219

___

### \_reachTargetAlpha

▸ `Private` **_reachTargetAlpha**(): `boolean`

Returns true if camera alpha reaches the target alpha

#### Returns

`boolean`

true if camera alpha reaches the target alpha

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/autoRotationBehavior.ts:182

___

### \_shouldAnimationStopForInteraction

▸ `Private` **_shouldAnimationStopForInteraction**(): `boolean`

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/autoRotationBehavior.ts:201

___

### \_userIsMoving

▸ `Private` **_userIsMoving**(): `boolean`

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/autoRotationBehavior.ts:226

___

### \_userIsZooming

▸ `Private` **_userIsZooming**(): `boolean`

Returns true if user is scrolling.

#### Returns

`boolean`

true if user is scrolling.

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/autoRotationBehavior.ts:193

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

https://github.com/babylon.js/core/src/Behaviors/Cameras/autoRotationBehavior.ts:113

___

### detach

▸ **detach**(): `void`

Detaches the behavior from its current arc rotate camera.

#### Returns

`void`

#### Implementation of

[Behavior](../interfaces/Behavior.md).[detach](../interfaces/Behavior.md#detach)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/autoRotationBehavior.ts:156

___

### init

▸ **init**(): `void`

Initializes the behavior.

#### Returns

`void`

#### Implementation of

[Behavior](../interfaces/Behavior.md).[init](../interfaces/Behavior.md#init)

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/autoRotationBehavior.ts:105

___

### resetLastInteractionTime

▸ **resetLastInteractionTime**(`customTime?`): `void`

Force-reset the last interaction time

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `customTime?` | `number` | an optional time that will be used instead of the current last interaction time. For example `Date.now()` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Behaviors/Cameras/autoRotationBehavior.ts:174
