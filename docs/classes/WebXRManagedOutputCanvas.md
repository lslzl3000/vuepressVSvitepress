[@dev/core](../README.md) / [Exports](../modules.md) / WebXRManagedOutputCanvas

# Class: WebXRManagedOutputCanvas

Creates a canvas that is added/removed from the webpage when entering/exiting XR

## Implements

- [`WebXRRenderTarget`](../interfaces/WebXRRenderTarget.md)

## Table of contents

### Constructors

- [constructor](WebXRManagedOutputCanvas.md#constructor)

### Properties

- [\_canvas](WebXRManagedOutputCanvas.md#_canvas)
- [\_engine](WebXRManagedOutputCanvas.md#_engine)
- [\_originalCanvasSize](WebXRManagedOutputCanvas.md#_originalcanvassize)
- [\_xrLayerWrapper](WebXRManagedOutputCanvas.md#_xrlayerwrapper)
- [canvasContext](WebXRManagedOutputCanvas.md#canvascontext)
- [onXRLayerInitObservable](WebXRManagedOutputCanvas.md#onxrlayerinitobservable)
- [xrLayer](WebXRManagedOutputCanvas.md#xrlayer)

### Methods

- [\_addCanvas](WebXRManagedOutputCanvas.md#_addcanvas)
- [\_removeCanvas](WebXRManagedOutputCanvas.md#_removecanvas)
- [\_setCanvasSize](WebXRManagedOutputCanvas.md#_setcanvassize)
- [\_setManagedOutputCanvas](WebXRManagedOutputCanvas.md#_setmanagedoutputcanvas)
- [dispose](WebXRManagedOutputCanvas.md#dispose)
- [initializeXRLayerAsync](WebXRManagedOutputCanvas.md#initializexrlayerasync)

## Constructors

### constructor

• **new WebXRManagedOutputCanvas**(`_xrSessionManager`, `_options?`)

Initializes the canvas to be added/removed upon entering/exiting xr

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `_xrSessionManager` | [`WebXRSessionManager`](WebXRSessionManager.md) | The XR Session manager |
| `_options` | [`WebXRManagedOutputCanvasOptions`](WebXRManagedOutputCanvasOptions.md) | optional configuration for this canvas output. defaults will be used if not provided |

#### Defined in

packages/dev/core/src/XR/webXRManagedOutputCanvas.ts:82

## Properties

### \_canvas

• `Private` **\_canvas**: [`Nullable`](../modules.md#nullable)`HTMLCanvasElement` = `null`

#### Defined in

packages/dev/core/src/XR/webXRManagedOutputCanvas.ts:53

___

### \_engine

• `Private` **\_engine**: [`Nullable`](../modules.md#nullable)[`ThinEngine`](ThinEngine.md) = `null`

#### Defined in

packages/dev/core/src/XR/webXRManagedOutputCanvas.ts:54

___

### \_originalCanvasSize

• `Private` **\_originalCanvasSize**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `height` | `number` |
| `width` | `number` |

#### Defined in

packages/dev/core/src/XR/webXRManagedOutputCanvas.ts:55

___

### \_xrLayerWrapper

• `Private` **\_xrLayerWrapper**: [`Nullable`](../modules.md#nullable)`WebXRLayerWrapper` = `null`

#### Defined in

packages/dev/core/src/XR/webXRManagedOutputCanvas.ts:70

___

### canvasContext

• **canvasContext**: `WebGLRenderingContext`

Rendering context of the canvas which can be used to display/mirror xr content

#### Implementation of

[WebXRRenderTarget](../interfaces/WebXRRenderTarget.md).[canvasContext](../interfaces/WebXRRenderTarget.md#canvascontext)

#### Defined in

packages/dev/core/src/XR/webXRManagedOutputCanvas.ts:63

___

### onXRLayerInitObservable

• **onXRLayerInitObservable**: [`Observable`](Observable.md)`XRWebGLLayer`

Observers registered here will be triggered when the xr layer was initialized

#### Defined in

packages/dev/core/src/XR/webXRManagedOutputCanvas.ts:75

___

### xrLayer

• **xrLayer**: [`Nullable`](../modules.md#nullable)`XRWebGLLayer` = `null`

xr layer for the canvas

#### Implementation of

[WebXRRenderTarget](../interfaces/WebXRRenderTarget.md).[xrLayer](../interfaces/WebXRRenderTarget.md#xrlayer)

#### Defined in

packages/dev/core/src/XR/webXRManagedOutputCanvas.ts:68

## Methods

### \_addCanvas

▸ `Private` **_addCanvas**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/webXRManagedOutputCanvas.ts:146

___

### \_removeCanvas

▸ `Private` **_removeCanvas**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/webXRManagedOutputCanvas.ts:159

___

### \_setCanvasSize

▸ `Private` **_setCanvasSize**(`init?`, `xrLayer?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `init` | `boolean` | `true` |
| `xrLayer` | [`Nullable`](../modules.md#nullable)`WebXRLayerWrapper` | `undefined` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/webXRManagedOutputCanvas.ts:166

___

### \_setManagedOutputCanvas

▸ `Private` **_setManagedOutputCanvas**(`canvas`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `canvas` | [`Nullable`](../modules.md#nullable)`HTMLCanvasElement` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/webXRManagedOutputCanvas.ts:191

___

### dispose

▸ **dispose**(): `void`

Disposes of the object

#### Returns

`void`

#### Implementation of

[WebXRRenderTarget](../interfaces/WebXRRenderTarget.md).[dispose](../interfaces/WebXRRenderTarget.md#dispose)

#### Defined in

packages/dev/core/src/XR/webXRManagedOutputCanvas.ts:108

___

### initializeXRLayerAsync

▸ **initializeXRLayerAsync**(`xrSession`): `Promise``XRWebGLLayer`

Initializes a XRWebGLLayer to be used as the session's baseLayer.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `xrSession` | `XRSession` | xr session |

#### Returns

`Promise``XRWebGLLayer`

a promise that will resolve once the XR Layer has been created

#### Implementation of

[WebXRRenderTarget](../interfaces/WebXRRenderTarget.md).[initializeXRLayerAsync](../interfaces/WebXRRenderTarget.md#initializexrlayerasync)

#### Defined in

packages/dev/core/src/XR/webXRManagedOutputCanvas.ts:118
