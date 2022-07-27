[@dev/core](../README.md) / [Exports](../modules.md) / ICanvas

# Interface: ICanvas

Class used to abstract a canvas

## Table of contents

### Properties

- [height](ICanvas.md#height)
- [width](ICanvas.md#width)

### Methods

- [getContext](ICanvas.md#getcontext)
- [toDataURL](ICanvas.md#todataurl)

## Properties

### height

• **height**: `number`

Canvas height.

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:13

___

### width

• **width**: `number`

Canvas width.

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:8

## Methods

### getContext

▸ **getContext**(`contextType`, `contextAttributes?`): [`ICanvasRenderingContext`](ICanvasRenderingContext.md)

returns a drawing context on the canvas.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `contextType` | `string` | context identifier. |
| `contextAttributes?` | `any` | context attributes. |

#### Returns

[`ICanvasRenderingContext`](ICanvasRenderingContext.md)

ICanvasRenderingContext object.

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:21

___

### toDataURL

▸ **toDataURL**(`mime`): `string`

returns a data URI containing a representation of the image in the format specified by the type parameter.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mime` | `string` | the image format. |

#### Returns

`string`

string containing the requested data URI.

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:28
