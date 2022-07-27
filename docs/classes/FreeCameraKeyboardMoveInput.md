[@dev/core](../README.md) / [Exports](../modules.md) / FreeCameraKeyboardMoveInput

# Class: FreeCameraKeyboardMoveInput

Manage the keyboard inputs to control the movement of a free camera.

**`See`**

https://doc.babylonjs.com/how_to/customizing_camera_inputs

## Implements

- [`ICameraInput`](../interfaces/ICameraInput.md)[`FreeCamera`](FreeCamera.md)

## Table of contents

### Constructors

- [constructor](FreeCameraKeyboardMoveInput.md#constructor)

### Properties

- [\_engine](FreeCameraKeyboardMoveInput.md#_engine)
- [\_keys](FreeCameraKeyboardMoveInput.md#_keys)
- [\_onCanvasBlurObserver](FreeCameraKeyboardMoveInput.md#_oncanvasblurobserver)
- [\_onKeyboardObserver](FreeCameraKeyboardMoveInput.md#_onkeyboardobserver)
- [\_scene](FreeCameraKeyboardMoveInput.md#_scene)
- [camera](FreeCameraKeyboardMoveInput.md#camera)
- [keysDown](FreeCameraKeyboardMoveInput.md#keysdown)
- [keysDownward](FreeCameraKeyboardMoveInput.md#keysdownward)
- [keysLeft](FreeCameraKeyboardMoveInput.md#keysleft)
- [keysRight](FreeCameraKeyboardMoveInput.md#keysright)
- [keysRotateLeft](FreeCameraKeyboardMoveInput.md#keysrotateleft)
- [keysRotateRight](FreeCameraKeyboardMoveInput.md#keysrotateright)
- [keysUp](FreeCameraKeyboardMoveInput.md#keysup)
- [keysUpward](FreeCameraKeyboardMoveInput.md#keysupward)
- [rotationSpeed](FreeCameraKeyboardMoveInput.md#rotationspeed)

### Methods

- [\_getLocalRotation](FreeCameraKeyboardMoveInput.md#_getlocalrotation)
- [attachControl](FreeCameraKeyboardMoveInput.md#attachcontrol)
- [checkInputs](FreeCameraKeyboardMoveInput.md#checkinputs)
- [detachControl](FreeCameraKeyboardMoveInput.md#detachcontrol)
- [getClassName](FreeCameraKeyboardMoveInput.md#getclassname)
- [getSimpleName](FreeCameraKeyboardMoveInput.md#getsimplename)

## Constructors

### constructor

• **new FreeCameraKeyboardMoveInput**()

## Properties

### \_engine

• `Private` **\_engine**: [`Engine`](Engine.md)

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraKeyboardMoveInput.ts:80

___

### \_keys

• `Private` **\_keys**: `number`[]

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraKeyboardMoveInput.ts:77

___

### \_onCanvasBlurObserver

• `Private` **\_onCanvasBlurObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Engine`](Engine.md)

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraKeyboardMoveInput.ts:78

___

### \_onKeyboardObserver

• `Private` **\_onKeyboardObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`KeyboardInfo`](KeyboardInfo.md)

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraKeyboardMoveInput.ts:79

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraKeyboardMoveInput.ts:81

___

### camera

• **camera**: [`FreeCamera`](FreeCamera.md)

Defines the camera the input is attached to.

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[camera](../interfaces/ICameraInput.md#camera)

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraKeyboardMoveInput.ts:21

___

### keysDown

• **keysDown**: `number`[]

Gets or Set the list of keyboard keys used to control the backward move of the camera.

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraKeyboardMoveInput.ts:39

___

### keysDownward

• **keysDownward**: `number`[]

Gets or Set the list of keyboard keys used to control the downward move of the camera.

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraKeyboardMoveInput.ts:45

___

### keysLeft

• **keysLeft**: `number`[]

Gets or Set the list of keyboard keys used to control the left strafe move of the camera.

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraKeyboardMoveInput.ts:51

___

### keysRight

• **keysRight**: `number`[]

Gets or Set the list of keyboard keys used to control the right strafe move of the camera.

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraKeyboardMoveInput.ts:57

___

### keysRotateLeft

• **keysRotateLeft**: `number`[] = `[]`

Gets or Set the list of keyboard keys used to control the left rotation move of the camera.

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraKeyboardMoveInput.ts:69

___

### keysRotateRight

• **keysRotateRight**: `number`[] = `[]`

Gets or Set the list of keyboard keys used to control the right rotation move of the camera.

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraKeyboardMoveInput.ts:75

___

### keysUp

• **keysUp**: `number`[]

Gets or Set the list of keyboard keys used to control the forward move of the camera.

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraKeyboardMoveInput.ts:27

___

### keysUpward

• **keysUpward**: `number`[]

Gets or Set the list of keyboard keys used to control the upward move of the camera.

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraKeyboardMoveInput.ts:33

___

### rotationSpeed

• **rotationSpeed**: `number` = `0.5`

Defines the pointer angular sensibility  along the X and Y axis or how fast is the camera rotating.

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraKeyboardMoveInput.ts:63

## Methods

### \_getLocalRotation

▸ `Private` **_getLocalRotation**(): `number`

#### Returns

`number`

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraKeyboardMoveInput.ts:231

___

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

packages/dev/core/src/Cameras/Inputs/freeCameraKeyboardMoveInput.ts:87

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

packages/dev/core/src/Cameras/Inputs/freeCameraKeyboardMoveInput.ts:171

___

### detachControl

▸ **detachControl**(): `void`

Detach the current controls from the specified dom element.

#### Returns

`void`

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[detachControl](../interfaces/ICameraInput.md#detachcontrol)

#### Defined in

packages/dev/core/src/Cameras/Inputs/freeCameraKeyboardMoveInput.ts:152

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

packages/dev/core/src/Cameras/Inputs/freeCameraKeyboardMoveInput.ts:214

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

packages/dev/core/src/Cameras/Inputs/freeCameraKeyboardMoveInput.ts:227
