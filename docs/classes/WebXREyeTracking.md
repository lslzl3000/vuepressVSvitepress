[@dev/core](../README.md) / [Exports](../modules.md) / WebXREyeTracking

# Class: WebXREyeTracking

The WebXR Eye Tracking feature grabs eye data from the device and provides it in an easy-access format.
Currently only enabled for BabylonNative applications.

## Hierarchy

- [`WebXRAbstractFeature`](WebXRAbstractFeature.md)

  ↳ **`WebXREyeTracking`**

## Table of contents

### Constructors

- [constructor](WebXREyeTracking.md#constructor)

### Properties

- [\_gazeRay](WebXREyeTracking.md#_gazeray)
- [\_latestEyeSpace](WebXREyeTracking.md#_latesteyespace)
- [\_xrSessionManager](WebXREyeTracking.md#_xrsessionmanager)
- [disableAutoAttach](WebXREyeTracking.md#disableautoattach)
- [isDisposed](WebXREyeTracking.md#isdisposed)
- [onEyeTrackingEndedObservable](WebXREyeTracking.md#oneyetrackingendedobservable)
- [onEyeTrackingFrameUpdateObservable](WebXREyeTracking.md#oneyetrackingframeupdateobservable)
- [onEyeTrackingStartedObservable](WebXREyeTracking.md#oneyetrackingstartedobservable)
- [xrNativeFeatureName](WebXREyeTracking.md#xrnativefeaturename)
- [Name](WebXREyeTracking.md#name)
- [Version](WebXREyeTracking.md#version)

### Accessors

- [attached](WebXREyeTracking.md#attached)
- [isEyeGazeValid](WebXREyeTracking.md#iseyegazevalid)

### Methods

- [\_addNewAttachObserver](WebXREyeTracking.md#_addnewattachobserver)
- [\_eyeTrackingEndListener](WebXREyeTracking.md#_eyetrackingendlistener)
- [\_eyeTrackingStartListener](WebXREyeTracking.md#_eyetrackingstartlistener)
- [\_init](WebXREyeTracking.md#_init)
- [\_onXRFrame](WebXREyeTracking.md#_onxrframe)
- [attach](WebXREyeTracking.md#attach)
- [detach](WebXREyeTracking.md#detach)
- [dispose](WebXREyeTracking.md#dispose)
- [getEyeGaze](WebXREyeTracking.md#geteyegaze)
- [isCompatible](WebXREyeTracking.md#iscompatible)

## Constructors

### constructor

• **new WebXREyeTracking**(`_xrSessionManager`)

Creates a new instance of the XR eye tracking feature.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `_xrSessionManager` | [`WebXRSessionManager`](WebXRSessionManager.md) | An instance of WebXRSessionManager. |

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[constructor](WebXRAbstractFeature.md#constructor)

#### Defined in

packages/dev/core/src/XR/features/WebXREyeTracking.ts:45

## Properties

### \_gazeRay

• `Private` **\_gazeRay**: [`Nullable`](../modules.md#nullable)[`Ray`](Ray.md)

#### Defined in

packages/dev/core/src/XR/features/WebXREyeTracking.ts:15

___

### \_latestEyeSpace

• `Private` **\_latestEyeSpace**: [`Nullable`](../modules.md#nullable)`XRSpace`

#### Defined in

packages/dev/core/src/XR/features/WebXREyeTracking.ts:14

___

### \_xrSessionManager

• `Protected` **\_xrSessionManager**: [`WebXRSessionManager`](WebXRSessionManager.md)

#### Inherited from

[WebXRAbstractFeature](WebXRAbstractFeature.md).[_xrSessionManager](WebXRAbstractFeature.md#_xrsessionmanager)

#### Defined in

packages/dev/core/src/XR/features/WebXRAbstractFeature.ts:37

___

### disableAutoAttach

• **disableAutoAttach**: `boolean` = `false`

Should auto-attach be disabled?

#### Inherited from

[WebXRAbstractFeature](WebXRAbstractFeature.md).[disableAutoAttach](WebXRAbstractFeature.md#disableautoattach)

#### Defined in

packages/dev/core/src/XR/features/WebXRAbstractFeature.ts:26

___

### isDisposed

• **isDisposed**: `boolean` = `false`

Is this feature disposed?

#### Inherited from

[WebXRAbstractFeature](WebXRAbstractFeature.md).[isDisposed](WebXRAbstractFeature.md#isdisposed)

#### Defined in

packages/dev/core/src/XR/features/WebXRAbstractFeature.ts:21

___

### onEyeTrackingEndedObservable

• `Readonly` **onEyeTrackingEndedObservable**: [`Observable`](Observable.md)`void`

This observable will notify registered observers when eye tracking ends

#### Defined in

packages/dev/core/src/XR/features/WebXREyeTracking.ts:35

___

### onEyeTrackingFrameUpdateObservable

• `Readonly` **onEyeTrackingFrameUpdateObservable**: [`Observable`](Observable.md)[`Ray`](Ray.md)

This observable will notify registered observers on each frame that has valid tracking

#### Defined in

packages/dev/core/src/XR/features/WebXREyeTracking.ts:39

___

### onEyeTrackingStartedObservable

• `Readonly` **onEyeTrackingStartedObservable**: [`Observable`](Observable.md)[`Ray`](Ray.md)

This observable will notify registered observers when eye tracking starts

#### Defined in

packages/dev/core/src/XR/features/WebXREyeTracking.ts:31

___

### xrNativeFeatureName

• **xrNativeFeatureName**: `string` = `""`

The name of the native xr feature name (like anchor, hit-test, or hand-tracking)

#### Inherited from

[WebXRAbstractFeature](WebXRAbstractFeature.md).[xrNativeFeatureName](WebXRAbstractFeature.md#xrnativefeaturename)

#### Defined in

packages/dev/core/src/XR/features/WebXRAbstractFeature.ts:31

___

### Name

▪ `Static` `Readonly` **Name**: ``"xr-eye-tracking"``

The module's name

#### Defined in

packages/dev/core/src/XR/features/WebXREyeTracking.ts:20

___

### Version

▪ `Static` `Readonly` **Version**: ``1``

The (Babylon) version of this module.
This is an integer representing the implementation version.
This number does not correspond to the WebXR specs version

#### Defined in

packages/dev/core/src/XR/features/WebXREyeTracking.ts:26

## Accessors

### attached

• `get` **attached**(): `boolean`

Is this feature attached

#### Returns

`boolean`

#### Inherited from

WebXRAbstractFeature.attached

#### Defined in

packages/dev/core/src/XR/features/WebXRAbstractFeature.ts:42

___

### isEyeGazeValid

• `get` **isEyeGazeValid**(): `boolean`

Returns whether the gaze data is valid or not

#### Returns

`boolean`

true if the data is valid

#### Defined in

packages/dev/core/src/XR/features/WebXREyeTracking.ts:75

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

packages/dev/core/src/XR/features/WebXRAbstractFeature.ts:113

___

### \_eyeTrackingEndListener

▸ `Private` **_eyeTrackingEndListener**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/features/WebXREyeTracking.ts:120

___

### \_eyeTrackingStartListener

▸ `Private` **_eyeTrackingStartListener**(`event`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | `XREyeTrackingSourceEvent` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/features/WebXREyeTracking.ts:114

___

### \_init

▸ `Private` **_init**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/features/WebXREyeTracking.ts:126

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

packages/dev/core/src/XR/features/WebXREyeTracking.ts:87

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

packages/dev/core/src/XR/features/WebXRAbstractFeature.ts:52

___

### detach

▸ **detach**(): `boolean`

detach this feature.

#### Returns

`boolean`

true if successful, false if failed or already detached

#### Inherited from

[WebXRAbstractFeature](WebXRAbstractFeature.md).[detach](WebXRAbstractFeature.md#detach)

#### Defined in

packages/dev/core/src/XR/features/WebXRAbstractFeature.ts:78

___

### dispose

▸ **dispose**(): `void`

Dispose this feature and all of the resources attached.

#### Returns

`void`

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[dispose](WebXRAbstractFeature.md#dispose)

#### Defined in

packages/dev/core/src/XR/features/WebXREyeTracking.ts:60

___

### getEyeGaze

▸ **getEyeGaze**(): [`Nullable`](../modules.md#nullable)[`Ray`](Ray.md)

Get a reference to the gaze ray. This data is valid while eye tracking persists, and will be set to null when gaze data is no longer available

#### Returns

[`Nullable`](../modules.md#nullable)[`Ray`](Ray.md)

a reference to the gaze ray if it exists and is valid, returns null otherwise.

#### Defined in

packages/dev/core/src/XR/features/WebXREyeTracking.ts:83

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

packages/dev/core/src/XR/features/WebXRAbstractFeature.ts:104
