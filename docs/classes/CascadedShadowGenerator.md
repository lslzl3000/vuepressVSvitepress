[@dev/core](../README.md) / [Exports](../modules.md) / CascadedShadowGenerator

# Class: CascadedShadowGenerator

A CSM implementation allowing casting shadows on large scenes.
Documentation : https://doc.babylonjs.com/babylon101/cascadedShadows
Based on: https://github.com/TheRealMJP/Shadows and https://johanmedestrom.wordpress.com/2016/03/18/opengl-cascaded-shadow-maps/

## Hierarchy

- [`ShadowGenerator`](ShadowGenerator.md)

  ↳ **`CascadedShadowGenerator`**

## Table of contents

### Constructors

- [constructor](CascadedShadowGenerator.md#constructor)

### Properties

- [\_autoCalcDepthBounds](CascadedShadowGenerator.md#_autocalcdepthbounds)
- [\_bias](CascadedShadowGenerator.md#_bias)
- [\_blurBoxOffset](CascadedShadowGenerator.md#_blurboxoffset)
- [\_blurKernel](CascadedShadowGenerator.md#_blurkernel)
- [\_blurPostProcesses](CascadedShadowGenerator.md#_blurpostprocesses)
- [\_blurScale](CascadedShadowGenerator.md#_blurscale)
- [\_boxBlurPostprocess](CascadedShadowGenerator.md#_boxblurpostprocess)
- [\_breaksAreDirty](CascadedShadowGenerator.md#_breaksaredirty)
- [\_cachedDefines](CascadedShadowGenerator.md#_cacheddefines)
- [\_cachedDirection](CascadedShadowGenerator.md#_cacheddirection)
- [\_cachedPosition](CascadedShadowGenerator.md#_cachedposition)
- [\_cascadeBlendPercentage](CascadedShadowGenerator.md#_cascadeblendpercentage)
- [\_cascadeMaxExtents](CascadedShadowGenerator.md#_cascademaxextents)
- [\_cascadeMinExtents](CascadedShadowGenerator.md#_cascademinextents)
- [\_cascades](CascadedShadowGenerator.md#_cascades)
- [\_contactHardeningLightSizeUVRatio](CascadedShadowGenerator.md#_contacthardeninglightsizeuvratio)
- [\_currentFaceIndex](CascadedShadowGenerator.md#_currentfaceindex)
- [\_currentFaceIndexCache](CascadedShadowGenerator.md#_currentfaceindexcache)
- [\_currentLayer](CascadedShadowGenerator.md#_currentlayer)
- [\_currentRenderId](CascadedShadowGenerator.md#_currentrenderid)
- [\_currentSceneUBO](CascadedShadowGenerator.md#_currentsceneubo)
- [\_darkness](CascadedShadowGenerator.md#_darkness)
- [\_debug](CascadedShadowGenerator.md#_debug)
- [\_defaultTextureMatrix](CascadedShadowGenerator.md#_defaulttexturematrix)
- [\_depthClamp](CascadedShadowGenerator.md#_depthclamp)
- [\_depthCorrection](CascadedShadowGenerator.md#_depthcorrection)
- [\_depthReducer](CascadedShadowGenerator.md#_depthreducer)
- [\_depthRenderer](CascadedShadowGenerator.md#_depthrenderer)
- [\_depthScale](CascadedShadowGenerator.md#_depthscale)
- [\_filter](CascadedShadowGenerator.md#_filter)
- [\_filteringQuality](CascadedShadowGenerator.md#_filteringquality)
- [\_freezeShadowCastersBoundingInfo](CascadedShadowGenerator.md#_freezeshadowcastersboundinginfo)
- [\_freezeShadowCastersBoundingInfoObservable](CascadedShadowGenerator.md#_freezeshadowcastersboundinginfoobservable)
- [\_frustumCenter](CascadedShadowGenerator.md#_frustumcenter)
- [\_frustumCornersWorldSpace](CascadedShadowGenerator.md#_frustumcornersworldspace)
- [\_frustumLengths](CascadedShadowGenerator.md#_frustumlengths)
- [\_kernelBlurXPostprocess](CascadedShadowGenerator.md#_kernelblurxpostprocess)
- [\_kernelBlurYPostprocess](CascadedShadowGenerator.md#_kernelblurypostprocess)
- [\_lambda](CascadedShadowGenerator.md#_lambda)
- [\_light](CascadedShadowGenerator.md#_light)
- [\_lightDirection](CascadedShadowGenerator.md#_lightdirection)
- [\_lightSizeUVCorrection](CascadedShadowGenerator.md#_lightsizeuvcorrection)
- [\_mapSize](CascadedShadowGenerator.md#_mapsize)
- [\_maxDistance](CascadedShadowGenerator.md#_maxdistance)
- [\_minDistance](CascadedShadowGenerator.md#_mindistance)
- [\_normalBias](CascadedShadowGenerator.md#_normalbias)
- [\_numCascades](CascadedShadowGenerator.md#_numcascades)
- [\_projectionMatrices](CascadedShadowGenerator.md#_projectionmatrices)
- [\_projectionMatrix](CascadedShadowGenerator.md#_projectionmatrix)
- [\_scbiMax](CascadedShadowGenerator.md#_scbimax)
- [\_scbiMin](CascadedShadowGenerator.md#_scbimin)
- [\_scene](CascadedShadowGenerator.md#_scene)
- [\_sceneUBOs](CascadedShadowGenerator.md#_sceneubos)
- [\_shadowCameraPos](CascadedShadowGenerator.md#_shadowcamerapos)
- [\_shadowCastersBoundingInfo](CascadedShadowGenerator.md#_shadowcastersboundinginfo)
- [\_shadowMap](CascadedShadowGenerator.md#_shadowmap)
- [\_shadowMap2](CascadedShadowGenerator.md#_shadowmap2)
- [\_shadowMaxZ](CascadedShadowGenerator.md#_shadowmaxz)
- [\_storedUniqueId](CascadedShadowGenerator.md#_storeduniqueid)
- [\_textureType](CascadedShadowGenerator.md#_texturetype)
- [\_transformMatrices](CascadedShadowGenerator.md#_transformmatrices)
- [\_transformMatricesAsArray](CascadedShadowGenerator.md#_transformmatricesasarray)
- [\_transformMatrix](CascadedShadowGenerator.md#_transformmatrix)
- [\_transparencyShadow](CascadedShadowGenerator.md#_transparencyshadow)
- [\_useKernelBlur](CascadedShadowGenerator.md#_usekernelblur)
- [\_useUBO](CascadedShadowGenerator.md#_useubo)
- [\_viewMatrices](CascadedShadowGenerator.md#_viewmatrices)
- [\_viewMatrix](CascadedShadowGenerator.md#_viewmatrix)
- [\_viewSpaceFrustumsZ](CascadedShadowGenerator.md#_viewspacefrustumsz)
- [customAllowRendering](CascadedShadowGenerator.md#customallowrendering)
- [customShaderOptions](CascadedShadowGenerator.md#customshaderoptions)
- [enableSoftTransparentShadow](CascadedShadowGenerator.md#enablesofttransparentshadow)
- [forceBackFacesOnly](CascadedShadowGenerator.md#forcebackfacesonly)
- [frustumEdgeFalloff](CascadedShadowGenerator.md#frustumedgefalloff)
- [id](CascadedShadowGenerator.md#id)
- [onAfterShadowMapRenderMeshObservable](CascadedShadowGenerator.md#onaftershadowmaprendermeshobservable)
- [onAfterShadowMapRenderObservable](CascadedShadowGenerator.md#onaftershadowmaprenderobservable)
- [onBeforeShadowMapRenderMeshObservable](CascadedShadowGenerator.md#onbeforeshadowmaprendermeshobservable)
- [onBeforeShadowMapRenderObservable](CascadedShadowGenerator.md#onbeforeshadowmaprenderobservable)
- [penumbraDarkness](CascadedShadowGenerator.md#penumbradarkness)
- [stabilizeCascades](CascadedShadowGenerator.md#stabilizecascades)
- [useOpacityTextureForTransparentShadow](CascadedShadowGenerator.md#useopacitytexturefortransparentshadow)
- [CLASSNAME](CascadedShadowGenerator.md#classname)
- [DEFAULT\_ALPHA\_CUTOFF](CascadedShadowGenerator.md#default_alpha_cutoff)
- [DEFAULT\_CASCADES\_COUNT](CascadedShadowGenerator.md#default_cascades_count)
- [FILTER\_BLURCLOSEEXPONENTIALSHADOWMAP](CascadedShadowGenerator.md#filter_blurcloseexponentialshadowmap)
- [FILTER\_BLUREXPONENTIALSHADOWMAP](CascadedShadowGenerator.md#filter_blurexponentialshadowmap)
- [FILTER\_CLOSEEXPONENTIALSHADOWMAP](CascadedShadowGenerator.md#filter_closeexponentialshadowmap)
- [FILTER\_EXPONENTIALSHADOWMAP](CascadedShadowGenerator.md#filter_exponentialshadowmap)
- [FILTER\_NONE](CascadedShadowGenerator.md#filter_none)
- [FILTER\_PCF](CascadedShadowGenerator.md#filter_pcf)
- [FILTER\_PCSS](CascadedShadowGenerator.md#filter_pcss)
- [FILTER\_POISSONSAMPLING](CascadedShadowGenerator.md#filter_poissonsampling)
- [MAX\_CASCADES\_COUNT](CascadedShadowGenerator.md#max_cascades_count)
- [MIN\_CASCADES\_COUNT](CascadedShadowGenerator.md#min_cascades_count)
- [QUALITY\_HIGH](CascadedShadowGenerator.md#quality_high)
- [QUALITY\_LOW](CascadedShadowGenerator.md#quality_low)
- [QUALITY\_MEDIUM](CascadedShadowGenerator.md#quality_medium)
- [\_FrustumCornersNDCSpace](CascadedShadowGenerator.md#_frustumcornersndcspace)

### Accessors

- [autoCalcDepthBounds](CascadedShadowGenerator.md#autocalcdepthbounds)
- [autoCalcDepthBoundsRefreshRate](CascadedShadowGenerator.md#autocalcdepthboundsrefreshrate)
- [bias](CascadedShadowGenerator.md#bias)
- [blurBoxOffset](CascadedShadowGenerator.md#blurboxoffset)
- [blurKernel](CascadedShadowGenerator.md#blurkernel)
- [blurScale](CascadedShadowGenerator.md#blurscale)
- [cascadeBlendPercentage](CascadedShadowGenerator.md#cascadeblendpercentage)
- [contactHardeningLightSizeUVRatio](CascadedShadowGenerator.md#contacthardeninglightsizeuvratio)
- [darkness](CascadedShadowGenerator.md#darkness)
- [debug](CascadedShadowGenerator.md#debug)
- [depthClamp](CascadedShadowGenerator.md#depthclamp)
- [depthScale](CascadedShadowGenerator.md#depthscale)
- [filter](CascadedShadowGenerator.md#filter)
- [filteringQuality](CascadedShadowGenerator.md#filteringquality)
- [freezeShadowCastersBoundingInfo](CascadedShadowGenerator.md#freezeshadowcastersboundinginfo)
- [lambda](CascadedShadowGenerator.md#lambda)
- [mapSize](CascadedShadowGenerator.md#mapsize)
- [maxDistance](CascadedShadowGenerator.md#maxdistance)
- [minDistance](CascadedShadowGenerator.md#mindistance)
- [normalBias](CascadedShadowGenerator.md#normalbias)
- [numCascades](CascadedShadowGenerator.md#numcascades)
- [shadowCastersBoundingInfo](CascadedShadowGenerator.md#shadowcastersboundinginfo)
- [shadowMaxZ](CascadedShadowGenerator.md#shadowmaxz)
- [transparencyShadow](CascadedShadowGenerator.md#transparencyshadow)
- [useBlurCloseExponentialShadowMap](CascadedShadowGenerator.md#useblurcloseexponentialshadowmap)
- [useBlurExponentialShadowMap](CascadedShadowGenerator.md#useblurexponentialshadowmap)
- [useCloseExponentialShadowMap](CascadedShadowGenerator.md#usecloseexponentialshadowmap)
- [useContactHardeningShadow](CascadedShadowGenerator.md#usecontacthardeningshadow)
- [useExponentialShadowMap](CascadedShadowGenerator.md#useexponentialshadowmap)
- [useKernelBlur](CascadedShadowGenerator.md#usekernelblur)
- [usePercentageCloserFiltering](CascadedShadowGenerator.md#usepercentagecloserfiltering)
- [usePoissonSampling](CascadedShadowGenerator.md#usepoissonsampling)
- [IsSupported](CascadedShadowGenerator.md#issupported)

### Methods

- [\_applyFilterValues](CascadedShadowGenerator.md#_applyfiltervalues)
- [\_bindCustomEffectForRenderSubMeshForShadowMap](CascadedShadowGenerator.md#_bindcustomeffectforrendersubmeshforshadowmap)
- [\_computeCascadeFrustum](CascadedShadowGenerator.md#_computecascadefrustum)
- [\_computeFrustumInWorldSpace](CascadedShadowGenerator.md#_computefrustuminworldspace)
- [\_computeMatrices](CascadedShadowGenerator.md#_computematrices)
- [\_computeShadowCastersBoundingInfo](CascadedShadowGenerator.md#_computeshadowcastersboundinginfo)
- [\_createTargetRenderTexture](CascadedShadowGenerator.md#_createtargetrendertexture)
- [\_disposeBlurPostProcesses](CascadedShadowGenerator.md#_disposeblurpostprocesses)
- [\_disposeRTTandPostProcesses](CascadedShadowGenerator.md#_disposerttandpostprocesses)
- [\_disposeSceneUBOs](CascadedShadowGenerator.md#_disposesceneubos)
- [\_initializeBlurRTTAndPostProcesses](CascadedShadowGenerator.md#_initializeblurrttandpostprocesses)
- [\_initializeGenerator](CascadedShadowGenerator.md#_initializegenerator)
- [\_initializeShadowMap](CascadedShadowGenerator.md#_initializeshadowmap)
- [\_isReadyCustomDefines](CascadedShadowGenerator.md#_isreadycustomdefines)
- [\_recreateSceneUBOs](CascadedShadowGenerator.md#_recreatesceneubos)
- [\_renderForShadowMap](CascadedShadowGenerator.md#_renderforshadowmap)
- [\_renderSubMeshForShadowMap](CascadedShadowGenerator.md#_rendersubmeshforshadowmap)
- [\_splitFrustum](CascadedShadowGenerator.md#_splitfrustum)
- [\_validateFilter](CascadedShadowGenerator.md#_validatefilter)
- [addShadowCaster](CascadedShadowGenerator.md#addshadowcaster)
- [bindShadowLight](CascadedShadowGenerator.md#bindshadowlight)
- [dispose](CascadedShadowGenerator.md#dispose)
- [forceCompilation](CascadedShadowGenerator.md#forcecompilation)
- [forceCompilationAsync](CascadedShadowGenerator.md#forcecompilationasync)
- [getCascadeMaxExtents](CascadedShadowGenerator.md#getcascademaxextents)
- [getCascadeMinExtents](CascadedShadowGenerator.md#getcascademinextents)
- [getCascadeProjectionMatrix](CascadedShadowGenerator.md#getcascadeprojectionmatrix)
- [getCascadeTransformMatrix](CascadedShadowGenerator.md#getcascadetransformmatrix)
- [getCascadeViewMatrix](CascadedShadowGenerator.md#getcascadeviewmatrix)
- [getClassName](CascadedShadowGenerator.md#getclassname)
- [getDarkness](CascadedShadowGenerator.md#getdarkness)
- [getLight](CascadedShadowGenerator.md#getlight)
- [getShadowMap](CascadedShadowGenerator.md#getshadowmap)
- [getShadowMapForRendering](CascadedShadowGenerator.md#getshadowmapforrendering)
- [getTransformMatrix](CascadedShadowGenerator.md#gettransformmatrix)
- [isReady](CascadedShadowGenerator.md#isready)
- [prepareDefines](CascadedShadowGenerator.md#preparedefines)
- [recreateShadowMap](CascadedShadowGenerator.md#recreateshadowmap)
- [removeShadowCaster](CascadedShadowGenerator.md#removeshadowcaster)
- [serialize](CascadedShadowGenerator.md#serialize)
- [setDarkness](CascadedShadowGenerator.md#setdarkness)
- [setDepthRenderer](CascadedShadowGenerator.md#setdepthrenderer)
- [setMinMaxDistance](CascadedShadowGenerator.md#setminmaxdistance)
- [setTransparencyShadow](CascadedShadowGenerator.md#settransparencyshadow)
- [splitFrustum](CascadedShadowGenerator.md#splitfrustum)
- [Parse](CascadedShadowGenerator.md#parse)

## Constructors

### constructor

• **new CascadedShadowGenerator**(`mapSize`, `light`, `usefulFloatFirst?`)

Creates a Cascaded Shadow Generator object.
A ShadowGenerator is the required tool to use the shadows.
Each directional light casting shadows needs to use its own ShadowGenerator.
Documentation : https://doc.babylonjs.com/babylon101/cascadedShadows

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mapSize` | `number` | The size of the texture what stores the shadows. Example : 1024. |
| `light` | [`DirectionalLight`](DirectionalLight.md) | The directional light object generating the shadows. |
| `usefulFloatFirst?` | `boolean` | By default the generator will try to use half float textures but if you need precision (for self shadowing for instance), you can use this option to enforce full float texture. |

#### Overrides

[ShadowGenerator](ShadowGenerator.md).[constructor](ShadowGenerator.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:746

## Properties

### \_autoCalcDepthBounds

• `Private` **\_autoCalcDepthBounds**: `boolean`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:434

___

### \_bias

• `Protected` **\_bias**: `number` = `0.00005`

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_bias](ShadowGenerator.md#_bias)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:257

___

### \_blurBoxOffset

• `Protected` **\_blurBoxOffset**: `number` = `1`

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_blurBoxOffset](ShadowGenerator.md#_blurboxoffset)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:285

___

### \_blurKernel

• `Protected` **\_blurKernel**: `number` = `1`

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_blurKernel](ShadowGenerator.md#_blurkernel)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:327

___

### \_blurPostProcesses

• `Protected` **\_blurPostProcesses**: [`PostProcess`](PostProcess.md)[]

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_blurPostProcesses](ShadowGenerator.md#_blurpostprocesses)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:810

___

### \_blurScale

• `Protected` **\_blurScale**: `number` = `2`

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_blurScale](ShadowGenerator.md#_blurscale)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:306

___

### \_boxBlurPostprocess

• `Protected` **\_boxBlurPostprocess**: [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_boxBlurPostprocess](ShadowGenerator.md#_boxblurpostprocess)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:807

___

### \_breaksAreDirty

• `Protected` **\_breaksAreDirty**: `boolean`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:203

___

### \_cachedDefines

• `Protected` **\_cachedDefines**: `string`

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_cachedDefines](ShadowGenerator.md#_cacheddefines)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:805

___

### \_cachedDirection

• `Protected` **\_cachedDirection**: [`Vector3`](Vector3.md)

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_cachedDirection](ShadowGenerator.md#_cacheddirection)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:804

___

### \_cachedPosition

• `Protected` **\_cachedPosition**: [`Vector3`](Vector3.md)

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_cachedPosition](ShadowGenerator.md#_cachedposition)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:803

___

### \_cascadeBlendPercentage

• `Private` **\_cascadeBlendPercentage**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:352

___

### \_cascadeMaxExtents

• `Private` **\_cascadeMaxExtents**: [`Vector3`](Vector3.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:258

___

### \_cascadeMinExtents

• `Private` **\_cascadeMinExtents**: [`Vector3`](Vector3.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:257

___

### \_cascades

• `Private` **\_cascades**: `ICascade`[]

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:278

___

### \_contactHardeningLightSizeUVRatio

• `Protected` **\_contactHardeningLightSizeUVRatio**: `number` = `0.1`

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_contactHardeningLightSizeUVRatio](ShadowGenerator.md#_contacthardeninglightsizeuvratio)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:592

___

### \_currentFaceIndex

• `Protected` **\_currentFaceIndex**: `number` = `0`

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_currentFaceIndex](ShadowGenerator.md#_currentfaceindex)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:812

___

### \_currentFaceIndexCache

• `Protected` **\_currentFaceIndexCache**: `number` = `0`

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_currentFaceIndexCache](ShadowGenerator.md#_currentfaceindexcache)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:813

___

### \_currentLayer

• `Private` **\_currentLayer**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:279

___

### \_currentRenderId

• `Protected` **\_currentRenderId**: `number`

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_currentRenderId](ShadowGenerator.md#_currentrenderid)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:806

___

### \_currentSceneUBO

• `Protected` **\_currentSceneUBO**: [`UniformBuffer`](UniformBuffer.md)

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_currentSceneUBO](ShadowGenerator.md#_currentsceneubo)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:819

___

### \_darkness

• `Protected` **\_darkness**: `number` = `0`

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_darkness](ShadowGenerator.md#_darkness)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:618

___

### \_debug

• `Protected` **\_debug**: `boolean`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:319

___

### \_defaultTextureMatrix

• `Protected` **\_defaultTextureMatrix**: [`Matrix`](Matrix.md)

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_defaultTextureMatrix](ShadowGenerator.md#_defaulttexturematrix)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:815

___

### \_depthClamp

• `Private` **\_depthClamp**: `boolean`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:334

___

### \_depthCorrection

• `Private` **\_depthCorrection**: `number`[]

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:287

___

### \_depthReducer

• `Private` **\_depthReducer**: [`Nullable`](../modules.md#nullable)[`DepthReducer`](DepthReducer.md)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:433

___

### \_depthRenderer

• `Private` **\_depthRenderer**: [`Nullable`](../modules.md#nullable)[`DepthRenderer`](DepthRenderer.md)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:415

___

### \_depthScale

• `Protected` **\_depthScale**: `number`

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_depthScale](ShadowGenerator.md#_depthscale)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:369

___

### \_filter

• `Protected` **\_filter**: `number` = `ShadowGenerator.FILTER_NONE`

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_filter](ShadowGenerator.md#_filter)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:388

___

### \_filteringQuality

• `Protected` **\_filteringQuality**: `number` = `ShadowGenerator.QUALITY_HIGH`

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_filteringQuality](ShadowGenerator.md#_filteringquality)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:550

___

### \_freezeShadowCastersBoundingInfo

• `Private` **\_freezeShadowCastersBoundingInfo**: `boolean`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:117

___

### \_freezeShadowCastersBoundingInfoObservable

• `Private` **\_freezeShadowCastersBoundingInfoObservable**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:118

___

### \_frustumCenter

• `Private` **\_frustumCenter**: [`Vector3`](Vector3.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:289

___

### \_frustumCornersWorldSpace

• `Private` **\_frustumCornersWorldSpace**: [`Vector3`](Vector3.md)[][]

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:288

___

### \_frustumLengths

• `Private` **\_frustumLengths**: `number`[]

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:285

___

### \_kernelBlurXPostprocess

• `Protected` **\_kernelBlurXPostprocess**: [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_kernelBlurXPostprocess](ShadowGenerator.md#_kernelblurxpostprocess)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:808

___

### \_kernelBlurYPostprocess

• `Protected` **\_kernelBlurYPostprocess**: [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_kernelBlurYPostprocess](ShadowGenerator.md#_kernelblurypostprocess)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:809

___

### \_lambda

• `Private` **\_lambda**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:367

___

### \_light

• `Protected` **\_light**: [`IShadowLight`](../interfaces/IShadowLight.md)

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_light](ShadowGenerator.md#_light)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:781

___

### \_lightDirection

• `Protected` **\_lightDirection**: [`Vector3`](Vector3.md)

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_lightDirection](ShadowGenerator.md#_lightdirection)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:798

___

### \_lightSizeUVCorrection

• `Private` **\_lightSizeUVCorrection**: `number`[]

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:286

___

### \_mapSize

• `Protected` **\_mapSize**: `number`

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_mapSize](ShadowGenerator.md#_mapsize)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:811

___

### \_maxDistance

• `Protected` **\_maxDistance**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:206

___

### \_minDistance

• `Protected` **\_minDistance**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:205

___

### \_normalBias

• `Protected` **\_normalBias**: `number` = `0`

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_normalBias](ShadowGenerator.md#_normalbias)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:271

___

### \_numCascades

• `Private` **\_numCascades**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:91

___

### \_projectionMatrices

• `Private` **\_projectionMatrices**: [`Matrix`](Matrix.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:282

___

### \_projectionMatrix

• `Protected` **\_projectionMatrix**: [`Matrix`](Matrix.md)

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_projectionMatrix](ShadowGenerator.md#_projectionmatrix)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:801

___

### \_scbiMax

• `Private` **\_scbiMax**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:147

___

### \_scbiMin

• `Private` **\_scbiMin**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:146

___

### \_scene

• `Protected` **\_scene**: [`Scene`](Scene.md)

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_scene](ShadowGenerator.md#_scene)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:797

___

### \_sceneUBOs

• `Protected` **\_sceneUBOs**: [`UniformBuffer`](UniformBuffer.md)[]

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_sceneUBOs](ShadowGenerator.md#_sceneubos)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:818

___

### \_shadowCameraPos

• `Private` **\_shadowCameraPos**: [`Vector3`](Vector3.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:290

___

### \_shadowCastersBoundingInfo

• `Protected` **\_shadowCastersBoundingInfo**: [`BoundingInfo`](BoundingInfo.md)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:188

___

### \_shadowMap

• `Protected` **\_shadowMap**: [`Nullable`](../modules.md#nullable)[`RenderTargetTexture`](RenderTargetTexture.md)

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_shadowMap](ShadowGenerator.md#_shadowmap)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:689

___

### \_shadowMap2

• `Protected` **\_shadowMap2**: [`Nullable`](../modules.md#nullable)[`RenderTargetTexture`](RenderTargetTexture.md)

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_shadowMap2](ShadowGenerator.md#_shadowmap2)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:690

___

### \_shadowMaxZ

• `Private` **\_shadowMaxZ**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:292

___

### \_storedUniqueId

• `Protected` **\_storedUniqueId**: [`Nullable`](../modules.md#nullable)`number`

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_storedUniqueId](ShadowGenerator.md#_storeduniqueid)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:816

___

### \_textureType

• `Protected` **\_textureType**: `number`

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_textureType](ShadowGenerator.md#_texturetype)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:814

___

### \_transformMatrices

• `Private` **\_transformMatrices**: [`Matrix`](Matrix.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:283

___

### \_transformMatricesAsArray

• `Private` **\_transformMatricesAsArray**: `Float32Array`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:284

___

### \_transformMatrix

• `Protected` **\_transformMatrix**: [`Matrix`](Matrix.md)

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_transformMatrix](ShadowGenerator.md#_transformmatrix)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:802

___

### \_transparencyShadow

• `Protected` **\_transparencyShadow**: `boolean` = `false`

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_transparencyShadow](ShadowGenerator.md#_transparencyshadow)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:653

___

### \_useKernelBlur

• `Protected` **\_useKernelBlur**: `boolean` = `false`

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_useKernelBlur](ShadowGenerator.md#_usekernelblur)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:348

___

### \_useUBO

• `Protected` **\_useUBO**: `boolean`

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_useUBO](ShadowGenerator.md#_useubo)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:817

___

### \_viewMatrices

• `Private` **\_viewMatrices**: [`Matrix`](Matrix.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:281

___

### \_viewMatrix

• `Protected` **\_viewMatrix**: [`Matrix`](Matrix.md)

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_viewMatrix](ShadowGenerator.md#_viewmatrix)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:800

___

### \_viewSpaceFrustumsZ

• `Private` **\_viewSpaceFrustumsZ**: `number`[]

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:280

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

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[customAllowRendering](ShadowGenerator.md#customallowrendering)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:233

___

### customShaderOptions

• **customShaderOptions**: [`ICustomShaderOptions`](../interfaces/ICustomShaderOptions.md)

Gets or sets the custom shader name to use

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[customShaderOptions](ShadowGenerator.md#customshaderoptions)

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

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[enableSoftTransparentShadow](ShadowGenerator.md#enablesofttransparentshadow)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:682

___

### forceBackFacesOnly

• **forceBackFacesOnly**: `boolean` = `false`

If true the shadow map is generated by rendering the back face of the mesh instead of the front face.
This can help with self-shadowing as the geometry making up the back of objects is slightly offset.
It might on the other hand introduce peter panning.

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[forceBackFacesOnly](ShadowGenerator.md#forcebackfacesonly)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:795

___

### frustumEdgeFalloff

• **frustumEdgeFalloff**: `number` = `0`

Controls the extent to which the shadows fade out at the edge of the frustum

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[frustumEdgeFalloff](ShadowGenerator.md#frustumedgefalloff)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:779

___

### id

• **id**: `string`

Gets or set the id of the shadow generator. It will be the one from the light if not defined

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[id](ShadowGenerator.md#id)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:227

___

### onAfterShadowMapRenderMeshObservable

• **onAfterShadowMapRenderMeshObservable**: [`Observable`](Observable.md)[`Mesh`](Mesh.md)

Observable triggered after a mesh is rendered in the shadow map.
Can be used to update internal effect state (that you can get from the onAfterShadowMapRenderObservable)

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[onAfterShadowMapRenderMeshObservable](ShadowGenerator.md#onaftershadowmaprendermeshobservable)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:255

___

### onAfterShadowMapRenderObservable

• **onAfterShadowMapRenderObservable**: [`Observable`](Observable.md)[`Effect`](Effect.md)

Observable triggered after the shadow is rendered. Can be used to restore internal effect state

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[onAfterShadowMapRenderObservable](ShadowGenerator.md#onaftershadowmaprenderobservable)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:243

___

### onBeforeShadowMapRenderMeshObservable

• **onBeforeShadowMapRenderMeshObservable**: [`Observable`](Observable.md)[`Mesh`](Mesh.md)

Observable triggered before a mesh is rendered in the shadow map.
Can be used to update internal effect state (that you can get from the onBeforeShadowMapRenderObservable)

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[onBeforeShadowMapRenderMeshObservable](ShadowGenerator.md#onbeforeshadowmaprendermeshobservable)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:249

___

### onBeforeShadowMapRenderObservable

• **onBeforeShadowMapRenderObservable**: [`Observable`](Observable.md)[`Effect`](Effect.md)

Observable triggered before the shadow is rendered. Can be used to update internal effect state

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[onBeforeShadowMapRenderObservable](ShadowGenerator.md#onbeforeshadowmaprenderobservable)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:238

___

### penumbraDarkness

• **penumbraDarkness**: `number`

Gets or sets the actual darkness of the soft shadows while using PCSS filtering (value between 0. and 1.)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:89

___

### stabilizeCascades

• **stabilizeCascades**: `boolean`

Sets this to true if you want that the edges of the shadows don't "swimm" / "shimmer" when rotating the camera.
The trade off is that you lose some precision in the shadow rendering when enabling this setting.

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:115

___

### useOpacityTextureForTransparentShadow

• **useOpacityTextureForTransparentShadow**: `boolean` = `false`

If this is true, use the opacity texture's alpha channel for transparent shadows instead of the diffuse one

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[useOpacityTextureForTransparentShadow](ShadowGenerator.md#useopacitytexturefortransparentshadow)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:687

___

### CLASSNAME

▪ `Static` **CLASSNAME**: `string` = `"CascadedShadowGenerator"`

Name of the CSM class

#### Overrides

[ShadowGenerator](ShadowGenerator.md).[CLASSNAME](ShadowGenerator.md#classname)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:61

___

### DEFAULT\_ALPHA\_CUTOFF

▪ `Static` **DEFAULT\_ALPHA\_CUTOFF**: `number` = `0.5`

Defines the default alpha cutoff value used for transparent alpha tested materials.

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[DEFAULT_ALPHA_CUTOFF](ShadowGenerator.md#default_alpha_cutoff)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:224

___

### DEFAULT\_CASCADES\_COUNT

▪ `Static` `Readonly` **DEFAULT\_CASCADES\_COUNT**: ``4``

Defines the default number of cascades used by the CSM.

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:66

___

### FILTER\_BLURCLOSEEXPONENTIALSHADOWMAP

▪ `Static` `Readonly` **FILTER\_BLURCLOSEEXPONENTIALSHADOWMAP**: ``5``

Shadow generator mode ESM: Blurred Exponential Shadow Mapping using the inverse of the exponential preventing
edge artifacts on steep falloff.
(http://developer.download.nvidia.com/presentations/2008/GDC/GDC08_SoftShadowMapping.pdf)

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[FILTER_BLURCLOSEEXPONENTIALSHADOWMAP](ShadowGenerator.md#filter_blurcloseexponentialshadowmap)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:179

___

### FILTER\_BLUREXPONENTIALSHADOWMAP

▪ `Static` `Readonly` **FILTER\_BLUREXPONENTIALSHADOWMAP**: ``3``

Shadow generator mode ESM: Blurred Exponential Shadow Mapping.
(http://developer.download.nvidia.com/presentations/2008/GDC/GDC08_SoftShadowMapping.pdf)

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[FILTER_BLUREXPONENTIALSHADOWMAP](ShadowGenerator.md#filter_blurexponentialshadowmap)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:167

___

### FILTER\_CLOSEEXPONENTIALSHADOWMAP

▪ `Static` `Readonly` **FILTER\_CLOSEEXPONENTIALSHADOWMAP**: ``4``

Shadow generator mode ESM: Exponential Shadow Mapping using the inverse of the exponential preventing
edge artifacts on steep falloff.
(http://developer.download.nvidia.com/presentations/2008/GDC/GDC08_SoftShadowMapping.pdf)

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[FILTER_CLOSEEXPONENTIALSHADOWMAP](ShadowGenerator.md#filter_closeexponentialshadowmap)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:173

___

### FILTER\_EXPONENTIALSHADOWMAP

▪ `Static` `Readonly` **FILTER\_EXPONENTIALSHADOWMAP**: ``1``

Shadow generator mode ESM: Exponential Shadow Mapping.
(http://developer.download.nvidia.com/presentations/2008/GDC/GDC08_SoftShadowMapping.pdf)

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[FILTER_EXPONENTIALSHADOWMAP](ShadowGenerator.md#filter_exponentialshadowmap)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:157

___

### FILTER\_NONE

▪ `Static` `Readonly` **FILTER\_NONE**: ``0``

Shadow generator mode None: no filtering applied.

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[FILTER_NONE](ShadowGenerator.md#filter_none)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:152

___

### FILTER\_PCF

▪ `Static` `Readonly` **FILTER\_PCF**: ``6``

Shadow generator mode PCF: Percentage Closer Filtering
benefits from Webgl 2 shadow samplers. Fallback to Poisson Sampling in Webgl 1
(https://developer.nvidia.com/gpugems/GPUGems/gpugems_ch11.html)

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[FILTER_PCF](ShadowGenerator.md#filter_pcf)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:185

___

### FILTER\_PCSS

▪ `Static` `Readonly` **FILTER\_PCSS**: ``7``

Shadow generator mode PCSS: Percentage Closering Soft Shadow.
benefits from Webgl 2 shadow samplers. Fallback to Poisson Sampling in Webgl 1
Contact Hardening

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[FILTER_PCSS](ShadowGenerator.md#filter_pcss)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:191

___

### FILTER\_POISSONSAMPLING

▪ `Static` `Readonly` **FILTER\_POISSONSAMPLING**: ``2``

Shadow generator mode Poisson Sampling: Percentage Closer Filtering.
(Multiple Tap around evenly distributed around the pixel are used to evaluate the shadow strength)

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[FILTER_POISSONSAMPLING](ShadowGenerator.md#filter_poissonsampling)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:162

___

### MAX\_CASCADES\_COUNT

▪ `Static` `Readonly` **MAX\_CASCADES\_COUNT**: ``4``

Defines the maximum number of cascades used by the CSM.

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:74

___

### MIN\_CASCADES\_COUNT

▪ `Static` `Readonly` **MIN\_CASCADES\_COUNT**: ``2``

Defines the minimum number of cascades used by the CSM.

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:70

___

### QUALITY\_HIGH

▪ `Static` `Readonly` **QUALITY\_HIGH**: ``0``

Reserved for PCF and PCSS
Highest Quality.

Execute PCF on a 5*5 kernel improving a lot the shadow aliasing artifacts.

Execute PCSS with 32 taps blocker search and 64 taps PCF.

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[QUALITY_HIGH](ShadowGenerator.md#quality_high)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:201

___

### QUALITY\_LOW

▪ `Static` `Readonly` **QUALITY\_LOW**: ``2``

Reserved for PCF and PCSS
The lowest quality but the fastest.

Execute PCF on a 1*1 kernel.

Execute PCSS with 16 taps blocker search and 16 taps PCF.

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[QUALITY_LOW](ShadowGenerator.md#quality_low)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:219

___

### QUALITY\_MEDIUM

▪ `Static` `Readonly` **QUALITY\_MEDIUM**: ``1``

Reserved for PCF and PCSS
Good tradeoff for quality/perf cross devices

Execute PCF on a 3*3 kernel.

Execute PCSS with 16 taps blocker search and 32 taps PCF.

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[QUALITY_MEDIUM](ShadowGenerator.md#quality_medium)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:210

___

### \_FrustumCornersNDCSpace

▪ `Static` `Private` `Readonly` **\_FrustumCornersNDCSpace**: [`Vector3`](Vector3.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:47

## Accessors

### autoCalcDepthBounds

• `get` **autoCalcDepthBounds**(): `boolean`

Gets or sets the autoCalcDepthBounds property.

When enabled, a depth rendering pass is first performed (with an internally created depth renderer or with the one
you provide by calling setDepthRenderer). Then, a min/max reducing is applied on the depth map to compute the
minimal and maximal depth of the map and those values are used as inputs for the setMinMaxDistance() function.
It can greatly enhance the shadow quality, at the expense of more GPU works.
When using this option, you should increase the value of the lambda parameter, and even set it to 1 for best results.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:445

• `set` **autoCalcDepthBounds**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:449

___

### autoCalcDepthBoundsRefreshRate

• `get` **autoCalcDepthBoundsRefreshRate**(): `number`

Defines the refresh rate of the min/max computation used when autoCalcDepthBounds is set to true
Use 0 to compute just once, 1 to compute on every frame, 2 to compute every two frames and so on...
Note that if you provided your own depth renderer through a call to setDepthRenderer, you are responsible
for setting the refresh rate on the renderer yourself!

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:491

• `set` **autoCalcDepthBoundsRefreshRate**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:495

___

### bias

• `get` **bias**(): `number`

Gets the bias: offset applied on the depth preventing acnea (in light direction).

#### Returns

`number`

#### Inherited from

ShadowGenerator.bias

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

#### Inherited from

ShadowGenerator.bias

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:267

___

### blurBoxOffset

• `get` **blurBoxOffset**(): `number`

Gets the blur box offset: offset applied during the blur pass.
Only useful if useKernelBlur = false

#### Returns

`number`

#### Inherited from

ShadowGenerator.blurBoxOffset

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

#### Inherited from

ShadowGenerator.blurBoxOffset

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:297

___

### blurKernel

• `get` **blurKernel**(): `number`

Gets the blur kernel: kernel size of the blur pass.
Only useful if useKernelBlur = true

#### Returns

`number`

#### Inherited from

ShadowGenerator.blurKernel

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

#### Inherited from

ShadowGenerator.blurKernel

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:339

___

### blurScale

• `get` **blurScale**(): `number`

Gets the blur scale: scale of the blurred texture compared to the main shadow map.
2 means half of the size.

#### Returns

`number`

#### Inherited from

ShadowGenerator.blurScale

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

#### Inherited from

ShadowGenerator.blurScale

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:318

___

### cascadeBlendPercentage

• `get` **cascadeBlendPercentage**(): `number`

Gets or sets the percentage of blending between two cascades (value between 0. and 1.).
It defaults to 0.1 (10% blending).

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:358

• `set` **cascadeBlendPercentage**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:362

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

#### Inherited from

ShadowGenerator.contactHardeningLightSizeUVRatio

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

#### Inherited from

ShadowGenerator.contactHardeningLightSizeUVRatio

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:614

___

### darkness

• `get` **darkness**(): `number`

Gets or sets the actual darkness of a shadow

#### Returns

`number`

#### Inherited from

ShadowGenerator.darkness

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:621

• `set` **darkness**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

ShadowGenerator.darkness

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:625

___

### debug

• `get` **debug**(): `boolean`

Gets or sets the debug flag.
When enabled, the cascades are materialized by different colors on the screen.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:325

• `set` **debug**(`dbg`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `dbg` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:329

___

### depthClamp

• `get` **depthClamp**(): `boolean`

Gets or sets the depth clamping value.

When enabled, it improves the shadow quality because the near z plane of the light frustum don't need to be adjusted
to account for the shadow casters far away.

Note that this property is incompatible with PCSS filtering, so it won't be used in that case.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:344

• `set` **depthClamp**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:348

___

### depthScale

• `get` **depthScale**(): `number`

Gets the depth scale used in ESM mode.

#### Returns

`number`

#### Inherited from

ShadowGenerator.depthScale

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

#### Inherited from

ShadowGenerator.depthScale

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:380

___

### filter

• `get` **filter**(): `number`

Gets the current mode of the shadow generator (normal, PCF, ESM...).
The returned value is a number equal to one of the available mode defined in ShadowMap.FILTER_x like _FILTER_NONE

#### Returns

`number`

#### Inherited from

ShadowGenerator.filter

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

#### Inherited from

ShadowGenerator.filter

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:400

___

### filteringQuality

• `get` **filteringQuality**(): `number`

Gets the PCF or PCSS Quality.
Only valid if usePercentageCloserFiltering or usePercentageCloserFiltering is true.

#### Returns

`number`

#### Inherited from

ShadowGenerator.filteringQuality

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

#### Inherited from

ShadowGenerator.filteringQuality

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:562

___

### freezeShadowCastersBoundingInfo

• `get` **freezeShadowCastersBoundingInfo**(): `boolean`

Enables or disables the shadow casters bounding info computation.
If your shadow casters don't move, you can disable this feature.
If it is enabled, the bounding box computation is done every frame.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:125

• `set` **freezeShadowCastersBoundingInfo**(`freeze`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `freeze` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:129

___

### lambda

• `get` **lambda**(): `number`

Gets or set the lambda parameter.
This parameter is used to split the camera frustum and create the cascades.
It's a value between 0. and 1.: If 0, the split is a uniform split of the frustum, if 1 it is a logarithmic split.
For all values in-between, it's a linear combination of the uniform and logarithm split algorithm.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:375

• `set` **lambda**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:379

___

### mapSize

• `get` **mapSize**(): `number`

Gets or sets the size of the texture what stores the shadows

#### Returns

`number`

#### Inherited from

ShadowGenerator.mapSize

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:832

• `set` **mapSize**(`size`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `size` | `number` |

#### Returns

`void`

#### Inherited from

ShadowGenerator.mapSize

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:836

___

### maxDistance

• `get` **maxDistance**(): `number`

Gets the maximal distance used in the cascade break computation

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:245

___

### minDistance

• `get` **minDistance**(): `number`

Gets the minimal distance used in the cascade break computation

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:240

___

### normalBias

• `get` **normalBias**(): `number`

Gets the normalBias: offset applied on the depth preventing acnea (along side the normal direction and proportional to the light/normal angle).

#### Returns

`number`

#### Inherited from

ShadowGenerator.normalBias

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

#### Inherited from

ShadowGenerator.normalBias

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:281

___

### numCascades

• `get` **numCascades**(): `number`

Gets or set the number of cascades used by the CSM.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:96

• `set` **numCascades**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:100

___

### shadowCastersBoundingInfo

• `get` **shadowCastersBoundingInfo**(): [`BoundingInfo`](BoundingInfo.md)

Gets or sets the shadow casters bounding info.
If you provide your own shadow casters bounding info, first enable freezeShadowCastersBoundingInfo
so that the system won't overwrite the bounds you provide

#### Returns

[`BoundingInfo`](BoundingInfo.md)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:195

• `set` **shadowCastersBoundingInfo**(`boundingInfo`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `boundingInfo` | [`BoundingInfo`](BoundingInfo.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:199

___

### shadowMaxZ

• `get` **shadowMaxZ**(): `number`

Gets the shadow max z distance. It's the limit beyond which shadows are not displayed.
It defaults to camera.maxZ

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:297

• `set` **shadowMaxZ**(`value`): `void`

Sets the shadow max z distance.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:306

___

### transparencyShadow

• `get` **transparencyShadow**(): `boolean`

Gets or sets the ability to have transparent shadow

#### Returns

`boolean`

#### Inherited from

ShadowGenerator.transparencyShadow

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:656

• `set` **transparencyShadow**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

ShadowGenerator.transparencyShadow

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:660

___

### useBlurCloseExponentialShadowMap

• `get` **useBlurCloseExponentialShadowMap**(): `boolean`

Gets if the current filter is set to filtered "close ESM" (using the inverse of the
exponential to prevent steep falloff artifacts).

#### Returns

`boolean`

#### Inherited from

ShadowGenerator.useBlurCloseExponentialShadowMap

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

#### Inherited from

ShadowGenerator.useBlurCloseExponentialShadowMap

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:523

___

### useBlurExponentialShadowMap

• `get` **useBlurExponentialShadowMap**(): `boolean`

Gets if the current filter is set to filtered ESM.

#### Returns

`boolean`

#### Inherited from

ShadowGenerator.useBlurExponentialShadowMap

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

#### Inherited from

ShadowGenerator.useBlurExponentialShadowMap

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:483

___

### useCloseExponentialShadowMap

• `get` **useCloseExponentialShadowMap**(): `boolean`

Gets if the current filter is set to "close ESM" (using the inverse of the
exponential to prevent steep falloff artifacts).

#### Returns

`boolean`

#### Inherited from

ShadowGenerator.useCloseExponentialShadowMap

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

#### Inherited from

ShadowGenerator.useCloseExponentialShadowMap

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:503

___

### useContactHardeningShadow

• `get` **useContactHardeningShadow**(): `boolean`

Gets if the current filter is set to "PCSS" (contact hardening).

#### Returns

`boolean`

#### Inherited from

ShadowGenerator.useContactHardeningShadow

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

#### Inherited from

ShadowGenerator.useContactHardeningShadow

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:583

___

### useExponentialShadowMap

• `get` **useExponentialShadowMap**(): `boolean`

Gets if the current filter is set to ESM.

#### Returns

`boolean`

#### Inherited from

ShadowGenerator.useExponentialShadowMap

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

#### Inherited from

ShadowGenerator.useExponentialShadowMap

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:465

___

### useKernelBlur

• `get` **useKernelBlur**(): `boolean`

Gets whether the blur pass is a kernel blur (if true) or box blur.
Only useful in filtered mode (useBlurExponentialShadowMap...)

#### Returns

`boolean`

#### Inherited from

ShadowGenerator.useKernelBlur

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

#### Inherited from

ShadowGenerator.useKernelBlur

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:360

___

### usePercentageCloserFiltering

• `get` **usePercentageCloserFiltering**(): `boolean`

Gets if the current filter is set to "PCF" (percentage closer filtering).

#### Returns

`boolean`

#### Inherited from

ShadowGenerator.usePercentageCloserFiltering

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

#### Inherited from

ShadowGenerator.usePercentageCloserFiltering

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:541

___

### usePoissonSampling

• `get` **usePoissonSampling**(): `boolean`

Gets if the current filter is set to Poisson Sampling.

#### Returns

`boolean`

#### Inherited from

ShadowGenerator.usePoissonSampling

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

#### Inherited from

ShadowGenerator.usePoissonSampling

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:446

___

### IsSupported

• `Static` `get` **IsSupported**(): `boolean`

Support test.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:721

## Methods

### \_applyFilterValues

▸ `Protected` **_applyFilterValues**(): `void`

#### Returns

`void`

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_applyFilterValues](ShadowGenerator.md#_applyfiltervalues)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:1310

___

### \_bindCustomEffectForRenderSubMeshForShadowMap

▸ `Protected` **_bindCustomEffectForRenderSubMeshForShadowMap**(`subMesh`, `effect`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `subMesh` | [`SubMesh`](SubMesh.md) |
| `effect` | [`Effect`](Effect.md) |

#### Returns

`void`

#### Overrides

[ShadowGenerator](ShadowGenerator.md).[_bindCustomEffectForRenderSubMeshForShadowMap](ShadowGenerator.md#_bindcustomeffectforrendersubmeshforshadowmap)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:876

___

### \_computeCascadeFrustum

▸ `Private` **_computeCascadeFrustum**(`cascadeIndex`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `cascadeIndex` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:661

___

### \_computeFrustumInWorldSpace

▸ `Private` **_computeFrustumInWorldSpace**(`cascadeIndex`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `cascadeIndex` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:626

___

### \_computeMatrices

▸ `Private` **_computeMatrices**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:545

___

### \_computeShadowCastersBoundingInfo

▸ `Protected` **_computeShadowCastersBoundingInfo**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:149

___

### \_createTargetRenderTexture

▸ `Protected` **_createTargetRenderTexture**(): `void`

#### Returns

`void`

#### Overrides

[ShadowGenerator](ShadowGenerator.md).[_createTargetRenderTexture](ShadowGenerator.md#_createtargetrendertexture)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:782

___

### \_disposeBlurPostProcesses

▸ `Protected` **_disposeBlurPostProcesses**(): `void`

#### Returns

`void`

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_disposeBlurPostProcesses](ShadowGenerator.md#_disposeblurpostprocesses)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:1866

___

### \_disposeRTTandPostProcesses

▸ `Protected` **_disposeRTTandPostProcesses**(): `void`

#### Returns

`void`

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_disposeRTTandPostProcesses](ShadowGenerator.md#_disposerttandpostprocesses)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:1890

___

### \_disposeSceneUBOs

▸ `Protected` **_disposeSceneUBOs**(): `void`

#### Returns

`void`

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_disposeSceneUBOs](ShadowGenerator.md#_disposesceneubos)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:1899

___

### \_initializeBlurRTTAndPostProcesses

▸ `Protected` **_initializeBlurRTTAndPostProcesses**(): `void`

#### Returns

`void`

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_initializeBlurRTTAndPostProcesses](ShadowGenerator.md#_initializeblurrttandpostprocesses)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:1019

___

### \_initializeGenerator

▸ `Protected` **_initializeGenerator**(): `void`

#### Returns

`void`

#### Overrides

[ShadowGenerator](ShadowGenerator.md).[_initializeGenerator](ShadowGenerator.md#_initializegenerator)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:757

___

### \_initializeShadowMap

▸ `Protected` **_initializeShadowMap**(): `void`

#### Returns

`void`

#### Overrides

[ShadowGenerator](ShadowGenerator.md).[_initializeShadowMap](ShadowGenerator.md#_initializeshadowmap)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:801

___

### \_isReadyCustomDefines

▸ `Protected` **_isReadyCustomDefines**(`defines`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `defines` | `any` |

#### Returns

`void`

#### Overrides

[ShadowGenerator](ShadowGenerator.md).[_isReadyCustomDefines](ShadowGenerator.md#_isreadycustomdefines)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:880

___

### \_recreateSceneUBOs

▸ `Protected` **_recreateSceneUBOs**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:709

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

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_renderForShadowMap](ShadowGenerator.md#_renderforshadowmap)

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

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[_renderSubMeshForShadowMap](ShadowGenerator.md#_rendersubmeshforshadowmap)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:1134

___

### \_splitFrustum

▸ `Private` **_splitFrustum**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:510

___

### \_validateFilter

▸ `Protected` **_validateFilter**(`filter`): `number`

#### Parameters

| Name | Type |
| :------ | :------ |
| `filter` | `number` |

#### Returns

`number`

#### Overrides

[ShadowGenerator](ShadowGenerator.md).[_validateFilter](ShadowGenerator.md#_validatefilter)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:76

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

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[addShadowCaster](ShadowGenerator.md#addshadowcaster)

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
| `effect` | [`Effect`](Effect.md) | The effect we are binfing the information for |

#### Returns

`void`

#### Overrides

[ShadowGenerator](ShadowGenerator.md).[bindShadowLight](ShadowGenerator.md#bindshadowlight)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:921

___

### dispose

▸ **dispose**(): `void`

Disposes the ShadowGenerator.
Returns nothing.

#### Returns

`void`

#### Overrides

[ShadowGenerator](ShadowGenerator.md).[dispose](ShadowGenerator.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:997

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

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[forceCompilation](ShadowGenerator.md#forcecompilation)

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

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[forceCompilationAsync](ShadowGenerator.md#forcecompilationasync)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:1393

___

### getCascadeMaxExtents

▸ **getCascadeMaxExtents**(`cascadeIndex`): [`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md)

Gets a cascade maximum extents

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `cascadeIndex` | `number` | index of the cascade |

#### Returns

[`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md)

the maximum cascade extents

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:274

___

### getCascadeMinExtents

▸ **getCascadeMinExtents**(`cascadeIndex`): [`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md)

Gets a cascade minimum extents

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `cascadeIndex` | `number` | index of the cascade |

#### Returns

[`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md)

the minimum cascade extents

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:265

___

### getCascadeProjectionMatrix

▸ **getCascadeProjectionMatrix**(`cascadeNum`): [`Nullable`](../modules.md#nullable)[`Matrix`](Matrix.md)

Gets the projection matrix corresponding to a given cascade

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `cascadeNum` | `number` | cascade to retrieve the projection matrix from |

#### Returns

[`Nullable`](../modules.md#nullable)[`Matrix`](Matrix.md)

the cascade projection matrix

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:402

___

### getCascadeTransformMatrix

▸ **getCascadeTransformMatrix**(`cascadeNum`): [`Nullable`](../modules.md#nullable)[`Matrix`](Matrix.md)

Gets the transformation matrix corresponding to a given cascade

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `cascadeNum` | `number` | cascade to retrieve the transformation matrix from |

#### Returns

[`Nullable`](../modules.md#nullable)[`Matrix`](Matrix.md)

the cascade transformation matrix

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:411

___

### getCascadeViewMatrix

▸ **getCascadeViewMatrix**(`cascadeNum`): [`Nullable`](../modules.md#nullable)[`Matrix`](Matrix.md)

Gets the view matrix corresponding to a given cascade

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `cascadeNum` | `number` | cascade to retrieve the view matrix from |

#### Returns

[`Nullable`](../modules.md#nullable)[`Matrix`](Matrix.md)

the cascade view matrix

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:393

___

### getClassName

▸ **getClassName**(): `string`

Gets the class name of that object

#### Returns

`string`

"CascadedShadowGenerator"

#### Overrides

[ShadowGenerator](ShadowGenerator.md).[getClassName](ShadowGenerator.md#getclassname)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:253

___

### getDarkness

▸ **getDarkness**(): `number`

Returns the darkness value (float). This can only decrease the actual darkness of a shadow.
0 means strongest and 1 would means no shadow.

#### Returns

`number`

the darkness.

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[getDarkness](ShadowGenerator.md#getdarkness)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:634

___

### getLight

▸ **getLight**(): [`IShadowLight`](../interfaces/IShadowLight.md)

Returns the associated light object.

#### Returns

[`IShadowLight`](../interfaces/IShadowLight.md)

the light generating the shadow

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[getLight](ShadowGenerator.md#getlight)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:786

___

### getShadowMap

▸ **getShadowMap**(): [`Nullable`](../modules.md#nullable)[`RenderTargetTexture`](RenderTargetTexture.md)

Gets the main RTT containing the shadow map (usually storing depth from the light point of view).

#### Returns

[`Nullable`](../modules.md#nullable)[`RenderTargetTexture`](RenderTargetTexture.md)

The render target texture if present otherwise, null

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[getShadowMap](ShadowGenerator.md#getshadowmap)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:696

___

### getShadowMapForRendering

▸ **getShadowMapForRendering**(): [`Nullable`](../modules.md#nullable)[`RenderTargetTexture`](RenderTargetTexture.md)

Gets the RTT used during rendering (can be a blurred version of the shadow map or the shadow map itself).

#### Returns

[`Nullable`](../modules.md#nullable)[`RenderTargetTexture`](RenderTargetTexture.md)

The render target texture if the shadow map is present otherwise, null

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[getShadowMapForRendering](ShadowGenerator.md#getshadowmapforrendering)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:704

___

### getTransformMatrix

▸ **getTransformMatrix**(): [`Matrix`](Matrix.md)

Gets the transformation matrix of the first cascade used to project the meshes into the map from the light point of view.
(eq to view projection * shadow projection matrices)

#### Returns

[`Matrix`](Matrix.md)

The transform matrix used to create the shadow map

#### Overrides

[ShadowGenerator](ShadowGenerator.md).[getTransformMatrix](ShadowGenerator.md#gettransformmatrix)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:989

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

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[isReady](ShadowGenerator.md#isready)

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

#### Overrides

[ShadowGenerator](ShadowGenerator.md).[prepareDefines](ShadowGenerator.md#preparedefines)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:889

___

### recreateShadowMap

▸ **recreateShadowMap**(): `void`

Recreates the shadow map dependencies like RTT and post processes. This can be used during the switch between
Cube and 2D textures for instance.

#### Returns

`void`

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[recreateShadowMap](ShadowGenerator.md#recreateshadowmap)

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

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[removeShadowCaster](ShadowGenerator.md#removeshadowcaster)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:756

___

### serialize

▸ **serialize**(): `any`

Serializes the shadow generator setup to a json object.

#### Returns

`any`

The serialized JSON object

#### Overrides

[ShadowGenerator](ShadowGenerator.md).[serialize](ShadowGenerator.md#serialize)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:1015

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

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[setDarkness](ShadowGenerator.md#setdarkness)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:642

___

### setDepthRenderer

▸ **setDepthRenderer**(`depthRenderer`): `void`

Sets the depth renderer to use when autoCalcDepthBounds is enabled.

Note that if no depth renderer is set, a new one will be automatically created internally when necessary.

You should call this function if you already have a depth renderer enabled in your scene, to avoid
doing multiple depth rendering each frame. If you provide your own depth renderer, make sure it stores linear depth!

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `depthRenderer` | [`Nullable`](../modules.md#nullable)[`DepthRenderer`](DepthRenderer.md) | The depth renderer to use when autoCalcDepthBounds is enabled. If you pass null or don't call this function at all, a depth renderer will be automatically created |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:425

___

### setMinMaxDistance

▸ **setMinMaxDistance**(`min`, `max`): `void`

Sets the minimal and maximal distances to use when computing the cascade breaks.

The values of min / max are typically the depth zmin and zmax values of your scene, for a given frame.
If you don't know these values, simply leave them to their defaults and don't call this function.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `min` | `number` | minimal distance for the breaks (default to 0.) |
| `max` | `number` | maximal distance for the breaks (default to 1.) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:216

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

#### Inherited from

[ShadowGenerator](ShadowGenerator.md).[setTransparencyShadow](ShadowGenerator.md#settransparencyshadow)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGenerator.ts:669

___

### splitFrustum

▸ **splitFrustum**(): `void`

Create the cascade breaks according to the lambda, shadowMaxZ and min/max distance properties, as well as the camera near and far planes.
This function is automatically called when updating lambda, shadowMaxZ and min/max distances, however you should call it yourself if
you change the camera near/far planes!

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:506

___

### Parse

▸ `Static` **Parse**(`parsedShadowGenerator`, `scene`): [`ShadowGenerator`](ShadowGenerator.md)

Parses a serialized ShadowGenerator and returns a new ShadowGenerator.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `parsedShadowGenerator` | `any` | The JSON object to parse |
| `scene` | [`Scene`](Scene.md) | The scene to create the shadow map for |

#### Returns

[`ShadowGenerator`](ShadowGenerator.md)

The parsed shadow generator

#### Overrides

[ShadowGenerator](ShadowGenerator.md).[Parse](ShadowGenerator.md#parse)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/cascadedShadowGenerator.ts:1055
