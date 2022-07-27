[@dev/core](../README.md) / [Exports](../modules.md) / SubMesh

# Class: SubMesh

Defines a subdivision inside a mesh

## Implements

- [`ICullable`](../interfaces/ICullable.md)

## Table of contents

### Constructors

- [constructor](SubMesh.md#constructor)

### Properties

- [\_boundingInfo](SubMesh.md#_boundinginfo)
- [\_currentMaterial](SubMesh.md#_currentmaterial)
- [\_engine](SubMesh.md#_engine)
- [\_linesIndexBuffer](SubMesh.md#_linesindexbuffer)
- [\_mainDrawWrapperOverride](SubMesh.md#_maindrawwrapperoverride)
- [\_mesh](SubMesh.md#_mesh)
- [\_renderingMesh](SubMesh.md#_renderingmesh)
- [indexCount](SubMesh.md#indexcount)
- [indexStart](SubMesh.md#indexstart)
- [materialIndex](SubMesh.md#materialindex)
- [verticesCount](SubMesh.md#verticescount)
- [verticesStart](SubMesh.md#verticesstart)

### Accessors

- [IsGlobal](SubMesh.md#isglobal)
- [effect](SubMesh.md#effect)
- [materialDefines](SubMesh.md#materialdefines)

### Methods

- [\_isMultiMaterial](SubMesh.md#_ismultimaterial)
- [canIntersects](SubMesh.md#canintersects)
- [clone](SubMesh.md#clone)
- [dispose](SubMesh.md#dispose)
- [getBoundingInfo](SubMesh.md#getboundinginfo)
- [getClassName](SubMesh.md#getclassname)
- [getEffectiveMesh](SubMesh.md#geteffectivemesh)
- [getMaterial](SubMesh.md#getmaterial)
- [getMesh](SubMesh.md#getmesh)
- [getRenderingMesh](SubMesh.md#getrenderingmesh)
- [getReplacementMesh](SubMesh.md#getreplacementmesh)
- [intersects](SubMesh.md#intersects)
- [isCompletelyInFrustum](SubMesh.md#iscompletelyinfrustum)
- [isInFrustum](SubMesh.md#isinfrustum)
- [projectToRef](SubMesh.md#projecttoref)
- [refreshBoundingInfo](SubMesh.md#refreshboundinginfo)
- [render](SubMesh.md#render)
- [resetDrawCache](SubMesh.md#resetdrawcache)
- [setBoundingInfo](SubMesh.md#setboundinginfo)
- [setEffect](SubMesh.md#seteffect)
- [updateBoundingInfo](SubMesh.md#updateboundinginfo)
- [AddToMesh](SubMesh.md#addtomesh)
- [CreateFromIndices](SubMesh.md#createfromindices)

## Constructors

### constructor

• **new SubMesh**(`materialIndex`, `verticesStart`, `verticesCount`, `indexStart`, `indexCount`, `mesh`, `renderingMesh?`, `createBoundingBox?`, `addToMesh?`)

Creates a new submesh

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `materialIndex` | `number` | `undefined` | defines the material index to use |
| `verticesStart` | `number` | `undefined` | defines vertex index start |
| `verticesCount` | `number` | `undefined` | defines vertices count |
| `indexStart` | `number` | `undefined` | defines index start |
| `indexCount` | `number` | `undefined` | defines indices count |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | `undefined` | defines the parent mesh |
| `renderingMesh?` | [`Mesh`](Mesh.md) | `undefined` | defines an optional rendering mesh |
| `createBoundingBox` | `boolean` | `true` | defines if bounding box should be created for this submesh |
| `addToMesh` | `boolean` | `true` | defines a boolean indicating that the submesh must be added to the mesh.subMeshes array (true by default) |

#### Defined in

https://github.com/babylon.js/core/src/Meshes/subMesh.ts:198

## Properties

### \_boundingInfo

• `Private` **\_boundingInfo**: [`BoundingInfo`](BoundingInfo.md)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/subMesh.ts:141

___

### \_currentMaterial

• `Private` **\_currentMaterial**: [`Nullable`](../modules.md#nullable)[`Material`](Material.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/subMesh.ts:159

___

### \_engine

• `Private` **\_engine**: [`Engine`](Engine.md)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/subMesh.ts:29

___

### \_linesIndexBuffer

• `Private` **\_linesIndexBuffer**: [`Nullable`](../modules.md#nullable)[`DataBuffer`](DataBuffer.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/subMesh.ts:142

___

### \_mainDrawWrapperOverride

• `Private` **\_mainDrawWrapperOverride**: [`Nullable`](../modules.md#nullable)`DrawWrapper` = `null`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/subMesh.ts:32

___

### \_mesh

• `Private` **\_mesh**: [`AbstractMesh`](AbstractMesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/subMesh.ts:139

___

### \_renderingMesh

• `Private` **\_renderingMesh**: [`Mesh`](Mesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/subMesh.ts:140

___

### indexCount

• **indexCount**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/subMesh.ts:208

___

### indexStart

• **indexStart**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/subMesh.ts:206

___

### materialIndex

• **materialIndex**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/subMesh.ts:200

___

### verticesCount

• **verticesCount**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/subMesh.ts:204

___

### verticesStart

• **verticesStart**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/subMesh.ts:202

## Accessors

### IsGlobal

• `get` **IsGlobal**(): `boolean`

Returns true if this submesh covers the entire parent mesh

**`Ignorenaming`**

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/subMesh.ts:237

___

### effect

• `get` **effect**(): [`Nullable`](../modules.md#nullable)[`Effect`](Effect.md)

Gets associated (main) effect (possibly the effect override if defined)

#### Returns

[`Nullable`](../modules.md#nullable)[`Effect`](Effect.md)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/subMesh.ts:78

___

### materialDefines

• `get` **materialDefines**(): [`Nullable`](../modules.md#nullable)[`MaterialDefines`](MaterialDefines.md)

Gets material defines used by the effect associated to the sub mesh

#### Returns

[`Nullable`](../modules.md#nullable)[`MaterialDefines`](MaterialDefines.md)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/subMesh.ts:37

• `set` **materialDefines**(`defines`): `void`

Sets material defines used by the effect associated to the sub mesh

#### Parameters

| Name | Type |
| :------ | :------ |
| `defines` | [`Nullable`](../modules.md#nullable)[`MaterialDefines`](MaterialDefines.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/subMesh.ts:44

## Methods

### \_isMultiMaterial

▸ `Private` **_isMultiMaterial**(`material`): material is MultiMaterial

#### Parameters

| Name | Type |
| :------ | :------ |
| `material` | [`Material`](Material.md) |

#### Returns

material is MultiMaterial

#### Defined in

https://github.com/babylon.js/core/src/Meshes/subMesh.ts:321

___

### canIntersects

▸ **canIntersects**(`ray`): `boolean`

Checks if the submesh intersects with a ray

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ray` | [`Ray`](Ray.md) | defines the ray to test |

#### Returns

`boolean`

true is the passed ray intersects the submesh bounding box

#### Defined in

https://github.com/babylon.js/core/src/Meshes/subMesh.ts:459

___

### clone

▸ **clone**(`newMesh`, `newRenderingMesh?`): [`SubMesh`](SubMesh.md)

Creates a new submesh from the passed mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newMesh` | [`AbstractMesh`](AbstractMesh.md) | defines the new hosting mesh |
| `newRenderingMesh?` | [`Mesh`](Mesh.md) | defines an optional rendering mesh |

#### Returns

[`SubMesh`](SubMesh.md)

the new submesh

#### Defined in

https://github.com/babylon.js/core/src/Meshes/subMesh.ts:708

___

### dispose

▸ **dispose**(): `void`

Release associated resources

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/subMesh.ts:729

___

### getBoundingInfo

▸ **getBoundingInfo**(): [`BoundingInfo`](BoundingInfo.md)

Returns the submesh BoundingInfo object

#### Returns

[`BoundingInfo`](BoundingInfo.md)

current bounding info (or mesh's one if the submesh is global)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/subMesh.ts:245

___

### getClassName

▸ **getClassName**(): `string`

Gets the class name

#### Returns

`string`

the string "SubMesh".

#### Defined in

https://github.com/babylon.js/core/src/Meshes/subMesh.ts:746

___

### getEffectiveMesh

▸ **getEffectiveMesh**(): [`AbstractMesh`](AbstractMesh.md)

Returns the effective mesh of the submesh

#### Returns

[`AbstractMesh`](AbstractMesh.md)

the effective mesh (could be different from parent mesh)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/subMesh.ts:291

___

### getMaterial

▸ **getMaterial**(`getDefaultMaterial?`): [`Nullable`](../modules.md#nullable)[`Material`](Material.md)

Returns the submesh material

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `getDefaultMaterial` | `boolean` | `true` | Defines whether or not to get the default material if nothing has been defined. |

#### Returns

[`Nullable`](../modules.md#nullable)[`Material`](Material.md)

null or the current material

#### Defined in

https://github.com/babylon.js/core/src/Meshes/subMesh.ts:302

___

### getMesh

▸ **getMesh**(): [`AbstractMesh`](AbstractMesh.md)

Returns the mesh of the current submesh

#### Returns

[`AbstractMesh`](AbstractMesh.md)

the parent mesh

#### Defined in

https://github.com/babylon.js/core/src/Meshes/subMesh.ts:267

___

### getRenderingMesh

▸ **getRenderingMesh**(): [`Mesh`](Mesh.md)

Returns the rendering mesh of the submesh

#### Returns

[`Mesh`](Mesh.md)

the rendering mesh (could be different from parent mesh)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/subMesh.ts:275

___

### getReplacementMesh

▸ **getReplacementMesh**(): [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

Returns the replacement mesh of the submesh

#### Returns

[`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

the replacement mesh (could be different from parent mesh)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/subMesh.ts:283

___

### intersects

▸ **intersects**(`ray`, `positions`, `indices`, `fastCheck?`, `trianglePredicate?`): [`Nullable`](../modules.md#nullable)`IntersectionInfo`

Intersects current submesh with a ray

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ray` | [`Ray`](Ray.md) | defines the ray to test |
| `positions` | [`Vector3`](Vector3.md)[] | defines mesh's positions array |
| `indices` | [`IndicesArray`](../modules.md#indicesarray) | defines mesh's indices array |
| `fastCheck?` | `boolean` | defines if the first intersection will be used (and not the closest) |
| `trianglePredicate?` | [`TrianglePickingPredicate`](../modules.md#trianglepickingpredicate) | defines an optional predicate used to select faces when a mesh intersection is detected |

#### Returns

[`Nullable`](../modules.md#nullable)`IntersectionInfo`

intersection info or null if no intersection

#### Defined in

https://github.com/babylon.js/core/src/Meshes/subMesh.ts:477

___

### isCompletelyInFrustum

▸ **isCompletelyInFrustum**(`frustumPlanes`): `boolean`

True is the submesh bounding box is completely inside the frustum defined by the passed array of planes

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `frustumPlanes` | [`Plane`](Plane.md)[] | defines the frustum planes |

#### Returns

`boolean`

true if the submesh is inside the frustum

#### Implementation of

[ICullable](../interfaces/ICullable.md).[isCompletelyInFrustum](../interfaces/ICullable.md#iscompletelyinfrustum)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/subMesh.ts:416

___

### isInFrustum

▸ **isInFrustum**(`frustumPlanes`): `boolean`

True is the submesh bounding box intersects the frustum defined by the passed array of planes.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `frustumPlanes` | [`Plane`](Plane.md)[] | defines the frustum planes |

#### Returns

`boolean`

true if the submesh is intersecting with the frustum

#### Implementation of

[ICullable](../interfaces/ICullable.md).[isInFrustum](../interfaces/ICullable.md#isinfrustum)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/subMesh.ts:402

___

### projectToRef

▸ **projectToRef**(`vector`, `positions`, `indices`, `ref`): `number`

Projects a point on this submesh and stores the result in "ref"

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vector` | [`Vector3`](Vector3.md) | point to project |
| `positions` | [`Vector3`](Vector3.md)[] | defines mesh's positions array |
| `indices` | [`IndicesArray`](../modules.md#indicesarray) | defines mesh's indices array |
| `ref` | [`Vector3`](Vector3.md) | vector that will store the result |

#### Returns

`number`

distance from the point and the submesh, or -1 if the mesh rendering mode doesn't support projections

#### Defined in

https://github.com/babylon.js/core/src/Meshes/subMesh.project.ts:21

___

### refreshBoundingInfo

▸ **refreshBoundingInfo**(`data?`): [`SubMesh`](SubMesh.md)

Sets a new updated BoundingInfo object to the submesh

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `data` | [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray) | `null` | defines an optional position array to use to determine the bounding info |

#### Returns

[`SubMesh`](SubMesh.md)

the SubMesh

#### Defined in

https://github.com/babylon.js/core/src/Meshes/subMesh.ts:332

___

### render

▸ **render**(`enableAlphaMode`): [`SubMesh`](SubMesh.md)

Renders the submesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `enableAlphaMode` | `boolean` | defines if alpha needs to be used |

#### Returns

[`SubMesh`](SubMesh.md)

the submesh

#### Defined in

https://github.com/babylon.js/core/src/Meshes/subMesh.ts:430

___

### resetDrawCache

▸ **resetDrawCache**(`passId?`): `void`

Resets the draw wrappers cache

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `passId?` | `number` | If provided, releases only the draw wrapper corresponding to this render pass id |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/subMesh.ts:123

___

### setBoundingInfo

▸ **setBoundingInfo**(`boundingInfo`): [`SubMesh`](SubMesh.md)

Sets the submesh BoundingInfo

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `boundingInfo` | [`BoundingInfo`](BoundingInfo.md) | defines the new bounding info to use |

#### Returns

[`SubMesh`](SubMesh.md)

the SubMesh

#### Defined in

https://github.com/babylon.js/core/src/Meshes/subMesh.ts:258

___

### setEffect

▸ **setEffect**(`effect`, `defines?`, `materialContext?`, `resetContext?`): `void`

Sets associated effect (effect used to render this submesh)

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `effect` | [`Nullable`](../modules.md#nullable)[`Effect`](Effect.md) | `undefined` | defines the effect to associate with |
| `defines` | [`Nullable`](../modules.md#nullable)`string` \| [`MaterialDefines`](MaterialDefines.md) | `null` | defines the set of defines used to compile this effect |
| `materialContext?` | `IMaterialContext` | `undefined` | material context associated to the effect |
| `resetContext` | `boolean` | `true` | true to reset the draw context |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/subMesh.ts:107

___

### updateBoundingInfo

▸ **updateBoundingInfo**(`world`): [`SubMesh`](SubMesh.md)

Updates the submesh BoundingInfo

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `world` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the world matrix to use to update the bounding info |

#### Returns

[`SubMesh`](SubMesh.md)

the submesh

#### Defined in

https://github.com/babylon.js/core/src/Meshes/subMesh.ts:384

___

### AddToMesh

▸ `Static` **AddToMesh**(`materialIndex`, `verticesStart`, `verticesCount`, `indexStart`, `indexCount`, `mesh`, `renderingMesh?`, `createBoundingBox?`): [`SubMesh`](SubMesh.md)

Add a new submesh to a mesh

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `materialIndex` | `number` | `undefined` | defines the material index to use |
| `verticesStart` | `number` | `undefined` | defines vertex index start |
| `verticesCount` | `number` | `undefined` | defines vertices count |
| `indexStart` | `number` | `undefined` | defines index start |
| `indexCount` | `number` | `undefined` | defines indices count |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | `undefined` | defines the parent mesh |
| `renderingMesh?` | [`Mesh`](Mesh.md) | `undefined` | defines an optional rendering mesh |
| `createBoundingBox` | `boolean` | `true` | defines if bounding box should be created for this submesh |

#### Returns

[`SubMesh`](SubMesh.md)

the new submesh

#### Defined in

https://github.com/babylon.js/core/src/Meshes/subMesh.ts:173

___

### CreateFromIndices

▸ `Static` **CreateFromIndices**(`materialIndex`, `startIndex`, `indexCount`, `mesh`, `renderingMesh?`, `createBoundingBox?`): [`SubMesh`](SubMesh.md)

Creates a new submesh from indices data

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `materialIndex` | `number` | `undefined` | the index of the main mesh material |
| `startIndex` | `number` | `undefined` | the index where to start the copy in the mesh indices array |
| `indexCount` | `number` | `undefined` | the number of indices to copy then from the startIndex |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | `undefined` | the main mesh to create the submesh from |
| `renderingMesh?` | [`Mesh`](Mesh.md) | `undefined` | the optional rendering mesh |
| `createBoundingBox` | `boolean` | `true` | defines if bounding box should be created for this submesh |

#### Returns

[`SubMesh`](SubMesh.md)

a new submesh

#### Defined in

https://github.com/babylon.js/core/src/Meshes/subMesh.ts:761
