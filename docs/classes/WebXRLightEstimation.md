[@dev/core](../README.md) / [Exports](../modules.md) / WebXRLightEstimation

# Class: WebXRLightEstimation

Light Estimation Feature

**`Since`**

5.0.0

## Hierarchy

- [`WebXRAbstractFeature`](WebXRAbstractFeature.md)

  ↳ **`WebXRLightEstimation`**

## Table of contents

### Constructors

- [constructor](WebXRLightEstimation.md#constructor)

### Properties

- [\_canvasContext](WebXRLightEstimation.md#_canvascontext)
- [\_cubeMapPollTime](WebXRLightEstimation.md#_cubemappolltime)
- [\_intensity](WebXRLightEstimation.md#_intensity)
- [\_lightColor](WebXRLightEstimation.md#_lightcolor)
- [\_lightDirection](WebXRLightEstimation.md#_lightdirection)
- [\_lightEstimationPollTime](WebXRLightEstimation.md#_lightestimationpolltime)
- [\_reflectionCubeMap](WebXRLightEstimation.md#_reflectioncubemap)
- [\_reflectionCubeMapTextureSize](WebXRLightEstimation.md#_reflectioncubemaptexturesize)
- [\_sphericalHarmonics](WebXRLightEstimation.md#_sphericalharmonics)
- [\_xrLightEstimate](WebXRLightEstimation.md#_xrlightestimate)
- [\_xrLightProbe](WebXRLightEstimation.md#_xrlightprobe)
- [\_xrSessionManager](WebXRLightEstimation.md#_xrsessionmanager)
- [\_xrWebGLBinding](WebXRLightEstimation.md#_xrwebglbinding)
- [directionalLight](WebXRLightEstimation.md#directionallight)
- [disableAutoAttach](WebXRLightEstimation.md#disableautoattach)
- [isDisposed](WebXRLightEstimation.md#isdisposed)
- [onReflectionCubeMapUpdatedObservable](WebXRLightEstimation.md#onreflectioncubemapupdatedobservable)
- [options](WebXRLightEstimation.md#options)
- [xrNativeFeatureName](WebXRLightEstimation.md#xrnativefeaturename)
- [Name](WebXRLightEstimation.md#name)
- [Version](WebXRLightEstimation.md#version)

### Accessors

- [attached](WebXRLightEstimation.md#attached)
- [reflectionCubeMapTexture](WebXRLightEstimation.md#reflectioncubemaptexture)
- [xrLightingEstimate](WebXRLightEstimation.md#xrlightingestimate)

### Methods

- [\_addNewAttachObserver](WebXRLightEstimation.md#_addnewattachobserver)
- [\_getCanvasContext](WebXRLightEstimation.md#_getcanvascontext)
- [\_getXRGLBinding](WebXRLightEstimation.md#_getxrglbinding)
- [\_onXRFrame](WebXRLightEstimation.md#_onxrframe)
- [\_updateReflectionCubeMap](WebXRLightEstimation.md#_updatereflectioncubemap)
- [attach](WebXRLightEstimation.md#attach)
- [detach](WebXRLightEstimation.md#detach)
- [dispose](WebXRLightEstimation.md#dispose)
- [isCompatible](WebXRLightEstimation.md#iscompatible)

## Constructors

### constructor

• **new WebXRLightEstimation**(`_xrSessionManager`, `options`)

Creates a new instance of the light estimation feature

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `_xrSessionManager` | [`WebXRSessionManager`](WebXRSessionManager.md) | an instance of WebXRSessionManager |
| `options` | [`IWebXRLightEstimationOptions`](../interfaces/IWebXRLightEstimationOptions.md) | options to use when constructing this feature |

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[constructor](WebXRAbstractFeature.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRLightEstimation.ts:136

## Properties

### \_canvasContext

• `Private` **\_canvasContext**: [`Nullable`](../modules.md#nullable)`WebGLRenderingContext` \| `WebGL2RenderingContext` = `null`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRLightEstimation.ts:89

___

### \_cubeMapPollTime

• `Private` **\_cubeMapPollTime**: `number`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRLightEstimation.ts:98

___

### \_intensity

• `Private` **\_intensity**: `number` = `1`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRLightEstimation.ts:96

___

### \_lightColor

• `Private` **\_lightColor**: [`Color3`](Color3.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRLightEstimation.ts:95

___

### \_lightDirection

• `Private` **\_lightDirection**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRLightEstimation.ts:94

___

### \_lightEstimationPollTime

• `Private` **\_lightEstimationPollTime**: `number`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRLightEstimation.ts:99

___

### \_reflectionCubeMap

• `Private` **\_reflectionCubeMap**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRLightEstimation.ts:90

___

### \_reflectionCubeMapTextureSize

• `Private` **\_reflectionCubeMapTextureSize**: `number` = `16`

ARCore's reflection cube map size is 16x16.
Once other systems support this feature we will need to change this to be dynamic.
see https://github.com/immersive-web/lighting-estimation/blob/main/lighting-estimation-explainer.md#cube-map-open-questions

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRLightEstimation.ts:117

___

### \_sphericalHarmonics

• `Private` **\_sphericalHarmonics**: [`SphericalHarmonics`](SphericalHarmonics.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRLightEstimation.ts:97

___

### \_xrLightEstimate

• `Private` **\_xrLightEstimate**: [`Nullable`](../modules.md#nullable)`XRLightEstimate` = `null`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRLightEstimation.ts:91

___

### \_xrLightProbe

• `Private` **\_xrLightProbe**: [`Nullable`](../modules.md#nullable)`XRLightProbe` = `null`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRLightEstimation.ts:92

___

### \_xrSessionManager

• `Protected` **\_xrSessionManager**: [`WebXRSessionManager`](WebXRSessionManager.md)

#### Inherited from

[WebXRAbstractFeature](WebXRAbstractFeature.md).[_xrSessionManager](WebXRAbstractFeature.md#_xrsessionmanager)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRAbstractFeature.ts:37

___

### \_xrWebGLBinding

• `Private` **\_xrWebGLBinding**: [`Nullable`](../modules.md#nullable)`XRWebGLBinding` = `null`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRLightEstimation.ts:93

___

### directionalLight

• **directionalLight**: [`Nullable`](../modules.md#nullable)[`DirectionalLight`](DirectionalLight.md) = `null`

If createDirectionalLightSource is set to true this light source will be created automatically.
Otherwise this can be set with an external directional light source.
This light will be updated whenever the light estimation values change.

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRLightEstimation.ts:124

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

### onReflectionCubeMapUpdatedObservable

• **onReflectionCubeMapUpdatedObservable**: [`Observable`](Observable.md)[`BaseTexture`](BaseTexture.md)

This observable will notify when the reflection cube map is updated.

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRLightEstimation.ts:129

___

### options

• `Readonly` **options**: [`IWebXRLightEstimationOptions`](../interfaces/IWebXRLightEstimationOptions.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRLightEstimation.ts:141

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

▪ `Static` `Readonly` **Name**: ``"xr-light-estimation"``

The module's name

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRLightEstimation.ts:104

___

### Version

▪ `Static` `Readonly` **Version**: ``1``

The (Babylon) version of this module.
This is an integer representing the implementation version.
This number does not correspond to the WebXR specs version

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRLightEstimation.ts:110

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

___

### reflectionCubeMapTexture

• `get` **reflectionCubeMapTexture**(): [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

While the estimated cube map is expected to update over time to better reflect the user's environment as they move around those changes are unlikely to happen with every XRFrame.
Since creating and processing the cube map is potentially expensive, especially if mip maps are needed, you can listen to the onReflectionCubeMapUpdatedObservable to determine
when it has been updated.

#### Returns

[`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRLightEstimation.ts:163

___

### xrLightingEstimate

• `get` **xrLightingEstimate**(): [`Nullable`](../modules.md#nullable)[`IWebXRLightEstimation`](../interfaces/IWebXRLightEstimation.md)

The most recent light estimate.  Available starting on the first frame where the device provides a light probe.

#### Returns

[`Nullable`](../modules.md#nullable)[`IWebXRLightEstimation`](../interfaces/IWebXRLightEstimation.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRLightEstimation.ts:170

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

### \_getCanvasContext

▸ `Private` **_getCanvasContext**(): `WebGLRenderingContext` \| `WebGL2RenderingContext`

#### Returns

`WebGLRenderingContext` \| `WebGL2RenderingContext`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRLightEstimation.ts:182

___

### \_getXRGLBinding

▸ `Private` **_getXRGLBinding**(): `XRWebGLBinding`

#### Returns

`XRWebGLBinding`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRLightEstimation.ts:189

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

https://github.com/babylon.js/core/src/XR/features/WebXRLightEstimation.ts:319

___

### \_updateReflectionCubeMap

▸ `Private` **_updateReflectionCubeMap**(): `void`

Event Listener for "reflectionchange" events.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRLightEstimation.ts:200

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

https://github.com/babylon.js/core/src/XR/features/WebXRLightEstimation.ts:246

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

https://github.com/babylon.js/core/src/XR/features/WebXRLightEstimation.ts:281

___

### dispose

▸ **dispose**(): `void`

Dispose this feature and all of the resources attached

#### Returns

`void`

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[dispose](WebXRAbstractFeature.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRLightEstimation.ts:300

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
