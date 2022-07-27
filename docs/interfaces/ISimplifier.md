[@dev/core](../README.md) / [Exports](../modules.md) / ISimplifier

# Interface: ISimplifier

A simplifier interface for future simplification implementations

**`See`**

https://doc.babylonjs.com/how_to/in-browser_mesh_simplification

## Implemented by

- [`QuadraticErrorSimplification`](../classes/QuadraticErrorSimplification.md)

## Table of contents

### Methods

- [simplify](ISimplifier.md#simplify)

## Methods

### simplify

▸ **simplify**(`settings`, `successCallback`, `errorCallback?`): `void`

Simplification of a given mesh according to the given settings.
Since this requires computation, it is assumed that the function runs async.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `settings` | [`ISimplificationSettings`](ISimplificationSettings.md) | The settings of the simplification, including quality and distance |
| `successCallback` | (`simplifiedMeshes`: [`Mesh`](../classes/Mesh.md)) => `void` | A callback that will be called after the mesh was simplified. |
| `errorCallback?` | () => `void` | in case of an error, this callback will be called. optional. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/meshSimplification.ts:20
