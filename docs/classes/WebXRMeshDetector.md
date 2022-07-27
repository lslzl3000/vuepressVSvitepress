[@dev/core](../README.md) / [Exports](../modules.md) / WebXRMeshDetector

# Class: WebXRMeshDetector

The mesh detector is used to detect meshes in the real world when in AR

## Hierarchy

- [`WebXRAbstractFeature`](WebXRAbstractFeature.md)

  ↳ **`WebXRMeshDetector`**

## Table of contents

### Constructors

- [constructor](WebXRMeshDetector.md#constructor)

### Properties

- [\_detectedMeshes](WebXRMeshDetector.md#_detectedmeshes)
- [\_xrSessionManager](WebXRMeshDetector.md#_xrsessionmanager)
- [disableAutoAttach](WebXRMeshDetector.md#disableautoattach)
- [isDisposed](WebXRMeshDetector.md#isdisposed)
- [onMeshAddedObservable](WebXRMeshDetector.md#onmeshaddedobservable)
- [onMeshRemovedObservable](WebXRMeshDetector.md#onmeshremovedobservable)
- [onMeshUpdatedObservable](WebXRMeshDetector.md#onmeshupdatedobservable)
- [xrNativeFeatureName](WebXRMeshDetector.md#xrnativefeaturename)
- [Name](WebXRMeshDetector.md#name)
- [Version](WebXRMeshDetector.md#version)

### Accessors

- [attached](WebXRMeshDetector.md#attached)

### Methods

- [\_addNewAttachObserver](WebXRMeshDetector.md#_addnewattachobserver)
- [\_init](WebXRMeshDetector.md#_init)
- [\_onXRFrame](WebXRMeshDetector.md#_onxrframe)
- [\_updateVertexDataWithXRMesh](WebXRMeshDetector.md#_updatevertexdatawithxrmesh)
- [attach](WebXRMeshDetector.md#attach)
- [detach](WebXRMeshDetector.md#detach)
- [dispose](WebXRMeshDetector.md#dispose)
- [isCompatible](WebXRMeshDetector.md#iscompatible)

## Constructors

### constructor

• **new WebXRMeshDetector**(`_xrSessionManager`, `_options?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `_xrSessionManager` | [`WebXRSessionManager`](WebXRSessionManager.md) |
| `_options` | [`IWebXRMeshDetectorOptions`](../interfaces/IWebXRMeshDetectorOptions.md) |

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[constructor](WebXRAbstractFeature.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRMeshDetector.ts:108

## Properties

### \_detectedMeshes

• `Private` **\_detectedMeshes**: `Map``XRMesh`, [`IWebXRVertexData`](../interfaces/IWebXRVertexData.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRMeshDetector.ts:82

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

### onMeshAddedObservable

• **onMeshAddedObservable**: [`Observable`](Observable.md)[`IWebXRVertexData`](../interfaces/IWebXRVertexData.md)

Observers registered here will be executed when a new mesh was added to the session

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRMeshDetector.ts:98

___

### onMeshRemovedObservable

• **onMeshRemovedObservable**: [`Observable`](Observable.md)[`IWebXRVertexData`](../interfaces/IWebXRVertexData.md)

Observers registered here will be executed when a mesh is no longer detected in the session

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRMeshDetector.ts:102

___

### onMeshUpdatedObservable

• **onMeshUpdatedObservable**: [`Observable`](Observable.md)[`IWebXRVertexData`](../interfaces/IWebXRVertexData.md)

Observers registered here will be executed when an existing mesh updates

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRMeshDetector.ts:106

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

▪ `Static` `Readonly` **Name**: ``"xr-mesh-detection"``

The module's name

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRMeshDetector.ts:87

___

### Version

▪ `Static` `Readonly` **Version**: ``1``

The (Babylon) version of this module.
This is an integer representing the implementation version.
This number does not correspond to the WebXR specs version

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRMeshDetector.ts:93

## Accessors

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

### \_init

▸ `Private` **_init**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRMeshDetector.ts:198

___

### \_onXRFrame

▸ `Protected` **_onXRFrame**(`frame`): `void`

Code in this function will be executed on each xrFrame received from the browser.
This function will not execute after the feature is detached.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `frame` | `XRFrame` | the current frame |

#### Returns

`void`

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[_onXRFrame](WebXRAbstractFeature.md#_onxrframe)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRMeshDetector.ts:148

___

### \_updateVertexDataWithXRMesh

▸ `Private` **_updateVertexDataWithXRMesh**(`xrMesh`, `mesh`, `xrFrame`): [`IWebXRVertexData`](../interfaces/IWebXRVertexData.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `xrMesh` | `XRMesh` |
| `mesh` | `Partial`[`IWebXRVertexData`](../interfaces/IWebXRVertexData.md) |
| `xrFrame` | `XRFrame` |

#### Returns

[`IWebXRVertexData`](../interfaces/IWebXRVertexData.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRMeshDetector.ts:211

___

### attach

▸ **attach**(`force?`): `boolean`

attach this feature

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `force?` | `boolean` | should attachment be forced (even when already attached) |

#### Returns

`boolean`

true if successful, false is failed or already attached

#### Inherited from

[WebXRAbstractFeature](WebXRAbstractFeature.md).[attach](WebXRAbstractFeature.md#attach)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRAbstractFeature.ts:52

___

### detach

▸ **detach**(): `boolean`

detach this feature.

#### Returns

`boolean`

true if successful, false if failed or already detached

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[detach](WebXRAbstractFeature.md#detach)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRMeshDetector.ts:120

___

### dispose

▸ **dispose**(): `void`

Dispose this feature and all of the resources attached

#### Returns

`void`

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[dispose](WebXRAbstractFeature.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRMeshDetector.ts:141

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
