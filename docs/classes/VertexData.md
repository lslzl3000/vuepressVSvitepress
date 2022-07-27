[@dev/core](../README.md) / [Exports](../modules.md) / VertexData

# Class: VertexData

This class contains the various kinds of data on every vertex of a mesh used in determining its shape and appearance

## Table of contents

### Constructors

- [constructor](VertexData.md#constructor)

### Properties

- [\_applyTo](VertexData.md#_applyto)
- [colors](VertexData.md#colors)
- [indices](VertexData.md#indices)
- [matricesIndices](VertexData.md#matricesindices)
- [matricesIndicesExtra](VertexData.md#matricesindicesextra)
- [matricesWeights](VertexData.md#matricesweights)
- [matricesWeightsExtra](VertexData.md#matricesweightsextra)
- [normals](VertexData.md#normals)
- [positions](VertexData.md#positions)
- [tangents](VertexData.md#tangents)
- [uvs](VertexData.md#uvs)
- [uvs2](VertexData.md#uvs2)
- [uvs3](VertexData.md#uvs3)
- [uvs4](VertexData.md#uvs4)
- [uvs5](VertexData.md#uvs5)
- [uvs6](VertexData.md#uvs6)
- [BACKSIDE](VertexData.md#backside)
- [DEFAULTSIDE](VertexData.md#defaultside)
- [DOUBLESIDE](VertexData.md#doubleside)
- [FRONTSIDE](VertexData.md#frontside)

### Methods

- [\_update](VertexData.md#_update)
- [\_validate](VertexData.md#_validate)
- [applyToGeometry](VertexData.md#applytogeometry)
- [applyToMesh](VertexData.md#applytomesh)
- [merge](VertexData.md#merge)
- [serialize](VertexData.md#serialize)
- [set](VertexData.md#set)
- [transform](VertexData.md#transform)
- [updateGeometry](VertexData.md#updategeometry)
- [updateMesh](VertexData.md#updatemesh)
- [ComputeNormals](VertexData.md#computenormals)
- [CreateBox](VertexData.md#createbox)
- [CreateCapsule](VertexData.md#createcapsule)
- [CreateCylinder](VertexData.md#createcylinder)
- [CreateDashedLines](VertexData.md#createdashedlines)
- [CreateDisc](VertexData.md#createdisc)
- [CreateGround](VertexData.md#createground)
- [CreateGroundFromHeightMap](VertexData.md#creategroundfromheightmap)
- [CreateIcoSphere](VertexData.md#createicosphere)
- [CreateLineSystem](VertexData.md#createlinesystem)
- [CreatePlane](VertexData.md#createplane)
- [CreatePolygon](VertexData.md#createpolygon)
- [CreatePolyhedron](VertexData.md#createpolyhedron)
- [CreateRibbon](VertexData.md#createribbon)
- [CreateSphere](VertexData.md#createsphere)
- [CreateTiledBox](VertexData.md#createtiledbox)
- [CreateTiledGround](VertexData.md#createtiledground)
- [CreateTiledPlane](VertexData.md#createtiledplane)
- [CreateTorus](VertexData.md#createtorus)
- [CreateTorusKnot](VertexData.md#createtorusknot)
- [ExtractFromGeometry](VertexData.md#extractfromgeometry)
- [ExtractFromMesh](VertexData.md#extractfrommesh)
- [ImportVertexData](VertexData.md#importvertexdata)
- [\_ExtractFrom](VertexData.md#_extractfrom)
- [\_FlipFaces](VertexData.md#_flipfaces)
- [\_MergeElement](VertexData.md#_mergeelement)
- [\_TransformVector3Coordinates](VertexData.md#_transformvector3coordinates)
- [\_TransformVector3Normals](VertexData.md#_transformvector3normals)
- [\_TransformVector4Normals](VertexData.md#_transformvector4normals)

## Constructors

### constructor

• **new VertexData**()

## Properties

### \_applyTo

• `Private` `Readonly` **\_applyTo**: 

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:279

___

### colors

• **colors**: [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray)

An array of the r, g, b, a, color of each vertex  [...., r, g, b, a, .....]

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:152

___

### indices

• **indices**: [`Nullable`](../modules.md#nullable)[`IndicesArray`](../modules.md#indicesarray)

An array of i, j, k the three vertex indices required for each triangular facet  [...., i, j, k .....]

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:177

___

### matricesIndices

• **matricesIndices**: [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray)

An array containing the list of indices to the array of matrices produced by bones, each vertex have up to 4 indices (8 if the matricesIndicesExtra is set).

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:157

___

### matricesIndicesExtra

• **matricesIndicesExtra**: [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray)

An array extending the number of possible indices

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:167

___

### matricesWeights

• **matricesWeights**: [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray)

An array containing the list of weights defining the weight of each indexed matrix in the final computation

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:162

___

### matricesWeightsExtra

• **matricesWeightsExtra**: [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray)

An array extending the number of possible weights when the number of indices is extended

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:172

___

### normals

• **normals**: [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray)

An array of the x, y, z normal vector of each vertex  [...., x, y, z, .....]

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:112

___

### positions

• **positions**: [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray)

An array of the x, y, z position of each vertex  [...., x, y, z, .....]

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:107

___

### tangents

• **tangents**: [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray)

An array of the x, y, z tangent vector of each vertex  [...., x, y, z, .....]

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:117

___

### uvs

• **uvs**: [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray)

An array of u,v which maps a texture image onto each vertex  [...., u, v, .....]

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:122

___

### uvs2

• **uvs2**: [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray)

A second array of u,v which maps a texture image onto each vertex  [...., u, v, .....]

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:127

___

### uvs3

• **uvs3**: [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray)

A third array of u,v which maps a texture image onto each vertex  [...., u, v, .....]

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:132

___

### uvs4

• **uvs4**: [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray)

A fourth array of u,v which maps a texture image onto each vertex  [...., u, v, .....]

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:137

___

### uvs5

• **uvs5**: [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray)

A fifth array of u,v which maps a texture image onto each vertex  [...., u, v, .....]

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:142

___

### uvs6

• **uvs6**: [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray)

A sixth array of u,v which maps a texture image onto each vertex  [...., u, v, .....]

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:147

___

### BACKSIDE

▪ `Static` `Readonly` **BACKSIDE**: ``1``

Mesh side orientation : usually the internal or back surface

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:94

___

### DEFAULTSIDE

▪ `Static` `Readonly` **DEFAULTSIDE**: ``0``

Mesh side orientation : by default, `FRONTSIDE`

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:102

___

### DOUBLESIDE

▪ `Static` `Readonly` **DOUBLESIDE**: ``2``

Mesh side orientation : both internal and external or front and back surfaces

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:98

___

### FRONTSIDE

▪ `Static` `Readonly` **FRONTSIDE**: ``0``

Mesh side orientation : usually the external or front surface

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:90

## Methods

### \_update

▸ `Private` **_update**(`meshOrGeometry`, `updateExtends?`, `makeItUnique?`): [`VertexData`](VertexData.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `meshOrGeometry` | [`IGetSetVerticesData`](../interfaces/IGetSetVerticesData.md) |
| `updateExtends?` | `boolean` |
| `makeItUnique?` | `boolean` |

#### Returns

[`VertexData`](VertexData.md)

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:398

___

### \_validate

▸ `Private` **_validate**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:825

___

### applyToGeometry

▸ **applyToGeometry**(`geometry`, `updatable?`): [`VertexData`](VertexData.md)

Associates the vertexData to the passed Geometry.
Sets it as updatable or not (default `false`)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `geometry` | [`Geometry`](Geometry.md) | the geometry the vertexData is applied to |
| `updatable?` | `boolean` | when used and having the value true allows new data to update the vertexData |

#### Returns

[`VertexData`](VertexData.md)

VertexData

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:254

___

### applyToMesh

▸ **applyToMesh**(`mesh`, `updatable?`): [`VertexData`](VertexData.md)

Associates the vertexData to the passed Mesh.
Sets it as updatable or not (default `false`)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`Mesh`](Mesh.md) | the mesh the vertexData is applied to |
| `updatable?` | `boolean` | when used and having the value true allows new data to update the vertexData |

#### Returns

[`VertexData`](VertexData.md)

the VertexData

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:242

___

### merge

▸ **merge**(`others`, `use32BitsIndices?`, `forceCloneIndices?`): [`VertexData`](VertexData.md)

Merges the passed VertexData into the current one

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `others` | [`VertexData`](VertexData.md) \| [`VertexData`](VertexData.md)[] | `undefined` | the VertexData to be merged into the current one |
| `use32BitsIndices` | `boolean` | `false` | defines a boolean indicating if indices must be store in a 32 bits array |
| `forceCloneIndices` | `boolean` | `false` | defines a boolean indicating if indices are forced to be cloned |

#### Returns

[`VertexData`](VertexData.md)

the modified VertexData

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:543

___

### serialize

▸ **serialize**(): `any`

Serializes the VertexData

#### Returns

`any`

a serialized object

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:893

___

### set

▸ **set**(`data`, `kind`): `void`

Uses the passed data array to set the set the values for the specified kind of data

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | [`FloatArray`](../modules.md#floatarray) | a linear array of floating numbers |
| `kind` | `string` | the type of data that is being set, eg positions, colors etc |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:184

___

### transform

▸ **transform**(`matrix`): [`VertexData`](VertexData.md)

Transforms each position and each normal of the vertexData according to the passed Matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `matrix` | [`Matrix`](Matrix.md) | the transforming matrix |

#### Returns

[`VertexData`](VertexData.md)

the VertexData

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:515

___

### updateGeometry

▸ **updateGeometry**(`geometry`): [`VertexData`](VertexData.md)

Updates the associated geometry

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `geometry` | [`Geometry`](Geometry.md) | the geometry to be updated |

#### Returns

[`VertexData`](VertexData.md)

VertexData.

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:274

___

### updateMesh

▸ **updateMesh**(`mesh`): [`VertexData`](VertexData.md)

Updates the associated mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`Mesh`](Mesh.md) | the mesh to be updated |

#### Returns

[`VertexData`](VertexData.md)

VertexData

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:264

___

### ComputeNormals

▸ `Static` **ComputeNormals**(`positions`, `indices`, `normals`, `options?`): `void`

Compute normals for given positions and indices

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `positions` | `any` | an array of vertex positions, [...., x, y, z, ......] |
| `indices` | `any` | an array of indices in groups of three for each triangular facet, [...., i, j, k, ......] |
| `normals` | `any` | an array of vertex normals, [...., x, y, z, ......] |
| `options?` | `Object` | an object used to set the following optional parameters for the TorusKnot, optional  * facetNormals : optional array of facet normals (vector3)  * facetPositions : optional array of facet positions (vector3)  * facetPartitioning : optional partitioning array. facetPositions is required for facetPartitioning computation  * ratio : optional partitioning ratio / bounding box, required for facetPartitioning computation  * bInfo : optional bounding info, required for facetPartitioning computation  * bbSize : optional bounding box size data, required for facetPartitioning computation  * subDiv : optional partitioning data about subdivisions on  each axis (int), required for facetPartitioning computation  * useRightHandedSystem: optional boolean to for right handed system computation  * depthSort : optional boolean to enable the facet depth sort computation  * distanceTo : optional Vector3 to compute the facet depth from this location  * depthSortedFacets : optional array of depthSortedFacets to store the facet distances from the reference location |
| `options.bInfo?` | `any` |  |
| `options.bbSize?` | [`Vector3`](Vector3.md) |  |
| `options.depthSort?` | `boolean` |  |
| `options.depthSortedFacets?` | `any` |  |
| `options.distanceTo?` | [`Vector3`](Vector3.md) |  |
| `options.facetNormals?` | `any` |  |
| `options.facetPartitioning?` | `any` |  |
| `options.facetPositions?` | `any` |  |
| `options.ratio?` | `number` |  |
| `options.subDiv?` | `any` |  |
| `options.useRightHandedSystem?` | `boolean` |  |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:1692

___

### CreateBox

▸ `Static` **CreateBox**(`options`): [`VertexData`](VertexData.md)

Creates the VertexData for a box

**`Deprecated`**

Please use CreateBoxVertexData from the BoxBuilder file instead

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | `Object` | an object used to set the following optional parameters for the box, required but can be empty  * size sets the width, height and depth of the box to the value of size, optional default 1  * width sets the width (x direction) of the box, overwrites the width set by size, optional, default size  * height sets the height (y direction) of the box, overwrites the height set by size, optional, default size  * depth sets the depth (z direction) of the box, overwrites the depth set by size, optional, default size  * faceUV an array of 6 Vector4 elements used to set different images to each box side  * faceColors an array of 6 Color3 elements used to set different colors to each box side  * sideOrientation optional and takes the values : Mesh.FRONTSIDE (default), Mesh.BACKSIDE or Mesh.DOUBLESIDE  * frontUvs only usable when you create a double-sided mesh, used to choose what parts of the texture image to crop and apply on the front side, optional, default vector4 (0, 0, 1, 1)  * backUVs only usable when you create a double-sided mesh, used to choose what parts of the texture image to crop and apply on the back side, optional, default vector4 (0, 0, 1, 1) |
| `options.backUVs?` | [`Vector4`](Vector4.md) |  |
| `options.depth?` | `number` |  |
| `options.faceColors?` | [`Color4`](Color4.md)[] |  |
| `options.faceUV?` | [`Vector4`](Vector4.md)[] |  |
| `options.frontUVs?` | [`Vector4`](Vector4.md) |  |
| `options.height?` | `number` |  |
| `options.sideOrientation?` | `number` |  |
| `options.size?` | `number` |  |
| `options.width?` | `number` |  |

#### Returns

[`VertexData`](VertexData.md)

the VertexData of the box

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:1111

___

### CreateCapsule

▸ `Static` **CreateCapsule**(`options?`): [`VertexData`](VertexData.md)

Creates the VertexData for a Capsule, inspired from https://github.com/maximeq/three-js-capsule-geometry/blob/master/src/CapsuleBufferGeometry.js

**`Deprecated`**

Please use CreateCapsuleVertexData from the capsuleBuilder file instead

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | [`ICreateCapsuleOptions`](../interfaces/ICreateCapsuleOptions.md) | an object used to set the following optional parameters for the capsule, required but can be empty |

#### Returns

[`VertexData`](VertexData.md)

the VertexData of the Capsule

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:1609

___

### CreateCylinder

▸ `Static` **CreateCylinder**(`options`): [`VertexData`](VertexData.md)

Creates the VertexData for a cylinder, cone or prism

**`Deprecated`**

please use CreateCylinderVertexData instead

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | `Object` | an object used to set the following optional parameters for the box, required but can be empty  * height sets the height (y direction) of the cylinder, optional, default 2  * diameterTop sets the diameter of the top of the cone, overwrites diameter,  optional, default diameter  * diameterBottom sets the diameter of the bottom of the cone, overwrites diameter,  optional, default diameter  * diameter sets the diameter of the top and bottom of the cone, optional default 1  * tessellation the number of prism sides, 3 for a triangular prism, optional, default 24  * subdivisions` the number of rings along the cylinder height, optional, default 1  * arc a number from 0 to 1, to create an unclosed cylinder based on the fraction of the circumference given by the arc value, optional, default 1  * faceColors an array of Color3 elements used to set different colors to the top, rings and bottom respectively  * faceUV an array of Vector4 elements used to set different images to the top, rings and bottom respectively  * hasRings when true makes each subdivision independently treated as a face for faceUV and faceColors, optional, default false  * enclose when true closes an open cylinder by adding extra flat faces between the height axis and vertical edges, think cut cake  * sideOrientation optional and takes the values : Mesh.FRONTSIDE (default), Mesh.BACKSIDE or Mesh.DOUBLESIDE  * frontUvs only usable when you create a double-sided mesh, used to choose what parts of the texture image to crop and apply on the front side, optional, default vector4 (0, 0, 1, 1)  * backUVs only usable when you create a double-sided mesh, used to choose what parts of the texture image to crop and apply on the back side, optional, default vector4 (0, 0, 1, 1) |
| `options.arc?` | `number` |  |
| `options.backUVs?` | [`Vector4`](Vector4.md) |  |
| `options.diameter?` | `number` |  |
| `options.diameterBottom?` | `number` |  |
| `options.diameterTop?` | `number` |  |
| `options.enclose?` | `boolean` |  |
| `options.faceColors?` | [`Color4`](Color4.md)[] |  |
| `options.faceUV?` | [`Vector4`](Vector4.md)[] |  |
| `options.frontUVs?` | [`Vector4`](Vector4.md) |  |
| `options.hasRings?` | `boolean` |  |
| `options.height?` | `number` |  |
| `options.sideOrientation?` | `number` |  |
| `options.subdivisions?` | `number` |  |
| `options.tessellation?` | `number` |  |

#### Returns

[`VertexData`](VertexData.md)

the VertexData of the cylinder, cone or prism

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:1281

___

### CreateDashedLines

▸ `Static` **CreateDashedLines**(`options`): [`VertexData`](VertexData.md)

Create the VertexData for a DashedLines

**`Deprecated`**

use CreateDashedLinesVertexData instead

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | `Object` | an object used to set the following optional parameters for the DashedLines, required but can be empty   - points an array successive Vector3   - dashSize the size of the dashes relative to the dash number, optional, default 3   - gapSize the size of the gap between two successive dashes relative to the dash number, optional, default 1   - dashNb the intended total number of dashes, optional, default 200 |
| `options.dashNb?` | `number` |  |
| `options.dashSize?` | `number` |  |
| `options.gapSize?` | `number` |  |
| `options.points` | [`Vector3`](Vector3.md)[] |  |

#### Returns

[`VertexData`](VertexData.md)

the VertexData for the DashedLines

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:1357

___

### CreateDisc

▸ `Static` **CreateDisc**(`options`): [`VertexData`](VertexData.md)

Creates the VertexData of the Disc or regular Polygon

**`Deprecated`**

use CreateDiscVertexData instead

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | `Object` | an object used to set the following optional parameters for the disc, required but can be empty  * radius the radius of the disc, optional default 0.5  * tessellation the number of polygon sides, optional, default 64  * arc a number from 0 to 1, to create an unclosed polygon based on the fraction of the circumference given by the arc value, optional, default 1  * sideOrientation optional and takes the values : Mesh.FRONTSIDE (default), Mesh.BACKSIDE or Mesh.DOUBLESIDE  * frontUvs only usable when you create a double-sided mesh, used to choose what parts of the texture image to crop and apply on the front side, optional, default vector4 (0, 0, 1, 1)  * backUVs only usable when you create a double-sided mesh, used to choose what parts of the texture image to crop and apply on the back side, optional, default vector4 (0, 0, 1, 1) |
| `options.arc?` | `number` |  |
| `options.backUVs?` | [`Vector4`](Vector4.md) |  |
| `options.frontUVs?` | [`Vector4`](Vector4.md) |  |
| `options.radius?` | `number` |  |
| `options.sideOrientation?` | `number` |  |
| `options.tessellation?` | `number` |  |

#### Returns

[`VertexData`](VertexData.md)

the VertexData of the box

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:1493

___

### CreateGround

▸ `Static` **CreateGround**(`options`): [`VertexData`](VertexData.md)

Creates the VertexData for a Ground

**`Deprecated`**

Please use CreateGroundVertexData instead

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | `Object` | an object used to set the following optional parameters for the Ground, required but can be empty   - width the width (x direction) of the ground, optional, default 1   - height the height (z direction) of the ground, optional, default 1   - subdivisions the number of subdivisions per side, optional, default 1 |
| `options.height?` | `number` |  |
| `options.subdivisions?` | `number` |  |
| `options.subdivisionsX?` | `number` |  |
| `options.subdivisionsY?` | `number` |  |
| `options.width?` | `number` |  |

#### Returns

[`VertexData`](VertexData.md)

the VertexData of the Ground

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:1375

___

### CreateGroundFromHeightMap

▸ `Static` **CreateGroundFromHeightMap**(`options`): [`VertexData`](VertexData.md)

Creates the VertexData of the Ground designed from a heightmap

**`Deprecated`**

use CreateGroundFromHeightMapVertexData instead

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | `Object` | an object used to set the following parameters for the Ground, required and provided by CreateGroundFromHeightMap  * width the width (x direction) of the ground  * height the height (z direction) of the ground  * subdivisions the number of subdivisions per side  * minHeight the minimum altitude on the ground, optional, default 0  * maxHeight the maximum altitude on the ground, optional default 1  * colorFilter the filter to apply to the image pixel colors to compute the height, optional Color3, default (0.3, 0.59, 0.11)  * buffer the array holding the image color data  * bufferWidth the width of image  * bufferHeight the height of image  * alphaFilter Remove any data where the alpha channel is below this value, defaults 0 (all data visible) |
| `options.alphaFilter` | `number` |  |
| `options.buffer` | `Uint8Array` |  |
| `options.bufferHeight` | `number` |  |
| `options.bufferWidth` | `number` |  |
| `options.colorFilter` | [`Color3`](Color3.md) |  |
| `options.height` | `number` |  |
| `options.maxHeight` | `number` |  |
| `options.minHeight` | `number` |  |
| `options.subdivisions` | `number` |  |
| `options.width` | `number` |  |

#### Returns

[`VertexData`](VertexData.md)

the VertexData of the Ground designed from a heightmap

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:1438

___

### CreateIcoSphere

▸ `Static` **CreateIcoSphere**(`options`): [`VertexData`](VertexData.md)

Creates the VertexData of the IcoSphere

**`Deprecated`**

use CreateIcoSphereVertexData instead

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | `Object` | an object used to set the following optional parameters for the IcoSphere, required but can be empty  * radius the radius of the IcoSphere, optional default 1  * radiusX allows stretching in the x direction, optional, default radius  * radiusY allows stretching in the y direction, optional, default radius  * radiusZ allows stretching in the z direction, optional, default radius  * flat when true creates a flat shaded mesh, optional, default true  * subdivisions increasing the subdivisions increases the number of faces, optional, default 4  * sideOrientation optional and takes the values : Mesh.FRONTSIDE (default), Mesh.BACKSIDE or Mesh.DOUBLESIDE  * frontUvs only usable when you create a double-sided mesh, used to choose what parts of the texture image to crop and apply on the front side, optional, default vector4 (0, 0, 1, 1)  * backUVs only usable when you create a double-sided mesh, used to choose what parts of the texture image to crop and apply on the back side, optional, default vector4 (0, 0, 1, 1) |
| `options.backUVs?` | [`Vector4`](Vector4.md) |  |
| `options.flat?` | `boolean` |  |
| `options.frontUVs?` | [`Vector4`](Vector4.md) |  |
| `options.radius?` | `number` |  |
| `options.radiusX?` | `number` |  |
| `options.radiusY?` | `number` |  |
| `options.radiusZ?` | `number` |  |
| `options.sideOrientation?` | `number` |  |
| `options.subdivisions?` | `number` |  |

#### Returns

[`VertexData`](VertexData.md)

the VertexData of the IcoSphere

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:1538

___

### CreateLineSystem

▸ `Static` **CreateLineSystem**(`options`): [`VertexData`](VertexData.md)

Creates the VertexData of the LineSystem

**`Deprecated`**

use CreateLineSystemVertexData instead

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | `Object` | an object used to set the following optional parameters for the LineSystem, required but can be empty   - lines an array of lines, each line being an array of successive Vector3   - colors an array of line colors, each of the line colors being an array of successive Color4, one per line point |
| `options.colors?` | [`Nullable`](../modules.md#nullable)[`Color4`](Color4.md)[][] |  |
| `options.lines` | [`Vector3`](Vector3.md)[][] |  |

#### Returns

[`VertexData`](VertexData.md)

the VertexData of the LineSystem

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:1339

___

### CreatePlane

▸ `Static` **CreatePlane**(`options`): [`VertexData`](VertexData.md)

Creates the VertexData for a Plane

**`Deprecated`**

use CreatePlaneVertexData instead

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | `Object` | an object used to set the following optional parameters for the plane, required but can be empty  * size sets the width and height of the plane to the value of size, optional default 1  * width sets the width (x direction) of the plane, overwrites the width set by size, optional, default size  * height sets the height (y direction) of the plane, overwrites the height set by size, optional, default size  * sideOrientation optional and takes the values : Mesh.FRONTSIDE (default), Mesh.BACKSIDE or Mesh.DOUBLESIDE  * frontUvs only usable when you create a double-sided mesh, used to choose what parts of the texture image to crop and apply on the front side, optional, default vector4 (0, 0, 1, 1)  * backUVs only usable when you create a double-sided mesh, used to choose what parts of the texture image to crop and apply on the back side, optional, default vector4 (0, 0, 1, 1) |
| `options.backUVs?` | [`Vector4`](Vector4.md) |  |
| `options.frontUVs?` | [`Vector4`](Vector4.md) |  |
| `options.height?` | `number` |  |
| `options.sideOrientation?` | `number` |  |
| `options.size?` | `number` |  |
| `options.width?` | `number` |  |

#### Returns

[`VertexData`](VertexData.md)

the VertexData of the box

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:1471

___

### CreatePolygon

▸ `Static` **CreatePolygon**(`polygon`, `sideOrientation`, `fUV?`, `fColors?`, `frontUVs?`, `backUVs?`, `wrap?`): [`VertexData`](VertexData.md)

Creates the VertexData for an irregular Polygon in the XoZ plane using a mesh built by polygonTriangulation.build()
All parameters are provided by CreatePolygon as needed

**`Deprecated`**

use CreatePolygonVertexData instead

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `polygon` | [`Mesh`](Mesh.md) | a mesh built from polygonTriangulation.build() |
| `sideOrientation` | `number` | takes the values Mesh.FRONTSIDE (default), Mesh.BACKSIDE or Mesh.DOUBLESIDE |
| `fUV?` | [`Vector4`](Vector4.md)[] | an array of Vector4 elements used to set different images to the top, rings and bottom respectively |
| `fColors?` | [`Color4`](Color4.md)[] | an array of Color3 elements used to set different colors to the top, rings and bottom respectively |
| `frontUVs?` | [`Vector4`](Vector4.md) | only usable when you create a double-sided mesh, used to choose what parts of the texture image to crop and apply on the front side, optional, default vector4 (0, 0, 1, 1) |
| `backUVs?` | [`Vector4`](Vector4.md) | only usable when you create a double-sided mesh, used to choose what parts of the texture image to crop and apply on the back side, optional, default vector4 (0, 0, 1, 1) |
| `wrap?` | `boolean` | a boolean, default false, when true and fUVs used texture is wrapped around all sides, when false texture is applied side |

#### Returns

[`VertexData`](VertexData.md)

the VertexData of the Polygon

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:1510

___

### CreatePolyhedron

▸ `Static` **CreatePolyhedron**(`options`): [`VertexData`](VertexData.md)

Creates the VertexData for a Polyhedron

**`Deprecated`**

use CreatePolyhedronVertexData instead

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | `Object` | an object used to set the following optional parameters for the polyhedron, required but can be empty  * type provided types are:   * 0 : Tetrahedron, 1 : Octahedron, 2 : Dodecahedron, 3 : Icosahedron, 4 : Rhombicuboctahedron, 5 : Triangular Prism, 6 : Pentagonal Prism, 7 : Hexagonal Prism, 8 : Square Pyramid (J1)   * 9 : Pentagonal Pyramid (J2), 10 : Triangular Dipyramid (J12), 11 : Pentagonal Dipyramid (J13), 12 : Elongated Square Dipyramid (J15), 13 : Elongated Pentagonal Dipyramid (J16), 14 : Elongated Pentagonal Cupola (J20)  * size the size of the IcoSphere, optional default 1  * sizeX allows stretching in the x direction, optional, default size  * sizeY allows stretching in the y direction, optional, default size  * sizeZ allows stretching in the z direction, optional, default size  * custom a number that overwrites the type to create from an extended set of polyhedron from https://www.babylonjs-playground.com/#21QRSK#15 with minimised editor  * faceUV an array of Vector4 elements used to set different images to the top, rings and bottom respectively  * faceColors an array of Color3 elements used to set different colors to the top, rings and bottom respectively  * flat when true creates a flat shaded mesh, optional, default true  * subdivisions increasing the subdivisions increases the number of faces, optional, default 4  * sideOrientation optional and takes the values : Mesh.FRONTSIDE (default), Mesh.BACKSIDE or Mesh.DOUBLESIDE  * frontUvs only usable when you create a double-sided mesh, used to choose what parts of the texture image to crop and apply on the front side, optional, default vector4 (0, 0, 1, 1)  * backUVs only usable when you create a double-sided mesh, used to choose what parts of the texture image to crop and apply on the back side, optional, default vector4 (0, 0, 1, 1) |
| `options.backUVs?` | [`Vector4`](Vector4.md) |  |
| `options.custom?` | `any` |  |
| `options.faceColors?` | [`Color4`](Color4.md)[] |  |
| `options.faceUV?` | [`Vector4`](Vector4.md)[] |  |
| `options.flat?` | `boolean` |  |
| `options.frontUVs?` | [`Vector4`](Vector4.md) |  |
| `options.sideOrientation?` | `number` |  |
| `options.size?` | `number` |  |
| `options.sizeX?` | `number` |  |
| `options.sizeY?` | `number` |  |
| `options.sizeZ?` | `number` |  |
| `options.type?` | `number` |  |

#### Returns

[`VertexData`](VertexData.md)

the VertexData of the Polyhedron

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:1586

___

### CreateRibbon

▸ `Static` **CreateRibbon**(`options`): [`VertexData`](VertexData.md)

Creates the VertexData for a Ribbon

**`Deprecated`**

use CreateRibbonVertexData instead

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | `Object` | an object used to set the following optional parameters for the ribbon, required but can be empty  * pathArray array of paths, each of which an array of successive Vector3  * closeArray creates a seam between the first and the last paths of the pathArray, optional, default false  * closePath creates a seam between the first and the last points of each path of the path array, optional, default false  * offset a positive integer, only used when pathArray contains a single path (offset = 10 means the point 1 is joined to the point 11), default rounded half size of the pathArray length  * sideOrientation optional and takes the values : Mesh.FRONTSIDE (default), Mesh.BACKSIDE or Mesh.DOUBLESIDE  * frontUvs only usable when you create a double-sided mesh, used to choose what parts of the texture image to crop and apply on the front side, optional, default vector4 (0, 0, 1, 1)  * backUVs only usable when you create a double-sided mesh, used to choose what parts of the texture image to crop and apply on the back side, optional, default vector4 (0, 0, 1, 1)  * invertUV swaps in the U and V coordinates when applying a texture, optional, default false  * uvs a linear array, of length 2 * number of vertices, of custom UV values, optional  * colors a linear array, of length 4 * number of vertices, of custom color values, optional |
| `options.backUVs?` | [`Vector4`](Vector4.md) |  |
| `options.closeArray?` | `boolean` |  |
| `options.closePath?` | `boolean` |  |
| `options.colors?` | [`Color4`](Color4.md)[] |  |
| `options.frontUVs?` | [`Vector4`](Vector4.md) |  |
| `options.invertUV?` | `boolean` |  |
| `options.offset?` | `number` |  |
| `options.pathArray` | [`Vector3`](Vector3.md)[][] |  |
| `options.sideOrientation?` | `number` |  |
| `options.uvs?` | [`Vector2`](Vector2.md)[] |  |

#### Returns

[`VertexData`](VertexData.md)

the VertexData of the ribbon

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:1072

___

### CreateSphere

▸ `Static` **CreateSphere**(`options`): [`VertexData`](VertexData.md)

Creates the VertexData for an ellipsoid, defaults to a sphere

**`Deprecated`**

use CreateSphereVertexData instead

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | `Object` | an object used to set the following optional parameters for the box, required but can be empty  * segments sets the number of horizontal strips optional, default 32  * diameter sets the axes dimensions, diameterX, diameterY and diameterZ to the value of diameter, optional default 1  * diameterX sets the diameterX (x direction) of the ellipsoid, overwrites the diameterX set by diameter, optional, default diameter  * diameterY sets the diameterY (y direction) of the ellipsoid, overwrites the diameterY set by diameter, optional, default diameter  * diameterZ sets the diameterZ (z direction) of the ellipsoid, overwrites the diameterZ set by diameter, optional, default diameter  * arc a number from 0 to 1, to create an unclosed ellipsoid based on the fraction of the circumference (latitude) given by the arc value, optional, default 1  * slice a number from 0 to 1, to create an unclosed ellipsoid based on the fraction of the height (latitude) given by the arc value, optional, default 1  * sideOrientation optional and takes the values : Mesh.FRONTSIDE (default), Mesh.BACKSIDE or Mesh.DOUBLESIDE  * frontUvs only usable when you create a double-sided mesh, used to choose what parts of the texture image to crop and apply on the front side, optional, default vector4 (0, 0, 1, 1)  * backUVs only usable when you create a double-sided mesh, used to choose what parts of the texture image to crop and apply on the back side, optional, default vector4 (0, 0, 1, 1) |
| `options.arc?` | `number` |  |
| `options.backUVs?` | [`Vector4`](Vector4.md) |  |
| `options.diameter?` | `number` |  |
| `options.diameterX?` | `number` |  |
| `options.diameterY?` | `number` |  |
| `options.diameterZ?` | `number` |  |
| `options.frontUVs?` | [`Vector4`](Vector4.md) |  |
| `options.segments?` | `number` |  |
| `options.sideOrientation?` | `number` |  |
| `options.slice?` | `number` |  |

#### Returns

[`VertexData`](VertexData.md)

the VertexData of the ellipsoid

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:1232

___

### CreateTiledBox

▸ `Static` **CreateTiledBox**(`options`): [`VertexData`](VertexData.md)

Creates the VertexData for a tiled box

**`Deprecated`**

Please use CreateTiledBoxVertexData instead

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | `Object` | an object used to set the following optional parameters for the box, required but can be empty  * faceTiles sets the pattern, tile size and number of tiles for a face  * faceUV an array of 6 Vector4 elements used to set different images to each box side  * faceColors an array of 6 Color3 elements used to set different colors to each box side  * sideOrientation optional and takes the values : Mesh.FRONTSIDE (default), Mesh.BACKSIDE or Mesh.DOUBLESIDE |
| `options.alignHorizontal?` | `number` |  |
| `options.alignVertical?` | `number` |  |
| `options.depth?` | `number` |  |
| `options.faceColors?` | [`Color4`](Color4.md)[] |  |
| `options.faceUV?` | [`Vector4`](Vector4.md)[] |  |
| `options.height?` | `number` |  |
| `options.pattern?` | `number` |  |
| `options.sideOrientation?` | `number` |  |
| `options.tileHeight?` | `number` |  |
| `options.tileSize?` | `number` |  |
| `options.tileWidth?` | `number` |  |
| `options.width?` | `number` |  |

#### Returns

[`VertexData`](VertexData.md)

the VertexData of the box

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:1147

___

### CreateTiledGround

▸ `Static` **CreateTiledGround**(`options`): [`VertexData`](VertexData.md)

Creates the VertexData for a TiledGround by subdividing the ground into tiles

**`Deprecated`**

use CreateTiledGroundVertexData instead

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | `Object` | an object used to set the following optional parameters for the Ground, required but can be empty  * xmin the ground minimum X coordinate, optional, default -1  * zmin the ground minimum Z coordinate, optional, default -1  * xmax the ground maximum X coordinate, optional, default 1  * zmax the ground maximum Z coordinate, optional, default 1  * subdivisions a javascript object {w: positive integer, h: positive integer}, `w` and `h` are the numbers of subdivisions on the ground width and height creating 'tiles', default {w: 6, h: 6}  * precision a javascript object {w: positive integer, h: positive integer}, `w` and `h` are the numbers of subdivisions on the tile width and height, default {w: 2, h: 2} |
| `options.precision?` | `Object` |  |
| `options.precision.h` | `number` | - |
| `options.precision.w` | `number` | - |
| `options.subdivisions?` | `Object` |  |
| `options.subdivisions.h` | `number` | - |
| `options.subdivisions.w` | `number` | - |
| `options.xmax` | `number` |  |
| `options.xmin` | `number` |  |
| `options.zmax` | `number` |  |
| `options.zmin` | `number` |  |

#### Returns

[`VertexData`](VertexData.md)

the VertexData of the TiledGround

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:1401

___

### CreateTiledPlane

▸ `Static` **CreateTiledPlane**(`options`): [`VertexData`](VertexData.md)

Creates the VertexData for a tiled plane

**`Deprecated`**

use CreateTiledPlaneVertexData instead

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | `Object` | an object used to set the following optional parameters for the box, required but can be empty  * pattern a limited pattern arrangement depending on the number  * tileSize sets the width, height and depth of the tile to the value of size, optional default 1  * tileWidth sets the width (x direction) of the tile, overwrites the width set by size, optional, default size  * tileHeight sets the height (y direction) of the tile, overwrites the height set by size, optional, default size  * sideOrientation optional and takes the values : Mesh.FRONTSIDE (default), Mesh.BACKSIDE or Mesh.DOUBLESIDE  * frontUvs only usable when you create a double-sided mesh, used to choose what parts of the texture image to crop and apply on the front side, optional, default vector4 (0, 0, 1, 1)  * backUVs only usable when you create a double-sided mesh, used to choose what parts of the texture image to crop and apply on the back side, optional, default vector4 (0, 0, 1, 1) |
| `options.alignHorizontal?` | `number` |  |
| `options.alignVertical?` | `number` |  |
| `options.backUVs?` | [`Vector4`](Vector4.md) |  |
| `options.frontUVs?` | [`Vector4`](Vector4.md) |  |
| `options.height?` | `number` |  |
| `options.pattern?` | `number` |  |
| `options.sideOrientation?` | `number` |  |
| `options.size?` | `number` |  |
| `options.tileHeight?` | `number` |  |
| `options.tileSize?` | `number` |  |
| `options.tileWidth?` | `number` |  |
| `options.width?` | `number` |  |

#### Returns

[`VertexData`](VertexData.md)

the VertexData of the tiled plane

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:1189

___

### CreateTorus

▸ `Static` **CreateTorus**(`options`): [`VertexData`](VertexData.md)

Creates the VertexData for a torus

**`Deprecated`**

use CreateTorusVertexData instead

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | `Object` | an object used to set the following optional parameters for the box, required but can be empty  * diameter the diameter of the torus, optional default 1  * thickness the diameter of the tube forming the torus, optional default 0.5  * tessellation the number of prism sides, 3 for a triangular prism, optional, default 24  * sideOrientation optional and takes the values : Mesh.FRONTSIDE (default), Mesh.BACKSIDE or Mesh.DOUBLESIDE  * frontUvs only usable when you create a double-sided mesh, used to choose what parts of the texture image to crop and apply on the front side, optional, default vector4 (0, 0, 1, 1)  * backUVs only usable when you create a double-sided mesh, used to choose what parts of the texture image to crop and apply on the back side, optional, default vector4 (0, 0, 1, 1) |
| `options.backUVs?` | [`Vector4`](Vector4.md) |  |
| `options.diameter?` | `number` |  |
| `options.frontUVs?` | [`Vector4`](Vector4.md) |  |
| `options.sideOrientation?` | `number` |  |
| `options.tessellation?` | `number` |  |
| `options.thickness?` | `number` |  |

#### Returns

[`VertexData`](VertexData.md)

the VertexData of the torus

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:1318

___

### CreateTorusKnot

▸ `Static` **CreateTorusKnot**(`options`): [`VertexData`](VertexData.md)

Creates the VertexData for a TorusKnot

**`Deprecated`**

use CreateTorusKnotVertexData instead

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | `Object` | an object used to set the following optional parameters for the TorusKnot, required but can be empty  * radius the radius of the torus knot, optional, default 2  * tube the thickness of the tube, optional, default 0.5  * radialSegments the number of sides on each tube segments, optional, default 32  * tubularSegments the number of tubes to decompose the knot into, optional, default 32  * p the number of windings around the z axis, optional,  default 2  * q the number of windings around the x axis, optional,  default 3  * sideOrientation optional and takes the values : Mesh.FRONTSIDE (default), Mesh.BACKSIDE or Mesh.DOUBLESIDE  * frontUvs only usable when you create a double-sided mesh, used to choose what parts of the texture image to crop and apply on the front side, optional, default vector4 (0, 0, 1, 1)  * backUVs only usable when you create a double-sided mesh, used to choose what parts of the texture image to crop and apply on the back side, optional, default vector4 (0, 0, 1, 1) |
| `options.backUVs?` | [`Vector4`](Vector4.md) |  |
| `options.frontUVs?` | [`Vector4`](Vector4.md) |  |
| `options.p?` | `number` |  |
| `options.q?` | `number` |  |
| `options.radialSegments?` | `number` |  |
| `options.radius?` | `number` |  |
| `options.sideOrientation?` | `number` |  |
| `options.tube?` | `number` |  |
| `options.tubularSegments?` | `number` |  |

#### Returns

[`VertexData`](VertexData.md)

the VertexData of the Torus Knot

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:1647

___

### ExtractFromGeometry

▸ `Static` **ExtractFromGeometry**(`geometry`, `copyWhenShared?`, `forceCopy?`): [`VertexData`](VertexData.md)

Extracts the vertexData from the geometry

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `geometry` | [`Geometry`](Geometry.md) | the geometry from which to extract the VertexData |
| `copyWhenShared?` | `boolean` | defines if the VertexData must be cloned when the geometry is shared between multiple meshes, optional, default false |
| `forceCopy?` | `boolean` | indicating that the VertexData must be cloned, optional, default false |

#### Returns

[`VertexData`](VertexData.md)

the object VertexData associated to the passed mesh

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:978

___

### ExtractFromMesh

▸ `Static` **ExtractFromMesh**(`mesh`, `copyWhenShared?`, `forceCopy?`): [`VertexData`](VertexData.md)

Extracts the vertexData from a mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`Mesh`](Mesh.md) | the mesh from which to extract the VertexData |
| `copyWhenShared?` | `boolean` | defines if the VertexData must be cloned when shared between multiple meshes, optional, default false |
| `forceCopy?` | `boolean` | indicating that the VertexData must be cloned, optional, default false |

#### Returns

[`VertexData`](VertexData.md)

the object VertexData associated to the passed mesh

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:967

___

### ImportVertexData

▸ `Static` **ImportVertexData**(`parsedVertexData`, `geometry`): `void`

Applies VertexData created from the imported parameters to the geometry

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `parsedVertexData` | `any` | the parsed data from an imported file |
| `geometry` | [`Geometry`](Geometry.md) | the geometry to apply the VertexData to |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:1980

___

### \_ExtractFrom

▸ `Static` `Private` **_ExtractFrom**(`meshOrGeometry`, `copyWhenShared?`, `forceCopy?`): [`VertexData`](VertexData.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `meshOrGeometry` | [`IGetSetVerticesData`](../interfaces/IGetSetVerticesData.md) |
| `copyWhenShared?` | `boolean` |
| `forceCopy?` | `boolean` |

#### Returns

[`VertexData`](VertexData.md)

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:982

___

### \_FlipFaces

▸ `Static` `Private` **_FlipFaces**(`indices`, `offset?`, `length?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `indices` | [`IndicesArray`](../modules.md#indicesarray) | `undefined` |
| `offset` | `number` | `0` |
| `length` | `number` | `indices.length` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:501

___

### \_MergeElement

▸ `Static` `Private` **_MergeElement**(`kind`, `source`, `transform`, `others`): [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray)

#### Parameters

| Name | Type |
| :------ | :------ |
| `kind` | `string` |
| `source` | [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray) |
| `transform` | `undefined` \| [`Matrix`](Matrix.md) |
| `others` | readonly readonly [[`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray), `undefined` \| [`Matrix`](Matrix.md)][] |

#### Returns

[`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray)

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:764

___

### \_TransformVector3Coordinates

▸ `Static` `Private` **_TransformVector3Coordinates**(`coordinates`, `transformation`, `offset?`, `length?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `coordinates` | [`FloatArray`](../modules.md#floatarray) | `undefined` |
| `transformation` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | `undefined` |
| `offset` | `number` | `0` |
| `length` | `number` | `coordinates.length` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:461

___

### \_TransformVector3Normals

▸ `Static` `Private` **_TransformVector3Normals**(`normals`, `transformation`, `offset?`, `length?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `normals` | [`FloatArray`](../modules.md#floatarray) | `undefined` |
| `transformation` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | `undefined` |
| `offset` | `number` | `0` |
| `length` | `number` | `normals.length` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:474

___

### \_TransformVector4Normals

▸ `Static` `Private` **_TransformVector4Normals**(`normals`, `transformation`, `offset?`, `length?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `normals` | [`FloatArray`](../modules.md#floatarray) | `undefined` |
| `transformation` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | `undefined` |
| `offset` | `number` | `0` |
| `length` | `number` | `normals.length` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/mesh.vertexData.ts:487
