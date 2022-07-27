[@dev/core](../README.md) / [Exports](../modules.md) / WebXRRenderTarget

# Interface: WebXRRenderTarget

Abstraction of the XR render target

## Hierarchy

- [`IDisposable`](IDisposable.md)

  ↳ **`WebXRRenderTarget`**

## Implemented by

- [`WebXRManagedOutputCanvas`](../classes/WebXRManagedOutputCanvas.md)

## Table of contents

### Properties

- [canvasContext](WebXRRenderTarget.md#canvascontext)
- [xrLayer](WebXRRenderTarget.md#xrlayer)

### Methods

- [dispose](WebXRRenderTarget.md#dispose)
- [initializeXRLayerAsync](WebXRRenderTarget.md#initializexrlayerasync)

## Properties

### canvasContext

• **canvasContext**: `WebGLRenderingContext`

xrpresent context of the canvas which can be used to display/mirror xr content

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRTypes.ts:51

___

### xrLayer

• **xrLayer**: [`Nullable`](../modules.md#nullable)`XRWebGLLayer`

xr layer for the canvas

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRTypes.ts:56

## Methods

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

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRTypes.ts:63
