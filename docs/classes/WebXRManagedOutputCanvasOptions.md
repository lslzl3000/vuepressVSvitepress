[@dev/core](../README.md) / [Exports](../modules.md) / WebXRManagedOutputCanvasOptions

# Class: WebXRManagedOutputCanvasOptions

Configuration object for WebXR output canvas

## Table of contents

### Constructors

- [constructor](WebXRManagedOutputCanvasOptions.md#constructor)

### Properties

- [canvasElement](WebXRManagedOutputCanvasOptions.md#canvaselement)
- [canvasOptions](WebXRManagedOutputCanvasOptions.md#canvasoptions)
- [newCanvasCssStyle](WebXRManagedOutputCanvasOptions.md#newcanvascssstyle)

### Methods

- [GetDefaults](WebXRManagedOutputCanvasOptions.md#getdefaults)

## Constructors

### constructor

• **new WebXRManagedOutputCanvasOptions**()

## Properties

### canvasElement

• `Optional` **canvasElement**: `HTMLCanvasElement`

An optional canvas in case you wish to create it yourself and provide it here.
If not provided, a new canvas will be created

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRManagedOutputCanvas.ts:18

___

### canvasOptions

• `Optional` **canvasOptions**: `XRWebGLLayerInit`

Options for this XR Layer output

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRManagedOutputCanvas.ts:22

___

### newCanvasCssStyle

• `Optional` **newCanvasCssStyle**: `string`

CSS styling for a newly created canvas (if not provided)

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRManagedOutputCanvas.ts:26

## Methods

### GetDefaults

▸ `Static` **GetDefaults**(`engine?`): [`WebXRManagedOutputCanvasOptions`](WebXRManagedOutputCanvasOptions.md)

Get the default values of the configuration object

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `engine?` | [`ThinEngine`](ThinEngine.md) | defines the engine to use (can be null) |

#### Returns

[`WebXRManagedOutputCanvasOptions`](WebXRManagedOutputCanvasOptions.md)

default values of this configuration object

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRManagedOutputCanvas.ts:33
