[@dev/core](../README.md) / [Exports](../modules.md) / MaterialHelper

# Class: MaterialHelper

"Static Class" containing the most commonly used helper while dealing with material for rendering purpose.

It contains the basic tools to help defining defines, binding uniform for the common part of the materials.

This works by convention in BabylonJS but is meant to be use only with shader following the in place naming rules and conventions.

## Table of contents

### Constructors

- [constructor](MaterialHelper.md#constructor)

### Properties

- [\_TempFogColor](MaterialHelper.md#_tempfogcolor)
- [\_TmpMorphInfluencers](MaterialHelper.md#_tmpmorphinfluencers)

### Methods

- [BindBonesParameters](MaterialHelper.md#bindbonesparameters)
- [BindClipPlane](MaterialHelper.md#bindclipplane)
- [BindFogParameters](MaterialHelper.md#bindfogparameters)
- [BindLight](MaterialHelper.md#bindlight)
- [BindLightProperties](MaterialHelper.md#bindlightproperties)
- [BindLights](MaterialHelper.md#bindlights)
- [BindLogDepth](MaterialHelper.md#bindlogdepth)
- [BindMorphTargetParameters](MaterialHelper.md#bindmorphtargetparameters)
- [BindSceneUniformBuffer](MaterialHelper.md#bindsceneuniformbuffer)
- [BindTextureMatrix](MaterialHelper.md#bindtexturematrix)
- [GetFogState](MaterialHelper.md#getfogstate)
- [HandleFallbacksForShadows](MaterialHelper.md#handlefallbacksforshadows)
- [PrepareAttributesForBakedVertexAnimation](MaterialHelper.md#prepareattributesforbakedvertexanimation)
- [PrepareAttributesForBones](MaterialHelper.md#prepareattributesforbones)
- [PrepareAttributesForInstances](MaterialHelper.md#prepareattributesforinstances)
- [PrepareAttributesForMorphTargets](MaterialHelper.md#prepareattributesformorphtargets)
- [PrepareAttributesForMorphTargetsInfluencers](MaterialHelper.md#prepareattributesformorphtargetsinfluencers)
- [PrepareDefinesForAttributes](MaterialHelper.md#preparedefinesforattributes)
- [PrepareDefinesForBakedVertexAnimation](MaterialHelper.md#preparedefinesforbakedvertexanimation)
- [PrepareDefinesForBones](MaterialHelper.md#preparedefinesforbones)
- [PrepareDefinesForFrameBoundValues](MaterialHelper.md#preparedefinesforframeboundvalues)
- [PrepareDefinesForLight](MaterialHelper.md#preparedefinesforlight)
- [PrepareDefinesForLights](MaterialHelper.md#preparedefinesforlights)
- [PrepareDefinesForMergedUV](MaterialHelper.md#preparedefinesformergeduv)
- [PrepareDefinesForMisc](MaterialHelper.md#preparedefinesformisc)
- [PrepareDefinesForMorphTargets](MaterialHelper.md#preparedefinesformorphtargets)
- [PrepareDefinesForMultiview](MaterialHelper.md#preparedefinesformultiview)
- [PrepareDefinesForOIT](MaterialHelper.md#preparedefinesforoit)
- [PrepareDefinesForPrePass](MaterialHelper.md#preparedefinesforprepass)
- [PrepareUniformsAndSamplersForLight](MaterialHelper.md#prepareuniformsandsamplersforlight)
- [PrepareUniformsAndSamplersList](MaterialHelper.md#prepareuniformsandsamplerslist)
- [PushAttributesForInstances](MaterialHelper.md#pushattributesforinstances)
- [\_CopyBonesTransformationMatrices](MaterialHelper.md#_copybonestransformationmatrices)

## Constructors

### constructor

• **new MaterialHelper**()

## Properties

### \_TempFogColor

▪ `Static` `Private` **\_TempFogColor**: [`Color3`](Color3.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialHelper.ts:932

___

### \_TmpMorphInfluencers

▪ `Static` `Private` **\_TmpMorphInfluencers**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `NUM_MORPH_INFLUENCERS` | `number` |

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialHelper.ts:773

## Methods

### BindBonesParameters

▸ `Static` **BindBonesParameters**(`mesh?`, `effect?`, `prePassConfiguration?`): `void`

Binds the bones information from the mesh to the effect.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh?` | [`AbstractMesh`](AbstractMesh.md) | The mesh we are binding the information to render |
| `effect?` | [`Effect`](Effect.md) | The effect we are binding the data to |
| `prePassConfiguration?` | `PrePassConfiguration` | Configuration for the prepass, in case prepass is activated |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialHelper.ts:959

___

### BindClipPlane

▸ `Static` **BindClipPlane**(`effect`, `scene`): `void`

Binds the clip plane information from the scene to the effect.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `effect` | [`Effect`](Effect.md) | The effect we are binding the data to |
| `scene` | [`Scene`](Scene.md) | The scene the clip plane information are extracted from |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialHelper.ts:1033

___

### BindFogParameters

▸ `Static` **BindFogParameters**(`scene`, `mesh`, `effect`, `linearSpace?`): `void`

Binds the fog information from the scene to the effect for the given mesh.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | `undefined` | The scene the lights belongs to |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | `undefined` | The mesh we are binding the information to render |
| `effect` | [`Effect`](Effect.md) | `undefined` | The effect we are binding the data to |
| `linearSpace` | `boolean` | `false` | Defines if the fog effect is applied in linear space |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialHelper.ts:940

___

### BindLight

▸ `Static` **BindLight**(`light`, `lightIndex`, `scene`, `effect`, `useSpecular`, `receiveShadows?`): `void`

Binds the lights information from the scene to the effect for the given mesh.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `light` | [`Light`](Light.md) | `undefined` | Light to bind |
| `lightIndex` | `number` | `undefined` | Light index |
| `scene` | [`Scene`](Scene.md) | `undefined` | The scene where the light belongs to |
| `effect` | [`Effect`](Effect.md) | `undefined` | The effect we are binding the data to |
| `useSpecular` | `boolean` | `undefined` | Defines if specular is supported |
| `receiveShadows` | `boolean` | `true` | Defines if the effect (mesh) we bind the light for receives shadows |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialHelper.ts:911

___

### BindLightProperties

▸ `Static` **BindLightProperties**(`light`, `effect`, `lightIndex`): `void`

Binds the light information to the effect.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `light` | [`Light`](Light.md) | The light containing the generator |
| `effect` | [`Effect`](Effect.md) | The effect we are binding the data to |
| `lightIndex` | `number` | The light index in the effect used to render |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialHelper.ts:898

___

### BindLights

▸ `Static` **BindLights**(`scene`, `mesh`, `effect`, `defines`, `maxSimultaneousLights?`): `void`

Binds the lights information from the scene to the effect for the given mesh.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | `undefined` | The scene the lights belongs to |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | `undefined` | The mesh we are binding the information to render |
| `effect` | [`Effect`](Effect.md) | `undefined` | The effect we are binding the data to |
| `defines` | `any` | `undefined` | The generated defines for the effect |
| `maxSimultaneousLights` | `number` | `4` | The maximum number of light that can be bound to the effect |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialHelper.ts:923

___

### BindLogDepth

▸ `Static` **BindLogDepth**(`defines`, `effect`, `scene`): `void`

Binds the logarithmic depth information from the scene to the effect for the given defines.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `defines` | `any` | The generated defines used in the effect |
| `effect` | [`Effect`](Effect.md) | The effect we are binding the data to |
| `scene` | [`Scene`](Scene.md) | The scene we are willing to render with logarithmic scale for |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialHelper.ts:1018

___

### BindMorphTargetParameters

▸ `Static` **BindMorphTargetParameters**(`abstractMesh`, `effect`): `void`

Binds the morph targets information from the mesh to the effect.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `abstractMesh` | [`AbstractMesh`](AbstractMesh.md) | The mesh we are binding the information to render |
| `effect` | [`Effect`](Effect.md) | The effect we are binding the data to |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialHelper.ts:1003

___

### BindSceneUniformBuffer

▸ `Static` **BindSceneUniformBuffer**(`effect`, `sceneUbo`): `void`

Binds the scene's uniform buffer to the effect.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `effect` | [`Effect`](Effect.md) | defines the effect to bind to the scene uniform buffer |
| `sceneUbo` | [`UniformBuffer`](UniformBuffer.md) | defines the uniform buffer storing scene data |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialHelper.ts:36

___

### BindTextureMatrix

▸ `Static` **BindTextureMatrix**(`texture`, `uniformBuffer`, `key`): `void`

Binds a texture matrix value to its corresponding uniform

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `texture` | [`BaseTexture`](BaseTexture.md) | The texture to bind the matrix for |
| `uniformBuffer` | [`UniformBuffer`](UniformBuffer.md) | The uniform buffer receiving the data |
| `key` | `string` | The channel key "diffuse", "specular"... used in the shader |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialHelper.ts:64

___

### GetFogState

▸ `Static` **GetFogState**(`mesh`, `scene`): `boolean`

Gets the current status of the fog (should it be enabled?)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | defines the mesh to evaluate for fog support |
| `scene` | [`Scene`](Scene.md) | defines the hosting scene |

#### Returns

`boolean`

true if fog must be enabled

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialHelper.ts:76

___

### HandleFallbacksForShadows

▸ `Static` **HandleFallbacksForShadows**(`defines`, `fallbacks`, `maxSimultaneousLights?`, `rank?`): `number`

This helps decreasing rank by rank the shadow quality (0 being the highest rank and quality)

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `defines` | `any` | `undefined` | The defines to update while falling back |
| `fallbacks` | [`EffectFallbacks`](EffectFallbacks.md) | `undefined` | The authorized effect fallbacks |
| `maxSimultaneousLights` | `number` | `4` | The maximum number of lights allowed |
| `rank` | `number` | `0` | the current rank of the Effect |

#### Returns

`number`

The newly affected rank

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialHelper.ts:731

___

### PrepareAttributesForBakedVertexAnimation

▸ `Static` **PrepareAttributesForBakedVertexAnimation**(`attribs`, `mesh`, `defines`): `void`

Prepares the list of attributes required for baked vertex animations according to the effect defines.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `attribs` | `string`[] | The current list of supported attribs |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | The mesh to prepare the morph targets attributes for |
| `defines` | `any` | The current Defines of the effect |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialHelper.ts:831

___

### PrepareAttributesForBones

▸ `Static` **PrepareAttributesForBones**(`attribs`, `mesh`, `defines`, `fallbacks`): `void`

Prepares the list of attributes required for bones according to the effect defines.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `attribs` | `string`[] | The current list of supported attribs |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | The mesh to prepare the bones attributes for |
| `defines` | `any` | The current Defines of the effect |
| `fallbacks` | [`EffectFallbacks`](EffectFallbacks.md) | The current effect fallback strategy |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialHelper.ts:846

___

### PrepareAttributesForInstances

▸ `Static` **PrepareAttributesForInstances**(`attribs`, `defines`): `void`

Check and prepare the list of attributes required for instances according to the effect defines.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `attribs` | `string`[] | The current list of supported attribs |
| `defines` | [`MaterialDefines`](MaterialDefines.md) | The current MaterialDefines of the effect |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialHelper.ts:864

___

### PrepareAttributesForMorphTargets

▸ `Static` **PrepareAttributesForMorphTargets**(`attribs`, `mesh`, `defines`): `void`

Prepares the list of attributes required for morph targets according to the effect defines.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `attribs` | `string`[] | The current list of supported attribs |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | The mesh to prepare the morph targets attributes for |
| `defines` | `any` | The current Defines of the effect |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialHelper.ts:791

___

### PrepareAttributesForMorphTargetsInfluencers

▸ `Static` **PrepareAttributesForMorphTargetsInfluencers**(`attribs`, `mesh`, `influencers`): `void`

Prepares the list of attributes required for morph targets according to the effect defines.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `attribs` | `string`[] | The current list of supported attribs |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | The mesh to prepare the morph targets attributes for |
| `influencers` | `number` | The number of influencers |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialHelper.ts:780

___

### PrepareDefinesForAttributes

▸ `Static` **PrepareDefinesForAttributes**(`mesh`, `defines`, `useVertexColor`, `useBones`, `useMorphTargets?`, `useVertexAlpha?`, `useBakedVertexAnimation?`): `boolean`

Prepares the defines used in the shader depending on the attributes data available in the mesh

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | `undefined` | The mesh containing the geometry data we will draw |
| `defines` | `any` | `undefined` | The defines to update |
| `useVertexColor` | `boolean` | `undefined` | Precise whether vertex colors should be used or not (override mesh info) |
| `useBones` | `boolean` | `undefined` | Precise whether bones should be used or not (override mesh info) |
| `useMorphTargets` | `boolean` | `false` | Precise whether morph targets should be used or not (override mesh info) |
| `useVertexAlpha` | `boolean` | `true` | Precise whether vertex alpha should be used or not (override mesh info) |
| `useBakedVertexAnimation` | `boolean` | `true` | Precise whether baked vertex animation should be used or not (override mesh info) |

#### Returns

`boolean`

false if defines are considered not dirty and have not been checked

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialHelper.ts:270

___

### PrepareDefinesForBakedVertexAnimation

▸ `Static` **PrepareDefinesForBakedVertexAnimation**(`mesh`, `defines`): `void`

Prepares the defines for baked vertex animation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | The mesh containing the geometry data we will draw |
| `defines` | `any` | The defines to update |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialHelper.ts:254

___

### PrepareDefinesForBones

▸ `Static` **PrepareDefinesForBones**(`mesh`, `defines`): `void`

Prepares the defines for bones

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | The mesh containing the geometry data we will draw |
| `defines` | `any` | The defines to update |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialHelper.ts:201

___

### PrepareDefinesForFrameBoundValues

▸ `Static` **PrepareDefinesForFrameBoundValues**(`scene`, `engine`, `defines`, `useInstances`, `useClipPlane?`, `useThinInstances?`): `void`

Helper used to prepare the list of defines associated with frame values for shader compilation

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | `undefined` | defines the current scene |
| `engine` | [`Engine`](Engine.md) | `undefined` | defines the current engine |
| `defines` | `any` | `undefined` | specifies the list of active defines |
| `useInstances` | `boolean` | `undefined` | defines if instances have to be turned on |
| `useClipPlane` | [`Nullable`](../modules.md#nullable)`boolean` | `null` | defines if clip plane have to be turned on |
| `useThinInstances` | `boolean` | `false` | defines if thin instances have to be turned on |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialHelper.ts:117

___

### PrepareDefinesForLight

▸ `Static` **PrepareDefinesForLight**(`scene`, `mesh`, `light`, `lightIndex`, `defines`, `specularSupported`, `state`): `void`

Prepares the defines related to the light information passed in parameter

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | The scene we are intending to draw |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | The mesh the effect is compiling for |
| `light` | [`Light`](Light.md) | The light the effect is compiling for |
| `lightIndex` | `number` | The index of the light |
| `defines` | `any` | The defines to update |
| `specularSupported` | `boolean` | Specifies whether specular is supported or not (override lights data) |
| `state` | `Object` | Defines the current state regarding what is needed (normals, etc...) |
| `state.lightmapMode` | `boolean` |  |
| `state.needNormals` | `boolean` |  |
| `state.needRebuild` | `boolean` |  |
| `state.shadowEnabled` | `boolean` |  |
| `state.specularEnabled` | `boolean` |  |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialHelper.ts:446

___

### PrepareDefinesForLights

▸ `Static` **PrepareDefinesForLights**(`scene`, `mesh`, `defines`, `specularSupported`, `maxSimultaneousLights?`, `disableLighting?`): `boolean`

Prepares the defines related to the light information passed in parameter

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | `undefined` | The scene we are intending to draw |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | `undefined` | The mesh the effect is compiling for |
| `defines` | `any` | `undefined` | The defines to update |
| `specularSupported` | `boolean` | `undefined` | Specifies whether specular is supported or not (override lights data) |
| `maxSimultaneousLights` | `number` | `4` | Specifies how manuy lights can be added to the effect at max |
| `disableLighting` | `boolean` | `false` | Specifies whether the lighting is disabled (override scene and light) |

#### Returns

`boolean`

true if normals will be required for the rest of the effect

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialHelper.ts:548

___

### PrepareDefinesForMergedUV

▸ `Static` **PrepareDefinesForMergedUV**(`texture`, `defines`, `key`): `void`

Helps preparing the defines values about the UVs in used in the effect.
UVs are shared as much as we can across channels in the shaders.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `texture` | [`BaseTexture`](BaseTexture.md) | The texture we are preparing the UVs for |
| `defines` | `any` | The defines to update |
| `key` | `string` | The channel key "diffuse", "specular"... used in the shader |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialHelper.ts:47

___

### PrepareDefinesForMisc

▸ `Static` **PrepareDefinesForMisc**(`mesh`, `scene`, `useLogarithmicDepth`, `pointsCloud`, `fogEnabled`, `alphaTest`, `defines`): `void`

Helper used to prepare the list of defines associated with misc. values for shader compilation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | defines the current mesh |
| `scene` | [`Scene`](Scene.md) | defines the current scene |
| `useLogarithmicDepth` | `boolean` | defines if logarithmic depth has to be turned on |
| `pointsCloud` | `boolean` | defines if point cloud rendering has to be turned on |
| `fogEnabled` | `boolean` | defines if fog has to be turned on |
| `alphaTest` | `boolean` | defines if alpha testing has to be turned on |
| `defines` | `any` | defines the current list of defines |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialHelper.ts:90

___

### PrepareDefinesForMorphTargets

▸ `Static` **PrepareDefinesForMorphTargets**(`mesh`, `defines`): `void`

Prepares the defines for morph targets

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | The mesh containing the geometry data we will draw |
| `defines` | `any` | The defines to update |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialHelper.ts:230

___

### PrepareDefinesForMultiview

▸ `Static` **PrepareDefinesForMultiview**(`scene`, `defines`): `void`

Prepares the defines related to multiview

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | The scene we are intending to draw |
| `defines` | `any` | The defines to update |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialHelper.ts:326

___

### PrepareDefinesForOIT

▸ `Static` **PrepareDefinesForOIT**(`scene`, `defines`, `needAlphaBlending`): `void`

Prepares the defines related to order independant transparency

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | The scene we are intending to draw |
| `defines` | `any` | The defines to update |
| `needAlphaBlending` | `boolean` | Determines if the material needs alpha blending |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialHelper.ts:342

___

### PrepareDefinesForPrePass

▸ `Static` **PrepareDefinesForPrePass**(`scene`, `defines`, `canRenderToMRT`): `void`

Prepares the defines related to the prepass

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | The scene we are intending to draw |
| `defines` | `any` | The defines to update |
| `canRenderToMRT` | `boolean` | Indicates if this material renders to several textures in the prepass |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialHelper.ts:360

___

### PrepareUniformsAndSamplersForLight

▸ `Static` **PrepareUniformsAndSamplersForLight**(`lightIndex`, `uniformsList`, `samplersList`, `projectedLightTexture?`, `uniformBuffersList?`, `updateOnlyBuffersList?`): `void`

Prepares the uniforms and samplers list to be used in the effect (for a specific light)

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `lightIndex` | `number` | `undefined` | defines the light index |
| `uniformsList` | `string`[] | `undefined` | The uniform list |
| `samplersList` | `string`[] | `undefined` | The sampler list |
| `projectedLightTexture?` | `any` | `undefined` | defines if projected texture must be used |
| `uniformBuffersList` | [`Nullable`](../modules.md#nullable)`string`[] | `null` | defines an optional list of uniform buffers |
| `updateOnlyBuffersList` | `boolean` | `false` | True to only update the uniformBuffersList array |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialHelper.ts:628

___

### PrepareUniformsAndSamplersList

▸ `Static` **PrepareUniformsAndSamplersList**(`uniformsListOrOptions`, `samplersList?`, `defines?`, `maxSimultaneousLights?`): `void`

Prepares the uniforms and samplers list to be used in the effect

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `uniformsListOrOptions` | `string`[] \| [`IEffectCreationOptions`](../interfaces/IEffectCreationOptions.md) | `undefined` | The uniform names to prepare or an EffectCreationOptions containing the list and extra information |
| `samplersList?` | `string`[] | `undefined` | The sampler list |
| `defines?` | `any` | `undefined` | The defines helping in the list generation |
| `maxSimultaneousLights` | `number` | `4` | The maximum number of simultaneous light allowed in the effect |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialHelper.ts:681

___

### PushAttributesForInstances

▸ `Static` **PushAttributesForInstances**(`attribs`, `needsPreviousMatrices?`): `void`

Add the list of attributes required for instances to the attribs array.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `attribs` | `string`[] | `undefined` | The current list of supported attribs |
| `needsPreviousMatrices` | `boolean` | `false` | If the shader needs previous matrices |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialHelper.ts:879

___

### \_CopyBonesTransformationMatrices

▸ `Static` `Private` **_CopyBonesTransformationMatrices**(`source`, `target`): `Float32Array`

#### Parameters

| Name | Type |
| :------ | :------ |
| `source` | `Float32Array` |
| `target` | `Float32Array` |

#### Returns

`Float32Array`

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialHelper.ts:992
