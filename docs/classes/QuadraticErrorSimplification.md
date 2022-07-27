[@dev/core](../README.md) / [Exports](../modules.md) / QuadraticErrorSimplification

# Class: QuadraticErrorSimplification

An implementation of the Quadratic Error simplification algorithm.
Original paper : http://www1.cs.columbia.edu/~cs4162/html05s/garland97.pdf
Ported mostly from QSlim and http://voxels.blogspot.de/2014/05/quadric-mesh-simplification-with-source.html to babylon JS

**`Author`**

RaananW

**`See`**

https://doc.babylonjs.com/how_to/in-browser_mesh_simplification

## Implements

- [`ISimplifier`](../interfaces/ISimplifier.md)

## Table of contents

### Constructors

- [constructor](QuadraticErrorSimplification.md#constructor)

### Properties

- [\_reconstructedMesh](QuadraticErrorSimplification.md#_reconstructedmesh)
- [\_references](QuadraticErrorSimplification.md#_references)
- [\_triangles](QuadraticErrorSimplification.md#_triangles)
- [\_vertices](QuadraticErrorSimplification.md#_vertices)
- [aggressiveness](QuadraticErrorSimplification.md#aggressiveness)
- [boundingBoxEpsilon](QuadraticErrorSimplification.md#boundingboxepsilon)
- [decimationIterations](QuadraticErrorSimplification.md#decimationiterations)
- [syncIterations](QuadraticErrorSimplification.md#synciterations)

### Methods

- [\_calculateError](QuadraticErrorSimplification.md#_calculateerror)
- [\_identifyBorder](QuadraticErrorSimplification.md#_identifyborder)
- [\_init](QuadraticErrorSimplification.md#_init)
- [\_initDecimatedMesh](QuadraticErrorSimplification.md#_initdecimatedmesh)
- [\_initWithMesh](QuadraticErrorSimplification.md#_initwithmesh)
- [\_isFlipped](QuadraticErrorSimplification.md#_isflipped)
- [\_reconstructMesh](QuadraticErrorSimplification.md#_reconstructmesh)
- [\_runDecimation](QuadraticErrorSimplification.md#_rundecimation)
- [\_updateMesh](QuadraticErrorSimplification.md#_updatemesh)
- [\_updateTriangles](QuadraticErrorSimplification.md#_updatetriangles)
- [\_vertexError](QuadraticErrorSimplification.md#_vertexerror)
- [simplify](QuadraticErrorSimplification.md#simplify)

## Constructors

### constructor

• **new QuadraticErrorSimplification**(`_mesh`)

Creates a new QuadraticErrorSimplification

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `_mesh` | [`Mesh`](Mesh.md) | defines the target mesh |

#### Defined in

https://github.com/babylon.js/core/src/Meshes/meshSimplification.ts:335

## Properties

### \_reconstructedMesh

• `Private` **\_reconstructedMesh**: [`Mesh`](Mesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/meshSimplification.ts:317

___

### \_references

• `Private` **\_references**: `Reference`[]

#### Defined in

https://github.com/babylon.js/core/src/Meshes/meshSimplification.ts:315

___

### \_triangles

• `Private` **\_triangles**: `DecimationTriangle`[]

#### Defined in

https://github.com/babylon.js/core/src/Meshes/meshSimplification.ts:313

___

### \_vertices

• `Private` **\_vertices**: `DecimationVertex`[]

#### Defined in

https://github.com/babylon.js/core/src/Meshes/meshSimplification.ts:314

___

### aggressiveness

• **aggressiveness**: `number`

Gets or sets the aggressiveness of the simplifier

#### Defined in

https://github.com/babylon.js/core/src/Meshes/meshSimplification.ts:323

___

### boundingBoxEpsilon

• **boundingBoxEpsilon**: `number`

Gets or sets the espilon to use for bounding box computation

#### Defined in

https://github.com/babylon.js/core/src/Meshes/meshSimplification.ts:329

___

### decimationIterations

• **decimationIterations**: `number`

Gets or sets the number of allowed iterations for decimation

#### Defined in

https://github.com/babylon.js/core/src/Meshes/meshSimplification.ts:326

___

### syncIterations

• **syncIterations**: `number` = `5000`

Gets or sets the number pf sync iterations

#### Defined in

https://github.com/babylon.js/core/src/Meshes/meshSimplification.ts:320

## Methods

### \_calculateError

▸ `Private` **_calculateError**(`vertex1`, `vertex2`, `pointResult?`): `number`

#### Parameters

| Name | Type |
| :------ | :------ |
| `vertex1` | `DecimationVertex` |
| `vertex2` | `DecimationVertex` |
| `pointResult?` | [`Vector3`](Vector3.md) |

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/meshSimplification.ts:868

___

### \_identifyBorder

▸ `Private` **_identifyBorder**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/meshSimplification.ts:763

___

### \_init

▸ `Private` **_init**(`callback`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | `Function` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/meshSimplification.ts:558

___

### \_initDecimatedMesh

▸ `Private` **_initDecimatedMesh**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/meshSimplification.ts:696

___

### \_initWithMesh

▸ `Private` **_initWithMesh**(`submeshIndex`, `callback`, `optimizeMesh?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `submeshIndex` | `number` |
| `callback` | `Function` |
| `optimizeMesh?` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/meshSimplification.ts:495

___

### \_isFlipped

▸ `Private` **_isFlipped**(`vertex1`, `vertex2`, `point`, `deletedArray`, `delTr`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `vertex1` | `DecimationVertex` |
| `vertex2` | `DecimationVertex` |
| `point` | [`Vector3`](Vector3.md) |
| `deletedArray` | `boolean`[] |
| `delTr` | `DecimationTriangle`[] |

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/meshSimplification.ts:704

___

### \_reconstructMesh

▸ `Private` **_reconstructMesh**(`submeshIndex`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `submeshIndex` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/meshSimplification.ts:580

___

### \_runDecimation

▸ `Private` **_runDecimation**(`settings`, `submeshIndex`, `successCallback`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `settings` | [`ISimplificationSettings`](../interfaces/ISimplificationSettings.md) |
| `submeshIndex` | `number` |
| `successCallback` | () => `void` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/meshSimplification.ts:371

___

### \_updateMesh

▸ `Private` **_updateMesh**(`identifyBorders?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `identifyBorders` | `boolean` | `false` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/meshSimplification.ts:799

___

### \_updateTriangles

▸ `Private` **_updateTriangles**(`origVertex`, `vertex`, `deletedArray`, `deletedTriangles`): `number`

#### Parameters

| Name | Type |
| :------ | :------ |
| `origVertex` | `DecimationVertex` |
| `vertex` | `DecimationVertex` |
| `deletedArray` | `boolean`[] |
| `deletedTriangles` | `number` |

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/meshSimplification.ts:739

___

### \_vertexError

▸ `Private` **_vertexError**(`q`, `point`): `number`

#### Parameters

| Name | Type |
| :------ | :------ |
| `q` | `QuadraticMatrix` |
| `point` | [`Vector3`](Vector3.md) |

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/meshSimplification.ts:850

___

### simplify

▸ **simplify**(`settings`, `successCallback`): `void`

Simplification of a given mesh according to the given settings.
Since this requires computation, it is assumed that the function runs async.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `settings` | [`ISimplificationSettings`](../interfaces/ISimplificationSettings.md) | The settings of the simplification, including quality and distance |
| `successCallback` | (`simplifiedMesh`: [`Mesh`](Mesh.md)) => `void` | A callback that will be called after the mesh was simplified. |

#### Returns

`void`

#### Implementation of

[ISimplifier](../interfaces/ISimplifier.md).[simplify](../interfaces/ISimplifier.md#simplify)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/meshSimplification.ts:347
