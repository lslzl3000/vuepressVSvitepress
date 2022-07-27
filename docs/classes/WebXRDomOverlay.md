[@dev/core](../README.md) / [Exports](../modules.md) / WebXRDomOverlay

# Class: WebXRDomOverlay

DOM Overlay Feature

**`Since`**

5.0.0

## Hierarchy

- [`WebXRAbstractFeature`](WebXRAbstractFeature.md)

  ↳ **`WebXRDomOverlay`**

## Table of contents

### Constructors

- [constructor](WebXRDomOverlay.md#constructor)

### Properties

- [\_beforeXRSelectListener](WebXRDomOverlay.md#_beforexrselectlistener)
- [\_domOverlayType](WebXRDomOverlay.md#_domoverlaytype)
- [\_element](WebXRDomOverlay.md#_element)
- [\_xrSessionManager](WebXRDomOverlay.md#_xrsessionmanager)
- [disableAutoAttach](WebXRDomOverlay.md#disableautoattach)
- [isDisposed](WebXRDomOverlay.md#isdisposed)
- [options](WebXRDomOverlay.md#options)
- [xrNativeFeatureName](WebXRDomOverlay.md#xrnativefeaturename)
- [Name](WebXRDomOverlay.md#name)
- [Version](WebXRDomOverlay.md#version)

### Accessors

- [attached](WebXRDomOverlay.md#attached)
- [domOverlayType](WebXRDomOverlay.md#domoverlaytype)

### Methods

- [\_addNewAttachObserver](WebXRDomOverlay.md#_addnewattachobserver)
- [\_onXRFrame](WebXRDomOverlay.md#_onxrframe)
- [attach](WebXRDomOverlay.md#attach)
- [detach](WebXRDomOverlay.md#detach)
- [dispose](WebXRDomOverlay.md#dispose)
- [getXRSessionInitExtension](WebXRDomOverlay.md#getxrsessioninitextension)
- [isCompatible](WebXRDomOverlay.md#iscompatible)

## Constructors

### constructor

• **new WebXRDomOverlay**(`_xrSessionManager`, `options`)

Creates a new instance of the dom-overlay feature

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `_xrSessionManager` | [`WebXRSessionManager`](WebXRSessionManager.md) | an instance of WebXRSessionManager |
| `options` | [`IWebXRDomOverlayOptions`](../interfaces/IWebXRDomOverlayOptions.md) | options to use when constructing this feature |

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[constructor](WebXRAbstractFeature.md#constructor)

#### Defined in

packages/dev/core/src/XR/features/WebXRDOMOverlay.ts:77

## Properties

### \_beforeXRSelectListener

• `Private` **\_beforeXRSelectListener**: [`Nullable`](../modules.md#nullable)`EventListenerOrEventListenerObject` = `null`

Event Listener to supress "beforexrselect" events.

#### Defined in

packages/dev/core/src/XR/features/WebXRDOMOverlay.ts:54

___

### \_domOverlayType

• `Private` **\_domOverlayType**: [`Nullable`](../modules.md#nullable)`WebXRDomOverlayType` = `null`

Type of overlay - non-null when available

#### Defined in

packages/dev/core/src/XR/features/WebXRDOMOverlay.ts:49

___

### \_element

• `Private` **\_element**: [`Nullable`](../modules.md#nullable)`Element` = `null`

Element used for overlay

#### Defined in

packages/dev/core/src/XR/features/WebXRDOMOverlay.ts:59

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

### options

• `Readonly` **options**: [`IWebXRDomOverlayOptions`](../interfaces/IWebXRDomOverlayOptions.md)

#### Defined in

packages/dev/core/src/XR/features/WebXRDOMOverlay.ts:82

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

▪ `Static` `Readonly` **Name**: ``"xr-dom-overlay"``

The module's name

#### Defined in

packages/dev/core/src/XR/features/WebXRDOMOverlay.ts:64

___

### Version

▪ `Static` `Readonly` **Version**: ``1``

The (Babylon) version of this module.
This is an integer representing the implementation version.
This number does not correspond to the WebXR specs version

#### Defined in

packages/dev/core/src/XR/features/WebXRDOMOverlay.ts:70

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

### domOverlayType

• `get` **domOverlayType**(): [`Nullable`](../modules.md#nullable)`WebXRDomOverlayType`

The type of DOM overlay (null when not supported).  Provided by UA and remains unchanged for duration of session.

#### Returns

[`Nullable`](../modules.md#nullable)`WebXRDomOverlayType`

#### Defined in

packages/dev/core/src/XR/features/WebXRDOMOverlay.ts:122

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

packages/dev/core/src/XR/features/WebXRDOMOverlay.ts:136

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

packages/dev/core/src/XR/features/WebXRDOMOverlay.ts:97

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

Dispose this feature and all of the resources attached

#### Returns

`void`

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[dispose](WebXRAbstractFeature.md#dispose)

#### Defined in

packages/dev/core/src/XR/features/WebXRDOMOverlay.ts:129

___

### getXRSessionInitExtension

▸ **getXRSessionInitExtension**(): `Promise``Partial``XRSessionInit`

Extends the session init object if needed

#### Returns

`Promise``Partial``XRSessionInit`

augmentation object for the xr session init object.

#### Defined in

packages/dev/core/src/XR/features/WebXRDOMOverlay.ts:144

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
