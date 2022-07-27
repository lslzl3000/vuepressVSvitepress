[@dev/core](../README.md) / [Exports](../modules.md) / FollowCameraInputsManager

# Class: FollowCameraInputsManager

Default Inputs manager for the FollowCamera.
It groups all the default supported inputs for ease of use.

**`See`**

https://doc.babylonjs.com/how_to/customizing_camera_inputs

## Hierarchy

- [`CameraInputsManager`](CameraInputsManager.md)[`FollowCamera`](FollowCamera.md)

  ↳ **`FollowCameraInputsManager`**

## Table of contents

### Constructors

- [constructor](FollowCameraInputsManager.md#constructor)

### Properties

- [attached](FollowCameraInputsManager.md#attached)
- [attachedToElement](FollowCameraInputsManager.md#attachedtoelement)
- [camera](FollowCameraInputsManager.md#camera)
- [checkInputs](FollowCameraInputsManager.md#checkinputs)
- [noPreventDefault](FollowCameraInputsManager.md#nopreventdefault)

### Methods

- [add](FollowCameraInputsManager.md#add)
- [addKeyboard](FollowCameraInputsManager.md#addkeyboard)
- [addMouseWheel](FollowCameraInputsManager.md#addmousewheel)
- [addPointers](FollowCameraInputsManager.md#addpointers)
- [addVRDeviceOrientation](FollowCameraInputsManager.md#addvrdeviceorientation)
- [attachElement](FollowCameraInputsManager.md#attachelement)
- [attachInput](FollowCameraInputsManager.md#attachinput)
- [clear](FollowCameraInputsManager.md#clear)
- [detachElement](FollowCameraInputsManager.md#detachelement)
- [parse](FollowCameraInputsManager.md#parse)
- [rebuildInputCheck](FollowCameraInputsManager.md#rebuildinputcheck)
- [remove](FollowCameraInputsManager.md#remove)
- [removeByType](FollowCameraInputsManager.md#removebytype)
- [serialize](FollowCameraInputsManager.md#serialize)

## Constructors

### constructor

• **new FollowCameraInputsManager**(`camera`)

Instantiates a new FollowCameraInputsManager.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `camera` | [`FollowCamera`](FollowCamera.md) | Defines the camera the inputs belong to |

#### Overrides

[CameraInputsManager](CameraInputsManager.md).[constructor](CameraInputsManager.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/followCameraInputsManager.ts:17

## Properties

### attached

• **attached**: [`CameraInputsMap`](../interfaces/CameraInputsMap.md)[`FollowCamera`](FollowCamera.md)

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

• **camera**: [`FollowCamera`](FollowCamera.md)

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
| `input` | [`ICameraInput`](../interfaces/ICameraInput.md)[`FollowCamera`](FollowCamera.md) | camera input method |

#### Returns

`void`

#### Inherited from

[CameraInputsManager](CameraInputsManager.md).[add](CameraInputsManager.md#add)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/cameraInputsManager.ts:110

___

### addKeyboard

▸ **addKeyboard**(): [`FollowCameraInputsManager`](FollowCameraInputsManager.md)

Add keyboard input support to the input manager.

#### Returns

[`FollowCameraInputsManager`](FollowCameraInputsManager.md)

the current input manager

#### Defined in

https://github.com/babylon.js/core/src/Cameras/followCameraInputsManager.ts:25

___

### addMouseWheel

▸ **addMouseWheel**(): [`FollowCameraInputsManager`](FollowCameraInputsManager.md)

Add mouse wheel input support to the input manager.

#### Returns

[`FollowCameraInputsManager`](FollowCameraInputsManager.md)

the current input manager

#### Defined in

https://github.com/babylon.js/core/src/Cameras/followCameraInputsManager.ts:34

___

### addPointers

▸ **addPointers**(): [`FollowCameraInputsManager`](FollowCameraInputsManager.md)

Add pointers input support to the input manager.

#### Returns

[`FollowCameraInputsManager`](FollowCameraInputsManager.md)

the current input manager

#### Defined in

https://github.com/babylon.js/core/src/Cameras/followCameraInputsManager.ts:43

___

### addVRDeviceOrientation

▸ **addVRDeviceOrientation**(): [`FollowCameraInputsManager`](FollowCameraInputsManager.md)

Add orientation input support to the input manager.

#### Returns

[`FollowCameraInputsManager`](FollowCameraInputsManager.md)

the current input manager

#### Defined in

https://github.com/babylon.js/core/src/Cameras/followCameraInputsManager.ts:52

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
| `input` | [`ICameraInput`](../interfaces/ICameraInput.md)[`FollowCamera`](FollowCamera.md) | Defines the input to attach |

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

#### Inherited from

[CameraInputsManager](CameraInputsManager.md).[clear](CameraInputsManager.md#clear)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/cameraInputsManager.ts:235

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
| `inputToRemove` | [`ICameraInput`](../interfaces/ICameraInput.md)[`FollowCamera`](FollowCamera.md) | camera input method |

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
