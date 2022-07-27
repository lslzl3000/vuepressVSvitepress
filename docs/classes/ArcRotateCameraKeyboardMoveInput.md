[@dev/core](../README.md) / [Exports](../modules.md) / ArcRotateCameraKeyboardMoveInput

# Class: ArcRotateCameraKeyboardMoveInput

Manage the keyboard inputs to control the movement of an arc rotate camera.

**`See`**

https://doc.babylonjs.com/how_to/customizing_camera_inputs

## Implements

- [`ICameraInput`](../interfaces/ICameraInput.md)[`ArcRotateCamera`](ArcRotateCamera.md)

## Table of contents

### Constructors

- [constructor](ArcRotateCameraKeyboardMoveInput.md#constructor)

### Properties

- [\_altPressed](ArcRotateCameraKeyboardMoveInput.md#_altpressed)
- [\_ctrlPressed](ArcRotateCameraKeyboardMoveInput.md#_ctrlpressed)
- [\_engine](ArcRotateCameraKeyboardMoveInput.md#_engine)
- [\_keys](ArcRotateCameraKeyboardMoveInput.md#_keys)
- [\_onCanvasBlurObserver](ArcRotateCameraKeyboardMoveInput.md#_oncanvasblurobserver)
- [\_onKeyboardObserver](ArcRotateCameraKeyboardMoveInput.md#_onkeyboardobserver)
- [\_scene](ArcRotateCameraKeyboardMoveInput.md#_scene)
- [angularSpeed](ArcRotateCameraKeyboardMoveInput.md#angularspeed)
- [camera](ArcRotateCameraKeyboardMoveInput.md#camera)
- [keysDown](ArcRotateCameraKeyboardMoveInput.md#keysdown)
- [keysLeft](ArcRotateCameraKeyboardMoveInput.md#keysleft)
- [keysReset](ArcRotateCameraKeyboardMoveInput.md#keysreset)
- [keysRight](ArcRotateCameraKeyboardMoveInput.md#keysright)
- [keysUp](ArcRotateCameraKeyboardMoveInput.md#keysup)
- [panningSensibility](ArcRotateCameraKeyboardMoveInput.md#panningsensibility)
- [useAltToZoom](ArcRotateCameraKeyboardMoveInput.md#usealttozoom)
- [zoomingSensibility](ArcRotateCameraKeyboardMoveInput.md#zoomingsensibility)

### Methods

- [attachControl](ArcRotateCameraKeyboardMoveInput.md#attachcontrol)
- [checkInputs](ArcRotateCameraKeyboardMoveInput.md#checkinputs)
- [detachControl](ArcRotateCameraKeyboardMoveInput.md#detachcontrol)
- [getClassName](ArcRotateCameraKeyboardMoveInput.md#getclassname)
- [getSimpleName](ArcRotateCameraKeyboardMoveInput.md#getsimplename)

## Constructors

### constructor

• **new ArcRotateCameraKeyboardMoveInput**()

## Properties

### \_altPressed

• `Private` **\_altPressed**: `boolean`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraKeyboardMoveInput.ts:83

___

### \_ctrlPressed

• `Private` **\_ctrlPressed**: `boolean`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraKeyboardMoveInput.ts:82

___

### \_engine

• `Private` **\_engine**: [`Engine`](Engine.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraKeyboardMoveInput.ts:86

___

### \_keys

• `Private` **\_keys**: `number`[]

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraKeyboardMoveInput.ts:81

___

### \_onCanvasBlurObserver

• `Private` **\_onCanvasBlurObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Engine`](Engine.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraKeyboardMoveInput.ts:84

___

### \_onKeyboardObserver

• `Private` **\_onKeyboardObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`KeyboardInfo`](KeyboardInfo.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraKeyboardMoveInput.ts:85

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraKeyboardMoveInput.ts:87

___

### angularSpeed

• **angularSpeed**: `number` = `0.01`

Rotation speed of the camera

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraKeyboardMoveInput.ts:79

___

### camera

• **camera**: [`ArcRotateCamera`](ArcRotateCamera.md)

Defines the camera the input is attached to.

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[camera](../interfaces/ICameraInput.md#camera)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraKeyboardMoveInput.ts:21

___

### keysDown

• **keysDown**: `number`[]

Defines the list of key codes associated with the down action (decrease alpha)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraKeyboardMoveInput.ts:33

___

### keysLeft

• **keysLeft**: `number`[]

Defines the list of key codes associated with the left action (increase beta)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraKeyboardMoveInput.ts:39

___

### keysReset

• **keysReset**: `number`[]

Defines the list of key codes associated with the reset action.
Those keys reset the camera to its last stored state (with the method camera.storeState())

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraKeyboardMoveInput.ts:52

___

### keysRight

• **keysRight**: `number`[]

Defines the list of key codes associated with the right action (decrease beta)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraKeyboardMoveInput.ts:45

___

### keysUp

• **keysUp**: `number`[]

Defines the list of key codes associated with the up action (increase alpha)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraKeyboardMoveInput.ts:27

___

### panningSensibility

• **panningSensibility**: `number` = `50.0`

Defines the panning sensibility of the inputs.
(How fast is the camera panning)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraKeyboardMoveInput.ts:59

___

### useAltToZoom

• **useAltToZoom**: `boolean` = `true`

Defines whether maintaining the alt key down switch the movement mode from
orientation to zoom.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraKeyboardMoveInput.ts:73

___

### zoomingSensibility

• **zoomingSensibility**: `number` = `25.0`

Defines the zooming sensibility of the inputs.
(How fast is the camera zooming)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraKeyboardMoveInput.ts:66

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

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraKeyboardMoveInput.ts:93

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

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraKeyboardMoveInput.ts:182

___

### detachControl

▸ **detachControl**(): `void`

Detach the current controls from the specified dom element.

#### Returns

`void`

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[detachControl](../interfaces/ICameraInput.md#detachcontrol)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraKeyboardMoveInput.ts:163

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

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraKeyboardMoveInput.ts:229

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

https://github.com/babylon.js/core/src/Cameras/Inputs/arcRotateCameraKeyboardMoveInput.ts:237
