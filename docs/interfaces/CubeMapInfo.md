[@dev/core](../README.md) / [Exports](../modules.md) / CubeMapInfo

# Interface: CubeMapInfo

CubeMap information grouping all the data for each faces as well as the cubemap size.

## Table of contents

### Properties

- [back](CubeMapInfo.md#back)
- [down](CubeMapInfo.md#down)
- [format](CubeMapInfo.md#format)
- [front](CubeMapInfo.md#front)
- [gammaSpace](CubeMapInfo.md#gammaspace)
- [left](CubeMapInfo.md#left)
- [right](CubeMapInfo.md#right)
- [size](CubeMapInfo.md#size)
- [type](CubeMapInfo.md#type)
- [up](CubeMapInfo.md#up)

## Properties

### back

• **back**: [`Nullable`](../modules.md#nullable)`ArrayBufferView`

The pixel array for the back face.
This is stored in format, left to right, up to down format.

#### Defined in

https://github.com/babylon.js/core/src/Misc/HighDynamicRange/panoramaToCubemap.ts:20

___

### down

• **down**: [`Nullable`](../modules.md#nullable)`ArrayBufferView`

The pixel array for the down face.
This is stored in format, left to right, up to down format.

#### Defined in

https://github.com/babylon.js/core/src/Misc/HighDynamicRange/panoramaToCubemap.ts:44

___

### format

• **format**: `number`

The format of the texture.

RGBA, RGB.

#### Defined in

https://github.com/babylon.js/core/src/Misc/HighDynamicRange/panoramaToCubemap.ts:58

___

### front

• **front**: [`Nullable`](../modules.md#nullable)`ArrayBufferView`

The pixel array for the front face.
This is stored in format, left to right, up to down format.

#### Defined in

https://github.com/babylon.js/core/src/Misc/HighDynamicRange/panoramaToCubemap.ts:14

___

### gammaSpace

• **gammaSpace**: `boolean`

Specifies whether the texture is in gamma space.

#### Defined in

https://github.com/babylon.js/core/src/Misc/HighDynamicRange/panoramaToCubemap.ts:70

___

### left

• **left**: [`Nullable`](../modules.md#nullable)`ArrayBufferView`

The pixel array for the left face.
This is stored in format, left to right, up to down format.

#### Defined in

https://github.com/babylon.js/core/src/Misc/HighDynamicRange/panoramaToCubemap.ts:26

___

### right

• **right**: [`Nullable`](../modules.md#nullable)`ArrayBufferView`

The pixel array for the right face.
This is stored in format, left to right, up to down format.

#### Defined in

https://github.com/babylon.js/core/src/Misc/HighDynamicRange/panoramaToCubemap.ts:32

___

### size

• **size**: `number`

The size of the cubemap stored.

Each faces will be size * size pixels.

#### Defined in

https://github.com/babylon.js/core/src/Misc/HighDynamicRange/panoramaToCubemap.ts:51

___

### type

• **type**: `number`

The type of the texture data.

UNSIGNED_INT, FLOAT.

#### Defined in

https://github.com/babylon.js/core/src/Misc/HighDynamicRange/panoramaToCubemap.ts:65

___

### up

• **up**: [`Nullable`](../modules.md#nullable)`ArrayBufferView`

The pixel array for the up face.
This is stored in format, left to right, up to down format.

#### Defined in

https://github.com/babylon.js/core/src/Misc/HighDynamicRange/panoramaToCubemap.ts:38
