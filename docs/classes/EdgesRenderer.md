[@dev/core](../README.md) / [Exports](../modules.md) / EdgesRenderer

# Class: EdgesRenderer

This class is used to generate edges of the mesh that could then easily be rendered in a scene.

## Hierarchy

- **`EdgesRenderer`**

  ↳ [`LineEdgesRenderer`](LineEdgesRenderer.md)

## Implements

- [`IEdgesRenderer`](../interfaces/IEdgesRenderer.md)

## Table of contents

### Constructors

- [constructor](EdgesRenderer.md#constructor)

### Properties

- [\_buffers](EdgesRenderer.md#_buffers)
- [\_buffersForInstances](EdgesRenderer.md#_buffersforinstances)
- [\_checkVerticesInsteadOfIndices](EdgesRenderer.md#_checkverticesinsteadofindices)
- [\_drawWrapper](EdgesRenderer.md#_drawwrapper)
- [\_epsilon](EdgesRenderer.md#_epsilon)
- [\_ib](EdgesRenderer.md#_ib)
- [\_indicesCount](EdgesRenderer.md#_indicescount)
- [\_lineShader](EdgesRenderer.md#_lineshader)
- [\_linesIndices](EdgesRenderer.md#_linesindices)
- [\_linesNormals](EdgesRenderer.md#_linesnormals)
- [\_linesPositions](EdgesRenderer.md#_linespositions)
- [\_meshDisposeObserver](EdgesRenderer.md#_meshdisposeobserver)
- [\_meshRebuildObserver](EdgesRenderer.md#_meshrebuildobserver)
- [\_options](EdgesRenderer.md#_options)
- [\_source](EdgesRenderer.md#_source)
- [customInstances](EdgesRenderer.md#custominstances)
- [edgesWidthScalerForOrthographic](EdgesRenderer.md#edgeswidthscalerfororthographic)
- [edgesWidthScalerForPerspective](EdgesRenderer.md#edgeswidthscalerforperspective)
- [isEnabled](EdgesRenderer.md#isenabled)

### Accessors

- [lineShader](EdgesRenderer.md#lineshader)
- [linesIndices](EdgesRenderer.md#linesindices)
- [linesNormals](EdgesRenderer.md#linesnormals)
- [linesPositions](EdgesRenderer.md#linespositions)

### Methods

- [\_checkEdge](EdgesRenderer.md#_checkedge)
- [\_generateEdgesLines](EdgesRenderer.md#_generateedgeslines)
- [\_generateEdgesLinesAlternate](EdgesRenderer.md#_generateedgeslinesalternate)
- [\_prepareRessources](EdgesRenderer.md#_prepareressources)
- [\_processEdgeForAdjacencies](EdgesRenderer.md#_processedgeforadjacencies)
- [\_processEdgeForAdjacenciesWithVertices](EdgesRenderer.md#_processedgeforadjacencieswithvertices)
- [\_tessellateTriangle](EdgesRenderer.md#_tessellatetriangle)
- [createLine](EdgesRenderer.md#createline)
- [dispose](EdgesRenderer.md#dispose)
- [isReady](EdgesRenderer.md#isready)
- [render](EdgesRenderer.md#render)
- [\_GetShader](EdgesRenderer.md#_getshader)

## Constructors

### constructor

• **new EdgesRenderer**(`source`, `epsilon?`, `checkVerticesInsteadOfIndices?`, `generateEdgesLines?`, `options?`)

Creates an instance of the EdgesRenderer. It is primarily use to display edges of a mesh.
Beware when you use this class with complex objects as the adjacencies computation can be really long

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `source` | [`AbstractMesh`](AbstractMesh.md) | `undefined` | Mesh used to create edges |
| `epsilon` | `number` | `0.95` | sum of angles in adjacency to check for edge |
| `checkVerticesInsteadOfIndices` | `boolean` | `false` | bases the edges detection on vertices vs indices. Note that this parameter is not used if options.useAlternateEdgeFinder = true |
| `generateEdgesLines` | `boolean` | `true` | should generate Lines or only prepare resources. |
| `options?` | [`IEdgesRendererOptions`](../interfaces/IEdgesRendererOptions.md) | `undefined` | The options to apply when generating the edges |

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:280

## Properties

### \_buffers

• `Protected` **\_buffers**: `Object` = `{}`

#### Index signature

▪ [key: `string`]: [`Nullable`](../modules.md#nullable)[`VertexBuffer`](VertexBuffer.md)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:206

___

### \_buffersForInstances

• `Protected` **\_buffersForInstances**: `Object` = `{}`

#### Index signature

▪ [key: `string`]: [`Nullable`](../modules.md#nullable)[`VertexBuffer`](VertexBuffer.md)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:207

___

### \_checkVerticesInsteadOfIndices

• `Protected` **\_checkVerticesInsteadOfIndices**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:208

___

### \_drawWrapper

• `Protected` `Optional` **\_drawWrapper**: `DrawWrapper`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:202

___

### \_epsilon

• `Protected` **\_epsilon**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:200

___

### \_ib

• `Protected` **\_ib**: [`DataBuffer`](DataBuffer.md)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:205

___

### \_indicesCount

• `Protected` **\_indicesCount**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:201

___

### \_lineShader

• `Protected` **\_lineShader**: [`ShaderMaterial`](ShaderMaterial.md)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:204

___

### \_linesIndices

• `Protected` **\_linesIndices**: `number`[]

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:199

___

### \_linesNormals

• `Protected` **\_linesNormals**: `number`[]

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:198

___

### \_linesPositions

• `Protected` **\_linesPositions**: `number`[]

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:197

___

### \_meshDisposeObserver

• `Private` **\_meshDisposeObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Node`](Node.md)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:212

___

### \_meshRebuildObserver

• `Private` **\_meshRebuildObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`AbstractMesh`](AbstractMesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:211

___

### \_options

• `Protected` **\_options**: [`Nullable`](../modules.md#nullable)[`IEdgesRendererOptions`](../interfaces/IEdgesRendererOptions.md)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:209

___

### \_source

• `Protected` **\_source**: [`AbstractMesh`](AbstractMesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:196

___

### customInstances

• **customInstances**: [`SmartArray`](SmartArray.md)[`Matrix`](Matrix.md)

List of instances to render in case the source mesh has instances

#### Implementation of

[IEdgesRenderer](../interfaces/IEdgesRenderer.md).[customInstances](../interfaces/IEdgesRenderer.md#custominstances)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:246

___

### edgesWidthScalerForOrthographic

• **edgesWidthScalerForOrthographic**: `number` = `1000.0`

Define the size of the edges with an orthographic camera

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:189

___

### edgesWidthScalerForPerspective

• **edgesWidthScalerForPerspective**: `number` = `50.0`

Define the size of the edges with a perspective camera

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:194

___

### isEnabled

• **isEnabled**: `boolean` = `true`

Gets or sets a boolean indicating if the edgesRenderer is active

#### Implementation of

[IEdgesRenderer](../interfaces/IEdgesRenderer.md).[isEnabled](../interfaces/IEdgesRenderer.md#isenabled)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:215

## Accessors

### lineShader

• `get` **lineShader**(): [`ShaderMaterial`](ShaderMaterial.md)

Gets or sets the shader used to draw the lines

#### Returns

[`ShaderMaterial`](ShaderMaterial.md)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:235

• `set` **lineShader**(`shader`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `shader` | [`ShaderMaterial`](ShaderMaterial.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:239

___

### linesIndices

• `get` **linesIndices**(): readonly `number`[]

Gets the indices generated by the edge renderer

#### Returns

readonly `number`[]

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:228

___

### linesNormals

• `get` **linesNormals**(): readonly `number`[]

Gets the normals generated by the edge renderer

#### Returns

readonly `number`[]

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:223

___

### linesPositions

• `get` **linesPositions**(): readonly `number`[]

Gets the vertices generated by the edge renderer

#### Returns

readonly `number`[]

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:218

## Methods

### \_checkEdge

▸ `Private` **_checkEdge**(`faceIndex`, `edge`, `faceNormals`, `p0`, `p1`): `void`

Checks if the pair of p0 and p1 is en edge

#### Parameters

| Name | Type |
| :------ | :------ |
| `faceIndex` | `number` |
| `edge` | `number` |
| `faceNormals` | [`Vector3`](Vector3.md)[] |
| `p0` | [`Vector3`](Vector3.md) |
| `p1` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:401

___

### \_generateEdgesLines

▸ `Private` **_generateEdgesLines**(): `void`

Generates lines edges from adjacencjes

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:770

___

### \_generateEdgesLinesAlternate

▸ `Private` **_generateEdgesLinesAlternate**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:533

___

### \_prepareRessources

▸ `Protected` **_prepareRessources**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:308

___

### \_processEdgeForAdjacencies

▸ `Protected` **_processEdgeForAdjacencies**(`pa`, `pb`, `p0`, `p1`, `p2`): `number`

#### Parameters

| Name | Type |
| :------ | :------ |
| `pa` | `number` |
| `pb` | `number` |
| `p0` | `number` |
| `p1` | `number` |
| `p2` | `number` |

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:359

___

### \_processEdgeForAdjacenciesWithVertices

▸ `Protected` **_processEdgeForAdjacenciesWithVertices**(`pa`, `pb`, `p0`, `p1`, `p2`): `number`

#### Parameters

| Name | Type |
| :------ | :------ |
| `pa` | [`Vector3`](Vector3.md) |
| `pb` | [`Vector3`](Vector3.md) |
| `p0` | [`Vector3`](Vector3.md) |
| `p1` | [`Vector3`](Vector3.md) |
| `p2` | [`Vector3`](Vector3.md) |

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:375

___

### \_tessellateTriangle

▸ `Private` **_tessellateTriangle**(`edgePoints`, `indexTriangle`, `indices`, `remapVertexIndices`): `void`

See https://playground.babylonjs.com/#R3JR6V#1 for a visual display of the algorithm

#### Parameters

| Name | Type |
| :------ | :------ |
| `edgePoints` | [`number`, `number`][][] |
| `indexTriangle` | `number` |
| `indices` | `number`[] |
| `remapVertexIndices` | `number`[] |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:443

___

### createLine

▸ `Protected` **createLine**(`p0`, `p1`, `offset`): `void`

push line into the position, normal and index buffer

#### Parameters

| Name | Type |
| :------ | :------ |
| `p0` | [`Vector3`](Vector3.md) |
| `p1` | [`Vector3`](Vector3.md) |
| `offset` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:425

___

### dispose

▸ **dispose**(): `void`

Releases the required resources for the edges renderer

#### Returns

`void`

#### Implementation of

[IEdgesRenderer](../interfaces/IEdgesRenderer.md).[dispose](../interfaces/IEdgesRenderer.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:336

___

### isReady

▸ **isReady**(): `boolean`

Checks whether or not the edges renderer is ready to render.

#### Returns

`boolean`

true if ready, otherwise false.

#### Implementation of

[IEdgesRenderer](../interfaces/IEdgesRenderer.md).[isReady](../interfaces/IEdgesRenderer.md#isready)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:917

___

### render

▸ **render**(): `void`

Renders the edges of the attached mesh,

#### Returns

`void`

#### Implementation of

[IEdgesRenderer](../interfaces/IEdgesRenderer.md).[render](../interfaces/IEdgesRenderer.md#render)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:924

___

### \_GetShader

▸ `Static` `Private` **_GetShader**(`scene`): [`ShaderMaterial`](ShaderMaterial.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `scene` | [`Scene`](Scene.md) |

#### Returns

[`ShaderMaterial`](ShaderMaterial.md)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:248
