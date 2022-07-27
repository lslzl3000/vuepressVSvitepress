[@dev/core](../README.md) / [Exports](../modules.md) / WebXRControllerPointerSelection

# Class: WebXRControllerPointerSelection

A module that will enable pointer selection for motion controllers of XR Input Sources

## Hierarchy

- [`WebXRAbstractFeature`](WebXRAbstractFeature.md)

  ↳ **`WebXRControllerPointerSelection`**

## Table of contents

### Constructors

- [constructor](WebXRControllerPointerSelection.md#constructor)

### Properties

- [\_attachedController](WebXRControllerPointerSelection.md#_attachedcontroller)
- [\_controllers](WebXRControllerPointerSelection.md#_controllers)
- [\_identityMatrix](WebXRControllerPointerSelection.md#_identitymatrix)
- [\_scene](WebXRControllerPointerSelection.md#_scene)
- [\_screenCoordinatesRef](WebXRControllerPointerSelection.md#_screencoordinatesref)
- [\_tmpVectorForPickCompare](WebXRControllerPointerSelection.md#_tmpvectorforpickcompare)
- [\_viewportRef](WebXRControllerPointerSelection.md#_viewportref)
- [\_xrSessionManager](WebXRControllerPointerSelection.md#_xrsessionmanager)
- [disableAutoAttach](WebXRControllerPointerSelection.md#disableautoattach)
- [disablePointerLighting](WebXRControllerPointerSelection.md#disablepointerlighting)
- [disableSelectionMeshLighting](WebXRControllerPointerSelection.md#disableselectionmeshlighting)
- [displayLaserPointer](WebXRControllerPointerSelection.md#displaylaserpointer)
- [displaySelectionMesh](WebXRControllerPointerSelection.md#displayselectionmesh)
- [isDisposed](WebXRControllerPointerSelection.md#isdisposed)
- [laserPointerDefaultColor](WebXRControllerPointerSelection.md#laserpointerdefaultcolor)
- [laserPointerPickedColor](WebXRControllerPointerSelection.md#laserpointerpickedcolor)
- [raySelectionPredicate](WebXRControllerPointerSelection.md#rayselectionpredicate)
- [selectionMeshDefaultColor](WebXRControllerPointerSelection.md#selectionmeshdefaultcolor)
- [selectionMeshPickedColor](WebXRControllerPointerSelection.md#selectionmeshpickedcolor)
- [xrNativeFeatureName](WebXRControllerPointerSelection.md#xrnativefeaturename)
- [Name](WebXRControllerPointerSelection.md#name)
- [Version](WebXRControllerPointerSelection.md#version)
- [\_IdCounter](WebXRControllerPointerSelection.md#_idcounter)

### Accessors

- [\_utilityLayerScene](WebXRControllerPointerSelection.md#_utilitylayerscene)
- [attached](WebXRControllerPointerSelection.md#attached)

### Methods

- [\_addNewAttachObserver](WebXRControllerPointerSelection.md#_addnewattachobserver)
- [\_attachController](WebXRControllerPointerSelection.md#_attachcontroller)
- [\_attachGazeMode](WebXRControllerPointerSelection.md#_attachgazemode)
- [\_attachScreenRayMode](WebXRControllerPointerSelection.md#_attachscreenraymode)
- [\_attachTrackedPointerRayMode](WebXRControllerPointerSelection.md#_attachtrackedpointerraymode)
- [\_augmentPointerInit](WebXRControllerPointerSelection.md#_augmentpointerinit)
- [\_convertNormalToDirectionOfRay](WebXRControllerPointerSelection.md#_convertnormaltodirectionofray)
- [\_detachController](WebXRControllerPointerSelection.md#_detachcontroller)
- [\_generateNewMeshPair](WebXRControllerPointerSelection.md#_generatenewmeshpair)
- [\_onXRFrame](WebXRControllerPointerSelection.md#_onxrframe)
- [\_pickingMoved](WebXRControllerPointerSelection.md#_pickingmoved)
- [\_updatePointerDistance](WebXRControllerPointerSelection.md#_updatepointerdistance)
- [attach](WebXRControllerPointerSelection.md#attach)
- [detach](WebXRControllerPointerSelection.md#detach)
- [dispose](WebXRControllerPointerSelection.md#dispose)
- [getMeshUnderPointer](WebXRControllerPointerSelection.md#getmeshunderpointer)
- [getXRControllerByPointerId](WebXRControllerPointerSelection.md#getxrcontrollerbypointerid)
- [isCompatible](WebXRControllerPointerSelection.md#iscompatible)

## Constructors

### constructor

• **new WebXRControllerPointerSelection**(`_xrSessionManager`, `_options`)

constructs a new background remover module

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `_xrSessionManager` | [`WebXRSessionManager`](WebXRSessionManager.md) | the session manager for this module |
| `_options` | [`IWebXRControllerPointerSelectionOptions`](../interfaces/IWebXRControllerPointerSelectionOptions.md) | read-only options to be used in this module |

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[constructor](WebXRAbstractFeature.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:255

## Properties

### \_attachedController

• `Private` **\_attachedController**: `string`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:198

___

### \_controllers

• `Private` **\_controllers**: `Object` = `{}`

#### Index signature

▪ [controllerUniqueId: `string`]: { `disabledByNearInteraction`: `boolean` ; `eventListeners?`: { [event in XREventType]?: Function } ; `finalPointerUpTriggered?`: `boolean` ; `id`: `number` ; `laserPointer`: [`AbstractMesh`](AbstractMesh.md) ; `meshUnderPointer`: [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md) ; `onButtonChangedObserver?`: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`WebXRControllerComponent`](WebXRControllerComponent.md) ; `onFrameObserver?`: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)`XRFrame` ; `pick`: [`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md) ; `pointerDownTriggered?`: `boolean` ; `screenCoordinates?`: { `x`: `number` ; `y`: `number`  } ; `selectionComponent?`: [`WebXRControllerComponent`](WebXRControllerComponent.md) ; `selectionMesh`: [`AbstractMesh`](AbstractMesh.md) ; `tmpRay`: [`Ray`](Ray.md) ; `webXRCamera?`: [`WebXRCamera`](WebXRCamera.md) ; `xrController?`: [`WebXRInputSource`](WebXRInputSource.md)  }

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:174

___

### \_identityMatrix

• `Private` **\_identityMatrix**: [`Matrix`](Matrix.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:381

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:195

___

### \_screenCoordinatesRef

• `Private` **\_screenCoordinatesRef**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:382

___

### \_tmpVectorForPickCompare

• `Private` **\_tmpVectorForPickCompare**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:196

___

### \_viewportRef

• `Private` **\_viewportRef**: [`Viewport`](Viewport.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:383

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

### disablePointerLighting

• **disablePointerLighting**: `boolean` = `true`

Disable lighting on the laser pointer (so it will always be visible)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:214

___

### disableSelectionMeshLighting

• **disableSelectionMeshLighting**: `boolean` = `true`

Disable lighting on the selection mesh (so it will always be visible)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:218

___

### displayLaserPointer

• **displayLaserPointer**: `boolean` = `true`

Should the laser pointer be displayed

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:222

___

### displaySelectionMesh

• **displaySelectionMesh**: `boolean` = `true`

Should the selection mesh be displayed (The ring at the end of the laser pointer)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:226

___

### isDisposed

• **isDisposed**: `boolean` = `false`

Is this feature disposed?

#### Inherited from

[WebXRAbstractFeature](WebXRAbstractFeature.md).[isDisposed](WebXRAbstractFeature.md#isdisposed)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRAbstractFeature.ts:21

___

### laserPointerDefaultColor

• **laserPointerDefaultColor**: [`Color3`](Color3.md)

Default color of the laser pointer

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:234

___

### laserPointerPickedColor

• **laserPointerPickedColor**: [`Color3`](Color3.md)

This color will be set to the laser pointer when selection is triggered

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:230

___

### raySelectionPredicate

• **raySelectionPredicate**: (`mesh`: [`AbstractMesh`](AbstractMesh.md)) => `boolean`

#### Type declaration

▸ (`mesh`): `boolean`

Optional filter to be used for ray selection.  This predicate shares behavior with
scene.pointerMovePredicate which takes priority if it is also assigned.

##### Parameters

| Name | Type |
| :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) |

##### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:248

___

### selectionMeshDefaultColor

• **selectionMeshDefaultColor**: [`Color3`](Color3.md)

default color of the selection ring

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:238

___

### selectionMeshPickedColor

• **selectionMeshPickedColor**: [`Color3`](Color3.md)

This color will be applied to the selection ring when selection is triggered

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:242

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

▪ `Static` `Readonly` **Name**: ``"xr-controller-pointer-selection"``

The module's name

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:203

___

### Version

▪ `Static` `Readonly` **Version**: ``1``

The (Babylon) version of this module.
This is an integer representing the implementation version.
This number does not correspond to the WebXR specs version

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:209

___

### \_IdCounter

▪ `Static` `Private` **\_IdCounter**: `number` = `200`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:128

## Accessors

### \_utilityLayerScene

• `Private` `get` **_utilityLayerScene**(): [`Scene`](Scene.md)

#### Returns

[`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:496

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

▸ `Private` **_attachController**(`xrController`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `xrController` | [`WebXRInputSource`](WebXRInputSource.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:130

___

### \_attachGazeMode

▸ `Private` **_attachGazeMode**(`xrController?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `xrController?` | [`WebXRInputSource`](WebXRInputSource.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:500

___

### \_attachScreenRayMode

▸ `Private` **_attachScreenRayMode**(`xrController`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `xrController` | [`WebXRInputSource`](WebXRInputSource.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:584

___

### \_attachTrackedPointerRayMode

▸ `Private` **_attachTrackedPointerRayMode**(`xrController`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `xrController` | [`WebXRInputSource`](WebXRInputSource.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:618

___

### \_augmentPointerInit

▸ `Private` **_augmentPointerInit**(`pointerEventInit`, `id`, `screenCoordinates?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `pointerEventInit` | `PointerEventInit` |
| `id` | `number` |
| `screenCoordinates?` | `Object` |
| `screenCoordinates.x` | `number` |
| `screenCoordinates.y` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:857

___

### \_convertNormalToDirectionOfRay

▸ `Private` **_convertNormalToDirectionOfRay**(`normal`, `ray`): [`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `normal` | [`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md) |
| `ray` | [`Ray`](Ray.md) |

#### Returns

[`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:706

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

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:716

___

### \_generateNewMeshPair

▸ `Private` **_generateNewMeshPair**(`meshParent`): `Object`

#### Parameters

| Name | Type |
| :------ | :------ |
| `meshParent` | [`Node`](Node.md) |

#### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `laserPointer` | [`AbstractMesh`](AbstractMesh.md) \| [`Mesh`](Mesh.md) |
| `selectionMesh` | [`Mesh`](Mesh.md) |

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:771

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

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:385

___

### \_pickingMoved

▸ `Private` **_pickingMoved**(`oldPick`, `newPick`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `oldPick` | [`PickingInfo`](PickingInfo.md) |
| `newPick` | [`PickingInfo`](PickingInfo.md) |

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:828

___

### \_updatePointerDistance

▸ `Private` **_updatePointerDistance**(`_laserPointer`, `distance?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `_laserPointer` | [`AbstractMesh`](AbstractMesh.md) | `undefined` |
| `distance` | `number` | `100` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:848

___

### attach

▸ **attach**(): `boolean`

attach this feature
Will usually be called by the features manager

#### Returns

`boolean`

true if successful.

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[attach](WebXRAbstractFeature.md#attach)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:266

___

### detach

▸ **detach**(): `boolean`

detach this feature.
Will usually be called by the features manager

#### Returns

`boolean`

true if successful.

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[detach](WebXRAbstractFeature.md#detach)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:307

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

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:325

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

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:339

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
