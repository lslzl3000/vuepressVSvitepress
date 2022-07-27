[@dev/core](../README.md) / [Exports](../modules.md) / FreeCameraGamepadInput

# Class: FreeCameraGamepadInput

Manage the gamepad inputs to control a free camera.

**`See`**

https://doc.babylonjs.com/how_to/customizing_camera_inputs

## Implements

- [`ICameraInput`](../interfaces/ICameraInput.md)[`FreeCamera`](FreeCamera.md)

## Table of contents

### Constructors

- [constructor](FreeCameraGamepadInput.md#constructor)

### Properties

- [\_cameraTransform](FreeCameraGamepadInput.md#_cameratransform)
- [\_deltaTransform](FreeCameraGamepadInput.md#_deltatransform)
- [\_onGamepadConnectedObserver](FreeCameraGamepadInput.md#_ongamepadconnectedobserver)
- [\_onGamepadDisconnectedObserver](FreeCameraGamepadInput.md#_ongamepaddisconnectedobserver)
- [\_vector2](FreeCameraGamepadInput.md#_vector2)
- [\_vector3](FreeCameraGamepadInput.md#_vector3)
- [\_yAxisScale](FreeCameraGamepadInput.md#_yaxisscale)
- [camera](FreeCameraGamepadInput.md#camera)
- [deadzoneDelta](FreeCameraGamepadInput.md#deadzonedelta)
- [gamepad](FreeCameraGamepadInput.md#gamepad)
- [gamepadAngularSensibility](FreeCameraGamepadInput.md#gamepadangularsensibility)
- [gamepadMoveSensibility](FreeCameraGamepadInput.md#gamepadmovesensibility)

### Accessors

- [invertYAxis](FreeCameraGamepadInput.md#invertyaxis)

### Methods

- [attachControl](FreeCameraGamepadInput.md#attachcontrol)
- [checkInputs](FreeCameraGamepadInput.md#checkinputs)
- [detachControl](FreeCameraGamepadInput.md#detachcontrol)
- [getClassName](FreeCameraGamepadInput.md#getclassname)
- [getSimpleName](FreeCameraGamepadInput.md#getsimplename)

## Constructors

### constructor

• **new FreeCameraGamepadInput**()

## Properties

### \_cameraTransform

• `Private` **\_cameraTransform**: [`Matrix`](Matrix.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraGamepadInput.ts:61

___

### \_deltaTransform

• `Private` **\_deltaTransform**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraGamepadInput.ts:62

___

### \_onGamepadConnectedObserver

• `Private` **\_onGamepadConnectedObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Gamepad`](Gamepad.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraGamepadInput.ts:59

___

### \_onGamepadDisconnectedObserver

• `Private` **\_onGamepadDisconnectedObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Gamepad`](Gamepad.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraGamepadInput.ts:60

___

### \_vector2

• `Private` **\_vector2**: [`Vector2`](Vector2.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraGamepadInput.ts:64

___

### \_vector3

• `Private` **\_vector3**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraGamepadInput.ts:63

___

### \_yAxisScale

• `Private` **\_yAxisScale**: `number` = `1.0`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraGamepadInput.ts:45

___

### camera

• **camera**: [`FreeCamera`](FreeCamera.md)

Define the camera the input is attached to.

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[camera](../interfaces/ICameraInput.md#camera)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraGamepadInput.ts:18

___

### deadzoneDelta

• **deadzoneDelta**: `number` = `0.1`

Defines the minimum value at which any analog stick input is ignored.
Note: This value should only be a value between 0 and 1.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraGamepadInput.ts:43

___

### gamepad

• **gamepad**: [`Nullable`](../modules.md#nullable)[`Gamepad`](Gamepad.md)

Define the Gamepad controlling the input

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraGamepadInput.ts:23

___

### gamepadAngularSensibility

• **gamepadAngularSensibility**: `number` = `200`

Defines the gamepad rotation sensibility.
This is the threshold from when rotation starts to be accounted for to prevent jittering.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraGamepadInput.ts:30

___

### gamepadMoveSensibility

• **gamepadMoveSensibility**: `number` = `40`

Defines the gamepad move sensibility.
This is the threshold from when moving starts to be accounted for for to prevent jittering.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraGamepadInput.ts:37

## Accessors

### invertYAxis

• `get` **invertYAxis**(): `boolean`

Gets or sets a boolean indicating that Yaxis (for right stick) should be inverted

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraGamepadInput.ts:50

• `set` **invertYAxis**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraGamepadInput.ts:54

## Methods

### attachControl

▸ **attachControl**(): `void`

Attach the input controls to a specific dom element to get the input from.

#### Returns

`void`

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[attachControl](../interfaces/ICameraInput.md#attachcontrol)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraGamepadInput.ts:69

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

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraGamepadInput.ts:107

___

### detachControl

▸ **detachControl**(): `void`

Detach the current controls from the specified dom element.

#### Returns

`void`

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[detachControl](../interfaces/ICameraInput.md#detachcontrol)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraGamepadInput.ts:97

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

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraGamepadInput.ts:144

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

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraGamepadInput.ts:152
