[@dev/core](../README.md) / [Exports](../modules.md) / WebXRAbstractMotionController

# Class: WebXRAbstractMotionController

An Abstract Motion controller
This class receives an xrInput and a profile layout and uses those to initialize the components
Each component has an observable to check for changes in value and state

## Hierarchy

- **`WebXRAbstractMotionController`**

  ↳ [`WebXRGenericHandController`](WebXRGenericHandController.md)

  ↳ [`WebXRGenericTriggerMotionController`](WebXRGenericTriggerMotionController.md)

  ↳ [`WebXRMicrosoftMixedRealityController`](WebXRMicrosoftMixedRealityController.md)

  ↳ [`WebXROculusTouchMotionController`](WebXROculusTouchMotionController.md)

  ↳ [`WebXRHTCViveMotionController`](WebXRHTCViveMotionController.md)

  ↳ [`WebXRProfiledMotionController`](WebXRProfiledMotionController.md)

## Implements

- [`IDisposable`](../interfaces/IDisposable.md)

## Table of contents

### Constructors

- [constructor](WebXRAbstractMotionController.md#constructor)

### Properties

- [\_doNotLoadControllerMesh](WebXRAbstractMotionController.md#_donotloadcontrollermesh)
- [\_modelReady](WebXRAbstractMotionController.md#_modelready)
- [components](WebXRAbstractMotionController.md#components)
- [disableAnimation](WebXRAbstractMotionController.md#disableanimation)
- [gamepadObject](WebXRAbstractMotionController.md#gamepadobject)
- [handedness](WebXRAbstractMotionController.md#handedness)
- [layout](WebXRAbstractMotionController.md#layout)
- [onModelLoadedObservable](WebXRAbstractMotionController.md#onmodelloadedobservable)
- [profileId](WebXRAbstractMotionController.md#profileid)
- [rootMesh](WebXRAbstractMotionController.md#rootmesh)
- [scene](WebXRAbstractMotionController.md#scene)

### Accessors

- [handness](WebXRAbstractMotionController.md#handness)

### Methods

- [\_getChildByName](WebXRAbstractMotionController.md#_getchildbyname)
- [\_getFilenameAndPath](WebXRAbstractMotionController.md#_getfilenameandpath)
- [\_getGenericFilenameAndPath](WebXRAbstractMotionController.md#_getgenericfilenameandpath)
- [\_getGenericParentMesh](WebXRAbstractMotionController.md#_getgenericparentmesh)
- [\_getImmediateChildByName](WebXRAbstractMotionController.md#_getimmediatechildbyname)
- [\_getModelLoadingConstraints](WebXRAbstractMotionController.md#_getmodelloadingconstraints)
- [\_initComponent](WebXRAbstractMotionController.md#_initcomponent)
- [\_processLoadedModel](WebXRAbstractMotionController.md#_processloadedmodel)
- [\_setRootMesh](WebXRAbstractMotionController.md#_setrootmesh)
- [\_updateModel](WebXRAbstractMotionController.md#_updatemodel)
- [dispose](WebXRAbstractMotionController.md#dispose)
- [getAllComponentsOfType](WebXRAbstractMotionController.md#getallcomponentsoftype)
- [getComponent](WebXRAbstractMotionController.md#getcomponent)
- [getComponentIds](WebXRAbstractMotionController.md#getcomponentids)
- [getComponentOfType](WebXRAbstractMotionController.md#getcomponentoftype)
- [getMainComponent](WebXRAbstractMotionController.md#getmaincomponent)
- [loadModel](WebXRAbstractMotionController.md#loadmodel)
- [pulse](WebXRAbstractMotionController.md#pulse)
- [updateFromXRFrame](WebXRAbstractMotionController.md#updatefromxrframe)
- [updateModel](WebXRAbstractMotionController.md#updatemodel)

## Constructors

### constructor

• **new WebXRAbstractMotionController**(`scene`, `layout`, `gamepadObject`, `handedness`, `_doNotLoadControllerMesh?`, `_controllerCache?`)

constructs a new abstract motion controller

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | `undefined` | the scene to which the model of the controller will be added |
| `layout` | [`IMotionControllerLayout`](../interfaces/IMotionControllerLayout.md) | `undefined` | The profile layout to load |
| `gamepadObject` | [`IMinimalMotionControllerObject`](../interfaces/IMinimalMotionControllerObject.md) | `undefined` | The gamepad object correlating to this controller |
| `handedness` | [`MotionControllerHandedness`](../modules.md#motioncontrollerhandedness) | `undefined` | handedness (left/right/none) of this controller |
| `_doNotLoadControllerMesh` | `boolean` | `false` | set this flag to ignore the mesh loading |
| `_controllerCache?` | { `filename`: `string` ; `meshes`: [`AbstractMesh`](AbstractMesh.md)[] ; `path`: `string`  }[] | `undefined` | a cache holding controller models already loaded in this session |

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:284

## Properties

### \_doNotLoadControllerMesh

• **\_doNotLoadControllerMesh**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:300

___

### \_modelReady

• `Private` **\_modelReady**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:248

___

### components

• `Readonly` **components**: `Object` = `{}`

A map of components (WebXRControllerComponent) in this motion controller
Components have a ComponentType and can also have both button and axis definitions

#### Index signature

▪ [id: `string`]: [`WebXRControllerComponent`](WebXRControllerComponent.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:254

___

### disableAnimation

• **disableAnimation**: `boolean` = `false`

Disable the model's animation. Can be set at any time.

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:261

___

### gamepadObject

• **gamepadObject**: [`IMinimalMotionControllerObject`](../interfaces/IMinimalMotionControllerObject.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:292

___

### handedness

• **handedness**: [`MotionControllerHandedness`](../modules.md#motioncontrollerhandedness)

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:296

___

### layout

• `Protected` **layout**: [`IMotionControllerLayout`](../interfaces/IMotionControllerLayout.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:288

___

### onModelLoadedObservable

• **onModelLoadedObservable**: [`Observable`](Observable.md)[`WebXRAbstractMotionController`](WebXRAbstractMotionController.md)

Observers registered here will be triggered when the model of this controller is done loading

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:265

___

### profileId

• `Abstract` **profileId**: `string`

The profile id of this motion controller

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:269

___

### rootMesh

• **rootMesh**: [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

The root mesh of the model. It is null if the model was not yet initialized

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:273

___

### scene

• `Protected` **scene**: [`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:286

## Accessors

### handness

• `get` **handness**(): [`MotionControllerHandedness`](../modules.md#motioncontrollerhandedness)

Backwards compatibility due to a deeply-integrated typo

#### Returns

[`MotionControllerHandedness`](../modules.md#motioncontrollerhandedness)

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:446

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

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:469

___

### \_getFilenameAndPath

▸ `Protected` `Abstract` **_getFilenameAndPath**(): `Object`

Get the filename and path for this controller's model

#### Returns

`Object`

a map of filename and path

| Name | Type |
| :------ | :------ |
| `filename` | `string` |
| `path` | `string` |

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:516

___

### \_getGenericFilenameAndPath

▸ `Private` **_getGenericFilenameAndPath**(): `Object`

#### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `filename` | `string` |
| `path` | `string` |

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:541

___

### \_getGenericParentMesh

▸ `Private` **_getGenericParentMesh**(`meshes`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `meshes` | [`AbstractMesh`](AbstractMesh.md)[] |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:548

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

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:474

___

### \_getModelLoadingConstraints

▸ `Protected` `Abstract` **_getModelLoadingConstraints**(): `boolean`

This function is called before the mesh is loaded. It checks for loading constraints.
For example, this function can check if the GLB loader is available
If this function returns false, the generic controller will be loaded instead

#### Returns

`boolean`

Is the client ready to load the mesh

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:523

___

### \_initComponent

▸ `Private` **_initComponent**(`id`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:232

___

### \_processLoadedModel

▸ `Protected` `Abstract` **_processLoadedModel**(`meshes`): `void`

This function will be called after the model was successfully loaded and can be used
for mesh transformations before it is available for the user

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `meshes` | [`AbstractMesh`](AbstractMesh.md)[] | the loaded meshes |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:529

___

### \_setRootMesh

▸ `Protected` `Abstract` **_setRootMesh**(`meshes`): `void`

Set the root mesh for this controller. Important for the WebXR controller class

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `meshes` | [`AbstractMesh`](AbstractMesh.md)[] | the loaded meshes |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:534

___

### \_updateModel

▸ `Protected` `Abstract` **_updateModel**(`xrFrame`): `void`

A function executed each frame that updates the mesh (if needed)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `xrFrame` | `XRFrame` | the current xrFrame |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:539

___

### dispose

▸ **dispose**(): `void`

Dispose this controller, the model mesh and all its components

#### Returns

`void`

#### Implementation of

[IDisposable](../interfaces/IDisposable.md).[dispose](../interfaces/IDisposable.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:317

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

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:332

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

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:343

___

### getComponentIds

▸ **getComponentIds**(): `string`[]

Get the list of components available in this motion controller

#### Returns

`string`[]

an array of strings correlating to available components

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:351

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

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:360

___

### getMainComponent

▸ **getMainComponent**(): [`WebXRControllerComponent`](WebXRControllerComponent.md)

Get the main (Select) component of this controller as defined in the layout

#### Returns

[`WebXRControllerComponent`](WebXRControllerComponent.md)

the main component of this controller

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:368

___

### loadModel

▸ **loadModel**(): `Promise``boolean`

Loads the model correlating to this controller
When the mesh is loaded, the onModelLoadedObservable will be triggered

#### Returns

`Promise``boolean`

A promise fulfilled with the result of the model loading

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:377

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

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:460

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

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:438

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

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:505
