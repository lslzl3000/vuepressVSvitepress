[@dev/core](../README.md) / [Exports](../modules.md) / BloomEffect

# Class: BloomEffect

The bloom effect spreads bright areas of an image to simulate artifacts seen in cameras

## Hierarchy

- [`PostProcessRenderEffect`](PostProcessRenderEffect.md)

  ↳ **`BloomEffect`**

## Table of contents

### Constructors

- [constructor](BloomEffect.md#constructor)

### Properties

- [\_blurX](BloomEffect.md#_blurx)
- [\_blurY](BloomEffect.md#_blury)
- [\_merge](BloomEffect.md#_merge)

### Accessors

- [isSupported](BloomEffect.md#issupported)
- [kernel](BloomEffect.md#kernel)
- [threshold](BloomEffect.md#threshold)
- [weight](BloomEffect.md#weight)

### Methods

- [disposeEffects](BloomEffect.md#disposeeffects)
- [getPostProcesses](BloomEffect.md#getpostprocesses)

## Constructors

### constructor

• **new BloomEffect**(`scene`, `_bloomScale`, `bloomWeight`, `bloomKernel`, `pipelineTextureType?`, `blockCompilation?`)

Creates a new instance of

**`See`**

BloomEffect

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | `undefined` | The scene the effect belongs to. |
| `_bloomScale` | `number` | `undefined` | The ratio of the blur texture to the input texture that should be used to compute the bloom. |
| `bloomWeight` | `number` | `undefined` | The the strength of bloom. |
| `bloomKernel` | `number` | `undefined` | The size of the kernel to be used when applying the blur. |
| `pipelineTextureType` | `number` | `0` | The type of texture to be used when performing the post processing. |
| `blockCompilation` | `boolean` | `false` | If compilation of the shader should not be done in the constructor. The updateEffect method can be used to compile the shader at a later time. (default: false) |

#### Overrides

[PostProcessRenderEffect](PostProcessRenderEffect.md).[constructor](PostProcessRenderEffect.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/bloomEffect.ts:68

## Properties

### \_blurX

• `Private` **\_blurX**: [`BlurPostProcess`](BlurPostProcess.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/bloomEffect.ts:24

___

### \_blurY

• `Private` **\_blurY**: [`BlurPostProcess`](BlurPostProcess.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/bloomEffect.ts:25

___

### \_merge

• `Private` **\_merge**: [`BloomMergePostProcess`](BloomMergePostProcess.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/bloomEffect.ts:26

## Accessors

### isSupported

• `get` **isSupported**(): `boolean`

Checks if all the post processes in the effect are supported.

#### Returns

`boolean`

#### Inherited from

PostProcessRenderEffect.isSupported

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderEffect.ts:49

___

### kernel

• `get` **kernel**(): `number`

Specifies the size of the bloom blur kernel, relative to the final output size

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/bloomEffect.ts:51

• `set` **kernel**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/bloomEffect.ts:54

___

### threshold

• `get` **threshold**(): `number`

The luminance threshold to find bright areas of the image to bloom.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/bloomEffect.ts:31

• `set` **threshold**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/bloomEffect.ts:34

___

### weight

• `get` **weight**(): `number`

The strength of the bloom.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/bloomEffect.ts:41

• `set` **weight**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/bloomEffect.ts:44

## Methods

### disposeEffects

▸ **disposeEffects**(`camera`): `void`

Disposes each of the internal effects for a given camera.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `camera` | [`Camera`](Camera.md) | The camera to dispose the effect on. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/bloomEffect.ts:136

___

### getPostProcesses

▸ **getPostProcesses**(`camera?`): [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)[]

Gets a list of the post processes contained in the effect.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `camera?` | [`Camera`](Camera.md) | The camera to get the post processes on. |

#### Returns

[`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)[]

The list of the post processes in the effect.

#### Inherited from

[PostProcessRenderEffect](PostProcessRenderEffect.md).[getPostProcesses](PostProcessRenderEffect.md#getpostprocesses)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderEffect.ts:249
