[@dev/core](../README.md) / [Exports](../modules.md) / IWebXRHitTestFeature

# Interface: IWebXRHitTestFeatureT

An interface for all Hit test features

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`IWebXRLegacyHitResult`](IWebXRLegacyHitResult.md) |

## Hierarchy

- [`IWebXRFeature`](IWebXRFeature.md)

  ↳ **`IWebXRHitTestFeature`**

## Implemented by

- [`WebXRHitTest`](../classes/WebXRHitTest.md)
- [`WebXRHitTestLegacy`](../classes/WebXRHitTestLegacy.md)

## Table of contents

### Properties

- [attached](IWebXRHitTestFeature.md#attached)
- [dependsOn](IWebXRHitTestFeature.md#dependson)
- [disableAutoAttach](IWebXRHitTestFeature.md#disableautoattach)
- [getXRSessionInitExtension](IWebXRHitTestFeature.md#getxrsessioninitextension)
- [isDisposed](IWebXRHitTestFeature.md#isdisposed)
- [onHitTestResultObservable](IWebXRHitTestFeature.md#onhittestresultobservable)
- [xrNativeFeatureName](IWebXRHitTestFeature.md#xrnativefeaturename)

### Methods

- [attach](IWebXRHitTestFeature.md#attach)
- [detach](IWebXRHitTestFeature.md#detach)
- [dispose](IWebXRHitTestFeature.md#dispose)
- [isCompatible](IWebXRHitTestFeature.md#iscompatible)

## Properties

### attached

• **attached**: `boolean`

Is this feature attached

#### Inherited from

[IWebXRFeature](IWebXRFeature.md).[attached](IWebXRFeature.md#attached)

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRFeaturesManager.ts:12

___

### dependsOn

• `Optional` **dependsOn**: `string`[]

A list of (Babylon WebXR) features this feature depends on

#### Inherited from

[IWebXRFeature](IWebXRFeature.md).[dependsOn](IWebXRFeature.md#dependson)

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRFeaturesManager.ts:55

___

### disableAutoAttach

• **disableAutoAttach**: `boolean`

Should auto-attach be disabled?

#### Inherited from

[IWebXRFeature](IWebXRFeature.md).[disableAutoAttach](IWebXRFeature.md#disableautoattach)

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

#### Inherited from

[IWebXRFeature](IWebXRFeature.md).[getXRSessionInitExtension](IWebXRFeature.md#getxrsessioninitextension)

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRFeaturesManager.ts:60

___

### isDisposed

• **isDisposed**: `boolean`

Was this feature disposed;

#### Inherited from

[IWebXRFeature](IWebXRFeature.md).[isDisposed](IWebXRFeature.md#isdisposed)

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRFeaturesManager.ts:45

___

### onHitTestResultObservable

• **onHitTestResultObservable**: [`Observable`](../classes/Observable.md)`T`[]

Triggered when new babylon (transformed) hit test results are available

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHitTestLegacy.ts:19

___

### xrNativeFeatureName

• `Optional` **xrNativeFeatureName**: `string`

The name of the native xr feature name, if applicable (like anchor, hit-test, or hand-tracking)

#### Inherited from

[IWebXRFeature](IWebXRFeature.md).[xrNativeFeatureName](IWebXRFeature.md#xrnativefeaturename)

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

#### Inherited from

[IWebXRFeature](IWebXRFeature.md).[attach](IWebXRFeature.md#attach)

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

#### Inherited from

[IWebXRFeature](IWebXRFeature.md).[detach](IWebXRFeature.md#detach)

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRFeaturesManager.ts:32

___

### dispose

▸ **dispose**(): `void`

Releases all held resources

#### Returns

`void`

#### Inherited from

[IWebXRFeature](IWebXRFeature.md).[dispose](IWebXRFeature.md#dispose)

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

#### Inherited from

[IWebXRFeature](IWebXRFeature.md).[isCompatible](IWebXRFeature.md#iscompatible)

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRFeaturesManager.ts:40
