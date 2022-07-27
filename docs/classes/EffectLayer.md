[@dev/core](../README.md) / [Exports](../modules.md) / EffectLayer

# Class: EffectLayer

The effect layer Helps adding post process effect blended with the main pass.

This can be for instance use to generate glow or highlight effects on the scene.

The effect layer class can not be used directly and is intented to inherited from to be
customized per effects.

## Hierarchy

- **`EffectLayer`**

  ↳ [`GlowLayer`](GlowLayer.md)

  ↳ [`HighlightLayer`](HighlightLayer.md)

## Table of contents

### Constructors

- [constructor](EffectLayer.md#constructor)

### Properties

- [\_effectLayerOptions](EffectLayer.md#_effectlayeroptions)
- [\_emissiveTextureAndColor](EffectLayer.md#_emissivetextureandcolor)
- [\_engine](EffectLayer.md#_engine)
- [\_indexBuffer](EffectLayer.md#_indexbuffer)
- [\_mainTexture](EffectLayer.md#_maintexture)
- [\_mainTextureDesiredSize](EffectLayer.md#_maintexturedesiredsize)
- [\_materialForRendering](EffectLayer.md#_materialforrendering)
- [\_maxSize](EffectLayer.md#_maxsize)
- [\_mergeDrawWrapper](EffectLayer.md#_mergedrawwrapper)
- [\_postProcesses](EffectLayer.md#_postprocesses)
- [\_scene](EffectLayer.md#_scene)
- [\_shouldRender](EffectLayer.md#_shouldrender)
- [\_textures](EffectLayer.md#_textures)
- [\_vertexBuffers](EffectLayer.md#_vertexbuffers)
- [disableBoundingBoxesFromEffectLayer](EffectLayer.md#disableboundingboxesfromeffectlayer)
- [isEnabled](EffectLayer.md#isenabled)
- [name](EffectLayer.md#name)
- [neutralColor](EffectLayer.md#neutralcolor)
- [onAfterComposeObservable](EffectLayer.md#onaftercomposeobservable)
- [onAfterRenderMeshToEffect](EffectLayer.md#onafterrendermeshtoeffect)
- [onBeforeComposeObservable](EffectLayer.md#onbeforecomposeobservable)
- [onBeforeRenderMainTextureObservable](EffectLayer.md#onbeforerendermaintextureobservable)
- [onBeforeRenderMeshToEffect](EffectLayer.md#onbeforerendermeshtoeffect)
- [onDisposeObservable](EffectLayer.md#ondisposeobservable)
- [onSizeChangedObservable](EffectLayer.md#onsizechangedobservable)

### Accessors

- [camera](EffectLayer.md#camera)
- [mainTexture](EffectLayer.md#maintexture)
- [renderingGroupId](EffectLayer.md#renderinggroupid)

### Methods

- [\_addCustomEffectDefines](EffectLayer.md#_addcustomeffectdefines)
- [\_canRenderMesh](EffectLayer.md#_canrendermesh)
- [\_createMainTexture](EffectLayer.md#_createmaintexture)
- [\_createMergeEffect](EffectLayer.md#_createmergeeffect)
- [\_createTextureAndPostProcesses](EffectLayer.md#_createtextureandpostprocesses)
- [\_disposeMesh](EffectLayer.md#_disposemesh)
- [\_disposeTextureAndPostProcesses](EffectLayer.md#_disposetextureandpostprocesses)
- [\_generateIndexBuffer](EffectLayer.md#_generateindexbuffer)
- [\_generateVertexBuffer](EffectLayer.md#_generatevertexbuffer)
- [\_init](EffectLayer.md#_init)
- [\_internalRender](EffectLayer.md#_internalrender)
- [\_isReady](EffectLayer.md#_isready)
- [\_numInternalDraws](EffectLayer.md#_numinternaldraws)
- [\_renderSubMesh](EffectLayer.md#_rendersubmesh)
- [\_setEmissiveTextureAndColor](EffectLayer.md#_setemissivetextureandcolor)
- [\_setMainTextureSize](EffectLayer.md#_setmaintexturesize)
- [\_shouldRenderEmissiveTextureForMesh](EffectLayer.md#_shouldrenderemissivetextureformesh)
- [\_shouldRenderMesh](EffectLayer.md#_shouldrendermesh)
- [\_useMeshMaterial](EffectLayer.md#_usemeshmaterial)
- [dispose](EffectLayer.md#dispose)
- [getClassName](EffectLayer.md#getclassname)
- [getEffectName](EffectLayer.md#geteffectname)
- [hasMesh](EffectLayer.md#hasmesh)
- [isReady](EffectLayer.md#isready)
- [needStencil](EffectLayer.md#needstencil)
- [render](EffectLayer.md#render)
- [serialize](EffectLayer.md#serialize)
- [setMaterialForRendering](EffectLayer.md#setmaterialforrendering)
- [shouldRender](EffectLayer.md#shouldrender)
- [Parse](EffectLayer.md#parse)

## Constructors

### constructor

• **new EffectLayer**(`name`, `scene?`)

Instantiates a new effect Layer and references it in the scene.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | The name of the layer |
| `scene?` | [`Scene`](Scene.md) | The scene to use the layer in |

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:213

## Properties

### \_effectLayerOptions

• `Private` **\_effectLayerOptions**: [`IEffectLayerOptions`](../interfaces/IEffectLayerOptions.md)

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:75

___

### \_emissiveTextureAndColor

• `Protected` **\_emissiveTextureAndColor**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `color` | [`Color4`](Color4.md) |
| `texture` | [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) |

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:86

___

### \_engine

• `Protected` **\_engine**: [`Engine`](Engine.md)

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:79

___

### \_indexBuffer

• `Private` **\_indexBuffer**: [`Nullable`](../modules.md#nullable)[`DataBuffer`](DataBuffer.md)

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:74

___

### \_mainTexture

• `Protected` **\_mainTexture**: [`RenderTargetTexture`](RenderTargetTexture.md)

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:82

___

### \_mainTextureDesiredSize

• `Protected` **\_mainTextureDesiredSize**: [`ISize`](../interfaces/ISize.md)

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:81

___

### \_materialForRendering

• `Private` **\_materialForRendering**: `Object` = `{}`

#### Index signature

▪ [id: `string`]: [[`AbstractMesh`](AbstractMesh.md), [`Material`](Material.md)]

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:181

___

### \_maxSize

• `Protected` **\_maxSize**: `number` = `0`

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:80

___

### \_mergeDrawWrapper

• `Private` **\_mergeDrawWrapper**: `DrawWrapper`[]

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:76

___

### \_postProcesses

• `Protected` **\_postProcesses**: [`PostProcess`](PostProcess.md)[] = `[]`

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:84

___

### \_scene

• `Protected` **\_scene**: [`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:78

___

### \_shouldRender

• `Protected` **\_shouldRender**: `boolean` = `true`

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:83

___

### \_textures

• `Protected` **\_textures**: [`BaseTexture`](BaseTexture.md)[] = `[]`

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:85

___

### \_vertexBuffers

• `Private` **\_vertexBuffers**: `Object` = `{}`

#### Index signature

▪ [key: `string`]: [`Nullable`](../modules.md#nullable)[`VertexBuffer`](VertexBuffer.md)

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:73

___

### disableBoundingBoxesFromEffectLayer

• **disableBoundingBoxesFromEffectLayer**: `boolean` = `false`

Specifies if the bounding boxes should be rendered normally or if they should undergo the effect of the layer

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:129

___

### isEnabled

• **isEnabled**: `boolean` = `true`

Specifies whether the highlight layer is enabled or not.

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:104

___

### name

• **name**: `string`

The name of the layer

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:92

___

### neutralColor

• **neutralColor**: [`Color4`](Color4.md)

The clear color of the texture used to generate the glow map.

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:98

___

### onAfterComposeObservable

• **onAfterComposeObservable**: [`Observable`](Observable.md)[`EffectLayer`](EffectLayer.md)

An event triggered when the generated texture has been merged in the scene.

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:159

___

### onAfterRenderMeshToEffect

• **onAfterRenderMeshToEffect**: [`Observable`](Observable.md)[`AbstractMesh`](AbstractMesh.md)

An event triggered after the mesh has been rendered into the effect render target.

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:154

___

### onBeforeComposeObservable

• **onBeforeComposeObservable**: [`Observable`](Observable.md)[`EffectLayer`](EffectLayer.md)

An event triggered when the generated texture is being merged in the scene.

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:144

___

### onBeforeRenderMainTextureObservable

• **onBeforeRenderMainTextureObservable**: [`Observable`](Observable.md)[`EffectLayer`](EffectLayer.md)

An event triggered when the effect layer is about rendering the main texture with the glowy parts.

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:139

___

### onBeforeRenderMeshToEffect

• **onBeforeRenderMeshToEffect**: [`Observable`](Observable.md)[`AbstractMesh`](AbstractMesh.md)

An event triggered when the mesh is rendered into the effect render target.

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:149

___

### onDisposeObservable

• **onDisposeObservable**: [`Observable`](Observable.md)[`EffectLayer`](EffectLayer.md)

An event triggered when the effect layer has been disposed.

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:134

___

### onSizeChangedObservable

• **onSizeChangedObservable**: [`Observable`](Observable.md)[`EffectLayer`](EffectLayer.md)

An event triggered when the effect layer changes its size.

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:164

## Accessors

### camera

• `get` **camera**(): [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md)

Gets the camera attached to the layer.

#### Returns

[`Nullable`](../modules.md#nullable)[`Camera`](Camera.md)

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:109

___

### mainTexture

• `get` **mainTexture**(): [`RenderTargetTexture`](RenderTargetTexture.md)

Gets the main texture where the effect is rendered

#### Returns

[`RenderTargetTexture`](RenderTargetTexture.md)

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:169

___

### renderingGroupId

• `get` **renderingGroupId**(): `number`

Gets the rendering group id the layer should render in.

#### Returns

`number`

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:117

• `set` **renderingGroupId**(`renderingGroupId`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `renderingGroupId` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:121

## Methods

### \_addCustomEffectDefines

▸ `Protected` **_addCustomEffectDefines**(`defines`): `void`

Adds specific effects defines.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `defines` | `string`[] | The defines to add specifics to. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:493

___

### \_canRenderMesh

▸ `Protected` **_canRenderMesh**(`mesh`, `material`): `boolean`

Returns true if the mesh can be rendered, otherwise false.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | The mesh to render |
| `material` | [`Material`](Material.md) | The material used on the mesh |

#### Returns

`boolean`

true if it can be rendered otherwise false

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:796

___

### \_createMainTexture

▸ `Protected` **_createMainTexture**(): `void`

Creates the main texture for the effect layer.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:377

___

### \_createMergeEffect

▸ `Protected` `Abstract` **_createMergeEffect**(): [`Effect`](Effect.md)

Create the merge effect. This is the shader use to blit the information back
to the main canvas at the end of the scene rendering.

#### Returns

[`Effect`](Effect.md)

The effect containing the shader used to merge the effect on the  main canvas

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:259

___

### \_createTextureAndPostProcesses

▸ `Protected` `Abstract` **_createTextureAndPostProcesses**(): `void`

Creates the render target textures and post processes used in the effect layer.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:264

___

### \_disposeMesh

▸ `Abstract` **_disposeMesh**(`mesh`): `void`

Free any resources and references associated to a mesh.
Internal use

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`Mesh`](Mesh.md) | The mesh to free. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:283

___

### \_disposeTextureAndPostProcesses

▸ `Private` **_disposeTextureAndPostProcesses**(): `void`

Dispose only the render target textures and post process.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:999

___

### \_generateIndexBuffer

▸ `Private` **_generateIndexBuffer**(): `void`

Generates the index buffer of the full screen quad blending to the main canvas.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:321

___

### \_generateVertexBuffer

▸ `Private` **_generateVertexBuffer**(): `void`

Generates the vertex buffer of the full screen quad blending to the main canvas.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:338

___

### \_init

▸ `Protected` **_init**(`options`): `void`

Initializes the effect layer with the required options.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | `Partial`[`IEffectLayerOptions`](../interfaces/IEffectLayerOptions.md) | Sets of none mandatory options to use with the layer (see IEffectLayerOptions for more information) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:303

___

### \_internalRender

▸ `Protected` `Abstract` **_internalRender**(`effect`, `renderIndex`): `void`

Implementation specific of rendering the generating effect on the main canvas.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `effect` | [`Effect`](Effect.md) | The effect used to render through |
| `renderIndex` | `number` | - |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:271

___

### \_isReady

▸ `Protected` **_isReady**(`subMesh`, `useInstances`, `emissiveTexture`): `boolean`

Checks for the readiness of the element composing the layer.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `subMesh` | [`SubMesh`](SubMesh.md) | the mesh to check for |
| `useInstances` | `boolean` | specify whether or not to use instances to render the mesh |
| `emissiveTexture` | [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) | the associated emissive texture used to generate the glow |

#### Returns

`boolean`

true if ready otherwise, false

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:504

___

### \_numInternalDraws

▸ `Protected` **_numInternalDraws**(): `number`

Number of times _internalRender will be called. Some effect layers need to render the mesh several times, so they should override this method with the number of times the mesh should be rendered

#### Returns

`number`

Number of times a mesh must be rendered in the layer

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:295

___

### \_renderSubMesh

▸ `Protected` **_renderSubMesh**(`subMesh`, `enableAlphaMode?`): `void`

Renders the submesh passed in parameter to the generation map.

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `subMesh` | [`SubMesh`](SubMesh.md) | `undefined` |
| `enableAlphaMode` | `boolean` | `false` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:813

___

### \_setEmissiveTextureAndColor

▸ `Protected` `Abstract` **_setEmissiveTextureAndColor**(`mesh`, `subMesh`, `material`): `void`

Sets the required values for both the emissive texture and and the main color.

#### Parameters

| Name | Type |
| :------ | :------ |
| `mesh` | [`Mesh`](Mesh.md) |
| `subMesh` | [`SubMesh`](SubMesh.md) |
| `material` | [`Material`](Material.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:276

___

### \_setMainTextureSize

▸ `Private` **_setMainTextureSize**(): `void`

Sets the main texture desired size which is the closest power of two
of the engine canvas size.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:354

___

### \_shouldRenderEmissiveTextureForMesh

▸ `Protected` **_shouldRenderEmissiveTextureForMesh**(): `boolean`

Returns true if the mesh should render, otherwise false.

#### Returns

`boolean`

true if it should render otherwise false

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:804

___

### \_shouldRenderMesh

▸ `Protected` **_shouldRenderMesh**(`mesh`): `boolean`

Returns true if the mesh should render, otherwise false.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | The mesh to render |

#### Returns

`boolean`

true if it should render otherwise false

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:786

___

### \_useMeshMaterial

▸ `Protected` **_useMeshMaterial**(`mesh`): `boolean`

Defines whether the current material of the mesh should be use to render the effect.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | defines the current mesh to render |

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:978

___

### dispose

▸ **dispose**(): `void`

Dispose the highlight layer and free resources.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:1020

___

### getClassName

▸ **getClassName**(): `string`

Gets the class name of the effect layer

#### Returns

`string`

the string with the class name of the effect layer

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:1062

___

### getEffectName

▸ `Abstract` **getEffectName**(): `string`

Get the effect name of the layer.

#### Returns

`string`

The effect name

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:238

___

### hasMesh

▸ **hasMesh**(`mesh`): `boolean`

Determine if a given mesh will be used in the current effect.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | mesh to test |

#### Returns

`boolean`

true if the mesh will be used

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:765

___

### isReady

▸ `Abstract` **isReady**(`subMesh`, `useInstances`): `boolean`

Checks for the readiness of the element composing the layer.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `subMesh` | [`SubMesh`](SubMesh.md) | the mesh to check for |
| `useInstances` | `boolean` | specify whether or not to use instances to render the mesh |

#### Returns

`boolean`

true if ready otherwise, false

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:246

___

### needStencil

▸ `Abstract` **needStencil**(): `boolean`

Returns whether or not the layer needs stencil enabled during the mesh rendering.

#### Returns

`boolean`

true if the effect requires stencil during the main canvas render pass.

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:252

___

### render

▸ **render**(): `void`

Renders the glowing part of the scene by blending the blurred glowing meshes on top of the rendered scene.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:693

___

### serialize

▸ `Optional` `Abstract` **serialize**(): `any`

Serializes this layer (Glow or Highlight for example)

#### Returns

`any`

a serialized layer object

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:289

___

### setMaterialForRendering

▸ **setMaterialForRendering**(`mesh`, `material?`): `void`

Sets a specific material to be used to render a mesh/a list of meshes in the layer

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) \| [`AbstractMesh`](AbstractMesh.md)[] | mesh or array of meshes |
| `material?` | [`Material`](Material.md) | material to use by the layer when rendering the mesh(es). If undefined is passed, the specific material created by the layer will be used. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:188

___

### shouldRender

▸ **shouldRender**(): `boolean`

Returns true if the layer contains information to display, otherwise false.

#### Returns

`boolean`

true if the glow layer should be rendered

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:776

___

### Parse

▸ `Static` **Parse**(`parsedEffectLayer`, `scene`, `rootUrl`): [`EffectLayer`](EffectLayer.md)

Creates an effect layer from parsed effect layer data

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `parsedEffectLayer` | `any` | defines effect layer data |
| `scene` | [`Scene`](Scene.md) | defines the current scene |
| `rootUrl` | `string` | defines the root URL containing the effect layer information |

#### Returns

[`EffectLayer`](EffectLayer.md)

a parsed effect Layer

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:1073
