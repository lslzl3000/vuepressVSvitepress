[@dev/core](../README.md) / [Exports](../modules.md) / TextureSampler

# Class: TextureSampler

Class used to store a texture sampler data

## Hierarchy

- **`TextureSampler`**

  ↳ [`InternalTexture`](InternalTexture.md)

## Table of contents

### Constructors

- [constructor](TextureSampler.md#constructor)

### Properties

- [\_useMipMaps](TextureSampler.md#_usemipmaps)
- [samplingMode](TextureSampler.md#samplingmode)

### Accessors

- [anisotropicFilteringLevel](TextureSampler.md#anisotropicfilteringlevel)
- [comparisonFunction](TextureSampler.md#comparisonfunction)
- [useMipMaps](TextureSampler.md#usemipmaps)
- [wrapR](TextureSampler.md#wrapr)
- [wrapU](TextureSampler.md#wrapu)
- [wrapV](TextureSampler.md#wrapv)

### Methods

- [compareSampler](TextureSampler.md#comparesampler)
- [setParameters](TextureSampler.md#setparameters)

## Constructors

### constructor

• **new TextureSampler**()

Creates a Sampler instance

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/textureSampler.ts:113

## Properties

### \_useMipMaps

• `Private` **\_useMipMaps**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/textureSampler.ts:82

___

### samplingMode

• **samplingMode**: `number` = `-1`

Gets the sampling mode of the texture

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/textureSampler.ts:11

## Accessors

### anisotropicFilteringLevel

• `get` **anisotropicFilteringLevel**(): [`Nullable`](../modules.md#nullable)`number`

With compliant hardware and browser (supporting anisotropic filtering)
this defines the level of anisotropic filtering in the texture.
The higher the better but the slower.

#### Returns

[`Nullable`](../modules.md#nullable)`number`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/textureSampler.ts:63

• `set` **anisotropicFilteringLevel**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)`number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/textureSampler.ts:67

___

### comparisonFunction

• `get` **comparisonFunction**(): `number`

Gets or sets the comparison function (Constants.LESS, Constants.EQUAL, etc). Set 0 to not use a comparison function

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/textureSampler.ts:74

• `set` **comparisonFunction**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/textureSampler.ts:78

___

### useMipMaps

• `get` **useMipMaps**(): `boolean`

Indicates to use the mip maps (if available on the texture).
Thanks to this flag, you can instruct the sampler to not sample the mipmaps even if they exist (and if the sampling mode is set to a value that normally samples the mipmaps!)

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/textureSampler.ts:87

• `set` **useMipMaps**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/textureSampler.ts:91

___

### wrapR

• `get` **wrapR**(): [`Nullable`](../modules.md#nullable)`number`

| Value | Type               | Description |
| ----- | ------------------ | ----------- |
| 0     | CLAMP_ADDRESSMODE  |             |
| 1     | WRAP_ADDRESSMODE   |             |
| 2     | MIRROR_ADDRESSMODE |             |

#### Returns

[`Nullable`](../modules.md#nullable)`number`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/textureSampler.ts:50

• `set` **wrapR**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)`number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/textureSampler.ts:54

___

### wrapU

• `get` **wrapU**(): [`Nullable`](../modules.md#nullable)`number`

| Value | Type               | Description |
| ----- | ------------------ | ----------- |
| 0     | CLAMP_ADDRESSMODE  |             |
| 1     | WRAP_ADDRESSMODE   |             |
| 2     | MIRROR_ADDRESSMODE |             |

#### Returns

[`Nullable`](../modules.md#nullable)`number`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/textureSampler.ts:20

• `set` **wrapU**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)`number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/textureSampler.ts:24

___

### wrapV

• `get` **wrapV**(): [`Nullable`](../modules.md#nullable)`number`

| Value | Type               | Description |
| ----- | ------------------ | ----------- |
| 0     | CLAMP_ADDRESSMODE  |             |
| 1     | WRAP_ADDRESSMODE   |             |
| 2     | MIRROR_ADDRESSMODE |             |

#### Returns

[`Nullable`](../modules.md#nullable)`number`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/textureSampler.ts:35

• `set` **wrapV**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)`number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/textureSampler.ts:39

## Methods

### compareSampler

▸ **compareSampler**(`other`): `boolean`

Compares this sampler with another one

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`TextureSampler`](TextureSampler.md) | sampler to compare with |

#### Returns

`boolean`

true if the samplers have the same parametres, else false

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/textureSampler.ts:148

___

### setParameters

▸ **setParameters**(`wrapU?`, `wrapV?`, `wrapR?`, `anisotropicFilteringLevel?`, `samplingMode?`, `comparisonFunction?`): [`TextureSampler`](TextureSampler.md)

Sets all the parameters of the sampler

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `wrapU` | `number` | `Constants.TEXTURE_WRAP_ADDRESSMODE` | u address mode (default: TEXTURE_WRAP_ADDRESSMODE) |
| `wrapV` | `number` | `Constants.TEXTURE_WRAP_ADDRESSMODE` | v address mode (default: TEXTURE_WRAP_ADDRESSMODE) |
| `wrapR` | `number` | `Constants.TEXTURE_WRAP_ADDRESSMODE` | r address mode (default: TEXTURE_WRAP_ADDRESSMODE) |
| `anisotropicFilteringLevel` | `number` | `1` | anisotropic level (default: 1) |
| `samplingMode` | `number` | `Constants.TEXTURE_BILINEAR_SAMPLINGMODE` | sampling mode (default: Constants.TEXTURE_BILINEAR_SAMPLINGMODE) |
| `comparisonFunction` | `number` | `0` | comparison function (default: 0 - no comparison function) |

#### Returns

[`TextureSampler`](TextureSampler.md)

the current sampler instance

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/textureSampler.ts:125
