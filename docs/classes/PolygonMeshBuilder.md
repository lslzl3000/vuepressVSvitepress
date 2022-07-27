[@dev/core](../README.md) / [Exports](../modules.md) / PolygonMeshBuilder

# Class: PolygonMeshBuilder

Builds a polygon

**`See`**

https://doc.babylonjs.com/how_to/polygonmeshbuilder

## Table of contents

### Constructors

- [constructor](PolygonMeshBuilder.md#constructor)

### Properties

- [\_eholes](PolygonMeshBuilder.md#_eholes)
- [\_epoints](PolygonMeshBuilder.md#_epoints)
- [\_holes](PolygonMeshBuilder.md#_holes)
- [\_name](PolygonMeshBuilder.md#_name)
- [\_outlinepoints](PolygonMeshBuilder.md#_outlinepoints)
- [\_points](PolygonMeshBuilder.md#_points)
- [\_scene](PolygonMeshBuilder.md#_scene)
- [bjsEarcut](PolygonMeshBuilder.md#bjsearcut)

### Methods

- [\_addSide](PolygonMeshBuilder.md#_addside)
- [\_addToepoint](PolygonMeshBuilder.md#_addtoepoint)
- [addHole](PolygonMeshBuilder.md#addhole)
- [build](PolygonMeshBuilder.md#build)
- [buildVertexData](PolygonMeshBuilder.md#buildvertexdata)

## Constructors

### constructor

• **new PolygonMeshBuilder**(`name`, `contours`, `scene?`, `earcutInjection?`)

Creates a PolygonMeshBuilder

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | name of the builder |
| `contours` | `any` | `undefined` | Path of the polygon |
| `scene?` | [`Scene`](Scene.md) | `undefined` | scene to add to when creating the mesh |
| `earcutInjection` | `any` | `earcut` | can be used to inject your own earcut reference |

#### Defined in

https://github.com/babylon.js/core/src/Meshes/polygonMesh.ts:173

## Properties

### \_eholes

• `Private` **\_eholes**: `number`[]

#### Defined in

https://github.com/babylon.js/core/src/Meshes/polygonMesh.ts:153

___

### \_epoints

• `Private` **\_epoints**: `number`[]

#### Defined in

https://github.com/babylon.js/core/src/Meshes/polygonMesh.ts:152

___

### \_holes

• `Private` **\_holes**: `PolygonPoints`[]

#### Defined in

https://github.com/babylon.js/core/src/Meshes/polygonMesh.ts:147

___

### \_name

• `Private` **\_name**: `string`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/polygonMesh.ts:149

___

### \_outlinepoints

• `Private` **\_outlinepoints**: `PolygonPoints`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/polygonMesh.ts:146

___

### \_points

• `Private` **\_points**: `PolygonPoints`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/polygonMesh.ts:145

___

### \_scene

• `Private` **\_scene**: [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/polygonMesh.ts:150

___

### bjsEarcut

• **bjsEarcut**: `any`

Babylon reference to the earcut plugin.

#### Defined in

https://github.com/babylon.js/core/src/Meshes/polygonMesh.ts:164

## Methods

### \_addSide

▸ `Private` **_addSide**(`positions`, `normals`, `uvs`, `indices`, `bounds`, `points`, `depth`, `flip`, `smoothingThreshold`): `void`

Adds a side to the polygon

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `positions` | `any`[] | points that make the polygon |
| `normals` | `any`[] | normals of the polygon |
| `uvs` | `any`[] | uvs of the polygon |
| `indices` | `any`[] | indices of the polygon |
| `bounds` | `any` | bounds of the polygon |
| `points` | `PolygonPoints` | points of the polygon |
| `depth` | `number` | depth of the polygon |
| `flip` | `boolean` | flip of the polygon |
| `smoothingThreshold` | `number` |  |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/polygonMesh.ts:309

___

### \_addToepoint

▸ `Private` **_addToepoint**(`points`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `points` | [`Vector2`](Vector2.md)[] |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/polygonMesh.ts:155

___

### addHole

▸ **addHole**(`hole`): [`PolygonMeshBuilder`](PolygonMeshBuilder.md)

Adds a hole within the polygon

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `hole` | [`Vector2`](Vector2.md)[] | Array of points defining the hole |

#### Returns

[`PolygonMeshBuilder`](PolygonMeshBuilder.md)

this

#### Defined in

https://github.com/babylon.js/core/src/Meshes/polygonMesh.ts:200

___

### build

▸ **build**(`updatable?`, `depth?`, `smoothingThreshold?`): [`Mesh`](Mesh.md)

Creates the polygon

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `updatable` | `boolean` | `false` | If the mesh should be updatable |
| `depth` | `number` | `0` | The depth of the mesh created |
| `smoothingThreshold` | `number` | `2` | Dot product threshold for smoothed normals |

#### Returns

[`Mesh`](Mesh.md)

the created mesh

#### Defined in

https://github.com/babylon.js/core/src/Meshes/polygonMesh.ts:219

___

### buildVertexData

▸ **buildVertexData**(`depth?`, `smoothingThreshold?`): [`VertexData`](VertexData.md)

Creates the polygon

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `depth` | `number` | `0` | The depth of the mesh created |
| `smoothingThreshold` | `number` | `2` | Dot product threshold for smoothed normals |

#### Returns

[`VertexData`](VertexData.md)

the created VertexData

#### Defined in

https://github.com/babylon.js/core/src/Meshes/polygonMesh.ts:238
