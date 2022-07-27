[@dev/core](../README.md) / [Exports](../modules.md) / AssetContainer

# Class: AssetContainer

Container with a set of assets that can be added or removed from a scene.

## Hierarchy

- [`AbstractScene`](AbstractScene.md)

  ↳ **`AssetContainer`**

## Table of contents

### Constructors

- [constructor](AssetContainer.md#constructor)

### Properties

- [\_onContextRestoredObserver](AssetContainer.md#_oncontextrestoredobserver)
- [\_wasAddedToScene](AssetContainer.md#_wasaddedtoscene)
- [actionManagers](AssetContainer.md#actionmanagers)
- [animationGroups](AssetContainer.md#animationgroups)
- [animations](AssetContainer.md#animations)
- [cameras](AssetContainer.md#cameras)
- [effectLayers](AssetContainer.md#effectlayers)
- [geometries](AssetContainer.md#geometries)
- [layers](AssetContainer.md#layers)
- [lensFlareSystems](AssetContainer.md#lensflaresystems)
- [lights](AssetContainer.md#lights)
- [materials](AssetContainer.md#materials)
- [meshes](AssetContainer.md#meshes)
- [morphTargetManagers](AssetContainer.md#morphtargetmanagers)
- [multiMaterials](AssetContainer.md#multimaterials)
- [particleSystems](AssetContainer.md#particlesystems)
- [postProcesses](AssetContainer.md#postprocesses)
- [prePassRenderer](AssetContainer.md#prepassrenderer)
- [proceduralTextures](AssetContainer.md#proceduraltextures)
- [reflectionProbes](AssetContainer.md#reflectionprobes)
- [rootNodes](AssetContainer.md#rootnodes)
- [scene](AssetContainer.md#scene)
- [skeletons](AssetContainer.md#skeletons)
- [sounds](AssetContainer.md#sounds)
- [subSurfaceConfiguration](AssetContainer.md#subsurfaceconfiguration)
- [textures](AssetContainer.md#textures)
- [transformNodes](AssetContainer.md#transformnodes)

### Accessors

- [environmentTexture](AssetContainer.md#environmenttexture)

### Methods

- [\_moveAssets](AssetContainer.md#_moveassets)
- [addAllToScene](AssetContainer.md#addalltoscene)
- [addEffectLayer](AssetContainer.md#addeffectlayer)
- [addLensFlareSystem](AssetContainer.md#addlensflaresystem)
- [addReflectionProbe](AssetContainer.md#addreflectionprobe)
- [addToScene](AssetContainer.md#addtoscene)
- [createRootMesh](AssetContainer.md#createrootmesh)
- [disablePrePassRenderer](AssetContainer.md#disableprepassrenderer)
- [disableSubSurfaceForPrePass](AssetContainer.md#disablesubsurfaceforprepass)
- [dispose](AssetContainer.md#dispose)
- [enablePrePassRenderer](AssetContainer.md#enableprepassrenderer)
- [enableSubSurfaceForPrePass](AssetContainer.md#enablesubsurfaceforprepass)
- [getGlowLayerByName](AssetContainer.md#getglowlayerbyname)
- [getHighlightLayerByName](AssetContainer.md#gethighlightlayerbyname)
- [getLensFlareSystemByID](AssetContainer.md#getlensflaresystembyid)
- [getLensFlareSystemById](AssetContainer.md#getlensflaresystembyid-1)
- [getLensFlareSystemByName](AssetContainer.md#getlensflaresystembyname)
- [getNodes](AssetContainer.md#getnodes)
- [instantiateModelsToScene](AssetContainer.md#instantiatemodelstoscene)
- [mergeAnimationsTo](AssetContainer.md#mergeanimationsto)
- [moveAllFromScene](AssetContainer.md#moveallfromscene)
- [removeAllFromScene](AssetContainer.md#removeallfromscene)
- [removeEffectLayer](AssetContainer.md#removeeffectlayer)
- [removeFromScene](AssetContainer.md#removefromscene)
- [removeLensFlareSystem](AssetContainer.md#removelensflaresystem)
- [removeReflectionProbe](AssetContainer.md#removereflectionprobe)
- [AddIndividualParser](AssetContainer.md#addindividualparser)
- [AddParser](AssetContainer.md#addparser)
- [GetIndividualParser](AssetContainer.md#getindividualparser)
- [GetParser](AssetContainer.md#getparser)
- [Parse](AssetContainer.md#parse)

## Constructors

### constructor

• **new AssetContainer**(`scene?`)

Instantiates an AssetContainer.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene?` | [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) | The scene the AssetContainer belongs to. |

#### Overrides

[AbstractScene](AbstractScene.md).[constructor](AbstractScene.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/assetContainer.ts:59

## Properties

### \_onContextRestoredObserver

• `Private` **\_onContextRestoredObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`ThinEngine`](ThinEngine.md)

#### Defined in

https://github.com/babylon.js/core/src/assetContainer.ts:48

___

### \_wasAddedToScene

• `Private` **\_wasAddedToScene**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/assetContainer.ts:47

___

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

### scene

• **scene**: [`Scene`](Scene.md)

The scene the AssetContainer belongs to.

#### Defined in

https://github.com/babylon.js/core/src/assetContainer.ts:53

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

### \_moveAssets

▸ `Private` **_moveAssets**`T`(`sourceAssets`, `targetAssets`, `keepAssets`): `void`

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `sourceAssets` | `T`[] |
| `targetAssets` | `T`[] |
| `keepAssets` | `T`[] |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/assetContainer.ts:586

___

### addAllToScene

▸ **addAllToScene**(): `void`

Adds all the assets from the container to the scene.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/assetContainer.ts:287

___

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

### addToScene

▸ **addToScene**(`predicate?`): `void`

Adds assets from the container to the scene.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `predicate` | [`Nullable`](../modules.md#nullable)(`entity`: `any`) => `boolean` | `null` | defines a predicate used to select which entity will be added (can be null) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/assetContainer.ts:312

___

### createRootMesh

▸ **createRootMesh**(): [`Mesh`](Mesh.md)

Adds all meshes in the asset container to a root mesh that can be used to position all the contained meshes. The root mesh is then added to the front of the meshes in the assetContainer.

#### Returns

[`Mesh`](Mesh.md)

the root mesh

#### Defined in

https://github.com/babylon.js/core/src/assetContainer.ts:636

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

### dispose

▸ **dispose**(): `void`

Disposes all the assets in the container

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/assetContainer.ts:510

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

### instantiateModelsToScene

▸ **instantiateModelsToScene**(`nameFunction?`, `cloneMaterials?`, `options?`): [`InstantiatedEntries`](InstantiatedEntries.md)

Instantiate or clone all meshes and add the new ones to the scene.
Skeletons and animation groups will all be cloned

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `nameFunction?` | (`sourceName`: `string`) => `string` | `undefined` | defines an optional function used to get new names for clones |
| `cloneMaterials` | `boolean` | `false` | defines an optional boolean that defines if materials must be cloned as well (false by default) |
| `options?` | `Object` | `undefined` | defines an optional list of options to control how to instantiate / clone models |
| `options.doNotInstantiate?` | `boolean` \| (`node`: [`TransformNode`](TransformNode.md)) => `boolean` | `undefined` | defines if the model must be instantiated or just cloned |
| `options.predicate?` | (`entity`: `any`) => `boolean` | `undefined` | - |

#### Returns

[`InstantiatedEntries`](InstantiatedEntries.md)

a list of rootNodes, skeletons and animation groups that were duplicated

#### Defined in

https://github.com/babylon.js/core/src/assetContainer.ts:108

___

### mergeAnimationsTo

▸ **mergeAnimationsTo**(`scene?`, `animatables`, `targetConverter?`): [`AnimationGroup`](AnimationGroup.md)[]

Merge animations (direct and animation groups) from this asset container into a scene

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `scene` | [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) | `EngineStore.LastCreatedScene` | is the instance of BABYLON.Scene to append to (default: last created scene) |
| `animatables` | [`Animatable`](Animatable.md)[] | `undefined` | set of animatables to retarget to a node from the scene |
| `targetConverter` | [`Nullable`](../modules.md#nullable)(`target`: `any`) => [`Nullable`](../modules.md#nullable)[`Node`](Node.md) | `null` | defines a function used to convert animation targets from the asset container to the scene (default: search node by name) |

#### Returns

[`AnimationGroup`](AnimationGroup.md)[]

an array of the new AnimationGroup added to the scene (empty array if none)

#### Defined in

https://github.com/babylon.js/core/src/assetContainer.ts:654

___

### moveAllFromScene

▸ **moveAllFromScene**(`keepAssets?`): `void`

Removes all the assets contained in the scene and adds them to the container.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `keepAssets?` | [`KeepAssets`](KeepAssets.md) | Set of assets to keep in the scene. (default: empty) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/assetContainer.ts:613

___

### removeAllFromScene

▸ **removeAllFromScene**(): `void`

Removes all the assets in the container from the scene

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/assetContainer.ts:402

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

### removeFromScene

▸ **removeFromScene**(`predicate?`): `void`

Removes assets in the container from the scene

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `predicate` | [`Nullable`](../modules.md#nullable)(`entity`: `any`) => `boolean` | `null` | defines a predicate used to select which entity will be added (can be null) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/assetContainer.ts:420

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
