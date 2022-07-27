[@dev/core](../README.md) / [Exports](../modules.md) / WebXRPlaneDetector

# Class: WebXRPlaneDetector

The plane detector is used to detect planes in the real world when in AR
For more information see https://github.com/immersive-web/real-world-geometry/

## Hierarchy

- [`WebXRAbstractFeature`](WebXRAbstractFeature.md)

  ↳ **`WebXRPlaneDetector`**

## Table of contents

### Constructors

- [constructor](WebXRPlaneDetector.md#constructor)

### Properties

- [\_detectedPlanes](WebXRPlaneDetector.md#_detectedplanes)
- [\_enabled](WebXRPlaneDetector.md#_enabled)
- [\_lastFrameDetected](WebXRPlaneDetector.md#_lastframedetected)
- [\_xrSessionManager](WebXRPlaneDetector.md#_xrsessionmanager)
- [disableAutoAttach](WebXRPlaneDetector.md#disableautoattach)
- [isDisposed](WebXRPlaneDetector.md#isdisposed)
- [onPlaneAddedObservable](WebXRPlaneDetector.md#onplaneaddedobservable)
- [onPlaneRemovedObservable](WebXRPlaneDetector.md#onplaneremovedobservable)
- [onPlaneUpdatedObservable](WebXRPlaneDetector.md#onplaneupdatedobservable)
- [xrNativeFeatureName](WebXRPlaneDetector.md#xrnativefeaturename)
- [Name](WebXRPlaneDetector.md#name)
- [Version](WebXRPlaneDetector.md#version)

### Accessors

- [attached](WebXRPlaneDetector.md#attached)

### Methods

- [\_addNewAttachObserver](WebXRPlaneDetector.md#_addnewattachobserver)
- [\_findIndexInPlaneArray](WebXRPlaneDetector.md#_findindexinplanearray)
- [\_init](WebXRPlaneDetector.md#_init)
- [\_onXRFrame](WebXRPlaneDetector.md#_onxrframe)
- [\_updatePlaneWithXRPlane](WebXRPlaneDetector.md#_updateplanewithxrplane)
- [attach](WebXRPlaneDetector.md#attach)
- [detach](WebXRPlaneDetector.md#detach)
- [dispose](WebXRPlaneDetector.md#dispose)
- [isCompatible](WebXRPlaneDetector.md#iscompatible)

## Constructors

### constructor

• **new WebXRPlaneDetector**(`_xrSessionManager`, `_options?`)

construct a new Plane Detector

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `_xrSessionManager` | [`WebXRSessionManager`](WebXRSessionManager.md) | an instance of xr Session manager |
| `_options` | [`IWebXRPlaneDetectorOptions`](../interfaces/IWebXRPlaneDetectorOptions.md) | configuration to use when constructing this feature |

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[constructor](WebXRAbstractFeature.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRPlaneDetector.ts:96

## Properties

### \_detectedPlanes

• `Private` **\_detectedPlanes**: [`IWebXRPlane`](../interfaces/IWebXRPlane.md)[] = `[]`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRPlaneDetector.ts:62

___

### \_enabled

• `Private` **\_enabled**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRPlaneDetector.ts:63

___

### \_lastFrameDetected

• `Private` **\_lastFrameDetected**: `XRPlaneSet`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRPlaneDetector.ts:64

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

### onPlaneAddedObservable

• **onPlaneAddedObservable**: [`Observable`](Observable.md)[`IWebXRPlane`](../interfaces/IWebXRPlane.md)

Observers registered here will be executed when a new plane was added to the session

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRPlaneDetector.ts:80

___

### onPlaneRemovedObservable

• **onPlaneRemovedObservable**: [`Observable`](Observable.md)[`IWebXRPlane`](../interfaces/IWebXRPlane.md)

Observers registered here will be executed when a plane is no longer detected in the session

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRPlaneDetector.ts:84

___

### onPlaneUpdatedObservable

• **onPlaneUpdatedObservable**: [`Observable`](Observable.md)[`IWebXRPlane`](../interfaces/IWebXRPlane.md)

Observers registered here will be executed when an existing plane updates (for example - expanded)
This can execute N times every frame

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRPlaneDetector.ts:89

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

▪ `Static` `Readonly` **Name**: ``"xr-plane-detection"``

The module's name

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRPlaneDetector.ts:69

___

### Version

▪ `Static` `Readonly` **Version**: ``1``

The (Babylon) version of this module.
This is an integer representing the implementation version.
This number does not correspond to the WebXR specs version

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRPlaneDetector.ts:75

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

### \_findIndexInPlaneArray

▸ `Private` **_findIndexInPlaneArray**(`xrPlane`): `number`

avoiding using Array.find for global support.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `xrPlane` | `XRPlane` | the plane to find in the array |

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRPlaneDetector.ts:237

___

### \_init

▸ `Private` **_init**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRPlaneDetector.ts:190

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

https://github.com/babylon.js/core/src/XR/features/WebXRPlaneDetector.ts:149

___

### \_updatePlaneWithXRPlane

▸ `Private` **_updatePlaneWithXRPlane**(`xrPlane`, `plane`, `xrFrame`): [`IWebXRPlane`](../interfaces/IWebXRPlane.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `xrPlane` | `XRPlane` |
| `plane` | `Partial`[`IWebXRPlane`](../interfaces/IWebXRPlane.md) |
| `xrFrame` | `XRFrame` |

#### Returns

[`IWebXRPlane`](../interfaces/IWebXRPlane.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRPlaneDetector.ts:211

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
Will usually be called by the features manager

#### Returns

`boolean`

true if successful.

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[detach](WebXRAbstractFeature.md#detach)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRPlaneDetector.ts:114

___

### dispose

▸ **dispose**(): `void`

Dispose this feature and all of the resources attached

#### Returns

`void`

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[dispose](WebXRAbstractFeature.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRPlaneDetector.ts:134

___

### isCompatible

▸ **isCompatible**(): `boolean`

Check if the needed objects are defined.
This does not mean that the feature is enabled, but that the objects needed are well defined.

#### Returns

`boolean`

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[isCompatible](WebXRAbstractFeature.md#iscompatible)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRPlaneDetector.ts:145
