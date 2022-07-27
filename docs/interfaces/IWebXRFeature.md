[@dev/core](../README.md) / [Exports](../modules.md) / IWebXRFeature

# Interface: IWebXRFeature

Defining the interface required for a (webxr) feature

## Hierarchy

- [`IDisposable`](IDisposable.md)

  ↳ **`IWebXRFeature`**

  ↳↳ [`IWebXRHitTestFeature`](IWebXRHitTestFeature.md)

## Implemented by

- [`WebXRAbstractFeature`](../classes/WebXRAbstractFeature.md)

## Table of contents

### Properties

- [attached](IWebXRFeature.md#attached)
- [dependsOn](IWebXRFeature.md#dependson)
- [disableAutoAttach](IWebXRFeature.md#disableautoattach)
- [getXRSessionInitExtension](IWebXRFeature.md#getxrsessioninitextension)
- [isDisposed](IWebXRFeature.md#isdisposed)
- [xrNativeFeatureName](IWebXRFeature.md#xrnativefeaturename)

### Methods

- [attach](IWebXRFeature.md#attach)
- [detach](IWebXRFeature.md#detach)
- [dispose](IWebXRFeature.md#dispose)
- [isCompatible](IWebXRFeature.md#iscompatible)

## Properties

### attached

• **attached**: `boolean`

Is this feature attached

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRFeaturesManager.ts:12

___

### dependsOn

• `Optional` **dependsOn**: `string`[]

A list of (Babylon WebXR) features this feature depends on

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRFeaturesManager.ts:55

___

### disableAutoAttach

• **disableAutoAttach**: `boolean`

Should auto-attach be disabled?

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRFeaturesManager.ts:16

___

### getXRSessionInitExtension

• `Optional` **getXRSessionInitExtension**: () => `Promise``Partial``XRSessionInit`

#### Type declaration

▸ (): `Promise``Partial``XRSessionInit`

If this feature requires to extend the XRSessionInit object, this function will return the partial XR session init object

##### Returns

`Promise``Partial``XRSessionInit`

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRFeaturesManager.ts:60

___

### isDisposed

• **isDisposed**: `boolean`

Was this feature disposed;

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRFeaturesManager.ts:45

___

### xrNativeFeatureName

• `Optional` **xrNativeFeatureName**: `string`

The name of the native xr feature name, if applicable (like anchor, hit-test, or hand-tracking)

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRFeaturesManager.ts:50

## Methods

### attach

▸ **attach**(`force?`): `boolean`

Attach the feature to the session
Will usually be called by the features manager

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `force?` | `boolean` | should attachment be forced (even when already attached) |

#### Returns

`boolean`

true if successful.

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRFeaturesManager.ts:25

___

### detach

▸ **detach**(): `boolean`

Detach the feature from the session
Will usually be called by the features manager

#### Returns

`boolean`

true if successful.

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRFeaturesManager.ts:32

___

### dispose

▸ **dispose**(): `void`

Releases all held resources

#### Returns

`void`

#### Inherited from

[IDisposable](IDisposable.md).[dispose](IDisposable.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:103

___

### isCompatible

▸ **isCompatible**(): `boolean`

This function will be executed during before enabling the feature and can be used to not-allow enabling it.
Note that at this point the session has NOT started, so this is purely checking if the browser supports it

#### Returns

`boolean`

whether or not the feature is compatible in this environment

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRFeaturesManager.ts:40
