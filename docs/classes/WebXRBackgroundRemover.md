[@dev/core](../README.md) / [Exports](../modules.md) / WebXRBackgroundRemover

# Class: WebXRBackgroundRemover

A module that will automatically disable background meshes when entering AR and will enable them when leaving AR.

## Hierarchy

- [`WebXRAbstractFeature`](WebXRAbstractFeature.md)

  ↳ **`WebXRBackgroundRemover`**

## Table of contents

### Constructors

- [constructor](WebXRBackgroundRemover.md#constructor)

### Properties

- [\_xrSessionManager](WebXRBackgroundRemover.md#_xrsessionmanager)
- [disableAutoAttach](WebXRBackgroundRemover.md#disableautoattach)
- [isDisposed](WebXRBackgroundRemover.md#isdisposed)
- [onBackgroundStateChangedObservable](WebXRBackgroundRemover.md#onbackgroundstatechangedobservable)
- [options](WebXRBackgroundRemover.md#options)
- [xrNativeFeatureName](WebXRBackgroundRemover.md#xrnativefeaturename)
- [Name](WebXRBackgroundRemover.md#name)
- [Version](WebXRBackgroundRemover.md#version)

### Accessors

- [attached](WebXRBackgroundRemover.md#attached)

### Methods

- [\_addNewAttachObserver](WebXRBackgroundRemover.md#_addnewattachobserver)
- [\_onXRFrame](WebXRBackgroundRemover.md#_onxrframe)
- [\_setBackgroundState](WebXRBackgroundRemover.md#_setbackgroundstate)
- [attach](WebXRBackgroundRemover.md#attach)
- [detach](WebXRBackgroundRemover.md#detach)
- [dispose](WebXRBackgroundRemover.md#dispose)
- [isCompatible](WebXRBackgroundRemover.md#iscompatible)

## Constructors

### constructor

• **new WebXRBackgroundRemover**(`_xrSessionManager`, `options?`)

constructs a new background remover module

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `_xrSessionManager` | [`WebXRSessionManager`](WebXRSessionManager.md) | the session manager for this module |
| `options` | [`IWebXRBackgroundRemoverOptions`](../interfaces/IWebXRBackgroundRemoverOptions.md) | read-only options to be used in this module |

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[constructor](WebXRAbstractFeature.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRBackgroundRemover.ts:60

## Properties

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

### onBackgroundStateChangedObservable

• **onBackgroundStateChangedObservable**: [`Observable`](Observable.md)`boolean`

registered observers will be triggered when the background state changes

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRBackgroundRemover.ts:53

___

### options

• `Readonly` **options**: [`IWebXRBackgroundRemoverOptions`](../interfaces/IWebXRBackgroundRemoverOptions.md) = `{}`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRBackgroundRemover.ts:65

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

▪ `Static` `Readonly` **Name**: ``"xr-background-remover"``

The module's name

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRBackgroundRemover.ts:42

___

### Version

▪ `Static` `Readonly` **Version**: ``1``

The (Babylon) version of this module.
This is an integer representing the implementation version.
This number does not correspond to the WebXR specs version

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRBackgroundRemover.ts:48

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

https://github.com/babylon.js/core/src/XR/features/WebXRBackgroundRemover.ts:100

___

### \_setBackgroundState

▸ `Private` **_setBackgroundState**(`newState`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `newState` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRBackgroundRemover.ts:104

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

https://github.com/babylon.js/core/src/XR/features/WebXRBackgroundRemover.ts:76

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

https://github.com/babylon.js/core/src/XR/features/WebXRBackgroundRemover.ts:87

___

### dispose

▸ **dispose**(): `void`

Dispose this feature and all of the resources attached

#### Returns

`void`

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[dispose](WebXRAbstractFeature.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRBackgroundRemover.ts:95

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
