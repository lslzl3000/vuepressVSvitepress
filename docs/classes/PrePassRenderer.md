[@dev/core](../README.md) / [Exports](../modules.md) / PrePassRenderer

# Class: PrePassRenderer

Renders a pre pass of the scene
This means every mesh in the scene will be rendered to a render target texture
And then this texture will be composited to the rendering canvas with post processes
It is necessary for effects like subsurface scattering or deferred shading

## Table of contents

### Constructors

- [constructor](PrePassRenderer.md#constructor)

### Properties

- [\_clearAttachments](PrePassRenderer.md#_clearattachments)
- [\_clearColor](PrePassRenderer.md#_clearcolor)
- [\_currentTarget](PrePassRenderer.md#_currenttarget)
- [\_defaultAttachments](PrePassRenderer.md#_defaultattachments)
- [\_effectConfigurations](PrePassRenderer.md#_effectconfigurations)
- [\_enabled](PrePassRenderer.md#_enabled)
- [\_engine](PrePassRenderer.md#_engine)
- [\_geometryBuffer](PrePassRenderer.md#_geometrybuffer)
- [\_isDirty](PrePassRenderer.md#_isdirty)
- [\_mrtFormats](PrePassRenderer.md#_mrtformats)
- [\_mrtLayout](PrePassRenderer.md#_mrtlayout)
- [\_mrtNames](PrePassRenderer.md#_mrtnames)
- [\_multiRenderAttachments](PrePassRenderer.md#_multirenderattachments)
- [\_needsCompositionForThisPass](PrePassRenderer.md#_needscompositionforthispass)
- [\_postProcessesSourceForThisPass](PrePassRenderer.md#_postprocessessourceforthispass)
- [\_scene](PrePassRenderer.md#_scene)
- [\_textureIndices](PrePassRenderer.md#_textureindices)
- [defaultRT](PrePassRenderer.md#defaultrt)
- [disableGammaTransform](PrePassRenderer.md#disablegammatransform)
- [doNotUseGeometryRendererFallback](PrePassRenderer.md#donotusegeometryrendererfallback)
- [excludedMaterials](PrePassRenderer.md#excludedmaterials)
- [excludedSkinnedMesh](PrePassRenderer.md#excludedskinnedmesh)
- [mrtCount](PrePassRenderer.md#mrtcount)
- [renderTargets](PrePassRenderer.md#rendertargets)
- [\_TextureFormats](PrePassRenderer.md#_textureformats)

### Accessors

- [currentRTisSceneRT](PrePassRenderer.md#currentrtisscenert)
- [enabled](PrePassRenderer.md#enabled)
- [isSupported](PrePassRenderer.md#issupported)
- [samples](PrePassRenderer.md#samples)

### Methods

- [\_bindFrameBuffer](PrePassRenderer.md#_bindframebuffer)
- [\_disable](PrePassRenderer.md#_disable)
- [\_enable](PrePassRenderer.md#_enable)
- [\_enableTextures](PrePassRenderer.md#_enabletextures)
- [\_getFirstPostProcess](PrePassRenderer.md#_getfirstpostprocess)
- [\_getPostProcessesSource](PrePassRenderer.md#_getpostprocessessource)
- [\_hasImageProcessing](PrePassRenderer.md#_hasimageprocessing)
- [\_linkInternalTexture](PrePassRenderer.md#_linkinternaltexture)
- [\_markAllMaterialsAsPrePassDirty](PrePassRenderer.md#_markallmaterialsasprepassdirty)
- [\_needsImageProcessing](PrePassRenderer.md#_needsimageprocessing)
- [\_prepareFrame](PrePassRenderer.md#_prepareframe)
- [\_refreshGeometryBufferRendererLink](PrePassRenderer.md#_refreshgeometrybufferrendererlink)
- [\_reinitializeAttachments](PrePassRenderer.md#_reinitializeattachments)
- [\_renderPostProcesses](PrePassRenderer.md#_renderpostprocesses)
- [\_resetLayout](PrePassRenderer.md#_resetlayout)
- [\_setEnabled](PrePassRenderer.md#_setenabled)
- [\_setRenderTargetEnabled](PrePassRenderer.md#_setrendertargetenabled)
- [\_setupOutputForThisPass](PrePassRenderer.md#_setupoutputforthispass)
- [\_update](PrePassRenderer.md#_update)
- [\_updateGeometryBufferLayout](PrePassRenderer.md#_updategeometrybufferlayout)
- [addEffectConfiguration](PrePassRenderer.md#addeffectconfiguration)
- [bindAttachmentsForEffect](PrePassRenderer.md#bindattachmentsforeffect)
- [dispose](PrePassRenderer.md#dispose)
- [getIndex](PrePassRenderer.md#getindex)
- [getRenderTarget](PrePassRenderer.md#getrendertarget)
- [markAsDirty](PrePassRenderer.md#markasdirty)
- [restoreAttachments](PrePassRenderer.md#restoreattachments)

## Constructors

### constructor

• **new PrePassRenderer**(`scene`)

Instantiates a prepass renderer

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | The scene |

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:227

## Properties

### \_clearAttachments

• `Private` **\_clearAttachments**: `number`[]

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:60

___

### \_clearColor

• `Private` `Readonly` **\_clearColor**: [`Color4`](Color4.md)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:202

___

### \_currentTarget

• `Private` **\_currentTarget**: `PrePassRenderTarget`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:195

___

### \_defaultAttachments

• `Private` **\_defaultAttachments**: `number`[]

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:59

___

### \_effectConfigurations

• `Private` **\_effectConfigurations**: `PrePassEffectConfiguration`[] = `[]`

Configuration for prepass effects

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:135

___

### \_enabled

• `Private` **\_enabled**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:204

___

### \_engine

• `Private` **\_engine**: [`Engine`](Engine.md)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:46

___

### \_geometryBuffer

• `Private` **\_geometryBuffer**: [`Nullable`](../modules.md#nullable)[`GeometryBufferRenderer`](GeometryBufferRenderer.md)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:168

___

### \_isDirty

• `Private` **\_isDirty**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:125

___

### \_mrtFormats

• `Private` **\_mrtFormats**: `number`[] = `[]`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:53

___

### \_mrtLayout

• `Private` **\_mrtLayout**: `number`[] = `[]`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:54

___

### \_mrtNames

• `Private` **\_mrtNames**: `string`[] = `[]`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:55

___

### \_multiRenderAttachments

• `Private` **\_multiRenderAttachments**: `number`[]

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:58

___

### \_needsCompositionForThisPass

• `Private` **\_needsCompositionForThisPass**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:206

___

### \_postProcessesSourceForThisPass

• `Private` **\_postProcessesSourceForThisPass**: [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:207

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:45

___

### \_textureIndices

• `Private` **\_textureIndices**: `number`[] = `[]`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:56

___

### defaultRT

• **defaultRT**: `PrePassRenderTarget`

The render target where the scene is directly rendered

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:130

___

### disableGammaTransform

• **disableGammaTransform**: `boolean` = `false`

Set to true to disable gamma transform in PrePass.
Can be useful in case you already proceed to gamma transform on a material level
and your post processes don't need to be in linear color space.

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:221

___

### doNotUseGeometryRendererFallback

• **doNotUseGeometryRendererFallback**: `boolean` = `true`

Prevents the PrePassRenderer from using the GeometryBufferRenderer as a fallback

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:173

___

### excludedMaterials

• **excludedMaterials**: [`Material`](Material.md)[] = `[]`

Force material to be excluded from the prepass
Can be useful when `useGeometryBufferFallback` is set to `true`
and you don't want a material to show in the effect.

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:43

___

### excludedSkinnedMesh

• **excludedSkinnedMesh**: [`AbstractMesh`](AbstractMesh.md)[] = `[]`

To save performance, we can excluded skinned meshes from the prepass

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:36

___

### mrtCount

• **mrtCount**: `number` = `0`

Number of textures in the multi render target texture where the scene is directly rendered

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:51

___

### renderTargets

• **renderTargets**: `PrePassRenderTarget`[] = `[]`

All the render targets generated by prepass

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:200

___

### \_TextureFormats

▪ `Static` `Private` **\_TextureFormats**: { `format`: `number` = Constants.TEXTURETYPE\_HALF\_FLOAT; `name`: `string` = "prePass\_Irradiance"; `type`: `number` = Constants.PREPASS\_IRRADIANCE\_TEXTURE\_TYPE }[]

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:82

## Accessors

### currentRTisSceneRT

• `get` **currentRTisSceneRT**(): `boolean`

Returns true if the currently rendered prePassRenderTarget is the one
associated with the scene.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:164

___

### enabled

• `get` **enabled**(): `boolean`

Indicates if the prepass is enabled

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:212

___

### isSupported

• `get` **isSupported**(): `boolean`

Indicates if rendering a prepass is supported

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:261

___

### samples

• `get` **samples**(): `number`

How many samples are used for MSAA of the scene render target

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:74

• `set` **samples**(`n`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `n` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:78

## Methods

### \_bindFrameBuffer

▸ `Private` **_bindFrameBuffer**(`prePassRenderTarget`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `prePassRenderTarget` | `PrePassRenderTarget` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:468

___

### \_disable

▸ `Private` **_disable**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:545

___

### \_enable

▸ `Private` **_enable**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:508

___

### \_enableTextures

▸ `Private` **_enableTextures**(`types`): `void`

Enables a texture on the MultiRenderTarget for prepass

#### Parameters

| Name | Type |
| :------ | :------ |
| `types` | `number`[] |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:693

___

### \_getFirstPostProcess

▸ `Private` **_getFirstPostProcess**(`postProcesses`): [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)

Internal, gets the first post proces.

#### Parameters

| Name | Type |
| :------ | :------ |
| `postProcesses` | [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)[] |

#### Returns

[`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)

the first post process to be run on this camera.

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:673

___

### \_getPostProcessesSource

▸ `Private` **_getPostProcessesSource**(`prePassRenderTarget`, `camera?`): [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)[]

#### Parameters

| Name | Type |
| :------ | :------ |
| `prePassRenderTarget` | `PrePassRenderTarget` |
| `camera?` | [`Camera`](Camera.md) |

#### Returns

[`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:559

___

### \_hasImageProcessing

▸ `Private` **_hasImageProcessing**(`postProcesses`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `postProcesses` | [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)[] |

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:654

___

### \_linkInternalTexture

▸ `Private` **_linkInternalTexture**(`prePassRenderTarget`, `postProcess`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `prePassRenderTarget` | `PrePassRenderTarget` |
| `postProcess` | [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:613

___

### \_markAllMaterialsAsPrePassDirty

▸ `Private` **_markAllMaterialsAsPrePassDirty**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:779

___

### \_needsImageProcessing

▸ `Private` **_needsImageProcessing**(): `boolean`

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:644

___

### \_prepareFrame

▸ `Private` **_prepareFrame**(`prePassRenderTarget`, `faceIndex?`, `layer?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `prePassRenderTarget` | `PrePassRenderTarget` |
| `faceIndex?` | `number` |
| `layer?` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:411

___

### \_refreshGeometryBufferRendererLink

▸ `Private` **_refreshGeometryBufferRendererLink**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:175

___

### \_reinitializeAttachments

▸ `Private` **_reinitializeAttachments**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:292

___

### \_renderPostProcesses

▸ `Private` **_renderPostProcesses**(`prePassRenderTarget`, `faceIndex?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `prePassRenderTarget` | `PrePassRenderTarget` |
| `faceIndex?` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:421

___

### \_resetLayout

▸ `Private` **_resetLayout**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:311

___

### \_setEnabled

▸ `Private` **_setEnabled**(`enabled`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `enabled` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:478

___

### \_setRenderTargetEnabled

▸ `Private` **_setRenderTargetEnabled**(`prePassRenderTarget`, `enabled`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `prePassRenderTarget` | `PrePassRenderTarget` |
| `enabled` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:482

___

### \_setupOutputForThisPass

▸ `Private` **_setupOutputForThisPass**(`prePassRenderTarget`, `camera?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `prePassRenderTarget` | `PrePassRenderTarget` |
| `camera?` | [`Camera`](Camera.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:576

___

### \_update

▸ `Private` **_update**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:715

___

### \_updateGeometryBufferLayout

▸ `Private` **_updateGeometryBufferLayout**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:323

___

### addEffectConfiguration

▸ **addEffectConfiguration**(`cfg`): `PrePassEffectConfiguration`

Adds an effect configuration to the prepass render target.
If an effect has already been added, it won't add it twice and will return the configuration
already present.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `cfg` | `PrePassEffectConfiguration` | the effect configuration |

#### Returns

`PrePassEffectConfiguration`

the effect configuration now used by the prepass

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:496

___

### bindAttachmentsForEffect

▸ **bindAttachmentsForEffect**(`effect`, `subMesh`): `void`

Sets the proper output textures to draw in the engine.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `effect` | [`Effect`](Effect.md) | The effect that is drawn. It can be or not be compatible with drawing to several output textures. |
| `subMesh` | [`SubMesh`](SubMesh.md) | Submesh on which the effect is applied |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:270

___

### dispose

▸ **dispose**(): `void`

Disposes the prepass renderer.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:790

___

### getIndex

▸ **getIndex**(`type`): `number`

Returns the index of a texture in the multi render target texture array.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | `number` | Texture type |

#### Returns

`number`

The index

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:67

___

### getRenderTarget

▸ **getRenderTarget**(): `PrePassRenderTarget`

#### Returns

`PrePassRenderTarget`

the prepass render target for the rendering pass.
If we are currently rendering a render target, it returns the PrePassRenderTarget
associated with that render target. Otherwise, it returns the scene default PrePassRenderTarget

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:142

___

### markAsDirty

▸ **markAsDirty**(): `void`

Marks the prepass renderer as dirty, triggering a check if the prepass is necessary for the next rendering.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:685

___

### restoreAttachments

▸ **restoreAttachments**(): `void`

Restores attachments for single texture draw.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRenderer.ts:376
