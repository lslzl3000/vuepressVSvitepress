[@dev/core](../README.md) / [Exports](../modules.md) / WebXRMicrosoftMixedRealityController

# Class: WebXRMicrosoftMixedRealityController

The motion controller class for all microsoft mixed reality controllers

## Hierarchy

- [`WebXRAbstractMotionController`](WebXRAbstractMotionController.md)

  ↳ **`WebXRMicrosoftMixedRealityController`**

## Table of contents

### Constructors

- [constructor](WebXRMicrosoftMixedRealityController.md#constructor)

### Properties

- [\_doNotLoadControllerMesh](WebXRMicrosoftMixedRealityController.md#_donotloadcontrollermesh)
- [\_mapping](WebXRMicrosoftMixedRealityController.md#_mapping)
- [components](WebXRMicrosoftMixedRealityController.md#components)
- [disableAnimation](WebXRMicrosoftMixedRealityController.md#disableanimation)
- [gamepadObject](WebXRMicrosoftMixedRealityController.md#gamepadobject)
- [handedness](WebXRMicrosoftMixedRealityController.md#handedness)
- [layout](WebXRMicrosoftMixedRealityController.md#layout)
- [onModelLoadedObservable](WebXRMicrosoftMixedRealityController.md#onmodelloadedobservable)
- [profileId](WebXRMicrosoftMixedRealityController.md#profileid)
- [rootMesh](WebXRMicrosoftMixedRealityController.md#rootmesh)
- [scene](WebXRMicrosoftMixedRealityController.md#scene)
- [MODEL\_BASE\_URL](WebXRMicrosoftMixedRealityController.md#model_base_url)
- [MODEL\_LEFT\_FILENAME](WebXRMicrosoftMixedRealityController.md#model_left_filename)
- [MODEL\_RIGHT\_FILENAME](WebXRMicrosoftMixedRealityController.md#model_right_filename)

### Accessors

- [handness](WebXRMicrosoftMixedRealityController.md#handness)

### Methods

- [\_getChildByName](WebXRMicrosoftMixedRealityController.md#_getchildbyname)
- [\_getFilenameAndPath](WebXRMicrosoftMixedRealityController.md#_getfilenameandpath)
- [\_getImmediateChildByName](WebXRMicrosoftMixedRealityController.md#_getimmediatechildbyname)
- [\_getModelLoadingConstraints](WebXRMicrosoftMixedRealityController.md#_getmodelloadingconstraints)
- [\_processLoadedModel](WebXRMicrosoftMixedRealityController.md#_processloadedmodel)
- [\_setRootMesh](WebXRMicrosoftMixedRealityController.md#_setrootmesh)
- [\_updateModel](WebXRMicrosoftMixedRealityController.md#_updatemodel)
- [dispose](WebXRMicrosoftMixedRealityController.md#dispose)
- [getAllComponentsOfType](WebXRMicrosoftMixedRealityController.md#getallcomponentsoftype)
- [getComponent](WebXRMicrosoftMixedRealityController.md#getcomponent)
- [getComponentIds](WebXRMicrosoftMixedRealityController.md#getcomponentids)
- [getComponentOfType](WebXRMicrosoftMixedRealityController.md#getcomponentoftype)
- [getMainComponent](WebXRMicrosoftMixedRealityController.md#getmaincomponent)
- [loadModel](WebXRMicrosoftMixedRealityController.md#loadmodel)
- [pulse](WebXRMicrosoftMixedRealityController.md#pulse)
- [updateFromXRFrame](WebXRMicrosoftMixedRealityController.md#updatefromxrframe)
- [updateModel](WebXRMicrosoftMixedRealityController.md#updatemodel)

## Constructors

### constructor

• **new WebXRMicrosoftMixedRealityController**(`scene`, `gamepadObject`, `handedness`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `scene` | [`Scene`](Scene.md) |
| `gamepadObject` | [`IMinimalMotionControllerObject`](../interfaces/IMinimalMotionControllerObject.md) |
| `handedness` | [`MotionControllerHandedness`](../modules.md#motioncontrollerhandedness) |

#### Overrides

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[constructor](WebXRAbstractMotionController.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRMicrosoftMixedRealityController.ts:85

## Properties

### \_doNotLoadControllerMesh

• **\_doNotLoadControllerMesh**: `boolean` = `false`

#### Inherited from

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[_doNotLoadControllerMesh](WebXRAbstractMotionController.md#_donotloadcontrollermesh)

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:300

___

### \_mapping

• `Protected` `Readonly` **\_mapping**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `axes` | { `xr-standard-thumbstick`: { `x-axis`: { `rootNodeName`: `string` = "THUMBSTICK\_X" } ; `y-axis`: { `rootNodeName`: `string` = "THUMBSTICK\_Y" }  } ; `xr-standard-touchpad`: { `x-axis`: { `rootNodeName`: `string` = "TOUCHPAD\_TOUCH\_X" } ; `y-axis`: { `rootNodeName`: `string` = "TOUCHPAD\_TOUCH\_Y" }  }  } |
| `axes.xr-standard-thumbstick` | { `x-axis`: { `rootNodeName`: `string` = "THUMBSTICK\_X" } ; `y-axis`: { `rootNodeName`: `string` = "THUMBSTICK\_Y" }  } |
| `axes.xr-standard-thumbstick.x-axis` | { `rootNodeName`: `string` = "THUMBSTICK\_X" } |
| `axes.xr-standard-thumbstick.x-axis.rootNodeName` | `string` |
| `axes.xr-standard-thumbstick.y-axis` | { `rootNodeName`: `string` = "THUMBSTICK\_Y" } |
| `axes.xr-standard-thumbstick.y-axis.rootNodeName` | `string` |
| `axes.xr-standard-touchpad` | { `x-axis`: { `rootNodeName`: `string` = "TOUCHPAD\_TOUCH\_X" } ; `y-axis`: { `rootNodeName`: `string` = "TOUCHPAD\_TOUCH\_Y" }  } |
| `axes.xr-standard-touchpad.x-axis` | { `rootNodeName`: `string` = "TOUCHPAD\_TOUCH\_X" } |
| `axes.xr-standard-touchpad.x-axis.rootNodeName` | `string` |
| `axes.xr-standard-touchpad.y-axis` | { `rootNodeName`: `string` = "TOUCHPAD\_TOUCH\_Y" } |
| `axes.xr-standard-touchpad.y-axis.rootNodeName` | `string` |
| `buttons` | { `xr-standard-squeeze`: { `componentProperty`: `string` = "state"; `rootNodeName`: `string` = "GRASP"; `states`: `string`[]  } ; `xr-standard-thumbstick`: { `componentProperty`: `string` = "state"; `rootNodeName`: `string` = "THUMBSTICK\_PRESS"; `states`: `string`[]  } ; `xr-standard-touchpad`: { `labelAnchorNodeName`: `string` = "squeeze-label"; `rootNodeName`: `string` = "TOUCHPAD\_PRESS"; `touchPointNodeName`: `string` = "TOUCH" } ; `xr-standard-trigger`: { `componentProperty`: `string` = "button"; `rootNodeName`: `string` = "SELECT"; `states`: `string`[]  }  } |
| `buttons.xr-standard-squeeze` | { `componentProperty`: `string` = "state"; `rootNodeName`: `string` = "GRASP"; `states`: `string`[]  } |
| `buttons.xr-standard-squeeze.componentProperty` | `string` |
| `buttons.xr-standard-squeeze.rootNodeName` | `string` |
| `buttons.xr-standard-squeeze.states` | `string`[] |
| `buttons.xr-standard-thumbstick` | { `componentProperty`: `string` = "state"; `rootNodeName`: `string` = "THUMBSTICK\_PRESS"; `states`: `string`[]  } |
| `buttons.xr-standard-thumbstick.componentProperty` | `string` |
| `buttons.xr-standard-thumbstick.rootNodeName` | `string` |
| `buttons.xr-standard-thumbstick.states` | `string`[] |
| `buttons.xr-standard-touchpad` | { `labelAnchorNodeName`: `string` = "squeeze-label"; `rootNodeName`: `string` = "TOUCHPAD\_PRESS"; `touchPointNodeName`: `string` = "TOUCH" } |
| `buttons.xr-standard-touchpad.labelAnchorNodeName` | `string` |
| `buttons.xr-standard-touchpad.rootNodeName` | `string` |
| `buttons.xr-standard-touchpad.touchPointNodeName` | `string` |
| `buttons.xr-standard-trigger` | { `componentProperty`: `string` = "button"; `rootNodeName`: `string` = "SELECT"; `states`: `string`[]  } |
| `buttons.xr-standard-trigger.componentProperty` | `string` |
| `buttons.xr-standard-trigger.rootNodeName` | `string` |
| `buttons.xr-standard-trigger.states` | `string`[] |
| `defaultAxis` | { `maxNodeName`: `string` = "MAX"; `minNodeName`: `string` = "MIN"; `valueNodeName`: `string` = "VALUE" } |
| `defaultAxis.maxNodeName` | `string` |
| `defaultAxis.minNodeName` | `string` |
| `defaultAxis.valueNodeName` | `string` |
| `defaultButton` | { `pressedNodeName`: `string` = "PRESSED"; `unpressedNodeName`: `string` = "UNPRESSED"; `valueNodeName`: `string` = "VALUE" } |
| `defaultButton.pressedNodeName` | `string` |
| `defaultButton.unpressedNodeName` | `string` |
| `defaultButton.valueNodeName` | `string` |

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRMicrosoftMixedRealityController.ts:17

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

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:254

___

### disableAnimation

• **disableAnimation**: `boolean` = `false`

Disable the model's animation. Can be set at any time.

#### Inherited from

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[disableAnimation](WebXRAbstractMotionController.md#disableanimation)

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:261

___

### gamepadObject

• **gamepadObject**: [`IMinimalMotionControllerObject`](../interfaces/IMinimalMotionControllerObject.md)

#### Inherited from

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[gamepadObject](WebXRAbstractMotionController.md#gamepadobject)

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:292

___

### handedness

• **handedness**: [`MotionControllerHandedness`](../modules.md#motioncontrollerhandedness)

#### Inherited from

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[handedness](WebXRAbstractMotionController.md#handedness)

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:296

___

### layout

• `Protected` **layout**: [`IMotionControllerLayout`](../interfaces/IMotionControllerLayout.md)

#### Inherited from

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[layout](WebXRAbstractMotionController.md#layout)

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:288

___

### onModelLoadedObservable

• **onModelLoadedObservable**: [`Observable`](Observable.md)[`WebXRAbstractMotionController`](WebXRAbstractMotionController.md)

Observers registered here will be triggered when the model of this controller is done loading

#### Inherited from

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[onModelLoadedObservable](WebXRAbstractMotionController.md#onmodelloadedobservable)

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:265

___

### profileId

• **profileId**: `string` = `"microsoft-mixed-reality"`

The profile id of this motion controller

#### Overrides

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[profileId](WebXRAbstractMotionController.md#profileid)

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRMicrosoftMixedRealityController.ts:83

___

### rootMesh

• **rootMesh**: [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

The root mesh of the model. It is null if the model was not yet initialized

#### Inherited from

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[rootMesh](WebXRAbstractMotionController.md#rootmesh)

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:273

___

### scene

• `Protected` **scene**: [`Scene`](Scene.md)

#### Inherited from

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[scene](WebXRAbstractMotionController.md#scene)

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:286

___

### MODEL\_BASE\_URL

▪ `Static` **MODEL\_BASE\_URL**: `string` = `"https://controllers.babylonjs.com/microsoft/"`

The base url used to load the left and right controller models

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRMicrosoftMixedRealityController.ts:73

___

### MODEL\_LEFT\_FILENAME

▪ `Static` **MODEL\_LEFT\_FILENAME**: `string` = `"left.glb"`

The name of the left controller model file

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRMicrosoftMixedRealityController.ts:77

___

### MODEL\_RIGHT\_FILENAME

▪ `Static` **MODEL\_RIGHT\_FILENAME**: `string` = `"right.glb"`

The name of the right controller model file

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRMicrosoftMixedRealityController.ts:81

## Accessors

### handness

• `get` **handness**(): [`MotionControllerHandedness`](../modules.md#motioncontrollerhandedness)

Backwards compatibility due to a deeply-integrated typo

#### Returns

[`MotionControllerHandedness`](../modules.md#motioncontrollerhandedness)

#### Inherited from

WebXRAbstractMotionController.handness

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

#### Inherited from

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[_getChildByName](WebXRAbstractMotionController.md#_getchildbyname)

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:469

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

https://github.com/babylon.js/core/src/XR/motionController/webXRMicrosoftMixedRealityController.ts:89

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

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:474

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

https://github.com/babylon.js/core/src/XR/motionController/webXRMicrosoftMixedRealityController.ts:106

___

### \_processLoadedModel

▸ `Protected` **_processLoadedModel**(`_meshes`): `void`

This function will be called after the model was successfully loaded and can be used
for mesh transformations before it is available for the user

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `_meshes` | [`AbstractMesh`](AbstractMesh.md)[] | the loaded meshes |

#### Returns

`void`

#### Overrides

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[_processLoadedModel](WebXRAbstractMotionController.md#_processloadedmodel)

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRMicrosoftMixedRealityController.ts:114

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

https://github.com/babylon.js/core/src/XR/motionController/webXRMicrosoftMixedRealityController.ts:202

___

### \_updateModel

▸ `Protected` **_updateModel**(): `void`

A function executed each frame that updates the mesh (if needed)

#### Returns

`void`

#### Overrides

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[_updateModel](WebXRAbstractMotionController.md#_updatemodel)

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRMicrosoftMixedRealityController.ts:227

___

### dispose

▸ **dispose**(): `void`

Dispose this controller, the model mesh and all its components

#### Returns

`void`

#### Inherited from

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[dispose](WebXRAbstractMotionController.md#dispose)

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

#### Inherited from

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[getAllComponentsOfType](WebXRAbstractMotionController.md#getallcomponentsoftype)

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

#### Inherited from

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[getComponent](WebXRAbstractMotionController.md#getcomponent)

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:343

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

#### Inherited from

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[getComponentOfType](WebXRAbstractMotionController.md#getcomponentoftype)

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:360

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

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:368

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

#### Inherited from

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[pulse](WebXRAbstractMotionController.md#pulse)

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

#### Inherited from

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[updateFromXRFrame](WebXRAbstractMotionController.md#updatefromxrframe)

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

#### Inherited from

[WebXRAbstractMotionController](WebXRAbstractMotionController.md).[updateModel](WebXRAbstractMotionController.md#updatemodel)

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:505
