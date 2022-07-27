[@dev/core](../README.md) / [Exports](../modules.md) / BoundingBoxRenderer

# Class: BoundingBoxRenderer

Component responsible of rendering the bounding box of the meshes in a scene.
This is usually used through the mesh.showBoundingBox or the scene.forceShowBoundingBoxes properties

## Implements

- [`ISceneComponent`](../interfaces/ISceneComponent.md)

## Table of contents

### Constructors

- [constructor](BoundingBoxRenderer.md#constructor)

### Properties

- [\_colorShader](BoundingBoxRenderer.md#_colorshader)
- [\_colorShaderForOcclusionQuery](BoundingBoxRenderer.md#_colorshaderforocclusionquery)
- [\_fillIndexBuffer](BoundingBoxRenderer.md#_fillindexbuffer)
- [\_fillIndexData](BoundingBoxRenderer.md#_fillindexdata)
- [\_indexBuffer](BoundingBoxRenderer.md#_indexbuffer)
- [\_renderPassIdForOcclusionQuery](BoundingBoxRenderer.md#_renderpassidforocclusionquery)
- [\_uniformBufferBack](BoundingBoxRenderer.md#_uniformbufferback)
- [\_uniformBufferFront](BoundingBoxRenderer.md#_uniformbufferfront)
- [\_vertexBuffers](BoundingBoxRenderer.md#_vertexbuffers)
- [backColor](BoundingBoxRenderer.md#backcolor)
- [enabled](BoundingBoxRenderer.md#enabled)
- [frontColor](BoundingBoxRenderer.md#frontcolor)
- [name](BoundingBoxRenderer.md#name)
- [onAfterBoxRenderingObservable](BoundingBoxRenderer.md#onafterboxrenderingobservable)
- [onBeforeBoxRenderingObservable](BoundingBoxRenderer.md#onbeforeboxrenderingobservable)
- [onResourcesReadyObservable](BoundingBoxRenderer.md#onresourcesreadyobservable)
- [scene](BoundingBoxRenderer.md#scene)
- [showBackLines](BoundingBoxRenderer.md#showbacklines)

### Methods

- [\_buildUniformLayout](BoundingBoxRenderer.md#_builduniformlayout)
- [\_createIndexBuffer](BoundingBoxRenderer.md#_createindexbuffer)
- [\_createWrappersForBoundingBox](BoundingBoxRenderer.md#_createwrappersforboundingbox)
- [\_evaluateSubMesh](BoundingBoxRenderer.md#_evaluatesubmesh)
- [\_preActiveMesh](BoundingBoxRenderer.md#_preactivemesh)
- [\_prepareResources](BoundingBoxRenderer.md#_prepareresources)
- [dispose](BoundingBoxRenderer.md#dispose)
- [rebuild](BoundingBoxRenderer.md#rebuild)
- [register](BoundingBoxRenderer.md#register)
- [render](BoundingBoxRenderer.md#render)
- [renderOcclusionBoundingBox](BoundingBoxRenderer.md#renderocclusionboundingbox)

## Constructors

### constructor

• **new BoundingBoxRenderer**(`scene`)

Instantiates a new bounding box renderer in a scene.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | the scene the  renderer renders in |

#### Defined in

packages/dev/core/src/Rendering/boundingBoxRenderer.ts:162

## Properties

### \_colorShader

• `Private` **\_colorShader**: [`ShaderMaterial`](ShaderMaterial.md)

#### Defined in

packages/dev/core/src/Rendering/boundingBoxRenderer.ts:148

___

### \_colorShaderForOcclusionQuery

• `Private` **\_colorShaderForOcclusionQuery**: [`ShaderMaterial`](ShaderMaterial.md)

#### Defined in

packages/dev/core/src/Rendering/boundingBoxRenderer.ts:149

___

### \_fillIndexBuffer

• `Private` **\_fillIndexBuffer**: [`Nullable`](../modules.md#nullable)[`DataBuffer`](DataBuffer.md) = `null`

#### Defined in

packages/dev/core/src/Rendering/boundingBoxRenderer.ts:152

___

### \_fillIndexData

• `Private` **\_fillIndexData**: [`Nullable`](../modules.md#nullable)[`IndicesArray`](../modules.md#indicesarray) = `null`

#### Defined in

packages/dev/core/src/Rendering/boundingBoxRenderer.ts:153

___

### \_indexBuffer

• `Private` **\_indexBuffer**: [`DataBuffer`](DataBuffer.md)

#### Defined in

packages/dev/core/src/Rendering/boundingBoxRenderer.ts:151

___

### \_renderPassIdForOcclusionQuery

• `Private` **\_renderPassIdForOcclusionQuery**: `number`

#### Defined in

packages/dev/core/src/Rendering/boundingBoxRenderer.ts:156

___

### \_uniformBufferBack

• `Private` **\_uniformBufferBack**: [`UniformBuffer`](UniformBuffer.md)

#### Defined in

packages/dev/core/src/Rendering/boundingBoxRenderer.ts:155

___

### \_uniformBufferFront

• `Private` **\_uniformBufferFront**: [`UniformBuffer`](UniformBuffer.md)

#### Defined in

packages/dev/core/src/Rendering/boundingBoxRenderer.ts:154

___

### \_vertexBuffers

• `Private` **\_vertexBuffers**: `Object` = `{}`

#### Index signature

▪ [key: `string`]: [`Nullable`](../modules.md#nullable)[`VertexBuffer`](VertexBuffer.md)

#### Defined in

packages/dev/core/src/Rendering/boundingBoxRenderer.ts:150

___

### backColor

• **backColor**: [`Color3`](Color3.md)

Color of the bounding box lines placed behind an object

#### Defined in

packages/dev/core/src/Rendering/boundingBoxRenderer.ts:117

___

### enabled

• **enabled**: `boolean` = `true`

When false, no bounding boxes will be rendered

#### Defined in

packages/dev/core/src/Rendering/boundingBoxRenderer.ts:141

___

### frontColor

• **frontColor**: [`Color3`](Color3.md)

Color of the bounding box lines placed in front of an object

#### Defined in

packages/dev/core/src/Rendering/boundingBoxRenderer.ts:113

___

### name

• `Readonly` **name**: ``"BoundingBoxRenderer"``

The component name helpful to identify the component in the list of scene components.

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[name](../interfaces/ISceneComponent.md#name)

#### Defined in

packages/dev/core/src/Rendering/boundingBoxRenderer.ts:103

___

### onAfterBoxRenderingObservable

• **onAfterBoxRenderingObservable**: [`Observable`](Observable.md)[`BoundingBox`](BoundingBox.md)

Observable raised after rendering a bounding box

#### Defined in

packages/dev/core/src/Rendering/boundingBoxRenderer.ts:131

___

### onBeforeBoxRenderingObservable

• **onBeforeBoxRenderingObservable**: [`Observable`](Observable.md)[`BoundingBox`](BoundingBox.md)

Observable raised before rendering a bounding box

#### Defined in

packages/dev/core/src/Rendering/boundingBoxRenderer.ts:126

___

### onResourcesReadyObservable

• **onResourcesReadyObservable**: [`Observable`](Observable.md)[`BoundingBoxRenderer`](BoundingBoxRenderer.md)

Observable raised after resources are created

#### Defined in

packages/dev/core/src/Rendering/boundingBoxRenderer.ts:136

___

### scene

• **scene**: [`Scene`](Scene.md)

The scene the component belongs to.

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[scene](../interfaces/ISceneComponent.md#scene)

#### Defined in

packages/dev/core/src/Rendering/boundingBoxRenderer.ts:108

___

### showBackLines

• **showBackLines**: `boolean` = `true`

Defines if the renderer should show the back lines or not

#### Defined in

packages/dev/core/src/Rendering/boundingBoxRenderer.ts:121

## Methods

### \_buildUniformLayout

▸ `Private` **_buildUniformLayout**(`ubo`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `ubo` | [`UniformBuffer`](UniformBuffer.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Rendering/boundingBoxRenderer.ts:171

___

### \_createIndexBuffer

▸ `Private` **_createIndexBuffer**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Rendering/boundingBoxRenderer.ts:255

___

### \_createWrappersForBoundingBox

▸ `Private` **_createWrappersForBoundingBox**(`boundingBox`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `boundingBox` | [`BoundingBox`](BoundingBox.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Rendering/boundingBoxRenderer.ts:370

___

### \_evaluateSubMesh

▸ `Private` **_evaluateSubMesh**(`mesh`, `subMesh`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) |
| `subMesh` | [`SubMesh`](SubMesh.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Rendering/boundingBoxRenderer.ts:192

___

### \_preActiveMesh

▸ `Private` **_preActiveMesh**(`mesh`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Rendering/boundingBoxRenderer.ts:202

___

### \_prepareResources

▸ `Private` **_prepareResources**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Rendering/boundingBoxRenderer.ts:210

___

### dispose

▸ **dispose**(): `void`

Dispose and release the resources attached to this renderer.

#### Returns

`void`

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[dispose](../interfaces/ISceneComponent.md#dispose)

#### Defined in

packages/dev/core/src/Rendering/boundingBoxRenderer.ts:455

___

### rebuild

▸ **rebuild**(): `void`

Rebuilds the elements related to this component in case of
context lost for instance.

#### Returns

`void`

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[rebuild](../interfaces/ISceneComponent.md#rebuild)

#### Defined in

packages/dev/core/src/Rendering/boundingBoxRenderer.ts:264

___

### register

▸ **register**(): `void`

Registers the component in a given scene

#### Returns

`void`

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[register](../interfaces/ISceneComponent.md#register)

#### Defined in

packages/dev/core/src/Rendering/boundingBoxRenderer.ts:182

___

### render

▸ **render**(`renderingGroupId`): `void`

Render the bounding boxes of a specific rendering group

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `renderingGroupId` | `number` | defines the rendering group to render |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Rendering/boundingBoxRenderer.ts:283

___

### renderOcclusionBoundingBox

▸ **renderOcclusionBoundingBox**(`mesh`): `void`

In case of occlusion queries, we can render the occlusion bounding box through this method

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | Define the mesh to render the occlusion bounding box for |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Rendering/boundingBoxRenderer.ts:386
