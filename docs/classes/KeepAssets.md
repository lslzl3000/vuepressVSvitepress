[@dev/core](../README.md) / [Exports](../modules.md) / KeepAssets

# Class: KeepAssets

Set of assets to keep when moving a scene into an asset container.

## Hierarchy

- [`AbstractScene`](AbstractScene.md)

  ↳ **`KeepAssets`**

## Table of contents

### Constructors

- [constructor](KeepAssets.md#constructor)

### Properties

- [actionManagers](KeepAssets.md#actionmanagers)
- [animationGroups](KeepAssets.md#animationgroups)
- [animations](KeepAssets.md#animations)
- [cameras](KeepAssets.md#cameras)
- [effectLayers](KeepAssets.md#effectlayers)
- [geometries](KeepAssets.md#geometries)
- [layers](KeepAssets.md#layers)
- [lensFlareSystems](KeepAssets.md#lensflaresystems)
- [lights](KeepAssets.md#lights)
- [materials](KeepAssets.md#materials)
- [meshes](KeepAssets.md#meshes)
- [morphTargetManagers](KeepAssets.md#morphtargetmanagers)
- [multiMaterials](KeepAssets.md#multimaterials)
- [particleSystems](KeepAssets.md#particlesystems)
- [postProcesses](KeepAssets.md#postprocesses)
- [prePassRenderer](KeepAssets.md#prepassrenderer)
- [proceduralTextures](KeepAssets.md#proceduraltextures)
- [reflectionProbes](KeepAssets.md#reflectionprobes)
- [rootNodes](KeepAssets.md#rootnodes)
- [skeletons](KeepAssets.md#skeletons)
- [sounds](KeepAssets.md#sounds)
- [subSurfaceConfiguration](KeepAssets.md#subsurfaceconfiguration)
- [textures](KeepAssets.md#textures)
- [transformNodes](KeepAssets.md#transformnodes)

### Accessors

- [environmentTexture](KeepAssets.md#environmenttexture)

### Methods

- [addEffectLayer](KeepAssets.md#addeffectlayer)
- [addLensFlareSystem](KeepAssets.md#addlensflaresystem)
- [addReflectionProbe](KeepAssets.md#addreflectionprobe)
- [disablePrePassRenderer](KeepAssets.md#disableprepassrenderer)
- [disableSubSurfaceForPrePass](KeepAssets.md#disablesubsurfaceforprepass)
- [enablePrePassRenderer](KeepAssets.md#enableprepassrenderer)
- [enableSubSurfaceForPrePass](KeepAssets.md#enablesubsurfaceforprepass)
- [getGlowLayerByName](KeepAssets.md#getglowlayerbyname)
- [getHighlightLayerByName](KeepAssets.md#gethighlightlayerbyname)
- [getLensFlareSystemByID](KeepAssets.md#getlensflaresystembyid)
- [getLensFlareSystemById](KeepAssets.md#getlensflaresystembyid-1)
- [getLensFlareSystemByName](KeepAssets.md#getlensflaresystembyname)
- [getNodes](KeepAssets.md#getnodes)
- [removeEffectLayer](KeepAssets.md#removeeffectlayer)
- [removeLensFlareSystem](KeepAssets.md#removelensflaresystem)
- [removeReflectionProbe](KeepAssets.md#removereflectionprobe)
- [AddIndividualParser](KeepAssets.md#addindividualparser)
- [AddParser](KeepAssets.md#addparser)
- [GetIndividualParser](KeepAssets.md#getindividualparser)
- [GetParser](KeepAssets.md#getparser)
- [Parse](KeepAssets.md#parse)

## Constructors

### constructor

• **new KeepAssets**()

#### Inherited from

[AbstractScene](AbstractScene.md).[constructor](AbstractScene.md#constructor)

## Properties

### actionManagers

• **actionManagers**: [`AbstractActionManager`](AbstractActionManager.md)[]

ActionManagers available on the scene.

**`Deprecated`**

#### Inherited from

[AbstractScene](AbstractScene.md).[actionManagers](AbstractScene.md#actionmanagers)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:192

___

### animationGroups

• **animationGroups**: [`AnimationGroup`](AnimationGroup.md)[]

All of the animation groups added to this scene

**`See`**

https://doc.babylonjs.com/divingDeeper/animation/groupAnimations

#### Inherited from

[AbstractScene](AbstractScene.md).[animationGroups](AbstractScene.md#animationgroups)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:151

___

### animations

• **animations**: [`Animation`](Animation.md)[] = `[]`

Gets a list of Animations associated with the scene

#### Inherited from

[AbstractScene](AbstractScene.md).[animations](AbstractScene.md#animations)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:145

___

### cameras

• **cameras**: [`Camera`](Camera.md)[]

All of the cameras added to this scene

**`See`**

https://doc.babylonjs.com/babylon101/cameras

#### Inherited from

[AbstractScene](AbstractScene.md).[cameras](AbstractScene.md#cameras)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:117

___

### effectLayers

• **effectLayers**: [`EffectLayer`](EffectLayer.md)[]

The list of effect layers (highlights/glow) added to the scene

**`See`**

 - https://doc.babylonjs.com/how_to/highlight_layer
 - https://doc.babylonjs.com/how_to/glow_layer

#### Inherited from

[AbstractScene](AbstractScene.md).[effectLayers](AbstractScene.md#effectlayers)

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayerSceneComponent.ts:33

___

### geometries

• **geometries**: [`Geometry`](Geometry.md)[]

The list of geometries used in the scene.

#### Inherited from

[AbstractScene](AbstractScene.md).[geometries](AbstractScene.md#geometries)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:177

___

### layers

• **layers**: [`Layer`](Layer.md)[]

The list of layers (background and foreground) of the scene

#### Inherited from

[AbstractScene](AbstractScene.md).[layers](AbstractScene.md#layers)

#### Defined in

https://github.com/babylon.js/core/src/Layers/layerSceneComponent.ts:16

___

### lensFlareSystems

• **lensFlareSystems**: [`LensFlareSystem`](LensFlareSystem.md)[]

The list of lens flare system added to the scene

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_lens_flares

#### Inherited from

[AbstractScene](AbstractScene.md).[lensFlareSystems](AbstractScene.md#lensflaresystems)

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlareSystemSceneComponent.ts:32

___

### lights

• **lights**: [`Light`](Light.md)[]

All of the lights added to this scene

**`See`**

https://doc.babylonjs.com/babylon101/lights

#### Inherited from

[AbstractScene](AbstractScene.md).[lights](AbstractScene.md#lights)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:123

___

### materials

• **materials**: [`Material`](Material.md)[]

All of the materials added to this scene
In the context of a Scene, it is not supposed to be modified manually.
Any addition or removal should be done using the addMaterial and removeMaterial Scene methods.
Note also that the order of the Material within the array is not significant and might change.

**`See`**

https://doc.babylonjs.com/babylon101/materials

#### Inherited from

[AbstractScene](AbstractScene.md).[materials](AbstractScene.md#materials)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:166

___

### meshes

• **meshes**: [`AbstractMesh`](AbstractMesh.md)[]

All of the (abstract) meshes added to this scene

#### Inherited from

[AbstractScene](AbstractScene.md).[meshes](AbstractScene.md#meshes)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:128

___

### morphTargetManagers

• **morphTargetManagers**: [`MorphTargetManager`](MorphTargetManager.md)[]

The list of morph target managers added to the scene

**`See`**

https://doc.babylonjs.com/how_to/how_to_dynamically_morph_a_mesh

#### Inherited from

[AbstractScene](AbstractScene.md).[morphTargetManagers](AbstractScene.md#morphtargetmanagers)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:172

___

### multiMaterials

• **multiMaterials**: [`MultiMaterial`](MultiMaterial.md)[]

All of the multi-materials added to this scene

**`See`**

https://doc.babylonjs.com/how_to/multi_materials

#### Inherited from

[AbstractScene](AbstractScene.md).[multiMaterials](AbstractScene.md#multimaterials)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:157

___

### particleSystems

• **particleSystems**: [`IParticleSystem`](../interfaces/IParticleSystem.md)[]

All of the particle systems added to this scene

**`See`**

https://doc.babylonjs.com/babylon101/particles

#### Inherited from

[AbstractScene](AbstractScene.md).[particleSystems](AbstractScene.md#particlesystems)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:140

___

### postProcesses

• **postProcesses**: [`PostProcess`](PostProcess.md)[]

The list of postprocesses added to the scene

#### Inherited from

[AbstractScene](AbstractScene.md).[postProcesses](AbstractScene.md#postprocesses)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:217

___

### prePassRenderer

• **prePassRenderer**: [`Nullable`](../modules.md#nullable)[`PrePassRenderer`](PrePassRenderer.md)

Gets or Sets the current prepass renderer associated to the scene.

#### Inherited from

[AbstractScene](AbstractScene.md).[prePassRenderer](AbstractScene.md#prepassrenderer)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRendererSceneComponent.ts:23

___

### proceduralTextures

• **proceduralTextures**: [`ProceduralTexture`](ProceduralTexture.md)[]

The list of procedural textures added to the scene

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_procedural_textures

#### Inherited from

[AbstractScene](AbstractScene.md).[proceduralTextures](AbstractScene.md#proceduraltextures)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTextureSceneComponent.ts:14

___

### reflectionProbes

• **reflectionProbes**: [`ReflectionProbe`](ReflectionProbe.md)[]

The list of reflection probes added to the scene

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_reflection_probes

#### Inherited from

[AbstractScene](AbstractScene.md).[reflectionProbes](AbstractScene.md#reflectionprobes)

#### Defined in

https://github.com/babylon.js/core/src/Probes/reflectionProbe.ts:17

___

### rootNodes

• **rootNodes**: [`Node`](Node.md)[]

Gets the list of root nodes (ie. nodes with no parent)

#### Inherited from

[AbstractScene](AbstractScene.md).[rootNodes](AbstractScene.md#rootnodes)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:112

___

### skeletons

• **skeletons**: [`Skeleton`](Skeleton.md)[]

The list of skeletons added to the scene

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_bones_and_skeletons

#### Inherited from

[AbstractScene](AbstractScene.md).[skeletons](AbstractScene.md#skeletons)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:134

___

### sounds

• **sounds**: [`Nullable`](../modules.md#nullable)[`Sound`](Sound.md)[]

The list of sounds used in the scene.

#### Inherited from

[AbstractScene](AbstractScene.md).[sounds](AbstractScene.md#sounds)

#### Defined in

https://github.com/babylon.js/core/src/Audio/audioSceneComponent.ts:51

___

### subSurfaceConfiguration

• **subSurfaceConfiguration**: [`Nullable`](../modules.md#nullable)`SubSurfaceConfiguration`

Gets or Sets the current prepass renderer associated to the scene.

#### Inherited from

[AbstractScene](AbstractScene.md).[subSurfaceConfiguration](AbstractScene.md#subsurfaceconfiguration)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/subSurfaceSceneComponent.ts:31

___

### textures

• **textures**: [`BaseTexture`](BaseTexture.md)[]

Textures to keep.

#### Inherited from

[AbstractScene](AbstractScene.md).[textures](AbstractScene.md#textures)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:197

___

### transformNodes

• **transformNodes**: [`TransformNode`](TransformNode.md)[]

All of the transform nodes added to this scene
In the context of a Scene, it is not supposed to be modified manually.
Any addition or removal should be done using the addTransformNode and removeTransformNode Scene methods.
Note also that the order of the TransformNode within the array is not significant and might change.

**`See`**

https://doc.babylonjs.com/how_to/transformnode

#### Inherited from

[AbstractScene](AbstractScene.md).[transformNodes](AbstractScene.md#transformnodes)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:186

## Accessors

### environmentTexture

• `get` **environmentTexture**(): [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Texture used in all pbr material as the reflection texture.
As in the majority of the scene they are the same (exception for multi room and so on),
this is easier to reference from here than from all the materials.

#### Returns

[`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

#### Inherited from

AbstractScene.environmentTexture

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:206

• `set` **environmentTexture**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) |

#### Returns

`void`

#### Inherited from

AbstractScene.environmentTexture

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:210

## Methods

### addEffectLayer

▸ **addEffectLayer**(`newEffectLayer`): `void`

Adds the given effect layer to this scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newEffectLayer` | [`EffectLayer`](EffectLayer.md) | defines the effect layer to add |

#### Returns

`void`

#### Inherited from

[AbstractScene](AbstractScene.md).[addEffectLayer](AbstractScene.md#addeffectlayer)

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayerSceneComponent.ts:46

___

### addLensFlareSystem

▸ **addLensFlareSystem**(`newLensFlareSystem`): `void`

Adds the given lens flare system to this scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newLensFlareSystem` | [`LensFlareSystem`](LensFlareSystem.md) | The lens flare system to add |

#### Returns

`void`

#### Inherited from

[AbstractScene](AbstractScene.md).[addLensFlareSystem](AbstractScene.md#addlensflaresystem)

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlareSystemSceneComponent.ts:45

___

### addReflectionProbe

▸ **addReflectionProbe**(`newReflectionProbe`): `void`

Adds the given reflection probe to this scene.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newReflectionProbe` | [`ReflectionProbe`](ReflectionProbe.md) | The reflection probe to add |

#### Returns

`void`

#### Inherited from

[AbstractScene](AbstractScene.md).[addReflectionProbe](AbstractScene.md#addreflectionprobe)

#### Defined in

https://github.com/babylon.js/core/src/Probes/reflectionProbe.ts:30

___

### disablePrePassRenderer

▸ **disablePrePassRenderer**(): `void`

Disables the prepass associated with the scene

#### Returns

`void`

#### Inherited from

[AbstractScene](AbstractScene.md).[disablePrePassRenderer](AbstractScene.md#disableprepassrenderer)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRendererSceneComponent.ts:34

___

### disableSubSurfaceForPrePass

▸ **disableSubSurfaceForPrePass**(): `void`

Disables the subsurface effect for prepass

#### Returns

`void`

#### Inherited from

[AbstractScene](AbstractScene.md).[disableSubSurfaceForPrePass](AbstractScene.md#disablesubsurfaceforprepass)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/subSurfaceSceneComponent.ts:42

___

### enablePrePassRenderer

▸ **enablePrePassRenderer**(): [`Nullable`](../modules.md#nullable)[`PrePassRenderer`](PrePassRenderer.md)

Enables the prepass and associates it with the scene

#### Returns

[`Nullable`](../modules.md#nullable)[`PrePassRenderer`](PrePassRenderer.md)

the PrePassRenderer

#### Inherited from

[AbstractScene](AbstractScene.md).[enablePrePassRenderer](AbstractScene.md#enableprepassrenderer)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRendererSceneComponent.ts:29

___

### enableSubSurfaceForPrePass

▸ **enableSubSurfaceForPrePass**(): [`Nullable`](../modules.md#nullable)`SubSurfaceConfiguration`

Enables the subsurface effect for prepass

#### Returns

[`Nullable`](../modules.md#nullable)`SubSurfaceConfiguration`

the SubSurfaceConfiguration

#### Inherited from

[AbstractScene](AbstractScene.md).[enableSubSurfaceForPrePass](AbstractScene.md#enablesubsurfaceforprepass)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/subSurfaceSceneComponent.ts:37

___

### getGlowLayerByName

▸ **getGlowLayerByName**(`name`): [`Nullable`](../modules.md#nullable)[`GlowLayer`](GlowLayer.md)

Return a the first highlight layer of the scene with a given name.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | The name of the highlight layer to look for. |

#### Returns

[`Nullable`](../modules.md#nullable)[`GlowLayer`](GlowLayer.md)

The highlight layer if found otherwise null.

#### Inherited from

[AbstractScene](AbstractScene.md).[getGlowLayerByName](AbstractScene.md#getglowlayerbyname)

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:36

___

### getHighlightLayerByName

▸ **getHighlightLayerByName**(`name`): [`Nullable`](../modules.md#nullable)[`HighlightLayer`](HighlightLayer.md)

Return a the first highlight layer of the scene with a given name.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | The name of the highlight layer to look for. |

#### Returns

[`Nullable`](../modules.md#nullable)[`HighlightLayer`](HighlightLayer.md)

The highlight layer if found otherwise null.

#### Inherited from

[AbstractScene](AbstractScene.md).[getHighlightLayerByName](AbstractScene.md#gethighlightlayerbyname)

#### Defined in

https://github.com/babylon.js/core/src/Layers/highlightLayer.ts:41

___

### getLensFlareSystemByID

▸ **getLensFlareSystemByID**(`id`): [`Nullable`](../modules.md#nullable)[`LensFlareSystem`](LensFlareSystem.md)

Gets a lens flare system using its Id

**`Deprecated`**

Please use getLensFlareSystemById instead

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | defines the Id to look for |

#### Returns

[`Nullable`](../modules.md#nullable)[`LensFlareSystem`](LensFlareSystem.md)

the lens flare system or null if not found

#### Inherited from

[AbstractScene](AbstractScene.md).[getLensFlareSystemByID](AbstractScene.md#getlensflaresystembyid)

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlareSystemSceneComponent.ts:60

___

### getLensFlareSystemById

▸ **getLensFlareSystemById**(`id`): [`Nullable`](../modules.md#nullable)[`LensFlareSystem`](LensFlareSystem.md)

Gets a lens flare system using its Id

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | defines the Id to look for |

#### Returns

[`Nullable`](../modules.md#nullable)[`LensFlareSystem`](LensFlareSystem.md)

the lens flare system or null if not found

#### Inherited from

[AbstractScene](AbstractScene.md).[getLensFlareSystemById](AbstractScene.md#getlensflaresystembyid-1)

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlareSystemSceneComponent.ts:67

___

### getLensFlareSystemByName

▸ **getLensFlareSystemByName**(`name`): [`Nullable`](../modules.md#nullable)[`LensFlareSystem`](LensFlareSystem.md)

Gets a lens flare system using its name

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the name to look for |

#### Returns

[`Nullable`](../modules.md#nullable)[`LensFlareSystem`](LensFlareSystem.md)

the lens flare system or null if not found

#### Inherited from

[AbstractScene](AbstractScene.md).[getLensFlareSystemByName](AbstractScene.md#getlensflaresystembyname)

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlareSystemSceneComponent.ts:52

___

### getNodes

▸ **getNodes**(): [`Node`](Node.md)[]

#### Returns

[`Node`](Node.md)[]

all meshes, lights, cameras, transformNodes and bones

#### Inherited from

[AbstractScene](AbstractScene.md).[getNodes](AbstractScene.md#getnodes)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:222

___

### removeEffectLayer

▸ **removeEffectLayer**(`toRemove`): `number`

Removes the given effect layer from this scene.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `toRemove` | [`EffectLayer`](EffectLayer.md) | defines the effect layer to remove |

#### Returns

`number`

the index of the removed effect layer

#### Inherited from

[AbstractScene](AbstractScene.md).[removeEffectLayer](AbstractScene.md#removeeffectlayer)

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayerSceneComponent.ts:40

___

### removeLensFlareSystem

▸ **removeLensFlareSystem**(`toRemove`): `number`

Removes the given lens flare system from this scene.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `toRemove` | [`LensFlareSystem`](LensFlareSystem.md) | The lens flare system to remove |

#### Returns

`number`

The index of the removed lens flare system

#### Inherited from

[AbstractScene](AbstractScene.md).[removeLensFlareSystem](AbstractScene.md#removelensflaresystem)

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlareSystemSceneComponent.ts:39

___

### removeReflectionProbe

▸ **removeReflectionProbe**(`toRemove`): `number`

Removes the given reflection probe from this scene.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `toRemove` | [`ReflectionProbe`](ReflectionProbe.md) | The reflection probe to remove |

#### Returns

`number`

The index of the removed reflection probe

#### Inherited from

[AbstractScene](AbstractScene.md).[removeReflectionProbe](AbstractScene.md#removereflectionprobe)

#### Defined in

https://github.com/babylon.js/core/src/Probes/reflectionProbe.ts:24

___

### AddIndividualParser

▸ `Static` **AddIndividualParser**(`name`, `parser`): `void`

Adds n individual parser in the list of available ones

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Defines the name of the parser |
| `parser` | [`IndividualBabylonFileParser`](../modules.md#individualbabylonfileparser) | Defines the parser to add |

#### Returns

`void`

#### Inherited from

[AbstractScene](AbstractScene.md).[AddIndividualParser](AbstractScene.md#addindividualparser)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:77

___

### AddParser

▸ `Static` **AddParser**(`name`, `parser`): `void`

Adds a parser in the list of available ones

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Defines the name of the parser |
| `parser` | [`BabylonFileParser`](../modules.md#babylonfileparser) | Defines the parser to add |

#### Returns

`void`

#### Inherited from

[AbstractScene](AbstractScene.md).[AddParser](AbstractScene.md#addparser)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:55

___

### GetIndividualParser

▸ `Static` **GetIndividualParser**(`name`): [`Nullable`](../modules.md#nullable)[`IndividualBabylonFileParser`](../modules.md#individualbabylonfileparser)

Gets an individual parser from the list of available ones

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Defines the name of the parser |

#### Returns

[`Nullable`](../modules.md#nullable)[`IndividualBabylonFileParser`](../modules.md#individualbabylonfileparser)

the requested parser or null

#### Inherited from

[AbstractScene](AbstractScene.md).[GetIndividualParser](AbstractScene.md#getindividualparser)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:86

___

### GetParser

▸ `Static` **GetParser**(`name`): [`Nullable`](../modules.md#nullable)[`BabylonFileParser`](../modules.md#babylonfileparser)

Gets a general parser from the list of available ones

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Defines the name of the parser |

#### Returns

[`Nullable`](../modules.md#nullable)[`BabylonFileParser`](../modules.md#babylonfileparser)

the requested parser or null

#### Inherited from

[AbstractScene](AbstractScene.md).[GetParser](AbstractScene.md#getparser)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:64

___

### Parse

▸ `Static` **Parse**(`jsonData`, `scene`, `container`, `rootUrl`): `void`

Parser json data and populate both a scene and its associated container object

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `jsonData` | `any` | Defines the data to parse |
| `scene` | [`Scene`](Scene.md) | Defines the scene to parse the data for |
| `container` | [`AssetContainer`](AssetContainer.md) | Defines the container attached to the parsing sequence |
| `rootUrl` | `string` | Defines the root url of the data |

#### Returns

`void`

#### Inherited from

[AbstractScene](AbstractScene.md).[Parse](AbstractScene.md#parse)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:101
