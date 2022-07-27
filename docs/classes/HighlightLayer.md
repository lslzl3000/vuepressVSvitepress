[@dev/core](../README.md) / [Exports](../modules.md) / HighlightLayer

# Class: HighlightLayer

The highlight layer Helps adding a glow effect around a mesh.

Once instantiated in a scene, simply use the addMesh or removeMesh method to add or remove
glowy meshes to your scene.

!!! THIS REQUIRES AN ACTIVE STENCIL BUFFER ON THE CANVAS !!!

## Hierarchy

- [`EffectLayer`](EffectLayer.md)

  ↳ **`HighlightLayer`**

## Table of contents

### Constructors

- [constructor](HighlightLayer.md#constructor)

### Properties

- [\_blurTexture](HighlightLayer.md#_blurtexture)
- [\_downSamplePostprocess](HighlightLayer.md#_downsamplepostprocess)
- [\_emissiveTextureAndColor](HighlightLayer.md#_emissivetextureandcolor)
- [\_engine](HighlightLayer.md#_engine)
- [\_excludedMeshes](HighlightLayer.md#_excludedmeshes)
- [\_horizontalBlurPostprocess](HighlightLayer.md#_horizontalblurpostprocess)
- [\_instanceGlowingMeshStencilReference](HighlightLayer.md#_instanceglowingmeshstencilreference)
- [\_mainTexture](HighlightLayer.md#_maintexture)
- [\_mainTextureDesiredSize](HighlightLayer.md#_maintexturedesiredsize)
- [\_maxSize](HighlightLayer.md#_maxsize)
- [\_meshes](HighlightLayer.md#_meshes)
- [\_options](HighlightLayer.md#_options)
- [\_postProcesses](HighlightLayer.md#_postprocesses)
- [\_scene](HighlightLayer.md#_scene)
- [\_shouldRender](HighlightLayer.md#_shouldrender)
- [\_textures](HighlightLayer.md#_textures)
- [\_verticalBlurPostprocess](HighlightLayer.md#_verticalblurpostprocess)
- [disableBoundingBoxesFromEffectLayer](HighlightLayer.md#disableboundingboxesfromeffectlayer)
- [innerGlow](HighlightLayer.md#innerglow)
- [isEnabled](HighlightLayer.md#isenabled)
- [name](HighlightLayer.md#name)
- [neutralColor](HighlightLayer.md#neutralcolor)
- [onAfterBlurObservable](HighlightLayer.md#onafterblurobservable)
- [onAfterComposeObservable](HighlightLayer.md#onaftercomposeobservable)
- [onAfterRenderMeshToEffect](HighlightLayer.md#onafterrendermeshtoeffect)
- [onBeforeBlurObservable](HighlightLayer.md#onbeforeblurobservable)
- [onBeforeComposeObservable](HighlightLayer.md#onbeforecomposeobservable)
- [onBeforeRenderMainTextureObservable](HighlightLayer.md#onbeforerendermaintextureobservable)
- [onBeforeRenderMeshToEffect](HighlightLayer.md#onbeforerendermeshtoeffect)
- [onDisposeObservable](HighlightLayer.md#ondisposeobservable)
- [onSizeChangedObservable](HighlightLayer.md#onsizechangedobservable)
- [outerGlow](HighlightLayer.md#outerglow)
- [EffectName](HighlightLayer.md#effectname)
- [GlowingMeshStencilReference](HighlightLayer.md#glowingmeshstencilreference)
- [NeutralColor](HighlightLayer.md#neutralcolor-1)
- [NormalMeshStencilReference](HighlightLayer.md#normalmeshstencilreference)

### Accessors

- [blurHorizontalSize](HighlightLayer.md#blurhorizontalsize)
- [blurVerticalSize](HighlightLayer.md#blurverticalsize)
- [camera](HighlightLayer.md#camera)
- [mainTexture](HighlightLayer.md#maintexture)
- [renderingGroupId](HighlightLayer.md#renderinggroupid)

### Methods

- [\_addCustomEffectDefines](HighlightLayer.md#_addcustomeffectdefines)
- [\_canRenderMesh](HighlightLayer.md#_canrendermesh)
- [\_createMainTexture](HighlightLayer.md#_createmaintexture)
- [\_createMergeEffect](HighlightLayer.md#_createmergeeffect)
- [\_createTextureAndPostProcesses](HighlightLayer.md#_createtextureandpostprocesses)
- [\_defaultStencilReference](HighlightLayer.md#_defaultstencilreference)
- [\_init](HighlightLayer.md#_init)
- [\_internalRender](HighlightLayer.md#_internalrender)
- [\_isReady](HighlightLayer.md#_isready)
- [\_numInternalDraws](HighlightLayer.md#_numinternaldraws)
- [\_renderSubMesh](HighlightLayer.md#_rendersubmesh)
- [\_setEmissiveTextureAndColor](HighlightLayer.md#_setemissivetextureandcolor)
- [\_shouldRenderEmissiveTextureForMesh](HighlightLayer.md#_shouldrenderemissivetextureformesh)
- [\_shouldRenderMesh](HighlightLayer.md#_shouldrendermesh)
- [\_useMeshMaterial](HighlightLayer.md#_usemeshmaterial)
- [addExcludedMesh](HighlightLayer.md#addexcludedmesh)
- [addMesh](HighlightLayer.md#addmesh)
- [dispose](HighlightLayer.md#dispose)
- [getClassName](HighlightLayer.md#getclassname)
- [getEffectName](HighlightLayer.md#geteffectname)
- [hasMesh](HighlightLayer.md#hasmesh)
- [isReady](HighlightLayer.md#isready)
- [needStencil](HighlightLayer.md#needstencil)
- [removeAllMeshes](HighlightLayer.md#removeallmeshes)
- [removeExcludedMesh](HighlightLayer.md#removeexcludedmesh)
- [removeMesh](HighlightLayer.md#removemesh)
- [render](HighlightLayer.md#render)
- [serialize](HighlightLayer.md#serialize)
- [setMaterialForRendering](HighlightLayer.md#setmaterialforrendering)
- [shouldRender](HighlightLayer.md#shouldrender)
- [Parse](HighlightLayer.md#parse)

## Constructors

### constructor

• **new HighlightLayer**(`name`, `scene?`, `options?`)

Instantiates a new highlight Layer and references it to the scene..

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | The name of the layer |
| `scene?` | [`Scene`](Scene.md) | The scene to use the layer in |
| `options?` | `Partial`[`IHighlightLayerOptions`](../interfaces/IHighlightLayerOptions.md) | Sets of none mandatory options to use with the layer (see IHighlightLayerOptions for more information) |

#### Overrides

[EffectLayer](EffectLayer.md).[constructor](EffectLayer.md#constructor)

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:280

## Properties

### \_blurTexture

• `Private` **\_blurTexture**: [`RenderTargetTexture`](RenderTargetTexture.md)

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:269

___

### \_downSamplePostprocess

• `Private` **\_downSamplePostprocess**: [`PassPostProcess`](PassPostProcess.md)

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:266

___

### \_emissiveTextureAndColor

• `Protected` **\_emissiveTextureAndColor**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `color` | [`Color4`](Color4.md) |
| `texture` | [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) |

#### Inherited from

[EffectLayer](EffectLayer.md).[_emissiveTextureAndColor](EffectLayer.md#_emissivetextureandcolor)

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:86

___

### \_engine

• `Protected` **\_engine**: [`Engine`](Engine.md)

#### Inherited from

[EffectLayer](EffectLayer.md).[_engine](EffectLayer.md#_engine)

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:79

___

### \_excludedMeshes

• `Private` **\_excludedMeshes**: [`Nullable`](../modules.md#nullable){ `[id: string]`: [`Nullable`](../modules.md#nullable)`IHighlightLayerExcludedMesh`;  } = `{}`

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:272

___

### \_horizontalBlurPostprocess

• `Private` **\_horizontalBlurPostprocess**: `GlowBlurPostProcess`

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:267

___

### \_instanceGlowingMeshStencilReference

• `Private` **\_instanceGlowingMeshStencilReference**: `number`

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:262

___

### \_mainTexture

• `Protected` **\_mainTexture**: [`RenderTargetTexture`](RenderTargetTexture.md)

#### Inherited from

[EffectLayer](EffectLayer.md).[_mainTexture](EffectLayer.md#_maintexture)

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:82

___

### \_mainTextureDesiredSize

• `Protected` **\_mainTextureDesiredSize**: [`ISize`](../interfaces/ISize.md)

#### Inherited from

[EffectLayer](EffectLayer.md).[_mainTextureDesiredSize](EffectLayer.md#_maintexturedesiredsize)

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:81

___

### \_maxSize

• `Protected` **\_maxSize**: `number` = `0`

#### Inherited from

[EffectLayer](EffectLayer.md).[_maxSize](EffectLayer.md#_maxsize)

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:80

___

### \_meshes

• `Private` **\_meshes**: [`Nullable`](../modules.md#nullable){ `[id: string]`: [`Nullable`](../modules.md#nullable)`IHighlightLayerMesh`;  } = `{}`

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:271

___

### \_options

• `Private` **\_options**: [`IHighlightLayerOptions`](../interfaces/IHighlightLayerOptions.md)

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:265

___

### \_postProcesses

• `Protected` **\_postProcesses**: [`PostProcess`](PostProcess.md)[] = `[]`

#### Inherited from

[EffectLayer](EffectLayer.md).[_postProcesses](EffectLayer.md#_postprocesses)

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:84

___

### \_scene

• `Protected` **\_scene**: [`Scene`](Scene.md)

#### Inherited from

[EffectLayer](EffectLayer.md).[_scene](EffectLayer.md#_scene)

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:78

___

### \_shouldRender

• `Protected` **\_shouldRender**: `boolean` = `true`

#### Inherited from

[EffectLayer](EffectLayer.md).[_shouldRender](EffectLayer.md#_shouldrender)

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:83

___

### \_textures

• `Protected` **\_textures**: [`BaseTexture`](BaseTexture.md)[] = `[]`

#### Inherited from

[EffectLayer](EffectLayer.md).[_textures](EffectLayer.md#_textures)

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:85

___

### \_verticalBlurPostprocess

• `Private` **\_verticalBlurPostprocess**: `GlowBlurPostProcess`

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:268

___

### disableBoundingBoxesFromEffectLayer

• **disableBoundingBoxesFromEffectLayer**: `boolean` = `false`

Specifies if the bounding boxes should be rendered normally or if they should undergo the effect of the layer

#### Inherited from

[EffectLayer](EffectLayer.md).[disableBoundingBoxesFromEffectLayer](EffectLayer.md#disableboundingboxesfromeffectlayer)

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:129

___

### innerGlow

• **innerGlow**: `boolean` = `true`

Specifies whether or not the inner glow is ACTIVE in the layer.

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:212

___

### isEnabled

• **isEnabled**: `boolean` = `true`

Specifies whether the highlight layer is enabled or not.

#### Inherited from

[EffectLayer](EffectLayer.md).[isEnabled](EffectLayer.md#isenabled)

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:104

___

### name

• **name**: `string`

The name of the layer

#### Inherited from

[EffectLayer](EffectLayer.md).[name](EffectLayer.md#name)

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:280

___

### neutralColor

• **neutralColor**: [`Color4`](Color4.md)

The clear color of the texture used to generate the glow map.

#### Inherited from

[EffectLayer](EffectLayer.md).[neutralColor](EffectLayer.md#neutralcolor)

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:98

___

### onAfterBlurObservable

• **onAfterBlurObservable**: [`Observable`](Observable.md)[`HighlightLayer`](HighlightLayer.md)

An event triggered when the highlight layer has been blurred.

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:260

___

### onAfterComposeObservable

• **onAfterComposeObservable**: [`Observable`](Observable.md)[`EffectLayer`](EffectLayer.md)

An event triggered when the generated texture has been merged in the scene.

#### Inherited from

[EffectLayer](EffectLayer.md).[onAfterComposeObservable](EffectLayer.md#onaftercomposeobservable)

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:159

___

### onAfterRenderMeshToEffect

• **onAfterRenderMeshToEffect**: [`Observable`](Observable.md)[`AbstractMesh`](AbstractMesh.md)

An event triggered after the mesh has been rendered into the effect render target.

#### Inherited from

[EffectLayer](EffectLayer.md).[onAfterRenderMeshToEffect](EffectLayer.md#onafterrendermeshtoeffect)

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:154

___

### onBeforeBlurObservable

• **onBeforeBlurObservable**: [`Observable`](Observable.md)[`HighlightLayer`](HighlightLayer.md)

An event triggered when the highlight layer is being blurred.

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:255

___

### onBeforeComposeObservable

• **onBeforeComposeObservable**: [`Observable`](Observable.md)[`EffectLayer`](EffectLayer.md)

An event triggered when the generated texture is being merged in the scene.

#### Inherited from

[EffectLayer](EffectLayer.md).[onBeforeComposeObservable](EffectLayer.md#onbeforecomposeobservable)

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:144

___

### onBeforeRenderMainTextureObservable

• **onBeforeRenderMainTextureObservable**: [`Observable`](Observable.md)[`EffectLayer`](EffectLayer.md)

An event triggered when the effect layer is about rendering the main texture with the glowy parts.

#### Inherited from

[EffectLayer](EffectLayer.md).[onBeforeRenderMainTextureObservable](EffectLayer.md#onbeforerendermaintextureobservable)

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:139

___

### onBeforeRenderMeshToEffect

• **onBeforeRenderMeshToEffect**: [`Observable`](Observable.md)[`AbstractMesh`](AbstractMesh.md)

An event triggered when the mesh is rendered into the effect render target.

#### Inherited from

[EffectLayer](EffectLayer.md).[onBeforeRenderMeshToEffect](EffectLayer.md#onbeforerendermeshtoeffect)

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:149

___

### onDisposeObservable

• **onDisposeObservable**: [`Observable`](Observable.md)[`EffectLayer`](EffectLayer.md)

An event triggered when the effect layer has been disposed.

#### Inherited from

[EffectLayer](EffectLayer.md).[onDisposeObservable](EffectLayer.md#ondisposeobservable)

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:134

___

### onSizeChangedObservable

• **onSizeChangedObservable**: [`Observable`](Observable.md)[`EffectLayer`](EffectLayer.md)

An event triggered when the effect layer changes its size.

#### Inherited from

[EffectLayer](EffectLayer.md).[onSizeChangedObservable](EffectLayer.md#onsizechangedobservable)

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:164

___

### outerGlow

• **outerGlow**: `boolean` = `true`

Specifies whether or not the outer glow is ACTIVE in the layer.

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:218

___

### EffectName

▪ `Static` `Readonly` **EffectName**: ``"HighlightLayer"``

Effect Name of the highlight layer.

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:190

___

### GlowingMeshStencilReference

▪ `Static` **GlowingMeshStencilReference**: `number` = `0x02`

Stencil value used for glowing meshes.

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:201

___

### NeutralColor

▪ `Static` **NeutralColor**: [`Color4`](Color4.md)

The neutral color used during the preparation of the glow effect.
This is black by default as the blend operation is a blend operation.

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:196

___

### NormalMeshStencilReference

▪ `Static` **NormalMeshStencilReference**: `number` = `0x01`

Stencil value used for the other meshes in the scene.

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:206

## Accessors

### blurHorizontalSize

• `get` **blurHorizontalSize**(): `number`

Gets the horizontal size of the blur.

#### Returns

`number`

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:239

• `set` **blurHorizontalSize**(`value`): `void`

Specifies the horizontal size of the blur.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:223

___

### blurVerticalSize

• `get` **blurVerticalSize**(): `number`

Gets the vertical size of the blur.

#### Returns

`number`

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:247

• `set` **blurVerticalSize**(`value`): `void`

Specifies the vertical size of the blur.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:231

___

### camera

• `get` **camera**(): [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md)

Gets the camera attached to the layer.

#### Returns

[`Nullable`](../modules.md#nullable)[`Camera`](Camera.md)

#### Inherited from

EffectLayer.camera

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:109

___

### mainTexture

• `get` **mainTexture**(): [`RenderTargetTexture`](RenderTargetTexture.md)

Gets the main texture where the effect is rendered

#### Returns

[`RenderTargetTexture`](RenderTargetTexture.md)

#### Inherited from

EffectLayer.mainTexture

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:169

___

### renderingGroupId

• `get` **renderingGroupId**(): `number`

Gets the rendering group id the layer should render in.

#### Returns

`number`

#### Inherited from

EffectLayer.renderingGroupId

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:117

• `set` **renderingGroupId**(`renderingGroupId`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `renderingGroupId` | `number` |

#### Returns

`void`

#### Inherited from

EffectLayer.renderingGroupId

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

#### Overrides

[EffectLayer](EffectLayer.md).[_addCustomEffectDefines](EffectLayer.md#_addcustomeffectdefines)

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:584

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

#### Overrides

[EffectLayer](EffectLayer.md).[_canRenderMesh](EffectLayer.md#_canrendermesh)

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:575

___

### \_createMainTexture

▸ `Protected` **_createMainTexture**(): `void`

Creates the main texture for the effect layer.

#### Returns

`void`

#### Inherited from

[EffectLayer](EffectLayer.md).[_createMainTexture](EffectLayer.md#_createmaintexture)

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:377

___

### \_createMergeEffect

▸ `Protected` **_createMergeEffect**(): [`Effect`](Effect.md)

Create the merge effect. This is the shader use to blit the information back
to the main canvas at the end of the scene rendering.

#### Returns

[`Effect`](Effect.md)

#### Overrides

[EffectLayer](EffectLayer.md).[_createMergeEffect](EffectLayer.md#_createmergeeffect)

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:330

___

### \_createTextureAndPostProcesses

▸ `Protected` **_createTextureAndPostProcesses**(): `void`

Creates the render target textures and post processes used in the highlight layer.

#### Returns

`void`

#### Overrides

[EffectLayer](EffectLayer.md).[_createTextureAndPostProcesses](EffectLayer.md#_createtextureandpostprocesses)

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:338

___

### \_defaultStencilReference

▸ `Private` **_defaultStencilReference**(`mesh`): `void`

Force the stencil to the normal expected value for none glowing parts

#### Parameters

| Name | Type |
| :------ | :------ |
| `mesh` | [`Mesh`](Mesh.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:769

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

#### Inherited from

[EffectLayer](EffectLayer.md).[_init](EffectLayer.md#_init)

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:303

___

### \_internalRender

▸ `Protected` **_internalRender**(`effect`, `renderIndex`): `void`

Implementation specific of rendering the generating effect on the main canvas.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `effect` | [`Effect`](Effect.md) | The effect used to render through |
| `renderIndex` | `number` |  |

#### Returns

`void`

#### Overrides

[EffectLayer](EffectLayer.md).[_internalRender](EffectLayer.md#_internalrender)

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:504

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

#### Inherited from

[EffectLayer](EffectLayer.md).[_isReady](EffectLayer.md#_isready)

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:504

___

### \_numInternalDraws

▸ `Protected` **_numInternalDraws**(): `number`

Number of times _internalRender will be called. Some effect layers need to render the mesh several times, so they should override this method with the number of times the mesh should be rendered

#### Returns

`number`

Number of times a mesh must be rendered in the layer

#### Overrides

[EffectLayer](EffectLayer.md).[_numInternalDraws](EffectLayer.md#_numinternaldraws)

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:322

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

#### Inherited from

[EffectLayer](EffectLayer.md).[_renderSubMesh](EffectLayer.md#_rendersubmesh)

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:813

___

### \_setEmissiveTextureAndColor

▸ `Protected` **_setEmissiveTextureAndColor**(`mesh`, `subMesh`, `material`): `void`

Sets the required values for both the emissive texture and and the main color.

#### Parameters

| Name | Type |
| :------ | :------ |
| `mesh` | [`Mesh`](Mesh.md) |
| `subMesh` | [`SubMesh`](SubMesh.md) |
| `material` | [`Material`](Material.md) |

#### Returns

`void`

#### Overrides

[EffectLayer](EffectLayer.md).[_setEmissiveTextureAndColor](EffectLayer.md#_setemissivetextureandcolor)

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:594

___

### \_shouldRenderEmissiveTextureForMesh

▸ `Protected` **_shouldRenderEmissiveTextureForMesh**(): `boolean`

Returns true if the mesh should render, otherwise false.

#### Returns

`boolean`

true if it should render otherwise false

#### Inherited from

[EffectLayer](EffectLayer.md).[_shouldRenderEmissiveTextureForMesh](EffectLayer.md#_shouldrenderemissivetextureformesh)

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:804

___

### \_shouldRenderMesh

▸ `Protected` **_shouldRenderMesh**(`mesh`): `boolean`

Returns true if the mesh should render, otherwise false.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`Mesh`](Mesh.md) | The mesh to render |

#### Returns

`boolean`

true if it should render otherwise false

#### Overrides

[EffectLayer](EffectLayer.md).[_shouldRenderMesh](EffectLayer.md#_shouldrendermesh)

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:556

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

#### Inherited from

[EffectLayer](EffectLayer.md).[_useMeshMaterial](EffectLayer.md#_usemeshmaterial)

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:978

___

### addExcludedMesh

▸ **addExcludedMesh**(`mesh`): `void`

Add a mesh in the exclusion list to prevent it to impact or being impacted by the highlight layer.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`Mesh`](Mesh.md) | The mesh to exclude from the highlight layer |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:614

___

### addMesh

▸ **addMesh**(`mesh`, `color`, `glowEmissiveOnly?`): `void`

Add a mesh in the highlight layer in order to make it glow with the chosen color.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `mesh` | [`Mesh`](Mesh.md) | `undefined` | The mesh to highlight |
| `color` | [`Color3`](Color3.md) | `undefined` | The color of the highlight |
| `glowEmissiveOnly` | `boolean` | `false` | Extract the glow from the emissive texture |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:679

___

### dispose

▸ **dispose**(): `void`

Dispose the highlight layer and free resources.

#### Returns

`void`

#### Overrides

[EffectLayer](EffectLayer.md).[dispose](EffectLayer.md#dispose)

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:787

___

### getClassName

▸ **getClassName**(): `string`

Gets the class name of the effect layer

#### Returns

`string`

the string with the class name of the effect layer

#### Overrides

[EffectLayer](EffectLayer.md).[getClassName](EffectLayer.md#getclassname)

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:828

___

### getEffectName

▸ **getEffectName**(): `string`

Get the effect name of the layer.

#### Returns

`string`

The effect name

#### Overrides

[EffectLayer](EffectLayer.md).[getEffectName](EffectLayer.md#geteffectname)

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:318

___

### hasMesh

▸ **hasMesh**(`mesh`): `boolean`

Determine if a given mesh will be highlighted by the current HighlightLayer

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | mesh to test |

#### Returns

`boolean`

true if the mesh will be highlighted by the current HighlightLayer

#### Overrides

[EffectLayer](EffectLayer.md).[hasMesh](EffectLayer.md#hasmesh)

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:661

___

### isReady

▸ **isReady**(`subMesh`, `useInstances`): `boolean`

Checks for the readiness of the element composing the layer.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `subMesh` | [`SubMesh`](SubMesh.md) | the mesh to check for |
| `useInstances` | `boolean` | specify whether or not to use instances to render the mesh |

#### Returns

`boolean`

true if ready otherwise, false

#### Overrides

[EffectLayer](EffectLayer.md).[isReady](EffectLayer.md#isready)

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:482

___

### needStencil

▸ **needStencil**(): `boolean`

Returns whether or not the layer needs stencil enabled during the mesh rendering.

#### Returns

`boolean`

#### Overrides

[EffectLayer](EffectLayer.md).[needStencil](EffectLayer.md#needstencil)

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:472

___

### removeAllMeshes

▸ **removeAllMeshes**(): `void`

Remove all the meshes currently referenced in the highlight layer

#### Returns

`void`

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:750

___

### removeExcludedMesh

▸ **removeExcludedMesh**(`mesh`): `void`

Remove a mesh from the exclusion list to let it impact or being impacted by the highlight layer.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`Mesh`](Mesh.md) | The mesh to highlight |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:637

___

### removeMesh

▸ **removeMesh**(`mesh`): `void`

Remove a mesh from the highlight layer in order to make it stop glowing.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`Mesh`](Mesh.md) | The mesh to highlight |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:721

___

### render

▸ **render**(): `void`

Renders the glowing part of the scene by blending the blurred glowing meshes on top of the rendered scene.

#### Returns

`void`

#### Inherited from

[EffectLayer](EffectLayer.md).[render](EffectLayer.md#render)

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:693

___

### serialize

▸ **serialize**(): `any`

Serializes this Highlight layer

#### Returns

`any`

a serialized Highlight layer object

#### Overrides

[EffectLayer](EffectLayer.md).[serialize](EffectLayer.md#serialize)

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:836

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

#### Inherited from

[EffectLayer](EffectLayer.md).[setMaterialForRendering](EffectLayer.md#setmaterialforrendering)

#### Defined in

packages/dev/core/src/Layers/effectLayer.ts:188

___

### shouldRender

▸ **shouldRender**(): `boolean`

Returns true if the layer contains information to display, otherwise false.

#### Returns

`boolean`

#### Overrides

[EffectLayer](EffectLayer.md).[shouldRender](EffectLayer.md#shouldrender)

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:543

___

### Parse

▸ `Static` **Parse**(`parsedHightlightLayer`, `scene`, `rootUrl`): [`HighlightLayer`](HighlightLayer.md)

Creates a Highlight layer from parsed Highlight layer data

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `parsedHightlightLayer` | `any` | defines the Highlight layer data |
| `scene` | [`Scene`](Scene.md) | defines the current scene |
| `rootUrl` | `string` | defines the root URL containing the Highlight layer information |

#### Returns

[`HighlightLayer`](HighlightLayer.md)

a parsed Highlight layer

#### Overrides

[EffectLayer](EffectLayer.md).[Parse](EffectLayer.md#parse)

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:880
