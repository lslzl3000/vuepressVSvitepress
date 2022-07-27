[@dev/core](../README.md) / [Exports](../modules.md) / SimplificationSettings

# Class: SimplificationSettings

Class used to specify simplification options

**`See`**

https://doc.babylonjs.com/how_to/in-browser_mesh_simplification

## Implements

- [`ISimplificationSettings`](../interfaces/ISimplificationSettings.md)

## Table of contents

### Constructors

- [constructor](SimplificationSettings.md#constructor)

### Properties

- [distance](SimplificationSettings.md#distance)
- [optimizeMesh](SimplificationSettings.md#optimizemesh)
- [quality](SimplificationSettings.md#quality)

## Constructors

### constructor

• **new SimplificationSettings**(`quality`, `distance`, `optimizeMesh?`)

Creates a SimplificationSettings

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `quality` | `number` | expected quality |
| `distance` | `number` | distance when this optimized version should be used |
| `optimizeMesh?` | `boolean` | already optimized mesh |

#### Defined in

https://github.com/babylon.js/core/src/Meshes/meshSimplification.ts:54

## Properties

### distance

• **distance**: `number`

Gets or sets the distance when this optimized version should be used

#### Implementation of

[ISimplificationSettings](../interfaces/ISimplificationSettings.md).[distance](../interfaces/ISimplificationSettings.md#distance)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/meshSimplification.ts:58

___

### optimizeMesh

• `Optional` **optimizeMesh**: `boolean`

Gets an already optimized mesh

#### Implementation of

[ISimplificationSettings](../interfaces/ISimplificationSettings.md).[optimizeMesh](../interfaces/ISimplificationSettings.md#optimizemesh)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/meshSimplification.ts:60

___

### quality

• **quality**: `number`

Gets or sets the expected quality

#### Implementation of

[ISimplificationSettings](../interfaces/ISimplificationSettings.md).[quality](../interfaces/ISimplificationSettings.md#quality)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/meshSimplification.ts:56
