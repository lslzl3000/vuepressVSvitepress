[@dev/core](../README.md) / [Exports](../modules.md) / FreeCameraInputsManager

# Class: FreeCameraInputsManager

Default Inputs manager for the FreeCamera.
It groups all the default supported inputs for ease of use.

**`See`**

https://doc.babylonjs.com/how_to/customizing_camera_inputs

## Hierarchy

- [`CameraInputsManager`](CameraInputsManager.md)[`FreeCamera`](FreeCamera.md)

  ↳ **`FreeCameraInputsManager`**

## Table of contents

### Constructors

- [constructor](FreeCameraInputsManager.md#constructor)

### Properties

- [attached](FreeCameraInputsManager.md#attached)
- [attachedToElement](FreeCameraInputsManager.md#attachedtoelement)
- [camera](FreeCameraInputsManager.md#camera)
- [checkInputs](FreeCameraInputsManager.md#checkinputs)
- [noPreventDefault](FreeCameraInputsManager.md#nopreventdefault)

### Methods

- [add](FreeCameraInputsManager.md#add)
- [addDeviceOrientation](FreeCameraInputsManager.md#adddeviceorientation)
- [addGamepad](FreeCameraInputsManager.md#addgamepad)
- [addKeyboard](FreeCameraInputsManager.md#addkeyboard)
- [addMouse](FreeCameraInputsManager.md#addmouse)
- [addMouseWheel](FreeCameraInputsManager.md#addmousewheel)
- [addTouch](FreeCameraInputsManager.md#addtouch)
- [addVirtualJoystick](FreeCameraInputsManager.md#addvirtualjoystick)
- [attachElement](FreeCameraInputsManager.md#attachelement)
- [attachInput](FreeCameraInputsManager.md#attachinput)
- [clear](FreeCameraInputsManager.md#clear)
- [detachElement](FreeCameraInputsManager.md#detachelement)
- [parse](FreeCameraInputsManager.md#parse)
- [rebuildInputCheck](FreeCameraInputsManager.md#rebuildinputcheck)
- [remove](FreeCameraInputsManager.md#remove)
- [removeByType](FreeCameraInputsManager.md#removebytype)
- [removeMouse](FreeCameraInputsManager.md#removemouse)
- [removeMouseWheel](FreeCameraInputsManager.md#removemousewheel)
- [serialize](FreeCameraInputsManager.md#serialize)

## Constructors

### constructor

• **new FreeCameraInputsManager**(`camera`)

Instantiates a new FreeCameraInputsManager.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `camera` | [`FreeCamera`](FreeCamera.md) | Defines the camera the inputs belong to |

#### Overrides

[CameraInputsManager](CameraInputsManager.md).[constructor](CameraInputsManager.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/freeCameraInputsManager.ts:27

## Properties

### attached

• **attached**: [`CameraInputsMap`](../interfaces/CameraInputsMap.md)[`FreeCamera`](FreeCamera.md)

Defines the list of inputs attached to the camera.

#### Inherited from

[CameraInputsManager](CameraInputsManager.md).[attached](CameraInputsManager.md#attached)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/cameraInputsManager.ts:71

___

### attachedToElement

• **attachedToElement**: `boolean` = `false`

Defines the dom element the camera is collecting inputs from.
This is null if the controls have not been attached.

#### Inherited from

[CameraInputsManager](CameraInputsManager.md).[attachedToElement](CameraInputsManager.md#attachedtoelement)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/cameraInputsManager.ts:77

___

### camera

• **camera**: [`FreeCamera`](FreeCamera.md)

Defined the camera the input manager belongs to.

#### Inherited from

[CameraInputsManager](CameraInputsManager.md).[camera](CameraInputsManager.md#camera)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/cameraInputsManager.ts:87

___

### checkInputs

• **checkInputs**: () => `void`

#### Type declaration

▸ (): `void`

Update the current camera state depending on the inputs that have been used this frame.
This is a dynamically created lambda to avoid the performance penalty of looping for inputs in the render loop.

##### Returns

`void`

#### Inherited from

[CameraInputsManager](CameraInputsManager.md).[checkInputs](CameraInputsManager.md#checkinputs)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/cameraInputsManager.ts:93

___

### noPreventDefault

• **noPreventDefault**: `boolean`

Defines whether event caught by the controls should call preventdefault() (https://developer.mozilla.org/en-US/docs/Web/API/Event/preventDefault)

#### Inherited from

[CameraInputsManager](CameraInputsManager.md).[noPreventDefault](CameraInputsManager.md#nopreventdefault)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/cameraInputsManager.ts:82

## Methods

### add

▸ **add**(`input`): `void`

Add an input method to a camera

**`See`**

https://doc.babylonjs.com/how_to/customizing_camera_inputs

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `input` | [`ICameraInput`](../interfaces/ICameraInput.md)[`FreeCamera`](FreeCamera.md) | camera input method |

#### Returns

`void`

#### Inherited from

[CameraInputsManager](CameraInputsManager.md).[add](CameraInputsManager.md#add)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/cameraInputsManager.ts:110

___

### addDeviceOrientation

▸ **addDeviceOrientation**(): [`FreeCameraInputsManager`](FreeCameraInputsManager.md)

Add orientation input support to the input manager.

#### Returns

[`FreeCameraInputsManager`](FreeCameraInputsManager.md)

the current input manager

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraDeviceOrientationInput.ts:21

___

### addGamepad

▸ **addGamepad**(): [`FreeCameraInputsManager`](FreeCameraInputsManager.md)

Adds gamepad input support to the FreeCameraInputsManager.

#### Returns

[`FreeCameraInputsManager`](FreeCameraInputsManager.md)

the FreeCameraInputsManager

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepadSceneComponent.ts:51

___

### addKeyboard

▸ **addKeyboard**(): [`FreeCameraInputsManager`](FreeCameraInputsManager.md)

Add keyboard input support to the input manager.

#### Returns

[`FreeCameraInputsManager`](FreeCameraInputsManager.md)

the current input manager

#### Defined in

https://github.com/babylon.js/core/src/Cameras/freeCameraInputsManager.ts:35

___

### addMouse

▸ **addMouse**(`touchEnabled?`): [`FreeCameraInputsManager`](FreeCameraInputsManager.md)

Add mouse input support to the input manager.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `touchEnabled` | `boolean` | `true` | if the FreeCameraMouseInput should support touch (default: true) |

#### Returns

[`FreeCameraInputsManager`](FreeCameraInputsManager.md)

the current input manager

#### Defined in

https://github.com/babylon.js/core/src/Cameras/freeCameraInputsManager.ts:45

___

### addMouseWheel

▸ **addMouseWheel**(): [`FreeCameraInputsManager`](FreeCameraInputsManager.md)

Add mouse wheel input support to the input manager.

#### Returns

[`FreeCameraInputsManager`](FreeCameraInputsManager.md)

the current input manager

#### Defined in

https://github.com/babylon.js/core/src/Cameras/freeCameraInputsManager.ts:68

___

### addTouch

▸ **addTouch**(): [`FreeCameraInputsManager`](FreeCameraInputsManager.md)

Add touch input support to the input manager.

#### Returns

[`FreeCameraInputsManager`](FreeCameraInputsManager.md)

the current input manager

#### Defined in

https://github.com/babylon.js/core/src/Cameras/freeCameraInputsManager.ts:91

___

### addVirtualJoystick

▸ **addVirtualJoystick**(): [`FreeCameraInputsManager`](FreeCameraInputsManager.md)

Add virtual joystick input support to the input manager.

#### Returns

[`FreeCameraInputsManager`](FreeCameraInputsManager.md)

the current input manager

#### Defined in

https://github.com/babylon.js/core/src/Cameras/Inputs/freeCameraVirtualJoystickInput.ts:15

___

### attachElement

▸ **attachElement**(`noPreventDefault?`): `void`

Attach the current manager inputs controls to a specific dom element to listen the events from.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `noPreventDefault` | `boolean` | `false` | Defines whether event caught by the controls should call preventdefault() (https://developer.mozilla.org/en-US/docs/Web/API/Event/preventDefault) |

#### Returns

`void`

#### Inherited from

[CameraInputsManager](CameraInputsManager.md).[attachElement](CameraInputsManager.md#attachelement)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/cameraInputsManager.ts:188

___

### attachInput

▸ **attachInput**(`input`): `void`

Attach the input controls to the currently attached dom element to listen the events from.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `input` | [`ICameraInput`](../interfaces/ICameraInput.md)[`FreeCamera`](FreeCamera.md) | Defines the input to attach |

#### Returns

`void`

#### Inherited from

[CameraInputsManager](CameraInputsManager.md).[attachInput](CameraInputsManager.md#attachinput)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/cameraInputsManager.ts:178

___

### clear

▸ **clear**(): `void`

Remove all attached input methods from a camera

#### Returns

`void`

#### Overrides

[CameraInputsManager](CameraInputsManager.md).[clear](CameraInputsManager.md#clear)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/freeCameraInputsManager.ts:99

___

### detachElement

▸ **detachElement**(`disconnect?`): `void`

Detach the current manager inputs controls from a specific dom element.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `disconnect` | `boolean` | `false` | Defines whether the input should be removed from the current list of attached inputs |

#### Returns

`void`

#### Inherited from

[CameraInputsManager](CameraInputsManager.md).[detachElement](CameraInputsManager.md#detachelement)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/cameraInputsManager.ts:206

___

### parse

▸ **parse**(`parsedCamera`): `void`

Parses an input manager serialized JSON to restore the previous list of inputs
and states associated to a camera.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `parsedCamera` | `any` | Defines the JSON to parse |

#### Returns

`void`

#### Inherited from

[CameraInputsManager](CameraInputsManager.md).[parse](CameraInputsManager.md#parse)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/cameraInputsManager.ts:266

___

### rebuildInputCheck

▸ **rebuildInputCheck**(): `void`

Rebuild the dynamic inputCheck function from the current list of
defined inputs in the manager.

#### Returns

`void`

#### Inherited from

[CameraInputsManager](CameraInputsManager.md).[rebuildInputCheck](CameraInputsManager.md#rebuildinputcheck)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/cameraInputsManager.ts:221

___

### remove

▸ **remove**(`inputToRemove`): `void`

Remove a specific input method from a camera
example: camera.inputs.remove(camera.inputs.attached.mouse);

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `inputToRemove` | [`ICameraInput`](../interfaces/ICameraInput.md)[`FreeCamera`](FreeCamera.md) | camera input method |

#### Returns

`void`

#### Inherited from

[CameraInputsManager](CameraInputsManager.md).[remove](CameraInputsManager.md#remove)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/cameraInputsManager.ts:137

___

### removeByType

▸ **removeByType**(`inputType`): `void`

Remove a specific input type from a camera
example: camera.inputs.remove("ArcRotateCameraGamepadInput");

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `inputType` | `string` | the type of the input to remove |

#### Returns

`void`

#### Inherited from

[CameraInputsManager](CameraInputsManager.md).[removeByType](CameraInputsManager.md#removebytype)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/cameraInputsManager.ts:154

___

### removeMouse

▸ **removeMouse**(): [`FreeCameraInputsManager`](FreeCameraInputsManager.md)

Removes the mouse input support from the manager

#### Returns

[`FreeCameraInputsManager`](FreeCameraInputsManager.md)

the current input manager

#### Defined in

https://github.com/babylon.js/core/src/Cameras/freeCameraInputsManager.ts:57

___

### removeMouseWheel

▸ **removeMouseWheel**(): [`FreeCameraInputsManager`](FreeCameraInputsManager.md)

Removes the mouse wheel input support from the manager

#### Returns

[`FreeCameraInputsManager`](FreeCameraInputsManager.md)

the current input manager

#### Defined in

https://github.com/babylon.js/core/src/Cameras/freeCameraInputsManager.ts:80

___

### serialize

▸ **serialize**(`serializedCamera`): `void`

Serialize the current input manager attached to a camera.
This ensures than once parsed,
the input associated to the camera will be identical to the current ones

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `serializedCamera` | `any` | Defines the camera serialization JSON the input serialization should write to |

#### Returns

`void`

#### Inherited from

[CameraInputsManager](CameraInputsManager.md).[serialize](CameraInputsManager.md#serialize)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/cameraInputsManager.ts:250
