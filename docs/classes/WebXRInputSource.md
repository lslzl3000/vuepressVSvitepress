[@dev/core](../README.md) / [Exports](../modules.md) / WebXRInputSource

# Class: WebXRInputSource

Represents an XR controller

## Table of contents

### Constructors

- [constructor](WebXRInputSource.md#constructor)

### Properties

- [\_disposed](WebXRInputSource.md#_disposed)
- [\_tmpVector](WebXRInputSource.md#_tmpvector)
- [\_uniqueId](WebXRInputSource.md#_uniqueid)
- [grip](WebXRInputSource.md#grip)
- [inputSource](WebXRInputSource.md#inputsource)
- [motionController](WebXRInputSource.md#motioncontroller)
- [onDisposeObservable](WebXRInputSource.md#ondisposeobservable)
- [onMeshLoadedObservable](WebXRInputSource.md#onmeshloadedobservable)
- [onMotionControllerInitObservable](WebXRInputSource.md#onmotioncontrollerinitobservable)
- [pointer](WebXRInputSource.md#pointer)

### Accessors

- [uniqueId](WebXRInputSource.md#uniqueid)

### Methods

- [dispose](WebXRInputSource.md#dispose)
- [getWorldPointerRayToRef](WebXRInputSource.md#getworldpointerraytoref)
- [updateFromXRFrame](WebXRInputSource.md#updatefromxrframe)

## Constructors

### constructor

• **new WebXRInputSource**(`_scene`, `inputSource`, `_options?`)

Creates the input source object

**`See`**

https://doc.babylonjs.com/how_to/webxr_controllers_support

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `_scene` | [`Scene`](Scene.md) | the scene which the controller should be associated to |
| `inputSource` | `XRInputSource` | the underlying input source for the controller |
| `_options` | [`IWebXRControllerOptions`](../interfaces/IWebXRControllerOptions.md) | options for this controller creation |

#### Defined in

packages/dev/core/src/XR/webXRInputSource.ts:90

## Properties

### \_disposed

• `Private` **\_disposed**: `boolean` = `false`

#### Defined in

packages/dev/core/src/XR/webXRInputSource.ts:44

___

### \_tmpVector

• `Private` **\_tmpVector**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/XR/webXRInputSource.ts:42

___

### \_uniqueId

• `Private` **\_uniqueId**: `string`

#### Defined in

packages/dev/core/src/XR/webXRInputSource.ts:43

___

### grip

• `Optional` **grip**: [`AbstractMesh`](AbstractMesh.md)

Represents the part of the controller that is held. This may not exist if the controller is the head mounted display itself, if that's the case only the pointer from the head will be available

#### Defined in

packages/dev/core/src/XR/webXRInputSource.ts:49

___

### inputSource

• **inputSource**: `XRInputSource`

#### Defined in

packages/dev/core/src/XR/webXRInputSource.ts:93

___

### motionController

• `Optional` **motionController**: [`WebXRAbstractMotionController`](WebXRAbstractMotionController.md)

If available, this is the gamepad object related to this controller.
Using this object it is possible to get click events and trackpad changes of the
webxr controller that is currently being used.

#### Defined in

packages/dev/core/src/XR/webXRInputSource.ts:55

___

### onDisposeObservable

• **onDisposeObservable**: [`Observable`](Observable.md)[`WebXRInputSource`](WebXRInputSource.md)

Event that fires when the controller is removed/disposed.
The object provided as event data is this controller, after associated assets were disposed.
uniqueId is still available.

#### Defined in

packages/dev/core/src/XR/webXRInputSource.ts:61

___

### onMeshLoadedObservable

• **onMeshLoadedObservable**: [`Observable`](Observable.md)[`AbstractMesh`](AbstractMesh.md)

Will be triggered when the mesh associated with the motion controller is done loading.
It is also possible that this will never trigger (!) if no mesh was loaded, or if the developer decides to load a different mesh
A shortened version of controller -> motion controller -> on mesh loaded.

#### Defined in

packages/dev/core/src/XR/webXRInputSource.ts:67

___

### onMotionControllerInitObservable

• **onMotionControllerInitObservable**: [`Observable`](Observable.md)[`WebXRAbstractMotionController`](WebXRAbstractMotionController.md)

Observers registered here will trigger when a motion controller profile was assigned to this xr controller

#### Defined in

packages/dev/core/src/XR/webXRInputSource.ts:71

___

### pointer

• **pointer**: [`AbstractMesh`](AbstractMesh.md)

Pointer which can be used to select objects or attach a visible laser to

#### Defined in

packages/dev/core/src/XR/webXRInputSource.ts:75

## Accessors

### uniqueId

• `get` **uniqueId**(): `string`

Get this controllers unique id

#### Returns

`string`

#### Defined in

packages/dev/core/src/XR/webXRInputSource.ts:144

## Methods

### dispose

▸ **dispose**(): `void`

Disposes of the object

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/webXRInputSource.ts:151

___

### getWorldPointerRayToRef

▸ **getWorldPointerRayToRef**(`result`, `gripIfAvailable?`): `void`

Gets a world space ray coming from the pointer or grip

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `result` | [`Ray`](Ray.md) | `undefined` | the resulting ray |
| `gripIfAvailable` | `boolean` | `false` | use the grip mesh instead of the pointer, if available |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/webXRInputSource.ts:171

___

### updateFromXRFrame

▸ **updateFromXRFrame**(`xrFrame`, `referenceSpace`, `xrCamera`): `void`

Updates the controller pose based on the given XRFrame

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `xrFrame` | `XRFrame` | xr frame to update the pose with |
| `referenceSpace` | `XRReferenceSpace` | reference space to use |
| `xrCamera` | [`WebXRCamera`](WebXRCamera.md) | the xr camera, used for parenting |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/webXRInputSource.ts:185
