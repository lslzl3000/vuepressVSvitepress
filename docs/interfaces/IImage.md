[@dev/core](../README.md) / [Exports](../modules.md) / IImage

# Interface: IImage

Class used to abstract am image to use with the canvas and its context

## Table of contents

### Properties

- [crossOrigin](IImage.md#crossorigin)
- [height](IImage.md#height)
- [naturalHeight](IImage.md#naturalheight)
- [naturalWidth](IImage.md#naturalwidth)
- [onerror](IImage.md#onerror)
- [onload](IImage.md#onload)
- [referrerPolicy](IImage.md#referrerpolicy)
- [src](IImage.md#src)
- [width](IImage.md#width)

## Properties

### crossOrigin

• **crossOrigin**: ``null`` \| `string`

provides support for CORS, defining how the element handles crossorigin requests,
thereby enabling the configuration of the CORS requests for the element's fetched data.

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:74

___

### height

• `Readonly` **height**: `number`

Image height.

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:58

___

### naturalHeight

• `Readonly` **naturalHeight**: `number`

The original height of the image resource before sizing.

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:63

___

### naturalWidth

• `Readonly` **naturalWidth**: `number`

The original width of the image resource before sizing.

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:68

___

### onerror

• **onerror**: ``null`` \| (`this`: `GlobalEventHandlers`, `ev`: `Event`) => `any`

Error callback.

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:43

___

### onload

• **onload**: ``null`` \| (`this`: `GlobalEventHandlers`, `ev`: `Event`) => `any`

onload callback.

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:38

___

### referrerPolicy

• **referrerPolicy**: `string`

provides support for referrer policy on xhr load request,
it is used to control the request header.

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:80

___

### src

• **src**: `string`

Image source.

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:48

___

### width

• `Readonly` **width**: `number`

Image width.

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:53
