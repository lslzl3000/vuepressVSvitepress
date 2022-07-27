[@dev/core](../README.md) / [Exports](../modules.md) / HDRFiltering

# Class: HDRFiltering

Filters HDR maps to get correct renderings of PBR reflections

## Table of contents

### Constructors

- [constructor](HDRFiltering.md#constructor)

### Properties

- [\_effectRenderer](HDRFiltering.md#_effectrenderer)
- [\_effectWrapper](HDRFiltering.md#_effectwrapper)
- [\_engine](HDRFiltering.md#_engine)
- [\_lodGenerationOffset](HDRFiltering.md#_lodgenerationoffset)
- [\_lodGenerationScale](HDRFiltering.md#_lodgenerationscale)
- [hdrScale](HDRFiltering.md#hdrscale)
- [quality](HDRFiltering.md#quality)

### Methods

- [\_createEffect](HDRFiltering.md#_createeffect)
- [\_createRenderTarget](HDRFiltering.md#_createrendertarget)
- [\_prefilterInternal](HDRFiltering.md#_prefilterinternal)
- [isReady](HDRFiltering.md#isready)
- [prefilter](HDRFiltering.md#prefilter)

## Constructors

### constructor

• **new HDRFiltering**(`engine`, `options?`)

Instantiates HDR filter for reflection maps

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `engine` | [`ThinEngine`](ThinEngine.md) | Thin engine |
| `options` | `IHDRFilteringOptions` | Options |

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Filtering/hdrFiltering.ts:58

## Properties

### \_effectRenderer

• `Private` **\_effectRenderer**: [`EffectRenderer`](EffectRenderer.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Filtering/hdrFiltering.ts:35

___

### \_effectWrapper

• `Private` **\_effectWrapper**: [`EffectWrapper`](EffectWrapper.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Filtering/hdrFiltering.ts:36

___

### \_engine

• `Private` **\_engine**: [`ThinEngine`](ThinEngine.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Filtering/hdrFiltering.ts:34

___

### \_lodGenerationOffset

• `Private` **\_lodGenerationOffset**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Filtering/hdrFiltering.ts:38

___

### \_lodGenerationScale

• `Private` **\_lodGenerationScale**: `number` = `0.8`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Filtering/hdrFiltering.ts:39

___

### hdrScale

• **hdrScale**: `number` = `1`

Scales pixel intensity for the input HDR map.

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Filtering/hdrFiltering.ts:50

___

### quality

• **quality**: `number` = `Constants.TEXTURE_FILTERING_QUALITY_OFFLINE`

Quality switch for prefiltering. Should be set to `Constants.TEXTURE_FILTERING_QUALITY_OFFLINE` unless
you care about baking speed.

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Filtering/hdrFiltering.ts:45

## Methods

### \_createEffect

▸ `Private` **_createEffect**(`texture`, `onCompiled?`): [`EffectWrapper`](EffectWrapper.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `texture` | [`BaseTexture`](BaseTexture.md) |
| `onCompiled?` | [`Nullable`](../modules.md#nullable)(`effect`: [`Effect`](Effect.md)) => `void` |

#### Returns

[`EffectWrapper`](EffectWrapper.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Filtering/hdrFiltering.ts:151

___

### \_createRenderTarget

▸ `Private` **_createRenderTarget**(`size`): [`RenderTargetWrapper`](RenderTargetWrapper.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `size` | `number` |

#### Returns

[`RenderTargetWrapper`](RenderTargetWrapper.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Filtering/hdrFiltering.ts:65

___

### \_prefilterInternal

▸ `Private` **_prefilterInternal**(`texture`): [`BaseTexture`](BaseTexture.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `texture` | [`BaseTexture`](BaseTexture.md) |

#### Returns

[`BaseTexture`](BaseTexture.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Filtering/hdrFiltering.ts:89

___

### isReady

▸ **isReady**(`texture`): `boolean`

Get a value indicating if the filter is ready to be used

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `texture` | [`BaseTexture`](BaseTexture.md) | Texture to filter |

#### Returns

`boolean`

true if the filter is ready

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Filtering/hdrFiltering.ts:179

___

### prefilter

▸ **prefilter**(`texture`, `onFinished?`): `Promise``void`

Prefilters a cube texture to have mipmap levels representing roughness values.
Prefiltering will be invoked at the end of next rendering pass.
This has to be done once the map is loaded, and has not been prefiltered by a third party software.
See http://blog.selfshadow.com/publications/s2013-shading-course/karis/s2013_pbs_epic_notes_v2.pdf for more information

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `texture` | [`BaseTexture`](BaseTexture.md) | `undefined` | Texture to filter |
| `onFinished` | [`Nullable`](../modules.md#nullable)() => `void` | `null` | Callback when filtering is done |

#### Returns

`Promise``void`

Promise called when prefiltering is done

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Filtering/hdrFiltering.ts:192
