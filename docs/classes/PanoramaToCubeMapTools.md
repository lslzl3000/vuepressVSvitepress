[@dev/core](../README.md) / [Exports](../modules.md) / PanoramaToCubeMapTools

# Class: PanoramaToCubeMapTools

Helper class useful to convert panorama picture to their cubemap representation in 6 faces.

## Table of contents

### Constructors

- [constructor](PanoramaToCubeMapTools.md#constructor)

### Properties

- [FACE\_BACK](PanoramaToCubeMapTools.md#face_back)
- [FACE\_DOWN](PanoramaToCubeMapTools.md#face_down)
- [FACE\_FRONT](PanoramaToCubeMapTools.md#face_front)
- [FACE\_LEFT](PanoramaToCubeMapTools.md#face_left)
- [FACE\_RIGHT](PanoramaToCubeMapTools.md#face_right)
- [FACE\_UP](PanoramaToCubeMapTools.md#face_up)

### Methods

- [CalcProjectionSpherical](PanoramaToCubeMapTools.md#calcprojectionspherical)
- [ConvertPanoramaToCubemap](PanoramaToCubeMapTools.md#convertpanoramatocubemap)
- [CreateCubemapTexture](PanoramaToCubeMapTools.md#createcubemaptexture)

## Constructors

### constructor

• **new PanoramaToCubeMapTools**()

## Properties

### FACE\_BACK

▪ `Static` `Private` **FACE\_BACK**: [`Vector3`](Vector3.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Misc/HighDynamicRange/panoramaToCubemap.ts:80

___

### FACE\_DOWN

▪ `Static` `Private` **FACE\_DOWN**: [`Vector3`](Vector3.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Misc/HighDynamicRange/panoramaToCubemap.ts:81

___

### FACE\_FRONT

▪ `Static` `Private` **FACE\_FRONT**: [`Vector3`](Vector3.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Misc/HighDynamicRange/panoramaToCubemap.ts:79

___

### FACE\_LEFT

▪ `Static` `Private` **FACE\_LEFT**: [`Vector3`](Vector3.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Misc/HighDynamicRange/panoramaToCubemap.ts:77

___

### FACE\_RIGHT

▪ `Static` `Private` **FACE\_RIGHT**: [`Vector3`](Vector3.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Misc/HighDynamicRange/panoramaToCubemap.ts:78

___

### FACE\_UP

▪ `Static` `Private` **FACE\_UP**: [`Vector3`](Vector3.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Misc/HighDynamicRange/panoramaToCubemap.ts:82

## Methods

### CalcProjectionSpherical

▸ `Static` `Private` **CalcProjectionSpherical**(`vDir`, `float32Array`, `inputWidth`, `inputHeight`): `any`

#### Parameters

| Name | Type |
| :------ | :------ |
| `vDir` | [`Vector3`](Vector3.md) |
| `float32Array` | `Float32Array` |
| `inputWidth` | `number` |
| `inputHeight` | `number` |

#### Returns

`any`

#### Defined in

https://github.com/babylon.js/core/src/Misc/HighDynamicRange/panoramaToCubemap.ts:158

___

### ConvertPanoramaToCubemap

▸ `Static` **ConvertPanoramaToCubemap**(`float32Array`, `inputWidth`, `inputHeight`, `size`): [`CubeMapInfo`](../interfaces/CubeMapInfo.md)

Converts a panorama stored in RGB right to left up to down format into a cubemap (6 faces).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `float32Array` | `Float32Array` | The source data. |
| `inputWidth` | `number` | The width of the input panorama. |
| `inputHeight` | `number` | The height of the input panorama. |
| `size` | `number` | The willing size of the generated cubemap (each faces will be size * size pixels) |

#### Returns

[`CubeMapInfo`](../interfaces/CubeMapInfo.md)

The cubemap data

#### Defined in

https://github.com/babylon.js/core/src/Misc/HighDynamicRange/panoramaToCubemap.ts:93

___

### CreateCubemapTexture

▸ `Static` `Private` **CreateCubemapTexture**(`texSize`, `faceData`, `float32Array`, `inputWidth`, `inputHeight`): `Float32Array`

#### Parameters

| Name | Type |
| :------ | :------ |
| `texSize` | `number` |
| `faceData` | [`Vector3`](Vector3.md)[] |
| `float32Array` | `Float32Array` |
| `inputWidth` | `number` |
| `inputHeight` | `number` |

#### Returns

`Float32Array`

#### Defined in

https://github.com/babylon.js/core/src/Misc/HighDynamicRange/panoramaToCubemap.ts:123
