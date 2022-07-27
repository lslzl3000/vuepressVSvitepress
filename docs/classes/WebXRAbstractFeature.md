[@dev/core](../README.md) / [Exports](../modules.md) / WebXRAbstractFeature

# Class: WebXRAbstractFeature

This is the base class for all WebXR features.
Since most features require almost the same resources and callbacks, this class can be used to simplify the development
Note that since the features manager is using the `IWebXRFeature` you are in no way obligated to use this class

## Hierarchy

- **`WebXRAbstractFeature`**

  ↳ [`WebXRHitTestLegacy`](WebXRHitTestLegacy.md)

  ↳ [`WebXRAnchorSystem`](WebXRAnchorSystem.md)

  ↳ [`WebXRPlaneDetector`](WebXRPlaneDetector.md)

  ↳ [`WebXRBackgroundRemover`](WebXRBackgroundRemover.md)

  ↳ [`WebXRMotionControllerTeleportation`](WebXRMotionControllerTeleportation.md)

  ↳ [`WebXRControllerPointerSelection`](WebXRControllerPointerSelection.md)

  ↳ [`WebXRControllerPhysics`](WebXRControllerPhysics.md)

  ↳ [`WebXRHitTest`](WebXRHitTest.md)

  ↳ [`WebXRFeaturePointSystem`](WebXRFeaturePointSystem.md)

  ↳ [`WebXRHandTracking`](WebXRHandTracking.md)

  ↳ [`WebXRMeshDetector`](WebXRMeshDetector.md)

  ↳ [`WebXRImageTracking`](WebXRImageTracking.md)

  ↳ [`WebXRNearInteraction`](WebXRNearInteraction.md)

  ↳ [`WebXRDomOverlay`](WebXRDomOverlay.md)

  ↳ [`WebXRControllerMovement`](WebXRControllerMovement.md)

  ↳ [`WebXRLightEstimation`](WebXRLightEstimation.md)

  ↳ [`WebXREyeTracking`](WebXREyeTracking.md)

  ↳ [`WebXRWalkingLocomotion`](WebXRWalkingLocomotion.md)

  ↳ [`WebXRLayers`](WebXRLayers.md)

## Implements

- [`IWebXRFeature`](../interfaces/IWebXRFeature.md)

## Table of contents

### Constructors

- [constructor](WebXRAbstractFeature.md#constructor)

### Properties

- [\_attached](WebXRAbstractFeature.md#_attached)
- [\_removeOnDetach](WebXRAbstractFeature.md#_removeondetach)
- [\_xrSessionManager](WebXRAbstractFeature.md#_xrsessionmanager)
- [disableAutoAttach](WebXRAbstractFeature.md#disableautoattach)
- [isDisposed](WebXRAbstractFeature.md#isdisposed)
- [xrNativeFeatureName](WebXRAbstractFeature.md#xrnativefeaturename)

### Accessors

- [attached](WebXRAbstractFeature.md#attached)

### Methods

- [\_addNewAttachObserver](WebXRAbstractFeature.md#_addnewattachobserver)
- [\_onXRFrame](WebXRAbstractFeature.md#_onxrframe)
- [attach](WebXRAbstractFeature.md#attach)
- [detach](WebXRAbstractFeature.md#detach)
- [dispose](WebXRAbstractFeature.md#dispose)
- [isCompatible](WebXRAbstractFeature.md#iscompatible)

## Constructors

### constructor

• **new WebXRAbstractFeature**(`_xrSessionManager`)

Construct a new (abstract) WebXR feature

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `_xrSessionManager` | [`WebXRSessionManager`](WebXRSessionManager.md) | the xr session manager for this feature |

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRAbstractFeature.ts:37

## Properties

### \_attached

• `Private` **\_attached**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRAbstractFeature.ts:12

___

### \_removeOnDetach

• `Private` **\_removeOnDetach**: { `observable`: [`Observable`](Observable.md)`any` ; `observer`: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)`any`  }[] = `[]`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRAbstractFeature.ts:13

___

### \_xrSessionManager

• `Protected` **\_xrSessionManager**: [`WebXRSessionManager`](WebXRSessionManager.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRAbstractFeature.ts:37

___

### disableAutoAttach

• **disableAutoAttach**: `boolean` = `false`

Should auto-attach be disabled?

#### Implementation of

[IWebXRFeature](../interfaces/IWebXRFeature.md).[disableAutoAttach](../interfaces/IWebXRFeature.md#disableautoattach)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRAbstractFeature.ts:26

___

### isDisposed

• **isDisposed**: `boolean` = `false`

Is this feature disposed?

#### Implementation of

[IWebXRFeature](../interfaces/IWebXRFeature.md).[isDisposed](../interfaces/IWebXRFeature.md#isdisposed)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRAbstractFeature.ts:21

___

### xrNativeFeatureName

• **xrNativeFeatureName**: `string` = `""`

The name of the native xr feature name (like anchor, hit-test, or hand-tracking)

#### Implementation of

[IWebXRFeature](../interfaces/IWebXRFeature.md).[xrNativeFeatureName](../interfaces/IWebXRFeature.md#xrnativefeaturename)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRAbstractFeature.ts:31

## Accessors

### attached

• `get` **attached**(): `boolean`

Is this feature attached

#### Returns

`boolean`

#### Implementation of

[IWebXRFeature](../interfaces/IWebXRFeature.md).[attached](../interfaces/IWebXRFeature.md#attached)

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

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRAbstractFeature.ts:113

___

### \_onXRFrame

▸ `Protected` `Abstract` **_onXRFrame**(`_xrFrame`): `void`

Code in this function will be executed on each xrFrame received from the browser.
This function will not execute after the feature is detached.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `_xrFrame` | `XRFrame` | the current frame |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRAbstractFeature.ts:125

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

#### Implementation of

[IWebXRFeature](../interfaces/IWebXRFeature.md).[attach](../interfaces/IWebXRFeature.md#attach)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRAbstractFeature.ts:52

___

### detach

▸ **detach**(): `boolean`

detach this feature.

#### Returns

`boolean`

true if successful, false if failed or already detached

#### Implementation of

[IWebXRFeature](../interfaces/IWebXRFeature.md).[detach](../interfaces/IWebXRFeature.md#detach)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRAbstractFeature.ts:78

___

### dispose

▸ **dispose**(): `void`

Dispose this feature and all of the resources attached

#### Returns

`void`

#### Implementation of

[IWebXRFeature](../interfaces/IWebXRFeature.md).[dispose](../interfaces/IWebXRFeature.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRAbstractFeature.ts:93

___

### isCompatible

▸ **isCompatible**(): `boolean`

This function will be executed during before enabling the feature and can be used to not-allow enabling it.
Note that at this point the session has NOT started, so this is purely checking if the browser supports it

#### Returns

`boolean`

whether or not the feature is compatible in this environment

#### Implementation of

[IWebXRFeature](../interfaces/IWebXRFeature.md).[isCompatible](../interfaces/IWebXRFeature.md#iscompatible)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRAbstractFeature.ts:104
