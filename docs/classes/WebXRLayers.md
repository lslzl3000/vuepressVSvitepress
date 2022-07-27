[@dev/core](../README.md) / [Exports](../modules.md) / WebXRLayers

# Class: WebXRLayers

Exposes the WebXR Layers API.

## Hierarchy

- [`WebXRAbstractFeature`](WebXRAbstractFeature.md)

  ↳ **`WebXRLayers`**

## Table of contents

### Constructors

- [constructor](WebXRLayers.md#constructor)

### Properties

- [\_existingLayers](WebXRLayers.md#_existinglayers)
- [\_glContext](WebXRLayers.md#_glcontext)
- [\_xrSessionManager](WebXRLayers.md#_xrsessionmanager)
- [\_xrWebGLBinding](WebXRLayers.md#_xrwebglbinding)
- [disableAutoAttach](WebXRLayers.md#disableautoattach)
- [isDisposed](WebXRLayers.md#isdisposed)
- [xrNativeFeatureName](WebXRLayers.md#xrnativefeaturename)
- [Name](WebXRLayers.md#name)
- [Version](WebXRLayers.md#version)

### Accessors

- [attached](WebXRLayers.md#attached)

### Methods

- [\_addNewAttachObserver](WebXRLayers.md#_addnewattachobserver)
- [\_onXRFrame](WebXRLayers.md#_onxrframe)
- [addXRSessionLayer](WebXRLayers.md#addxrsessionlayer)
- [attach](WebXRLayers.md#attach)
- [createProjectionLayer](WebXRLayers.md#createprojectionlayer)
- [createXRWebGLLayer](WebXRLayers.md#createxrwebgllayer)
- [detach](WebXRLayers.md#detach)
- [dispose](WebXRLayers.md#dispose)
- [isCompatible](WebXRLayers.md#iscompatible)
- [setXRSessionLayers](WebXRLayers.md#setxrsessionlayers)

## Constructors

### constructor

• **new WebXRLayers**(`_xrSessionManager`, `_options?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `_xrSessionManager` | [`WebXRSessionManager`](WebXRSessionManager.md) |
| `_options` | [`IWebXRLayersOptions`](../interfaces/IWebXRLayersOptions.md) |

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[constructor](WebXRAbstractFeature.md#constructor)

#### Defined in

packages/dev/core/src/XR/features/WebXRLayers.ts:207

## Properties

### \_existingLayers

• `Private` **\_existingLayers**: `WebXRLayerWrapper`[] = `[]`

Already-created layers

#### Defined in

packages/dev/core/src/XR/features/WebXRLayers.ts:202

___

### \_glContext

• `Private` **\_glContext**: `WebGLRenderingContext` \| `WebGL2RenderingContext`

#### Defined in

packages/dev/core/src/XR/features/WebXRLayers.ts:204

___

### \_xrSessionManager

• `Protected` **\_xrSessionManager**: [`WebXRSessionManager`](WebXRSessionManager.md)

#### Inherited from

[WebXRAbstractFeature](WebXRAbstractFeature.md).[_xrSessionManager](WebXRAbstractFeature.md#_xrsessionmanager)

#### Defined in

packages/dev/core/src/XR/features/WebXRAbstractFeature.ts:37

___

### \_xrWebGLBinding

• `Private` **\_xrWebGLBinding**: `XRWebGLBinding`

#### Defined in

packages/dev/core/src/XR/features/WebXRLayers.ts:205

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

### xrNativeFeatureName

• **xrNativeFeatureName**: `string` = `""`

The name of the native xr feature name (like anchor, hit-test, or hand-tracking)

#### Inherited from

[WebXRAbstractFeature](WebXRAbstractFeature.md).[xrNativeFeatureName](WebXRAbstractFeature.md#xrnativefeaturename)

#### Defined in

packages/dev/core/src/XR/features/WebXRAbstractFeature.ts:31

___

### Name

▪ `Static` `Readonly` **Name**: ``"xr-layers"``

The module's name

#### Defined in

packages/dev/core/src/XR/features/WebXRLayers.ts:192

___

### Version

▪ `Static` `Readonly` **Version**: ``1``

The (Babylon) version of this module.
This is an integer representing the implementation version.
This number does not correspond to the WebXR specs version

#### Defined in

packages/dev/core/src/XR/features/WebXRLayers.ts:198

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

packages/dev/core/src/XR/features/WebXRLayers.ts:315

___

### addXRSessionLayer

▸ **addXRSessionLayer**(`wrappedLayer`): `void`

Add a new layer to the already-existing list of layers

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `wrappedLayer` | `WebXRLayerWrapper` | the new layer to add to the existing ones |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/features/WebXRLayers.ts:280

___

### attach

▸ **attach**(): `boolean`

Attach this feature.
Will usually be called by the features manager.

#### Returns

`boolean`

true if successful.

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[attach](WebXRAbstractFeature.md#attach)

#### Defined in

packages/dev/core/src/XR/features/WebXRLayers.ts:218

___

### createProjectionLayer

▸ **createProjectionLayer**(`params?`, `multiview?`): `WebXRProjectionLayerWrapper`

Creates a new XRProjectionLayer.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `params` | `XRProjectionLayerInit` | `defaultXRProjectionLayerInit` | an object providing configuration options for the new XRProjectionLayer. |
| `multiview` | `boolean` | `false` | whether the projection layer should render with multiview. |

#### Returns

`WebXRProjectionLayerWrapper`

the projection layer

#### Defined in

packages/dev/core/src/XR/features/WebXRLayers.ts:262

___

### createXRWebGLLayer

▸ **createXRWebGLLayer**(`params?`): `WebXRWebGLLayerWrapper`

Creates a new XRWebGLLayer.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `params` | `XRWebGLLayerInit` | `defaultXRWebGLLayerInit` | an object providing configuration options for the new XRWebGLLayer |

#### Returns

`WebXRWebGLLayerWrapper`

the XRWebGLLayer

#### Defined in

packages/dev/core/src/XR/features/WebXRLayers.ts:251

___

### detach

▸ **detach**(): `boolean`

detach this feature.

#### Returns

`boolean`

true if successful, false if failed or already detached

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[detach](WebXRAbstractFeature.md#detach)

#### Defined in

packages/dev/core/src/XR/features/WebXRLayers.ts:238

___

### dispose

▸ **dispose**(): `void`

Dispose this feature and all of the resources attached.

#### Returns

`void`

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[dispose](WebXRAbstractFeature.md#dispose)

#### Defined in

packages/dev/core/src/XR/features/WebXRLayers.ts:311

___

### isCompatible

▸ **isCompatible**(): `boolean`

This function will be executed during before enabling the feature and can be used to not-allow enabling it.
Note that at this point the session has NOT started, so this is purely checking if the browser supports it

#### Returns

`boolean`

whether or not the feature is compatible in this environment

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[isCompatible](WebXRAbstractFeature.md#iscompatible)

#### Defined in

packages/dev/core/src/XR/features/WebXRLayers.ts:303

___

### setXRSessionLayers

▸ **setXRSessionLayers**(`wrappedLayers`): `void`

Sets the layers to be used by the XR session.
Note that you must call this function with any layers you wish to render to
since it adds them to the XR session's render state
(replacing any layers that were added in a previous call to setXRSessionLayers or updateRenderState).
This method also sets up the session manager's render target texture provider
as the first layer in the array, which feeds the WebXR camera(s) attached to the session.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `wrappedLayers` | `WebXRLayerWrapper`[] | An array of WebXRLayerWrapper, usually returned from the WebXRLayers createLayer functions. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/features/WebXRLayers.ts:293
