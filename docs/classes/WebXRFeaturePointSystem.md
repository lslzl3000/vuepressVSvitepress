[@dev/core](../README.md) / [Exports](../modules.md) / WebXRFeaturePointSystem

# Class: WebXRFeaturePointSystem

The feature point system is used to detect feature points from real world geometry.
This feature is currently experimental and only supported on BabylonNative, and should not be used in the browser.
The newly introduced API can be seen in webxr.nativeextensions.d.ts and described in FeaturePoints.md.

## Hierarchy

- [`WebXRAbstractFeature`](WebXRAbstractFeature.md)

  ↳ **`WebXRFeaturePointSystem`**

## Table of contents

### Constructors

- [constructor](WebXRFeaturePointSystem.md#constructor)

### Properties

- [\_enabled](WebXRFeaturePointSystem.md#_enabled)
- [\_featurePointCloud](WebXRFeaturePointSystem.md#_featurepointcloud)
- [\_xrSessionManager](WebXRFeaturePointSystem.md#_xrsessionmanager)
- [disableAutoAttach](WebXRFeaturePointSystem.md#disableautoattach)
- [isDisposed](WebXRFeaturePointSystem.md#isdisposed)
- [onFeaturePointsAddedObservable](WebXRFeaturePointSystem.md#onfeaturepointsaddedobservable)
- [onFeaturePointsUpdatedObservable](WebXRFeaturePointSystem.md#onfeaturepointsupdatedobservable)
- [xrNativeFeatureName](WebXRFeaturePointSystem.md#xrnativefeaturename)
- [Name](WebXRFeaturePointSystem.md#name)
- [Version](WebXRFeaturePointSystem.md#version)

### Accessors

- [attached](WebXRFeaturePointSystem.md#attached)
- [featurePointCloud](WebXRFeaturePointSystem.md#featurepointcloud)

### Methods

- [\_addNewAttachObserver](WebXRFeaturePointSystem.md#_addnewattachobserver)
- [\_init](WebXRFeaturePointSystem.md#_init)
- [\_onXRFrame](WebXRFeaturePointSystem.md#_onxrframe)
- [attach](WebXRFeaturePointSystem.md#attach)
- [detach](WebXRFeaturePointSystem.md#detach)
- [dispose](WebXRFeaturePointSystem.md#dispose)
- [isCompatible](WebXRFeaturePointSystem.md#iscompatible)

## Constructors

### constructor

• **new WebXRFeaturePointSystem**(`_xrSessionManager`)

construct the feature point system

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `_xrSessionManager` | [`WebXRSessionManager`](WebXRSessionManager.md) | an instance of xr Session manager |

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[constructor](WebXRAbstractFeature.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRFeaturePointSystem.ts:62

## Properties

### \_enabled

• `Private` **\_enabled**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRFeaturePointSystem.ts:28

___

### \_featurePointCloud

• `Private` **\_featurePointCloud**: [`IWebXRFeaturePoint`](../interfaces/IWebXRFeaturePoint.md)[] = `[]`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRFeaturePointSystem.ts:29

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

### onFeaturePointsAddedObservable

• `Readonly` **onFeaturePointsAddedObservable**: [`Observable`](Observable.md)`number`[]

Observers registered here will be executed whenever new feature points are added (on XRFrame while the session is tracking).
Will notify the observers about which feature points have been added.

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRFeaturePointSystem.ts:45

___

### onFeaturePointsUpdatedObservable

• `Readonly` **onFeaturePointsUpdatedObservable**: [`Observable`](Observable.md)`number`[]

Observers registered here will be executed whenever a feature point has been updated (on XRFrame while the session is tracking).
Will notify the observers about which feature points have been updated.

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRFeaturePointSystem.ts:50

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

▪ `Static` `Readonly` **Name**: ``"xr-feature-points"``

The module's name

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRFeaturePointSystem.ts:34

___

### Version

▪ `Static` `Readonly` **Version**: ``1``

The (Babylon) version of this module.
This is an integer representing the implementation version.
This number does not correspond to the WebXR specs version

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRFeaturePointSystem.ts:40

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

___

### featurePointCloud

• `get` **featurePointCloud**(): [`IWebXRFeaturePoint`](../interfaces/IWebXRFeaturePoint.md)[]

The current feature point cloud maintained across frames.

#### Returns

[`IWebXRFeaturePoint`](../interfaces/IWebXRFeaturePoint.md)[]

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRFeaturePointSystem.ts:54

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

Initializes the feature. If the feature point feature is not available for this environment do not mark the feature as enabled.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRFeaturePointSystem.ts:154

___

### \_onXRFrame

▸ `Protected` **_onXRFrame**(`frame`): `void`

On receiving a new XR frame if this feature is attached notify observers new feature point data is available.

#### Parameters

| Name | Type |
| :------ | :------ |
| `frame` | `XRFrame` |

#### Returns

`void`

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[_onXRFrame](WebXRAbstractFeature.md#_onxrframe)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRFeaturePointSystem.ts:104

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

Detach this feature.
Will usually be called by the features manager

#### Returns

`boolean`

true if successful.

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[detach](WebXRAbstractFeature.md#detach)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRFeaturePointSystem.ts:80

___

### dispose

▸ **dispose**(): `void`

Dispose this feature and all of the resources attached

#### Returns

`void`

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[dispose](WebXRAbstractFeature.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRFeaturePointSystem.ts:92

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
