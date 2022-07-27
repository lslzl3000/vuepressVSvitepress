[@dev/core](../README.md) / [Exports](../modules.md) / DepthPeelingRenderer

# Class: DepthPeelingRenderer

The depth peeling renderer that performs
Order independant transparency (OIT).
This should not be instanciated directly, as it is part of a scene component

## Table of contents

### Constructors

- [constructor](DepthPeelingRenderer.md#constructor)

### Properties

- [\_blendBackEffectWrapper](DepthPeelingRenderer.md#_blendbackeffectwrapper)
- [\_blendBackEffectWrapperPingPong](DepthPeelingRenderer.md#_blendbackeffectwrapperpingpong)
- [\_blendBackMrt](DepthPeelingRenderer.md#_blendbackmrt)
- [\_blendBackTexture](DepthPeelingRenderer.md#_blendbacktexture)
- [\_candidateSubMeshes](DepthPeelingRenderer.md#_candidatesubmeshes)
- [\_colorCache](DepthPeelingRenderer.md#_colorcache)
- [\_colorMrts](DepthPeelingRenderer.md#_colormrts)
- [\_currentPingPongState](DepthPeelingRenderer.md#_currentpingpongstate)
- [\_depthMrts](DepthPeelingRenderer.md#_depthmrts)
- [\_effectRenderer](DepthPeelingRenderer.md#_effectrenderer)
- [\_engine](DepthPeelingRenderer.md#_engine)
- [\_excludedSubMeshes](DepthPeelingRenderer.md#_excludedsubmeshes)
- [\_finalEffectWrapper](DepthPeelingRenderer.md#_finaleffectwrapper)
- [\_layoutCache](DepthPeelingRenderer.md#_layoutcache)
- [\_layoutCacheFormat](DepthPeelingRenderer.md#_layoutcacheformat)
- [\_passCount](DepthPeelingRenderer.md#_passcount)
- [\_prePassEffectConfiguration](DepthPeelingRenderer.md#_prepasseffectconfiguration)
- [\_renderPassIds](DepthPeelingRenderer.md#_renderpassids)
- [\_scene](DepthPeelingRenderer.md#_scene)
- [\_thinTextures](DepthPeelingRenderer.md#_thintextures)
- [\_useRenderPasses](DepthPeelingRenderer.md#_userenderpasses)
- [\_DEPTH\_CLEAR\_VALUE](DepthPeelingRenderer.md#_depth_clear_value)
- [\_MAX\_DEPTH](DepthPeelingRenderer.md#_max_depth)
- [\_MIN\_DEPTH](DepthPeelingRenderer.md#_min_depth)

### Accessors

- [passCount](DepthPeelingRenderer.md#passcount)
- [useRenderPasses](DepthPeelingRenderer.md#userenderpasses)

### Methods

- [\_createEffects](DepthPeelingRenderer.md#_createeffects)
- [\_createRenderPassIds](DepthPeelingRenderer.md#_createrenderpassids)
- [\_createTextures](DepthPeelingRenderer.md#_createtextures)
- [\_disposeTextures](DepthPeelingRenderer.md#_disposetextures)
- [\_finalCompose](DepthPeelingRenderer.md#_finalcompose)
- [\_releaseRenderPassIds](DepthPeelingRenderer.md#_releaserenderpassids)
- [\_renderSubMeshes](DepthPeelingRenderer.md#_rendersubmeshes)
- [\_updateTextureReferences](DepthPeelingRenderer.md#_updatetexturereferences)
- [\_updateTextures](DepthPeelingRenderer.md#_updatetextures)
- [bind](DepthPeelingRenderer.md#bind)
- [dispose](DepthPeelingRenderer.md#dispose)
- [render](DepthPeelingRenderer.md#render)
- [setPrePassRenderer](DepthPeelingRenderer.md#setprepassrenderer)

## Constructors

### constructor

• **new DepthPeelingRenderer**(`scene`, `passCount?`)

Instanciates the depth peeling renderer

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | `undefined` | Scene to attach to |
| `passCount` | `number` | `5` | Number of depth layers to peel |

#### Defined in

packages/dev/core/src/Rendering/depthPeelingRenderer.ts:120

## Properties

### \_blendBackEffectWrapper

• `Private` **\_blendBackEffectWrapper**: [`EffectWrapper`](EffectWrapper.md)

#### Defined in

packages/dev/core/src/Rendering/depthPeelingRenderer.ts:57

___

### \_blendBackEffectWrapperPingPong

• `Private` **\_blendBackEffectWrapperPingPong**: [`EffectWrapper`](EffectWrapper.md)

#### Defined in

packages/dev/core/src/Rendering/depthPeelingRenderer.ts:58

___

### \_blendBackMrt

• `Private` **\_blendBackMrt**: [`MultiRenderTarget`](MultiRenderTarget.md)

#### Defined in

packages/dev/core/src/Rendering/depthPeelingRenderer.ts:55

___

### \_blendBackTexture

• `Private` **\_blendBackTexture**: [`InternalTexture`](InternalTexture.md)

#### Defined in

packages/dev/core/src/Rendering/depthPeelingRenderer.ts:65

___

### \_candidateSubMeshes

• `Private` **\_candidateSubMeshes**: [`SmartArray`](SmartArray.md)[`SubMesh`](SubMesh.md)

#### Defined in

packages/dev/core/src/Rendering/depthPeelingRenderer.ts:69

___

### \_colorCache

• `Private` **\_colorCache**: [`Color4`](Color4.md)[]

#### Defined in

packages/dev/core/src/Rendering/depthPeelingRenderer.ts:76

___

### \_colorMrts

• `Private` **\_colorMrts**: [`MultiRenderTarget`](MultiRenderTarget.md)[]

#### Defined in

packages/dev/core/src/Rendering/depthPeelingRenderer.ts:54

___

### \_currentPingPongState

• `Private` **\_currentPingPongState**: `number` = `0`

#### Defined in

packages/dev/core/src/Rendering/depthPeelingRenderer.ts:62

___

### \_depthMrts

• `Private` **\_depthMrts**: [`MultiRenderTarget`](MultiRenderTarget.md)[]

#### Defined in

packages/dev/core/src/Rendering/depthPeelingRenderer.ts:52

___

### \_effectRenderer

• `Private` **\_effectRenderer**: [`EffectRenderer`](EffectRenderer.md)

#### Defined in

packages/dev/core/src/Rendering/depthPeelingRenderer.ts:60

___

### \_engine

• `Private` **\_engine**: [`Engine`](Engine.md)

#### Defined in

packages/dev/core/src/Rendering/depthPeelingRenderer.ts:51

___

### \_excludedSubMeshes

• `Private` **\_excludedSubMeshes**: [`SmartArray`](SmartArray.md)[`SubMesh`](SubMesh.md)

#### Defined in

packages/dev/core/src/Rendering/depthPeelingRenderer.ts:70

___

### \_finalEffectWrapper

• `Private` **\_finalEffectWrapper**: [`EffectWrapper`](EffectWrapper.md)

#### Defined in

packages/dev/core/src/Rendering/depthPeelingRenderer.ts:59

___

### \_layoutCache

• `Private` **\_layoutCache**: `number`[][] = `[]`

#### Defined in

packages/dev/core/src/Rendering/depthPeelingRenderer.ts:67

___

### \_layoutCacheFormat

• `Private` **\_layoutCacheFormat**: `boolean`[][]

#### Defined in

packages/dev/core/src/Rendering/depthPeelingRenderer.ts:66

___

### \_passCount

• `Private` **\_passCount**: `number`

#### Defined in

packages/dev/core/src/Rendering/depthPeelingRenderer.ts:82

___

### \_prePassEffectConfiguration

• `Private` **\_prePassEffectConfiguration**: `DepthPeelingEffectConfiguration`

#### Defined in

packages/dev/core/src/Rendering/depthPeelingRenderer.ts:63

___

### \_renderPassIds

• `Private` **\_renderPassIds**: `number`[]

#### Defined in

packages/dev/core/src/Rendering/depthPeelingRenderer.ts:68

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/Rendering/depthPeelingRenderer.ts:50

___

### \_thinTextures

• `Private` **\_thinTextures**: [`ThinTexture`](ThinTexture.md)[] = `[]`

#### Defined in

packages/dev/core/src/Rendering/depthPeelingRenderer.ts:53

___

### \_useRenderPasses

• `Private` **\_useRenderPasses**: `boolean`

#### Defined in

packages/dev/core/src/Rendering/depthPeelingRenderer.ts:98

___

### \_DEPTH\_CLEAR\_VALUE

▪ `Static` `Private` **\_DEPTH\_CLEAR\_VALUE**: `number` = `-99999.0`

#### Defined in

packages/dev/core/src/Rendering/depthPeelingRenderer.ts:72

___

### \_MAX\_DEPTH

▪ `Static` `Private` **\_MAX\_DEPTH**: `number` = `1`

#### Defined in

packages/dev/core/src/Rendering/depthPeelingRenderer.ts:74

___

### \_MIN\_DEPTH

▪ `Static` `Private` **\_MIN\_DEPTH**: `number` = `0`

#### Defined in

packages/dev/core/src/Rendering/depthPeelingRenderer.ts:73

## Accessors

### passCount

• `get` **passCount**(): `number`

Number of depth peeling passes. As we are using dual depth peeling, each pass two levels of transparency are processed.

#### Returns

`number`

#### Defined in

packages/dev/core/src/Rendering/depthPeelingRenderer.ts:86

• `set` **passCount**(`count`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `count` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Rendering/depthPeelingRenderer.ts:90

___

### useRenderPasses

• `get` **useRenderPasses**(): `boolean`

Instructs the renderer to use render passes. It is an optimization that makes the rendering faster for some engines (like WebGPU) but that consumes more memory, so it is disabled by default.

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Rendering/depthPeelingRenderer.ts:102

• `set` **useRenderPasses**(`usePasses`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `usePasses` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Rendering/depthPeelingRenderer.ts:106

## Methods

### \_createEffects

▸ `Private` **_createEffects**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Rendering/depthPeelingRenderer.ts:264

___

### \_createRenderPassIds

▸ `Private` **_createRenderPassIds**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Rendering/depthPeelingRenderer.ts:143

___

### \_createTextures

▸ `Private` **_createTextures**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Rendering/depthPeelingRenderer.ts:161

___

### \_disposeTextures

▸ `Private` **_disposeTextures**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Rendering/depthPeelingRenderer.ts:206

___

### \_finalCompose

▸ `Private` **_finalCompose**(`writeId`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `writeId` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Rendering/depthPeelingRenderer.ts:355

___

### \_releaseRenderPassIds

▸ `Private` **_releaseRenderPassIds**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Rendering/depthPeelingRenderer.ts:154

___

### \_renderSubMeshes

▸ `Private` **_renderSubMeshes**(`transparentSubMeshes`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `transparentSubMeshes` | [`SmartArray`](SmartArray.md)[`SubMesh`](SubMesh.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Rendering/depthPeelingRenderer.ts:308

___

### \_updateTextureReferences

▸ `Private` **_updateTextureReferences**(): `boolean`

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Rendering/depthPeelingRenderer.ts:234

___

### \_updateTextures

▸ `Private` **_updateTextures**(): `boolean`

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Rendering/depthPeelingRenderer.ts:226

___

### bind

▸ **bind**(`effect`): `void`

Binds depth peeling textures on an effect

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `effect` | [`Effect`](Effect.md) | The effect to bind textures on |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Rendering/depthPeelingRenderer.ts:303

___

### dispose

▸ **dispose**(): `void`

Disposes the depth peeling renderer and associated ressources

#### Returns

`void`

#### Defined in

packages/dev/core/src/Rendering/depthPeelingRenderer.ts:506

___

### render

▸ **render**(`transparentSubMeshes`): [`SmartArray`](SmartArray.md)[`SubMesh`](SubMesh.md)

Renders transparent submeshes with depth peeling

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `transparentSubMeshes` | [`SmartArray`](SmartArray.md)[`SubMesh`](SubMesh.md) | List of transparent meshes to render |

#### Returns

[`SmartArray`](SmartArray.md)[`SubMesh`](SubMesh.md)

The array of submeshes that could not be handled by this renderer

#### Defined in

packages/dev/core/src/Rendering/depthPeelingRenderer.ts:372

___

### setPrePassRenderer

▸ **setPrePassRenderer**(`prePassRenderer`): `void`

Links to the prepass renderer

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `prePassRenderer` | [`PrePassRenderer`](PrePassRenderer.md) | The scene PrePassRenderer |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Rendering/depthPeelingRenderer.ts:295
