[@dev/core](../README.md) / [Exports](../modules.md) / WebXRHitTest

# Class: WebXRHitTest

The currently-working hit-test module.
Hit test (or Ray-casting) is used to interact with the real world.
For further information read here - https://github.com/immersive-web/hit-test

Tested on chrome (mobile) 80.

## Hierarchy

- [`WebXRAbstractFeature`](WebXRAbstractFeature.md)

  ↳ **`WebXRHitTest`**

## Implements

- [`IWebXRHitTestFeature`](../interfaces/IWebXRHitTestFeature.md)[`IWebXRHitResult`](../interfaces/IWebXRHitResult.md)

## Table of contents

### Constructors

- [constructor](WebXRHitTest.md#constructor)

### Properties

- [\_tmpMat](WebXRHitTest.md#_tmpmat)
- [\_tmpPos](WebXRHitTest.md#_tmppos)
- [\_tmpQuat](WebXRHitTest.md#_tmpquat)
- [\_transientXrHitTestSource](WebXRHitTest.md#_transientxrhittestsource)
- [\_xrHitTestSource](WebXRHitTest.md#_xrhittestsource)
- [\_xrSessionManager](WebXRHitTest.md#_xrsessionmanager)
- [autoCloneTransformation](WebXRHitTest.md#autoclonetransformation)
- [disableAutoAttach](WebXRHitTest.md#disableautoattach)
- [isDisposed](WebXRHitTest.md#isdisposed)
- [onHitTestResultObservable](WebXRHitTest.md#onhittestresultobservable)
- [options](WebXRHitTest.md#options)
- [paused](WebXRHitTest.md#paused)
- [xrNativeFeatureName](WebXRHitTest.md#xrnativefeaturename)
- [Name](WebXRHitTest.md#name)
- [Version](WebXRHitTest.md#version)

### Accessors

- [attached](WebXRHitTest.md#attached)

### Methods

- [\_addNewAttachObserver](WebXRHitTest.md#_addnewattachobserver)
- [\_initHitTestSource](WebXRHitTest.md#_inithittestsource)
- [\_onXRFrame](WebXRHitTest.md#_onxrframe)
- [\_processWebXRHitTestResult](WebXRHitTest.md#_processwebxrhittestresult)
- [attach](WebXRHitTest.md#attach)
- [detach](WebXRHitTest.md#detach)
- [dispose](WebXRHitTest.md#dispose)
- [isCompatible](WebXRHitTest.md#iscompatible)

## Constructors

### constructor

• **new WebXRHitTest**(`_xrSessionManager`, `options?`)

Creates a new instance of the hit test feature

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `_xrSessionManager` | [`WebXRSessionManager`](WebXRSessionManager.md) | an instance of WebXRSessionManager |
| `options` | [`IWebXRHitTestOptions`](../interfaces/IWebXRHitTestOptions.md) | options to use when constructing this feature |

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[constructor](WebXRAbstractFeature.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTest.ts:143

## Properties

### \_tmpMat

• `Private` **\_tmpMat**: [`Matrix`](Matrix.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTest.ts:81

___

### \_tmpPos

• `Private` **\_tmpPos**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTest.ts:82

___

### \_tmpQuat

• `Private` **\_tmpQuat**: [`Quaternion`](Quaternion.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTest.ts:83

___

### \_transientXrHitTestSource

• `Private` **\_transientXrHitTestSource**: [`Nullable`](../modules.md#nullable)`XRTransientInputHitTestSource`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTest.ts:84

___

### \_xrHitTestSource

• `Private` **\_xrHitTestSource**: [`Nullable`](../modules.md#nullable)`XRHitTestSource`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTest.ts:86

___

### \_xrSessionManager

• `Protected` **\_xrSessionManager**: [`WebXRSessionManager`](WebXRSessionManager.md)

#### Inherited from

[WebXRAbstractFeature](WebXRAbstractFeature.md).[_xrSessionManager](WebXRAbstractFeature.md#_xrsessionmanager)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRAbstractFeature.ts:37

___

### autoCloneTransformation

• **autoCloneTransformation**: `boolean` = `false`

When set to true, each hit test will have its own position/rotation objects
When set to false, position and rotation objects will be reused for each hit test. It is expected that
the developers will clone them or copy them as they see fit.

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTest.ts:127

___

### disableAutoAttach

• **disableAutoAttach**: `boolean` = `false`

Should auto-attach be disabled?

#### Implementation of

[IWebXRHitTestFeature](../interfaces/IWebXRHitTestFeature.md).[disableAutoAttach](../interfaces/IWebXRHitTestFeature.md#disableautoattach)

#### Inherited from

[WebXRAbstractFeature](WebXRAbstractFeature.md).[disableAutoAttach](WebXRAbstractFeature.md#disableautoattach)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRAbstractFeature.ts:26

___

### isDisposed

• **isDisposed**: `boolean` = `false`

Is this feature disposed?

#### Implementation of

[IWebXRHitTestFeature](../interfaces/IWebXRHitTestFeature.md).[isDisposed](../interfaces/IWebXRHitTestFeature.md#isdisposed)

#### Inherited from

[WebXRAbstractFeature](WebXRAbstractFeature.md).[isDisposed](WebXRAbstractFeature.md#isdisposed)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRAbstractFeature.ts:21

___

### onHitTestResultObservable

• **onHitTestResultObservable**: [`Observable`](Observable.md)[`IWebXRHitResult`](../interfaces/IWebXRHitResult.md)[]

Triggered when new babylon (transformed) hit test results are available
Note - this will be called when results come back from the device. It can be an empty array!!

#### Implementation of

[IWebXRHitTestFeature](../interfaces/IWebXRHitTestFeature.md).[onHitTestResultObservable](../interfaces/IWebXRHitTestFeature.md#onhittestresultobservable)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTest.ts:132

___

### options

• `Readonly` **options**: [`IWebXRHitTestOptions`](../interfaces/IWebXRHitTestOptions.md) = `{}`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTest.ts:148

___

### paused

• **paused**: `boolean` = `false`

Use this to temporarily pause hit test checks.

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTest.ts:136

___

### xrNativeFeatureName

• **xrNativeFeatureName**: `string` = `""`

The name of the native xr feature name (like anchor, hit-test, or hand-tracking)

#### Implementation of

[IWebXRHitTestFeature](../interfaces/IWebXRHitTestFeature.md).[xrNativeFeatureName](../interfaces/IWebXRHitTestFeature.md#xrnativefeaturename)

#### Inherited from

[WebXRAbstractFeature](WebXRAbstractFeature.md).[xrNativeFeatureName](WebXRAbstractFeature.md#xrnativefeaturename)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRAbstractFeature.ts:31

___

### Name

▪ `Static` `Readonly` **Name**: ``"xr-hit-test"``

The module's name

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTest.ts:114

___

### Version

▪ `Static` `Readonly` **Version**: ``2``

The (Babylon) version of this module.
This is an integer representing the implementation version.
This number does not correspond to the WebXR specs version

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTest.ts:120

## Accessors

### attached

• `get` **attached**(): `boolean`

Is this feature attached

#### Returns

`boolean`

#### Implementation of

[IWebXRHitTestFeature](../interfaces/IWebXRHitTestFeature.md).[attached](../interfaces/IWebXRHitTestFeature.md#attached)

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

### \_initHitTestSource

▸ `Private` **_initHitTestSource**(`referenceSpace`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `referenceSpace` | `XRReferenceSpace` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTest.ts:87

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

https://github.com/babylon.js/core/src/XR/features/WebXRHitTest.ts:221

___

### \_processWebXRHitTestResult

▸ `Private` **_processWebXRHitTestResult**(`hitTestResults`, `inputSource?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `hitTestResults` | `XRHitTestResult`[] |
| `inputSource?` | `XRInputSource` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTest.ts:240

___

### attach

▸ **attach**(): `boolean`

attach this feature
Will usually be called by the features manager

#### Returns

`boolean`

true if successful.

#### Implementation of

[IWebXRHitTestFeature](../interfaces/IWebXRHitTestFeature.md).[attach](../interfaces/IWebXRHitTestFeature.md#attach)

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[attach](WebXRAbstractFeature.md#attach)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTest.ts:161

___

### detach

▸ **detach**(): `boolean`

detach this feature.
Will usually be called by the features manager

#### Returns

`boolean`

true if successful.

#### Implementation of

[IWebXRHitTestFeature](../interfaces/IWebXRHitTestFeature.md).[detach](../interfaces/IWebXRHitTestFeature.md#detach)

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[detach](WebXRAbstractFeature.md#detach)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTest.ts:197

___

### dispose

▸ **dispose**(): `void`

Dispose this feature and all of the resources attached

#### Returns

`void`

#### Implementation of

[IWebXRHitTestFeature](../interfaces/IWebXRHitTestFeature.md).[dispose](../interfaces/IWebXRHitTestFeature.md#dispose)

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[dispose](WebXRAbstractFeature.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTest.ts:216

___

### isCompatible

▸ **isCompatible**(): `boolean`

This function will be executed during before enabling the feature and can be used to not-allow enabling it.
Note that at this point the session has NOT started, so this is purely checking if the browser supports it

#### Returns

`boolean`

whether or not the feature is compatible in this environment

#### Implementation of

[IWebXRHitTestFeature](../interfaces/IWebXRHitTestFeature.md).[isCompatible](../interfaces/IWebXRHitTestFeature.md#iscompatible)

#### Inherited from

[WebXRAbstractFeature](WebXRAbstractFeature.md).[isCompatible](WebXRAbstractFeature.md#iscompatible)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRAbstractFeature.ts:104
