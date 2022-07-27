[@dev/core](../README.md) / [Exports](../modules.md) / Octree

# Class: OctreeT

Octrees are a really powerful data structure that can quickly select entities based on space coordinates.

**`See`**

https://doc.babylonjs.com/how_to/optimizing_your_scene_with_octrees

## Type parameters

| Name |
| :------ |
| `T` |

## Table of contents

### Constructors

- [constructor](Octree.md#constructor)

### Properties

- [\_creationFunc](Octree.md#_creationfunc)
- [\_maxBlockCapacity](Octree.md#_maxblockcapacity)
- [\_selectionContent](Octree.md#_selectioncontent)
- [blocks](Octree.md#blocks)
- [dynamicContent](Octree.md#dynamiccontent)
- [maxDepth](Octree.md#maxdepth)

### Methods

- [addMesh](Octree.md#addmesh)
- [intersects](Octree.md#intersects)
- [intersectsRay](Octree.md#intersectsray)
- [removeMesh](Octree.md#removemesh)
- [select](Octree.md#select)
- [update](Octree.md#update)
- [CreationFuncForMeshes](Octree.md#creationfuncformeshes)
- [CreationFuncForSubMeshes](Octree.md#creationfuncforsubmeshes)

## Constructors

### constructor

• **new Octree**`T`(`creationFunc`, `maxBlockCapacity?`, `maxDepth?`)

Creates a octree

**`See`**

https://doc.babylonjs.com/how_to/optimizing_your_scene_with_octrees

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `creationFunc` | (`entry`: `T`, `block`: [`OctreeBlock`](OctreeBlock.md)`T`) => `void` | `undefined` | function to be used to instantiate the octree |
| `maxBlockCapacity?` | `number` | `undefined` | defines the maximum number of meshes you want on your octree's leaves (default: 64) |
| `maxDepth` | `number` | `2` | defines the maximum depth (sub-levels) for your octree. Default value is 2, which means 8 8 8 = 512 blocks :) (This parameter takes precedence over capacity.) |

#### Defined in

packages/dev/core/src/Culling/Octrees/octree.ts:35

## Properties

### \_creationFunc

• `Private` **\_creationFunc**: (`entry`: `T`, `block`: [`OctreeBlock`](OctreeBlock.md)`T`) => `void`

#### Type declaration

▸ (`entry`, `block`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `entry` | `T` |
| `block` | [`OctreeBlock`](OctreeBlock.md)`T` |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Culling/Octrees/octree.ts:26

___

### \_maxBlockCapacity

• `Private` **\_maxBlockCapacity**: `number`

#### Defined in

packages/dev/core/src/Culling/Octrees/octree.ts:24

___

### \_selectionContent

• `Private` **\_selectionContent**: [`SmartArrayNoDuplicate`](SmartArrayNoDuplicate.md)`T`

#### Defined in

packages/dev/core/src/Culling/Octrees/octree.ts:25

___

### blocks

• **blocks**: [`OctreeBlock`](OctreeBlock.md)`T`[]

Blocks within the octree containing objects

#### Defined in

packages/dev/core/src/Culling/Octrees/octree.ts:18

___

### dynamicContent

• **dynamicContent**: `T`[]

Content stored in the octree

#### Defined in

packages/dev/core/src/Culling/Octrees/octree.ts:22

___

### maxDepth

• **maxDepth**: `number` = `2`

#### Defined in

packages/dev/core/src/Culling/Octrees/octree.ts:39

## Methods

### addMesh

▸ **addMesh**(`entry`): `void`

Adds a mesh to the octree

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `entry` | `T` | Mesh to add to the octree |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Culling/Octrees/octree.ts:61

___

### intersects

▸ **intersects**(`sphereCenter`, `sphereRadius`, `allowDuplicate?`): [`SmartArray`](SmartArray.md)`T`

Test if the octree intersect with the given bounding sphere and if yes, then add its content to the selection array

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sphereCenter` | [`Vector3`](Vector3.md) | defines the bounding sphere center |
| `sphereRadius` | `number` | defines the bounding sphere radius |
| `allowDuplicate?` | `boolean` | defines if the selection array can contains duplicated entries |

#### Returns

[`SmartArray`](SmartArray.md)`T`

an array of objects that intersect the sphere

#### Defined in

packages/dev/core/src/Culling/Octrees/octree.ts:109

___

### intersectsRay

▸ **intersectsRay**(`ray`): [`SmartArray`](SmartArray.md)`T`

Test if the octree intersect with the given ray and if yes, then add its content to resulting array

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ray` | [`Ray`](Ray.md) | defines the ray to test with |

#### Returns

[`SmartArray`](SmartArray.md)`T`

array of intersected objects

#### Defined in

packages/dev/core/src/Culling/Octrees/octree.ts:131

___

### removeMesh

▸ **removeMesh**(`entry`): `void`

Remove an element from the octree

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `entry` | `T` | defines the element to remove |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Culling/Octrees/octree.ts:72

___

### select

▸ **select**(`frustumPlanes`, `allowDuplicate?`): [`SmartArray`](SmartArray.md)`T`

Selects an array of meshes within the frustum

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `frustumPlanes` | [`Plane`](Plane.md)[] | The frustum planes to use which will select all meshes within it |
| `allowDuplicate?` | `boolean` | If duplicate objects are allowed in the resulting object array |

#### Returns

[`SmartArray`](SmartArray.md)`T`

array of meshes within the frustum

#### Defined in

packages/dev/core/src/Culling/Octrees/octree.ts:85

___

### update

▸ **update**(`worldMin`, `worldMax`, `entries`): `void`

Updates the octree by adding blocks for the passed in meshes within the min and max world parameters

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `worldMin` | [`Vector3`](Vector3.md) | worldMin for the octree blocks var blockSize = new Vector3((worldMax.x - worldMin.x) / 2, (worldMax.y - worldMin.y) / 2, (worldMax.z - worldMin.z) / 2); |
| `worldMax` | [`Vector3`](Vector3.md) | worldMax for the octree blocks var blockSize = new Vector3((worldMax.x - worldMin.x) / 2, (worldMax.y - worldMin.y) / 2, (worldMax.z - worldMin.z) / 2); |
| `entries` | `T`[] | meshes to be added to the octree blocks |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Culling/Octrees/octree.ts:53

___

### CreationFuncForMeshes

▸ `Static` **CreationFuncForMeshes**(`entry`, `block`): `void`

Adds a mesh into the octree block if it intersects the block

#### Parameters

| Name | Type |
| :------ | :------ |
| `entry` | [`AbstractMesh`](AbstractMesh.md) |
| `block` | [`OctreeBlock`](OctreeBlock.md)[`AbstractMesh`](AbstractMesh.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Culling/Octrees/octree.ts:149

___

### CreationFuncForSubMeshes

▸ `Static` **CreationFuncForSubMeshes**(`entry`, `block`): `void`

Adds a submesh into the octree block if it intersects the block

#### Parameters

| Name | Type |
| :------ | :------ |
| `entry` | [`SubMesh`](SubMesh.md) |
| `block` | [`OctreeBlock`](OctreeBlock.md)[`SubMesh`](SubMesh.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Culling/Octrees/octree.ts:161
