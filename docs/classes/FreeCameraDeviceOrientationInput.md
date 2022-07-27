[@dev/core](../README.md) / [Exports](../modules.md) / FreeCameraDeviceOrientationInput

# Class: FreeCameraDeviceOrientationInput

Takes information about the orientation of the device as reported by the deviceorientation event to orient the camera.
Screen rotation is taken into account.

**`See`**

https://doc.babylonjs.com/how_to/customizing_camera_inputs

## Implements

- [`ICameraInput`](../interfaces/ICameraInput.md)[`FreeCamera`](FreeCamera.md)

## Table of contents

### Constructors

- [constructor](FreeCameraDeviceOrientationInput.md#constructor)

### Properties

- [\_alpha](FreeCameraDeviceOrientationInput.md#_alpha)
- [\_beta](FreeCameraDeviceOrientationInput.md#_beta)
- [\_camera](FreeCameraDeviceOrientationInput.md#_camera)
- [\_constantTranform](FreeCameraDeviceOrientationInput.md#_constanttranform)
- [\_gamma](FreeCameraDeviceOrientationInput.md#_gamma)
- [\_screenOrientationAngle](FreeCameraDeviceOrientationInput.md#_screenorientationangle)
- [\_screenQuaternion](FreeCameraDeviceOrientationInput.md#_screenquaternion)

### Accessors

- [camera](FreeCameraDeviceOrientationInput.md#camera)

### Methods

- [\_deviceOrientation](FreeCameraDeviceOrientationInput.md#_deviceorientation)
- [\_orientationChanged](FreeCameraDeviceOrientationInput.md#_orientationchanged)
- [attachControl](FreeCameraDeviceOrientationInput.md#attachcontrol)
- [checkInputs](FreeCameraDeviceOrientationInput.md#checkinputs)
- [detachControl](FreeCameraDeviceOrientationInput.md#detachcontrol)
- [getClassName](FreeCameraDeviceOrientationInput.md#getclassname)
- [getSimpleName](FreeCameraDeviceOrientationInput.md#getsimplename)
- [WaitForOrientationChangeAsync](FreeCameraDeviceOrientationInput.md#waitfororientationchangeasync)

## Constructors

### constructor

• **new FreeCameraDeviceOrientationInput**()

Instantiates a new input

**`See`**

https://doc.babylonjs.com/how_to/customizing_camera_inputs

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraDeviceOrientationInput.ts:106

## Properties

### \_alpha

• `Private` **\_alpha**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraDeviceOrientationInput.ts:51

___

### \_beta

• `Private` **\_beta**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraDeviceOrientationInput.ts:52

___

### \_camera

• `Private` **\_camera**: [`FreeCamera`](FreeCamera.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraDeviceOrientationInput.ts:44

___

### \_constantTranform

• `Private` **\_constantTranform**: [`Quaternion`](Quaternion.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraDeviceOrientationInput.ts:48

___

### \_gamma

• `Private` **\_gamma**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraDeviceOrientationInput.ts:53

___

### \_screenOrientationAngle

• `Private` **\_screenOrientationAngle**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraDeviceOrientationInput.ts:46

___

### \_screenQuaternion

• `Private` **\_screenQuaternion**: [`Quaternion`](Quaternion.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraDeviceOrientationInput.ts:49

## Accessors

### camera

• `get` **camera**(): [`FreeCamera`](FreeCamera.md)

Define the camera controlled by the input.

#### Returns

[`FreeCamera`](FreeCamera.md)

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[camera](../interfaces/ICameraInput.md#camera)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraDeviceOrientationInput.ts:114

• `set` **camera**(`camera`): `void`

Defines the camera the input is attached to.

#### Parameters

| Name | Type |
| :------ | :------ |
| `camera` | [`FreeCamera`](FreeCamera.md) |

#### Returns

`void`

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[camera](../interfaces/ICameraInput.md#camera)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraDeviceOrientationInput.ts:118

## Methods

### \_deviceOrientation

▸ `Private` **_deviceOrientation**(`evt`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `evt` | `DeviceOrientationEvent` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraDeviceOrientationInput.ts:174

___

### \_orientationChanged

▸ `Private` **_orientationChanged**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraDeviceOrientationInput.ts:163

___

### attachControl

▸ **attachControl**(): `void`

Attach the input controls to a specific dom element to get the input from.

#### Returns

`void`

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[attachControl](../interfaces/ICameraInput.md#attachcontrol)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraDeviceOrientationInput.ts:133

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

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraDeviceOrientationInput.ts:196

___

### detachControl

▸ **detachControl**(): `void`

Detach the current controls from the specified dom element.

#### Returns

`void`

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[detachControl](../interfaces/ICameraInput.md#detachcontrol)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraDeviceOrientationInput.ts:186

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

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraDeviceOrientationInput.ts:214

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

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraDeviceOrientationInput.ts:222

___

### WaitForOrientationChangeAsync

▸ `Static` **WaitForOrientationChangeAsync**(`timeout?`): `Promise``void`

Can be used to detect if a device orientation sensor is available on a device

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `timeout?` | `number` | amount of time in milliseconds to wait for a response from the sensor (default: infinite) |

#### Returns

`Promise``void`

a promise that will resolve on orientation change

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraDeviceOrientationInput.ts:60
