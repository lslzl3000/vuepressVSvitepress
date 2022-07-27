[@dev/core](../README.md) / [Exports](../modules.md) / WebXRHitTestLegacy

# Class: WebXRHitTestLegacy

The currently-working hit-test module.
Hit test (or Ray-casting) is used to interact with the real world.
For further information read here - https://github.com/immersive-web/hit-test

## Hierarchy

- [`WebXRAbstractFeature`](WebXRAbstractFeature.md)

  ↳ **`WebXRHitTestLegacy`**

## Implements

- [`IWebXRHitTestFeature`](../interfaces/IWebXRHitTestFeature.md)[`IWebXRLegacyHitResult`](../interfaces/IWebXRLegacyHitResult.md)

## Table of contents

### Constructors

- [constructor](WebXRHitTestLegacy.md#constructor)

### Properties

- [\_direction](WebXRHitTestLegacy.md#_direction)
- [\_mat](WebXRHitTestLegacy.md#_mat)
- [\_onSelectEnabled](WebXRHitTestLegacy.md#_onselectenabled)
- [\_origin](WebXRHitTestLegacy.md#_origin)
- [\_xrSessionManager](WebXRHitTestLegacy.md#_xrsessionmanager)
- [disableAutoAttach](WebXRHitTestLegacy.md#disableautoattach)
- [isDisposed](WebXRHitTestLegacy.md#isdisposed)
- [lastNativeXRHitResults](WebXRHitTestLegacy.md#lastnativexrhitresults)
- [onHitTestResultObservable](WebXRHitTestLegacy.md#onhittestresultobservable)
- [options](WebXRHitTestLegacy.md#options)
- [xrNativeFeatureName](WebXRHitTestLegacy.md#xrnativefeaturename)
- [Name](WebXRHitTestLegacy.md#name)
- [Version](WebXRHitTestLegacy.md#version)

### Accessors

- [attached](WebXRHitTestLegacy.md#attached)

### Methods

- [\_addNewAttachObserver](WebXRHitTestLegacy.md#_addnewattachobserver)
- [\_onHitTestResults](WebXRHitTestLegacy.md#_onhittestresults)
- [\_onSelect](WebXRHitTestLegacy.md#_onselect)
- [\_onXRFrame](WebXRHitTestLegacy.md#_onxrframe)
- [attach](WebXRHitTestLegacy.md#attach)
- [detach](WebXRHitTestLegacy.md#detach)
- [dispose](WebXRHitTestLegacy.md#dispose)
- [isCompatible](WebXRHitTestLegacy.md#iscompatible)
- [XRHitTestWithRay](WebXRHitTestLegacy.md#xrhittestwithray)
- [XRHitTestWithSelectEvent](WebXRHitTestLegacy.md#xrhittestwithselectevent)

## Constructors

### constructor

• **new WebXRHitTestLegacy**(`_xrSessionManager`, `options?`)

Creates a new instance of the (legacy version) hit test feature

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `_xrSessionManager` | [`WebXRSessionManager`](WebXRSessionManager.md) | an instance of WebXRSessionManager |
| `options` | [`IWebXRLegacyHitTestOptions`](../interfaces/IWebXRLegacyHitTestOptions.md) | options to use when constructing this feature |

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[constructor](WebXRAbstractFeature.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTestLegacy.ts:87

## Properties

### \_direction

• `Private` **\_direction**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTestLegacy.ts:57

___

### \_mat

• `Private` **\_mat**: [`Matrix`](Matrix.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTestLegacy.ts:58

___

### \_onSelectEnabled

• `Private` **\_onSelectEnabled**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTestLegacy.ts:59

___

### \_origin

• `Private` **\_origin**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTestLegacy.ts:60

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

### lastNativeXRHitResults

• **lastNativeXRHitResults**: `XRHitResult`[] = `[]`

Populated with the last native XR Hit Results

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTestLegacy.ts:76

___

### onHitTestResultObservable

• **onHitTestResultObservable**: [`Observable`](Observable.md)[`IWebXRLegacyHitResult`](../interfaces/IWebXRLegacyHitResult.md)[]

Triggered when new babylon (transformed) hit test results are available

#### Implementation of

[IWebXRHitTestFeature](../interfaces/IWebXRHitTestFeature.md).[onHitTestResultObservable](../interfaces/IWebXRHitTestFeature.md#onhittestresultobservable)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTestLegacy.ts:80

___

### options

• `Readonly` **options**: [`IWebXRLegacyHitTestOptions`](../interfaces/IWebXRLegacyHitTestOptions.md) = `{}`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTestLegacy.ts:92

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

https://github.com/babylon.js/core/src/XR/features/WebXRHitTestLegacy.ts:65

___

### Version

▪ `Static` `Readonly` **Version**: ``1``

The (Babylon) version of this module.
This is an integer representing the implementation version.
This number does not correspond to the WebXR specs version

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTestLegacy.ts:71

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

### \_onHitTestResults

▸ `Private` **_onHitTestResults**(`xrResults`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `xrResults` | `XRHitResult`[] |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTestLegacy.ts:193

___

### \_onSelect

▸ `Private` **_onSelect**(`event`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | `XRInputSourceEvent` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTestLegacy.ts:214

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

https://github.com/babylon.js/core/src/XR/features/WebXRHitTestLegacy.ts:172

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

https://github.com/babylon.js/core/src/XR/features/WebXRHitTestLegacy.ts:137

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

https://github.com/babylon.js/core/src/XR/features/WebXRHitTestLegacy.ts:154

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

https://github.com/babylon.js/core/src/XR/features/WebXRHitTestLegacy.ts:167

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

___

### XRHitTestWithRay

▸ `Static` **XRHitTestWithRay**(`xrSession`, `xrRay`, `referenceSpace`, `filter?`): `Promise``XRHitResult`[]

execute a hit test with an XR Ray

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `xrSession` | `XRSession` | a native xrSession that will execute this hit test |
| `xrRay` | `XRRay` | the ray (position and direction) to use for ray-casting |
| `referenceSpace` | `XRReferenceSpace` | native XR reference space to use for the hit-test |
| `filter?` | (`result`: `XRHitResult`) => `boolean` | filter function that will filter the results |

#### Returns

`Promise``XRHitResult`[]

a promise that resolves with an array of native XR hit result in xr coordinates system

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTestLegacy.ts:108

___

### XRHitTestWithSelectEvent

▸ `Static` **XRHitTestWithSelectEvent**(`event`, `referenceSpace`): `Promise``XRHitResult`[]

Execute a hit test on the current running session using a select event returned from a transient input (such as touch)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `event` | `XRInputSourceEvent` | the (select) event to use to select with |
| `referenceSpace` | `XRReferenceSpace` | the reference space to use for this hit test |

#### Returns

`Promise``XRHitResult`[]

a promise that resolves with an array of native XR hit result in xr coordinates system

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTestLegacy.ts:121
