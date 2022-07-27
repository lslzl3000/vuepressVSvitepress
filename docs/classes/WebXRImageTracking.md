[@dev/core](../README.md) / [Exports](../modules.md) / WebXRImageTracking

# Class: WebXRImageTracking

Image tracking for immersive AR sessions.
Providing a list of images and their estimated widths will enable tracking those images in the real world.

## Hierarchy

- [`WebXRAbstractFeature`](WebXRAbstractFeature.md)

  ↳ **`WebXRImageTracking`**

## Table of contents

### Constructors

- [constructor](WebXRImageTracking.md#constructor)

### Properties

- [\_originalTrackingRequest](WebXRImageTracking.md#_originaltrackingrequest)
- [\_trackableScoreStatus](WebXRImageTracking.md#_trackablescorestatus)
- [\_trackedImages](WebXRImageTracking.md#_trackedimages)
- [\_xrSessionManager](WebXRImageTracking.md#_xrsessionmanager)
- [disableAutoAttach](WebXRImageTracking.md#disableautoattach)
- [isDisposed](WebXRImageTracking.md#isdisposed)
- [onTrackableImageFoundObservable](WebXRImageTracking.md#ontrackableimagefoundobservable)
- [onTrackedImageUpdatedObservable](WebXRImageTracking.md#ontrackedimageupdatedobservable)
- [onUntrackableImageFoundObservable](WebXRImageTracking.md#onuntrackableimagefoundobservable)
- [options](WebXRImageTracking.md#options)
- [xrNativeFeatureName](WebXRImageTracking.md#xrnativefeaturename)
- [Name](WebXRImageTracking.md#name)
- [Version](WebXRImageTracking.md#version)

### Accessors

- [attached](WebXRImageTracking.md#attached)

### Methods

- [\_addNewAttachObserver](WebXRImageTracking.md#_addnewattachobserver)
- [\_checkScoresAsync](WebXRImageTracking.md#_checkscoresasync)
- [\_onXRFrame](WebXRImageTracking.md#_onxrframe)
- [attach](WebXRImageTracking.md#attach)
- [detach](WebXRImageTracking.md#detach)
- [dispose](WebXRImageTracking.md#dispose)
- [getTrackedImageById](WebXRImageTracking.md#gettrackedimagebyid)
- [getXRSessionInitExtension](WebXRImageTracking.md#getxrsessioninitextension)
- [isCompatible](WebXRImageTracking.md#iscompatible)

## Constructors

### constructor

• **new WebXRImageTracking**(`_xrSessionManager`, `options`)

constructs the image tracking feature

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `_xrSessionManager` | [`WebXRSessionManager`](WebXRSessionManager.md) | the session manager for this module |
| `options` | [`IWebXRImageTrackingOptions`](../interfaces/IWebXRImageTrackingOptions.md) | read-only options to be used in this module |

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[constructor](WebXRAbstractFeature.md#constructor)

#### Defined in

packages/dev/core/src/XR/features/WebXRImageTracking.ts:114

## Properties

### \_originalTrackingRequest

• `Private` **\_originalTrackingRequest**: `XRTrackedImageInit`[]

#### Defined in

packages/dev/core/src/XR/features/WebXRImageTracking.ts:107

___

### \_trackableScoreStatus

• `Private` **\_trackableScoreStatus**: `ImageTrackingScoreStatus` = `ImageTrackingScoreStatus.NotReceived`

#### Defined in

packages/dev/core/src/XR/features/WebXRImageTracking.ts:104

___

### \_trackedImages

• `Private` **\_trackedImages**: [`IWebXRTrackedImage`](../interfaces/IWebXRTrackedImage.md)[] = `[]`

#### Defined in

packages/dev/core/src/XR/features/WebXRImageTracking.ts:105

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

### onTrackableImageFoundObservable

• **onTrackableImageFoundObservable**: [`Observable`](Observable.md)[`IWebXRTrackedImage`](../interfaces/IWebXRTrackedImage.md)

An image was deemed trackable, and the system will start tracking it.

#### Defined in

packages/dev/core/src/XR/features/WebXRImageTracking.ts:98

___

### onTrackedImageUpdatedObservable

• **onTrackedImageUpdatedObservable**: [`Observable`](Observable.md)[`IWebXRTrackedImage`](../interfaces/IWebXRTrackedImage.md)

The image was found and its state was updated.

#### Defined in

packages/dev/core/src/XR/features/WebXRImageTracking.ts:102

___

### onUntrackableImageFoundObservable

• **onUntrackableImageFoundObservable**: [`Observable`](Observable.md)`number`

This will be triggered if the underlying system deems an image untrackable.
The index is the index of the image from the array used to initialize the feature.

#### Defined in

packages/dev/core/src/XR/features/WebXRImageTracking.ts:94

___

### options

• `Readonly` **options**: [`IWebXRImageTrackingOptions`](../interfaces/IWebXRImageTrackingOptions.md)

#### Defined in

packages/dev/core/src/XR/features/WebXRImageTracking.ts:119

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

▪ `Static` `Readonly` **Name**: ``"xr-image-tracking"``

The module's name

#### Defined in

packages/dev/core/src/XR/features/WebXRImageTracking.ts:82

___

### Version

▪ `Static` `Readonly` **Version**: ``1``

The (Babylon) version of this module.
This is an integer representing the implementation version.
This number does not correspond to the WebXR specs version

#### Defined in

packages/dev/core/src/XR/features/WebXRImageTracking.ts:88

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

### \_checkScoresAsync

▸ `Private` **_checkScoresAsync**(): `Promise``void`

#### Returns

`Promise``void`

#### Defined in

packages/dev/core/src/XR/features/WebXRImageTracking.ts:258

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

packages/dev/core/src/XR/features/WebXRImageTracking.ts:204

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

packages/dev/core/src/XR/features/WebXRImageTracking.ts:131

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

packages/dev/core/src/XR/features/WebXRImageTracking.ts:141

___

### dispose

▸ **dispose**(): `void`

Dispose this feature and all of the resources attached

#### Returns

`void`

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[dispose](WebXRAbstractFeature.md#dispose)

#### Defined in

packages/dev/core/src/XR/features/WebXRImageTracking.ts:158

___

### getTrackedImageById

▸ **getTrackedImageById**(`id`): [`Nullable`](../modules.md#nullable)[`IWebXRTrackedImage`](../interfaces/IWebXRTrackedImage.md)

Get a tracked image by its ID.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `number` | the id of the image to load (position in the init array) |

#### Returns

[`Nullable`](../modules.md#nullable)[`IWebXRTrackedImage`](../interfaces/IWebXRTrackedImage.md)

a trackable image, if exists in this location

#### Defined in

packages/dev/core/src/XR/features/WebXRImageTracking.ts:151

___

### getXRSessionInitExtension

▸ **getXRSessionInitExtension**(): `Promise``Partial``XRSessionInit`

Extends the session init object if needed

#### Returns

`Promise``Partial``XRSessionInit`

augmentation object fo the xr session init object.

#### Defined in

packages/dev/core/src/XR/features/WebXRImageTracking.ts:173

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
