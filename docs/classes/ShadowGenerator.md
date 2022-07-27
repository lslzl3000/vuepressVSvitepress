[@dev/core](../README.md) / [Exports](../modules.md) / ShadowGenerator

# Class: ShadowGenerator

Default implementation IShadowGenerator.
This is the main object responsible of generating shadows in the framework.
Documentation: https://doc.babylonjs.com/babylon101/shadows

## Hierarchy

- **`ShadowGenerator`**

  ↳ [`CascadedShadowGenerator`](CascadedShadowGenerator.md)

## Implements

- [`IShadowGenerator`](../interfaces/IShadowGenerator.md)

## Table of contents

### Constructors

- [constructor](ShadowGenerator.md#constructor)

### Properties

- [\_bias](ShadowGenerator.md#_bias)
- [\_blurBoxOffset](ShadowGenerator.md#_blurboxoffset)
- [\_blurKernel](ShadowGenerator.md#_blurkernel)
- [\_blurPostProcesses](ShadowGenerator.md#_blurpostprocesses)
- [\_blurScale](ShadowGenerator.md#_blurscale)
- [\_boxBlurPostprocess](ShadowGenerator.md#_boxblurpostprocess)
- [\_cachedDefines](ShadowGenerator.md#_cacheddefines)
- [\_cachedDirection](ShadowGenerator.md#_cacheddirection)
- [\_cachedPosition](ShadowGenerator.md#_cachedposition)
- [\_contactHardeningLightSizeUVRatio](ShadowGenerator.md#_contacthardeninglightsizeuvratio)
- [\_currentFaceIndex](ShadowGenerator.md#_currentfaceindex)
- [\_currentFaceIndexCache](ShadowGenerator.md#_currentfaceindexcache)
- [\_currentRenderId](ShadowGenerator.md#_currentrenderid)
- [\_currentSceneUBO](ShadowGenerator.md#_currentsceneubo)
- [\_darkness](ShadowGenerator.md#_darkness)
- [\_defaultTextureMatrix](ShadowGenerator.md#_defaulttexturematrix)
- [\_depthScale](ShadowGenerator.md#_depthscale)
- [\_filter](ShadowGenerator.md#_filter)
- [\_filteringQuality](ShadowGenerator.md#_filteringquality)
- [\_kernelBlurXPostprocess](ShadowGenerator.md#_kernelblurxpostprocess)
- [\_kernelBlurYPostprocess](ShadowGenerator.md#_kernelblurypostprocess)
- [\_light](ShadowGenerator.md#_light)
- [\_lightDirection](ShadowGenerator.md#_lightdirection)
- [\_mapSize](ShadowGenerator.md#_mapsize)
- [\_normalBias](ShadowGenerator.md#_normalbias)
- [\_projectionMatrix](ShadowGenerator.md#_projectionmatrix)
- [\_scene](ShadowGenerator.md#_scene)
- [\_sceneUBOs](ShadowGenerator.md#_sceneubos)
- [\_shadowMap](ShadowGenerator.md#_shadowmap)
- [\_shadowMap2](ShadowGenerator.md#_shadowmap2)
- [\_storedUniqueId](ShadowGenerator.md#_storeduniqueid)
- [\_textureType](ShadowGenerator.md#_texturetype)
- [\_transformMatrix](ShadowGenerator.md#_transformmatrix)
- [\_transparencyShadow](ShadowGenerator.md#_transparencyshadow)
- [\_useKernelBlur](ShadowGenerator.md#_usekernelblur)
- [\_useUBO](ShadowGenerator.md#_useubo)
- [\_viewMatrix](ShadowGenerator.md#_viewmatrix)
- [customAllowRendering](ShadowGenerator.md#customallowrendering)
- [customShaderOptions](ShadowGenerator.md#customshaderoptions)
- [enableSoftTransparentShadow](ShadowGenerator.md#enablesofttransparentshadow)
- [forceBackFacesOnly](ShadowGenerator.md#forcebackfacesonly)
- [frustumEdgeFalloff](ShadowGenerator.md#frustumedgefalloff)
- [id](ShadowGenerator.md#id)
- [onAfterShadowMapRenderMeshObservable](ShadowGenerator.md#onaftershadowmaprendermeshobservable)
- [onAfterShadowMapRenderObservable](ShadowGenerator.md#onaftershadowmaprenderobservable)
- [onBeforeShadowMapRenderMeshObservable](ShadowGenerator.md#onbeforeshadowmaprendermeshobservable)
- [onBeforeShadowMapRenderObservable](ShadowGenerator.md#onbeforeshadowmaprenderobservable)
- [useOpacityTextureForTransparentShadow](ShadowGenerator.md#useopacitytexturefortransparentshadow)
- [CLASSNAME](ShadowGenerator.md#classname)
- [DEFAULT\_ALPHA\_CUTOFF](ShadowGenerator.md#default_alpha_cutoff)
- [FILTER\_BLURCLOSEEXPONENTIALSHADOWMAP](ShadowGenerator.md#filter_blurcloseexponentialshadowmap)
- [FILTER\_BLUREXPONENTIALSHADOWMAP](ShadowGenerator.md#filter_blurexponentialshadowmap)
- [FILTER\_CLOSEEXPONENTIALSHADOWMAP](ShadowGenerator.md#filter_closeexponentialshadowmap)
- [FILTER\_EXPONENTIALSHADOWMAP](ShadowGenerator.md#filter_exponentialshadowmap)
- [FILTER\_NONE](ShadowGenerator.md#filter_none)
- [FILTER\_PCF](ShadowGenerator.md#filter_pcf)
- [FILTER\_PCSS](ShadowGenerator.md#filter_pcss)
- [FILTER\_POISSONSAMPLING](ShadowGenerator.md#filter_poissonsampling)
- [QUALITY\_HIGH](ShadowGenerator.md#quality_high)
- [QUALITY\_LOW](ShadowGenerator.md#quality_low)
- [QUALITY\_MEDIUM](ShadowGenerator.md#quality_medium)

### Accessors

- [bias](ShadowGenerator.md#bias)
- [blurBoxOffset](ShadowGenerator.md#blurboxoffset)
- [blurKernel](ShadowGenerator.md#blurkernel)
- [blurScale](ShadowGenerator.md#blurscale)
- [contactHardeningLightSizeUVRatio](ShadowGenerator.md#contacthardeninglightsizeuvratio)
- [darkness](ShadowGenerator.md#darkness)
- [depthScale](ShadowGenerator.md#depthscale)
- [filter](ShadowGenerator.md#filter)
- [filteringQuality](ShadowGenerator.md#filteringquality)
- [mapSize](ShadowGenerator.md#mapsize)
- [normalBias](ShadowGenerator.md#normalbias)
- [transparencyShadow](ShadowGenerator.md#transparencyshadow)
- [useBlurCloseExponentialShadowMap](ShadowGenerator.md#useblurcloseexponentialshadowmap)
- [useBlurExponentialShadowMap](ShadowGenerator.md#useblurexponentialshadowmap)
- [useCloseExponentialShadowMap](ShadowGenerator.md#usecloseexponentialshadowmap)
- [useContactHardeningShadow](ShadowGenerator.md#usecontacthardeningshadow)
- [useExponentialShadowMap](ShadowGenerator.md#useexponentialshadowmap)
- [useKernelBlur](ShadowGenerator.md#usekernelblur)
- [usePercentageCloserFiltering](ShadowGenerator.md#usepercentagecloserfiltering)
- [usePoissonSampling](ShadowGenerator.md#usepoissonsampling)

### Methods

- [\_applyFilterValues](ShadowGenerator.md#_applyfiltervalues)
- [\_bindCustomEffectForRenderSubMeshForShadowMap](ShadowGenerator.md#_bindcustomeffectforrendersubmeshforshadowmap)
- [\_createTargetRenderTexture](ShadowGenerator.md#_createtargetrendertexture)
- [\_disposeBlurPostProcesses](ShadowGenerator.md#_disposeblurpostprocesses)
- [\_disposeRTTandPostProcesses](ShadowGenerator.md#_disposerttandpostprocesses)
- [\_disposeSceneUBOs](ShadowGenerator.md#_disposesceneubos)
- [\_initializeBlurRTTAndPostProcesses](ShadowGenerator.md#_initializeblurrttandpostprocesses)
- [\_initializeGenerator](ShadowGenerator.md#_initializegenerator)
- [\_initializeShadowMap](ShadowGenerator.md#_initializeshadowmap)
- [\_isReadyCustomDefines](ShadowGenerator.md#_isreadycustomdefines)
- [\_prepareShadowDefines](ShadowGenerator.md#_prepareshadowdefines)
- [\_renderForShadowMap](ShadowGenerator.md#_renderforshadowmap)
- [\_renderSubMeshForShadowMap](ShadowGenerator.md#_rendersubmeshforshadowmap)
- [\_validateFilter](ShadowGenerator.md#_validatefilter)
- [addShadowCaster](ShadowGenerator.md#addshadowcaster)
- [bindShadowLight](ShadowGenerator.md#bindshadowlight)
- [dispose](ShadowGenerator.md#dispose)
- [forceCompilation](ShadowGenerator.md#forcecompilation)
- [forceCompilationAsync](ShadowGenerator.md#forcecompilationasync)
- [getClassName](ShadowGenerator.md#getclassname)
- [getDarkness](ShadowGenerator.md#getdarkness)
- [getLight](ShadowGenerator.md#getlight)
- [getShadowMap](ShadowGenerator.md#getshadowmap)
- [getShadowMapForRendering](ShadowGenerator.md#getshadowmapforrendering)
- [getTransformMatrix](ShadowGenerator.md#gettransformmatrix)
- [isReady](ShadowGenerator.md#isready)
- [prepareDefines](ShadowGenerator.md#preparedefines)
- [recreateShadowMap](ShadowGenerator.md#recreateshadowmap)
- [removeShadowCaster](ShadowGenerator.md#removeshadowcaster)
- [serialize](ShadowGenerator.md#serialize)
- [setDarkness](ShadowGenerator.md#setdarkness)
- [setTransparencyShadow](ShadowGenerator.md#settransparencyshadow)
- [Parse](ShadowGenerator.md#parse)

## Constructors

### constructor

• **new ShadowGenerator**(`mapSize`, `light`, `usefullFloatFirst?`)

Creates a ShadowGenerator object.
A ShadowGenerator is the required tool to use the shadows.
Each light casting shadows needs to use its own ShadowGenerator.
Documentation : https://doc.babylonjs.com/babylon101/shadows

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mapSize` | `number` | The size of the texture what stores the shadows. Example : 1024. |
| `light` | [`IShadowLight`](../interfaces/IShadowLight.md) | The light object generating the shadows. |
| `usefullFloatFirst?` | `boolean` | By default the generator will try to use half float textures but if you need precision (for self shadowing for instance), you can use this option to enforce full float texture. |

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:851

## Properties

### \_bias

• `Protected` **\_bias**: `number` = `0.00005`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:257

___

### \_blurBoxOffset

• `Protected` **\_blurBoxOffset**: `number` = `1`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:285

___

### \_blurKernel

• `Protected` **\_blurKernel**: `number` = `1`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:327

___

### \_blurPostProcesses

• `Protected` **\_blurPostProcesses**: [`PostProcess`](PostProcess.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:810

___

### \_blurScale

• `Protected` **\_blurScale**: `number` = `2`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:306

___

### \_boxBlurPostprocess

• `Protected` **\_boxBlurPostprocess**: [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:807

___

### \_cachedDefines

• `Protected` **\_cachedDefines**: `string`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:805

___

### \_cachedDirection

• `Protected` **\_cachedDirection**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:804

___

### \_cachedPosition

• `Protected` **\_cachedPosition**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:803

___

### \_contactHardeningLightSizeUVRatio

• `Protected` **\_contactHardeningLightSizeUVRatio**: `number` = `0.1`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:592

___

### \_currentFaceIndex

• `Protected` **\_currentFaceIndex**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:812

___

### \_currentFaceIndexCache

• `Protected` **\_currentFaceIndexCache**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:813

___

### \_currentRenderId

• `Protected` **\_currentRenderId**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:806

___

### \_currentSceneUBO

• `Protected` **\_currentSceneUBO**: [`UniformBuffer`](UniformBuffer.md)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:819

___

### \_darkness

• `Protected` **\_darkness**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:618

___

### \_defaultTextureMatrix

• `Protected` **\_defaultTextureMatrix**: [`Matrix`](Matrix.md)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:815

___

### \_depthScale

• `Protected` **\_depthScale**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:369

___

### \_filter

• `Protected` **\_filter**: `number` = `ShadowGenerator.FILTER_NONE`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:388

___

### \_filteringQuality

• `Protected` **\_filteringQuality**: `number` = `ShadowGenerator.QUALITY_HIGH`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:550

___

### \_kernelBlurXPostprocess

• `Protected` **\_kernelBlurXPostprocess**: [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:808

___

### \_kernelBlurYPostprocess

• `Protected` **\_kernelBlurYPostprocess**: [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:809

___

### \_light

• `Protected` **\_light**: [`IShadowLight`](../interfaces/IShadowLight.md)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:781

___

### \_lightDirection

• `Protected` **\_lightDirection**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:798

___

### \_mapSize

• `Protected` **\_mapSize**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:811

___

### \_normalBias

• `Protected` **\_normalBias**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:271

___

### \_projectionMatrix

• `Protected` **\_projectionMatrix**: [`Matrix`](Matrix.md)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:801

___

### \_scene

• `Protected` **\_scene**: [`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:797

___

### \_sceneUBOs

• `Protected` **\_sceneUBOs**: [`UniformBuffer`](UniformBuffer.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:818

___

### \_shadowMap

• `Protected` **\_shadowMap**: [`Nullable`](../modules.md#nullable)[`RenderTargetTexture`](RenderTargetTexture.md)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:689

___

### \_shadowMap2

• `Protected` **\_shadowMap2**: [`Nullable`](../modules.md#nullable)[`RenderTargetTexture`](RenderTargetTexture.md)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:690

___

### \_storedUniqueId

• `Protected` **\_storedUniqueId**: [`Nullable`](../modules.md#nullable)`number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:816

___

### \_textureType

• `Protected` **\_textureType**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:814

___

### \_transformMatrix

• `Protected` **\_transformMatrix**: [`Matrix`](Matrix.md)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:802

___

### \_transparencyShadow

• `Protected` **\_transparencyShadow**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:653

___

### \_useKernelBlur

• `Protected` **\_useKernelBlur**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:348

___

### \_useUBO

• `Protected` **\_useUBO**: `boolean`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:817

___

### \_viewMatrix

• `Protected` **\_viewMatrix**: [`Matrix`](Matrix.md)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:800

___

### customAllowRendering

• **customAllowRendering**: (`subMesh`: [`SubMesh`](SubMesh.md)) => `boolean`

#### Type declaration

▸ (`subMesh`): `boolean`

Gets or sets a custom function to allow/disallow rendering a sub mesh in the shadow map

##### Parameters

| Name | Type |
| :------ | :------ |
| `subMesh` | [`SubMesh`](SubMesh.md) |

##### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:233

___

### customShaderOptions

• **customShaderOptions**: [`ICustomShaderOptions`](../interfaces/ICustomShaderOptions.md)

Gets or sets the custom shader name to use

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:230

___

### enableSoftTransparentShadow

• **enableSoftTransparentShadow**: `boolean` = `false`

Enables or disables shadows with varying strength based on the transparency
When it is enabled, the strength of the shadow is taken equal to mesh.visibility
If you enabled an alpha texture on your material, the alpha value red from the texture is also combined to compute the strength:
         mesh.visibility * alphaTexture.a
The texture used is the diffuse by default, but it can be set to the opacity by setting useOpacityTextureForTransparentShadow
Note that by definition transparencyShadow must be set to true for enableSoftTransparentShadow to work!

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:682

___

### forceBackFacesOnly

• **forceBackFacesOnly**: `boolean` = `false`

If true the shadow map is generated by rendering the back face of the mesh instead of the front face.
This can help with self-shadowing as the geometry making up the back of objects is slightly offset.
It might on the other hand introduce peter panning.

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:795

___

### frustumEdgeFalloff

• **frustumEdgeFalloff**: `number` = `0`

Controls the extent to which the shadows fade out at the edge of the frustum

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:779

___

### id

• **id**: `string`

Gets or set the id of the shadow generator. It will be the one from the light if not defined

#### Implementation of

[IShadowGenerator](../interfaces/IShadowGenerator.md).[id](../interfaces/IShadowGenerator.md#id)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:227

___

### onAfterShadowMapRenderMeshObservable

• **onAfterShadowMapRenderMeshObservable**: [`Observable`](Observable.md)[`Mesh`](Mesh.md)

Observable triggered after a mesh is rendered in the shadow map.
Can be used to update internal effect state (that you can get from the onAfterShadowMapRenderObservable)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:255

___

### onAfterShadowMapRenderObservable

• **onAfterShadowMapRenderObservable**: [`Observable`](Observable.md)[`Effect`](Effect.md)

Observable triggered after the shadow is rendered. Can be used to restore internal effect state

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:243

___

### onBeforeShadowMapRenderMeshObservable

• **onBeforeShadowMapRenderMeshObservable**: [`Observable`](Observable.md)[`Mesh`](Mesh.md)

Observable triggered before a mesh is rendered in the shadow map.
Can be used to update internal effect state (that you can get from the onBeforeShadowMapRenderObservable)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:249

___

### onBeforeShadowMapRenderObservable

• **onBeforeShadowMapRenderObservable**: [`Observable`](Observable.md)[`Effect`](Effect.md)

Observable triggered before the shadow is rendered. Can be used to update internal effect state

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:238

___

### useOpacityTextureForTransparentShadow

• **useOpacityTextureForTransparentShadow**: `boolean` = `false`

If this is true, use the opacity texture's alpha channel for transparent shadows instead of the diffuse one

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:687

___

### CLASSNAME

▪ `Static` **CLASSNAME**: `string` = `"ShadowGenerator"`

Name of the shadow generator class

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:147

___

### DEFAULT\_ALPHA\_CUTOFF

▪ `Static` **DEFAULT\_ALPHA\_CUTOFF**: `number` = `0.5`

Defines the default alpha cutoff value used for transparent alpha tested materials.

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:224

___

### FILTER\_BLURCLOSEEXPONENTIALSHADOWMAP

▪ `Static` `Readonly` **FILTER\_BLURCLOSEEXPONENTIALSHADOWMAP**: ``5``

Shadow generator mode ESM: Blurred Exponential Shadow Mapping using the inverse of the exponential preventing
edge artifacts on steep falloff.
(http://developer.download.nvidia.com/presentations/2008/GDC/GDC08_SoftShadowMapping.pdf)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:179

___

### FILTER\_BLUREXPONENTIALSHADOWMAP

▪ `Static` `Readonly` **FILTER\_BLUREXPONENTIALSHADOWMAP**: ``3``

Shadow generator mode ESM: Blurred Exponential Shadow Mapping.
(http://developer.download.nvidia.com/presentations/2008/GDC/GDC08_SoftShadowMapping.pdf)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:167

___

### FILTER\_CLOSEEXPONENTIALSHADOWMAP

▪ `Static` `Readonly` **FILTER\_CLOSEEXPONENTIALSHADOWMAP**: ``4``

Shadow generator mode ESM: Exponential Shadow Mapping using the inverse of the exponential preventing
edge artifacts on steep falloff.
(http://developer.download.nvidia.com/presentations/2008/GDC/GDC08_SoftShadowMapping.pdf)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:173

___

### FILTER\_EXPONENTIALSHADOWMAP

▪ `Static` `Readonly` **FILTER\_EXPONENTIALSHADOWMAP**: ``1``

Shadow generator mode ESM: Exponential Shadow Mapping.
(http://developer.download.nvidia.com/presentations/2008/GDC/GDC08_SoftShadowMapping.pdf)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:157

___

### FILTER\_NONE

▪ `Static` `Readonly` **FILTER\_NONE**: ``0``

Shadow generator mode None: no filtering applied.

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:152

___

### FILTER\_PCF

▪ `Static` `Readonly` **FILTER\_PCF**: ``6``

Shadow generator mode PCF: Percentage Closer Filtering
benefits from Webgl 2 shadow samplers. Fallback to Poisson Sampling in Webgl 1
(https://developer.nvidia.com/gpugems/GPUGems/gpugems_ch11.html)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:185

___

### FILTER\_PCSS

▪ `Static` `Readonly` **FILTER\_PCSS**: ``7``

Shadow generator mode PCSS: Percentage Closering Soft Shadow.
benefits from Webgl 2 shadow samplers. Fallback to Poisson Sampling in Webgl 1
Contact Hardening

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:191

___

### FILTER\_POISSONSAMPLING

▪ `Static` `Readonly` **FILTER\_POISSONSAMPLING**: ``2``

Shadow generator mode Poisson Sampling: Percentage Closer Filtering.
(Multiple Tap around evenly distributed around the pixel are used to evaluate the shadow strength)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:162

___

### QUALITY\_HIGH

▪ `Static` `Readonly` **QUALITY\_HIGH**: ``0``

Reserved for PCF and PCSS
Highest Quality.

Execute PCF on a 5*5 kernel improving a lot the shadow aliasing artifacts.

Execute PCSS with 32 taps blocker search and 64 taps PCF.

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:201

___

### QUALITY\_LOW

▪ `Static` `Readonly` **QUALITY\_LOW**: ``2``

Reserved for PCF and PCSS
The lowest quality but the fastest.

Execute PCF on a 1*1 kernel.

Execute PCSS with 16 taps blocker search and 16 taps PCF.

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:219

___

### QUALITY\_MEDIUM

▪ `Static` `Readonly` **QUALITY\_MEDIUM**: ``1``

Reserved for PCF and PCSS
Good tradeoff for quality/perf cross devices

Execute PCF on a 3*3 kernel.

Execute PCSS with 16 taps blocker search and 32 taps PCF.

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:210

## Accessors

### bias

• `get` **bias**(): `number`

Gets the bias: offset applied on the depth preventing acnea (in light direction).

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:261

• `set` **bias**(`bias`): `void`

Sets the bias: offset applied on the depth preventing acnea (in light direction).

#### Parameters

| Name | Type |
| :------ | :------ |
| `bias` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:267

___

### blurBoxOffset

• `get` **blurBoxOffset**(): `number`

Gets the blur box offset: offset applied during the blur pass.
Only useful if useKernelBlur = false

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:290

• `set` **blurBoxOffset**(`value`): `void`

Sets the blur box offset: offset applied during the blur pass.
Only useful if useKernelBlur = false

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:297

___

### blurKernel

• `get` **blurKernel**(): `number`

Gets the blur kernel: kernel size of the blur pass.
Only useful if useKernelBlur = true

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:332

• `set` **blurKernel**(`value`): `void`

Sets the blur kernel: kernel size of the blur pass.
Only useful if useKernelBlur = true

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:339

___

### blurScale

• `get` **blurScale**(): `number`

Gets the blur scale: scale of the blurred texture compared to the main shadow map.
2 means half of the size.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:311

• `set` **blurScale**(`value`): `void`

Sets the blur scale: scale of the blurred texture compared to the main shadow map.
2 means half of the size.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:318

___

### contactHardeningLightSizeUVRatio

• `get` **contactHardeningLightSizeUVRatio**(): `number`

Gets the Light Size (in shadow map uv unit) used in PCSS to determine the blocker search area and the penumbra size.
Using a ratio helps keeping shape stability independently of the map size.

It does not account for the light projection as it was having too much
instability during the light setup or during light position changes.

Only valid if useContactHardeningShadow is true.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:602

• `set` **contactHardeningLightSizeUVRatio**(`contactHardeningLightSizeUVRatio`): `void`

Sets the Light Size (in shadow map uv unit) used in PCSS to determine the blocker search area and the penumbra size.
Using a ratio helps keeping shape stability independently of the map size.

It does not account for the light projection as it was having too much
instability during the light setup or during light position changes.

Only valid if useContactHardeningShadow is true.

#### Parameters

| Name | Type |
| :------ | :------ |
| `contactHardeningLightSizeUVRatio` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:614

___

### darkness

• `get` **darkness**(): `number`

Gets or sets the actual darkness of a shadow

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:621

• `set` **darkness**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:625

___

### depthScale

• `get` **depthScale**(): `number`

Gets the depth scale used in ESM mode.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:373

• `set` **depthScale**(`value`): `void`

Sets the depth scale used in ESM mode.
This can override the scale stored on the light.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:380

___

### filter

• `get` **filter**(): `number`

Gets the current mode of the shadow generator (normal, PCF, ESM...).
The returned value is a number equal to one of the available mode defined in ShadowMap.FILTER_x like _FILTER_NONE

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:393

• `set` **filter**(`value`): `void`

Sets the current mode of the shadow generator (normal, PCF, ESM...).
The returned value is a number equal to one of the available mode defined in ShadowMap.FILTER_x like _FILTER_NONE

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:400

___

### filteringQuality

• `get` **filteringQuality**(): `number`

Gets the PCF or PCSS Quality.
Only valid if usePercentageCloserFiltering or usePercentageCloserFiltering is true.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:555

• `set` **filteringQuality**(`filteringQuality`): `void`

Sets the PCF or PCSS Quality.
Only valid if usePercentageCloserFiltering or usePercentageCloserFiltering is true.

#### Parameters

| Name | Type |
| :------ | :------ |
| `filteringQuality` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:562

___

### mapSize

• `get` **mapSize**(): `number`

Gets or sets the size of the texture what stores the shadows

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:832

• `set` **mapSize**(`size`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `size` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:836

___

### normalBias

• `get` **normalBias**(): `number`

Gets the normalBias: offset applied on the depth preventing acnea (along side the normal direction and proportional to the light/normal angle).

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:275

• `set` **normalBias**(`normalBias`): `void`

Sets the normalBias: offset applied on the depth preventing acnea (along side the normal direction and proportional to the light/normal angle).

#### Parameters

| Name | Type |
| :------ | :------ |
| `normalBias` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:281

___

### transparencyShadow

• `get` **transparencyShadow**(): `boolean`

Gets or sets the ability to have transparent shadow

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:656

• `set` **transparencyShadow**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:660

___

### useBlurCloseExponentialShadowMap

• `get` **useBlurCloseExponentialShadowMap**(): `boolean`

Gets if the current filter is set to filtered "close ESM" (using the inverse of the
exponential to prevent steep falloff artifacts).

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:516

• `set` **useBlurCloseExponentialShadowMap**(`value`): `void`

Sets the current filter to filtered "close ESM" (using the inverse of the
exponential to prevent steep falloff artifacts).

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:523

___

### useBlurExponentialShadowMap

• `get` **useBlurExponentialShadowMap**(): `boolean`

Gets if the current filter is set to filtered ESM.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:477

• `set` **useBlurExponentialShadowMap**(`value`): `void`

Gets if the current filter is set to filtered  ESM.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:483

___

### useCloseExponentialShadowMap

• `get` **useCloseExponentialShadowMap**(): `boolean`

Gets if the current filter is set to "close ESM" (using the inverse of the
exponential to prevent steep falloff artifacts).

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:496

• `set` **useCloseExponentialShadowMap**(`value`): `void`

Sets the current filter to "close ESM" (using the inverse of the
exponential to prevent steep falloff artifacts).

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:503

___

### useContactHardeningShadow

• `get` **useContactHardeningShadow**(): `boolean`

Gets if the current filter is set to "PCSS" (contact hardening).

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:577

• `set` **useContactHardeningShadow**(`value`): `void`

Sets the current filter to "PCSS" (contact hardening).

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:583

___

### useExponentialShadowMap

• `get` **useExponentialShadowMap**(): `boolean`

Gets if the current filter is set to ESM.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:459

• `set` **useExponentialShadowMap**(`value`): `void`

Sets the current filter is to ESM.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:465

___

### useKernelBlur

• `get` **useKernelBlur**(): `boolean`

Gets whether the blur pass is a kernel blur (if true) or box blur.
Only useful in filtered mode (useBlurExponentialShadowMap...)

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:353

• `set` **useKernelBlur**(`value`): `void`

Sets whether the blur pass is a kernel blur (if true) or box blur.
Only useful in filtered mode (useBlurExponentialShadowMap...)

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:360

___

### usePercentageCloserFiltering

• `get` **usePercentageCloserFiltering**(): `boolean`

Gets if the current filter is set to "PCF" (percentage closer filtering).

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:535

• `set` **usePercentageCloserFiltering**(`value`): `void`

Sets the current filter to "PCF" (percentage closer filtering).

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:541

___

### usePoissonSampling

• `get` **usePoissonSampling**(): `boolean`

Gets if the current filter is set to Poisson Sampling.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:440

• `set` **usePoissonSampling**(`value`): `void`

Sets the current filter to Poisson Sampling.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:446

## Methods

### \_applyFilterValues

▸ `Protected` **_applyFilterValues**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:1310

___

### \_bindCustomEffectForRenderSubMeshForShadowMap

▸ `Protected` **_bindCustomEffectForRenderSubMeshForShadowMap**(`subMesh`, `effect`, `mesh`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `subMesh` | [`SubMesh`](SubMesh.md) |
| `effect` | [`Effect`](Effect.md) |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:1130

___

### \_createTargetRenderTexture

▸ `Protected` **_createTargetRenderTexture**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:896

___

### \_disposeBlurPostProcesses

▸ `Protected` **_disposeBlurPostProcesses**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:1866

___

### \_disposeRTTandPostProcesses

▸ `Protected` **_disposeRTTandPostProcesses**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:1890

___

### \_disposeSceneUBOs

▸ `Protected` **_disposeSceneUBOs**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:1899

___

### \_initializeBlurRTTAndPostProcesses

▸ `Protected` **_initializeBlurRTTAndPostProcesses**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:1019

___

### \_initializeGenerator

▸ `Protected` **_initializeGenerator**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:891

___

### \_initializeShadowMap

▸ `Protected` **_initializeShadowMap**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:917

___

### \_isReadyCustomDefines

▸ `Protected` **_isReadyCustomDefines**(`defines`, `subMesh`, `useInstances`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `defines` | `any` |
| `subMesh` | [`SubMesh`](SubMesh.md) |
| `useInstances` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:1402

___

### \_prepareShadowDefines

▸ `Private` **_prepareShadowDefines**(`subMesh`, `useInstances`, `defines`, `isTransparent`): `string`[]

#### Parameters

| Name | Type |
| :------ | :------ |
| `subMesh` | [`SubMesh`](SubMesh.md) |
| `useInstances` | `boolean` |
| `defines` | `string`[] |
| `isTransparent` | `boolean` |

#### Returns

`string`[]

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:1404

___

### \_renderForShadowMap

▸ `Protected` **_renderForShadowMap**(`opaqueSubMeshes`, `alphaTestSubMeshes`, `transparentSubMeshes`, `depthOnlySubMeshes`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `opaqueSubMeshes` | [`SmartArray`](SmartArray.md)[`SubMesh`](SubMesh.md) |
| `alphaTestSubMeshes` | [`SmartArray`](SmartArray.md)[`SubMesh`](SubMesh.md) |
| `transparentSubMeshes` | [`SmartArray`](SmartArray.md)[`SubMesh`](SubMesh.md) |
| `depthOnlySubMeshes` | [`SmartArray`](SmartArray.md)[`SubMesh`](SubMesh.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:1096

___

### \_renderSubMeshForShadowMap

▸ `Protected` **_renderSubMeshForShadowMap**(`subMesh`, `isTransparent?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `subMesh` | [`SubMesh`](SubMesh.md) | `undefined` |
| `isTransparent` | `boolean` | `false` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:1134

___

### \_validateFilter

▸ `Protected` **_validateFilter**(`filter`): `number`

#### Parameters

| Name | Type |
| :------ | :------ |
| `filter` | `number` |

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:384

___

### addShadowCaster

▸ **addShadowCaster**(`mesh`, `includeDescendants?`): [`ShadowGenerator`](ShadowGenerator.md)

Helper function to add a mesh and its descendants to the list of shadow casters.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | `undefined` | Mesh to add |
| `includeDescendants` | `boolean` | `true` | boolean indicating if the descendants should be added. Default to true |

#### Returns

[`ShadowGenerator`](ShadowGenerator.md)

the Shadow Generator itself

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:726

___

### bindShadowLight

▸ **bindShadowLight**(`lightIndex`, `effect`): `void`

Binds the shadow related information inside of an effect (information like near, far, darkness...
defined in the generator but impacting the effect).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `lightIndex` | `string` | Index of the light in the enabled light list of the material owning the effect |
| `effect` | [`Effect`](Effect.md) | The effect we are binding the information for |

#### Returns

`void`

#### Implementation of

[IShadowGenerator](../interfaces/IShadowGenerator.md).[bindShadowLight](../interfaces/IShadowGenerator.md#bindshadowlight)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:1728

___

### dispose

▸ **dispose**(): `void`

Disposes the ShadowGenerator.
Returns nothing.

#### Returns

`void`

#### Implementation of

[IShadowGenerator](../interfaces/IShadowGenerator.md).[dispose](../interfaces/IShadowGenerator.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:1912

___

### forceCompilation

▸ **forceCompilation**(`onCompiled?`, `options?`): `void`

Forces all the attached effect to compile to enable rendering only once ready vs. lazily compiling effects.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `onCompiled?` | (`generator`: [`IShadowGenerator`](../interfaces/IShadowGenerator.md)) => `void` | Callback triggered at the and of the effects compilation |
| `options?` | `Partial`{ `useInstances`: `boolean`  } | Sets of optional options forcing the compilation with different modes |

#### Returns

`void`

#### Implementation of

[IShadowGenerator](../interfaces/IShadowGenerator.md).[forceCompilation](../interfaces/IShadowGenerator.md#forcecompilation)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:1327

___

### forceCompilationAsync

▸ **forceCompilationAsync**(`options?`): `Promise``void`

Forces all the attached effect to compile to enable rendering only once ready vs. lazily compiling effects.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options?` | `Partial`{ `useInstances`: `boolean`  } | Sets of optional options forcing the compilation with different modes |

#### Returns

`Promise``void`

A promise that resolves when the compilation completes

#### Implementation of

[IShadowGenerator](../interfaces/IShadowGenerator.md).[forceCompilationAsync](../interfaces/IShadowGenerator.md#forcecompilationasync)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:1393

___

### getClassName

▸ **getClassName**(): `string`

Gets the class name of that object

#### Returns

`string`

"ShadowGenerator"

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:716

___

### getDarkness

▸ **getDarkness**(): `number`

Returns the darkness value (float). This can only decrease the actual darkness of a shadow.
0 means strongest and 1 would means no shadow.

#### Returns

`number`

the darkness.

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:634

___

### getLight

▸ **getLight**(): [`IShadowLight`](../interfaces/IShadowLight.md)

Returns the associated light object.

#### Returns

[`IShadowLight`](../interfaces/IShadowLight.md)

the light generating the shadow

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:786

___

### getShadowMap

▸ **getShadowMap**(): [`Nullable`](../modules.md#nullable)[`RenderTargetTexture`](RenderTargetTexture.md)

Gets the main RTT containing the shadow map (usually storing depth from the light point of view).

#### Returns

[`Nullable`](../modules.md#nullable)[`RenderTargetTexture`](RenderTargetTexture.md)

The render target texture if present otherwise, null

#### Implementation of

[IShadowGenerator](../interfaces/IShadowGenerator.md).[getShadowMap](../interfaces/IShadowGenerator.md#getshadowmap)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:696

___

### getShadowMapForRendering

▸ **getShadowMapForRendering**(): [`Nullable`](../modules.md#nullable)[`RenderTargetTexture`](RenderTargetTexture.md)

Gets the RTT used during rendering (can be a blurred version of the shadow map or the shadow map itself).

#### Returns

[`Nullable`](../modules.md#nullable)[`RenderTargetTexture`](RenderTargetTexture.md)

The render target texture if the shadow map is present otherwise, null

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:704

___

### getTransformMatrix

▸ **getTransformMatrix**(): [`Matrix`](Matrix.md)

Gets the transformation matrix used to project the meshes into the map from the light point of view.
(eq to shadow projection matrix * light transform matrix)

#### Returns

[`Matrix`](Matrix.md)

The transform matrix used to create the shadow map

#### Implementation of

[IShadowGenerator](../interfaces/IShadowGenerator.md).[getTransformMatrix](../interfaces/IShadowGenerator.md#gettransformmatrix)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:1784

___

### isReady

▸ **isReady**(`subMesh`, `useInstances`, `isTransparent`): `boolean`

Determine whether the shadow generator is ready or not (mainly all effects and related post processes needs to be ready).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `subMesh` | [`SubMesh`](SubMesh.md) | The submesh we want to render in the shadow map |
| `useInstances` | `boolean` | Defines whether will draw in the map using instances |
| `isTransparent` | `boolean` | Indicates that isReady is called for a transparent subMesh |

#### Returns

`boolean`

true if ready otherwise, false

#### Implementation of

[IShadowGenerator](../interfaces/IShadowGenerator.md).[isReady](../interfaces/IShadowGenerator.md#isready)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:1435

___

### prepareDefines

▸ **prepareDefines**(`defines`, `lightIndex`): `void`

Prepare all the defines in a material relying on a shadow map at the specified light index.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `defines` | `any` | Defines of the material we want to update |
| `lightIndex` | `number` | Index of the light in the enabled light list of the material |

#### Returns

`void`

#### Implementation of

[IShadowGenerator](../interfaces/IShadowGenerator.md).[prepareDefines](../interfaces/IShadowGenerator.md#preparedefines)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:1683

___

### recreateShadowMap

▸ **recreateShadowMap**(): `void`

Recreates the shadow map dependencies like RTT and post processes. This can be used during the switch between
Cube and 2D textures for instance.

#### Returns

`void`

#### Implementation of

[IShadowGenerator](../interfaces/IShadowGenerator.md).[recreateShadowMap](../interfaces/IShadowGenerator.md#recreateshadowmap)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:1835

___

### removeShadowCaster

▸ **removeShadowCaster**(`mesh`, `includeDescendants?`): [`ShadowGenerator`](ShadowGenerator.md)

Helper function to remove a mesh and its descendants from the list of shadow casters

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | `undefined` | Mesh to remove |
| `includeDescendants` | `boolean` | `true` | boolean indicating if the descendants should be removed. Default to true |

#### Returns

[`ShadowGenerator`](ShadowGenerator.md)

the Shadow Generator itself

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:756

___

### serialize

▸ **serialize**(): `any`

Serializes the shadow generator setup to a json object.

#### Returns

`any`

The serialized JSON object

#### Implementation of

[IShadowGenerator](../interfaces/IShadowGenerator.md).[serialize](../interfaces/IShadowGenerator.md#serialize)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:1932

___

### setDarkness

▸ **setDarkness**(`darkness`): [`ShadowGenerator`](ShadowGenerator.md)

Sets the darkness value (float). This can only decrease the actual darkness of a shadow.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `darkness` | `number` | The darkness value 0 means strongest and 1 would means no shadow. |

#### Returns

[`ShadowGenerator`](ShadowGenerator.md)

the shadow generator allowing fluent coding.

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:642

___

### setTransparencyShadow

▸ **setTransparencyShadow**(`transparent`): [`ShadowGenerator`](ShadowGenerator.md)

Sets the ability to have transparent shadow (boolean).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `transparent` | `boolean` | True if transparent else False |

#### Returns

[`ShadowGenerator`](ShadowGenerator.md)

the shadow generator allowing fluent coding

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:669

___

### Parse

▸ `Static` **Parse**(`parsedShadowGenerator`, `scene`, `constr?`): [`ShadowGenerator`](ShadowGenerator.md)

Parses a serialized ShadowGenerator and returns a new ShadowGenerator.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `parsedShadowGenerator` | `any` | The JSON object to parse |
| `scene` | [`Scene`](Scene.md) | The scene to create the shadow map for |
| `constr?` | (`mapSize`: `number`, `light`: [`IShadowLight`](../interfaces/IShadowLight.md)) => [`ShadowGenerator`](ShadowGenerator.md) | A function that builds a shadow generator or undefined to create an instance of the default shadow generator |

#### Returns

[`ShadowGenerator`](ShadowGenerator.md)

The parsed shadow generator

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:1984
