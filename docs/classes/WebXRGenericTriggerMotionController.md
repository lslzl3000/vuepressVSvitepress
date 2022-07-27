[@dev/core](../README.md) / [Exports](../modules.md) / WebXRGenericTriggerMotionController

# Class: WebXRGenericTriggerMotionController

A generic trigger-only motion controller for WebXR

## Hierarchy

- [`WebXRAbstractMotionController`](WebXRAbstractMotionController.md)

  ↳ **`WebXRGenericTriggerMotionController`**

## Table of contents

### Constructors

- [constructor](WebXRGenericTriggerMotionController.md#constructor)

### Properties

- [\_doNotLoadControllerMesh](WebXRGenericTriggerMotionController.md#_donotloadcontrollermesh)
- [components](WebXRGenericTriggerMotionController.md#components)
- [disableAnimation](WebXRGenericTriggerMotionController.md#disableanimation)
- [gamepadObject](WebXRGenericTriggerMotionController.md#gamepadobject)
- [handedness](WebXRGenericTriggerMotionController.md#handedness)
- [layout](WebXRGenericTriggerMotionController.md#layout)
- [onModelLoadedObservable](WebXRGenericTriggerMotionController.md#onmodelloadedobservable)
- [profileId](WebXRGenericTriggerMotionController.md#profileid)
- [rootMesh](WebXRGenericTriggerMotionController.md#rootmesh)
- [scene](WebXRGenericTriggerMotionController.md#scene)
- [ProfileId](WebXRGenericTriggerMotionController.md#profileid-1)

### Accessors

- [handness](WebXRGenericTriggerMotionController.md#handness)

### Methods

- [\_getChildByName](WebXRGenericTriggerMotionController.md#_getchildbyname)
- [\_getFilenameAndPath](WebXRGenericTriggerMotionController.md#_getfilenameandpath)
- [\_getImmediateChildByName](WebXRGenericTriggerMotionController.md#_getimmediatechildbyname)
- [\_getModelLoadingConstraints](WebXRGenericTriggerMotionController.md#_getmodelloadingconstraints)
- [\_processLoadedModel](WebXRGenericTriggerMotionController.md#_processloadedmodel)
- [\_setRootMesh](WebXRGenericTriggerMotionController.md#_setrootmesh)
- [\_updateModel](WebXRGenericTriggerMotionController.md#_updatemodel)
- [dispose](WebXRGenericTriggerMotionController.md#dispose)
- [getAllComponentsOfType](WebXRGenericTriggerMotionController.md#getallcomponentsoftype)
- [getComponent](WebXRGenericTriggerMotionController.md#getcomponent)
- [getComponentIds](WebXRGenericTriggerMotionController.md#getcomponentids)
- [getComponentOfType](WebXRGenericTriggerMotionController.md#getcomponentoftype)
- [getMainComponent](WebXRGenericTriggerMotionController.md#getmaincomponent)
- [loadModel](WebXRGenericTriggerMotionController.md#loadmodel)
- [pulse](WebXRGenericTriggerMotionController.md#pulse)
- [updateFromXRFrame](WebXRGenericTriggerMotionController.md#updatefromxrframe)
- [updateModel](WebXRGenericTriggerMotionController.md#updatemodel)

## Constructors

### constructor

• **new WebXRGenericTriggerMotionController**(`scene`, `gamepadObject`, `handedness`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `scene` | [`Scene`](Scene.md) |
| `gamepadObject` | [`IMinimalMotionControllerObject`](../interfaces/IMinimalMotionControllerObject.md) |
| `handedness` | [`MotionControllerHandedness`](../modules.md#motioncontrollerhandedness) |

#### Overrides

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[constructor](WebXRAbstractMotionController.md#constructor)

#### Defined in

packages/dev/core/src/XR/motionController/webXRGenericMotionController.ts:19

## Properties

### \_doNotLoadControllerMesh

• **\_doNotLoadControllerMesh**: `boolean` = `false`

#### Inherited from

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[_doNotLoadControllerMesh](WebXRAbstractMotionController.md#_donotloadcontrollermesh)

#### Defined in

packages/dev/core/src/XR/motionController/webXRAbstractMotionController.ts:300

___

### components

• `Readonly` **components**: `Object` = `{}`

A map of components (WebXRControllerComponent) in this motion controller
Components have a ComponentType and can also have both button and axis definitions

#### Index signature

▪ [id: `string`]: [`WebXRControllerComponent`](WebXRControllerComponent.md)

#### Inherited from

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[components](WebXRAbstractMotionController.md#components)

#### Defined in

packages/dev/core/src/XR/motionController/webXRAbstractMotionController.ts:254

___

### disableAnimation

• **disableAnimation**: `boolean` = `false`

Disable the model's animation. Can be set at any time.

#### Inherited from

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[disableAnimation](WebXRAbstractMotionController.md#disableanimation)

#### Defined in

packages/dev/core/src/XR/motionController/webXRAbstractMotionController.ts:261

___

### gamepadObject

• **gamepadObject**: [`IMinimalMotionControllerObject`](../interfaces/IMinimalMotionControllerObject.md)

#### Inherited from

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[gamepadObject](WebXRAbstractMotionController.md#gamepadobject)

#### Defined in

packages/dev/core/src/XR/motionController/webXRAbstractMotionController.ts:292

___

### handedness

• **handedness**: [`MotionControllerHandedness`](../modules.md#motioncontrollerhandedness)

#### Inherited from

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[handedness](WebXRAbstractMotionController.md#handedness)

#### Defined in

packages/dev/core/src/XR/motionController/webXRAbstractMotionController.ts:296

___

### layout

• `Protected` **layout**: [`IMotionControllerLayout`](../interfaces/IMotionControllerLayout.md)

#### Inherited from

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[layout](WebXRAbstractMotionController.md#layout)

#### Defined in

packages/dev/core/src/XR/motionController/webXRAbstractMotionController.ts:288

___

### onModelLoadedObservable

• **onModelLoadedObservable**: [`Observable`](Observable.md)[`WebXRAbstractMotionController`](WebXRAbstractMotionController.md)

Observers registered here will be triggered when the model of this controller is done loading

#### Inherited from

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[onModelLoadedObservable](WebXRAbstractMotionController.md#onmodelloadedobservable)

#### Defined in

packages/dev/core/src/XR/motionController/webXRAbstractMotionController.ts:265

___

### profileId

• **profileId**: `string` = `WebXRGenericTriggerMotionController.ProfileId`

The profile id of this motion controller

#### Overrides

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[profileId](WebXRAbstractMotionController.md#profileid)

#### Defined in

packages/dev/core/src/XR/motionController/webXRGenericMotionController.ts:17

___

### rootMesh

• **rootMesh**: [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

The root mesh of the model. It is null if the model was not yet initialized

#### Inherited from

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[rootMesh](WebXRAbstractMotionController.md#rootmesh)

#### Defined in

packages/dev/core/src/XR/motionController/webXRAbstractMotionController.ts:273

___

### scene

• `Protected` **scene**: [`Scene`](Scene.md)

#### Inherited from

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[scene](WebXRAbstractMotionController.md#scene)

#### Defined in

packages/dev/core/src/XR/motionController/webXRAbstractMotionController.ts:286

___

### ProfileId

▪ `Static` **ProfileId**: `string` = `"generic-trigger"`

Static version of the profile id of this controller

#### Defined in

packages/dev/core/src/XR/motionController/webXRGenericMotionController.ts:15

## Accessors

### handness

• `get` **handness**(): [`MotionControllerHandedness`](../modules.md#motioncontrollerhandedness)

Backwards compatibility due to a deeply-integrated typo

#### Returns

[`MotionControllerHandedness`](../modules.md#motioncontrollerhandedness)

#### Inherited from

WebXRAbstractMotionController.handness

#### Defined in

packages/dev/core/src/XR/motionController/webXRAbstractMotionController.ts:446

## Methods

### \_getChildByName

▸ `Protected` **_getChildByName**(`node`, `name`): `undefined` \| [`AbstractMesh`](AbstractMesh.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `node` | [`AbstractMesh`](AbstractMesh.md) |
| `name` | `string` |

#### Returns

`undefined` \| [`AbstractMesh`](AbstractMesh.md)

#### Inherited from

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[_getChildByName](WebXRAbstractMotionController.md#_getchildbyname)

#### Defined in

packages/dev/core/src/XR/motionController/webXRAbstractMotionController.ts:469

___

### \_getFilenameAndPath

▸ `Protected` **_getFilenameAndPath**(): `Object`

Get the filename and path for this controller's model

#### Returns

`Object`

a map of filename and path

| Name | Type |
| :------ | :------ |
| `filename` | `string` |
| `path` | `string` |

#### Overrides

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[_getFilenameAndPath](WebXRAbstractMotionController.md#_getfilenameandpath)

#### Defined in

packages/dev/core/src/XR/motionController/webXRGenericMotionController.ts:23

___

### \_getImmediateChildByName

▸ `Protected` **_getImmediateChildByName**(`node`, `name`): `undefined` \| [`AbstractMesh`](AbstractMesh.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `node` | [`AbstractMesh`](AbstractMesh.md) |
| `name` | `string` |

#### Returns

`undefined` \| [`AbstractMesh`](AbstractMesh.md)

#### Inherited from

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[_getImmediateChildByName](WebXRAbstractMotionController.md#_getimmediatechildbyname)

#### Defined in

packages/dev/core/src/XR/motionController/webXRAbstractMotionController.ts:474

___

### \_getModelLoadingConstraints

▸ `Protected` **_getModelLoadingConstraints**(): `boolean`

This function is called before the mesh is loaded. It checks for loading constraints.
For example, this function can check if the GLB loader is available
If this function returns false, the generic controller will be loaded instead

#### Returns

`boolean`

Is the client ready to load the mesh

#### Overrides

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[_getModelLoadingConstraints](WebXRAbstractMotionController.md#_getmodelloadingconstraints)

#### Defined in

packages/dev/core/src/XR/motionController/webXRGenericMotionController.ts:30

___

### \_processLoadedModel

▸ `Protected` **_processLoadedModel**(`meshes`): `void`

This function will be called after the model was successfully loaded and can be used
for mesh transformations before it is available for the user

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `meshes` | [`AbstractMesh`](AbstractMesh.md)[] | the loaded meshes |

#### Returns

`void`

#### Overrides

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[_processLoadedModel](WebXRAbstractMotionController.md#_processloadedmodel)

#### Defined in

packages/dev/core/src/XR/motionController/webXRGenericMotionController.ts:35

___

### \_setRootMesh

▸ `Protected` **_setRootMesh**(`meshes`): `void`

Set the root mesh for this controller. Important for the WebXR controller class

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `meshes` | [`AbstractMesh`](AbstractMesh.md)[] | the loaded meshes |

#### Returns

`void`

#### Overrides

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[_setRootMesh](WebXRAbstractMotionController.md#_setrootmesh)

#### Defined in

packages/dev/core/src/XR/motionController/webXRGenericMotionController.ts:39

___

### \_updateModel

▸ `Protected` **_updateModel**(): `void`

A function executed each frame that updates the mesh (if needed)

#### Returns

`void`

#### Overrides

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[_updateModel](WebXRAbstractMotionController.md#_updatemodel)

#### Defined in

packages/dev/core/src/XR/motionController/webXRGenericMotionController.ts:52

___

### dispose

▸ **dispose**(): `void`

Dispose this controller, the model mesh and all its components

#### Returns

`void`

#### Inherited from

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[dispose](WebXRAbstractMotionController.md#dispose)

#### Defined in

packages/dev/core/src/XR/motionController/webXRAbstractMotionController.ts:317

___

### getAllComponentsOfType

▸ **getAllComponentsOfType**(`type`): [`WebXRControllerComponent`](WebXRControllerComponent.md)[]

Returns all components of specific type

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | [`MotionControllerComponentType`](../modules.md#motioncontrollercomponenttype) | the type to search for |

#### Returns

[`WebXRControllerComponent`](WebXRControllerComponent.md)[]

an array of components with this type

#### Inherited from

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[getAllComponentsOfType](WebXRAbstractMotionController.md#getallcomponentsoftype)

#### Defined in

packages/dev/core/src/XR/motionController/webXRAbstractMotionController.ts:332

___

### getComponent

▸ **getComponent**(`id`): [`WebXRControllerComponent`](WebXRControllerComponent.md)

get a component based an its component id as defined in layout.components

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | the id of the component |

#### Returns

[`WebXRControllerComponent`](WebXRControllerComponent.md)

the component correlates to the id or undefined if not found

#### Inherited from

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[getComponent](WebXRAbstractMotionController.md#getcomponent)

#### Defined in

packages/dev/core/src/XR/motionController/webXRAbstractMotionController.ts:343

___

### getComponentIds

▸ **getComponentIds**(): `string`[]

Get the list of components available in this motion controller

#### Returns

`string`[]

an array of strings correlating to available components

#### Inherited from

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[getComponentIds](WebXRAbstractMotionController.md#getcomponentids)

#### Defined in

packages/dev/core/src/XR/motionController/webXRAbstractMotionController.ts:351

___

### getComponentOfType

▸ **getComponentOfType**(`type`): [`Nullable`](../modules.md#nullable)[`WebXRControllerComponent`](WebXRControllerComponent.md)

Get the first component of specific type

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | [`MotionControllerComponentType`](../modules.md#motioncontrollercomponenttype) | type of component to find |

#### Returns

[`Nullable`](../modules.md#nullable)[`WebXRControllerComponent`](WebXRControllerComponent.md)

a controller component or null if not found

#### Inherited from

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[getComponentOfType](WebXRAbstractMotionController.md#getcomponentoftype)

#### Defined in

packages/dev/core/src/XR/motionController/webXRAbstractMotionController.ts:360

___

### getMainComponent

▸ **getMainComponent**(): [`WebXRControllerComponent`](WebXRControllerComponent.md)

Get the main (Select) component of this controller as defined in the layout

#### Returns

[`WebXRControllerComponent`](WebXRControllerComponent.md)

the main component of this controller

#### Inherited from

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[getMainComponent](WebXRAbstractMotionController.md#getmaincomponent)

#### Defined in

packages/dev/core/src/XR/motionController/webXRAbstractMotionController.ts:368

___

### loadModel

▸ **loadModel**(): `Promise``boolean`

Loads the model correlating to this controller
When the mesh is loaded, the onModelLoadedObservable will be triggered

#### Returns

`Promise``boolean`

A promise fulfilled with the result of the model loading

#### Inherited from

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[loadModel](WebXRAbstractMotionController.md#loadmodel)

#### Defined in

packages/dev/core/src/XR/motionController/webXRAbstractMotionController.ts:377

___

### pulse

▸ **pulse**(`value`, `duration`, `hapticActuatorIndex?`): `Promise``boolean`

Pulse (vibrate) this controller
If the controller does not support pulses, this function will fail silently and return Promise directly after called
Consecutive calls to this function will cancel the last pulse call

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `value` | `number` | `undefined` | the strength of the pulse in 0.0...1.0 range |
| `duration` | `number` | `undefined` | Duration of the pulse in milliseconds |
| `hapticActuatorIndex` | `number` | `0` | optional index of actuator (will usually be 0) |

#### Returns

`Promise``boolean`

a promise that will send true when the pulse has ended and false if the device doesn't support pulse or an error accrued

#### Inherited from

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[pulse](WebXRAbstractMotionController.md#pulse)

#### Defined in

packages/dev/core/src/XR/motionController/webXRAbstractMotionController.ts:460

___

### updateFromXRFrame

▸ **updateFromXRFrame**(`xrFrame`): `void`

Update this model using the current XRFrame

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `xrFrame` | `XRFrame` | the current xr frame to use and update the model |

#### Returns

`void`

#### Inherited from

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[updateFromXRFrame](WebXRAbstractMotionController.md#updatefromxrframe)

#### Defined in

packages/dev/core/src/XR/motionController/webXRAbstractMotionController.ts:438

___

### updateModel

▸ `Protected` **updateModel**(`xrFrame`): `void`

Update the model itself with the current frame data

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `xrFrame` | `XRFrame` | the frame to use for updating the model mesh |

#### Returns

`void`

#### Inherited from

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[updateModel](WebXRAbstractMotionController.md#updatemodel)

#### Defined in

packages/dev/core/src/XR/motionController/webXRAbstractMotionController.ts:505
