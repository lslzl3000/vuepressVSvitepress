[@dev/core](../README.md) / [Exports](../modules.md) / WebXRNearInteraction

# Class: WebXRNearInteraction

A module that will enable near interaction near interaction for hands and motion controllers of XR Input Sources

## Hierarchy

- [`WebXRAbstractFeature`](WebXRAbstractFeature.md)

  ↳ **`WebXRNearInteraction`**

## Table of contents

### Constructors

- [constructor](WebXRNearInteraction.md#constructor)

### Properties

- [\_attachedController](WebXRNearInteraction.md#_attachedcontroller)
- [\_controllerPickRadius](WebXRNearInteraction.md#_controllerpickradius)
- [\_controllers](WebXRNearInteraction.md#_controllers)
- [\_farInteractionFeature](WebXRNearInteraction.md#_farinteractionfeature)
- [\_hoverRadius](WebXRNearInteraction.md#_hoverradius)
- [\_nearGrabLengthScale](WebXRNearInteraction.md#_neargrablengthscale)
- [\_pickRadius](WebXRNearInteraction.md#_pickradius)
- [\_scene](WebXRNearInteraction.md#_scene)
- [\_tmpRay](WebXRNearInteraction.md#_tmpray)
- [\_xrSessionManager](WebXRNearInteraction.md#_xrsessionmanager)
- [disableAutoAttach](WebXRNearInteraction.md#disableautoattach)
- [isDisposed](WebXRNearInteraction.md#isdisposed)
- [selectionMeshDefaultColor](WebXRNearInteraction.md#selectionmeshdefaultcolor)
- [selectionMeshPickedColor](WebXRNearInteraction.md#selectionmeshpickedcolor)
- [xrNativeFeatureName](WebXRNearInteraction.md#xrnativefeaturename)
- [Name](WebXRNearInteraction.md#name)
- [Version](WebXRNearInteraction.md#version)
- [\_IdCounter](WebXRNearInteraction.md#_idcounter)

### Accessors

- [\_utilityLayerScene](WebXRNearInteraction.md#_utilitylayerscene)
- [attached](WebXRNearInteraction.md#attached)

### Methods

- [\_addNewAttachObserver](WebXRNearInteraction.md#_addnewattachobserver)
- [\_attachController](WebXRNearInteraction.md#_attachcontroller)
- [\_attachNearInteractionMode](WebXRNearInteraction.md#_attachnearinteractionmode)
- [\_controllerAvailablePredicate](WebXRNearInteraction.md#_controlleravailablepredicate)
- [\_detachController](WebXRNearInteraction.md#_detachcontroller)
- [\_generateNewTouchPointMesh](WebXRNearInteraction.md#_generatenewtouchpointmesh)
- [\_generateVisualCue](WebXRNearInteraction.md#_generatevisualcue)
- [\_handleTransitionAnimation](WebXRNearInteraction.md#_handletransitionanimation)
- [\_isControllerReadyForNearInteraction](WebXRNearInteraction.md#_iscontrollerreadyfornearinteraction)
- [\_nearGrabPredicate](WebXRNearInteraction.md#_neargrabpredicate)
- [\_nearInteractionPredicate](WebXRNearInteraction.md#_nearinteractionpredicate)
- [\_nearPickPredicate](WebXRNearInteraction.md#_nearpickpredicate)
- [\_onXRFrame](WebXRNearInteraction.md#_onxrframe)
- [\_pickWithSphere](WebXRNearInteraction.md#_pickwithsphere)
- [\_processTouchPoint](WebXRNearInteraction.md#_processtouchpoint)
- [attach](WebXRNearInteraction.md#attach)
- [detach](WebXRNearInteraction.md#detach)
- [dispose](WebXRNearInteraction.md#dispose)
- [getMeshUnderPointer](WebXRNearInteraction.md#getmeshunderpointer)
- [getXRControllerByPointerId](WebXRNearInteraction.md#getxrcontrollerbypointerid)
- [isCompatible](WebXRNearInteraction.md#iscompatible)
- [setFarInteractionFeature](WebXRNearInteraction.md#setfarinteractionfeature)
- [PickMeshWithSphere](WebXRNearInteraction.md#pickmeshwithsphere)

## Constructors

### constructor

• **new WebXRNearInteraction**(`_xrSessionManager`, `_options`)

constructs a new background remover module

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `_xrSessionManager` | [`WebXRSessionManager`](WebXRSessionManager.md) | the session manager for this module |
| `_options` | [`IWebXRNearInteractionOptions`](../interfaces/IWebXRNearInteractionOptions.md) | read-only options to be used in this module |

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[constructor](WebXRAbstractFeature.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:227

## Properties

### \_attachedController

• `Private` **\_attachedController**: `string`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:198

___

### \_controllerPickRadius

• `Private` `Readonly` **\_controllerPickRadius**: ``0.03``

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:406

___

### \_controllers

• `Private` **\_controllers**: `Object` = `{}`

#### Index signature

▪ [controllerUniqueId: `string`]: `ControllerData`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:193

___

### \_farInteractionFeature

• `Private` **\_farInteractionFeature**: [`Nullable`](../modules.md#nullable)[`WebXRControllerPointerSelection`](WebXRControllerPointerSelection.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:200

___

### \_hoverRadius

• `Private` `Readonly` **\_hoverRadius**: ``0.1``

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:404

___

### \_nearGrabLengthScale

• `Private` `Readonly` **\_nearGrabLengthScale**: ``5``

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:407

___

### \_pickRadius

• `Private` `Readonly` **\_pickRadius**: ``0.02``

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:405

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:196

___

### \_tmpRay

• `Private` **\_tmpRay**: [`Ray`](Ray.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:141

___

### \_xrSessionManager

• `Protected` **\_xrSessionManager**: [`WebXRSessionManager`](WebXRSessionManager.md)

#### Inherited from

[WebXRAbstractFeature](WebXRAbstractFeature.md).[_xrSessionManager](WebXRAbstractFeature.md#_xrsessionmanager)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRAbstractFeature.ts:37

___

### disableAutoAttach

• **disableAutoAttach**: `boolean` = `false`

Should auto-attach be disabled?

#### Inherited from

[WebXRAbstractFeature](WebXRAbstractFeature.md).[disableAutoAttach](WebXRAbstractFeature.md#disableautoattach)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRAbstractFeature.ts:26

___

### isDisposed

• **isDisposed**: `boolean` = `false`

Is this feature disposed?

#### Inherited from

[WebXRAbstractFeature](WebXRAbstractFeature.md).[isDisposed](WebXRAbstractFeature.md#isdisposed)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRAbstractFeature.ts:21

___

### selectionMeshDefaultColor

• **selectionMeshDefaultColor**: [`Color3`](Color3.md)

default color of the selection ring

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:216

___

### selectionMeshPickedColor

• **selectionMeshPickedColor**: [`Color3`](Color3.md)

This color will be applied to the selection ring when selection is triggered

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:220

___

### xrNativeFeatureName

• **xrNativeFeatureName**: `string` = `""`

The name of the native xr feature name (like anchor, hit-test, or hand-tracking)

#### Inherited from

[WebXRAbstractFeature](WebXRAbstractFeature.md).[xrNativeFeatureName](WebXRAbstractFeature.md#xrnativefeaturename)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRAbstractFeature.ts:31

___

### Name

▪ `Static` `Readonly` **Name**: ``"xr-near-interaction"``

The module's name

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:205

___

### Version

▪ `Static` `Readonly` **Version**: ``1``

The (Babylon) version of this module.
This is an integer representing the implementation version.
This number does not correspond to the WebXR specs version

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:211

___

### \_IdCounter

▪ `Static` `Private` **\_IdCounter**: `number` = `200`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:139

## Accessors

### \_utilityLayerScene

• `Private` `get` **_utilityLayerScene**(): [`Scene`](Scene.md)

#### Returns

[`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:579

___

### attached

• `get` **attached**(): `boolean`

Is this feature attached

#### Returns

`boolean`

#### Inherited from

WebXRAbstractFeature.attached

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRAbstractFeature.ts:42

## Methods

### \_addNewAttachObserver

▸ `Protected` **_addNewAttachObserver**`T`(`observable`, `callback`): `void`

This is used to register callbacks that will automatically be removed when detach is called.

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `observable` | [`Observable`](Observable.md)`T` | the observable to which the observer will be attached |
| `callback` | (`eventData`: `T`, `eventState`: [`EventState`](EventState.md)) => `void` | the callback to register |

#### Returns

`void`

#### Inherited from

[WebXRAbstractFeature](WebXRAbstractFeature.md).[_addNewAttachObserver](WebXRAbstractFeature.md#_addnewattachobserver)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRAbstractFeature.ts:113

___

### \_attachController

▸ `Private` **_attachController**(`xrController`): ``null`` \| `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `xrController` | [`WebXRInputSource`](WebXRInputSource.md) |

#### Returns

``null`` \| `void`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:143

___

### \_attachNearInteractionMode

▸ `Private` **_attachNearInteractionMode**(`xrController`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `xrController` | [`WebXRInputSource`](WebXRInputSource.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:613

___

### \_controllerAvailablePredicate

▸ `Private` **_controllerAvailablePredicate**(`mesh`, `controllerId`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) |
| `controllerId` | `string` |

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:344

___

### \_detachController

▸ `Private` **_detachController**(`xrControllerUniqueId`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `xrControllerUniqueId` | `string` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:736

___

### \_generateNewTouchPointMesh

▸ `Private` **_generateNewTouchPointMesh**(): `Object`

#### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `hydrateCollisionMeshFunction` | (`isHydration`: `boolean`) => `void` |
| `touchCollisionMesh` | [`Mesh`](Mesh.md) |
| `touchCollisionMeshFunction` | (`isTouch`: `boolean`) => `void` |

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:787

___

### \_generateVisualCue

▸ `Private` **_generateVisualCue**(): [`Mesh`](Mesh.md)

#### Returns

[`Mesh`](Mesh.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:583

___

### \_handleTransitionAnimation

▸ `Private` **_handleTransitionAnimation**(`controllerData`, `newState`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `controllerData` | `ControllerData` |
| `newState` | `ControllerOrbAnimationState` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:357

___

### \_isControllerReadyForNearInteraction

▸ `Private` **_isControllerReadyForNearInteraction**(`id`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `number` |

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:605

___

### \_nearGrabPredicate

▸ `Private` **_nearGrabPredicate**(`mesh`): `boolean`

Filter used for near interaction grab

#### Parameters

| Name | Type |
| :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) |

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:332

___

### \_nearInteractionPredicate

▸ `Private` **_nearInteractionPredicate**(`mesh`): `boolean`

Filter used for any near interaction

#### Parameters

| Name | Type |
| :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) |

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:340

___

### \_nearPickPredicate

▸ `Private` **_nearPickPredicate**(`mesh`): `boolean`

Filter used for near interaction pick and hover

#### Parameters

| Name | Type |
| :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) |

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:324

___

### \_onXRFrame

▸ `Protected` **_onXRFrame**(`_xrFrame`): `void`

Code in this function will be executed on each xrFrame received from the browser.
This function will not execute after the feature is detached.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `_xrFrame` | `XRFrame` | the current frame |

#### Returns

`void`

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[_onXRFrame](WebXRAbstractFeature.md#_onxrframe)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:427

___

### \_pickWithSphere

▸ `Private` **_pickWithSphere**(`controllerData`, `radius`, `sceneToUse`, `predicate`): [`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `controllerData` | `ControllerData` |
| `radius` | `number` |
| `sceneToUse` | [`Scene`](Scene.md) |
| `predicate` | (`mesh`: [`AbstractMesh`](AbstractMesh.md)) => `boolean` |

#### Returns

[`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:875

___

### \_processTouchPoint

▸ `Private` **_processTouchPoint**(`id`, `position`, `orientation`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `position` | [`Vector3`](Vector3.md) |
| `orientation` | [`Quaternion`](Quaternion.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:409

___

### attach

▸ **attach**(): `boolean`

Attach this feature
Will usually be called by the features manager

#### Returns

`boolean`

true if successful.

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[attach](WebXRAbstractFeature.md#attach)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:245

___

### detach

▸ **detach**(): `boolean`

Detach this feature.
Will usually be called by the features manager

#### Returns

`boolean`

true if successful.

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[detach](WebXRAbstractFeature.md#detach)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:267

___

### dispose

▸ **dispose**(): `void`

Dispose this feature and all of the resources attached

#### Returns

`void`

#### Inherited from

[WebXRAbstractFeature](WebXRAbstractFeature.md).[dispose](WebXRAbstractFeature.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRAbstractFeature.ts:93

___

### getMeshUnderPointer

▸ **getMeshUnderPointer**(`controllerId`): [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

Will get the mesh under a specific pointer.
`scene.meshUnderPointer` will only return one mesh - either left or right.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `controllerId` | `string` | the controllerId to check |

#### Returns

[`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

The mesh under pointer or null if no mesh is under the pointer

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:285

___

### getXRControllerByPointerId

▸ **getXRControllerByPointerId**(`id`): [`Nullable`](../modules.md#nullable)[`WebXRInputSource`](WebXRInputSource.md)

Get the xr controller that correlates to the pointer id in the pointer event

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `number` | the pointer id to search for |

#### Returns

[`Nullable`](../modules.md#nullable)[`WebXRInputSource`](WebXRInputSource.md)

the controller that correlates to this id or null if not found

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:299

___

### isCompatible

▸ **isCompatible**(): `boolean`

This function will be executed during before enabling the feature and can be used to not-allow enabling it.
Note that at this point the session has NOT started, so this is purely checking if the browser supports it

#### Returns

`boolean`

whether or not the feature is compatible in this environment

#### Inherited from

[WebXRAbstractFeature](WebXRAbstractFeature.md).[isCompatible](WebXRAbstractFeature.md#iscompatible)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRAbstractFeature.ts:104

___

### setFarInteractionFeature

▸ **setFarInteractionFeature**(`farInteractionFeature`): `void`

This function sets webXRControllerPointerSelection feature that will be disabled when
the hover range is reached for a mesh and will be reattached when not in hover range.
This is used to remove the selection rays when moving.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `farInteractionFeature` | [`Nullable`](../modules.md#nullable)[`WebXRControllerPointerSelection`](WebXRControllerPointerSelection.md) | the feature to disable when finger is in hover range for a mesh |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:316

___

### PickMeshWithSphere

▸ `Static` **PickMeshWithSphere**(`mesh`, `sphere`, `skipBoundingInfo?`): [`PickingInfo`](PickingInfo.md)

Picks a mesh with a sphere

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | `undefined` | the mesh to pick |
| `sphere` | [`BoundingSphere`](BoundingSphere.md) | `undefined` | picking sphere in world coordinates |
| `skipBoundingInfo` | `boolean` | `false` | a boolean indicating if we should skip the bounding info check |

#### Returns

[`PickingInfo`](PickingInfo.md)

the picking info

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:911
