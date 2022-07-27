[@dev/core](../README.md) / [Exports](../modules.md) / FlyCameraKeyboardInput

# Class: FlyCameraKeyboardInput

Listen to keyboard events to control the camera.

**`See`**

https://doc.babylonjs.com/how_to/customizing_camera_inputs

## Implements

- [`ICameraInput`](../interfaces/ICameraInput.md)[`FlyCamera`](FlyCamera.md)

## Table of contents

### Constructors

- [constructor](FlyCameraKeyboardInput.md#constructor)

### Properties

- [\_engine](FlyCameraKeyboardInput.md#_engine)
- [\_keys](FlyCameraKeyboardInput.md#_keys)
- [\_onCanvasBlurObserver](FlyCameraKeyboardInput.md#_oncanvasblurobserver)
- [\_onKeyboardObserver](FlyCameraKeyboardInput.md#_onkeyboardobserver)
- [\_scene](FlyCameraKeyboardInput.md#_scene)
- [camera](FlyCameraKeyboardInput.md#camera)
- [keysBackward](FlyCameraKeyboardInput.md#keysbackward)
- [keysDown](FlyCameraKeyboardInput.md#keysdown)
- [keysForward](FlyCameraKeyboardInput.md#keysforward)
- [keysLeft](FlyCameraKeyboardInput.md#keysleft)
- [keysRight](FlyCameraKeyboardInput.md#keysright)
- [keysUp](FlyCameraKeyboardInput.md#keysup)

### Methods

- [attachControl](FlyCameraKeyboardInput.md#attachcontrol)
- [checkInputs](FlyCameraKeyboardInput.md#checkinputs)
- [detachControl](FlyCameraKeyboardInput.md#detachcontrol)
- [getClassName](FlyCameraKeyboardInput.md#getclassname)
- [getSimpleName](FlyCameraKeyboardInput.md#getsimplename)

## Constructors

### constructor

• **new FlyCameraKeyboardInput**()

## Properties

### \_engine

• `Private` **\_engine**: [`Engine`](Engine.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/flyCameraKeyboardInput.ts:63

___

### \_keys

• `Private` **\_keys**: `number`[]

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/flyCameraKeyboardInput.ts:60

___

### \_onCanvasBlurObserver

• `Private` **\_onCanvasBlurObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Engine`](Engine.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/flyCameraKeyboardInput.ts:61

___

### \_onKeyboardObserver

• `Private` **\_onKeyboardObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`KeyboardInfo`](KeyboardInfo.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/flyCameraKeyboardInput.ts:62

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/flyCameraKeyboardInput.ts:64

___

### camera

• **camera**: [`FlyCamera`](FlyCamera.md)

Defines the camera the input is attached to.

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[camera](../interfaces/ICameraInput.md#camera)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/flyCameraKeyboardInput.ts:22

___

### keysBackward

• **keysBackward**: `number`[]

The list of keyboard keys used to control the backward move of the camera.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/flyCameraKeyboardInput.ts:34

___

### keysDown

• **keysDown**: `number`[]

The list of keyboard keys used to control the backward move of the camera.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/flyCameraKeyboardInput.ts:46

___

### keysForward

• **keysForward**: `number`[]

The list of keyboard keys used to control the forward move of the camera.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/flyCameraKeyboardInput.ts:28

___

### keysLeft

• **keysLeft**: `number`[]

The list of keyboard keys used to control the left strafe move of the camera.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/flyCameraKeyboardInput.ts:58

___

### keysRight

• **keysRight**: `number`[]

The list of keyboard keys used to control the right strafe move of the camera.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/flyCameraKeyboardInput.ts:52

___

### keysUp

• **keysUp**: `number`[]

The list of keyboard keys used to control the forward move of the camera.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/flyCameraKeyboardInput.ts:40

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

https://github.com/babylon.js/core/src/Cameras/Inputs/flyCameraKeyboardInput.ts:70

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

https://github.com/babylon.js/core/src/Cameras/Inputs/flyCameraKeyboardInput.ts:172

___

### detachControl

▸ **detachControl**(): `void`

Detach the current controls from the specified dom element.

#### Returns

`void`

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[detachControl](../interfaces/ICameraInput.md#detachcontrol)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/flyCameraKeyboardInput.ts:130

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

https://github.com/babylon.js/core/src/Cameras/Inputs/flyCameraKeyboardInput.ts:149

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

https://github.com/babylon.js/core/src/Cameras/Inputs/flyCameraKeyboardInput.ts:164
