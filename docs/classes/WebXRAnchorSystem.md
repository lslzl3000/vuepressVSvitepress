[@dev/core](../README.md) / [Exports](../modules.md) / WebXRAnchorSystem

# Class: WebXRAnchorSystem

An implementation of the anchor system for WebXR.
For further information see https://github.com/immersive-web/anchors/

## Hierarchy

- [`WebXRAbstractFeature`](WebXRAbstractFeature.md)

  ↳ **`WebXRAnchorSystem`**

## Table of contents

### Constructors

- [constructor](WebXRAnchorSystem.md#constructor)

### Properties

- [\_futureAnchors](WebXRAnchorSystem.md#_futureanchors)
- [\_lastFrameDetected](WebXRAnchorSystem.md#_lastframedetected)
- [\_referenceSpaceForFrameAnchors](WebXRAnchorSystem.md#_referencespaceforframeanchors)
- [\_tmpQuaternion](WebXRAnchorSystem.md#_tmpquaternion)
- [\_tmpVector](WebXRAnchorSystem.md#_tmpvector)
- [\_trackedAnchors](WebXRAnchorSystem.md#_trackedanchors)
- [\_xrSessionManager](WebXRAnchorSystem.md#_xrsessionmanager)
- [disableAutoAttach](WebXRAnchorSystem.md#disableautoattach)
- [isDisposed](WebXRAnchorSystem.md#isdisposed)
- [onAnchorAddedObservable](WebXRAnchorSystem.md#onanchoraddedobservable)
- [onAnchorRemovedObservable](WebXRAnchorSystem.md#onanchorremovedobservable)
- [onAnchorUpdatedObservable](WebXRAnchorSystem.md#onanchorupdatedobservable)
- [xrNativeFeatureName](WebXRAnchorSystem.md#xrnativefeaturename)
- [Name](WebXRAnchorSystem.md#name)
- [Version](WebXRAnchorSystem.md#version)

### Accessors

- [anchors](WebXRAnchorSystem.md#anchors)
- [attached](WebXRAnchorSystem.md#attached)
- [referenceSpaceForFrameAnchors](WebXRAnchorSystem.md#referencespaceforframeanchors)

### Methods

- [\_addNewAttachObserver](WebXRAnchorSystem.md#_addnewattachobserver)
- [\_createAnchorAtTransformation](WebXRAnchorSystem.md#_createanchorattransformation)
- [\_findIndexInAnchorArray](WebXRAnchorSystem.md#_findindexinanchorarray)
- [\_onXRFrame](WebXRAnchorSystem.md#_onxrframe)
- [\_populateTmpTransformation](WebXRAnchorSystem.md#_populatetmptransformation)
- [\_updateAnchorWithXRFrame](WebXRAnchorSystem.md#_updateanchorwithxrframe)
- [addAnchorAtPositionAndRotationAsync](WebXRAnchorSystem.md#addanchoratpositionandrotationasync)
- [addAnchorPointUsingHitTestResultAsync](WebXRAnchorSystem.md#addanchorpointusinghittestresultasync)
- [attach](WebXRAnchorSystem.md#attach)
- [detach](WebXRAnchorSystem.md#detach)
- [dispose](WebXRAnchorSystem.md#dispose)
- [isCompatible](WebXRAnchorSystem.md#iscompatible)

## Constructors

### constructor

• **new WebXRAnchorSystem**(`_xrSessionManager`, `_options?`)

constructs a new anchor system

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `_xrSessionManager` | [`WebXRSessionManager`](WebXRSessionManager.md) | an instance of WebXRSessionManager |
| `_options` | [`IWebXRAnchorSystemOptions`](../interfaces/IWebXRAnchorSystemOptions.md) | configuration object for this feature |

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[constructor](WebXRAbstractFeature.md#constructor)

#### Defined in

packages/dev/core/src/XR/features/WebXRAnchorSystem.ts:137

## Properties

### \_futureAnchors

• `Private` **\_futureAnchors**: `IWebXRFutureAnchor`[] = `[]`

#### Defined in

packages/dev/core/src/XR/features/WebXRAnchorSystem.ts:97

___

### \_lastFrameDetected

• `Private` **\_lastFrameDetected**: `XRAnchorSet`

#### Defined in

packages/dev/core/src/XR/features/WebXRAnchorSystem.ts:91

___

### \_referenceSpaceForFrameAnchors

• `Private` **\_referenceSpaceForFrameAnchors**: `XRReferenceSpace`

#### Defined in

packages/dev/core/src/XR/features/WebXRAnchorSystem.ts:95

___

### \_tmpQuaternion

• `Private` **\_tmpQuaternion**: [`Quaternion`](Quaternion.md)

#### Defined in

packages/dev/core/src/XR/features/WebXRAnchorSystem.ts:143

___

### \_tmpVector

• `Private` **\_tmpVector**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/XR/features/WebXRAnchorSystem.ts:142

___

### \_trackedAnchors

• `Private` **\_trackedAnchors**: [`IWebXRAnchor`](../interfaces/IWebXRAnchor.md)[] = `[]`

#### Defined in

packages/dev/core/src/XR/features/WebXRAnchorSystem.ts:93

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

### onAnchorAddedObservable

• **onAnchorAddedObservable**: [`Observable`](Observable.md)[`IWebXRAnchor`](../interfaces/IWebXRAnchor.md)

Observers registered here will be executed when a new anchor was added to the session

#### Defined in

packages/dev/core/src/XR/features/WebXRAnchorSystem.ts:113

___

### onAnchorRemovedObservable

• **onAnchorRemovedObservable**: [`Observable`](Observable.md)[`IWebXRAnchor`](../interfaces/IWebXRAnchor.md)

Observers registered here will be executed when an anchor was removed from the session

#### Defined in

packages/dev/core/src/XR/features/WebXRAnchorSystem.ts:117

___

### onAnchorUpdatedObservable

• **onAnchorUpdatedObservable**: [`Observable`](Observable.md)[`IWebXRAnchor`](../interfaces/IWebXRAnchor.md)

Observers registered here will be executed when an existing anchor updates
This can execute N times every frame

#### Defined in

packages/dev/core/src/XR/features/WebXRAnchorSystem.ts:122

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

▪ `Static` `Readonly` **Name**: ``"xr-anchor-system"``

The module's name

#### Defined in

packages/dev/core/src/XR/features/WebXRAnchorSystem.ts:102

___

### Version

▪ `Static` `Readonly` **Version**: ``1``

The (Babylon) version of this module.
This is an integer representing the implementation version.
This number does not correspond to the WebXR specs version

#### Defined in

packages/dev/core/src/XR/features/WebXRAnchorSystem.ts:108

## Accessors

### anchors

• `get` **anchors**(): [`IWebXRAnchor`](../interfaces/IWebXRAnchor.md)[]

Get the list of anchors currently being tracked by the system

#### Returns

[`IWebXRAnchor`](../interfaces/IWebXRAnchor.md)[]

#### Defined in

packages/dev/core/src/XR/features/WebXRAnchorSystem.ts:247

___

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

### referenceSpaceForFrameAnchors

• `set` **referenceSpaceForFrameAnchors**(`referenceSpace`): `void`

Set the reference space to use for anchor creation, when not using a hit test.
Will default to the session's reference space if not defined

#### Parameters

| Name | Type |
| :------ | :------ |
| `referenceSpace` | `XRReferenceSpace` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/features/WebXRAnchorSystem.ts:128

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

### \_createAnchorAtTransformation

▸ `Private` **_createAnchorAtTransformation**(`xrTransformation`, `xrFrame`): `Promise``XRAnchor`

#### Parameters

| Name | Type |
| :------ | :------ |
| `xrTransformation` | `XRRigidTransform` |
| `xrFrame` | `XRFrame` |

#### Returns

`Promise``XRAnchor`

#### Defined in

packages/dev/core/src/XR/features/WebXRAnchorSystem.ts:398

___

### \_findIndexInAnchorArray

▸ `Private` **_findIndexInAnchorArray**(`xrAnchor`): `number`

avoiding using Array.find for global support.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `xrAnchor` | `XRAnchor` | the plane to find in the array |

#### Returns

`number`

#### Defined in

packages/dev/core/src/XR/features/WebXRAnchorSystem.ts:369

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

packages/dev/core/src/XR/features/WebXRAnchorSystem.ts:292

___

### \_populateTmpTransformation

▸ `Private` **_populateTmpTransformation**(`position`, `rotationQuaternion`): `Object`

#### Parameters

| Name | Type |
| :------ | :------ |
| `position` | [`Vector3`](Vector3.md) |
| `rotationQuaternion` | [`Quaternion`](Quaternion.md) |

#### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `position` | [`Vector3`](Vector3.md) |
| `rotationQuaternion` | [`Quaternion`](Quaternion.md) |

#### Defined in

packages/dev/core/src/XR/features/WebXRAnchorSystem.ts:145

___

### \_updateAnchorWithXRFrame

▸ `Private` **_updateAnchorWithXRFrame**(`xrAnchor`, `anchor`, `xrFrame`): [`IWebXRAnchor`](../interfaces/IWebXRAnchor.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `xrAnchor` | `XRAnchor` |
| `anchor` | `Partial`[`IWebXRAnchor`](../interfaces/IWebXRAnchor.md) |
| `xrFrame` | `XRFrame` |

#### Returns

[`IWebXRAnchor`](../interfaces/IWebXRAnchor.md)

#### Defined in

packages/dev/core/src/XR/features/WebXRAnchorSystem.ts:378

___

### addAnchorAtPositionAndRotationAsync

▸ **addAnchorAtPositionAndRotationAsync**(`position`, `rotationQuaternion?`, `forceCreateInCurrentFrame?`): `Promise`[`IWebXRAnchor`](../interfaces/IWebXRAnchor.md)

Add a new anchor at a specific position and rotation
This function will add a new anchor per default in the next available frame. Unless forced, the createAnchor function
will be called in the next xrFrame loop to make sure that the anchor can be created correctly.
An anchor is tracked only after it is added to the trackerAnchors in xrFrame. The promise returned here does not yet guaranty that.
Use onAnchorAddedObservable to get newly added anchors if you require tracking guaranty.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `position` | [`Vector3`](Vector3.md) | `undefined` | the position in which to add an anchor |
| `rotationQuaternion` | [`Quaternion`](Quaternion.md) | `undefined` | an optional rotation for the anchor transformation |
| `forceCreateInCurrentFrame` | `boolean` | `false` | force the creation of this anchor in the current frame. Must be called inside xrFrame loop! |

#### Returns

`Promise`[`IWebXRAnchor`](../interfaces/IWebXRAnchor.md)

A promise that fulfills when babylon has created the corresponding WebXRAnchor object and tracking has begun

#### Defined in

packages/dev/core/src/XR/features/WebXRAnchorSystem.ts:215

___

### addAnchorPointUsingHitTestResultAsync

▸ **addAnchorPointUsingHitTestResultAsync**(`hitTestResult`, `position?`, `rotationQuaternion?`): `Promise`[`IWebXRAnchor`](../interfaces/IWebXRAnchor.md)

Create a new anchor point using a hit test result at a specific point in the scene
An anchor is tracked only after it is added to the trackerAnchors in xrFrame. The promise returned here does not yet guaranty that.
Use onAnchorAddedObservable to get newly added anchors if you require tracking guaranty.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `hitTestResult` | [`IWebXRHitResult`](../interfaces/IWebXRHitResult.md) | The hit test result to use for this anchor creation |
| `position` | [`Vector3`](Vector3.md) | an optional position offset for this anchor |
| `rotationQuaternion` | [`Quaternion`](Quaternion.md) | an optional rotation offset for this anchor |

#### Returns

`Promise`[`IWebXRAnchor`](../interfaces/IWebXRAnchor.md)

A promise that fulfills when babylon has created the corresponding WebXRAnchor object and tracking has begun

#### Defined in

packages/dev/core/src/XR/features/WebXRAnchorSystem.ts:169

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
Will usually be called by the features manager

#### Returns

`boolean`

true if successful.

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[detach](WebXRAbstractFeature.md#detach)

#### Defined in

packages/dev/core/src/XR/features/WebXRAnchorSystem.ts:257

___

### dispose

▸ **dispose**(): `void`

Dispose this feature and all of the resources attached

#### Returns

`void`

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[dispose](WebXRAbstractFeature.md#dispose)

#### Defined in

packages/dev/core/src/XR/features/WebXRAnchorSystem.ts:284

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
