[@dev/core](../README.md) / [Exports](../modules.md) / LineEdgesRenderer

# Class: LineEdgesRenderer

LineEdgesRenderer for LineMeshes to remove unnecessary triangulation

## Hierarchy

- [`EdgesRenderer`](EdgesRenderer.md)

  ↳ **`LineEdgesRenderer`**

## Table of contents

### Constructors

- [constructor](LineEdgesRenderer.md#constructor)

### Properties

- [\_buffers](LineEdgesRenderer.md#_buffers)
- [\_buffersForInstances](LineEdgesRenderer.md#_buffersforinstances)
- [\_checkVerticesInsteadOfIndices](LineEdgesRenderer.md#_checkverticesinsteadofindices)
- [\_drawWrapper](LineEdgesRenderer.md#_drawwrapper)
- [\_epsilon](LineEdgesRenderer.md#_epsilon)
- [\_ib](LineEdgesRenderer.md#_ib)
- [\_indicesCount](LineEdgesRenderer.md#_indicescount)
- [\_lineShader](LineEdgesRenderer.md#_lineshader)
- [\_linesIndices](LineEdgesRenderer.md#_linesindices)
- [\_linesNormals](LineEdgesRenderer.md#_linesnormals)
- [\_linesPositions](LineEdgesRenderer.md#_linespositions)
- [\_options](LineEdgesRenderer.md#_options)
- [\_source](LineEdgesRenderer.md#_source)
- [customInstances](LineEdgesRenderer.md#custominstances)
- [edgesWidthScalerForOrthographic](LineEdgesRenderer.md#edgeswidthscalerfororthographic)
- [edgesWidthScalerForPerspective](LineEdgesRenderer.md#edgeswidthscalerforperspective)
- [isEnabled](LineEdgesRenderer.md#isenabled)

### Accessors

- [lineShader](LineEdgesRenderer.md#lineshader)
- [linesIndices](LineEdgesRenderer.md#linesindices)
- [linesNormals](LineEdgesRenderer.md#linesnormals)
- [linesPositions](LineEdgesRenderer.md#linespositions)

### Methods

- [\_checkEdge](LineEdgesRenderer.md#_checkedge)
- [\_generateEdgesLines](LineEdgesRenderer.md#_generateedgeslines)
- [\_prepareRessources](LineEdgesRenderer.md#_prepareressources)
- [\_processEdgeForAdjacencies](LineEdgesRenderer.md#_processedgeforadjacencies)
- [\_processEdgeForAdjacenciesWithVertices](LineEdgesRenderer.md#_processedgeforadjacencieswithvertices)
- [createLine](LineEdgesRenderer.md#createline)
- [dispose](LineEdgesRenderer.md#dispose)
- [isReady](LineEdgesRenderer.md#isready)
- [render](LineEdgesRenderer.md#render)

## Constructors

### constructor

• **new LineEdgesRenderer**(`source`, `epsilon?`, `checkVerticesInsteadOfIndices?`)

This constructor turns off auto generating edges line in Edges Renderer to make it here.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `source` | [`AbstractMesh`](AbstractMesh.md) | `undefined` | LineMesh used to generate edges |
| `epsilon` | `number` | `0.95` | not important (specified angle for edge detection) |
| `checkVerticesInsteadOfIndices` | `boolean` | `false` | not important for LineMesh |

#### Overrides

[EdgesRenderer](EdgesRenderer.md).[constructor](EdgesRenderer.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:1025

## Properties

### \_buffers

• `Protected` **\_buffers**: `Object` = `{}`

#### Index signature

▪ [key: `string`]: [`Nullable`](../modules.md#nullable)[`VertexBuffer`](VertexBuffer.md)

#### Inherited from

[EdgesRenderer](EdgesRenderer.md).[_buffers](EdgesRenderer.md#_buffers)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:206

___

### \_buffersForInstances

• `Protected` **\_buffersForInstances**: `Object` = `{}`

#### Index signature

▪ [key: `string`]: [`Nullable`](../modules.md#nullable)[`VertexBuffer`](VertexBuffer.md)

#### Inherited from

[EdgesRenderer](EdgesRenderer.md).[_buffersForInstances](EdgesRenderer.md#_buffersforinstances)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:207

___

### \_checkVerticesInsteadOfIndices

• `Protected` **\_checkVerticesInsteadOfIndices**: `boolean` = `false`

#### Inherited from

[EdgesRenderer](EdgesRenderer.md).[_checkVerticesInsteadOfIndices](EdgesRenderer.md#_checkverticesinsteadofindices)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:208

___

### \_drawWrapper

• `Protected` `Optional` **\_drawWrapper**: `DrawWrapper`

#### Inherited from

[EdgesRenderer](EdgesRenderer.md).[_drawWrapper](EdgesRenderer.md#_drawwrapper)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:202

___

### \_epsilon

• `Protected` **\_epsilon**: `number`

#### Inherited from

[EdgesRenderer](EdgesRenderer.md).[_epsilon](EdgesRenderer.md#_epsilon)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:200

___

### \_ib

• `Protected` **\_ib**: [`DataBuffer`](DataBuffer.md)

#### Inherited from

[EdgesRenderer](EdgesRenderer.md).[_ib](EdgesRenderer.md#_ib)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:205

___

### \_indicesCount

• `Protected` **\_indicesCount**: `number`

#### Inherited from

[EdgesRenderer](EdgesRenderer.md).[_indicesCount](EdgesRenderer.md#_indicescount)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:201

___

### \_lineShader

• `Protected` **\_lineShader**: [`ShaderMaterial`](ShaderMaterial.md)

#### Inherited from

[EdgesRenderer](EdgesRenderer.md).[_lineShader](EdgesRenderer.md#_lineshader)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:204

___

### \_linesIndices

• `Protected` **\_linesIndices**: `number`[]

#### Inherited from

[EdgesRenderer](EdgesRenderer.md).[_linesIndices](EdgesRenderer.md#_linesindices)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:199

___

### \_linesNormals

• `Protected` **\_linesNormals**: `number`[]

#### Inherited from

[EdgesRenderer](EdgesRenderer.md).[_linesNormals](EdgesRenderer.md#_linesnormals)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:198

___

### \_linesPositions

• `Protected` **\_linesPositions**: `number`[]

#### Inherited from

[EdgesRenderer](EdgesRenderer.md).[_linesPositions](EdgesRenderer.md#_linespositions)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:197

___

### \_options

• `Protected` **\_options**: [`Nullable`](../modules.md#nullable)[`IEdgesRendererOptions`](../interfaces/IEdgesRendererOptions.md)

#### Inherited from

[EdgesRenderer](EdgesRenderer.md).[_options](EdgesRenderer.md#_options)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:209

___

### \_source

• `Protected` **\_source**: [`AbstractMesh`](AbstractMesh.md)

#### Inherited from

[EdgesRenderer](EdgesRenderer.md).[_source](EdgesRenderer.md#_source)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:196

___

### customInstances

• **customInstances**: [`SmartArray`](SmartArray.md)[`Matrix`](Matrix.md)

List of instances to render in case the source mesh has instances

#### Inherited from

[EdgesRenderer](EdgesRenderer.md).[customInstances](EdgesRenderer.md#custominstances)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:246

___

### edgesWidthScalerForOrthographic

• **edgesWidthScalerForOrthographic**: `number` = `1000.0`

Define the size of the edges with an orthographic camera

#### Inherited from

[EdgesRenderer](EdgesRenderer.md).[edgesWidthScalerForOrthographic](EdgesRenderer.md#edgeswidthscalerfororthographic)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:189

___

### edgesWidthScalerForPerspective

• **edgesWidthScalerForPerspective**: `number` = `50.0`

Define the size of the edges with a perspective camera

#### Inherited from

[EdgesRenderer](EdgesRenderer.md).[edgesWidthScalerForPerspective](EdgesRenderer.md#edgeswidthscalerforperspective)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:194

___

### isEnabled

• **isEnabled**: `boolean` = `true`

Gets or sets a boolean indicating if the edgesRenderer is active

#### Inherited from

[EdgesRenderer](EdgesRenderer.md).[isEnabled](EdgesRenderer.md#isenabled)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:215

## Accessors

### lineShader

• `get` **lineShader**(): [`ShaderMaterial`](ShaderMaterial.md)

Gets or sets the shader used to draw the lines

#### Returns

[`ShaderMaterial`](ShaderMaterial.md)

#### Inherited from

EdgesRenderer.lineShader

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:235

• `set` **lineShader**(`shader`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `shader` | [`ShaderMaterial`](ShaderMaterial.md) |

#### Returns

`void`

#### Inherited from

EdgesRenderer.lineShader

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:239

___

### linesIndices

• `get` **linesIndices**(): readonly `number`[]

Gets the indices generated by the edge renderer

#### Returns

readonly `number`[]

#### Inherited from

EdgesRenderer.linesIndices

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:228

___

### linesNormals

• `get` **linesNormals**(): readonly `number`[]

Gets the normals generated by the edge renderer

#### Returns

readonly `number`[]

#### Inherited from

EdgesRenderer.linesNormals

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:223

___

### linesPositions

• `get` **linesPositions**(): readonly `number`[]

Gets the vertices generated by the edge renderer

#### Returns

readonly `number`[]

#### Inherited from

EdgesRenderer.linesPositions

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

#### Inherited from

[EdgesRenderer](EdgesRenderer.md).[_checkEdge](EdgesRenderer.md#_checkedge)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:401

___

### \_generateEdgesLines

▸ **_generateEdgesLines**(): `void`

Generate edges for each line in LinesMesh. Every Line should be rendered as edge.

#### Returns

`void`

#### Overrides

[EdgesRenderer](EdgesRenderer.md).[_generateEdgesLines](EdgesRenderer.md#_generateedgeslines)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:1033

___

### \_prepareRessources

▸ `Protected` **_prepareRessources**(): `void`

#### Returns

`void`

#### Inherited from

[EdgesRenderer](EdgesRenderer.md).[_prepareRessources](EdgesRenderer.md#_prepareressources)

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

#### Inherited from

[EdgesRenderer](EdgesRenderer.md).[_processEdgeForAdjacencies](EdgesRenderer.md#_processedgeforadjacencies)

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

#### Inherited from

[EdgesRenderer](EdgesRenderer.md).[_processEdgeForAdjacenciesWithVertices](EdgesRenderer.md#_processedgeforadjacencieswithvertices)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:375

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

#### Inherited from

[EdgesRenderer](EdgesRenderer.md).[createLine](EdgesRenderer.md#createline)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:425

___

### dispose

▸ **dispose**(): `void`

Releases the required resources for the edges renderer

#### Returns

`void`

#### Inherited from

[EdgesRenderer](EdgesRenderer.md).[dispose](EdgesRenderer.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:336

___

### isReady

▸ **isReady**(): `boolean`

Checks whether or not the edges renderer is ready to render.

#### Returns

`boolean`

true if ready, otherwise false.

#### Inherited from

[EdgesRenderer](EdgesRenderer.md).[isReady](EdgesRenderer.md#isready)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:917

___

### render

▸ **render**(): `void`

Renders the edges of the attached mesh,

#### Returns

`void`

#### Inherited from

[EdgesRenderer](EdgesRenderer.md).[render](EdgesRenderer.md#render)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:924
