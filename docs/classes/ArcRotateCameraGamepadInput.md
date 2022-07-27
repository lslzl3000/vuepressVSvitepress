[@dev/core](../README.md) / [Exports](../modules.md) / ArcRotateCameraGamepadInput

# Class: ArcRotateCameraGamepadInput

Manage the gamepad inputs to control an arc rotate camera.

**`See`**

https://doc.babylonjs.com/how_to/customizing_camera_inputs

## Implements

- [`ICameraInput`](../interfaces/ICameraInput.md)[`ArcRotateCamera`](ArcRotateCamera.md)

## Table of contents

### Constructors

- [constructor](ArcRotateCameraGamepadInput.md#constructor)

### Properties

- [\_onGamepadConnectedObserver](ArcRotateCameraGamepadInput.md#_ongamepadconnectedobserver)
- [\_onGamepadDisconnectedObserver](ArcRotateCameraGamepadInput.md#_ongamepaddisconnectedobserver)
- [\_yAxisScale](ArcRotateCameraGamepadInput.md#_yaxisscale)
- [camera](ArcRotateCameraGamepadInput.md#camera)
- [gamepad](ArcRotateCameraGamepadInput.md#gamepad)
- [gamepadMoveSensibility](ArcRotateCameraGamepadInput.md#gamepadmovesensibility)
- [gamepadRotationSensibility](ArcRotateCameraGamepadInput.md#gamepadrotationsensibility)

### Accessors

- [invertYAxis](ArcRotateCameraGamepadInput.md#invertyaxis)

### Methods

- [attachControl](ArcRotateCameraGamepadInput.md#attachcontrol)
- [checkInputs](ArcRotateCameraGamepadInput.md#checkinputs)
- [detachControl](ArcRotateCameraGamepadInput.md#detachcontrol)
- [getClassName](ArcRotateCameraGamepadInput.md#getclassname)
- [getSimpleName](ArcRotateCameraGamepadInput.md#getsimplename)

## Constructors

### constructor

• **new ArcRotateCameraGamepadInput**()

## Properties

### \_onGamepadConnectedObserver

• `Private` **\_onGamepadConnectedObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Gamepad`](Gamepad.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraGamepadInput.ts:50

___

### \_onGamepadDisconnectedObserver

• `Private` **\_onGamepadDisconnectedObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Gamepad`](Gamepad.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraGamepadInput.ts:51

___

### \_yAxisScale

• `Private` **\_yAxisScale**: `number` = `1.0`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraGamepadInput.ts:37

___

### camera

• **camera**: [`ArcRotateCamera`](ArcRotateCamera.md)

Defines the camera the input is attached to.

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[camera](../interfaces/ICameraInput.md#camera)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraGamepadInput.ts:16

___

### gamepad

• **gamepad**: [`Nullable`](../modules.md#nullable)[`Gamepad`](Gamepad.md)

Defines the gamepad the input is gathering event from.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraGamepadInput.ts:21

___

### gamepadMoveSensibility

• **gamepadMoveSensibility**: `number` = `40`

Defines the gamepad move sensibility.
This is the threshold from when moving starts to be accounted for for to prevent jittering.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraGamepadInput.ts:35

___

### gamepadRotationSensibility

• **gamepadRotationSensibility**: `number` = `80`

Defines the gamepad rotation sensibility.
This is the threshold from when rotation starts to be accounted for to prevent jittering.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraGamepadInput.ts:28

## Accessors

### invertYAxis

• `get` **invertYAxis**(): `boolean`

Gets or sets a boolean indicating that Yaxis (for right stick) should be inverted

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraGamepadInput.ts:42

• `set` **invertYAxis**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraGamepadInput.ts:46

## Methods

### attachControl

▸ **attachControl**(): `void`

Attach the input controls to a specific dom element to get the input from.

#### Returns

`void`

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[attachControl](../interfaces/ICameraInput.md#attachcontrol)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraGamepadInput.ts:56

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

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraGamepadInput.ts:89

___

### detachControl

▸ **detachControl**(): `void`

Detach the current controls from the specified dom element.

#### Returns

`void`

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[detachControl](../interfaces/ICameraInput.md#detachcontrol)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraGamepadInput.ts:79

___

### getClassName

▸ **getClassName**(): `string`

Gets the class name of the current intput.

#### Returns

`string`

the class name

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[getClassName](../interfaces/ICameraInput.md#getclassname)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraGamepadInput.ts:124

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

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraGamepadInput.ts:132
