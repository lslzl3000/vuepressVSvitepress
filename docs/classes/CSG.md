[@dev/core](../README.md) / [Exports](../modules.md) / CSG

# Class: CSG

Class for building Constructive Solid Geometry

## Table of contents

### Constructors

- [constructor](CSG.md#constructor)

### Properties

- [\_polygons](CSG.md#_polygons)
- [matrix](CSG.md#matrix)
- [position](CSG.md#position)
- [rotation](CSG.md#rotation)
- [rotationQuaternion](CSG.md#rotationquaternion)
- [scaling](CSG.md#scaling)

### Methods

- [buildMeshGeometry](CSG.md#buildmeshgeometry)
- [clone](CSG.md#clone)
- [copyTransformAttributes](CSG.md#copytransformattributes)
- [intersect](CSG.md#intersect)
- [intersectInPlace](CSG.md#intersectinplace)
- [inverse](CSG.md#inverse)
- [inverseInPlace](CSG.md#inverseinplace)
- [subtract](CSG.md#subtract)
- [subtractInPlace](CSG.md#subtractinplace)
- [toMesh](CSG.md#tomesh)
- [union](CSG.md#union)
- [unionInPlace](CSG.md#unioninplace)
- [FromMesh](CSG.md#frommesh)
- [\_FromPolygons](CSG.md#_frompolygons)

## Constructors

### constructor

• **new CSG**()

## Properties

### \_polygons

• `Private` **\_polygons**: `Polygon`[]

#### Defined in

https://github.com/babylon.js/core/src/Meshes/csg.ts:426

___

### matrix

• **matrix**: [`Matrix`](Matrix.md)

The world matrix

#### Defined in

https://github.com/babylon.js/core/src/Meshes/csg.ts:430

___

### position

• **position**: [`Vector3`](Vector3.md)

Stores the position

#### Defined in

https://github.com/babylon.js/core/src/Meshes/csg.ts:434

___

### rotation

• **rotation**: [`Vector3`](Vector3.md)

Stores the rotation

#### Defined in

https://github.com/babylon.js/core/src/Meshes/csg.ts:438

___

### rotationQuaternion

• **rotationQuaternion**: [`Nullable`](../modules.md#nullable)[`Quaternion`](Quaternion.md)

Stores the rotation quaternion

#### Defined in

https://github.com/babylon.js/core/src/Meshes/csg.ts:442

___

### scaling

• **scaling**: [`Vector3`](Vector3.md)

Stores the scaling vector

#### Defined in

https://github.com/babylon.js/core/src/Meshes/csg.ts:446

## Methods

### buildMeshGeometry

▸ **buildMeshGeometry**(`name`, `scene?`, `keepSubMeshes?`): [`Mesh`](Mesh.md)

Build Raw mesh from CSG
Coordinates here are in world space

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | The name of the mesh geometry |
| `scene?` | [`Scene`](Scene.md) | The Scene |
| `keepSubMeshes?` | `boolean` | Specifies if the submeshes should be kept |

#### Returns

[`Mesh`](Mesh.md)

A new Mesh

#### Defined in

https://github.com/babylon.js/core/src/Meshes/csg.ts:717

___

### clone

▸ **clone**(): [`CSG`](CSG.md)

Clones, or makes a deep copy, of the CSG

#### Returns

[`CSG`](CSG.md)

A new CSG

#### Defined in

https://github.com/babylon.js/core/src/Meshes/csg.ts:554

___

### copyTransformAttributes

▸ **copyTransformAttributes**(`csg`): [`CSG`](CSG.md)

This is used to keep meshes transformations so they can be restored
when we build back a Babylon Mesh
NB : All CSG operations are performed in world coordinates

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `csg` | [`CSG`](CSG.md) | The CSG to copy the transform attributes from |

#### Returns

[`CSG`](CSG.md)

This CSG

#### Defined in

https://github.com/babylon.js/core/src/Meshes/csg.ts:699

___

### intersect

▸ **intersect**(`csg`): [`CSG`](CSG.md)

Intersect this CSG with another CSG

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `csg` | [`CSG`](CSG.md) | The CSG to intersect against this CSG |

#### Returns

[`CSG`](CSG.md)

A new CSG

#### Defined in

https://github.com/babylon.js/core/src/Meshes/csg.ts:640

___

### intersectInPlace

▸ **intersectInPlace**(`csg`): `void`

Intersects this CSG with another CSG in place

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `csg` | [`CSG`](CSG.md) | The CSG to intersect against this CSG |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/csg.ts:657

___

### inverse

▸ **inverse**(): [`CSG`](CSG.md)

Return a new CSG solid with solid and empty space switched. This solid is
not modified.

#### Returns

[`CSG`](CSG.md)

A new CSG solid with solid and empty space switched

#### Defined in

https://github.com/babylon.js/core/src/Meshes/csg.ts:677

___

### inverseInPlace

▸ **inverseInPlace**(): `void`

Inverses the CSG in place

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/csg.ts:686

___

### subtract

▸ **subtract**(`csg`): [`CSG`](CSG.md)

Subtracts this CSG with another CSG

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `csg` | [`CSG`](CSG.md) | The CSG to subtract against this CSG |

#### Returns

[`CSG`](CSG.md)

A new CSG

#### Defined in

https://github.com/babylon.js/core/src/Meshes/csg.ts:601

___

### subtractInPlace

▸ **subtractInPlace**(`csg`): `void`

Subtracts this CSG with another CSG in place

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `csg` | [`CSG`](CSG.md) | The CSG to subtract against this CSG |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/csg.ts:619

___

### toMesh

▸ **toMesh**(`name`, `material?`, `scene?`, `keepSubMeshes?`): [`Mesh`](Mesh.md)

Build Mesh from CSG taking material and transforms into account

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | The name of the Mesh |
| `material` | [`Nullable`](../modules.md#nullable)[`Material`](Material.md) | `null` | The material of the Mesh |
| `scene?` | [`Scene`](Scene.md) | `undefined` | The Scene |
| `keepSubMeshes?` | `boolean` | `undefined` | Specifies if submeshes should be kept |

#### Returns

[`Mesh`](Mesh.md)

The new Mesh

#### Defined in

https://github.com/babylon.js/core/src/Meshes/csg.ts:888

___

### union

▸ **union**(`csg`): [`CSG`](CSG.md)

Unions this CSG with another CSG

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `csg` | [`CSG`](CSG.md) | The CSG to union against this CSG |

#### Returns

[`CSG`](CSG.md)

The unioned CSG

#### Defined in

https://github.com/babylon.js/core/src/Meshes/csg.ts:566

___

### unionInPlace

▸ **unionInPlace**(`csg`): `void`

Unions this CSG with another CSG in place

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `csg` | [`CSG`](CSG.md) | The CSG to union against this CSG |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/csg.ts:582

___

### FromMesh

▸ `Static` **FromMesh**(`mesh`, `absolute?`): [`CSG`](CSG.md)

Convert the Mesh to CSG

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `mesh` | [`Mesh`](Mesh.md) | `undefined` | The Mesh to convert to CSG |
| `absolute` | `boolean` | `false` | If true, the final (local) matrix transformation is set to the identity and not to that of `mesh`. It can help when dealing with right-handed meshes (default: false) |

#### Returns

[`CSG`](CSG.md)

A new CSG from the Mesh

#### Defined in

https://github.com/babylon.js/core/src/Meshes/csg.ts:454

___

### \_FromPolygons

▸ `Static` `Private` **_FromPolygons**(`polygons`): [`CSG`](CSG.md)

Construct a CSG solid from a list of `CSG.Polygon` instances.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `polygons` | `Polygon`[] | Polygons used to construct a CSG solid |

#### Returns

[`CSG`](CSG.md)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/csg.ts:544
