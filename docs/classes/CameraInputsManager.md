[@dev/core](../README.md) / [Exports](../modules.md) / CameraInputsManager

# Class: CameraInputsManagerTCamera

This represents the input manager used within a camera.
It helps dealing with all the different kind of input attached to a camera.

**`See`**

https://doc.babylonjs.com/how_to/customizing_camera_inputs

## Type parameters

| Name | Type |
| :------ | :------ |
| `TCamera` | extends [`Camera`](Camera.md) |

## Hierarchy

- **`CameraInputsManager`**

  ↳ [`FreeCameraInputsManager`](FreeCameraInputsManager.md)

  ↳ [`ArcRotateCameraInputsManager`](ArcRotateCameraInputsManager.md)

  ↳ [`FlyCameraInputsManager`](FlyCameraInputsManager.md)

  ↳ [`FollowCameraInputsManager`](FollowCameraInputsManager.md)

## Table of contents

### Constructors

- [constructor](CameraInputsManager.md#constructor)

### Properties

- [attached](CameraInputsManager.md#attached)
- [attachedToElement](CameraInputsManager.md#attachedtoelement)
- [camera](CameraInputsManager.md#camera)
- [checkInputs](CameraInputsManager.md#checkinputs)
- [noPreventDefault](CameraInputsManager.md#nopreventdefault)

### Methods

- [\_addCheckInputs](CameraInputsManager.md#_addcheckinputs)
- [add](CameraInputsManager.md#add)
- [attachElement](CameraInputsManager.md#attachelement)
- [attachInput](CameraInputsManager.md#attachinput)
- [clear](CameraInputsManager.md#clear)
- [detachElement](CameraInputsManager.md#detachelement)
- [parse](CameraInputsManager.md#parse)
- [rebuildInputCheck](CameraInputsManager.md#rebuildinputcheck)
- [remove](CameraInputsManager.md#remove)
- [removeByType](CameraInputsManager.md#removebytype)
- [serialize](CameraInputsManager.md#serialize)

## Constructors

### constructor

• **new CameraInputsManager**`TCamera`(`camera`)

Instantiate a new Camera Input Manager.

#### Type parameters

| Name | Type |
| :------ | :------ |
| `TCamera` | extends [`Camera`](Camera.md)`TCamera` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `camera` | `TCamera` | Defines the camera the input manager belongs to |

#### Defined in

packages/dev/core/src/Cameras/cameraInputsManager.ts:99

## Properties

### attached

• **attached**: [`CameraInputsMap`](../interfaces/CameraInputsMap.md)`TCamera`

Defines the list of inputs attached to the camera.

#### Defined in

packages/dev/core/src/Cameras/cameraInputsManager.ts:71

___

### attachedToElement

• **attachedToElement**: `boolean` = `false`

Defines the dom element the camera is collecting inputs from.
This is null if the controls have not been attached.

#### Defined in

packages/dev/core/src/Cameras/cameraInputsManager.ts:77

___

### camera

• **camera**: `TCamera`

Defined the camera the input manager belongs to.

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

#### Defined in

packages/dev/core/src/Cameras/cameraInputsManager.ts:93

___

### noPreventDefault

• **noPreventDefault**: `boolean`

Defines whether event caught by the controls should call preventdefault() (https://developer.mozilla.org/en-US/docs/Web/API/Event/preventDefault)

#### Defined in

packages/dev/core/src/Cameras/cameraInputsManager.ts:82

## Methods

### \_addCheckInputs

▸ `Private` **_addCheckInputs**(`fn`): () => `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `fn` | () => `void` |

#### Returns

`fn`

▸ (): `void`

##### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/cameraInputsManager.ts:166

___

### add

▸ **add**(`input`): `void`

Add an input method to a camera

**`See`**

https://doc.babylonjs.com/how_to/customizing_camera_inputs

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `input` | [`ICameraInput`](../interfaces/ICameraInput.md)`TCamera` | camera input method |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/cameraInputsManager.ts:110

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

#### Defined in

packages/dev/core/src/Cameras/cameraInputsManager.ts:188

___

### attachInput

▸ **attachInput**(`input`): `void`

Attach the input controls to the currently attached dom element to listen the events from.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `input` | [`ICameraInput`](../interfaces/ICameraInput.md)`TCamera` | Defines the input to attach |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/cameraInputsManager.ts:178

___

### clear

▸ **clear**(): `void`

Remove all attached input methods from a camera

#### Returns

`void`

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

#### Defined in

packages/dev/core/src/Cameras/cameraInputsManager.ts:266

___

### rebuildInputCheck

▸ **rebuildInputCheck**(): `void`

Rebuild the dynamic inputCheck function from the current list of
defined inputs in the manager.

#### Returns

`void`

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
| `inputToRemove` | [`ICameraInput`](../interfaces/ICameraInput.md)`TCamera` | camera input method |

#### Returns

`void`

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

#### Defined in

packages/dev/core/src/Cameras/cameraInputsManager.ts:250
