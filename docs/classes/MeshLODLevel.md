[@dev/core](../README.md) / [Exports](../modules.md) / MeshLODLevel

# Class: MeshLODLevel

Class used to represent a specific level of detail of a mesh

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_lod

## Table of contents

### Constructors

- [constructor](MeshLODLevel.md#constructor)

### Properties

- [distanceOrScreenCoverage](MeshLODLevel.md#distanceorscreencoverage)
- [mesh](MeshLODLevel.md#mesh)

## Constructors

### constructor

• **new MeshLODLevel**(`distanceOrScreenCoverage`, `mesh`)

Creates a new LOD level

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `distanceOrScreenCoverage` | `number` | defines either the distance or the screen coverage where this level should start being displayed |
| `mesh` | [`Nullable`](../modules.md#nullable)[`Mesh`](Mesh.md) | defines the mesh to use to render this level |

#### Defined in

packages/dev/core/src/Meshes/meshLODLevel.ts:14

## Properties

### distanceOrScreenCoverage

• **distanceOrScreenCoverage**: `number`

#### Defined in

packages/dev/core/src/Meshes/meshLODLevel.ts:16

___

### mesh

• **mesh**: [`Nullable`](../modules.md#nullable)[`Mesh`](Mesh.md)

#### Defined in

packages/dev/core/src/Meshes/meshLODLevel.ts:18
