[@dev/core](../README.md) / [Exports](../modules.md) / ICanvasGradient

# Interface: ICanvasGradient

Class used to abstract a canvas gradient

## Table of contents

### Methods

- [addColorStop](ICanvasGradient.md#addcolorstop)

## Methods

### addColorStop

▸ **addColorStop**(`offset`, `color`): `void`

adds a new color stop, defined by an offset and a color, to a given canvas gradient.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `offset` | `number` | A number between 0 and 1, inclusive, representing the position of the color stop. 0 represents the start of the gradient and 1 represents the end. |
| `color` | `string` | value representing the color of the stop. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:92
