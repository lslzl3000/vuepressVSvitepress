[@dev/core](../README.md) / [Exports](../modules.md) / PostProcessRenderEffect

# Class: PostProcessRenderEffect

This represents a set of one or more post processes in Babylon.
A post process can be used to apply a shader to a texture after it is rendered.

**`Example`**

```ts
https://doc.babylonjs.com/how_to/how_to_use_postprocessrenderpipeline
```

## Hierarchy

- **`PostProcessRenderEffect`**

  ↳ [`BloomEffect`](BloomEffect.md)

  ↳ [`DepthOfFieldEffect`](DepthOfFieldEffect.md)

## Table of contents

### Constructors

- [constructor](PostProcessRenderEffect.md#constructor)

### Properties

- [\_cameras](PostProcessRenderEffect.md#_cameras)
- [\_getPostProcesses](PostProcessRenderEffect.md#_getpostprocesses)
- [\_indicesForCamera](PostProcessRenderEffect.md#_indicesforcamera)
- [\_postProcesses](PostProcessRenderEffect.md#_postprocesses)
- [\_singleInstance](PostProcessRenderEffect.md#_singleinstance)

### Accessors

- [isSupported](PostProcessRenderEffect.md#issupported)

### Methods

- [getPostProcesses](PostProcessRenderEffect.md#getpostprocesses)

## Constructors

### constructor

• **new PostProcessRenderEffect**(`engine`, `name`, `getPostProcesses`, `singleInstance?`)

Instantiates a post process render effect.
A post process can be used to apply a shader to a texture after it is rendered.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `engine` | [`Engine`](Engine.md) | The engine the effect is tied to |
| `name` | `string` | The name of the effect |
| `getPostProcesses` | () => [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md) \| [`PostProcess`](PostProcess.md)[] | A function that returns a set of post processes which the effect will run in order to be run. |
| `singleInstance?` | `boolean` | False if this post process can be run on multiple cameras. (default: true) |

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderEffect.ts:34

## Properties

### \_cameras

• `Private` **\_cameras**: `Object`

#### Index signature

▪ [key: `string`]: [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderEffect.ts:17

___

### \_getPostProcesses

• `Private` **\_getPostProcesses**: () => [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md) \| [`PostProcess`](PostProcess.md)[]

#### Type declaration

▸ (): [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md) \| [`PostProcess`](PostProcess.md)[]

##### Returns

[`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md) \| [`PostProcess`](PostProcess.md)[]

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderEffect.ts:13

___

### \_indicesForCamera

• `Private` **\_indicesForCamera**: `Object`

#### Index signature

▪ [key: `string`]: `number`[]

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderEffect.ts:18

___

### \_postProcesses

• `Private` **\_postProcesses**: `Object`

#### Index signature

▪ [Key: `string`]: [`PostProcess`](PostProcess.md)[]

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderEffect.ts:12

___

### \_singleInstance

• `Private` **\_singleInstance**: `boolean`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderEffect.ts:15

## Accessors

### isSupported

• `get` **isSupported**(): `boolean`

Checks if all the post processes in the effect are supported.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderEffect.ts:49

## Methods

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

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderEffect.ts:249
