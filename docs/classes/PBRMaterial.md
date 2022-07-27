[@dev/core](../README.md) / [Exports](../modules.md) / PBRMaterial

# Class: PBRMaterial

The Physically based material of BJS.

This offers the main features of a standard PBR material.
For more information, please refer to the documentation :
https://doc.babylonjs.com/how_to/physically_based_rendering

## Hierarchy

- [`PBRBaseMaterial`](PBRBaseMaterial.md)

  ↳ **`PBRMaterial`**

## Table of contents

### Constructors

- [constructor](PBRMaterial.md#constructor)

### Properties

- [\_activeEffect](PBRMaterial.md#_activeeffect)
- [\_alpha](PBRMaterial.md#_alpha)
- [\_backFaceCulling](PBRMaterial.md#_backfaceculling)
- [\_cacheHasRenderTargetTextures](PBRMaterial.md#_cachehasrendertargettextures)
- [\_cullBackFaces](PBRMaterial.md#_cullbackfaces)
- [\_drawWrapper](PBRMaterial.md#_drawwrapper)
- [\_eventInfo](PBRMaterial.md#_eventinfo)
- [\_imageProcessingConfiguration](PBRMaterial.md#_imageprocessingconfiguration)
- [\_needToBindSceneUbo](PBRMaterial.md#_needtobindsceneubo)
- [\_normalMatrix](PBRMaterial.md#_normalmatrix)
- [\_onEffectCreatedObservable](PBRMaterial.md#_oneffectcreatedobservable)
- [\_transparencyMode](PBRMaterial.md#_transparencymode)
- [albedoColor](PBRMaterial.md#albedocolor)
- [albedoTexture](PBRMaterial.md#albedotexture)
- [allowShaderHotSwapping](PBRMaterial.md#allowshaderhotswapping)
- [alphaCutOff](PBRMaterial.md#alphacutoff)
- [ambientColor](PBRMaterial.md#ambientcolor)
- [ambientTexture](PBRMaterial.md#ambienttexture)
- [ambientTextureImpactOnAnalyticalLights](PBRMaterial.md#ambienttextureimpactonanalyticallights)
- [ambientTextureStrength](PBRMaterial.md#ambienttexturestrength)
- [animations](PBRMaterial.md#animations)
- [anisotropy](PBRMaterial.md#anisotropy)
- [brdf](PBRMaterial.md#brdf)
- [bumpTexture](PBRMaterial.md#bumptexture)
- [checkReadyOnEveryCall](PBRMaterial.md#checkreadyoneverycall)
- [checkReadyOnlyOnce](PBRMaterial.md#checkreadyonlyonce)
- [clearCoat](PBRMaterial.md#clearcoat)
- [customShaderNameResolve](PBRMaterial.md#customshadernameresolve)
- [depthFunction](PBRMaterial.md#depthfunction)
- [detailMap](PBRMaterial.md#detailmap)
- [directIntensity](PBRMaterial.md#directintensity)
- [disableBumpMap](PBRMaterial.md#disablebumpmap)
- [disableColorWrite](PBRMaterial.md#disablecolorwrite)
- [disableDepthWrite](PBRMaterial.md#disabledepthwrite)
- [disableLighting](PBRMaterial.md#disablelighting)
- [doNotSerialize](PBRMaterial.md#donotserialize)
- [emissiveColor](PBRMaterial.md#emissivecolor)
- [emissiveIntensity](PBRMaterial.md#emissiveintensity)
- [emissiveTexture](PBRMaterial.md#emissivetexture)
- [enableSpecularAntiAliasing](PBRMaterial.md#enablespecularantialiasing)
- [environmentBRDFTexture](PBRMaterial.md#environmentbrdftexture)
- [environmentIntensity](PBRMaterial.md#environmentintensity)
- [forceAlphaTest](PBRMaterial.md#forcealphatest)
- [forceDepthWrite](PBRMaterial.md#forcedepthwrite)
- [forceIrradianceInFragment](PBRMaterial.md#forceirradianceinfragment)
- [forceNormalForward](PBRMaterial.md#forcenormalforward)
- [getRenderTargetTextures](PBRMaterial.md#getrendertargettextures)
- [id](PBRMaterial.md#id)
- [inspectableCustomProperties](PBRMaterial.md#inspectablecustomproperties)
- [invertNormalMapX](PBRMaterial.md#invertnormalmapx)
- [invertNormalMapY](PBRMaterial.md#invertnormalmapy)
- [iridescence](PBRMaterial.md#iridescence)
- [lightmapTexture](PBRMaterial.md#lightmaptexture)
- [maxSimultaneousLights](PBRMaterial.md#maxsimultaneouslights)
- [metadata](PBRMaterial.md#metadata)
- [metallic](PBRMaterial.md#metallic)
- [metallicF0Factor](PBRMaterial.md#metallicf0factor)
- [metallicReflectanceColor](PBRMaterial.md#metallicreflectancecolor)
- [metallicReflectanceTexture](PBRMaterial.md#metallicreflectancetexture)
- [metallicTexture](PBRMaterial.md#metallictexture)
- [microSurface](PBRMaterial.md#microsurface)
- [microSurfaceTexture](PBRMaterial.md#microsurfacetexture)
- [name](PBRMaterial.md#name)
- [onCompiled](PBRMaterial.md#oncompiled)
- [onDisposeObservable](PBRMaterial.md#ondisposeobservable)
- [onError](PBRMaterial.md#onerror)
- [opacityTexture](PBRMaterial.md#opacitytexture)
- [parallaxScaleBias](PBRMaterial.md#parallaxscalebias)
- [pluginManager](PBRMaterial.md#pluginmanager)
- [pointSize](PBRMaterial.md#pointsize)
- [prePassConfiguration](PBRMaterial.md#prepassconfiguration)
- [reflectanceTexture](PBRMaterial.md#reflectancetexture)
- [reflectionColor](PBRMaterial.md#reflectioncolor)
- [reflectionTexture](PBRMaterial.md#reflectiontexture)
- [reflectivityColor](PBRMaterial.md#reflectivitycolor)
- [reflectivityTexture](PBRMaterial.md#reflectivitytexture)
- [reservedDataStore](PBRMaterial.md#reserveddatastore)
- [roughness](PBRMaterial.md#roughness)
- [separateCullingPass](PBRMaterial.md#separatecullingpass)
- [shadowDepthWrapper](PBRMaterial.md#shadowdepthwrapper)
- [sheen](PBRMaterial.md#sheen)
- [sideOrientation](PBRMaterial.md#sideorientation)
- [specularIntensity](PBRMaterial.md#specularintensity)
- [state](PBRMaterial.md#state)
- [stencil](PBRMaterial.md#stencil)
- [subSurface](PBRMaterial.md#subsurface)
- [twoSidedLighting](PBRMaterial.md#twosidedlighting)
- [uniqueId](PBRMaterial.md#uniqueid)
- [unlit](PBRMaterial.md#unlit)
- [useAlphaFresnel](PBRMaterial.md#usealphafresnel)
- [useAlphaFromAlbedoTexture](PBRMaterial.md#usealphafromalbedotexture)
- [useAmbientInGrayScale](PBRMaterial.md#useambientingrayscale)
- [useAmbientOcclusionFromMetallicTextureRed](PBRMaterial.md#useambientocclusionfrommetallictexturered)
- [useAutoMicroSurfaceFromReflectivityMap](PBRMaterial.md#useautomicrosurfacefromreflectivitymap)
- [useHorizonOcclusion](PBRMaterial.md#usehorizonocclusion)
- [useLightmapAsShadowmap](PBRMaterial.md#uselightmapasshadowmap)
- [useLinearAlphaFresnel](PBRMaterial.md#uselinearalphafresnel)
- [useMetallnessFromMetallicTextureBlue](PBRMaterial.md#usemetallnessfrommetallictextureblue)
- [useMicroSurfaceFromReflectivityMapAlpha](PBRMaterial.md#usemicrosurfacefromreflectivitymapalpha)
- [useObjectSpaceNormalMap](PBRMaterial.md#useobjectspacenormalmap)
- [useOnlyMetallicFromMetallicReflectanceTexture](PBRMaterial.md#useonlymetallicfrommetallicreflectancetexture)
- [useParallax](PBRMaterial.md#useparallax)
- [useParallaxOcclusion](PBRMaterial.md#useparallaxocclusion)
- [useRadianceOcclusion](PBRMaterial.md#useradianceocclusion)
- [useRadianceOverAlpha](PBRMaterial.md#useradianceoveralpha)
- [useRoughnessFromMetallicTextureAlpha](PBRMaterial.md#useroughnessfrommetallictexturealpha)
- [useRoughnessFromMetallicTextureGreen](PBRMaterial.md#useroughnessfrommetallictexturegreen)
- [useSpecularOverAlpha](PBRMaterial.md#usespecularoveralpha)
- [zOffset](PBRMaterial.md#zoffset)
- [zOffsetUnits](PBRMaterial.md#zoffsetunits)
- [AllDirtyFlag](PBRMaterial.md#alldirtyflag)
- [AttributesDirtyFlag](PBRMaterial.md#attributesdirtyflag)
- [ClockWiseSideOrientation](PBRMaterial.md#clockwisesideorientation)
- [CounterClockWiseSideOrientation](PBRMaterial.md#counterclockwisesideorientation)
- [DEFAULT\_AO\_ON\_ANALYTICAL\_LIGHTS](PBRMaterial.md#default_ao_on_analytical_lights)
- [FresnelDirtyFlag](PBRMaterial.md#fresneldirtyflag)
- [LIGHTFALLOFF\_GLTF](PBRMaterial.md#lightfalloff_gltf)
- [LIGHTFALLOFF\_PHYSICAL](PBRMaterial.md#lightfalloff_physical)
- [LIGHTFALLOFF\_STANDARD](PBRMaterial.md#lightfalloff_standard)
- [LightDirtyFlag](PBRMaterial.md#lightdirtyflag)
- [LineListDrawMode](PBRMaterial.md#linelistdrawmode)
- [LineLoopDrawMode](PBRMaterial.md#lineloopdrawmode)
- [LineStripDrawMode](PBRMaterial.md#linestripdrawmode)
- [MATERIAL\_ALPHABLEND](PBRMaterial.md#material_alphablend)
- [MATERIAL\_ALPHATEST](PBRMaterial.md#material_alphatest)
- [MATERIAL\_ALPHATESTANDBLEND](PBRMaterial.md#material_alphatestandblend)
- [MATERIAL\_NORMALBLENDMETHOD\_RNM](PBRMaterial.md#material_normalblendmethod_rnm)
- [MATERIAL\_NORMALBLENDMETHOD\_WHITEOUT](PBRMaterial.md#material_normalblendmethod_whiteout)
- [MATERIAL\_OPAQUE](PBRMaterial.md#material_opaque)
- [MiscDirtyFlag](PBRMaterial.md#miscdirtyflag)
- [OnEventObservable](PBRMaterial.md#oneventobservable)
- [PBRMATERIAL\_ALPHABLEND](PBRMaterial.md#pbrmaterial_alphablend)
- [PBRMATERIAL\_ALPHATEST](PBRMaterial.md#pbrmaterial_alphatest)
- [PBRMATERIAL\_ALPHATESTANDBLEND](PBRMaterial.md#pbrmaterial_alphatestandblend)
- [PBRMATERIAL\_OPAQUE](PBRMaterial.md#pbrmaterial_opaque)
- [PointFillMode](PBRMaterial.md#pointfillmode)
- [PointListDrawMode](PBRMaterial.md#pointlistdrawmode)
- [PrePassDirtyFlag](PBRMaterial.md#prepassdirtyflag)
- [TextureDirtyFlag](PBRMaterial.md#texturedirtyflag)
- [TriangleFanDrawMode](PBRMaterial.md#trianglefandrawmode)
- [TriangleFillMode](PBRMaterial.md#trianglefillmode)
- [TriangleStripDrawMode](PBRMaterial.md#trianglestripdrawmode)
- [WireFrameFillMode](PBRMaterial.md#wireframefillmode)

### Accessors

- [\_disableAlphaBlending](PBRMaterial.md#_disablealphablending)
- [alpha](PBRMaterial.md#alpha)
- [alphaMode](PBRMaterial.md#alphamode)
- [backFaceCulling](PBRMaterial.md#backfaceculling)
- [cameraColorCurves](PBRMaterial.md#cameracolorcurves)
- [cameraColorCurvesEnabled](PBRMaterial.md#cameracolorcurvesenabled)
- [cameraColorGradingEnabled](PBRMaterial.md#cameracolorgradingenabled)
- [cameraColorGradingTexture](PBRMaterial.md#cameracolorgradingtexture)
- [cameraContrast](PBRMaterial.md#cameracontrast)
- [cameraExposure](PBRMaterial.md#cameraexposure)
- [cameraToneMappingEnabled](PBRMaterial.md#cameratonemappingenabled)
- [canRenderToMRT](PBRMaterial.md#canrendertomrt)
- [cullBackFaces](PBRMaterial.md#cullbackfaces)
- [fillMode](PBRMaterial.md#fillmode)
- [fogEnabled](PBRMaterial.md#fogenabled)
- [hasRenderTargetTextures](PBRMaterial.md#hasrendertargettextures)
- [imageProcessingConfiguration](PBRMaterial.md#imageprocessingconfiguration)
- [indexOfRefraction](PBRMaterial.md#indexofrefraction)
- [invertRefractionY](PBRMaterial.md#invertrefractiony)
- [isFrozen](PBRMaterial.md#isfrozen)
- [isPrePassCapable](PBRMaterial.md#isprepasscapable)
- [linkRefractionWithTransparency](PBRMaterial.md#linkrefractionwithtransparency)
- [needDepthPrePass](PBRMaterial.md#needdepthprepass)
- [onBind](PBRMaterial.md#onbind)
- [onBindObservable](PBRMaterial.md#onbindobservable)
- [onDispose](PBRMaterial.md#ondispose)
- [onEffectCreatedObservable](PBRMaterial.md#oneffectcreatedobservable)
- [onUnBindObservable](PBRMaterial.md#onunbindobservable)
- [pointsCloud](PBRMaterial.md#pointscloud)
- [realTimeFiltering](PBRMaterial.md#realtimefiltering)
- [realTimeFilteringQuality](PBRMaterial.md#realtimefilteringquality)
- [refractionTexture](PBRMaterial.md#refractiontexture)
- [transparencyMode](PBRMaterial.md#transparencymode)
- [useGLTFLightFalloff](PBRMaterial.md#usegltflightfalloff)
- [useLogarithmicDepth](PBRMaterial.md#uselogarithmicdepth)
- [usePhysicalLightFalloff](PBRMaterial.md#usephysicallightfalloff)
- [wireframe](PBRMaterial.md#wireframe)

### Methods

- [\_afterBind](PBRMaterial.md#_afterbind)
- [\_attachImageProcessingConfiguration](PBRMaterial.md#_attachimageprocessingconfiguration)
- [\_hasAlphaChannel](PBRMaterial.md#_hasalphachannel)
- [\_isReadyForSubMesh](PBRMaterial.md#_isreadyforsubmesh)
- [\_markAllSubMeshesAsAllDirty](PBRMaterial.md#_markallsubmeshesasalldirty)
- [\_markAllSubMeshesAsAttributesDirty](PBRMaterial.md#_markallsubmeshesasattributesdirty)
- [\_markAllSubMeshesAsDirty](PBRMaterial.md#_markallsubmeshesasdirty)
- [\_markAllSubMeshesAsFresnelAndMiscDirty](PBRMaterial.md#_markallsubmeshesasfresnelandmiscdirty)
- [\_markAllSubMeshesAsFresnelDirty](PBRMaterial.md#_markallsubmeshesasfresneldirty)
- [\_markAllSubMeshesAsImageProcessingDirty](PBRMaterial.md#_markallsubmeshesasimageprocessingdirty)
- [\_markAllSubMeshesAsLightsDirty](PBRMaterial.md#_markallsubmeshesaslightsdirty)
- [\_markAllSubMeshesAsMiscDirty](PBRMaterial.md#_markallsubmeshesasmiscdirty)
- [\_markAllSubMeshesAsPrePassDirty](PBRMaterial.md#_markallsubmeshesasprepassdirty)
- [\_markAllSubMeshesAsTexturesAndMiscDirty](PBRMaterial.md#_markallsubmeshesastexturesandmiscdirty)
- [\_markAllSubMeshesAsTexturesDirty](PBRMaterial.md#_markallsubmeshesastexturesdirty)
- [\_markScenePrePassDirty](PBRMaterial.md#_marksceneprepassdirty)
- [\_mustRebind](PBRMaterial.md#_mustrebind)
- [\_shouldTurnAlphaTestOn](PBRMaterial.md#_shouldturnalphateston)
- [\_shouldUseAlphaFromAlbedoTexture](PBRMaterial.md#_shouldusealphafromalbedotexture)
- [bind](PBRMaterial.md#bind)
- [bindEyePosition](PBRMaterial.md#bindeyeposition)
- [bindForSubMesh](PBRMaterial.md#bindforsubmesh)
- [bindOnlyNormalMatrix](PBRMaterial.md#bindonlynormalmatrix)
- [bindOnlyWorldMatrix](PBRMaterial.md#bindonlyworldmatrix)
- [bindView](PBRMaterial.md#bindview)
- [bindViewProjection](PBRMaterial.md#bindviewprojection)
- [buildUniformLayout](PBRMaterial.md#builduniformlayout)
- [clone](PBRMaterial.md#clone)
- [dispose](PBRMaterial.md#dispose)
- [forceCompilation](PBRMaterial.md#forcecompilation)
- [forceCompilationAsync](PBRMaterial.md#forcecompilationasync)
- [freeze](PBRMaterial.md#freeze)
- [getActiveTextures](PBRMaterial.md#getactivetextures)
- [getAlphaTestTexture](PBRMaterial.md#getalphatesttexture)
- [getAnimatables](PBRMaterial.md#getanimatables)
- [getBindedMeshes](PBRMaterial.md#getbindedmeshes)
- [getClassName](PBRMaterial.md#getclassname)
- [getEffect](PBRMaterial.md#geteffect)
- [getScene](PBRMaterial.md#getscene)
- [hasTexture](PBRMaterial.md#hastexture)
- [isMetallicWorkflow](PBRMaterial.md#ismetallicworkflow)
- [isReady](PBRMaterial.md#isready)
- [isReadyForSubMesh](PBRMaterial.md#isreadyforsubmesh)
- [markAsDirty](PBRMaterial.md#markasdirty)
- [markDirty](PBRMaterial.md#markdirty)
- [needAlphaBlending](PBRMaterial.md#needalphablending)
- [needAlphaBlendingForMesh](PBRMaterial.md#needalphablendingformesh)
- [needAlphaTesting](PBRMaterial.md#needalphatesting)
- [resetDrawCache](PBRMaterial.md#resetdrawcache)
- [serialize](PBRMaterial.md#serialize)
- [setPrePassRenderer](PBRMaterial.md#setprepassrenderer)
- [toString](PBRMaterial.md#tostring)
- [unbind](PBRMaterial.md#unbind)
- [unfreeze](PBRMaterial.md#unfreeze)
- [Parse](PBRMaterial.md#parse)

## Constructors

### constructor

• **new PBRMaterial**(`name`, `scene?`)

Instantiates a new PBRMaterial instance.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | The material name |
| `scene?` | [`Scene`](Scene.md) | The scene the material will be use in. |

#### Overrides

[PBRBaseMaterial](PBRBaseMaterial.md).[constructor](PBRBaseMaterial.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:749

## Properties

### \_activeEffect

• `Protected` **\_activeEffect**: [`Effect`](Effect.md)

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[_activeEffect](PBRBaseMaterial.md#_activeeffect)

#### Defined in

https://github.com/babylon.js/core/src/Materials/pushMaterial.ts:14

___

### \_alpha

• `Protected` **\_alpha**: `number` = `1.0`

The alpha value of the material

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[_alpha](PBRBaseMaterial.md#_alpha)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:292

___

### \_backFaceCulling

• `Protected` **\_backFaceCulling**: `boolean` = `true`

Specifies if back face culling is enabled

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[_backFaceCulling](PBRBaseMaterial.md#_backfaceculling)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:328

___

### \_cacheHasRenderTargetTextures

• `Protected` **\_cacheHasRenderTargetTextures**: `boolean` = `false`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[_cacheHasRenderTargetTextures](PBRBaseMaterial.md#_cachehasrendertargettextures)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:888

___

### \_cullBackFaces

• `Protected` **\_cullBackFaces**: `boolean` = `true`

Specifies if back or front faces should be culled (when culling is enabled)

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[_cullBackFaces](PBRBaseMaterial.md#_cullbackfaces)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:352

___

### \_drawWrapper

• `Protected` **\_drawWrapper**: `DrawWrapper`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[_drawWrapper](PBRBaseMaterial.md#_drawwrapper)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:705

___

### \_eventInfo

• `Protected` **\_eventInfo**: `MaterialPluginDisposed` & `MaterialPluginHasTexture` & `MaterialPluginIsReadyForSubMesh` & `MaterialPluginGetDefineNames` & `MaterialPluginPrepareEffect` & `MaterialPluginPrepareDefines` & `MaterialPluginPrepareUniformBuffer` & `MaterialPluginBindForSubMesh` & `MaterialPluginGetAnimatables` & `MaterialPluginGetActiveTextures` & `MaterialPluginFillRenderTargetTextures` & `MaterialPluginHasRenderTargetTextures` & `MaterialPluginHardBindForSubMesh`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[_eventInfo](PBRBaseMaterial.md#_eventinfo)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:770

___

### \_imageProcessingConfiguration

• `Protected` **\_imageProcessingConfiguration**: [`ImageProcessingConfiguration`](ImageProcessingConfiguration.md)

Default configuration related to image processing available in the PBR Material.

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[_imageProcessingConfiguration](PBRBaseMaterial.md#_imageprocessingconfiguration)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:764

___

### \_needToBindSceneUbo

• `Protected` **\_needToBindSceneUbo**: `boolean`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[_needToBindSceneUbo](PBRBaseMaterial.md#_needtobindsceneubo)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:727

___

### \_normalMatrix

• `Protected` **\_normalMatrix**: [`Matrix`](Matrix.md)

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[_normalMatrix](PBRBaseMaterial.md#_normalmatrix)

#### Defined in

https://github.com/babylon.js/core/src/Materials/pushMaterial.ts:16

___

### \_onEffectCreatedObservable

• `Protected` **\_onEffectCreatedObservable**: [`Nullable`](../modules.md#nullable)[`Observable`](Observable.md){ `effect`: [`Effect`](Effect.md) ; `subMesh`: [`Nullable`](../modules.md#nullable)[`SubMesh`](SubMesh.md)  }

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[_onEffectCreatedObservable](PBRBaseMaterial.md#_oneffectcreatedobservable)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:477

___

### \_transparencyMode

• `Protected` **\_transparencyMode**: [`Nullable`](../modules.md#nullable)`number` = `null`

The transparency mode of the material.

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[_transparencyMode](PBRBaseMaterial.md#_transparencymode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:959

___

### albedoColor

• **albedoColor**: [`Color3`](Color3.md)

AKA Diffuse Color in other nomenclature.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:269

___

### albedoTexture

• **albedoTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

AKA Diffuse Texture in standard nomenclature.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:91

___

### allowShaderHotSwapping

• **allowShaderHotSwapping**: `boolean` = `true`

Gets or sets a boolean indicating that the material is allowed (if supported) to do shader hot swapping.
This means that the material can keep using a previous shader while a new one is being compiled.
This is mostly used when shader parallel compilation is supported (true by default)

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[allowShaderHotSwapping](PBRBaseMaterial.md#allowshaderhotswapping)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:227

___

### alphaCutOff

• **alphaCutOff**: `number` = `0.4`

Defines the alpha limits in alpha test mode.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:364

___

### ambientColor

• **ambientColor**: [`Color3`](Color3.md)

The color of a material in ambient lighting.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:262

___

### ambientTexture

• **ambientTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

AKA Occlusion Texture in other nomenclature.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:98

___

### ambientTextureImpactOnAnalyticalLights

• **ambientTextureImpactOnAnalyticalLights**: `number` = `PBRMaterial.DEFAULT_AO_ON_ANALYTICAL_LIGHTS`

Defines how much the AO map is occluding the analytical lights (point spot...).
1 means it completely occludes it
0 mean it has no impact

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:114

___

### ambientTextureStrength

• **ambientTextureStrength**: `number` = `1.0`

AKA Occlusion Texture Intensity in other nomenclature.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:105

___

### animations

• **animations**: [`Nullable`](../modules.md#nullable)[`Animation`](Animation.md)[] = `null`

Stores the animations for the material

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[animations](PBRBaseMaterial.md#animations)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:415

___

### anisotropy

• `Readonly` **anisotropy**: [`PBRAnisotropicConfiguration`](PBRAnisotropicConfiguration.md)

Defines the anisotropic parameters for the material.

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[anisotropy](PBRBaseMaterial.md#anisotropy)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:861

___

### brdf

• `Readonly` **brdf**: `PBRBRDFConfiguration`

Defines the BRDF parameters for the material.

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[brdf](PBRBaseMaterial.md#brdf)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:866

___

### bumpTexture

• **bumpTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Stores surface normal data used to displace a mesh in a texture.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:233

___

### checkReadyOnEveryCall

• **checkReadyOnEveryCall**: `boolean` = `false`

Specifies if the ready state should be checked on each call

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[checkReadyOnEveryCall](PBRBaseMaterial.md#checkreadyoneverycall)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:265

___

### checkReadyOnlyOnce

• **checkReadyOnlyOnce**: `boolean` = `false`

Specifies if the ready state should be checked once

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[checkReadyOnlyOnce](PBRBaseMaterial.md#checkreadyonlyonce)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:271

___

### clearCoat

• `Readonly` **clearCoat**: [`PBRClearCoatConfiguration`](PBRClearCoatConfiguration.md)

Defines the clear coat layer parameters for the material.

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[clearCoat](PBRBaseMaterial.md#clearcoat)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:851

___

### customShaderNameResolve

• **customShaderNameResolve**: (`shaderName`: `string`, `uniforms`: `string`[], `uniformBuffers`: `string`[], `samplers`: `string`[], `defines`: `string`[] \| [`MaterialDefines`](MaterialDefines.md), `attributes?`: `string`[], `options?`: [`ICustomShaderNameResolveOptions`](../interfaces/ICustomShaderNameResolveOptions.md)) => `string`

#### Type declaration

▸ (`shaderName`, `uniforms`, `uniformBuffers`, `samplers`, `defines`, `attributes?`, `options?`): `string`

Custom callback helping to override the default shader used in the material.

##### Parameters

| Name | Type |
| :------ | :------ |
| `shaderName` | `string` |
| `uniforms` | `string`[] |
| `uniformBuffers` | `string`[] |
| `samplers` | `string`[] |
| `defines` | `string`[] \| [`MaterialDefines`](MaterialDefines.md) |
| `attributes?` | `string`[] |
| `options?` | [`ICustomShaderNameResolveOptions`](../interfaces/ICustomShaderNameResolveOptions.md) |

##### Returns

`string`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[customShaderNameResolve](PBRBaseMaterial.md#customshadernameresolve)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:207

___

### depthFunction

• **depthFunction**: `number` = `0`

Specifies the depth function that should be used. 0 means the default engine function

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[depthFunction](PBRBaseMaterial.md#depthfunction)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:584

___

### detailMap

• `Readonly` **detailMap**: [`DetailMapConfiguration`](DetailMapConfiguration.md)

Defines the detail map parameters for the material.

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[detailMap](PBRBaseMaterial.md#detailmap)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:886

___

### directIntensity

• **directIntensity**: `number` = `1.0`

Intensity of the direct lights e.g. the four lights available in your scene.
This impacts both the direct diffuse and specular highlights.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:53

___

### disableBumpMap

• **disableBumpMap**: `boolean` = `false`

Debug Control allowing disabling the bump map on this material.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:84

___

### disableColorWrite

• **disableColorWrite**: `boolean` = `false`

Specifies if color writing should be disabled

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[disableColorWrite](PBRBaseMaterial.md#disablecolorwrite)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:572

___

### disableDepthWrite

• **disableDepthWrite**: `boolean` = `false`

Specifies if depth writing should be disabled

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[disableDepthWrite](PBRBaseMaterial.md#disabledepthwrite)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:566

___

### disableLighting

• **disableLighting**: `boolean` = `false`

If sets to true, disables all the lights affecting the material.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:519

___

### doNotSerialize

• **doNotSerialize**: `boolean` = `false`

Specifies if the material should be serialized

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[doNotSerialize](PBRBaseMaterial.md#donotserialize)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:405

___

### emissiveColor

• **emissiveColor**: [`Color3`](Color3.md)

The color emitted from the material.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:290

___

### emissiveIntensity

• **emissiveIntensity**: `number` = `1.0`

Intensity of the emissive part of the material.
This helps controlling the emissive effect without modifying the emissive color.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:61

___

### emissiveTexture

• **emissiveTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Stores the emissive values in a texture.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:135

___

### enableSpecularAntiAliasing

• **enableSpecularAntiAliasing**: `boolean` = `false`

Enables specular anti aliasing in the PBR shader.
It will both interacts on the Geometry for analytical and IBL lighting.
It also prefilter the roughness map based on the bump values.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:597

___

### environmentBRDFTexture

• **environmentBRDFTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) = `null`

Let user defines the brdf lookup texture used for IBL.
A default 8bit version is embedded but you could point at :
* Default texture: https://assets.babylonjs.com/environments/correlatedMSBRDF_RGBD.png
* Default 16bit pixel depth texture: https://assets.babylonjs.com/environments/correlatedMSBRDF.dds
* LEGACY Default None correlated https://assets.babylonjs.com/environments/uncorrelatedBRDF_RGBD.png
* LEGACY Default None correlated 16bit pixel depth https://assets.babylonjs.com/environments/uncorrelatedBRDF.dds

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:581

___

### environmentIntensity

• **environmentIntensity**: `number` = `1.0`

Intensity of the environment e.g. how much the environment will light the object
either through harmonics for rough material or through the reflection for shiny ones.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:69

___

### forceAlphaTest

• **forceAlphaTest**: `boolean` = `false`

Enforces alpha test in opaque or blend mode in order to improve the performances of some situations.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:357

___

### forceDepthWrite

• **forceDepthWrite**: `boolean` = `false`

Specifies if depth writing should be forced

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[forceDepthWrite](PBRBaseMaterial.md#forcedepthwrite)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:578

___

### forceIrradianceInFragment

• **forceIrradianceInFragment**: `boolean` = `false`

Force the shader to compute irradiance in the fragment shader in order to take bump in account.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:526

___

### forceNormalForward

• **forceNormalForward**: `boolean` = `false`

Force normal to face away from face.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:588

___

### getRenderTargetTextures

• **getRenderTargetTextures**: [`Nullable`](../modules.md#nullable)() => [`SmartArray`](SmartArray.md)[`RenderTargetTexture`](RenderTargetTexture.md) = `null`

Callback triggered to get the render target textures

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[getRenderTargetTextures](PBRBaseMaterial.md#getrendertargettextures)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:391

___

### id

• **id**: `string`

The ID of the material

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[id](PBRBaseMaterial.md#id)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:233

___

### inspectableCustomProperties

• **inspectableCustomProperties**: [`IInspectable`](../interfaces/IInspectable.md)[]

List of inspectable custom properties (used by the Inspector)

**`See`**

https://doc.babylonjs.com/how_to/debug_layer#extensibility

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[inspectableCustomProperties](PBRBaseMaterial.md#inspectablecustomproperties)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:298

___

### invertNormalMapX

• **invertNormalMapX**: `boolean` = `false`

If sets to true, x component of normal map value will invert (x = 1.0 - x).

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:540

___

### invertNormalMapY

• **invertNormalMapY**: `boolean` = `false`

If sets to true, y component of normal map value will invert (y = 1.0 - y).

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:547

___

### iridescence

• `Readonly` **iridescence**: [`PBRIridescenceConfiguration`](PBRIridescenceConfiguration.md)

Defines the iridescence layer parameters for the material.

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[iridescence](PBRBaseMaterial.md#iridescence)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:856

___

### lightmapTexture

• **lightmapTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Stores the pre-calculated light information of a mesh in a texture.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:240

___

### maxSimultaneousLights

• **maxSimultaneousLights**: `number` = `4`

Number of Simultaneous lights allowed on the material.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:533

___

### metadata

• **metadata**: `any` = `null`

Gets or sets user defined metadata

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[metadata](PBRBaseMaterial.md#metadata)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:254

___

### metallic

• **metallic**: [`Nullable`](../modules.md#nullable)`number`

Specifies the metallic scalar of the metallic/roughness workflow.
Can also be used to scale the metalness values of the metallic texture.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:157

___

### metallicF0Factor

• **metallicF0Factor**: `number` = `1`

In metallic workflow, specifies an F0 factor to help configuring the material F0.
By default the indexOfrefraction is used to compute F0;

This is used as a factor against the default reflectance at normal incidence to tweak it.

F0 = defaultF0 * metallicF0Factor * metallicReflectanceColor;
F90 = metallicReflectanceColor;

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:178

___

### metallicReflectanceColor

• **metallicReflectanceColor**: [`Color3`](Color3.md)

In metallic workflow, specifies an F90 color to help configuring the material F90.
By default the F90 is always 1;

Please note that this factor is also used as a factor against the default reflectance at normal incidence.

F0 = defaultF0 * metallicF0Factor * metallicReflectanceColor
F90 = metallicReflectanceColor;

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:191

___

### metallicReflectanceTexture

• **metallicReflectanceTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Defines to store metallicReflectanceColor in RGB and metallicF0Factor in A
This is multiplied against the scalar values defined in the material.
If useOnlyMetallicFromMetallicReflectanceTexture is true, don't use the RGB channels, only A

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:208

___

### metallicTexture

• **metallicTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Used to switch from specular/glossiness to metallic/roughness workflow.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:149

___

### microSurface

• **microSurface**: `number` = `1.0`

AKA Glossiness in other nomenclature.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:297

___

### microSurfaceTexture

• **microSurfaceTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Used to enable roughness/glossiness fetch from a separate channel depending on the current mode.
Gray Scale represents roughness in metallic mode and glossiness in specular mode.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:226

___

### name

• **name**: `string`

The name of the material

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[name](PBRBaseMaterial.md#name)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:248

___

### onCompiled

• **onCompiled**: [`Nullable`](../modules.md#nullable)(`effect`: [`Effect`](Effect.md)) => `void` = `null`

Callback triggered when the material is compiled

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[onCompiled](PBRBaseMaterial.md#oncompiled)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:381

___

### onDisposeObservable

• **onDisposeObservable**: [`Observable`](Observable.md)[`Material`](Material.md)

An event triggered when the material is disposed

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[onDisposeObservable](PBRBaseMaterial.md#ondisposeobservable)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:420

___

### onError

• **onError**: [`Nullable`](../modules.md#nullable)(`effect`: [`Effect`](Effect.md), `errors`: `string`) => `void` = `null`

Callback triggered when an error occurs

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[onError](PBRBaseMaterial.md#onerror)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:386

___

### opacityTexture

• **opacityTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Stores the alpha values in a texture. Use luminance if texture.getAlphaFromRGB is true.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:121

___

### parallaxScaleBias

• **parallaxScaleBias**: `number` = `0.05`

Controls the scale bias of the parallax mode.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:512

___

### pluginManager

• `Optional` **pluginManager**: [`MaterialPluginManager`](MaterialPluginManager.md)

Plugin manager for this material

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[pluginManager](PBRBaseMaterial.md#pluginmanager)

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginManager.ts:30

___

### pointSize

• **pointSize**: `number` = `1.0`

Stores the size of points

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[pointSize](PBRBaseMaterial.md#pointsize)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:620

___

### prePassConfiguration

• `Readonly` **prePassConfiguration**: `PrePassConfiguration`

Defines additional PrePass parameters for the material.

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[prePassConfiguration](PBRBaseMaterial.md#prepassconfiguration)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:881

___

### reflectanceTexture

• **reflectanceTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Defines to store reflectanceColor in RGB
This is multiplied against the scalar values defined in the material.
If both reflectanceTexture and metallicReflectanceTexture textures are provided and useOnlyMetallicFromMetallicReflectanceTexture
is false, metallicReflectanceTexture takes priority and reflectanceTexture is not used

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:218

___

### reflectionColor

• **reflectionColor**: [`Color3`](Color3.md)

The color reflected from the material.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:283

___

### reflectionTexture

• **reflectionTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Stores the reflection values in a texture.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:128

___

### reflectivityColor

• **reflectivityColor**: [`Color3`](Color3.md)

AKA Specular Color in other nomenclature.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:276

___

### reflectivityTexture

• **reflectivityTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

AKA Specular texture in other nomenclature.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:142

___

### reservedDataStore

• **reservedDataStore**: `any` = `null`

For internal use only. Please do not use.

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[reservedDataStore](PBRBaseMaterial.md#reserveddatastore)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:259

___

### roughness

• **roughness**: [`Nullable`](../modules.md#nullable)`number`

Specifies the roughness scalar of the metallic/roughness workflow.
Can also be used to scale the roughness values of the metallic texture.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:165

___

### separateCullingPass

• **separateCullingPass**: `boolean` = `false`

Specifies if there should be a separate pass for culling

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[separateCullingPass](PBRBaseMaterial.md#separatecullingpass)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:590

___

### shadowDepthWrapper

• **shadowDepthWrapper**: [`Nullable`](../modules.md#nullable)[`ShadowDepthWrapper`](ShadowDepthWrapper.md) = `null`

Custom shadow depth material to use for shadow rendering instead of the in-built one

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[shadowDepthWrapper](PBRBaseMaterial.md#shadowdepthwrapper)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:220

___

### sheen

• `Readonly` **sheen**: [`PBRSheenConfiguration`](PBRSheenConfiguration.md)

Defines the Sheen parameters for the material.

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[sheen](PBRBaseMaterial.md#sheen)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:871

___

### sideOrientation

• **sideOrientation**: `number`

Stores the value for side orientation

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[sideOrientation](PBRBaseMaterial.md#sideorientation)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:376

___

### specularIntensity

• **specularIntensity**: `number` = `1.0`

This is a special control allowing the reduction of the specular highlights coming from the
four lights of the scene. Those highlights may not be needed in full environment lighting.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:77

___

### state

• **state**: `string` = `""`

The state of the material

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[state](PBRBaseMaterial.md#state)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:277

___

### stencil

• `Readonly` **stencil**: `MaterialStencilState`

Gives access to the stencil properties of the material

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[stencil](PBRBaseMaterial.md#stencil)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:697

___

### subSurface

• `Readonly` **subSurface**: [`PBRSubSurfaceConfiguration`](PBRSubSurfaceConfiguration.md)

Defines the SubSurface parameters for the material.

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[subSurface](PBRBaseMaterial.md#subsurface)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:876

___

### twoSidedLighting

• **twoSidedLighting**: `boolean` = `false`

If sets to true and backfaceCulling is false, normals will be flipped on the backside.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:554

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the material

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[uniqueId](PBRBaseMaterial.md#uniqueid)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:239

___

### unlit

• **unlit**: `boolean` = `false`

If set to true, no lighting calculations will be applied.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:620

___

### useAlphaFresnel

• **useAlphaFresnel**: `boolean` = `false`

A fresnel is applied to the alpha of the model to ensure grazing angles edges are not alpha tested.
And/Or occlude the blended part. (alpha is converted to gamma to compute the fresnel)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:562

___

### useAlphaFromAlbedoTexture

• **useAlphaFromAlbedoTexture**: `boolean` = `false`

Specifies that the alpha is coming form the albedo channel alpha channel for alpha blending.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:350

___

### useAmbientInGrayScale

• **useAmbientInGrayScale**: `boolean` = `false`

Specifies if the ambient texture contains the ambient occlusion information in its red channel only.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:414

___

### useAmbientOcclusionFromMetallicTextureRed

• **useAmbientOcclusionFromMetallicTextureRed**: `boolean` = `false`

Specifies if the metallic texture contains the ambient occlusion information in its red channel.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:407

___

### useAutoMicroSurfaceFromReflectivityMap

• **useAutoMicroSurfaceFromReflectivityMap**: `boolean` = `false`

In case the reflectivity map does not contain the microsurface information in its alpha channel,
The material will try to infer what glossiness each pixel should be.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:422

___

### useHorizonOcclusion

• **useHorizonOcclusion**: `boolean` = `true`

This parameters will enable/disable Horizon occlusion to prevent normal maps to look shiny when the normal
makes the reflect vector face the model (under horizon).

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:605

___

### useLightmapAsShadowmap

• **useLightmapAsShadowmap**: `boolean` = `false`

If true, the light map contains occlusion information instead of lighting info.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:343

___

### useLinearAlphaFresnel

• **useLinearAlphaFresnel**: `boolean` = `false`

A fresnel is applied to the alpha of the model to ensure grazing angles edges are not alpha tested.
And/Or occlude the blended part. (alpha stays linear to compute the fresnel)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:570

___

### useMetallnessFromMetallicTextureBlue

• **useMetallnessFromMetallicTextureBlue**: `boolean` = `false`

Specifies if the metallic texture contains the metallness information in its blue channel.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:400

___

### useMicroSurfaceFromReflectivityMapAlpha

• **useMicroSurfaceFromReflectivityMapAlpha**: `boolean` = `false`

Specifies if the reflectivity texture contains the glossiness information in its alpha channel.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:379

___

### useObjectSpaceNormalMap

• **useObjectSpaceNormalMap**: `boolean` = `false`

Allows using an object space normal map (instead of tangent space).

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:491

___

### useOnlyMetallicFromMetallicReflectanceTexture

• **useOnlyMetallicFromMetallicReflectanceTexture**: `boolean` = `false`

Specifies that only the A channel from metallicReflectanceTexture should be used.
If false, both RGB and A channels will be used

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:199

___

### useParallax

• **useParallax**: `boolean` = `false`

Allows using the bump map in parallax mode.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:498

___

### useParallaxOcclusion

• **useParallaxOcclusion**: `boolean` = `false`

Allows using the bump map in parallax occlusion mode.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:505

___

### useRadianceOcclusion

• **useRadianceOcclusion**: `boolean` = `true`

This parameters will enable/disable radiance occlusion by preventing the radiance to lit
too much the area relying on ambient texture to define their ambient occlusion.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:613

___

### useRadianceOverAlpha

• **useRadianceOverAlpha**: `boolean` = `true`

Specifies that the material will keeps the reflection highlights over a transparent surface (only the most luminous ones).
A car glass is a good example of that. When the street lights reflects on it you can not see what is behind.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:484

___

### useRoughnessFromMetallicTextureAlpha

• **useRoughnessFromMetallicTextureAlpha**: `boolean` = `true`

Specifies if the metallic texture contains the roughness information in its alpha channel.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:386

___

### useRoughnessFromMetallicTextureGreen

• **useRoughnessFromMetallicTextureGreen**: `boolean` = `false`

Specifies if the metallic texture contains the roughness information in its green channel.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:393

___

### useSpecularOverAlpha

• **useSpecularOverAlpha**: `boolean` = `true`

Specifies that the material will keep the specular highlights over a transparent surface (only the most luminous ones).
A car glass is a good example of that. When sun reflects on it you can not see what is behind.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:372

___

### zOffset

• **zOffset**: `number` = `0`

Stores the z offset Factor value

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[zOffset](PBRBaseMaterial.md#zoffset)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:626

___

### zOffsetUnits

• **zOffsetUnits**: `number` = `0`

Stores the z offset Units value

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[zOffsetUnits](PBRBaseMaterial.md#zoffsetunits)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:632

___

### AllDirtyFlag

▪ `Static` `Readonly` **AllDirtyFlag**: ``63``

The all dirty flag value

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[AllDirtyFlag](PBRBaseMaterial.md#alldirtyflag)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:164

___

### AttributesDirtyFlag

▪ `Static` `Readonly` **AttributesDirtyFlag**: ``8``

The dirty attribute flag value

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[AttributesDirtyFlag](PBRBaseMaterial.md#attributesdirtyflag)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:149

___

### ClockWiseSideOrientation

▪ `Static` `Readonly` **ClockWiseSideOrientation**: ``0``

Stores the clock-wise side orientation

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[ClockWiseSideOrientation](PBRBaseMaterial.md#clockwisesideorientation)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:124

___

### CounterClockWiseSideOrientation

▪ `Static` `Readonly` **CounterClockWiseSideOrientation**: ``1``

Stores the counter clock-wise side orientation

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[CounterClockWiseSideOrientation](PBRBaseMaterial.md#counterclockwisesideorientation)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:129

___

### DEFAULT\_AO\_ON\_ANALYTICAL\_LIGHTS

▪ `Static` **DEFAULT\_AO\_ON\_ANALYTICAL\_LIGHTS**: `number` = `PBRBaseMaterial.DEFAULT_AO_ON_ANALYTICAL_LIGHTS`

Defines the default value of how much AO map is occluding the analytical lights
(point spot...).

#### Overrides

[PBRBaseMaterial](PBRBaseMaterial.md).[DEFAULT_AO_ON_ANALYTICAL_LIGHTS](PBRBaseMaterial.md#default_ao_on_analytical_lights)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:45

___

### FresnelDirtyFlag

▪ `Static` `Readonly` **FresnelDirtyFlag**: ``4``

The dirty fresnel flag value

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[FresnelDirtyFlag](PBRBaseMaterial.md#fresneldirtyflag)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:144

___

### LIGHTFALLOFF\_GLTF

▪ `Static` `Readonly` **LIGHTFALLOFF\_GLTF**: ``1``

PBRMaterialLightFalloff gltf: light is falling off as described in the gltf moving to PBR document
to enhance interoperability with other engines.

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[LIGHTFALLOFF_GLTF](PBRBaseMaterial.md#lightfalloff_gltf)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:312

___

### LIGHTFALLOFF\_PHYSICAL

▪ `Static` `Readonly` **LIGHTFALLOFF\_PHYSICAL**: ``0``

PBRMaterialLightFalloff Physical: light is falling off following the inverse squared distance law.

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[LIGHTFALLOFF_PHYSICAL](PBRBaseMaterial.md#lightfalloff_physical)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:306

___

### LIGHTFALLOFF\_STANDARD

▪ `Static` `Readonly` **LIGHTFALLOFF\_STANDARD**: ``2``

PBRMaterialLightFalloff Standard: light is falling off like in the standard material
to enhance interoperability with other materials.

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[LIGHTFALLOFF_STANDARD](PBRBaseMaterial.md#lightfalloff_standard)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:318

___

### LightDirtyFlag

▪ `Static` `Readonly` **LightDirtyFlag**: ``2``

The dirty light flag value

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[LightDirtyFlag](PBRBaseMaterial.md#lightdirtyflag)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:139

___

### LineListDrawMode

▪ `Static` `Readonly` **LineListDrawMode**: ``4``

Returns the line list draw mode

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[LineListDrawMode](PBRBaseMaterial.md#linelistdrawmode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:103

___

### LineLoopDrawMode

▪ `Static` `Readonly` **LineLoopDrawMode**: ``5``

Returns the line loop draw mode

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[LineLoopDrawMode](PBRBaseMaterial.md#lineloopdrawmode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:107

___

### LineStripDrawMode

▪ `Static` `Readonly` **LineStripDrawMode**: ``6``

Returns the line strip draw mode

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[LineStripDrawMode](PBRBaseMaterial.md#linestripdrawmode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:111

___

### MATERIAL\_ALPHABLEND

▪ `Static` `Readonly` **MATERIAL\_ALPHABLEND**: ``2``

MaterialTransparencyMode: Pixels are blended (according to the alpha mode) with the already drawn pixels in the current frame buffer.

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[MATERIAL_ALPHABLEND](PBRBaseMaterial.md#material_alphablend)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:179

___

### MATERIAL\_ALPHATEST

▪ `Static` `Readonly` **MATERIAL\_ALPHATEST**: ``1``

MaterialTransparencyMode: Alpha Test mode, pixel are discarded below a certain threshold defined by the alpha cutoff value.

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[MATERIAL_ALPHATEST](PBRBaseMaterial.md#material_alphatest)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:174

___

### MATERIAL\_ALPHATESTANDBLEND

▪ `Static` `Readonly` **MATERIAL\_ALPHATESTANDBLEND**: ``3``

MaterialTransparencyMode: Pixels are blended (according to the alpha mode) with the already drawn pixels in the current frame buffer.
They are also discarded below the alpha cutoff threshold to improve performances.

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[MATERIAL_ALPHATESTANDBLEND](PBRBaseMaterial.md#material_alphatestandblend)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:185

___

### MATERIAL\_NORMALBLENDMETHOD\_RNM

▪ `Static` `Readonly` **MATERIAL\_NORMALBLENDMETHOD\_RNM**: ``1``

The Reoriented Normal Mapping method is used to blend normals.
Details of the algorithm can be found here: https://blog.selfshadow.com/publications/blending-in-detail/

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[MATERIAL_NORMALBLENDMETHOD_RNM](PBRBaseMaterial.md#material_normalblendmethod_rnm)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:197

___

### MATERIAL\_NORMALBLENDMETHOD\_WHITEOUT

▪ `Static` `Readonly` **MATERIAL\_NORMALBLENDMETHOD\_WHITEOUT**: ``0``

The Whiteout method is used to blend normals.
Details of the algorithm can be found here: https://blog.selfshadow.com/publications/blending-in-detail/

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[MATERIAL_NORMALBLENDMETHOD_WHITEOUT](PBRBaseMaterial.md#material_normalblendmethod_whiteout)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:191

___

### MATERIAL\_OPAQUE

▪ `Static` `Readonly` **MATERIAL\_OPAQUE**: ``0``

MaterialTransparencyMode: No transparency mode, Alpha channel is not use.

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[MATERIAL_OPAQUE](PBRBaseMaterial.md#material_opaque)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:169

___

### MiscDirtyFlag

▪ `Static` `Readonly` **MiscDirtyFlag**: ``16``

The dirty misc flag value

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[MiscDirtyFlag](PBRBaseMaterial.md#miscdirtyflag)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:154

___

### OnEventObservable

▪ `Static` **OnEventObservable**: [`Observable`](Observable.md)[`Material`](Material.md)

Event observable which raises global events common to all materials (like MaterialPluginEvent.Created)

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[OnEventObservable](PBRBaseMaterial.md#oneventobservable)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:202

___

### PBRMATERIAL\_ALPHABLEND

▪ `Static` `Readonly` **PBRMATERIAL\_ALPHABLEND**: ``2``

PBRMaterialTransparencyMode: Pixels are blended (according to the alpha mode) with the already drawn pixels in the current frame buffer.

#### Overrides

[PBRBaseMaterial](PBRBaseMaterial.md).[PBRMATERIAL_ALPHABLEND](PBRBaseMaterial.md#pbrmaterial_alphablend)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:33

___

### PBRMATERIAL\_ALPHATEST

▪ `Static` `Readonly` **PBRMATERIAL\_ALPHATEST**: ``1``

PBRMaterialTransparencyMode: Alpha Test mode, pixel are discarded below a certain threshold defined by the alpha cutoff value.

#### Overrides

[PBRBaseMaterial](PBRBaseMaterial.md).[PBRMATERIAL_ALPHATEST](PBRBaseMaterial.md#pbrmaterial_alphatest)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:28

___

### PBRMATERIAL\_ALPHATESTANDBLEND

▪ `Static` `Readonly` **PBRMATERIAL\_ALPHATESTANDBLEND**: ``3``

PBRMaterialTransparencyMode: Pixels are blended (according to the alpha mode) with the already drawn pixels in the current frame buffer.
They are also discarded below the alpha cutoff threshold to improve performances.

#### Overrides

[PBRBaseMaterial](PBRBaseMaterial.md).[PBRMATERIAL_ALPHATESTANDBLEND](PBRBaseMaterial.md#pbrmaterial_alphatestandblend)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:39

___

### PBRMATERIAL\_OPAQUE

▪ `Static` `Readonly` **PBRMATERIAL\_OPAQUE**: ``0``

PBRMaterialTransparencyMode: No transparency mode, Alpha channel is not use.

#### Overrides

[PBRBaseMaterial](PBRBaseMaterial.md).[PBRMATERIAL_OPAQUE](PBRBaseMaterial.md#pbrmaterial_opaque)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:23

___

### PointFillMode

▪ `Static` `Readonly` **PointFillMode**: ``2``

Returns the point fill mode

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[PointFillMode](PBRBaseMaterial.md#pointfillmode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:95

___

### PointListDrawMode

▪ `Static` `Readonly` **PointListDrawMode**: ``3``

Returns the point list draw mode

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[PointListDrawMode](PBRBaseMaterial.md#pointlistdrawmode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:99

___

### PrePassDirtyFlag

▪ `Static` `Readonly` **PrePassDirtyFlag**: ``32``

The dirty prepass flag value

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[PrePassDirtyFlag](PBRBaseMaterial.md#prepassdirtyflag)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:159

___

### TextureDirtyFlag

▪ `Static` `Readonly` **TextureDirtyFlag**: ``1``

The dirty texture flag value

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[TextureDirtyFlag](PBRBaseMaterial.md#texturedirtyflag)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:134

___

### TriangleFanDrawMode

▪ `Static` `Readonly` **TriangleFanDrawMode**: ``8``

Returns the triangle fan draw mode

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[TriangleFanDrawMode](PBRBaseMaterial.md#trianglefandrawmode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:119

___

### TriangleFillMode

▪ `Static` `Readonly` **TriangleFillMode**: ``0``

Returns the triangle fill mode

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[TriangleFillMode](PBRBaseMaterial.md#trianglefillmode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:87

___

### TriangleStripDrawMode

▪ `Static` `Readonly` **TriangleStripDrawMode**: ``7``

Returns the triangle strip draw mode

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[TriangleStripDrawMode](PBRBaseMaterial.md#trianglestripdrawmode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:115

___

### WireFrameFillMode

▪ `Static` `Readonly` **WireFrameFillMode**: ``1``

Returns the wireframe mode

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[WireFrameFillMode](PBRBaseMaterial.md#wireframefillmode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:91

## Accessors

### \_disableAlphaBlending

• `Protected` `get` **_disableAlphaBlending**(): `boolean`

Returns true if alpha blending should be disabled.

#### Returns

`boolean`

#### Inherited from

PBRBaseMaterial.\_disableAlphaBlending

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:970

___

### alpha

• `get` **alpha**(): `number`

Gets the alpha value of the material

#### Returns

`number`

#### Inherited from

PBRBaseMaterial.alpha

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:320

• `set` **alpha**(`value`): `void`

Sets the alpha value of the material

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

PBRBaseMaterial.alpha

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:303

___

### alphaMode

• `get` **alphaMode**(): `number`

Gets the value of the alpha mode

#### Returns

`number`

#### Inherited from

PBRBaseMaterial.alphaMode

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:525

• `set` **alphaMode**(`value`): `void`

Sets the value of the alpha mode.

| Value | Type | Description |
| --- | --- | --- |
| 0 | ALPHA_DISABLE |   |
| 1 | ALPHA_ADD |   |
| 2 | ALPHA_COMBINE |   |
| 3 | ALPHA_SUBTRACT |   |
| 4 | ALPHA_MULTIPLY |   |
| 5 | ALPHA_MAXIMIZED |   |
| 6 | ALPHA_ONEONE |   |
| 7 | ALPHA_PREMULTIPLIED |   |
| 8 | ALPHA_PREMULTIPLIED_PORTERDUFF |   |
| 9 | ALPHA_INTERPOLATE |   |
| 10 | ALPHA_SCREENMODE |   |

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

PBRBaseMaterial.alphaMode

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:514

___

### backFaceCulling

• `get` **backFaceCulling**(): `boolean`

Gets the culling state

#### Returns

`boolean`

#### Inherited from

PBRBaseMaterial.backFaceCulling

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:344

• `set` **backFaceCulling**(`value`): `void`

Sets the culling state (true to enable culling, false to disable)

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

PBRBaseMaterial.backFaceCulling

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:333

___

### cameraColorCurves

• `get` **cameraColorCurves**(): [`Nullable`](../modules.md#nullable)[`ColorCurves`](ColorCurves.md)

The color grading curves provide additional color adjustment that is applied after any color grading transform (3D LUT).
They allow basic adjustment of saturation and small exposure adjustments, along with color filter tinting to provide white balance adjustment or more stylistic effects.
These are similar to controls found in many professional imaging or colorist software. The global controls are applied to the entire image. For advanced tuning, extra controls are provided to adjust the shadow, midtone and highlight areas of the image;
corresponding to low luminance, medium luminance, and high luminance areas respectively.

#### Returns

[`Nullable`](../modules.md#nullable)[`ColorCurves`](ColorCurves.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:730

• `set` **cameraColorCurves**(`value`): `void`

The color grading curves provide additional color adjustment that is applied after any color grading transform (3D LUT).
They allow basic adjustment of saturation and small exposure adjustments, along with color filter tinting to provide white balance adjustment or more stylistic effects.
These are similar to controls found in many professional imaging or colorist software. The global controls are applied to the entire image. For advanced tuning, extra controls are provided to adjust the shadow, midtone and highlight areas of the image;
corresponding to low luminance, medium luminance, and high luminance areas respectively.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`ColorCurves`](ColorCurves.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:739

___

### cameraColorCurvesEnabled

• `get` **cameraColorCurvesEnabled**(): `boolean`

Gets whether the color curves effect is enabled.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:644

• `set` **cameraColorCurvesEnabled**(`value`): `void`

Sets whether the color curves effect is enabled.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:650

___

### cameraColorGradingEnabled

• `get` **cameraColorGradingEnabled**(): `boolean`

Gets whether the color grading effect is enabled.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:657

• `set` **cameraColorGradingEnabled**(`value`): `void`

Gets whether the color grading effect is enabled.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:663

___

### cameraColorGradingTexture

• `get` **cameraColorGradingTexture**(): [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Gets the Color Grading 2D Lookup Texture.

#### Returns

[`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:714

• `set` **cameraColorGradingTexture**(`value`): `void`

Sets the Color Grading 2D Lookup Texture.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:720

___

### cameraContrast

• `get` **cameraContrast**(): `number`

Gets The camera contrast used on this material.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:700

• `set` **cameraContrast**(`value`): `void`

Sets The camera contrast used on this material.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:707

___

### cameraExposure

• `get` **cameraExposure**(): `number`

The camera exposure used on this material.
This property is here and not in the camera to allow controlling exposure without full screen post process.
This corresponds to a photographic exposure.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:685

• `set` **cameraExposure**(`value`): `void`

The camera exposure used on this material.
This property is here and not in the camera to allow controlling exposure without full screen post process.
This corresponds to a photographic exposure.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:693

___

### cameraToneMappingEnabled

• `get` **cameraToneMappingEnabled**(): `boolean`

Gets whether tonemapping is enabled or not.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:670

• `set` **cameraToneMappingEnabled**(`value`): `void`

Sets whether tonemapping is enabled or not

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:676

___

### canRenderToMRT

• `get` **canRenderToMRT**(): `boolean`

Can this material render to several textures at once

#### Returns

`boolean`

#### Inherited from

PBRBaseMaterial.canRenderToMRT

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:742

___

### cullBackFaces

• `get` **cullBackFaces**(): `boolean`

Gets the type of faces that should be culled

#### Returns

`boolean`

#### Inherited from

PBRBaseMaterial.cullBackFaces

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:368

• `set` **cullBackFaces**(`value`): `void`

Sets the type of faces that should be culled (true for back faces, false for front faces)

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

PBRBaseMaterial.cullBackFaces

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:357

___

### fillMode

• `get` **fillMode**(): `number`

Gets the material fill mode

#### Returns

`number`

#### Inherited from

PBRBaseMaterial.fillMode

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:677

• `set` **fillMode**(`value`): `void`

Sets the material fill mode

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

PBRBaseMaterial.fillMode

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:685

___

### fogEnabled

• `get` **fogEnabled**(): `boolean`

Gets the value of the fog enabled state

#### Returns

`boolean`

#### Inherited from

PBRBaseMaterial.fogEnabled

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:612

• `set` **fogEnabled**(`value`): `void`

Sets the state for enabling fog

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

PBRBaseMaterial.fogEnabled

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:601

___

### hasRenderTargetTextures

• `get` **hasRenderTargetTextures**(): `boolean`

Gets a boolean indicating that current material needs to register RTT

#### Returns

`boolean`

#### Inherited from

PBRBaseMaterial.hasRenderTargetTextures

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:930

___

### imageProcessingConfiguration

• `get` **imageProcessingConfiguration**(): [`ImageProcessingConfiguration`](ImageProcessingConfiguration.md)

Gets the image processing configuration used either in this material.

#### Returns

[`ImageProcessingConfiguration`](ImageProcessingConfiguration.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:625

• `set` **imageProcessingConfiguration**(`value`): `void`

Sets the Default image processing configuration used either in the this material.

If sets to null, the scene one is in use.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`ImageProcessingConfiguration`](ImageProcessingConfiguration.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:634

___

### indexOfRefraction

• `get` **indexOfRefraction**(): `number`

Index of refraction of the material base layer.
https://en.wikipedia.org/wiki/List_of_refractive_indices

This does not only impact refraction but also the Base F0 of Dielectric Materials.

From dielectric fresnel rules: F0 = square((iorT - iorI) / (iorT + iorI))

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:307

• `set` **indexOfRefraction**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:310

___

### invertRefractionY

• `get` **invertRefractionY**(): `boolean`

Controls if refraction needs to be inverted on Y. This could be useful for procedural texture.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:317

• `set` **invertRefractionY**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:320

___

### isFrozen

• `get` **isFrozen**(): `boolean`

Specifies if updates for the material been locked

#### Returns

`boolean`

#### Inherited from

PBRBaseMaterial.isFrozen

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:883

___

### isPrePassCapable

• `get` **isPrePassCapable**(): `boolean`

Can this material render to prepass

#### Returns

`boolean`

#### Inherited from

PBRBaseMaterial.isPrePassCapable

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:941

___

### linkRefractionWithTransparency

• `get` **linkRefractionWithTransparency**(): `boolean`

This parameters will make the material used its opacity to control how much it is refracting against not.
Materials half opaque for instance using refraction could benefit from this control.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:328

• `set` **linkRefractionWithTransparency**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:331

___

### needDepthPrePass

• `get` **needDepthPrePass**(): `boolean`

Gets the depth pre-pass value

#### Returns

`boolean`

#### Inherited from

PBRBaseMaterial.needDepthPrePass

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:551

• `set` **needDepthPrePass**(`value`): `void`

Sets the need depth pre-pass value

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

PBRBaseMaterial.needDepthPrePass

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:538

___

### onBind

• `set` **onBind**(`callback`): `void`

Called during a bind event

#### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | (`Mesh`: [`AbstractMesh`](AbstractMesh.md)) => `void` |

#### Returns

`void`

#### Inherited from

PBRBaseMaterial.onBind

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:459

___

### onBindObservable

• `get` **onBindObservable**(): [`Observable`](Observable.md)[`AbstractMesh`](AbstractMesh.md)

An event triggered when the material is bound

#### Returns

[`Observable`](Observable.md)[`AbstractMesh`](AbstractMesh.md)

#### Inherited from

PBRBaseMaterial.onBindObservable

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:443

___

### onDispose

• `set` **onDispose**(`callback`): `void`

Called during a dispose event

#### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | () => `void` |

#### Returns

`void`

#### Inherited from

PBRBaseMaterial.onDispose

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:431

___

### onEffectCreatedObservable

• `get` **onEffectCreatedObservable**(): [`Observable`](Observable.md){ `effect`: [`Effect`](Effect.md) ; `subMesh`: [`Nullable`](../modules.md#nullable)[`SubMesh`](SubMesh.md)  }

An event triggered when the effect is (re)created

#### Returns

[`Observable`](Observable.md){ `effect`: [`Effect`](Effect.md) ; `subMesh`: [`Nullable`](../modules.md#nullable)[`SubMesh`](SubMesh.md)  }

#### Inherited from

PBRBaseMaterial.onEffectCreatedObservable

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:482

___

### onUnBindObservable

• `get` **onUnBindObservable**(): [`Observable`](Observable.md)[`Material`](Material.md)

An event triggered when the material is unbound

#### Returns

[`Observable`](Observable.md)[`Material`](Material.md)

#### Inherited from

PBRBaseMaterial.onUnBindObservable

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:469

___

### pointsCloud

• `get` **pointsCloud**(): `boolean`

Gets the value specifying if point clouds are enabled

#### Returns

`boolean`

#### Inherited from

PBRBaseMaterial.pointsCloud

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:656

• `set` **pointsCloud**(`value`): `void`

Sets the state of point cloud mode

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

PBRBaseMaterial.pointsCloud

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:670

___

### realTimeFiltering

• `get` **realTimeFiltering**(): `boolean`

Enables realtime filtering on the texture.

#### Returns

`boolean`

#### Inherited from

PBRBaseMaterial.realTimeFiltering

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:719

• `set` **realTimeFiltering**(`b`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `b` | `boolean` |

#### Returns

`void`

#### Inherited from

PBRBaseMaterial.realTimeFiltering

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:722

___

### realTimeFilteringQuality

• `get` **realTimeFilteringQuality**(): `number`

Quality switch for realtime filtering

#### Returns

`number`

#### Inherited from

PBRBaseMaterial.realTimeFilteringQuality

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:731

• `set` **realTimeFilteringQuality**(`n`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `n` | `number` |

#### Returns

`void`

#### Inherited from

PBRBaseMaterial.realTimeFilteringQuality

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:734

___

### refractionTexture

• `get` **refractionTexture**(): [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Stores the refracted light information in a texture.

#### Returns

[`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:245

• `set` **refractionTexture**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:248

___

### transparencyMode

• `get` **transparencyMode**(): [`Nullable`](../modules.md#nullable)`number`

Gets the current transparency mode.

#### Returns

[`Nullable`](../modules.md#nullable)`number`

#### Inherited from

PBRBaseMaterial.transparencyMode

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:964

• `set` **transparencyMode**(`value`): `void`

Sets the transparency mode of the material.

| Value | Type                                | Description |
| ----- | ----------------------------------- | ----------- |
| 0     | OPAQUE                              |             |
| 1     | ALPHATEST                           |             |
| 2     | ALPHABLEND                          |             |
| 3     | ALPHATESTANDBLEND                   |             |

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)`number` |

#### Returns

`void`

#### Inherited from

PBRBaseMaterial.transparencyMode

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:980

___

### useGLTFLightFalloff

• `get` **useGLTFLightFalloff**(): `boolean`

In order to support the falloff compatibility with gltf, a special mode has been added
to reproduce the gltf light falloff.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:456

• `set` **useGLTFLightFalloff**(`value`): `void`

In order to support the falloff compatibility with gltf, a special mode has been added
to reproduce the gltf light falloff.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:465

___

### useLogarithmicDepth

• `get` **useLogarithmicDepth**(): `boolean`

Enabled the use of logarithmic depth buffers, which is good for wide depth buffers.

#### Returns

`boolean`

#### Inherited from

PBRBaseMaterial.useLogarithmicDepth

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:955

• `set` **useLogarithmicDepth**(`value`): `void`

Enabled the use of logarithmic depth buffers, which is good for wide depth buffers.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

PBRBaseMaterial.useLogarithmicDepth

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:963

___

### usePhysicalLightFalloff

• `get` **usePhysicalLightFalloff**(): `boolean`

BJS is using an hardcoded light falloff based on a manually sets up range.
In PBR, one way to represents the falloff is to use the inverse squared root algorithm.
This parameter can help you switch back to the BJS mode in order to create scenes using both materials.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:429

• `set` **usePhysicalLightFalloff**(`value`): `void`

BJS is using an hardcoded light falloff based on a manually sets up range.
In PBR, one way to represents the falloff is to use the inverse squared root algorithm.
This parameter can help you switch back to the BJS mode in order to create scenes using both materials.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:439

___

### wireframe

• `get` **wireframe**(): `boolean`

#### Returns

`boolean`

#### Inherited from

PBRBaseMaterial.wireframe

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:634

• `set` **wireframe**(`value`): `void`

Sets the state of wireframe mode

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

PBRBaseMaterial.wireframe

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:649

## Methods

### \_afterBind

▸ `Protected` **_afterBind**(`mesh?`, `effect?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `mesh?` | [`Mesh`](Mesh.md) | `undefined` |
| `effect` | [`Nullable`](../modules.md#nullable)[`Effect`](Effect.md) | `null` |

#### Returns

`void`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[_afterBind](PBRBaseMaterial.md#_afterbind)

#### Defined in

https://github.com/babylon.js/core/src/Materials/pushMaterial.ts:80

___

### \_attachImageProcessingConfiguration

▸ `Protected` **_attachImageProcessingConfiguration**(`configuration`): `void`

Attaches a new image processing configuration to the PBR Material.

#### Parameters

| Name | Type |
| :------ | :------ |
| `configuration` | [`Nullable`](../modules.md#nullable)[`ImageProcessingConfiguration`](ImageProcessingConfiguration.md) |

#### Returns

`void`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[_attachImageProcessingConfiguration](PBRBaseMaterial.md#_attachimageprocessingconfiguration)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:775

___

### \_hasAlphaChannel

▸ `Protected` **_hasAlphaChannel**(): `boolean`

Specifies whether or not there is a usable alpha channel for transparency.

#### Returns

`boolean`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[_hasAlphaChannel](PBRBaseMaterial.md#_hasalphachannel)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:1014

___

### \_isReadyForSubMesh

▸ `Protected` **_isReadyForSubMesh**(`subMesh`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `subMesh` | [`SubMesh`](SubMesh.md) |

#### Returns

`boolean`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[_isReadyForSubMesh](PBRBaseMaterial.md#_isreadyforsubmesh)

#### Defined in

https://github.com/babylon.js/core/src/Materials/pushMaterial.ts:43

___

### \_markAllSubMeshesAsAllDirty

▸ `Protected` **_markAllSubMeshesAsAllDirty**(): `void`

Indicates that we need to re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[_markAllSubMeshesAsAllDirty](PBRBaseMaterial.md#_markallsubmeshesasalldirty)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1543

___

### \_markAllSubMeshesAsAttributesDirty

▸ `Protected` **_markAllSubMeshesAsAttributesDirty**(): `void`

Indicates that attributes need to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[_markAllSubMeshesAsAttributesDirty](PBRBaseMaterial.md#_markallsubmeshesasattributesdirty)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1585

___

### \_markAllSubMeshesAsDirty

▸ `Protected` **_markAllSubMeshesAsDirty**(`func`): `void`

Marks all submeshes of a material to indicate that their material defines need to be re-calculated

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `func` | (`defines`: [`MaterialDefines`](MaterialDefines.md)) => `void` | defines a function which checks material defines against the submeshes |

#### Returns

`void`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[_markAllSubMeshesAsDirty](PBRBaseMaterial.md#_markallsubmeshesasdirty)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1498

___

### \_markAllSubMeshesAsFresnelAndMiscDirty

▸ `Protected` **_markAllSubMeshesAsFresnelAndMiscDirty**(): `void`

Indicates that fresnel and misc need to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[_markAllSubMeshesAsFresnelAndMiscDirty](PBRBaseMaterial.md#_markallsubmeshesasfresnelandmiscdirty)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1571

___

### \_markAllSubMeshesAsFresnelDirty

▸ `Protected` **_markAllSubMeshesAsFresnelDirty**(): `void`

Indicates that fresnel needs to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[_markAllSubMeshesAsFresnelDirty](PBRBaseMaterial.md#_markallsubmeshesasfresneldirty)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1564

___

### \_markAllSubMeshesAsImageProcessingDirty

▸ `Protected` **_markAllSubMeshesAsImageProcessingDirty**(): `void`

Indicates that image processing needs to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[_markAllSubMeshesAsImageProcessingDirty](PBRBaseMaterial.md#_markallsubmeshesasimageprocessingdirty)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1550

___

### \_markAllSubMeshesAsLightsDirty

▸ `Protected` **_markAllSubMeshesAsLightsDirty**(): `void`

Indicates that lights need to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[_markAllSubMeshesAsLightsDirty](PBRBaseMaterial.md#_markallsubmeshesaslightsdirty)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1578

___

### \_markAllSubMeshesAsMiscDirty

▸ `Protected` **_markAllSubMeshesAsMiscDirty**(): `void`

Indicates that misc needs to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[_markAllSubMeshesAsMiscDirty](PBRBaseMaterial.md#_markallsubmeshesasmiscdirty)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1592

___

### \_markAllSubMeshesAsPrePassDirty

▸ `Protected` **_markAllSubMeshesAsPrePassDirty**(): `void`

Indicates that prepass needs to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[_markAllSubMeshesAsPrePassDirty](PBRBaseMaterial.md#_markallsubmeshesasprepassdirty)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1599

___

### \_markAllSubMeshesAsTexturesAndMiscDirty

▸ `Protected` **_markAllSubMeshesAsTexturesAndMiscDirty**(): `void`

Indicates that textures and misc need to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[_markAllSubMeshesAsTexturesAndMiscDirty](PBRBaseMaterial.md#_markallsubmeshesastexturesandmiscdirty)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1606

___

### \_markAllSubMeshesAsTexturesDirty

▸ `Protected` **_markAllSubMeshesAsTexturesDirty**(): `void`

Indicates that textures need to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[_markAllSubMeshesAsTexturesDirty](PBRBaseMaterial.md#_markallsubmeshesastexturesdirty)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1557

___

### \_markScenePrePassDirty

▸ `Protected` **_markScenePrePassDirty**(): `void`

Indicates that the scene should check if the rendering now needs a prepass

#### Returns

`void`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[_markScenePrePassDirty](PBRBaseMaterial.md#_marksceneprepassdirty)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1529

___

### \_mustRebind

▸ `Protected` **_mustRebind**(`scene`, `effect`, `visibility?`): `boolean`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | `undefined` |
| `effect` | [`Effect`](Effect.md) | `undefined` |
| `visibility` | `number` | `1` |

#### Returns

`boolean`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[_mustRebind](PBRBaseMaterial.md#_mustrebind)

#### Defined in

https://github.com/babylon.js/core/src/Materials/pushMaterial.ts:85

___

### \_shouldTurnAlphaTestOn

▸ `Protected` **_shouldTurnAlphaTestOn**(`mesh`): `boolean`

Specifies if material alpha testing should be turned on for the mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | defines the mesh to check |

#### Returns

`boolean`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[_shouldTurnAlphaTestOn](PBRBaseMaterial.md#_shouldturnalphateston)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1040

___

### \_shouldUseAlphaFromAlbedoTexture

▸ `Protected` **_shouldUseAlphaFromAlbedoTexture**(): `boolean`

Specifies whether or not the alpha value of the albedo texture should be used for alpha blending.

#### Returns

`boolean`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[_shouldUseAlphaFromAlbedoTexture](PBRBaseMaterial.md#_shouldusealphafromalbedotexture)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:1007

___

### bind

▸ **bind**(`world`, `mesh?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `world` | [`Matrix`](Matrix.md) |
| `mesh?` | [`Mesh`](Mesh.md) |

#### Returns

`void`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[bind](PBRBaseMaterial.md#bind)

#### Defined in

https://github.com/babylon.js/core/src/Materials/pushMaterial.ts:72

___

### bindEyePosition

▸ **bindEyePosition**(`effect`, `variableName?`): `void`

Binds the view matrix to the effect

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `effect` | [`Effect`](Effect.md) | defines the effect to bind the view matrix to |
| `variableName?` | `string` | name of the shader variable that will hold the eye position |

#### Returns

`void`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[bindEyePosition](PBRBaseMaterial.md#bindeyeposition)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1168

___

### bindForSubMesh

▸ **bindForSubMesh**(`world`, `mesh`, `subMesh`): `void`

Binds the submesh data.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `world` | [`Matrix`](Matrix.md) | The world matrix. |
| `mesh` | [`Mesh`](Mesh.md) | The BJS mesh. |
| `subMesh` | [`SubMesh`](SubMesh.md) | A submesh of the BJS mesh. |

#### Returns

`void`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[bindForSubMesh](PBRBaseMaterial.md#bindforsubmesh)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:1956

___

### bindOnlyNormalMatrix

▸ **bindOnlyNormalMatrix**(`normalMatrix`): `void`

Binds the given normal matrix to the active effect

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `normalMatrix` | [`Matrix`](Matrix.md) | the matrix to bind |

#### Returns

`void`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[bindOnlyNormalMatrix](PBRBaseMaterial.md#bindonlynormalmatrix)

#### Defined in

https://github.com/babylon.js/core/src/Materials/pushMaterial.ts:68

___

### bindOnlyWorldMatrix

▸ **bindOnlyWorldMatrix**(`world`): `void`

Binds the given world matrix to the active effect

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `world` | [`Matrix`](Matrix.md) | the matrix to bind |

#### Returns

`void`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[bindOnlyWorldMatrix](PBRBaseMaterial.md#bindonlyworldmatrix)

#### Defined in

https://github.com/babylon.js/core/src/Materials/pushMaterial.ts:59

___

### bindView

▸ **bindView**(`effect`): `void`

Binds the view matrix to the effect

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `effect` | [`Effect`](Effect.md) | defines the effect to bind the view matrix to |

#### Returns

`void`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[bindView](PBRBaseMaterial.md#bindview)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1142

___

### bindViewProjection

▸ **bindViewProjection**(`effect`): `void`

Binds the view projection and projection matrices to the effect

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `effect` | [`Effect`](Effect.md) | defines the effect to bind the view projection and projection matrices to |

#### Returns

`void`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[bindViewProjection](PBRBaseMaterial.md#bindviewprojection)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1154

___

### buildUniformLayout

▸ **buildUniformLayout**(): `void`

Initializes the uniform buffer layout for the shader.

#### Returns

`void`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[buildUniformLayout](PBRBaseMaterial.md#builduniformlayout)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:1883

___

### clone

▸ **clone**(`name`): [`PBRMaterial`](PBRMaterial.md)

Makes a duplicate of the current material.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | name to use for the new material. |

#### Returns

[`PBRMaterial`](PBRMaterial.md)

#### Overrides

[PBRBaseMaterial](PBRBaseMaterial.md).[clone](PBRBaseMaterial.md#clone)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:766

___

### dispose

▸ **dispose**(`forceDisposeEffect?`, `forceDisposeTextures?`): `void`

Disposes the resources of the material.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `forceDisposeEffect?` | `boolean` | Forces the disposal of effects. |
| `forceDisposeTextures?` | `boolean` | Forces the disposal of all textures. |

#### Returns

`void`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[dispose](PBRBaseMaterial.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:2496

___

### forceCompilation

▸ **forceCompilation**(`mesh`, `onCompiled?`, `options?`): `void`

Force shader compilation

#### Parameters

| Name | Type |
| :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) |
| `onCompiled?` | (`material`: [`Material`](Material.md)) => `void` |
| `options?` | `Partial`[`IMaterialCompilationOptions`](../interfaces/IMaterialCompilationOptions.md) |

#### Returns

`void`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[forceCompilation](PBRBaseMaterial.md#forcecompilation)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:1848

___

### forceCompilationAsync

▸ **forceCompilationAsync**(`mesh`, `options?`): `Promise``void`

Force shader compilation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | defines the mesh that will use this material |
| `options?` | `Partial`[`IMaterialCompilationOptions`](../interfaces/IMaterialCompilationOptions.md) | defines additional options for compiling the shaders |

#### Returns

`Promise``void`

a promise that resolves when the compilation completes

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[forceCompilationAsync](PBRBaseMaterial.md#forcecompilationasync)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1392

___

### freeze

▸ **freeze**(): `void`

Locks updates for the material

#### Returns

`void`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[freeze](PBRBaseMaterial.md#freeze)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:890

___

### getActiveTextures

▸ **getActiveTextures**(): [`BaseTexture`](BaseTexture.md)[]

Returns an array of the actively used textures.

#### Returns

[`BaseTexture`](BaseTexture.md)[]

- Array of BaseTextures

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[getActiveTextures](PBRBaseMaterial.md#getactivetextures)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:2364

___

### getAlphaTestTexture

▸ **getAlphaTestTexture**(): [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Gets the texture used for the alpha test.

#### Returns

[`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[getAlphaTestTexture](PBRBaseMaterial.md#getalphatesttexture)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:1021

___

### getAnimatables

▸ **getAnimatables**(): [`IAnimatable`](../interfaces/IAnimatable.md)[]

Returns the animatable textures.

#### Returns

[`IAnimatable`](../interfaces/IAnimatable.md)[]

- Array of animatable textures.

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[getAnimatables](PBRBaseMaterial.md#getanimatables)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:2308

___

### getBindedMeshes

▸ **getBindedMeshes**(): [`AbstractMesh`](AbstractMesh.md)[]

Gets the meshes bound to the material

#### Returns

[`AbstractMesh`](AbstractMesh.md)[]

an array of meshes bound to the material

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[getBindedMeshes](PBRBaseMaterial.md#getbindedmeshes)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1289

___

### getClassName

▸ **getClassName**(): `string`

Returns the name of this material class.

#### Returns

`string`

#### Overrides

[PBRBaseMaterial](PBRBaseMaterial.md).[getClassName](PBRBaseMaterial.md#getclassname)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:758

___

### getEffect

▸ **getEffect**(): [`Effect`](Effect.md)

#### Returns

[`Effect`](Effect.md)

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[getEffect](PBRBaseMaterial.md#geteffect)

#### Defined in

https://github.com/babylon.js/core/src/Materials/pushMaterial.ts:23

___

### getScene

▸ **getScene**(): [`Scene`](Scene.md)

Returns the current scene

#### Returns

[`Scene`](Scene.md)

a Scene

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[getScene](PBRBaseMaterial.md#getscene)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:947

___

### hasTexture

▸ **hasTexture**(`texture`): `boolean`

Checks to see if a texture is used in the material.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `texture` | [`BaseTexture`](BaseTexture.md) | Base texture to use. |

#### Returns

`boolean`

- Boolean specifying if a texture is used in the material.

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[hasTexture](PBRBaseMaterial.md#hastexture)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:2423

___

### isMetallicWorkflow

▸ **isMetallicWorkflow**(): `boolean`

Specifies if the material uses metallic roughness workflow.

#### Returns

`boolean`

boolean specifying if the material uses metallic roughness workflow.

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[isMetallicWorkflow](PBRBaseMaterial.md#ismetallicworkflow)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:1208

___

### isReady

▸ **isReady**(`mesh?`, `useInstances?`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `mesh?` | [`AbstractMesh`](AbstractMesh.md) |
| `useInstances?` | `boolean` |

#### Returns

`boolean`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[isReady](PBRBaseMaterial.md#isready)

#### Defined in

https://github.com/babylon.js/core/src/Materials/pushMaterial.ts:27

___

### isReadyForSubMesh

▸ **isReadyForSubMesh**(`mesh`, `subMesh`, `useInstances?`): `boolean`

Specifies that the submesh is ready to be used.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | BJS mesh. |
| `subMesh` | [`SubMesh`](SubMesh.md) | A submesh of the BJS mesh.  Used to check if it is ready. |
| `useInstances?` | `boolean` | Specifies that instances should be used. |

#### Returns

`boolean`

- boolean indicating that the submesh is ready or not.

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[isReadyForSubMesh](PBRBaseMaterial.md#isreadyforsubmesh)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:1032

___

### markAsDirty

▸ **markAsDirty**(`flag`): `void`

Marks a define in the material to indicate that it needs to be re-computed

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `flag` | `number` | defines a flag used to determine which parts of the material have to be marked as dirty |

#### Returns

`void`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[markAsDirty](PBRBaseMaterial.md#markasdirty)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1437

___

### markDirty

▸ **markDirty**(): `void`

Marks the material to indicate that it needs to be re-calculated

#### Returns

`void`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[markDirty](PBRBaseMaterial.md#markdirty)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1055

___

### needAlphaBlending

▸ **needAlphaBlending**(): `boolean`

Specifies whether or not this material should be rendered in alpha blend mode.

#### Returns

`boolean`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[needAlphaBlending](PBRBaseMaterial.md#needalphablending)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:981

___

### needAlphaBlendingForMesh

▸ **needAlphaBlendingForMesh**(`mesh`): `boolean`

Specifies if the mesh will require alpha blending

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | defines the mesh to check |

#### Returns

`boolean`

a boolean specifying if alpha blending is needed for the mesh

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[needAlphaBlendingForMesh](PBRBaseMaterial.md#needalphablendingformesh)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1016

___

### needAlphaTesting

▸ **needAlphaTesting**(): `boolean`

Specifies whether or not this material should be rendered in alpha test mode.

#### Returns

`boolean`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[needAlphaTesting](PBRBaseMaterial.md#needalphatesting)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:992

___

### resetDrawCache

▸ **resetDrawCache**(): `void`

Resets the draw wrappers cache for all submeshes that are using this material

#### Returns

`void`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[resetDrawCache](PBRBaseMaterial.md#resetdrawcache)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1478

___

### serialize

▸ **serialize**(): `any`

Serializes this PBR Material.

#### Returns

`any`

- An object with the serialized material.

#### Overrides

[PBRBaseMaterial](PBRBaseMaterial.md).[serialize](PBRBaseMaterial.md#serialize)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:786

___

### setPrePassRenderer

▸ **setPrePassRenderer**(): `boolean`

Sets the required values to the prepass renderer.

#### Returns

`boolean`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[setPrePassRenderer](PBRBaseMaterial.md#setprepassrenderer)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:2478

___

### toString

▸ **toString**(`fullDetails?`): `string`

Returns a string representation of the current material

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fullDetails?` | `boolean` | defines a boolean indicating which levels of logging is desired |

#### Returns

`string`

a string with material information

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[toString](PBRBaseMaterial.md#tostring)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:867

___

### unbind

▸ **unbind**(): `void`

Unbinds the material from the mesh

#### Returns

`void`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[unbind](PBRBaseMaterial.md#unbind)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1222

___

### unfreeze

▸ **unfreeze**(): `void`

Unlocks updates for the material

#### Returns

`void`

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[unfreeze](PBRBaseMaterial.md#unfreeze)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:898

___

### Parse

▸ `Static` **Parse**(`source`, `scene`, `rootUrl`): [`PBRMaterial`](PBRMaterial.md)

Parses a PBR Material from a serialized object.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | `any` | Serialized object. |
| `scene` | [`Scene`](Scene.md) | BJS scene instance. |
| `rootUrl` | `string` | url for the scene object |

#### Returns

[`PBRMaterial`](PBRMaterial.md)

- PBRMaterial

#### Overrides

[PBRBaseMaterial](PBRBaseMaterial.md).[Parse](PBRBaseMaterial.md#parse)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrMaterial.ts:808
