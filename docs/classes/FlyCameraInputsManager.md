[@dev/core](../README.md) / [Exports](../modules.md) / FlyCameraInputsManager

# Class: FlyCameraInputsManager

Default Inputs manager for the FlyCamera.
It groups all the default supported inputs for ease of use.

**`See`**

https://doc.babylonjs.com/how_to/customizing_camera_inputs

## Hierarchy

- [`CameraInputsManager`](CameraInputsManager.md)[`FlyCamera`](FlyCamera.md)

  ↳ **`FlyCameraInputsManager`**

## Table of contents

### Constructors

- [constructor](FlyCameraInputsManager.md#constructor)

### Properties

- [attached](FlyCameraInputsManager.md#attached)
- [attachedToElement](FlyCameraInputsManager.md#attachedtoelement)
- [camera](FlyCameraInputsManager.md#camera)
- [checkInputs](FlyCameraInputsManager.md#checkinputs)
- [noPreventDefault](FlyCameraInputsManager.md#nopreventdefault)

### Methods

- [add](FlyCameraInputsManager.md#add)
- [addKeyboard](FlyCameraInputsManager.md#addkeyboard)
- [addMouse](FlyCameraInputsManager.md#addmouse)
- [attachElement](FlyCameraInputsManager.md#attachelement)
- [attachInput](FlyCameraInputsManager.md#attachinput)
- [clear](FlyCameraInputsManager.md#clear)
- [detachElement](FlyCameraInputsManager.md#detachelement)
- [parse](FlyCameraInputsManager.md#parse)
- [rebuildInputCheck](FlyCameraInputsManager.md#rebuildinputcheck)
- [remove](FlyCameraInputsManager.md#remove)
- [removeByType](FlyCameraInputsManager.md#removebytype)
- [serialize](FlyCameraInputsManager.md#serialize)

## Constructors

### constructor

• **new FlyCameraInputsManager**(`camera`)

Instantiates a new FlyCameraInputsManager.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `camera` | [`FlyCamera`](FlyCamera.md) | Defines the camera the inputs belong to. |

#### Overrides

[CameraInputsManager](CameraInputsManager.md).[constructor](CameraInputsManager.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/flyCameraInputsManager.ts:16

## Properties

### attached

• **attached**: [`CameraInputsMap`](../interfaces/CameraInputsMap.md)[`FlyCamera`](FlyCamera.md)

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

• **camera**: [`FlyCamera`](FlyCamera.md)

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
| `input` | [`ICameraInput`](../interfaces/ICameraInput.md)[`FlyCamera`](FlyCamera.md) | camera input method |

#### Returns

`void`

#### Inherited from

[CameraInputsManager](CameraInputsManager.md).[add](CameraInputsManager.md#add)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/cameraInputsManager.ts:110

___

### addKeyboard

▸ **addKeyboard**(): [`FlyCameraInputsManager`](FlyCameraInputsManager.md)

Add keyboard input support to the input manager.

#### Returns

[`FlyCameraInputsManager`](FlyCameraInputsManager.md)

the new FlyCameraKeyboardMoveInput().

#### Defined in

https://github.com/babylon.js/core/src/Cameras/flyCameraInputsManager.ts:24

___

### addMouse

▸ **addMouse**(): [`FlyCameraInputsManager`](FlyCameraInputsManager.md)

Add mouse input support to the input manager.

#### Returns

[`FlyCameraInputsManager`](FlyCameraInputsManager.md)

the new FlyCameraMouseInput().

#### Defined in

https://github.com/babylon.js/core/src/Cameras/flyCameraInputsManager.ts:33

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
| `input` | [`ICameraInput`](../interfaces/ICameraInput.md)[`FlyCamera`](FlyCamera.md) | Defines the input to attach |

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
| `inputToRemove` | [`ICameraInput`](../interfaces/ICameraInput.md)[`FlyCamera`](FlyCamera.md) | camera input method |

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
