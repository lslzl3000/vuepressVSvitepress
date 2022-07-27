[@dev/core](../README.md) / [Exports](../modules.md) / ICameraInput

# Interface: ICameraInputTCamera

This is the contract to implement in order to create a new input class.
Inputs are dealing with listening to user actions and moving the camera accordingly.

## Type parameters

| Name | Type |
| :------ | :------ |
| `TCamera` | extends [`Camera`](../classes/Camera.md) |

## Implemented by

- [`ArcRotateCameraGamepadInput`](../classes/ArcRotateCameraGamepadInput.md)
- [`ArcRotateCameraKeyboardMoveInput`](../classes/ArcRotateCameraKeyboardMoveInput.md)
- [`ArcRotateCameraMouseWheelInput`](../classes/ArcRotateCameraMouseWheelInput.md)
- [`ArcRotateCameraVRDeviceOrientationInput`](../classes/ArcRotateCameraVRDeviceOrientationInput.md)
- [`BaseCameraMouseWheelInput`](../classes/BaseCameraMouseWheelInput.md)
- [`BaseCameraPointersInput`](../classes/BaseCameraPointersInput.md)
- [`FlyCameraKeyboardInput`](../classes/FlyCameraKeyboardInput.md)
- [`FlyCameraMouseInput`](../classes/FlyCameraMouseInput.md)
- [`FollowCameraKeyboardMoveInput`](../classes/FollowCameraKeyboardMoveInput.md)
- [`FollowCameraMouseWheelInput`](../classes/FollowCameraMouseWheelInput.md)
- [`FreeCameraDeviceOrientationInput`](../classes/FreeCameraDeviceOrientationInput.md)
- [`FreeCameraGamepadInput`](../classes/FreeCameraGamepadInput.md)
- [`FreeCameraKeyboardMoveInput`](../classes/FreeCameraKeyboardMoveInput.md)
- [`FreeCameraMouseInput`](../classes/FreeCameraMouseInput.md)
- [`FreeCameraTouchInput`](../classes/FreeCameraTouchInput.md)
- [`FreeCameraVirtualJoystickInput`](../classes/FreeCameraVirtualJoystickInput.md)

## Table of contents

### Properties

- [camera](ICameraInput.md#camera)
- [checkInputs](ICameraInput.md#checkinputs)

### Methods

- [attachControl](ICameraInput.md#attachcontrol)
- [detachControl](ICameraInput.md#detachcontrol)
- [getClassName](ICameraInput.md#getclassname)
- [getSimpleName](ICameraInput.md#getsimplename)

## Properties

### camera

• **camera**: [`Nullable`](../modules.md#nullable)`TCamera`

Defines the camera the input is attached to.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/cameraInputsManager.ts:21

___

### checkInputs

• `Optional` **checkInputs**: () => `void`

#### Type declaration

▸ (): `void`

Update the current camera state depending on the inputs that have been used this frame.
This is a dynamically created lambda to avoid the performance penalty of looping for inputs in the render loop.

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/cameraInputsManager.ts:45

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

#### Defined in

https://github.com/babylon.js/core/src/Cameras/cameraInputsManager.ts:36

___

### detachControl

▸ **detachControl**(): `void`

Detach the current controls from the specified dom element.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/cameraInputsManager.ts:40

___

### getClassName

▸ **getClassName**(): `string`

Gets the class name of the current input.

#### Returns

`string`

the class name

#### Defined in

https://github.com/babylon.js/core/src/Cameras/cameraInputsManager.ts:26

___

### getSimpleName

▸ **getSimpleName**(): `string`

Get the friendly name associated with the input class.

#### Returns

`string`

the input friendly name

#### Defined in

https://github.com/babylon.js/core/src/Cameras/cameraInputsManager.ts:31
