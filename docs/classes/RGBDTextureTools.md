[@dev/core](../README.md) / [Exports](../modules.md) / RGBDTextureTools

# Class: RGBDTextureTools

Class used to host RGBD texture specific utilities

## Table of contents

### Constructors

- [constructor](RGBDTextureTools.md#constructor)

### Methods

- [EncodeTextureToRGBD](RGBDTextureTools.md#encodetexturetorgbd)
- [ExpandRGBDTexture](RGBDTextureTools.md#expandrgbdtexture)

## Constructors

### constructor

• **new RGBDTextureTools**()

## Methods

### EncodeTextureToRGBD

▸ `Static` **EncodeTextureToRGBD**(`internalTexture`, `scene`, `outputTextureType?`): `Promise`[`InternalTexture`](InternalTexture.md)

Encode the texture to RGBD if possible.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `internalTexture` | [`InternalTexture`](InternalTexture.md) | `undefined` | the texture to encode |
| `scene` | [`Scene`](Scene.md) | `undefined` | the scene hosting the texture |
| `outputTextureType` | `number` | `Constants.TEXTURETYPE_UNSIGNED_BYTE` | type of the texture in which the encoding is performed |

#### Returns

`Promise`[`InternalTexture`](InternalTexture.md)

a promise with the internalTexture having its texture replaced by the result of the processing

#### Defined in

https://github.com/babylon.js/core/src/Misc/rgbdTextureTools.ts:121

___

### ExpandRGBDTexture

▸ `Static` **ExpandRGBDTexture**(`texture`): `void`

Expand the RGBD Texture from RGBD to Half Float if possible.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `texture` | [`Texture`](Texture.md) | the texture to expand. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/rgbdTextureTools.ts:21
