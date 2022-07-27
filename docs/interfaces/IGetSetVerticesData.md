[@dev/core](../README.md) / [Exports](../modules.md) / IGetSetVerticesData

# Interface: IGetSetVerticesData

Define an interface for all classes that will get and set the data on vertices

## Implemented by

- [`AbstractMesh`](../classes/AbstractMesh.md)
- [`Geometry`](../classes/Geometry.md)
- [`Mesh`](../classes/Mesh.md)

## Table of contents

### Methods

- [getIndices](IGetSetVerticesData.md#getindices)
- [getVerticesData](IGetSetVerticesData.md#getverticesdata)
- [isVerticesDataPresent](IGetSetVerticesData.md#isverticesdatapresent)
- [setIndices](IGetSetVerticesData.md#setindices)
- [setVerticesData](IGetSetVerticesData.md#setverticesdata)
- [updateVerticesData](IGetSetVerticesData.md#updateverticesdata)

## Methods

### getIndices

▸ **getIndices**(`copyWhenShared?`, `forceCopy?`): [`Nullable`](../modules.md#nullable)[`IndicesArray`](../modules.md#indicesarray)

Returns an array of integers or a typed array (Int32Array, Uint32Array, Uint16Array) populated with the mesh indices.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `copyWhenShared?` | `boolean` | If true (default false) and and if the mesh geometry is shared among some other meshes, the returned array is a copy of the internal one. |
| `forceCopy?` | `boolean` | defines a boolean indicating that the returned array must be cloned upon returning it |

#### Returns

[`Nullable`](../modules.md#nullable)[`IndicesArray`](../modules.md#indicesarray)

the indices array or an empty array if the mesh has no geometry

#### Defined in

https://github.com/babylon.js/core/src/Meshes/mesh.vertexData.ts:45

___

### getVerticesData

▸ **getVerticesData**(`kind`, `copyWhenShared?`, `forceCopy?`): [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray)

Gets a specific vertex data attached to this geometry. Float data is constructed if the vertex buffer data cannot be returned directly.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `kind` | `string` | defines the data kind (Position, normal, etc...) |
| `copyWhenShared?` | `boolean` | defines if the returned array must be cloned upon returning it if the current geometry is shared between multiple meshes |
| `forceCopy?` | `boolean` | defines a boolean indicating that the returned array must be cloned upon returning it |

#### Returns

[`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray)

a float array containing vertex data

#### Defined in

https://github.com/babylon.js/core/src/Meshes/mesh.vertexData.ts:38

___

### isVerticesDataPresent

▸ **isVerticesDataPresent**(`kind`): `boolean`

Gets a boolean indicating if specific vertex data is present

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `kind` | `string` | defines the vertex data kind to use |

#### Returns

`boolean`

true is data kind is present

#### Defined in

https://github.com/babylon.js/core/src/Meshes/mesh.vertexData.ts:30

___

### setIndices

▸ **setIndices**(`indices`, `totalVertices`, `updatable?`): `void`

Creates a new index buffer

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `indices` | [`IndicesArray`](../modules.md#indicesarray) | defines the indices to store in the index buffer |
| `totalVertices` | [`Nullable`](../modules.md#nullable)`number` | defines the total number of vertices (could be null) |
| `updatable?` | `boolean` | defines if the index buffer must be flagged as updatable (false by default) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/mesh.vertexData.ts:80

___

### setVerticesData

▸ **setVerticesData**(`kind`, `data`, `updatable`): `void`

Set specific vertex data

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `kind` | `string` | defines the data kind (Position, normal, etc...) |
| `data` | [`FloatArray`](../modules.md#floatarray) | defines the vertex data to use |
| `updatable` | `boolean` | defines if the vertex must be flagged as updatable (false as default) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/mesh.vertexData.ts:53

___

### updateVerticesData

▸ **updateVerticesData**(`kind`, `data`, `updateExtends?`, `makeItUnique?`): `void`

Update a specific associated vertex buffer

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `kind` | `string` | defines which buffer to write to (positions, indices, normals, etc). Possible `kind` values :  - VertexBuffer.PositionKind  - VertexBuffer.UVKind  - VertexBuffer.UV2Kind  - VertexBuffer.UV3Kind  - VertexBuffer.UV4Kind  - VertexBuffer.UV5Kind  - VertexBuffer.UV6Kind  - VertexBuffer.ColorKind  - VertexBuffer.MatricesIndicesKind  - VertexBuffer.MatricesIndicesExtraKind  - VertexBuffer.MatricesWeightsKind  - VertexBuffer.MatricesWeightsExtraKind |
| `data` | [`FloatArray`](../modules.md#floatarray) | defines the data source |
| `updateExtends?` | `boolean` | defines if extends info of the mesh must be updated (can be null). This is mostly useful for "position" kind |
| `makeItUnique?` | `boolean` | defines if the geometry associated with the mesh must be cloned to make the change only for this mesh (and not all meshes associated with the same geometry) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/mesh.vertexData.ts:73
