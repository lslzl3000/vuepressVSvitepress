[@dev/core](../README.md) / [Exports](../modules.md) / AbstractScene

# Class: AbstractScene

Base class of the scene acting as a container for the different elements composing a scene.
This class is dynamically extended by the different components of the scene increasing
flexibility and reducing coupling

## Hierarchy

- **`AbstractScene`**

  ↳ [`KeepAssets`](KeepAssets.md)

  ↳ [`AssetContainer`](AssetContainer.md)

  ↳ [`Scene`](Scene.md)

## Table of contents

### Constructors

- [constructor](AbstractScene.md#constructor)

### Properties

- [actionManagers](AbstractScene.md#actionmanagers)
- [animationGroups](AbstractScene.md#animationgroups)
- [animations](AbstractScene.md#animations)
- [cameras](AbstractScene.md#cameras)
- [effectLayers](AbstractScene.md#effectlayers)
- [geometries](AbstractScene.md#geometries)
- [layers](AbstractScene.md#layers)
- [lensFlareSystems](AbstractScene.md#lensflaresystems)
- [lights](AbstractScene.md#lights)
- [materials](AbstractScene.md#materials)
- [meshes](AbstractScene.md#meshes)
- [morphTargetManagers](AbstractScene.md#morphtargetmanagers)
- [multiMaterials](AbstractScene.md#multimaterials)
- [particleSystems](AbstractScene.md#particlesystems)
- [postProcesses](AbstractScene.md#postprocesses)
- [prePassRenderer](AbstractScene.md#prepassrenderer)
- [proceduralTextures](AbstractScene.md#proceduraltextures)
- [reflectionProbes](AbstractScene.md#reflectionprobes)
- [rootNodes](AbstractScene.md#rootnodes)
- [skeletons](AbstractScene.md#skeletons)
- [sounds](AbstractScene.md#sounds)
- [subSurfaceConfiguration](AbstractScene.md#subsurfaceconfiguration)
- [textures](AbstractScene.md#textures)
- [transformNodes](AbstractScene.md#transformnodes)
- [\_BabylonFileParsers](AbstractScene.md#_babylonfileparsers)
- [\_IndividualBabylonFileParsers](AbstractScene.md#_individualbabylonfileparsers)

### Accessors

- [environmentTexture](AbstractScene.md#environmenttexture)

### Methods

- [addEffectLayer](AbstractScene.md#addeffectlayer)
- [addLensFlareSystem](AbstractScene.md#addlensflaresystem)
- [addReflectionProbe](AbstractScene.md#addreflectionprobe)
- [disablePrePassRenderer](AbstractScene.md#disableprepassrenderer)
- [disableSubSurfaceForPrePass](AbstractScene.md#disablesubsurfaceforprepass)
- [enablePrePassRenderer](AbstractScene.md#enableprepassrenderer)
- [enableSubSurfaceForPrePass](AbstractScene.md#enablesubsurfaceforprepass)
- [getGlowLayerByName](AbstractScene.md#getglowlayerbyname)
- [getHighlightLayerByName](AbstractScene.md#gethighlightlayerbyname)
- [getLensFlareSystemByID](AbstractScene.md#getlensflaresystembyid)
- [getLensFlareSystemById](AbstractScene.md#getlensflaresystembyid-1)
- [getLensFlareSystemByName](AbstractScene.md#getlensflaresystembyname)
- [getNodes](AbstractScene.md#getnodes)
- [removeEffectLayer](AbstractScene.md#removeeffectlayer)
- [removeLensFlareSystem](AbstractScene.md#removelensflaresystem)
- [removeReflectionProbe](AbstractScene.md#removereflectionprobe)
- [AddIndividualParser](AbstractScene.md#addindividualparser)
- [AddParser](AbstractScene.md#addparser)
- [GetIndividualParser](AbstractScene.md#getindividualparser)
- [GetParser](AbstractScene.md#getparser)
- [Parse](AbstractScene.md#parse)

## Constructors

### constructor

• **new AbstractScene**()

## Properties

### actionManagers

• **actionManagers**: [`AbstractActionManager`](AbstractActionManager.md)[]

ActionManagers available on the scene.

**`Deprecated`**

#### Defined in

packages/dev/core/src/abstractScene.ts:192

___

### animationGroups

• **animationGroups**: [`AnimationGroup`](AnimationGroup.md)[]

All of the animation groups added to this scene

**`See`**

https://doc.babylonjs.com/divingDeeper/animation/groupAnimations

#### Defined in

packages/dev/core/src/abstractScene.ts:151

___

### animations

• **animations**: [`Animation`](Animation.md)[] = `[]`

Gets a list of Animations associated with the scene

#### Defined in

packages/dev/core/src/abstractScene.ts:145

___

### cameras

• **cameras**: [`Camera`](Camera.md)[]

All of the cameras added to this scene

**`See`**

https://doc.babylonjs.com/babylon101/cameras

#### Defined in

packages/dev/core/src/abstractScene.ts:117

___

### effectLayers

• **effectLayers**: [`EffectLayer`](EffectLayer.md)[]

The list of effect layers (highlights/glow) added to the scene

**`See`**

 - https://doc.babylonjs.com/how_to/highlight_layer
 - https://doc.babylonjs.com/how_to/glow_layer

#### Defined in

packages/dev/core/src/Layers/effectLayerSceneComponent.ts:33

___

### geometries

• **geometries**: [`Geometry`](Geometry.md)[]

The list of geometries used in the scene.

#### Defined in

packages/dev/core/src/abstractScene.ts:177

___

### layers

• **layers**: [`Layer`](Layer.md)[]

The list of layers (background and foreground) of the scene

#### Defined in

packages/dev/core/src/Layers/layerSceneComponent.ts:16

___

### lensFlareSystems

• **lensFlareSystems**: [`LensFlareSystem`](LensFlareSystem.md)[]

The list of lens flare system added to the scene

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_lens_flares

#### Defined in

packages/dev/core/src/LensFlares/lensFlareSystemSceneComponent.ts:32

___

### lights

• **lights**: [`Light`](Light.md)[]

All of the lights added to this scene

**`See`**

https://doc.babylonjs.com/babylon101/lights

#### Defined in

packages/dev/core/src/abstractScene.ts:123

___

### materials

• **materials**: [`Material`](Material.md)[]

All of the materials added to this scene
In the context of a Scene, it is not supposed to be modified manually.
Any addition or removal should be done using the addMaterial and removeMaterial Scene methods.
Note also that the order of the Material within the array is not significant and might change.

**`See`**

https://doc.babylonjs.com/babylon101/materials

#### Defined in

packages/dev/core/src/abstractScene.ts:166

___

### meshes

• **meshes**: [`AbstractMesh`](AbstractMesh.md)[]

All of the (abstract) meshes added to this scene

#### Defined in

packages/dev/core/src/abstractScene.ts:128

___

### morphTargetManagers

• **morphTargetManagers**: [`MorphTargetManager`](MorphTargetManager.md)[]

The list of morph target managers added to the scene

**`See`**

https://doc.babylonjs.com/how_to/how_to_dynamically_morph_a_mesh

#### Defined in

packages/dev/core/src/abstractScene.ts:172

___

### multiMaterials

• **multiMaterials**: [`MultiMaterial`](MultiMaterial.md)[]

All of the multi-materials added to this scene

**`See`**

https://doc.babylonjs.com/how_to/multi_materials

#### Defined in

packages/dev/core/src/abstractScene.ts:157

___

### particleSystems

• **particleSystems**: [`IParticleSystem`](../interfaces/IParticleSystem.md)[]

All of the particle systems added to this scene

**`See`**

https://doc.babylonjs.com/babylon101/particles

#### Defined in

packages/dev/core/src/abstractScene.ts:140

___

### postProcesses

• **postProcesses**: [`PostProcess`](PostProcess.md)[]

The list of postprocesses added to the scene

#### Defined in

packages/dev/core/src/abstractScene.ts:217

___

### prePassRenderer

• **prePassRenderer**: [`Nullable`](../modules.md#nullable)[`PrePassRenderer`](PrePassRenderer.md)

Gets or Sets the current prepass renderer associated to the scene.

#### Defined in

packages/dev/core/src/Rendering/prePassRendererSceneComponent.ts:23

___

### proceduralTextures

• **proceduralTextures**: [`ProceduralTexture`](ProceduralTexture.md)[]

The list of procedural textures added to the scene

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_procedural_textures

#### Defined in

packages/dev/core/src/Materials/Textures/Procedurals/proceduralTextureSceneComponent.ts:14

___

### reflectionProbes

• **reflectionProbes**: [`ReflectionProbe`](ReflectionProbe.md)[]

The list of reflection probes added to the scene

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_reflection_probes

#### Defined in

packages/dev/core/src/Probes/reflectionProbe.ts:17

___

### rootNodes

• **rootNodes**: [`Node`](Node.md)[]

Gets the list of root nodes (ie. nodes with no parent)

#### Defined in

packages/dev/core/src/abstractScene.ts:112

___

### skeletons

• **skeletons**: [`Skeleton`](Skeleton.md)[]

The list of skeletons added to the scene

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_bones_and_skeletons

#### Defined in

packages/dev/core/src/abstractScene.ts:134

___

### sounds

• **sounds**: [`Nullable`](../modules.md#nullable)[`Sound`](Sound.md)[]

The list of sounds used in the scene.

#### Defined in

packages/dev/core/src/Audio/audioSceneComponent.ts:51

___

### subSurfaceConfiguration

• **subSurfaceConfiguration**: [`Nullable`](../modules.md#nullable)`SubSurfaceConfiguration`

Gets or Sets the current prepass renderer associated to the scene.

#### Defined in

packages/dev/core/src/Rendering/subSurfaceSceneComponent.ts:31

___

### textures

• **textures**: [`BaseTexture`](BaseTexture.md)[]

Textures to keep.

#### Defined in

packages/dev/core/src/abstractScene.ts:197

___

### transformNodes

• **transformNodes**: [`TransformNode`](TransformNode.md)[]

All of the transform nodes added to this scene
In the context of a Scene, it is not supposed to be modified manually.
Any addition or removal should be done using the addTransformNode and removeTransformNode Scene methods.
Note also that the order of the TransformNode within the array is not significant and might change.

**`See`**

https://doc.babylonjs.com/how_to/transformnode

#### Defined in

packages/dev/core/src/abstractScene.ts:186

___

### \_BabylonFileParsers

▪ `Static` `Private` **\_BabylonFileParsers**: `Object` = `{}`

Stores the list of available parsers in the application.

#### Index signature

▪ [key: `string`]: [`BabylonFileParser`](../modules.md#babylonfileparser)

#### Defined in

packages/dev/core/src/abstractScene.ts:43

___

### \_IndividualBabylonFileParsers

▪ `Static` `Private` **\_IndividualBabylonFileParsers**: `Object` = `{}`

Stores the list of available individual parsers in the application.

#### Index signature

▪ [key: `string`]: [`IndividualBabylonFileParser`](../modules.md#individualbabylonfileparser)

#### Defined in

packages/dev/core/src/abstractScene.ts:48

## Accessors

### environmentTexture

• `get` **environmentTexture**(): [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Texture used in all pbr material as the reflection texture.
As in the majority of the scene they are the same (exception for multi room and so on),
this is easier to reference from here than from all the materials.

#### Returns

[`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

#### Defined in

packages/dev/core/src/abstractScene.ts:206

• `set` **environmentTexture**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/abstractScene.ts:210

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

#### Defined in

packages/dev/core/src/Layers/effectLayerSceneComponent.ts:46

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

#### Defined in

packages/dev/core/src/LensFlares/lensFlareSystemSceneComponent.ts:45

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

#### Defined in

packages/dev/core/src/Probes/reflectionProbe.ts:30

___

### disablePrePassRenderer

▸ **disablePrePassRenderer**(): `void`

Disables the prepass associated with the scene

#### Returns

`void`

#### Defined in

packages/dev/core/src/Rendering/prePassRendererSceneComponent.ts:34

___

### disableSubSurfaceForPrePass

▸ **disableSubSurfaceForPrePass**(): `void`

Disables the subsurface effect for prepass

#### Returns

`void`

#### Defined in

packages/dev/core/src/Rendering/subSurfaceSceneComponent.ts:42

___

### enablePrePassRenderer

▸ **enablePrePassRenderer**(): [`Nullable`](../modules.md#nullable)[`PrePassRenderer`](PrePassRenderer.md)

Enables the prepass and associates it with the scene

#### Returns

[`Nullable`](../modules.md#nullable)[`PrePassRenderer`](PrePassRenderer.md)

the PrePassRenderer

#### Defined in

packages/dev/core/src/Rendering/prePassRendererSceneComponent.ts:29

___

### enableSubSurfaceForPrePass

▸ **enableSubSurfaceForPrePass**(): [`Nullable`](../modules.md#nullable)`SubSurfaceConfiguration`

Enables the subsurface effect for prepass

#### Returns

[`Nullable`](../modules.md#nullable)`SubSurfaceConfiguration`

the SubSurfaceConfiguration

#### Defined in

packages/dev/core/src/Rendering/subSurfaceSceneComponent.ts:37

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

#### Defined in

packages/dev/core/src/Layers/glowLayer.ts:36

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

#### Defined in

packages/dev/core/src/Layers/highlightLayer.ts:41

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

#### Defined in

packages/dev/core/src/LensFlares/lensFlareSystemSceneComponent.ts:60

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

#### Defined in

packages/dev/core/src/LensFlares/lensFlareSystemSceneComponent.ts:67

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

#### Defined in

packages/dev/core/src/LensFlares/lensFlareSystemSceneComponent.ts:52

___

### getNodes

▸ **getNodes**(): [`Node`](Node.md)[]

#### Returns

[`Node`](Node.md)[]

all meshes, lights, cameras, transformNodes and bones

#### Defined in

packages/dev/core/src/abstractScene.ts:222

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

#### Defined in

packages/dev/core/src/Layers/effectLayerSceneComponent.ts:40

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

#### Defined in

packages/dev/core/src/LensFlares/lensFlareSystemSceneComponent.ts:39

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

#### Defined in

packages/dev/core/src/Probes/reflectionProbe.ts:24

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

#### Defined in

packages/dev/core/src/abstractScene.ts:77

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

#### Defined in

packages/dev/core/src/abstractScene.ts:55

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

#### Defined in

packages/dev/core/src/abstractScene.ts:86

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

#### Defined in

packages/dev/core/src/abstractScene.ts:64

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

#### Defined in

packages/dev/core/src/abstractScene.ts:101
