[@dev/core](../README.md) / [Exports](../modules.md) / HDRTools

# Class: HDRTools

This groups tools to convert HDR texture to native colors array.

## Table of contents

### Constructors

- [constructor](HDRTools.md#constructor)

### Methods

- [GetCubeMapTextureData](HDRTools.md#getcubemaptexturedata)
- [RGBE\_ReadHeader](HDRTools.md#rgbe_readheader)
- [RGBE\_ReadPixels](HDRTools.md#rgbe_readpixels)
- [\_Ldexp](HDRTools.md#_ldexp)
- [\_RGBEReadPixelsNOTRLE](HDRTools.md#_rgbereadpixelsnotrle)
- [\_RGBEReadPixelsRLE](HDRTools.md#_rgbereadpixelsrle)
- [\_ReadStringLine](HDRTools.md#_readstringline)
- [\_Rgbe2float](HDRTools.md#_rgbe2float)

## Constructors

### constructor

• **new HDRTools**()

## Methods

### GetCubeMapTextureData

▸ `Static` **GetCubeMapTextureData**(`buffer`, `size`): [`CubeMapInfo`](../interfaces/CubeMapInfo.md)

Returns the cubemap information (each faces texture data) extracted from an RGBE texture.
This RGBE texture needs to store the information as a panorama.

More information on this format are available here:
https://en.wikipedia.org/wiki/RGBE_image_format

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `buffer` | `ArrayBuffer` | The binary file stored in an array buffer. |
| `size` | `number` | The expected size of the extracted cubemap. |

#### Returns

[`CubeMapInfo`](../interfaces/CubeMapInfo.md)

The Cube Map information.

#### Defined in

https://github.com/babylon.js/core/src/Misc/HighDynamicRange/hdr.ts:146

___

### RGBE\_ReadHeader

▸ `Static` **RGBE_ReadHeader**(`uint8array`): [`HDRInfo`](../interfaces/HDRInfo.md)

Reads header information from an RGBE texture stored in a native array.
More information on this format are available here:
https://en.wikipedia.org/wiki/RGBE_image_format

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uint8array` | `Uint8Array` | The binary file stored in  native array. |

#### Returns

[`HDRInfo`](../interfaces/HDRInfo.md)

The header information.

#### Defined in

https://github.com/babylon.js/core/src/Misc/HighDynamicRange/hdr.ts:81

___

### RGBE\_ReadPixels

▸ `Static` **RGBE_ReadPixels**(`uint8array`, `hdrInfo`): `Float32Array`

Returns the pixels data extracted from an RGBE texture.
This pixels will be stored left to right up to down in the R G B order in one array.

More information on this format are available here:
https://en.wikipedia.org/wiki/RGBE_image_format

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uint8array` | `Uint8Array` | The binary file stored in an array buffer. |
| `hdrInfo` | [`HDRInfo`](../interfaces/HDRInfo.md) | The header information of the file. |

#### Returns

`Float32Array`

The pixels data in RGB right to left up to down order.

#### Defined in

https://github.com/babylon.js/core/src/Misc/HighDynamicRange/hdr.ts:168

___

### \_Ldexp

▸ `Static` `Private` **_Ldexp**(`mantissa`, `exponent`): `number`

#### Parameters

| Name | Type |
| :------ | :------ |
| `mantissa` | `number` |
| `exponent` | `number` |

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Misc/HighDynamicRange/hdr.ts:28

___

### \_RGBEReadPixelsNOTRLE

▸ `Static` `Private` **_RGBEReadPixelsNOTRLE**(`uint8array`, `hdrInfo`): `Float32Array`

#### Parameters

| Name | Type |
| :------ | :------ |
| `uint8array` | `Uint8Array` |
| `hdrInfo` | [`HDRInfo`](../interfaces/HDRInfo.md) |

#### Returns

`Float32Array`

#### Defined in

https://github.com/babylon.js/core/src/Misc/HighDynamicRange/hdr.ts:257

___

### \_RGBEReadPixelsRLE

▸ `Static` `Private` **_RGBEReadPixelsRLE**(`uint8array`, `hdrInfo`): `Float32Array`

#### Parameters

| Name | Type |
| :------ | :------ |
| `uint8array` | `Uint8Array` |
| `hdrInfo` | [`HDRInfo`](../interfaces/HDRInfo.md) |

#### Returns

`Float32Array`

#### Defined in

https://github.com/babylon.js/core/src/Misc/HighDynamicRange/hdr.ts:172

___

### \_ReadStringLine

▸ `Static` `Private` **_ReadStringLine**(`uint8array`, `startIndex`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `uint8array` | `Uint8Array` |
| `startIndex` | `number` |

#### Returns

`string`

#### Defined in

https://github.com/babylon.js/core/src/Misc/HighDynamicRange/hdr.ts:55

___

### \_Rgbe2float

▸ `Static` `Private` **_Rgbe2float**(`float32array`, `red`, `green`, `blue`, `exponent`, `index`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `float32array` | `Float32Array` |
| `red` | `number` |
| `green` | `number` |
| `blue` | `number` |
| `exponent` | `number` |
| `index` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/HighDynamicRange/hdr.ts:40
