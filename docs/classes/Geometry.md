[@dev/core](../README.md) / [Exports](../modules.md) / Geometry

# Class: Geometry

Class used to store geometry data (vertex buffers + index buffer)

## Implements

- [`IGetSetVerticesData`](../interfaces/IGetSetVerticesData.md)

## Table of contents

### Constructors

- [constructor](Geometry.md#constructor)

### Properties

- [\_boundingBias](Geometry.md#_boundingbias)
- [\_engine](Geometry.md#_engine)
- [\_extend](Geometry.md#_extend)
- [\_indexBuffer](Geometry.md#_indexbuffer)
- [\_indexBufferIsUpdatable](Geometry.md#_indexbufferisupdatable)
- [\_isDisposed](Geometry.md#_isdisposed)
- [\_meshes](Geometry.md#_meshes)
- [\_positionsCache](Geometry.md#_positionscache)
- [\_scene](Geometry.md#_scene)
- [\_totalVertices](Geometry.md#_totalvertices)
- [\_updatable](Geometry.md#_updatable)
- [\_vertexArrayObjects](Geometry.md#_vertexarrayobjects)
- [delayLoadState](Geometry.md#delayloadstate)
- [delayLoadingFile](Geometry.md#delayloadingfile)
- [id](Geometry.md#id)
- [onGeometryUpdated](Geometry.md#ongeometryupdated)
- [uniqueId](Geometry.md#uniqueid)
- [useBoundingInfoFromGeometry](Geometry.md#useboundinginfofromgeometry)

### Accessors

- [boundingBias](Geometry.md#boundingbias)
- [doNotSerialize](Geometry.md#donotserialize)
- [extend](Geometry.md#extend)
- [meshes](Geometry.md#meshes)

### Methods

- [\_applyToMesh](Geometry.md#_applytomesh)
- [\_disposeVertexArrayObjects](Geometry.md#_disposevertexarrayobjects)
- [\_notifyUpdate](Geometry.md#_notifyupdate)
- [\_queueLoad](Geometry.md#_queueload)
- [\_toNumberArray](Geometry.md#_tonumberarray)
- [\_updateBoundingInfo](Geometry.md#_updateboundinginfo)
- [\_updateExtend](Geometry.md#_updateextend)
- [applyToMesh](Geometry.md#applytomesh)
- [clearCachedData](Geometry.md#clearcacheddata)
- [copy](Geometry.md#copy)
- [dispose](Geometry.md#dispose)
- [getEngine](Geometry.md#getengine)
- [getIndexBuffer](Geometry.md#getindexbuffer)
- [getIndices](Geometry.md#getindices)
- [getScene](Geometry.md#getscene)
- [getTotalIndices](Geometry.md#gettotalindices)
- [getTotalVertices](Geometry.md#gettotalvertices)
- [getVertexBuffer](Geometry.md#getvertexbuffer)
- [getVertexBuffers](Geometry.md#getvertexbuffers)
- [getVerticesData](Geometry.md#getverticesdata)
- [getVerticesDataKinds](Geometry.md#getverticesdatakinds)
- [isDisposed](Geometry.md#isdisposed)
- [isReady](Geometry.md#isready)
- [isVertexBufferUpdatable](Geometry.md#isvertexbufferupdatable)
- [isVerticesDataPresent](Geometry.md#isverticesdatapresent)
- [load](Geometry.md#load)
- [releaseForMesh](Geometry.md#releaseformesh)
- [removeVerticesData](Geometry.md#removeverticesdata)
- [serialize](Geometry.md#serialize)
- [serializeVerticeData](Geometry.md#serializeverticedata)
- [setAllVerticesData](Geometry.md#setallverticesdata)
- [setIndices](Geometry.md#setindices)
- [setVerticesBuffer](Geometry.md#setverticesbuffer)
- [setVerticesData](Geometry.md#setverticesdata)
- [toLeftHanded](Geometry.md#tolefthanded)
- [updateIndices](Geometry.md#updateindices)
- [updateVerticesData](Geometry.md#updateverticesdata)
- [updateVerticesDataDirectly](Geometry.md#updateverticesdatadirectly)
- [CreateGeometryForMesh](Geometry.md#creategeometryformesh)
- [ExtractFromMesh](Geometry.md#extractfrommesh)
- [Parse](Geometry.md#parse)
- [RandomId](Geometry.md#randomid)
- [\_CleanMatricesWeights](Geometry.md#_cleanmatricesweights)
- [\_GetGeometryByLoadedUniqueId](Geometry.md#_getgeometrybyloadeduniqueid)

## Constructors

### constructor

• **new Geometry**(`id`, `scene?`, `vertexData?`, `updatable?`, `mesh?`)

Creates a new geometry

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `id` | `string` | `undefined` | defines the unique ID |
| `scene?` | [`Scene`](Scene.md) | `undefined` | defines the hosting scene |
| `vertexData?` | [`VertexData`](VertexData.md) | `undefined` | defines the VertexData used to get geometry data |
| `updatable` | `boolean` | `false` | defines if geometry must be updatable (false by default) |
| `mesh` | [`Nullable`](../modules.md#nullable)[`Mesh`](Mesh.md) | `null` | defines the mesh that will be associated with the geometry |

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:139

## Properties

### \_boundingBias

• `Private` **\_boundingBias**: [`Vector2`](Vector2.md)

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:65

___

### \_engine

• `Private` **\_engine**: [`Engine`](Engine.md)

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:54

___

### \_extend

• `Private` **\_extend**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `maximum` | [`Vector3`](Vector3.md) |
| `minimum` | [`Vector3`](Vector3.md) |

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:64

___

### \_indexBuffer

• `Private` **\_indexBuffer**: [`Nullable`](../modules.md#nullable)[`DataBuffer`](DataBuffer.md)

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:68

___

### \_indexBufferIsUpdatable

• `Private` **\_indexBufferIsUpdatable**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:69

___

### \_isDisposed

• `Private` **\_isDisposed**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:63

___

### \_meshes

• `Private` **\_meshes**: [`Mesh`](Mesh.md)[]

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:55

___

### \_positionsCache

• `Private` **\_positionsCache**: [`Vector3`](Vector3.md)[] = `[]`

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:82

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:53

___

### \_totalVertices

• `Private` **\_totalVertices**: `number` = `0`

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:56

___

### \_updatable

• `Private` **\_updatable**: `boolean`

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:77

___

### \_vertexArrayObjects

• `Private` **\_vertexArrayObjects**: `Object`

#### Index signature

▪ [key: `string`]: `WebGLVertexArrayObject`

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:76

___

### delayLoadState

• **delayLoadState**: `number` = `Constants.DELAYLOADSTATE_NONE`

Gets the delay loading state of the geometry (none by default which means not delayed)

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:42

___

### delayLoadingFile

• **delayLoadingFile**: [`Nullable`](../modules.md#nullable)`string`

Gets the file containing the data to load when running in delay load state

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:46

___

### id

• **id**: `string`

Gets or sets the ID of the geometry

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:34

___

### onGeometryUpdated

• **onGeometryUpdated**: (`geometry`: [`Geometry`](Geometry.md), `kind?`: `string`) => `void`

#### Type declaration

▸ (`geometry`, `kind?`): `void`

Callback called when the geometry is updated

##### Parameters

| Name | Type |
| :------ | :------ |
| `geometry` | [`Geometry`](Geometry.md) |
| `kind?` | `string` |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:50

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique ID of the geometry

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:38

___

### useBoundingInfoFromGeometry

• **useBoundingInfoFromGeometry**: `boolean` = `false`

If set to true (false by default), the bounding info applied to the meshes sharing this geometry will be the bounding info defined at the class level
and won't be computed based on the vertex positions (which is what we get when useBoundingInfoFromGeometry = false)

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:129

## Accessors

### boundingBias

• `get` **boundingBias**(): [`Vector2`](Vector2.md)

Gets or sets the Bias Vector to apply on the bounding elements (box/sphere), the max extend is computed as v += v * bias.x + bias.y, the min is computed as v -= v * bias.x + bias.y

#### Returns

[`Vector2`](Vector2.md)

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:90

• `set` **boundingBias**(`value`): `void`

Gets or sets the Bias Vector to apply on the bounding elements (box/sphere), the max extend is computed as v += v * bias.x + bias.y, the min is computed as v -= v * bias.x + bias.y

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Vector2`](Vector2.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:97

___

### doNotSerialize

• `get` **doNotSerialize**(): `boolean`

Gets a value indicating that the geometry should not be serialized

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:206

___

### extend

• `get` **extend**(): `Object`

Gets the current extend of the geometry

#### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `maximum` | [`Vector3`](Vector3.md) |
| `minimum` | [`Vector3`](Vector3.md) |

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:175

___

### meshes

• `get` **meshes**(): [`Mesh`](Mesh.md)[]

Get the list of meshes using this geometry

#### Returns

[`Mesh`](Mesh.md)[]

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:121

## Methods

### \_applyToMesh

▸ `Private` **_applyToMesh**(`mesh`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `mesh` | [`Mesh`](Mesh.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:720

___

### \_disposeVertexArrayObjects

▸ `Private` **_disposeVertexArrayObjects**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:901

___

### \_notifyUpdate

▸ `Private` **_notifyUpdate**(`kind?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `kind?` | `string` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:754

___

### \_queueLoad

▸ `Private` **_queueLoad**(`scene`, `onLoaded?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `scene` | [`Scene`](Scene.md) |
| `onLoaded?` | () => `void` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:790

___

### \_toNumberArray

▸ `Private` **_toNumberArray**(`origin`): `number`[]

#### Parameters

| Name | Type |
| :------ | :------ |
| `origin` | [`Nullable`](../modules.md#nullable)`Float32Array` \| [`IndicesArray`](../modules.md#indicesarray) |

#### Returns

`number`[]

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:1037

___

### \_updateBoundingInfo

▸ `Private` **_updateBoundingInfo**(`updateExtends`, `data`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `updateExtends` | `boolean` |
| `data` | [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:362

___

### \_updateExtend

▸ `Private` **_updateExtend**(`data?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `data` | [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray) | `null` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:700

___

### applyToMesh

▸ **applyToMesh**(`mesh`): `void`

Apply current geometry to a given mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`Mesh`](Mesh.md) | defines the mesh to apply geometry to |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:669

___

### clearCachedData

▸ **clearCachedData**(): `void`

Release any memory retained by the cached data on the Geometry.

Call this function to reduce memory footprint of the mesh.
Vertex buffers will not store CPU data anymore (this will prevent picking, collisions or physics to work correctly)

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:1051

___

### copy

▸ **copy**(`id`): [`Geometry`](Geometry.md)

Clone the current geometry into a new geometry

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | defines the unique ID of the new geometry |

#### Returns

[`Geometry`](Geometry.md)

a new geometry object

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:966

___

### dispose

▸ **dispose**(): `void`

Free all associated resources

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:919

___

### getEngine

▸ **getEngine**(): [`Engine`](Engine.md)

Gets the hosting engine

#### Returns

[`Engine`](Engine.md)

the hosting Engine

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:191

___

### getIndexBuffer

▸ **getIndexBuffer**(): [`Nullable`](../modules.md#nullable)[`DataBuffer`](DataBuffer.md)

Gets the index buffer

#### Returns

[`Nullable`](../modules.md#nullable)[`DataBuffer`](DataBuffer.md)

the index buffer

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:617

___

### getIndices

▸ **getIndices**(`copyWhenShared?`, `forceCopy?`): [`Nullable`](../modules.md#nullable)[`IndicesArray`](../modules.md#indicesarray)

Gets the index buffer array

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `copyWhenShared?` | `boolean` | defines if the returned array must be cloned upon returning it if the current geometry is shared between multiple meshes |
| `forceCopy?` | `boolean` | defines a boolean indicating that the returned array must be cloned upon returning it |

#### Returns

[`Nullable`](../modules.md#nullable)[`IndicesArray`](../modules.md#indicesarray)

the index buffer array

#### Implementation of

[IGetSetVerticesData](../interfaces/IGetSetVerticesData.md).[getIndices](../interfaces/IGetSetVerticesData.md#getindices)

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:601

___

### getScene

▸ **getScene**(): [`Scene`](Scene.md)

Gets the hosting scene

#### Returns

[`Scene`](Scene.md)

the hosting Scene

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:183

___

### getTotalIndices

▸ **getTotalIndices**(): `number`

Return the total number of indices

#### Returns

`number`

the total number of indices

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:588

___

### getTotalVertices

▸ **getTotalVertices**(): `number`

Gets total number of vertices

#### Returns

`number`

the total number of vertices

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:429

___

### getVertexBuffer

▸ **getVertexBuffer**(`kind`): [`Nullable`](../modules.md#nullable)[`VertexBuffer`](VertexBuffer.md)

Gets a specific vertex buffer

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `kind` | `string` | defines the data kind (Position, normal, etc...) |

#### Returns

[`Nullable`](../modules.md#nullable)[`VertexBuffer`](VertexBuffer.md)

a VertexBuffer

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:473

___

### getVertexBuffers

▸ **getVertexBuffers**(): [`Nullable`](../modules.md#nullable){ `[key: string]`: [`VertexBuffer`](VertexBuffer.md);  }

Returns all vertex buffers

#### Returns

[`Nullable`](../modules.md#nullable){ `[key: string]`: [`VertexBuffer`](VertexBuffer.md);  }

an object holding all vertex buffers indexed by kind

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:484

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

#### Implementation of

[IGetSetVerticesData](../interfaces/IGetSetVerticesData.md).[getVerticesData](../interfaces/IGetSetVerticesData.md#getverticesdata)

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:444

___

### getVerticesDataKinds

▸ **getVerticesDataKinds**(): `string`[]

Gets a list of all attached data kinds (Position, normal, etc...)

#### Returns

`string`[]

a list of string containing all kinds

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:510

___

### isDisposed

▸ **isDisposed**(): `boolean`

Gets a value indicating if the geometry is disposed

#### Returns

`boolean`

true if the geometry was disposed

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:897

___

### isReady

▸ **isReady**(): `boolean`

Defines if the geometry is ready to use

#### Returns

`boolean`

true if the geometry is ready to be used

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:199

___

### isVertexBufferUpdatable

▸ **isVertexBufferUpdatable**(`kind`): `boolean`

Returns a boolean defining if the vertex data for the requested `kind` is updatable

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `kind` | `string` | defines the data kind (Position, normal, etc...) |

#### Returns

`boolean`

true if the vertex buffer with the specified kind is updatable

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:458

___

### isVerticesDataPresent

▸ **isVerticesDataPresent**(`kind`): `boolean`

Gets a boolean indicating if specific vertex buffer is present

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `kind` | `string` | defines the data kind (Position, normal, etc...) |

#### Returns

`boolean`

true if data is present

#### Implementation of

[IGetSetVerticesData](../interfaces/IGetSetVerticesData.md).[isVerticesDataPresent](../interfaces/IGetSetVerticesData.md#isverticesdatapresent)

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:496

___

### load

▸ **load**(`scene`, `onLoaded?`): `void`

Load the geometry if it was flagged as delay loaded

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | defines the hosting scene |
| `onLoaded?` | () => `void` | defines a callback called when the geometry is loaded |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:773

___

### releaseForMesh

▸ **releaseForMesh**(`mesh`, `shouldDispose?`): `void`

Release the associated resources for a specific mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`Mesh`](Mesh.md) | defines the source mesh |
| `shouldDispose?` | `boolean` | defines if the geometry must be disposed if there is no more mesh pointing to it |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:644

___

### removeVerticesData

▸ **removeVerticesData**(`kind`): `void`

Removes a specific vertex data

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `kind` | `string` | defines the data kind (Position, normal, etc...) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:264

___

### serialize

▸ **serialize**(): `any`

Serialize the current geometry info (and not the vertices data) into a JSON object

#### Returns

`any`

a JSON representation of the current geometry data (without the vertices data)

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:1023

___

### serializeVerticeData

▸ **serializeVerticeData**(): `any`

Serialize all vertices data into a JSON object

#### Returns

`any`

a JSON representation of the current geometry data

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:1067

___

### setAllVerticesData

▸ **setAllVerticesData**(`vertexData`, `updatable?`): `void`

Affects all geometry data in one call

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vertexData` | [`VertexData`](VertexData.md) | defines the geometry data |
| `updatable?` | `boolean` | defines if the geometry must be flagged as updatable (false as default) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:239

___

### setIndices

▸ **setIndices**(`indices`, `totalVertices?`, `updatable?`): `void`

Creates a new index buffer

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `indices` | [`IndicesArray`](../modules.md#indicesarray) | `undefined` | defines the indices to store in the index buffer |
| `totalVertices` | [`Nullable`](../modules.md#nullable)`number` | `null` | defines the total number of vertices (could be null) |
| `updatable` | `boolean` | `false` | defines if the index buffer must be flagged as updatable (false by default) |

#### Returns

`void`

#### Implementation of

[IGetSetVerticesData](../interfaces/IGetSetVerticesData.md).[setIndices](../interfaces/IGetSetVerticesData.md#setindices)

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:560

___

### setVerticesBuffer

▸ **setVerticesBuffer**(`buffer`, `totalVertices?`, `disposeExistingBuffer?`): `void`

Affect a vertex buffer to the geometry. the vertexBuffer.getKind() function is used to determine where to store the data

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `buffer` | [`VertexBuffer`](VertexBuffer.md) | `undefined` | defines the vertex buffer to use |
| `totalVertices` | [`Nullable`](../modules.md#nullable)`number` | `null` | defines the total number of vertices for position kind (could be null) |
| `disposeExistingBuffer` | `boolean` | `true` | disposes the existing buffer, if any (default: true) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:281

___

### setVerticesData

▸ **setVerticesData**(`kind`, `data`, `updatable?`, `stride?`): `void`

Set specific vertex data

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `kind` | `string` | `undefined` | defines the data kind (Position, normal, etc...) |
| `data` | [`FloatArray`](../modules.md#floatarray) | `undefined` | defines the vertex data to use |
| `updatable` | `boolean` | `false` | defines if the vertex must be flagged as updatable (false as default) |
| `stride?` | `number` | `undefined` | defines the stride to use (0 by default). This value is deduced from the kind value if not specified |

#### Returns

`void`

#### Implementation of

[IGetSetVerticesData](../interfaces/IGetSetVerticesData.md).[setVerticesData](../interfaces/IGetSetVerticesData.md#setverticesdata)

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:251

___

### toLeftHanded

▸ **toLeftHanded**(): `void`

Invert the geometry to move from a right handed system to a left handed one.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:828

___

### updateIndices

▸ **updateIndices**(`indices`, `offset?`, `gpuMemoryOnly?`): `void`

Update index buffer

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `indices` | [`IndicesArray`](../modules.md#indicesarray) | `undefined` | defines the indices to store in the index buffer |
| `offset?` | `number` | `undefined` | defines the offset in the target buffer where to store the data |
| `gpuMemoryOnly` | `boolean` | `false` | defines a boolean indicating that only the GPU memory must be updated leaving the CPU version of the indices unchanged (false by default) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:532

___

### updateVerticesData

▸ **updateVerticesData**(`kind`, `data`, `updateExtends?`): `void`

Update a specific vertex buffer
This function will create a new buffer if the current one is not updatable

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `kind` | `string` | `undefined` | defines the data kind (Position, normal, etc...) |
| `data` | [`FloatArray`](../modules.md#floatarray) | `undefined` | defines the data to use |
| `updateExtends` | `boolean` | `false` | defines if the geometry extends must be recomputed (false by default) |

#### Returns

`void`

#### Implementation of

[IGetSetVerticesData](../interfaces/IGetSetVerticesData.md).[updateVerticesData](../interfaces/IGetSetVerticesData.md#updateverticesdata)

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:347

___

### updateVerticesDataDirectly

▸ **updateVerticesDataDirectly**(`kind`, `data`, `offset`, `useBytes?`): `void`

Update a specific vertex buffer
This function will directly update the underlying DataBuffer according to the passed numeric array or Float32Array
It will do nothing if the buffer is not updatable

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `kind` | `string` | `undefined` | defines the data kind (Position, normal, etc...) |
| `data` | [`DataArray`](../modules.md#dataarray) | `undefined` | defines the data to use |
| `offset` | `number` | `undefined` | defines the offset in the target buffer where to store the data |
| `useBytes` | `boolean` | `false` | set to true if the offset is in bytes |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:329

___

### CreateGeometryForMesh

▸ `Static` **CreateGeometryForMesh**(`mesh`): [`Geometry`](Geometry.md)

Static function used to attach a new empty geometry to a mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`Mesh`](Mesh.md) | defines the mesh to attach the geometry to |

#### Returns

[`Geometry`](Geometry.md)

the new Geometry

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:112

___

### ExtractFromMesh

▸ `Static` **ExtractFromMesh**(`mesh`, `id`): [`Nullable`](../modules.md#nullable)[`Geometry`](Geometry.md)

Extracts a clone of a mesh geometry

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`Mesh`](Mesh.md) | defines the source mesh |
| `id` | `string` | defines the unique ID of the new geometry object |

#### Returns

[`Nullable`](../modules.md#nullable)[`Geometry`](Geometry.md)

the new geometry object

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:1168

___

### Parse

▸ `Static` **Parse**(`parsedVertexData`, `scene`, `rootUrl`): [`Nullable`](../modules.md#nullable)[`Geometry`](Geometry.md)

Create a new geometry from persisted data (Using .babylon file format)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `parsedVertexData` | `any` | defines the persisted data |
| `scene` | [`Scene`](Scene.md) | defines the hosting scene |
| `rootUrl` | `string` | defines the root url to use to load assets (like delayed data) |

#### Returns

[`Nullable`](../modules.md#nullable)[`Geometry`](Geometry.md)

the new geometry object

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:1545

___

### RandomId

▸ `Static` **RandomId**(): `string`

You should now use Tools.RandomId(), this method is still here for legacy reasons.
Implementation from http://stackoverflow.com/questions/105034/how-to-create-a-guid-uuid-in-javascript/2117523#answer-2117523
Be aware Math.random() could cause collisions, but:
"All but 6 of the 128 bits of the ID are randomly generated, which means that for any two ids, there's a 1 in 2^^122 (or 5.3x10^^36) chance they'll collide"

#### Returns

`string`

a string containing a new GUID

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:1185

___

### \_CleanMatricesWeights

▸ `Static` `Private` **_CleanMatricesWeights**(`parsedGeometry`, `mesh`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `parsedGeometry` | `any` |
| `mesh` | [`Mesh`](Mesh.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:1466

___

### \_GetGeometryByLoadedUniqueId

▸ `Static` `Private` **_GetGeometryByLoadedUniqueId**(`uniqueId`, `scene`): ``null`` \| [`Geometry`](Geometry.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `uniqueId` | `string` |
| `scene` | [`Scene`](Scene.md) |

#### Returns

``null`` \| [`Geometry`](Geometry.md)

#### Defined in

packages/dev/core/src/Meshes/geometry.ts:1189
