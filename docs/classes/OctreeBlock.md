[@dev/core](../README.md) / [Exports](../modules.md) / OctreeBlock

# Class: OctreeBlockT

Class used to store a cell in an octree

**`See`**

https://doc.babylonjs.com/how_to/optimizing_your_scene_with_octrees

## Type parameters

| Name |
| :------ |
| `T` |

## Table of contents

### Constructors

- [constructor](OctreeBlock.md#constructor)

### Properties

- [\_boundingVectors](OctreeBlock.md#_boundingvectors)
- [\_capacity](OctreeBlock.md#_capacity)
- [\_creationFunc](OctreeBlock.md#_creationfunc)
- [\_depth](OctreeBlock.md#_depth)
- [\_maxDepth](OctreeBlock.md#_maxdepth)
- [\_maxPoint](OctreeBlock.md#_maxpoint)
- [\_minPoint](OctreeBlock.md#_minpoint)
- [blocks](OctreeBlock.md#blocks)
- [entries](OctreeBlock.md#entries)

### Accessors

- [capacity](OctreeBlock.md#capacity)
- [maxPoint](OctreeBlock.md#maxpoint)
- [minPoint](OctreeBlock.md#minpoint)

### Methods

- [addEntries](OctreeBlock.md#addentries)
- [addEntry](OctreeBlock.md#addentry)
- [createInnerBlocks](OctreeBlock.md#createinnerblocks)
- [intersects](OctreeBlock.md#intersects)
- [intersectsRay](OctreeBlock.md#intersectsray)
- [removeEntry](OctreeBlock.md#removeentry)
- [select](OctreeBlock.md#select)

## Constructors

### constructor

• **new OctreeBlock**`T`(`minPoint`, `maxPoint`, `capacity`, `depth`, `maxDepth`, `creationFunc`)

Creates a new block

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `minPoint` | [`Vector3`](Vector3.md) | defines the minimum vector (in world space) of the block's bounding box |
| `maxPoint` | [`Vector3`](Vector3.md) | defines the maximum vector (in world space) of the block's bounding box |
| `capacity` | `number` | defines the maximum capacity of this block (if capacity is reached the block will be split into sub blocks) |
| `depth` | `number` | defines the current depth of this block in the octree |
| `maxDepth` | `number` | defines the maximal depth allowed (beyond this value, the capacity is ignored) |
| `creationFunc` | (`entry`: `T`, `block`: [`OctreeBlock`](OctreeBlock.md)`T`) => `void` | defines a callback to call when an element is added to the block |

#### Defined in

https://github.com/babylon.js/core/src/Culling/Octrees/octreeBlock.ts:49

## Properties

### \_boundingVectors

• `Private` **\_boundingVectors**: [`Vector3`](Vector3.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Culling/Octrees/octreeBlock.ts:37

___

### \_capacity

• `Private` **\_capacity**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Culling/Octrees/octreeBlock.ts:34

___

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

https://github.com/babylon.js/core/src/Culling/Octrees/octreeBlock.ts:38

___

### \_depth

• `Private` **\_depth**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Culling/Octrees/octreeBlock.ts:32

___

### \_maxDepth

• `Private` **\_maxDepth**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Culling/Octrees/octreeBlock.ts:33

___

### \_maxPoint

• `Private` **\_maxPoint**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Culling/Octrees/octreeBlock.ts:36

___

### \_minPoint

• `Private` **\_minPoint**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Culling/Octrees/octreeBlock.ts:35

___

### blocks

• **blocks**: [`OctreeBlock`](OctreeBlock.md)`T`[]

Gets the list of block children

#### Defined in

https://github.com/babylon.js/core/src/Culling/Octrees/octreeBlock.ts:30

___

### entries

• **entries**: `T`[]

Gets the content of the current block

#### Defined in

https://github.com/babylon.js/core/src/Culling/Octrees/octreeBlock.ts:25

## Accessors

### capacity

• `get` **capacity**(): `number`

Gets the maximum capacity of this block (if capacity is reached the block will be split into sub blocks)

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Culling/Octrees/octreeBlock.ts:85

___

### maxPoint

• `get` **maxPoint**(): [`Vector3`](Vector3.md)

Gets the maximum vector (in world space) of the block's bounding box

#### Returns

[`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Culling/Octrees/octreeBlock.ts:99

___

### minPoint

• `get` **minPoint**(): [`Vector3`](Vector3.md)

Gets the minimum vector (in world space) of the block's bounding box

#### Returns

[`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Culling/Octrees/octreeBlock.ts:92

## Methods

### addEntries

▸ **addEntries**(`entries`): `void`

Add an array of elements to this block

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `entries` | `T`[] | defines the array of elements to add |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Culling/Octrees/octreeBlock.ts:149

___

### addEntry

▸ **addEntry**(`entry`): `void`

Add a new element to this block

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `entry` | `T` | defines the element to add |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Culling/Octrees/octreeBlock.ts:109

___

### createInnerBlocks

▸ **createInnerBlocks**(): `void`

Subdivide the content into child blocks (this block will then be empty)

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Culling/Octrees/octreeBlock.ts:226

___

### intersects

▸ **intersects**(`sphereCenter`, `sphereRadius`, `selection`, `allowDuplicate?`): `void`

Test if the current block intersect with the given bounding sphere and if yes, then add its content to the selection array

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sphereCenter` | [`Vector3`](Vector3.md) | defines the bounding sphere center |
| `sphereRadius` | `number` | defines the bounding sphere radius |
| `selection` | [`SmartArrayNoDuplicate`](SmartArrayNoDuplicate.md)`T` | defines the array to store current content if selection is positive |
| `allowDuplicate?` | `boolean` | defines if the selection array can contains duplicated entries |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Culling/Octrees/octreeBlock.ts:187

___

### intersectsRay

▸ **intersectsRay**(`ray`, `selection`): `void`

Test if the current block intersect with the given ray and if yes, then add its content to the selection array

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ray` | [`Ray`](Ray.md) | defines the ray to test with |
| `selection` | [`SmartArrayNoDuplicate`](SmartArrayNoDuplicate.md)`T` | defines the array to store current content if selection is positive |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Culling/Octrees/octreeBlock.ts:210

___

### removeEntry

▸ **removeEntry**(`entry`): `void`

Remove an element from this block

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `entry` | `T` | defines the element to remove |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Culling/Octrees/octreeBlock.ts:129

___

### select

▸ **select**(`frustumPlanes`, `selection`, `allowDuplicate?`): `void`

Test if the current block intersects the frustum planes and if yes, then add its content to the selection array

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `frustumPlanes` | [`Plane`](Plane.md)[] | defines the frustum planes to test |
| `selection` | [`SmartArrayNoDuplicate`](SmartArrayNoDuplicate.md)`T` | defines the array to store current content if selection is positive |
| `allowDuplicate?` | `boolean` | defines if the selection array can contains duplicated entries |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Culling/Octrees/octreeBlock.ts:162
