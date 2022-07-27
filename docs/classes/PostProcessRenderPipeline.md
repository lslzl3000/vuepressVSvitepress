[@dev/core](../README.md) / [Exports](../modules.md) / PostProcessRenderPipeline

# Class: PostProcessRenderPipeline

PostProcessRenderPipeline

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_postprocessrenderpipeline

## Hierarchy

- **`PostProcessRenderPipeline`**

  ↳ [`DefaultRenderingPipeline`](DefaultRenderingPipeline.md)

  ↳ [`LensRenderingPipeline`](LensRenderingPipeline.md)

  ↳ [`SSAO2RenderingPipeline`](SSAO2RenderingPipeline.md)

  ↳ [`SSAORenderingPipeline`](SSAORenderingPipeline.md)

  ↳ [`StandardRenderingPipeline`](StandardRenderingPipeline.md)

## Table of contents

### Constructors

- [constructor](PostProcessRenderPipeline.md#constructor)

### Properties

- [\_renderEffects](PostProcessRenderPipeline.md#_rendereffects)
- [\_renderEffectsForIsolatedPass](PostProcessRenderPipeline.md#_rendereffectsforisolatedpass)
- [inspectableCustomProperties](PostProcessRenderPipeline.md#inspectablecustomproperties)

### Accessors

- [cameras](PostProcessRenderPipeline.md#cameras)
- [isSupported](PostProcessRenderPipeline.md#issupported)
- [name](PostProcessRenderPipeline.md#name)

### Methods

- [\_enableMSAAOnFirstPostProcess](PostProcessRenderPipeline.md#_enablemsaaonfirstpostprocess)
- [addEffect](PostProcessRenderPipeline.md#addeffect)
- [dispose](PostProcessRenderPipeline.md#dispose)
- [getClassName](PostProcessRenderPipeline.md#getclassname)
- [setPrePassRenderer](PostProcessRenderPipeline.md#setprepassrenderer)

## Constructors

### constructor

• **new PostProcessRenderPipeline**(`_engine`, `name`)

Initializes a PostProcessRenderPipeline

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `_engine` | [`Engine`](Engine.md) | engine to add the pipeline to |
| `name` | `string` | name of the pipeline |

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderPipeline.ts:51

## Properties

### \_renderEffects

• `Private` **\_renderEffects**: `Object`

#### Index signature

▪ [key: `string`]: [`PostProcessRenderEffect`](PostProcessRenderEffect.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderPipeline.ts:16

___

### \_renderEffectsForIsolatedPass

• `Private` **\_renderEffectsForIsolatedPass**: [`PostProcessRenderEffect`](PostProcessRenderEffect.md)[]

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderPipeline.ts:17

___

### inspectableCustomProperties

• **inspectableCustomProperties**: [`IInspectable`](../interfaces/IInspectable.md)[]

List of inspectable custom properties (used by the Inspector)

**`See`**

https://doc.babylonjs.com/how_to/debug_layer#extensibility

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderPipeline.ts:23

## Accessors

### cameras

• `get` **cameras**(): [`Camera`](Camera.md)[]

Gets the list of attached cameras

#### Returns

[`Camera`](Camera.md)[]

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderPipeline.ts:42

___

### isSupported

• `get` **isSupported**(): `boolean`

If all the render effects in the pipeline are supported

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderPipeline.ts:71

___

### name

• `get` **name**(): `string`

Gets pipeline name

#### Returns

`string`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderPipeline.ts:37

## Methods

### \_enableMSAAOnFirstPostProcess

▸ `Protected` **_enableMSAAOnFirstPostProcess**(`sampleCount`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `sampleCount` | `number` |

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderPipeline.ts:228

___

### addEffect

▸ **addEffect**(`renderEffect`): `void`

Adds an effect to the pipeline

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `renderEffect` | [`PostProcessRenderEffect`](PostProcessRenderEffect.md) | the effect to add |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderPipeline.ts:87

___

### dispose

▸ **dispose**(): `void`

Disposes of the pipeline

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderPipeline.ts:258

___

### getClassName

▸ **getClassName**(): `string`

Gets the class name

#### Returns

`string`

"PostProcessRenderPipeline"

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderPipeline.ts:64

___

### setPrePassRenderer

▸ **setPrePassRenderer**(`prePassRenderer`): `boolean`

Sets the required values to the prepass renderer.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `prePassRenderer` | [`PrePassRenderer`](PrePassRenderer.md) | defines the prepass renderer to setup. |

#### Returns

`boolean`

true if the pre pass is needed.

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderPipeline.ts:250
