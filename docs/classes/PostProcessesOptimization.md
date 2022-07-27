[@dev/core](../README.md) / [Exports](../modules.md) / PostProcessesOptimization

# Class: PostProcessesOptimization

Defines an optimization used to turn post-processes off

**`Description`**

More details at https://doc.babylonjs.com/how_to/how_to_use_sceneoptimizer

## Hierarchy

- [`SceneOptimization`](SceneOptimization.md)

  ↳ **`PostProcessesOptimization`**

## Table of contents

### Constructors

- [constructor](PostProcessesOptimization.md#constructor)

### Properties

- [priority](PostProcessesOptimization.md#priority)

### Methods

- [apply](PostProcessesOptimization.md#apply)
- [getDescription](PostProcessesOptimization.md#getdescription)

## Constructors

### constructor

• **new PostProcessesOptimization**(`priority?`)

Creates the SceneOptimization object

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `priority` | `number` | `0` | defines the priority of this optimization (0 by default which means first in the list) |

#### Inherited from

[SceneOptimization](SceneOptimization.md).[constructor](SceneOptimization.md#constructor)

#### Defined in

packages/dev/core/src/Misc/sceneOptimizer.ts:37

## Properties

### priority

• **priority**: `number` = `0`

#### Inherited from

[SceneOptimization](SceneOptimization.md).[priority](SceneOptimization.md#priority)

#### Defined in

packages/dev/core/src/Misc/sceneOptimizer.ts:41

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

packages/dev/core/src/Misc/sceneOptimizer.ts:214

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

packages/dev/core/src/Misc/sceneOptimizer.ts:204
