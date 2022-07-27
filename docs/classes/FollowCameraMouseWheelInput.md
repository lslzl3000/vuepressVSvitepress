[@dev/core](../README.md) / [Exports](../modules.md) / FollowCameraMouseWheelInput

# Class: FollowCameraMouseWheelInput

Manage the mouse wheel inputs to control a follow camera.

**`See`**

https://doc.babylonjs.com/how_to/customizing_camera_inputs

## Implements

- [`ICameraInput`](../interfaces/ICameraInput.md)[`FollowCamera`](FollowCamera.md)

## Table of contents

### Constructors

- [constructor](FollowCameraMouseWheelInput.md#constructor)

### Properties

- [\_observer](FollowCameraMouseWheelInput.md#_observer)
- [\_wheel](FollowCameraMouseWheelInput.md#_wheel)
- [axisControlHeight](FollowCameraMouseWheelInput.md#axiscontrolheight)
- [axisControlRadius](FollowCameraMouseWheelInput.md#axiscontrolradius)
- [axisControlRotation](FollowCameraMouseWheelInput.md#axiscontrolrotation)
- [camera](FollowCameraMouseWheelInput.md#camera)
- [wheelDeltaPercentage](FollowCameraMouseWheelInput.md#wheeldeltapercentage)
- [wheelPrecision](FollowCameraMouseWheelInput.md#wheelprecision)

### Methods

- [attachControl](FollowCameraMouseWheelInput.md#attachcontrol)
- [detachControl](FollowCameraMouseWheelInput.md#detachcontrol)
- [getClassName](FollowCameraMouseWheelInput.md#getclassname)
- [getSimpleName](FollowCameraMouseWheelInput.md#getsimplename)

## Constructors

### constructor

• **new FollowCameraMouseWheelInput**()

## Properties

### \_observer

• `Private` **\_observer**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`PointerInfo`](PointerInfo.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraMouseWheelInput.ts:55

___

### \_wheel

• `Private` **\_wheel**: [`Nullable`](../modules.md#nullable)(`p`: [`PointerInfo`](PointerInfo.md), `s`: [`EventState`](EventState.md)) => `void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraMouseWheelInput.ts:54

___

### axisControlHeight

• **axisControlHeight**: `boolean` = `false`

Moue wheel controls height. (Mouse wheel modifies camera.heightOffset value.)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraMouseWheelInput.ts:32

___

### axisControlRadius

• **axisControlRadius**: `boolean` = `true`

Moue wheel controls zoom. (Mouse wheel modifies camera.radius value.)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraMouseWheelInput.ts:26

___

### axisControlRotation

• **axisControlRotation**: `boolean` = `false`

Moue wheel controls angle. (Mouse wheel modifies camera.rotationOffset value.)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraMouseWheelInput.ts:38

___

### camera

• **camera**: [`FollowCamera`](FollowCamera.md)

Defines the camera the input is attached to.

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[camera](../interfaces/ICameraInput.md#camera)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraMouseWheelInput.ts:20

___

### wheelDeltaPercentage

• **wheelDeltaPercentage**: `number` = `0`

wheelDeltaPercentage will be used instead of wheelPrecision if different from 0.
It defines the percentage of current camera.radius to use as delta when wheel is used.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraMouseWheelInput.ts:52

___

### wheelPrecision

• **wheelPrecision**: `number` = `3.0`

Gets or Set the mouse wheel precision or how fast is the camera moves in
relation to mouseWheel events.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraMouseWheelInput.ts:45

## Methods

### attachControl

▸ **attachControl**(`noPreventDefault?`): `void`

Attach the input controls to a specific dom element to get the input from.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `noPreventDefault?` | `boolean` | Defines whether event caught by the controls should call preventdefault() (https://developer.mozilla.org/en-US/docs/Web/API/Event/preventDefault) |

#### Returns

`void`

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[attachControl](../interfaces/ICameraInput.md#attachcontrol)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraMouseWheelInput.ts:61

___

### detachControl

▸ **detachControl**(): `void`

Detach the current controls from the specified dom element.

#### Returns

`void`

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[detachControl](../interfaces/ICameraInput.md#detachcontrol)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraMouseWheelInput.ts:123

___

### getClassName

▸ **getClassName**(): `string`

Gets the class name of the current input.

#### Returns

`string`

the class name

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[getClassName](../interfaces/ICameraInput.md#getclassname)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraMouseWheelInput.ts:135

___

### getSimpleName

▸ **getSimpleName**(): `string`

Get the friendly name associated with the input class.

#### Returns

`string`

the input friendly name

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[getSimpleName](../interfaces/ICameraInput.md#getsimplename)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/followCameraMouseWheelInput.ts:143
