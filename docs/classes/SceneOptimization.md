[@dev/core](../README.md) / [Exports](../modules.md) / SceneOptimization

# Class: SceneOptimization

Defines the root class used to create scene optimization to use with SceneOptimizer

**`Description`**

More details at https://doc.babylonjs.com/how_to/how_to_use_sceneoptimizer

## Hierarchy

- **`SceneOptimization`**

  ↳ [`TextureOptimization`](TextureOptimization.md)

  ↳ [`HardwareScalingOptimization`](HardwareScalingOptimization.md)

  ↳ [`ShadowsOptimization`](ShadowsOptimization.md)

  ↳ [`PostProcessesOptimization`](PostProcessesOptimization.md)

  ↳ [`LensFlaresOptimization`](LensFlaresOptimization.md)

  ↳ [`CustomOptimization`](CustomOptimization.md)

  ↳ [`ParticlesOptimization`](ParticlesOptimization.md)

  ↳ [`RenderTargetsOptimization`](RenderTargetsOptimization.md)

  ↳ [`MergeMeshesOptimization`](MergeMeshesOptimization.md)

## Table of contents

### Constructors

- [constructor](SceneOptimization.md#constructor)

### Properties

- [priority](SceneOptimization.md#priority)

### Methods

- [apply](SceneOptimization.md#apply)
- [getDescription](SceneOptimization.md#getdescription)

## Constructors

### constructor

• **new SceneOptimization**(`priority?`)

Creates the SceneOptimization object

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `priority` | `number` | `0` | defines the priority of this optimization (0 by default which means first in the list) |

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:37

## Properties

### priority

• **priority**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:41

## Methods

### apply

▸ **apply**(`scene`, `optimizer`): `boolean`

This function will be called by the SceneOptimizer when its priority is reached in order to apply the change required by the current optimization

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | defines the current scene where to apply this optimization |
| `optimizer` | [`SceneOptimizer`](SceneOptimizer.md) | defines the current optimizer |

#### Returns

`boolean`

true if everything that can be done was applied

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:29

___

### getDescription

▸ **getDescription**(): `string`

Gets a string describing the action executed by the current optimization

#### Returns

`string`

description string

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:19
