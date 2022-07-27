[@dev/core](../README.md) / [Exports](../modules.md) / FreeCameraTouchInput

# Class: FreeCameraTouchInput

Manage the touch inputs to control the movement of a free camera.

**`See`**

https://doc.babylonjs.com/how_to/customizing_camera_inputs

## Implements

- [`ICameraInput`](../interfaces/ICameraInput.md)[`FreeCamera`](FreeCamera.md)

## Table of contents

### Constructors

- [constructor](FreeCameraTouchInput.md#constructor)

### Properties

- [\_isSafari](FreeCameraTouchInput.md#_issafari)
- [\_observer](FreeCameraTouchInput.md#_observer)
- [\_offsetX](FreeCameraTouchInput.md#_offsetx)
- [\_offsetY](FreeCameraTouchInput.md#_offsety)
- [\_onLostFocus](FreeCameraTouchInput.md#_onlostfocus)
- [\_pointerInput](FreeCameraTouchInput.md#_pointerinput)
- [\_pointerPressed](FreeCameraTouchInput.md#_pointerpressed)
- [allowMouse](FreeCameraTouchInput.md#allowmouse)
- [camera](FreeCameraTouchInput.md#camera)
- [singleFingerRotate](FreeCameraTouchInput.md#singlefingerrotate)
- [touchAngularSensibility](FreeCameraTouchInput.md#touchangularsensibility)
- [touchMoveSensibility](FreeCameraTouchInput.md#touchmovesensibility)

### Methods

- [attachControl](FreeCameraTouchInput.md#attachcontrol)
- [checkInputs](FreeCameraTouchInput.md#checkinputs)
- [detachControl](FreeCameraTouchInput.md#detachcontrol)
- [getClassName](FreeCameraTouchInput.md#getclassname)
- [getSimpleName](FreeCameraTouchInput.md#getsimplename)

## Constructors

### constructor

• **new FreeCameraTouchInput**(`allowMouse?`)

Manage the touch inputs to control the movement of a free camera.

**`See`**

https://doc.babylonjs.com/how_to/customizing_camera_inputs

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `allowMouse` | `boolean` | `false` | Defines if mouse events can be treated as touch events |

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraTouchInput.ts:55

## Properties

### \_isSafari

• `Private` **\_isSafari**: `boolean`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraTouchInput.ts:48

___

### \_observer

• `Private` **\_observer**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`PointerInfo`](PointerInfo.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraTouchInput.ts:46

___

### \_offsetX

• `Private` **\_offsetX**: [`Nullable`](../modules.md#nullable)`number` = `null`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraTouchInput.ts:41

___

### \_offsetY

• `Private` **\_offsetY**: [`Nullable`](../modules.md#nullable)`number` = `null`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraTouchInput.ts:42

___

### \_onLostFocus

• `Private` **\_onLostFocus**: [`Nullable`](../modules.md#nullable)(`e`: `FocusEvent`) => `any`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraTouchInput.ts:47

___

### \_pointerInput

• `Private` `Optional` **\_pointerInput**: (`p`: [`PointerInfo`](PointerInfo.md), `s`: [`EventState`](EventState.md)) => `void`

#### Type declaration

▸ (`p`, `s`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `p` | [`PointerInfo`](PointerInfo.md) |
| `s` | [`EventState`](EventState.md) |

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraTouchInput.ts:45

___

### \_pointerPressed

• `Private` **\_pointerPressed**: `number`[]

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraTouchInput.ts:44

___

### allowMouse

• **allowMouse**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraTouchInput.ts:59

___

### camera

• **camera**: [`FreeCamera`](FreeCamera.md)

Defines the camera the input is attached to.

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[camera](../interfaces/ICameraInput.md#camera)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraTouchInput.ts:20

___

### singleFingerRotate

• **singleFingerRotate**: `boolean` = `false`

Swap touch actions so that one touch is used for rotation and multiple for movement

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraTouchInput.ts:39

___

### touchAngularSensibility

• **touchAngularSensibility**: `number` = `200000.0`

Defines the touch sensibility for rotation.
The lower the faster.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraTouchInput.ts:27

___

### touchMoveSensibility

• **touchMoveSensibility**: `number` = `250.0`

Defines the touch sensibility for move.
The lower the faster.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraTouchInput.ts:34

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

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraTouchInput.ts:68

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

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraTouchInput.ts:179

___

### detachControl

▸ **detachControl**(): `void`

Detach the current controls from the specified dom element.

#### Returns

`void`

#### Implementation of

[ICameraInput](../interfaces/ICameraInput.md).[detachControl](../interfaces/ICameraInput.md#detachcontrol)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraTouchInput.ts:156

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

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraTouchInput.ts:207

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

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraTouchInput.ts:215
