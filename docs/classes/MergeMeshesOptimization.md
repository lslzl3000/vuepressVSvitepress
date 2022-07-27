[@dev/core](../README.md) / [Exports](../modules.md) / MergeMeshesOptimization

# Class: MergeMeshesOptimization

Defines an optimization used to merge meshes with compatible materials

**`Description`**

More details at https://doc.babylonjs.com/how_to/how_to_use_sceneoptimizer

## Hierarchy

- [`SceneOptimization`](SceneOptimization.md)

  ↳ **`MergeMeshesOptimization`**

## Table of contents

### Constructors

- [constructor](MergeMeshesOptimization.md#constructor)

### Properties

- [priority](MergeMeshesOptimization.md#priority)
- [\_UpdateSelectionTree](MergeMeshesOptimization.md#_updateselectiontree)

### Accessors

- [UpdateSelectionTree](MergeMeshesOptimization.md#updateselectiontree)

### Methods

- [\_canBeMerged](MergeMeshesOptimization.md#_canbemerged)
- [apply](MergeMeshesOptimization.md#apply)
- [getDescription](MergeMeshesOptimization.md#getdescription)

## Constructors

### constructor

• **new MergeMeshesOptimization**(`priority?`)

Creates the SceneOptimization object

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `priority` | `number` | `0` | defines the priority of this optimization (0 by default which means first in the list) |

#### Inherited from

[SceneOptimization](SceneOptimization.md).[constructor](SceneOptimization.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:37

## Properties

### priority

• **priority**: `number` = `0`

#### Inherited from

[SceneOptimization](SceneOptimization.md).[priority](SceneOptimization.md#priority)

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:41

___

### \_UpdateSelectionTree

▪ `Static` `Private` **\_UpdateSelectionTree**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:341

## Accessors

### UpdateSelectionTree

• `Static` `get` **UpdateSelectionTree**(): `boolean`

Gets or sets a boolean which defines if optimization octree has to be updated

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:346

• `Static` `set` **UpdateSelectionTree**(`value`): `void`

Gets or sets a boolean which defines if optimization octree has to be updated

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:353

## Methods

### \_canBeMerged

▸ `Private` **_canBeMerged**(`abstractMesh`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `abstractMesh` | [`AbstractMesh`](AbstractMesh.md) |

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:365

___

### apply

▸ **apply**(`scene`, `optimizer`, `updateSelectionTree?`): `boolean`

This function will be called by the SceneOptimizer when its priority is reached in order to apply the change required by the current optimization

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | defines the current scene where to apply this optimization |
| `optimizer` | [`SceneOptimizer`](SceneOptimizer.md) | defines the current optimizer |
| `updateSelectionTree?` | `boolean` | defines that the selection octree has to be updated (false by default) |

#### Returns

`boolean`

true if everything that can be done was applied

#### Overrides

[SceneOptimization](SceneOptimization.md).[apply](SceneOptimization.md#apply)

#### Defined in

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:398

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

https://github.com/babylon.js/core/src/Misc/sceneOptimizer.ts:361
