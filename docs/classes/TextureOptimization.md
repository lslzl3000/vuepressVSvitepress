[@dev/core](../README.md) / [Exports](../modules.md) / TextureOptimization

# Class: TextureOptimization

Defines an optimization used to reduce the size of render target textures

**`Description`**

More details at https://doc.babylonjs.com/how_to/how_to_use_sceneoptimizer

## Hierarchy

- [`SceneOptimization`](SceneOptimization.md)

  ↳ **`TextureOptimization`**

## Table of contents

### Constructors

- [constructor](TextureOptimization.md#constructor)

### Properties

- [maximumSize](TextureOptimization.md#maximumsize)
- [priority](TextureOptimization.md#priority)
- [step](TextureOptimization.md#step)

### Methods

- [apply](TextureOptimization.md#apply)
- [getDescription](TextureOptimization.md#getdescription)

## Constructors

### constructor

• **new TextureOptimization**(`priority?`, `maximumSize?`, `step?`)

Creates the TextureOptimization object

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `priority` | `number` | `0` | defines the priority of this optimization (0 by default which means first in the list) |
| `maximumSize` | `number` | `1024` | defines the maximum sized allowed for textures (1024 is the default value). If a texture is bigger, it will be scaled down using a factor defined by the step parameter |
| `step` | `number` | `0.5` | defines the factor (0.5 by default) used to scale down textures bigger than maximum sized allowed. |

#### Overrides

[SceneOptimization](SceneOptimization.md).[constructor](SceneOptimization.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:64

## Properties

### maximumSize

• **maximumSize**: `number` = `1024`

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:72

___

### priority

• **priority**: `number` = `0`

#### Inherited from

[SceneOptimization](SceneOptimization.md).[priority](SceneOptimization.md#priority)

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:68

___

### step

• **step**: `number` = `0.5`

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:76

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

#### Overrides

[SceneOptimization](SceneOptimization.md).[apply](SceneOptimization.md#apply)

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:87

___

### getDescription

▸ **getDescription**(): `string`

Gets a string describing the action executed by the current optimization

#### Returns

`string`

description string

#### Overrides

[SceneOptimization](SceneOptimization.md).[getDescription](SceneOptimization.md#getdescription)

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:54
