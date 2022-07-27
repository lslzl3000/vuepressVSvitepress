[@dev/core](../README.md) / [Exports](../modules.md) / ISimplificationSettings

# Interface: ISimplificationSettings

Expected simplification settings.
Quality should be between 0 and 1 (1 being 100%, 0 being 0%)

**`See`**

https://doc.babylonjs.com/how_to/in-browser_mesh_simplification

## Implemented by

- [`SimplificationSettings`](../classes/SimplificationSettings.md)

## Table of contents

### Properties

- [distance](ISimplificationSettings.md#distance)
- [optimizeMesh](ISimplificationSettings.md#optimizemesh)
- [quality](ISimplificationSettings.md#quality)

## Properties

### distance

• **distance**: `number`

Gets or sets the distance when this optimized version should be used

#### Defined in

https://github.com/babylon.js/core/src/Meshes/meshSimplification.ts:36

___

### optimizeMesh

• `Optional` **optimizeMesh**: `boolean`

Gets an already optimized mesh

#### Defined in

https://github.com/babylon.js/core/src/Meshes/meshSimplification.ts:40

___

### quality

• **quality**: `number`

Gets or sets the expected quality

#### Defined in

https://github.com/babylon.js/core/src/Meshes/meshSimplification.ts:32
