[@dev/core](../README.md) / [Exports](../modules.md) / ArcRotateCameraInputsManager

# Class: ArcRotateCameraInputsManager

Default Inputs manager for the ArcRotateCamera.
It groups all the default supported inputs for ease of use.

**`See`**

https://doc.babylonjs.com/how_to/customizing_camera_inputs

## Hierarchy

- [`CameraInputsManager`](CameraInputsManager.md)[`ArcRotateCamera`](ArcRotateCamera.md)

  ↳ **`ArcRotateCameraInputsManager`**

## Table of contents

### Constructors

- [constructor](ArcRotateCameraInputsManager.md#constructor)

### Properties

- [attached](ArcRotateCameraInputsManager.md#attached)
- [attachedToElement](ArcRotateCameraInputsManager.md#attachedtoelement)
- [camera](ArcRotateCameraInputsManager.md#camera)
- [checkInputs](ArcRotateCameraInputsManager.md#checkinputs)
- [noPreventDefault](ArcRotateCameraInputsManager.md#nopreventdefault)

### Methods

- [add](ArcRotateCameraInputsManager.md#add)
- [addGamepad](ArcRotateCameraInputsManager.md#addgamepad)
- [addKeyboard](ArcRotateCameraInputsManager.md#addkeyboard)
- [addMouseWheel](ArcRotateCameraInputsManager.md#addmousewheel)
- [addPointers](ArcRotateCameraInputsManager.md#addpointers)
- [addVRDeviceOrientation](ArcRotateCameraInputsManager.md#addvrdeviceorientation)
- [attachElement](ArcRotateCameraInputsManager.md#attachelement)
- [attachInput](ArcRotateCameraInputsManager.md#attachinput)
- [clear](ArcRotateCameraInputsManager.md#clear)
- [detachElement](ArcRotateCameraInputsManager.md#detachelement)
- [parse](ArcRotateCameraInputsManager.md#parse)
- [rebuildInputCheck](ArcRotateCameraInputsManager.md#rebuildinputcheck)
- [remove](ArcRotateCameraInputsManager.md#remove)
- [removeByType](ArcRotateCameraInputsManager.md#removebytype)
- [serialize](ArcRotateCameraInputsManager.md#serialize)

## Constructors

### constructor

• **new ArcRotateCameraInputsManager**(`camera`)

Instantiates a new ArcRotateCameraInputsManager.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `camera` | [`ArcRotateCamera`](ArcRotateCamera.md) | Defines the camera the inputs belong to |

#### Overrides

[CameraInputsManager](CameraInputsManager.md).[constructor](CameraInputsManager.md#constructor)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCameraInputsManager.ts:17

## Properties

### attached

• **attached**: [`CameraInputsMap`](../interfaces/CameraInputsMap.md)[`ArcRotateCamera`](ArcRotateCamera.md)

Defines the list of inputs attached to the camera.

#### Inherited from

[CameraInputsManager](CameraInputsManager.md).[attached](CameraInputsManager.md#attached)

#### Defined in

packages/dev/core/src/Cameras/cameraInputsManager.ts:71

___

### attachedToElement

• **attachedToElement**: `boolean` = `false`

Defines the dom element the camera is collecting inputs from.
This is null if the controls have not been attached.

#### Inherited from

[CameraInputsManager](CameraInputsManager.md).[attachedToElement](CameraInputsManager.md#attachedtoelement)

#### Defined in

packages/dev/core/src/Cameras/cameraInputsManager.ts:77

___

### camera

• **camera**: [`ArcRotateCamera`](ArcRotateCamera.md)

Defined the camera the input manager belongs to.

#### Inherited from

[CameraInputsManager](CameraInputsManager.md).[camera](CameraInputsManager.md#camera)

#### Defined in

packages/dev/core/src/Cameras/cameraInputsManager.ts:87

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

packages/dev/core/src/Cameras/cameraInputsManager.ts:93

___

### noPreventDefault

• **noPreventDefault**: `boolean`

Defines whether event caught by the controls should call preventdefault() (https://developer.mozilla.org/en-US/docs/Web/API/Event/preventDefault)

#### Inherited from

[CameraInputsManager](CameraInputsManager.md).[noPreventDefault](CameraInputsManager.md#nopreventdefault)

#### Defined in

packages/dev/core/src/Cameras/cameraInputsManager.ts:82

## Methods

### add

▸ **add**(`input`): `void`

Add an input method to a camera

**`See`**

https://doc.babylonjs.com/how_to/customizing_camera_inputs

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `input` | [`ICameraInput`](../interfaces/ICameraInput.md)[`ArcRotateCamera`](ArcRotateCamera.md) | camera input method |

#### Returns

`void`

#### Inherited from

[CameraInputsManager](CameraInputsManager.md).[add](CameraInputsManager.md#add)

#### Defined in

packages/dev/core/src/Cameras/cameraInputsManager.ts:110

___

### addGamepad

▸ **addGamepad**(): [`ArcRotateCameraInputsManager`](ArcRotateCameraInputsManager.md)

Adds gamepad input support to the ArcRotateCamera InputManager.

#### Returns

[`ArcRotateCameraInputsManager`](ArcRotateCameraInputsManager.md)

the camera inputs manager

#### Defined in

packages/dev/core/src/Gamepads/gamepadSceneComponent.ts:72

___

### addKeyboard

▸ **addKeyboard**(): [`ArcRotateCameraInputsManager`](ArcRotateCameraInputsManager.md)

Add keyboard input support to the input manager.

#### Returns

[`ArcRotateCameraInputsManager`](ArcRotateCameraInputsManager.md)

the current input manager

#### Defined in

packages/dev/core/src/Cameras/arcRotateCameraInputsManager.ts:43

___

### addMouseWheel

▸ **addMouseWheel**(): [`ArcRotateCameraInputsManager`](ArcRotateCameraInputsManager.md)

Add mouse wheel input support to the input manager.

#### Returns

[`ArcRotateCameraInputsManager`](ArcRotateCameraInputsManager.md)

the current input manager

#### Defined in

packages/dev/core/src/Cameras/arcRotateCameraInputsManager.ts:25

___

### addPointers

▸ **addPointers**(): [`ArcRotateCameraInputsManager`](ArcRotateCameraInputsManager.md)

Add pointers input support to the input manager.

#### Returns

[`ArcRotateCameraInputsManager`](ArcRotateCameraInputsManager.md)

the current input manager

#### Defined in

packages/dev/core/src/Cameras/arcRotateCameraInputsManager.ts:34

___

### addVRDeviceOrientation

▸ **addVRDeviceOrientation**(): [`ArcRotateCameraInputsManager`](ArcRotateCameraInputsManager.md)

Add orientation input support to the input manager.

#### Returns

[`ArcRotateCameraInputsManager`](ArcRotateCameraInputsManager.md)

the current input manager

#### Defined in

packages/dev/core/src/Cameras/Inputs/arcRotateCameraVRDeviceOrientationInput.ts:14

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

packages/dev/core/src/Cameras/cameraInputsManager.ts:188

___

### attachInput

▸ **attachInput**(`input`): `void`

Attach the input controls to the currently attached dom element to listen the events from.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `input` | [`ICameraInput`](../interfaces/ICameraInput.md)[`ArcRotateCamera`](ArcRotateCamera.md) | Defines the input to attach |

#### Returns

`void`

#### Inherited from

[CameraInputsManager](CameraInputsManager.md).[attachInput](CameraInputsManager.md#attachinput)

#### Defined in

packages/dev/core/src/Cameras/cameraInputsManager.ts:178

___

### clear

▸ **clear**(): `void`

Remove all attached input methods from a camera

#### Returns

`void`

#### Inherited from

[CameraInputsManager](CameraInputsManager.md).[clear](CameraInputsManager.md#clear)

#### Defined in

packages/dev/core/src/Cameras/cameraInputsManager.ts:235

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

packages/dev/core/src/Cameras/cameraInputsManager.ts:206

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

packages/dev/core/src/Cameras/cameraInputsManager.ts:266

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

packages/dev/core/src/Cameras/cameraInputsManager.ts:221

___

### remove

▸ **remove**(`inputToRemove`): `void`

Remove a specific input method from a camera
example: camera.inputs.remove(camera.inputs.attached.mouse);

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `inputToRemove` | [`ICameraInput`](../interfaces/ICameraInput.md)[`ArcRotateCamera`](ArcRotateCamera.md) | camera input method |

#### Returns

`void`

#### Inherited from

[CameraInputsManager](CameraInputsManager.md).[remove](CameraInputsManager.md#remove)

#### Defined in

packages/dev/core/src/Cameras/cameraInputsManager.ts:137

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

packages/dev/core/src/Cameras/cameraInputsManager.ts:154

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

packages/dev/core/src/Cameras/cameraInputsManager.ts:250
