[@dev/core](../README.md) / [Exports](../modules.md) / SceneOptions

# Interface: SceneOptions

Interface defining initialization parameters for Scene class

## Table of contents

### Properties

- [useClonedMeshMap](SceneOptions.md#useclonedmeshmap)
- [useGeometryUniqueIdsMap](SceneOptions.md#usegeometryuniqueidsmap)
- [useMaterialMeshMap](SceneOptions.md#usematerialmeshmap)
- [virtual](SceneOptions.md#virtual)

## Properties

### useClonedMeshMap

• `Optional` **useClonedMeshMap**: `boolean`

Defines that each mesh of the scene should keep up-to-date a map of referencing cloned meshes for fast disposing
It will improve performance when the number of mesh becomes important, but might consume a bit more memory

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:124

___

### useGeometryUniqueIdsMap

• `Optional` **useGeometryUniqueIdsMap**: `boolean`

Defines that scene should keep up-to-date a map of geometry to enable fast look-up by uniqueId
It will improve performance when the number of geometries becomes important.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:112

___

### useMaterialMeshMap

• `Optional` **useMaterialMeshMap**: `boolean`

Defines that each material of the scene should keep up-to-date a map of referencing meshes for fast disposing
It will improve performance when the number of mesh becomes important, but might consume a bit more memory

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:118

___

### virtual

• `Optional` **virtual**: `boolean`

Defines if the creation of the scene should impact the engine (Eg. UtilityLayer's scene)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:127
