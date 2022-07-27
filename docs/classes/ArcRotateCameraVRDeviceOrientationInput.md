[@dev/core](../README.md) / [Exports](../modules.md) / ArcRotateCameraVRDeviceOrientationInput

# Class: ArcRotateCameraVRDeviceOrientationInput

Manage the device orientation inputs (gyroscope) to control an arc rotate camera.

**`See`**

https://doc.babylonjs.com/how_to/customizing_camera_inputs

## Implements

- [`ICameraInput`](../interfaces/ICameraInput.md)[`ArcRotateCamera`](ArcRotateCamera.md)

## Table of contents

### Constructors

- [constructor](ArcRotateCameraVRDeviceOrientationInput.md#constructor)

### Properties

- [\_alpha](ArcRotateCameraVRDeviceOrientationInput.md#_alpha)
- [\_deviceOrientationHandler](ArcRotateCameraVRDeviceOrientationInput.md#_deviceorientationhandler)
- [\_dirty](ArcRotateCameraVRDeviceOrientationInput.md#_dirty)
- [\_gamma](ArcRotateCameraVRDeviceOrientationInput.md#_gamma)
- [alphaCorrection](ArcRotateCameraVRDeviceOrientationInput.md#alphacorrection)
- [camera](ArcRotateCameraVRDeviceOrientationInput.md#camera)
- [gammaCorrection](ArcRotateCameraVRDeviceOrientationInput.md#gammacorrection)

### Methods

- [attachControl](ArcRotateCameraVRDeviceOrientationInput.md#attachcontrol)
- [checkInputs](ArcRotateCameraVRDeviceOrientationInput.md#checkinputs)
- [detachControl](ArcRotateCameraVRDeviceOrientationInput.md#detachcontrol)
- [getClassName](ArcRotateCameraVRDeviceOrientationInput.md#getclassname)
- [getSimpleName](ArcRotateCameraVRDeviceOrientationInput.md#getsimplename)

## Constructors

### constructor

• **new ArcRotateCameraVRDeviceOrientationInput**()

Instantiate a new ArcRotateCameraVRDeviceOrientationInput.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraVRDeviceOrientationInput.ts:56

## Properties

### \_alpha

• `Private` **\_alpha**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraVRDeviceOrientationInput.ts:47

___

### \_deviceOrientationHandler

• `Private` **\_deviceOrientationHandler**: () => `void`

#### Type declaration

▸ (): `void`

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraVRDeviceOrientationInput.ts:51

___

### \_dirty

• `Private` **\_dirty**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraVRDeviceOrientationInput.ts:49

___

### \_gamma

• `Private` **\_gamma**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraVRDeviceOrientationInput.ts:48

___

### alphaCorrection

• **alphaCorrection**: `number` = `1`

Defines a correction factor applied on the alpha value retrieved from the orientation events.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraVRDeviceOrientationInput.ts:40

___

### camera

• **camera**: [`ArcRotateCamera`](ArcRotateCamera.md)

Defines the camera the input is attached to.

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[camera](../interfaces/ICameraInput.md#camera)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraVRDeviceOrientationInput.ts:35

___

### gammaCorrection

• **gammaCorrection**: `number` = `1`

Defines a correction factor applied on the gamma value retrieved from the orientation events.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraVRDeviceOrientationInput.ts:45

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

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraVRDeviceOrientationInput.ts:64

___

### checkInputs

▸ **checkInputs**(): `void`

Update the current camera state depending on the inputs that have been used this frame.
This is a dynamically created lambda to avoid the performance penalty of looping for inputs in the render loop.

#### Returns

`void`

#### Implementation of

ICameraInput.checkInputs

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraVRDeviceOrientationInput.ts:112

___

### detachControl

▸ **detachControl**(): `void`

Detach the current controls from the specified dom element.

#### Returns

`void`

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[detachControl](../interfaces/ICameraInput.md#detachcontrol)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraVRDeviceOrientationInput.ts:128

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

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraVRDeviceOrientationInput.ts:136

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

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraVRDeviceOrientationInput.ts:144
