[@dev/core](../README.md) / [Exports](../modules.md) / CubeMapToSphericalPolynomialTools

# Class: CubeMapToSphericalPolynomialTools

Helper class dealing with the extraction of spherical polynomial dataArray
from a cube map.

## Table of contents

### Constructors

- [constructor](CubeMapToSphericalPolynomialTools.md#constructor)

### Properties

- [\_FileFaces](CubeMapToSphericalPolynomialTools.md#_filefaces)

### Methods

- [ConvertCubeMapTextureToSphericalPolynomial](CubeMapToSphericalPolynomialTools.md#convertcubemaptexturetosphericalpolynomial)
- [ConvertCubeMapToSphericalPolynomial](CubeMapToSphericalPolynomialTools.md#convertcubemaptosphericalpolynomial)
- [\_AreaElement](CubeMapToSphericalPolynomialTools.md#_areaelement)

## Constructors

### constructor

• **new CubeMapToSphericalPolynomialTools**()

## Properties

### \_FileFaces

▪ `Static` `Private` **\_FileFaces**: `FileFaceOrientation`[]

#### Defined in

https://github.com/babylon.js/core/src/Misc/HighDynamicRange/cubemapToSphericalPolynomial.ts:30

## Methods

### ConvertCubeMapTextureToSphericalPolynomial

▸ `Static` **ConvertCubeMapTextureToSphericalPolynomial**(`texture`): [`Nullable`](../modules.md#nullable)`Promise`[`SphericalPolynomial`](SphericalPolynomial.md)

Converts a texture to the according Spherical Polynomial data.
This extracts the first 3 orders only as they are the only one used in the lighting.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `texture` | [`BaseTexture`](BaseTexture.md) | The texture to extract the information from. |

#### Returns

[`Nullable`](../modules.md#nullable)`Promise`[`SphericalPolynomial`](SphericalPolynomial.md)

The Spherical Polynomial data.

#### Defined in

https://github.com/babylon.js/core/src/Misc/HighDynamicRange/cubemapToSphericalPolynomial.ts:46

___

### ConvertCubeMapToSphericalPolynomial

▸ `Static` **ConvertCubeMapToSphericalPolynomial**(`cubeInfo`): [`SphericalPolynomial`](SphericalPolynomial.md)

Converts a cubemap to the according Spherical Polynomial data.
This extracts the first 3 orders only as they are the only one used in the lighting.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `cubeInfo` | [`CubeMapInfo`](../interfaces/CubeMapInfo.md) | The Cube map to extract the information from. |

#### Returns

[`SphericalPolynomial`](SphericalPolynomial.md)

The Spherical Polynomial data.

#### Defined in

https://github.com/babylon.js/core/src/Misc/HighDynamicRange/cubemapToSphericalPolynomial.ts:116

___

### \_AreaElement

▸ `Static` `Private` **_AreaElement**(`x`, `y`): `number`

Compute the area on the unit sphere of the rectangle defined by (x,y) and the origin
See https://www.rorydriscoll.com/2012/01/15/cubemap-texel-solid-angle/

#### Parameters

| Name | Type |
| :------ | :------ |
| `x` | `number` |
| `y` | `number` |

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Misc/HighDynamicRange/cubemapToSphericalPolynomial.ts:105
