[@dev/core](../README.md) / [Exports](../modules.md) / GlowLayer

# Class: GlowLayer

The glow layer Helps adding a glow effect around the emissive parts of a mesh.

Once instantiated in a scene, by default, all the emissive meshes will glow.

Documentation: https://doc.babylonjs.com/how_to/glow_layer

## Hierarchy

- [`EffectLayer`](EffectLayer.md)

  ↳ **`GlowLayer`**

## Table of contents

### Constructors

- [constructor](GlowLayer.md#constructor)

### Properties

- [\_blurTexture1](GlowLayer.md#_blurtexture1)
- [\_blurTexture2](GlowLayer.md#_blurtexture2)
- [\_emissiveTextureAndColor](GlowLayer.md#_emissivetextureandcolor)
- [\_engine](GlowLayer.md#_engine)
- [\_excludedMeshes](GlowLayer.md#_excludedmeshes)
- [\_horizontalBlurPostprocess1](GlowLayer.md#_horizontalblurpostprocess1)
- [\_horizontalBlurPostprocess2](GlowLayer.md#_horizontalblurpostprocess2)
- [\_includedOnlyMeshes](GlowLayer.md#_includedonlymeshes)
- [\_intensity](GlowLayer.md#_intensity)
- [\_mainTexture](GlowLayer.md#_maintexture)
- [\_mainTextureDesiredSize](GlowLayer.md#_maintexturedesiredsize)
- [\_maxSize](GlowLayer.md#_maxsize)
- [\_meshesUsingTheirOwnMaterials](GlowLayer.md#_meshesusingtheirownmaterials)
- [\_options](GlowLayer.md#_options)
- [\_postProcesses](GlowLayer.md#_postprocesses)
- [\_postProcesses1](GlowLayer.md#_postprocesses1)
- [\_postProcesses2](GlowLayer.md#_postprocesses2)
- [\_scene](GlowLayer.md#_scene)
- [\_shouldRender](GlowLayer.md#_shouldrender)
- [\_textures](GlowLayer.md#_textures)
- [\_verticalBlurPostprocess1](GlowLayer.md#_verticalblurpostprocess1)
- [\_verticalBlurPostprocess2](GlowLayer.md#_verticalblurpostprocess2)
- [customEmissiveColorSelector](GlowLayer.md#customemissivecolorselector)
- [customEmissiveTextureSelector](GlowLayer.md#customemissivetextureselector)
- [disableBoundingBoxesFromEffectLayer](GlowLayer.md#disableboundingboxesfromeffectlayer)
- [isEnabled](GlowLayer.md#isenabled)
- [name](GlowLayer.md#name)
- [neutralColor](GlowLayer.md#neutralcolor)
- [onAfterComposeObservable](GlowLayer.md#onaftercomposeobservable)
- [onAfterRenderMeshToEffect](GlowLayer.md#onafterrendermeshtoeffect)
- [onBeforeComposeObservable](GlowLayer.md#onbeforecomposeobservable)
- [onBeforeRenderMainTextureObservable](GlowLayer.md#onbeforerendermaintextureobservable)
- [onBeforeRenderMeshToEffect](GlowLayer.md#onbeforerendermeshtoeffect)
- [onDisposeObservable](GlowLayer.md#ondisposeobservable)
- [onSizeChangedObservable](GlowLayer.md#onsizechangedobservable)
- [DefaultBlurKernelSize](GlowLayer.md#defaultblurkernelsize)
- [DefaultTextureRatio](GlowLayer.md#defaulttextureratio)
- [EffectName](GlowLayer.md#effectname)

### Accessors

- [blurKernelSize](GlowLayer.md#blurkernelsize)
- [camera](GlowLayer.md#camera)
- [intensity](GlowLayer.md#intensity)
- [mainTexture](GlowLayer.md#maintexture)
- [renderingGroupId](GlowLayer.md#renderinggroupid)

### Methods

- [\_addCustomEffectDefines](GlowLayer.md#_addcustomeffectdefines)
- [\_canRenderMesh](GlowLayer.md#_canrendermesh)
- [\_createMainTexture](GlowLayer.md#_createmaintexture)
- [\_createMergeEffect](GlowLayer.md#_createmergeeffect)
- [\_createTextureAndPostProcesses](GlowLayer.md#_createtextureandpostprocesses)
- [\_init](GlowLayer.md#_init)
- [\_internalRender](GlowLayer.md#_internalrender)
- [\_isReady](GlowLayer.md#_isready)
- [\_numInternalDraws](GlowLayer.md#_numinternaldraws)
- [\_renderSubMesh](GlowLayer.md#_rendersubmesh)
- [\_setEmissiveTextureAndColor](GlowLayer.md#_setemissivetextureandcolor)
- [\_shouldRenderEmissiveTextureForMesh](GlowLayer.md#_shouldrenderemissivetextureformesh)
- [\_shouldRenderMesh](GlowLayer.md#_shouldrendermesh)
- [\_useMeshMaterial](GlowLayer.md#_usemeshmaterial)
- [addExcludedMesh](GlowLayer.md#addexcludedmesh)
- [addIncludedOnlyMesh](GlowLayer.md#addincludedonlymesh)
- [dispose](GlowLayer.md#dispose)
- [getClassName](GlowLayer.md#getclassname)
- [getEffectName](GlowLayer.md#geteffectname)
- [hasMesh](GlowLayer.md#hasmesh)
- [isReady](GlowLayer.md#isready)
- [needStencil](GlowLayer.md#needstencil)
- [referenceMeshToUseItsOwnMaterial](GlowLayer.md#referencemeshtouseitsownmaterial)
- [removeExcludedMesh](GlowLayer.md#removeexcludedmesh)
- [removeIncludedOnlyMesh](GlowLayer.md#removeincludedonlymesh)
- [render](GlowLayer.md#render)
- [serialize](GlowLayer.md#serialize)
- [setMaterialForRendering](GlowLayer.md#setmaterialforrendering)
- [shouldRender](GlowLayer.md#shouldrender)
- [unReferenceMeshFromUsingItsOwnMaterial](GlowLayer.md#unreferencemeshfromusingitsownmaterial)
- [Parse](GlowLayer.md#parse)

## Constructors

### constructor

• **new GlowLayer**(`name`, `scene?`, `options?`)

Instantiates a new glow Layer and references it to the scene.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | The name of the layer |
| `scene?` | [`Scene`](Scene.md) | The scene to use the layer in |
| `options?` | `Partial`[`IGlowLayerOptions`](../interfaces/IGlowLayerOptions.md) | Sets of none mandatory options to use with the layer (see IGlowLayerOptions for more information) |

#### Overrides

[EffectLayer](EffectLayer.md).[constructor](EffectLayer.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:185

## Properties

### \_blurTexture1

• `Private` **\_blurTexture1**: [`RenderTargetTexture`](RenderTargetTexture.md)

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:161

___

### \_blurTexture2

• `Private` **\_blurTexture2**: [`RenderTargetTexture`](RenderTargetTexture.md)

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:162

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

https://github.com/babylon.js/core/src/Layers/effectLayer.ts:86

___

### \_engine

• `Protected` **\_engine**: [`Engine`](Engine.md)

#### Inherited from

[EffectLayer](EffectLayer.md).[_engine](EffectLayer.md#_engine)

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayer.ts:79

___

### \_excludedMeshes

• `Private` **\_excludedMeshes**: `number`[] = `[]`

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:167

___

### \_horizontalBlurPostprocess1

• `Private` **\_horizontalBlurPostprocess1**: [`BlurPostProcess`](BlurPostProcess.md)

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:157

___

### \_horizontalBlurPostprocess2

• `Private` **\_horizontalBlurPostprocess2**: [`BlurPostProcess`](BlurPostProcess.md)

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:159

___

### \_includedOnlyMeshes

• `Private` **\_includedOnlyMeshes**: `number`[] = `[]`

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:166

___

### \_intensity

• `Private` **\_intensity**: `number` = `1.0`

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:156

___

### \_mainTexture

• `Protected` **\_mainTexture**: [`RenderTargetTexture`](RenderTargetTexture.md)

#### Inherited from

[EffectLayer](EffectLayer.md).[_mainTexture](EffectLayer.md#_maintexture)

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayer.ts:82

___

### \_mainTextureDesiredSize

• `Protected` **\_mainTextureDesiredSize**: [`ISize`](../interfaces/ISize.md)

#### Inherited from

[EffectLayer](EffectLayer.md).[_mainTextureDesiredSize](EffectLayer.md#_maintexturedesiredsize)

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayer.ts:81

___

### \_maxSize

• `Protected` **\_maxSize**: `number` = `0`

#### Inherited from

[EffectLayer](EffectLayer.md).[_maxSize](EffectLayer.md#_maxsize)

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayer.ts:80

___

### \_meshesUsingTheirOwnMaterials

• `Private` **\_meshesUsingTheirOwnMaterials**: `number`[] = `[]`

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:168

___

### \_options

• `Private` **\_options**: [`IGlowLayerOptions`](../interfaces/IGlowLayerOptions.md)

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:154

___

### \_postProcesses

• `Protected` **\_postProcesses**: [`PostProcess`](PostProcess.md)[] = `[]`

#### Inherited from

[EffectLayer](EffectLayer.md).[_postProcesses](EffectLayer.md#_postprocesses)

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayer.ts:84

___

### \_postProcesses1

• `Private` **\_postProcesses1**: [`PostProcess`](PostProcess.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:163

___

### \_postProcesses2

• `Private` **\_postProcesses2**: [`PostProcess`](PostProcess.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:164

___

### \_scene

• `Protected` **\_scene**: [`Scene`](Scene.md)

#### Inherited from

[EffectLayer](EffectLayer.md).[_scene](EffectLayer.md#_scene)

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayer.ts:78

___

### \_shouldRender

• `Protected` **\_shouldRender**: `boolean` = `true`

#### Inherited from

[EffectLayer](EffectLayer.md).[_shouldRender](EffectLayer.md#_shouldrender)

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayer.ts:83

___

### \_textures

• `Protected` **\_textures**: [`BaseTexture`](BaseTexture.md)[] = `[]`

#### Inherited from

[EffectLayer](EffectLayer.md).[_textures](EffectLayer.md#_textures)

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayer.ts:85

___

### \_verticalBlurPostprocess1

• `Private` **\_verticalBlurPostprocess1**: [`BlurPostProcess`](BlurPostProcess.md)

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:158

___

### \_verticalBlurPostprocess2

• `Private` **\_verticalBlurPostprocess2**: [`BlurPostProcess`](BlurPostProcess.md)

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:160

___

### customEmissiveColorSelector

• **customEmissiveColorSelector**: (`mesh`: [`Mesh`](Mesh.md), `subMesh`: [`SubMesh`](SubMesh.md), `material`: [`Material`](Material.md), `result`: [`Color4`](Color4.md)) => `void`

#### Type declaration

▸ (`mesh`, `subMesh`, `material`, `result`): `void`

Callback used to let the user override the color selection on a per mesh basis

##### Parameters

| Name | Type |
| :------ | :------ |
| `mesh` | [`Mesh`](Mesh.md) |
| `subMesh` | [`SubMesh`](SubMesh.md) |
| `material` | [`Material`](Material.md) |
| `result` | [`Color4`](Color4.md) |

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:173

___

### customEmissiveTextureSelector

• **customEmissiveTextureSelector**: (`mesh`: [`Mesh`](Mesh.md), `subMesh`: [`SubMesh`](SubMesh.md), `material`: [`Material`](Material.md)) => [`Texture`](Texture.md)

#### Type declaration

▸ (`mesh`, `subMesh`, `material`): [`Texture`](Texture.md)

Callback used to let the user override the texture selection on a per mesh basis

##### Parameters

| Name | Type |
| :------ | :------ |
| `mesh` | [`Mesh`](Mesh.md) |
| `subMesh` | [`SubMesh`](SubMesh.md) |
| `material` | [`Material`](Material.md) |

##### Returns

[`Texture`](Texture.md)

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:177

___

### disableBoundingBoxesFromEffectLayer

• **disableBoundingBoxesFromEffectLayer**: `boolean` = `false`

Specifies if the bounding boxes should be rendered normally or if they should undergo the effect of the layer

#### Inherited from

[EffectLayer](EffectLayer.md).[disableBoundingBoxesFromEffectLayer](EffectLayer.md#disableboundingboxesfromeffectlayer)

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayer.ts:129

___

### isEnabled

• **isEnabled**: `boolean` = `true`

Specifies whether the highlight layer is enabled or not.

#### Inherited from

[EffectLayer](EffectLayer.md).[isEnabled](EffectLayer.md#isenabled)

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayer.ts:104

___

### name

• **name**: `string`

The name of the layer

#### Inherited from

[EffectLayer](EffectLayer.md).[name](EffectLayer.md#name)

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayer.ts:92

___

### neutralColor

• **neutralColor**: [`Color4`](Color4.md)

The clear color of the texture used to generate the glow map.

#### Inherited from

[EffectLayer](EffectLayer.md).[neutralColor](EffectLayer.md#neutralcolor)

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayer.ts:98

___

### onAfterComposeObservable

• **onAfterComposeObservable**: [`Observable`](Observable.md)[`EffectLayer`](EffectLayer.md)

An event triggered when the generated texture has been merged in the scene.

#### Inherited from

[EffectLayer](EffectLayer.md).[onAfterComposeObservable](EffectLayer.md#onaftercomposeobservable)

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayer.ts:159

___

### onAfterRenderMeshToEffect

• **onAfterRenderMeshToEffect**: [`Observable`](Observable.md)[`AbstractMesh`](AbstractMesh.md)

An event triggered after the mesh has been rendered into the effect render target.

#### Inherited from

[EffectLayer](EffectLayer.md).[onAfterRenderMeshToEffect](EffectLayer.md#onafterrendermeshtoeffect)

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayer.ts:154

___

### onBeforeComposeObservable

• **onBeforeComposeObservable**: [`Observable`](Observable.md)[`EffectLayer`](EffectLayer.md)

An event triggered when the generated texture is being merged in the scene.

#### Inherited from

[EffectLayer](EffectLayer.md).[onBeforeComposeObservable](EffectLayer.md#onbeforecomposeobservable)

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayer.ts:144

___

### onBeforeRenderMainTextureObservable

• **onBeforeRenderMainTextureObservable**: [`Observable`](Observable.md)[`EffectLayer`](EffectLayer.md)

An event triggered when the effect layer is about rendering the main texture with the glowy parts.

#### Inherited from

[EffectLayer](EffectLayer.md).[onBeforeRenderMainTextureObservable](EffectLayer.md#onbeforerendermaintextureobservable)

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayer.ts:139

___

### onBeforeRenderMeshToEffect

• **onBeforeRenderMeshToEffect**: [`Observable`](Observable.md)[`AbstractMesh`](AbstractMesh.md)

An event triggered when the mesh is rendered into the effect render target.

#### Inherited from

[EffectLayer](EffectLayer.md).[onBeforeRenderMeshToEffect](EffectLayer.md#onbeforerendermeshtoeffect)

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayer.ts:149

___

### onDisposeObservable

• **onDisposeObservable**: [`Observable`](Observable.md)[`EffectLayer`](EffectLayer.md)

An event triggered when the effect layer has been disposed.

#### Inherited from

[EffectLayer](EffectLayer.md).[onDisposeObservable](EffectLayer.md#ondisposeobservable)

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayer.ts:134

___

### onSizeChangedObservable

• **onSizeChangedObservable**: [`Observable`](Observable.md)[`EffectLayer`](EffectLayer.md)

An event triggered when the effect layer changes its size.

#### Inherited from

[EffectLayer](EffectLayer.md).[onSizeChangedObservable](EffectLayer.md#onsizechangedobservable)

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayer.ts:164

___

### DefaultBlurKernelSize

▪ `Static` **DefaultBlurKernelSize**: `number` = `32`

The default blur kernel size used for the glow.

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:113

___

### DefaultTextureRatio

▪ `Static` **DefaultTextureRatio**: `number` = `0.5`

The default texture size ratio used for the glow.

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:118

___

### EffectName

▪ `Static` `Readonly` **EffectName**: ``"GlowLayer"``

Effect Name of the layer.

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:108

## Accessors

### blurKernelSize

• `get` **blurKernelSize**(): `number`

Gets the kernel size of the blur.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:133

• `set` **blurKernelSize**(`value`): `void`

Sets the kernel size of the blur.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:123

___

### camera

• `get` **camera**(): [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md)

Gets the camera attached to the layer.

#### Returns

[`Nullable`](../modules.md#nullable)[`Camera`](Camera.md)

#### Inherited from

EffectLayer.camera

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayer.ts:109

___

### intensity

• `get` **intensity**(): `number`

Gets the glow intensity.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:148

• `set` **intensity**(`value`): `void`

Sets the glow intensity.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:141

___

### mainTexture

• `get` **mainTexture**(): [`RenderTargetTexture`](RenderTargetTexture.md)

Gets the main texture where the effect is rendered

#### Returns

[`RenderTargetTexture`](RenderTargetTexture.md)

#### Inherited from

EffectLayer.mainTexture

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayer.ts:169

___

### renderingGroupId

• `get` **renderingGroupId**(): `number`

Gets the rendering group id the layer should render in.

#### Returns

`number`

#### Inherited from

EffectLayer.renderingGroupId

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayer.ts:117

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

https://github.com/babylon.js/core/src/Layers/effectLayer.ts:121

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

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:496

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

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:416

___

### \_createMainTexture

▸ `Protected` **_createMainTexture**(): `void`

Creates the main texture for the effect layer.

#### Returns

`void`

#### Inherited from

[EffectLayer](EffectLayer.md).[_createMainTexture](EffectLayer.md#_createmaintexture)

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayer.ts:377

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

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:224

___

### \_createTextureAndPostProcesses

▸ `Protected` **_createTextureAndPostProcesses**(): `void`

Creates the render target textures and post processes used in the glow layer.

#### Returns

`void`

#### Overrides

[EffectLayer](EffectLayer.md).[_createTextureAndPostProcesses](EffectLayer.md#_createtextureandpostprocesses)

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:237

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

https://github.com/babylon.js/core/src/Layers/effectLayer.ts:303

___

### \_internalRender

▸ `Protected` **_internalRender**(`effect`): `void`

Implementation specific of rendering the generating effect on the main canvas.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `effect` | [`Effect`](Effect.md) | The effect used to render through |

#### Returns

`void`

#### Overrides

[EffectLayer](EffectLayer.md).[_internalRender](EffectLayer.md#_internalrender)

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:424

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

https://github.com/babylon.js/core/src/Layers/effectLayer.ts:504

___

### \_numInternalDraws

▸ `Protected` **_numInternalDraws**(): `number`

Number of times _internalRender will be called. Some effect layers need to render the mesh several times, so they should override this method with the number of times the mesh should be rendered

#### Returns

`number`

Number of times a mesh must be rendered in the layer

#### Inherited from

[EffectLayer](EffectLayer.md).[_numInternalDraws](EffectLayer.md#_numinternaldraws)

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayer.ts:295

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

https://github.com/babylon.js/core/src/Layers/effectLayer.ts:813

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

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:449

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

https://github.com/babylon.js/core/src/Layers/effectLayer.ts:804

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

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:488

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

#### Overrides

[EffectLayer](EffectLayer.md).[_useMeshMaterial](EffectLayer.md#_usemeshmaterial)

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:569

___

### addExcludedMesh

▸ **addExcludedMesh**(`mesh`): `void`

Add a mesh in the exclusion list to prevent it to impact or being impacted by the glow layer.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`Mesh`](Mesh.md) | The mesh to exclude from the glow layer |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:504

___

### addIncludedOnlyMesh

▸ **addIncludedOnlyMesh**(`mesh`): `void`

Add a mesh in the inclusion list to impact or being impacted by the glow layer.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`Mesh`](Mesh.md) | The mesh to include in the glow layer |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:525

___

### dispose

▸ **dispose**(): `void`

Dispose the highlight layer and free resources.

#### Returns

`void`

#### Inherited from

[EffectLayer](EffectLayer.md).[dispose](EffectLayer.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayer.ts:1020

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

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:618

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

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:216

___

### hasMesh

▸ **hasMesh**(`mesh`): `boolean`

Determine if a given mesh will be used in the glow layer

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | The mesh to test |

#### Returns

`boolean`

true if the mesh will be highlighted by the current glow layer

#### Overrides

[EffectLayer](EffectLayer.md).[hasMesh](EffectLayer.md#hasmesh)

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:547

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

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:391

___

### needStencil

▸ **needStencil**(): `boolean`

Returns whether or not the layer needs stencil enabled during the mesh rendering.

#### Returns

`boolean`

#### Overrides

[EffectLayer](EffectLayer.md).[needStencil](EffectLayer.md#needstencil)

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:406

___

### referenceMeshToUseItsOwnMaterial

▸ **referenceMeshToUseItsOwnMaterial**(`mesh`): `void`

Add a mesh to be rendered through its own material and not with emissive only.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | The mesh for which we need to use its material |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:580

___

### removeExcludedMesh

▸ **removeExcludedMesh**(`mesh`): `void`

Remove a mesh from the exclusion list to let it impact or being impacted by the glow layer.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`Mesh`](Mesh.md) | The mesh to remove |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:514

___

### removeIncludedOnlyMesh

▸ **removeIncludedOnlyMesh**(`mesh`): `void`

Remove a mesh from the Inclusion list to prevent it to impact or being impacted by the glow layer.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`Mesh`](Mesh.md) | The mesh to remove |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:535

___

### render

▸ **render**(): `void`

Renders the glowing part of the scene by blending the blurred glowing meshes on top of the rendered scene.

#### Returns

`void`

#### Inherited from

[EffectLayer](EffectLayer.md).[render](EffectLayer.md#render)

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayer.ts:693

___

### serialize

▸ **serialize**(): `any`

Serializes this glow layer

#### Returns

`any`

a serialized glow layer object

#### Overrides

[EffectLayer](EffectLayer.md).[serialize](EffectLayer.md#serialize)

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:626

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

https://github.com/babylon.js/core/src/Layers/effectLayer.ts:188

___

### shouldRender

▸ **shouldRender**(): `boolean`

Returns true if the layer contains information to display, otherwise false.

#### Returns

`boolean`

true if the glow layer should be rendered

#### Inherited from

[EffectLayer](EffectLayer.md).[shouldRender](EffectLayer.md#shouldrender)

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayer.ts:776

___

### unReferenceMeshFromUsingItsOwnMaterial

▸ **unReferenceMeshFromUsingItsOwnMaterial**(`mesh`): `void`

Remove a mesh from being rendered through its own material and not with emissive only.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | The mesh for which we need to not use its material |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:594

___

### Parse

▸ `Static` **Parse**(`parsedGlowLayer`, `scene`, `rootUrl`): [`GlowLayer`](GlowLayer.md)

Creates a Glow Layer from parsed glow layer data

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `parsedGlowLayer` | `any` | defines glow layer data |
| `scene` | [`Scene`](Scene.md) | defines the current scene |
| `rootUrl` | `string` | defines the root URL containing the glow layer information |

#### Returns

[`GlowLayer`](GlowLayer.md)

a parsed Glow Layer

#### Overrides

[EffectLayer](EffectLayer.md).[Parse](EffectLayer.md#parse)

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:666
