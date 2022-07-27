[@dev/core](../README.md) / [Exports](../modules.md) / PBRSpecularGlossinessMaterial

# Class: PBRSpecularGlossinessMaterial

The PBR material of BJS following the specular glossiness convention.

This fits to the PBR convention in the GLTF definition:
https://github.com/KhronosGroup/glTF/tree/2.0/extensions/Khronos/KHR_materials_pbrSpecularGlossiness

## Hierarchy

- [`PBRBaseSimpleMaterial`](PBRBaseSimpleMaterial.md)

  ↳ **`PBRSpecularGlossinessMaterial`**

## Table of contents

### Constructors

- [constructor](PBRSpecularGlossinessMaterial.md#constructor)

### Properties

- [\_activeEffect](PBRSpecularGlossinessMaterial.md#_activeeffect)
- [\_alpha](PBRSpecularGlossinessMaterial.md#_alpha)
- [\_backFaceCulling](PBRSpecularGlossinessMaterial.md#_backfaceculling)
- [\_cacheHasRenderTargetTextures](PBRSpecularGlossinessMaterial.md#_cachehasrendertargettextures)
- [\_cullBackFaces](PBRSpecularGlossinessMaterial.md#_cullbackfaces)
- [\_drawWrapper](PBRSpecularGlossinessMaterial.md#_drawwrapper)
- [\_eventInfo](PBRSpecularGlossinessMaterial.md#_eventinfo)
- [\_imageProcessingConfiguration](PBRSpecularGlossinessMaterial.md#_imageprocessingconfiguration)
- [\_needToBindSceneUbo](PBRSpecularGlossinessMaterial.md#_needtobindsceneubo)
- [\_normalMatrix](PBRSpecularGlossinessMaterial.md#_normalmatrix)
- [\_onEffectCreatedObservable](PBRSpecularGlossinessMaterial.md#_oneffectcreatedobservable)
- [\_transparencyMode](PBRSpecularGlossinessMaterial.md#_transparencymode)
- [allowShaderHotSwapping](PBRSpecularGlossinessMaterial.md#allowshaderhotswapping)
- [alphaCutOff](PBRSpecularGlossinessMaterial.md#alphacutoff)
- [animations](PBRSpecularGlossinessMaterial.md#animations)
- [anisotropy](PBRSpecularGlossinessMaterial.md#anisotropy)
- [brdf](PBRSpecularGlossinessMaterial.md#brdf)
- [checkReadyOnEveryCall](PBRSpecularGlossinessMaterial.md#checkreadyoneverycall)
- [checkReadyOnlyOnce](PBRSpecularGlossinessMaterial.md#checkreadyonlyonce)
- [clearCoat](PBRSpecularGlossinessMaterial.md#clearcoat)
- [customShaderNameResolve](PBRSpecularGlossinessMaterial.md#customshadernameresolve)
- [depthFunction](PBRSpecularGlossinessMaterial.md#depthfunction)
- [detailMap](PBRSpecularGlossinessMaterial.md#detailmap)
- [diffuseColor](PBRSpecularGlossinessMaterial.md#diffusecolor)
- [diffuseTexture](PBRSpecularGlossinessMaterial.md#diffusetexture)
- [disableColorWrite](PBRSpecularGlossinessMaterial.md#disablecolorwrite)
- [disableDepthWrite](PBRSpecularGlossinessMaterial.md#disabledepthwrite)
- [disableLighting](PBRSpecularGlossinessMaterial.md#disablelighting)
- [doNotSerialize](PBRSpecularGlossinessMaterial.md#donotserialize)
- [emissiveColor](PBRSpecularGlossinessMaterial.md#emissivecolor)
- [emissiveTexture](PBRSpecularGlossinessMaterial.md#emissivetexture)
- [environmentTexture](PBRSpecularGlossinessMaterial.md#environmenttexture)
- [forceDepthWrite](PBRSpecularGlossinessMaterial.md#forcedepthwrite)
- [getRenderTargetTextures](PBRSpecularGlossinessMaterial.md#getrendertargettextures)
- [glossiness](PBRSpecularGlossinessMaterial.md#glossiness)
- [id](PBRSpecularGlossinessMaterial.md#id)
- [inspectableCustomProperties](PBRSpecularGlossinessMaterial.md#inspectablecustomproperties)
- [invertNormalMapX](PBRSpecularGlossinessMaterial.md#invertnormalmapx)
- [invertNormalMapY](PBRSpecularGlossinessMaterial.md#invertnormalmapy)
- [iridescence](PBRSpecularGlossinessMaterial.md#iridescence)
- [lightmapTexture](PBRSpecularGlossinessMaterial.md#lightmaptexture)
- [maxSimultaneousLights](PBRSpecularGlossinessMaterial.md#maxsimultaneouslights)
- [metadata](PBRSpecularGlossinessMaterial.md#metadata)
- [name](PBRSpecularGlossinessMaterial.md#name)
- [normalTexture](PBRSpecularGlossinessMaterial.md#normaltexture)
- [occlusionStrength](PBRSpecularGlossinessMaterial.md#occlusionstrength)
- [occlusionTexture](PBRSpecularGlossinessMaterial.md#occlusiontexture)
- [onCompiled](PBRSpecularGlossinessMaterial.md#oncompiled)
- [onDisposeObservable](PBRSpecularGlossinessMaterial.md#ondisposeobservable)
- [onError](PBRSpecularGlossinessMaterial.md#onerror)
- [pluginManager](PBRSpecularGlossinessMaterial.md#pluginmanager)
- [pointSize](PBRSpecularGlossinessMaterial.md#pointsize)
- [prePassConfiguration](PBRSpecularGlossinessMaterial.md#prepassconfiguration)
- [reservedDataStore](PBRSpecularGlossinessMaterial.md#reserveddatastore)
- [separateCullingPass](PBRSpecularGlossinessMaterial.md#separatecullingpass)
- [shadowDepthWrapper](PBRSpecularGlossinessMaterial.md#shadowdepthwrapper)
- [sheen](PBRSpecularGlossinessMaterial.md#sheen)
- [sideOrientation](PBRSpecularGlossinessMaterial.md#sideorientation)
- [specularColor](PBRSpecularGlossinessMaterial.md#specularcolor)
- [specularGlossinessTexture](PBRSpecularGlossinessMaterial.md#specularglossinesstexture)
- [state](PBRSpecularGlossinessMaterial.md#state)
- [stencil](PBRSpecularGlossinessMaterial.md#stencil)
- [subSurface](PBRSpecularGlossinessMaterial.md#subsurface)
- [uniqueId](PBRSpecularGlossinessMaterial.md#uniqueid)
- [useLightmapAsShadowmap](PBRSpecularGlossinessMaterial.md#uselightmapasshadowmap)
- [zOffset](PBRSpecularGlossinessMaterial.md#zoffset)
- [zOffsetUnits](PBRSpecularGlossinessMaterial.md#zoffsetunits)
- [AllDirtyFlag](PBRSpecularGlossinessMaterial.md#alldirtyflag)
- [AttributesDirtyFlag](PBRSpecularGlossinessMaterial.md#attributesdirtyflag)
- [ClockWiseSideOrientation](PBRSpecularGlossinessMaterial.md#clockwisesideorientation)
- [CounterClockWiseSideOrientation](PBRSpecularGlossinessMaterial.md#counterclockwisesideorientation)
- [DEFAULT\_AO\_ON\_ANALYTICAL\_LIGHTS](PBRSpecularGlossinessMaterial.md#default_ao_on_analytical_lights)
- [FresnelDirtyFlag](PBRSpecularGlossinessMaterial.md#fresneldirtyflag)
- [LIGHTFALLOFF\_GLTF](PBRSpecularGlossinessMaterial.md#lightfalloff_gltf)
- [LIGHTFALLOFF\_PHYSICAL](PBRSpecularGlossinessMaterial.md#lightfalloff_physical)
- [LIGHTFALLOFF\_STANDARD](PBRSpecularGlossinessMaterial.md#lightfalloff_standard)
- [LightDirtyFlag](PBRSpecularGlossinessMaterial.md#lightdirtyflag)
- [LineListDrawMode](PBRSpecularGlossinessMaterial.md#linelistdrawmode)
- [LineLoopDrawMode](PBRSpecularGlossinessMaterial.md#lineloopdrawmode)
- [LineStripDrawMode](PBRSpecularGlossinessMaterial.md#linestripdrawmode)
- [MATERIAL\_ALPHABLEND](PBRSpecularGlossinessMaterial.md#material_alphablend)
- [MATERIAL\_ALPHATEST](PBRSpecularGlossinessMaterial.md#material_alphatest)
- [MATERIAL\_ALPHATESTANDBLEND](PBRSpecularGlossinessMaterial.md#material_alphatestandblend)
- [MATERIAL\_NORMALBLENDMETHOD\_RNM](PBRSpecularGlossinessMaterial.md#material_normalblendmethod_rnm)
- [MATERIAL\_NORMALBLENDMETHOD\_WHITEOUT](PBRSpecularGlossinessMaterial.md#material_normalblendmethod_whiteout)
- [MATERIAL\_OPAQUE](PBRSpecularGlossinessMaterial.md#material_opaque)
- [MiscDirtyFlag](PBRSpecularGlossinessMaterial.md#miscdirtyflag)
- [OnEventObservable](PBRSpecularGlossinessMaterial.md#oneventobservable)
- [PBRMATERIAL\_ALPHABLEND](PBRSpecularGlossinessMaterial.md#pbrmaterial_alphablend)
- [PBRMATERIAL\_ALPHATEST](PBRSpecularGlossinessMaterial.md#pbrmaterial_alphatest)
- [PBRMATERIAL\_ALPHATESTANDBLEND](PBRSpecularGlossinessMaterial.md#pbrmaterial_alphatestandblend)
- [PBRMATERIAL\_OPAQUE](PBRSpecularGlossinessMaterial.md#pbrmaterial_opaque)
- [PointFillMode](PBRSpecularGlossinessMaterial.md#pointfillmode)
- [PointListDrawMode](PBRSpecularGlossinessMaterial.md#pointlistdrawmode)
- [PrePassDirtyFlag](PBRSpecularGlossinessMaterial.md#prepassdirtyflag)
- [TextureDirtyFlag](PBRSpecularGlossinessMaterial.md#texturedirtyflag)
- [TriangleFanDrawMode](PBRSpecularGlossinessMaterial.md#trianglefandrawmode)
- [TriangleFillMode](PBRSpecularGlossinessMaterial.md#trianglefillmode)
- [TriangleStripDrawMode](PBRSpecularGlossinessMaterial.md#trianglestripdrawmode)
- [WireFrameFillMode](PBRSpecularGlossinessMaterial.md#wireframefillmode)

### Accessors

- [\_disableAlphaBlending](PBRSpecularGlossinessMaterial.md#_disablealphablending)
- [alpha](PBRSpecularGlossinessMaterial.md#alpha)
- [alphaMode](PBRSpecularGlossinessMaterial.md#alphamode)
- [backFaceCulling](PBRSpecularGlossinessMaterial.md#backfaceculling)
- [canRenderToMRT](PBRSpecularGlossinessMaterial.md#canrendertomrt)
- [cullBackFaces](PBRSpecularGlossinessMaterial.md#cullbackfaces)
- [doubleSided](PBRSpecularGlossinessMaterial.md#doublesided)
- [fillMode](PBRSpecularGlossinessMaterial.md#fillmode)
- [fogEnabled](PBRSpecularGlossinessMaterial.md#fogenabled)
- [hasRenderTargetTextures](PBRSpecularGlossinessMaterial.md#hasrendertargettextures)
- [isFrozen](PBRSpecularGlossinessMaterial.md#isfrozen)
- [isPrePassCapable](PBRSpecularGlossinessMaterial.md#isprepasscapable)
- [needDepthPrePass](PBRSpecularGlossinessMaterial.md#needdepthprepass)
- [onBind](PBRSpecularGlossinessMaterial.md#onbind)
- [onBindObservable](PBRSpecularGlossinessMaterial.md#onbindobservable)
- [onDispose](PBRSpecularGlossinessMaterial.md#ondispose)
- [onEffectCreatedObservable](PBRSpecularGlossinessMaterial.md#oneffectcreatedobservable)
- [onUnBindObservable](PBRSpecularGlossinessMaterial.md#onunbindobservable)
- [pointsCloud](PBRSpecularGlossinessMaterial.md#pointscloud)
- [realTimeFiltering](PBRSpecularGlossinessMaterial.md#realtimefiltering)
- [realTimeFilteringQuality](PBRSpecularGlossinessMaterial.md#realtimefilteringquality)
- [transparencyMode](PBRSpecularGlossinessMaterial.md#transparencymode)
- [useLogarithmicDepth](PBRSpecularGlossinessMaterial.md#uselogarithmicdepth)
- [useMicroSurfaceFromReflectivityMapAlpha](PBRSpecularGlossinessMaterial.md#usemicrosurfacefromreflectivitymapalpha)
- [wireframe](PBRSpecularGlossinessMaterial.md#wireframe)

### Methods

- [\_afterBind](PBRSpecularGlossinessMaterial.md#_afterbind)
- [\_attachImageProcessingConfiguration](PBRSpecularGlossinessMaterial.md#_attachimageprocessingconfiguration)
- [\_hasAlphaChannel](PBRSpecularGlossinessMaterial.md#_hasalphachannel)
- [\_isReadyForSubMesh](PBRSpecularGlossinessMaterial.md#_isreadyforsubmesh)
- [\_markAllSubMeshesAsAllDirty](PBRSpecularGlossinessMaterial.md#_markallsubmeshesasalldirty)
- [\_markAllSubMeshesAsAttributesDirty](PBRSpecularGlossinessMaterial.md#_markallsubmeshesasattributesdirty)
- [\_markAllSubMeshesAsDirty](PBRSpecularGlossinessMaterial.md#_markallsubmeshesasdirty)
- [\_markAllSubMeshesAsFresnelAndMiscDirty](PBRSpecularGlossinessMaterial.md#_markallsubmeshesasfresnelandmiscdirty)
- [\_markAllSubMeshesAsFresnelDirty](PBRSpecularGlossinessMaterial.md#_markallsubmeshesasfresneldirty)
- [\_markAllSubMeshesAsImageProcessingDirty](PBRSpecularGlossinessMaterial.md#_markallsubmeshesasimageprocessingdirty)
- [\_markAllSubMeshesAsLightsDirty](PBRSpecularGlossinessMaterial.md#_markallsubmeshesaslightsdirty)
- [\_markAllSubMeshesAsMiscDirty](PBRSpecularGlossinessMaterial.md#_markallsubmeshesasmiscdirty)
- [\_markAllSubMeshesAsPrePassDirty](PBRSpecularGlossinessMaterial.md#_markallsubmeshesasprepassdirty)
- [\_markAllSubMeshesAsTexturesAndMiscDirty](PBRSpecularGlossinessMaterial.md#_markallsubmeshesastexturesandmiscdirty)
- [\_markAllSubMeshesAsTexturesDirty](PBRSpecularGlossinessMaterial.md#_markallsubmeshesastexturesdirty)
- [\_markScenePrePassDirty](PBRSpecularGlossinessMaterial.md#_marksceneprepassdirty)
- [\_mustRebind](PBRSpecularGlossinessMaterial.md#_mustrebind)
- [\_shouldTurnAlphaTestOn](PBRSpecularGlossinessMaterial.md#_shouldturnalphateston)
- [\_shouldUseAlphaFromAlbedoTexture](PBRSpecularGlossinessMaterial.md#_shouldusealphafromalbedotexture)
- [bind](PBRSpecularGlossinessMaterial.md#bind)
- [bindEyePosition](PBRSpecularGlossinessMaterial.md#bindeyeposition)
- [bindForSubMesh](PBRSpecularGlossinessMaterial.md#bindforsubmesh)
- [bindOnlyNormalMatrix](PBRSpecularGlossinessMaterial.md#bindonlynormalmatrix)
- [bindOnlyWorldMatrix](PBRSpecularGlossinessMaterial.md#bindonlyworldmatrix)
- [bindView](PBRSpecularGlossinessMaterial.md#bindview)
- [bindViewProjection](PBRSpecularGlossinessMaterial.md#bindviewprojection)
- [buildUniformLayout](PBRSpecularGlossinessMaterial.md#builduniformlayout)
- [clone](PBRSpecularGlossinessMaterial.md#clone)
- [dispose](PBRSpecularGlossinessMaterial.md#dispose)
- [forceCompilation](PBRSpecularGlossinessMaterial.md#forcecompilation)
- [forceCompilationAsync](PBRSpecularGlossinessMaterial.md#forcecompilationasync)
- [freeze](PBRSpecularGlossinessMaterial.md#freeze)
- [getActiveTextures](PBRSpecularGlossinessMaterial.md#getactivetextures)
- [getAlphaTestTexture](PBRSpecularGlossinessMaterial.md#getalphatesttexture)
- [getAnimatables](PBRSpecularGlossinessMaterial.md#getanimatables)
- [getBindedMeshes](PBRSpecularGlossinessMaterial.md#getbindedmeshes)
- [getClassName](PBRSpecularGlossinessMaterial.md#getclassname)
- [getEffect](PBRSpecularGlossinessMaterial.md#geteffect)
- [getScene](PBRSpecularGlossinessMaterial.md#getscene)
- [hasTexture](PBRSpecularGlossinessMaterial.md#hastexture)
- [isMetallicWorkflow](PBRSpecularGlossinessMaterial.md#ismetallicworkflow)
- [isReady](PBRSpecularGlossinessMaterial.md#isready)
- [isReadyForSubMesh](PBRSpecularGlossinessMaterial.md#isreadyforsubmesh)
- [markAsDirty](PBRSpecularGlossinessMaterial.md#markasdirty)
- [markDirty](PBRSpecularGlossinessMaterial.md#markdirty)
- [needAlphaBlending](PBRSpecularGlossinessMaterial.md#needalphablending)
- [needAlphaBlendingForMesh](PBRSpecularGlossinessMaterial.md#needalphablendingformesh)
- [needAlphaTesting](PBRSpecularGlossinessMaterial.md#needalphatesting)
- [resetDrawCache](PBRSpecularGlossinessMaterial.md#resetdrawcache)
- [serialize](PBRSpecularGlossinessMaterial.md#serialize)
- [setPrePassRenderer](PBRSpecularGlossinessMaterial.md#setprepassrenderer)
- [toString](PBRSpecularGlossinessMaterial.md#tostring)
- [unbind](PBRSpecularGlossinessMaterial.md#unbind)
- [unfreeze](PBRSpecularGlossinessMaterial.md#unfreeze)
- [Parse](PBRSpecularGlossinessMaterial.md#parse)

## Constructors

### constructor

• **new PBRSpecularGlossinessMaterial**(`name`, `scene?`)

Instantiates a new PBRSpecularGlossinessMaterial instance.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | The material name |
| `scene?` | [`Scene`](Scene.md) | The scene the material will be use in. |

#### Overrides

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[constructor](PBRBaseSimpleMaterial.md#constructor)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrSpecularGlossinessMaterial.ts:65

## Properties

### \_activeEffect

• `Protected` **\_activeEffect**: [`Effect`](Effect.md)

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[_activeEffect](PBRBaseSimpleMaterial.md#_activeeffect)

#### Defined in

packages/dev/core/src/Materials/pushMaterial.ts:14

___

### \_alpha

• `Protected` **\_alpha**: `number` = `1.0`

The alpha value of the material

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[_alpha](PBRBaseSimpleMaterial.md#_alpha)

#### Defined in

packages/dev/core/src/Materials/material.ts:292

___

### \_backFaceCulling

• `Protected` **\_backFaceCulling**: `boolean` = `true`

Specifies if back face culling is enabled

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[_backFaceCulling](PBRBaseSimpleMaterial.md#_backfaceculling)

#### Defined in

packages/dev/core/src/Materials/material.ts:328

___

### \_cacheHasRenderTargetTextures

• `Protected` **\_cacheHasRenderTargetTextures**: `boolean` = `false`

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[_cacheHasRenderTargetTextures](PBRBaseSimpleMaterial.md#_cachehasrendertargettextures)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:888

___

### \_cullBackFaces

• `Protected` **\_cullBackFaces**: `boolean` = `true`

Specifies if back or front faces should be culled (when culling is enabled)

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[_cullBackFaces](PBRBaseSimpleMaterial.md#_cullbackfaces)

#### Defined in

packages/dev/core/src/Materials/material.ts:352

___

### \_drawWrapper

• `Protected` **\_drawWrapper**: `DrawWrapper`

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[_drawWrapper](PBRBaseSimpleMaterial.md#_drawwrapper)

#### Defined in

packages/dev/core/src/Materials/material.ts:705

___

### \_eventInfo

• `Protected` **\_eventInfo**: `MaterialPluginDisposed` & `MaterialPluginHasTexture` & `MaterialPluginIsReadyForSubMesh` & `MaterialPluginGetDefineNames` & `MaterialPluginPrepareEffect` & `MaterialPluginPrepareDefines` & `MaterialPluginPrepareUniformBuffer` & `MaterialPluginBindForSubMesh` & `MaterialPluginGetAnimatables` & `MaterialPluginGetActiveTextures` & `MaterialPluginFillRenderTargetTextures` & `MaterialPluginHasRenderTargetTextures` & `MaterialPluginHardBindForSubMesh`

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[_eventInfo](PBRBaseSimpleMaterial.md#_eventinfo)

#### Defined in

packages/dev/core/src/Materials/material.ts:770

___

### \_imageProcessingConfiguration

• `Protected` **\_imageProcessingConfiguration**: [`ImageProcessingConfiguration`](ImageProcessingConfiguration.md)

Default configuration related to image processing available in the PBR Material.

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[_imageProcessingConfiguration](PBRBaseSimpleMaterial.md#_imageprocessingconfiguration)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:764

___

### \_needToBindSceneUbo

• `Protected` **\_needToBindSceneUbo**: `boolean`

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[_needToBindSceneUbo](PBRBaseSimpleMaterial.md#_needtobindsceneubo)

#### Defined in

packages/dev/core/src/Materials/material.ts:727

___

### \_normalMatrix

• `Protected` **\_normalMatrix**: [`Matrix`](Matrix.md)

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[_normalMatrix](PBRBaseSimpleMaterial.md#_normalmatrix)

#### Defined in

packages/dev/core/src/Materials/pushMaterial.ts:16

___

### \_onEffectCreatedObservable

• `Protected` **\_onEffectCreatedObservable**: [`Nullable`](../modules.md#nullable)[`Observable`](Observable.md){ `effect`: [`Effect`](Effect.md) ; `subMesh`: [`Nullable`](../modules.md#nullable)[`SubMesh`](SubMesh.md)  }

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[_onEffectCreatedObservable](PBRBaseSimpleMaterial.md#_oneffectcreatedobservable)

#### Defined in

packages/dev/core/src/Materials/material.ts:477

___

### \_transparencyMode

• `Protected` **\_transparencyMode**: [`Nullable`](../modules.md#nullable)`number` = `null`

The transparency mode of the material.

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[_transparencyMode](PBRBaseSimpleMaterial.md#_transparencymode)

#### Defined in

packages/dev/core/src/Materials/material.ts:959

___

### allowShaderHotSwapping

• **allowShaderHotSwapping**: `boolean` = `true`

Gets or sets a boolean indicating that the material is allowed (if supported) to do shader hot swapping.
This means that the material can keep using a previous shader while a new one is being compiled.
This is mostly used when shader parallel compilation is supported (true by default)

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[allowShaderHotSwapping](PBRBaseSimpleMaterial.md#allowshaderhotswapping)

#### Defined in

packages/dev/core/src/Materials/material.ts:227

___

### alphaCutOff

• **alphaCutOff**: `number`

Defines the alpha limits in alpha test mode.

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[alphaCutOff](PBRBaseSimpleMaterial.md#alphacutoff)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseSimpleMaterial.ts:90

___

### animations

• **animations**: [`Nullable`](../modules.md#nullable)[`Animation`](Animation.md)[] = `null`

Stores the animations for the material

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[animations](PBRBaseSimpleMaterial.md#animations)

#### Defined in

packages/dev/core/src/Materials/material.ts:415

___

### anisotropy

• `Readonly` **anisotropy**: [`PBRAnisotropicConfiguration`](PBRAnisotropicConfiguration.md)

Defines the anisotropic parameters for the material.

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[anisotropy](PBRBaseSimpleMaterial.md#anisotropy)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:861

___

### brdf

• `Readonly` **brdf**: `PBRBRDFConfiguration`

Defines the BRDF parameters for the material.

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[brdf](PBRBaseSimpleMaterial.md#brdf)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:866

___

### checkReadyOnEveryCall

• **checkReadyOnEveryCall**: `boolean` = `false`

Specifies if the ready state should be checked on each call

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[checkReadyOnEveryCall](PBRBaseSimpleMaterial.md#checkreadyoneverycall)

#### Defined in

packages/dev/core/src/Materials/material.ts:265

___

### checkReadyOnlyOnce

• **checkReadyOnlyOnce**: `boolean` = `false`

Specifies if the ready state should be checked once

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[checkReadyOnlyOnce](PBRBaseSimpleMaterial.md#checkreadyonlyonce)

#### Defined in

packages/dev/core/src/Materials/material.ts:271

___

### clearCoat

• `Readonly` **clearCoat**: [`PBRClearCoatConfiguration`](PBRClearCoatConfiguration.md)

Defines the clear coat layer parameters for the material.

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[clearCoat](PBRBaseSimpleMaterial.md#clearcoat)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:851

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

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[customShaderNameResolve](PBRBaseSimpleMaterial.md#customshadernameresolve)

#### Defined in

packages/dev/core/src/Materials/material.ts:207

___

### depthFunction

• **depthFunction**: `number` = `0`

Specifies the depth function that should be used. 0 means the default engine function

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[depthFunction](PBRBaseSimpleMaterial.md#depthfunction)

#### Defined in

packages/dev/core/src/Materials/material.ts:584

___

### detailMap

• `Readonly` **detailMap**: [`DetailMapConfiguration`](DetailMapConfiguration.md)

Defines the detail map parameters for the material.

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[detailMap](PBRBaseSimpleMaterial.md#detailmap)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:886

___

### diffuseColor

• **diffuseColor**: [`Color3`](Color3.md)

Specifies the diffuse color of the material.

#### Defined in

packages/dev/core/src/Materials/PBR/pbrSpecularGlossinessMaterial.ts:21

___

### diffuseTexture

• **diffuseTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Specifies the diffuse texture of the material. This can also contains the opacity value in its alpha
channel.

#### Defined in

packages/dev/core/src/Materials/PBR/pbrSpecularGlossinessMaterial.ts:29

___

### disableColorWrite

• **disableColorWrite**: `boolean` = `false`

Specifies if color writing should be disabled

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[disableColorWrite](PBRBaseSimpleMaterial.md#disablecolorwrite)

#### Defined in

packages/dev/core/src/Materials/material.ts:572

___

### disableDepthWrite

• **disableDepthWrite**: `boolean` = `false`

Specifies if depth writing should be disabled

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[disableDepthWrite](PBRBaseSimpleMaterial.md#disabledepthwrite)

#### Defined in

packages/dev/core/src/Materials/material.ts:566

___

### disableLighting

• **disableLighting**: `boolean` = `false`

If sets to true, disables all the lights affecting the material.

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[disableLighting](PBRBaseSimpleMaterial.md#disablelighting)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseSimpleMaterial.ts:27

___

### doNotSerialize

• **doNotSerialize**: `boolean` = `false`

Specifies if the material should be serialized

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[doNotSerialize](PBRBaseSimpleMaterial.md#donotserialize)

#### Defined in

packages/dev/core/src/Materials/material.ts:405

___

### emissiveColor

• **emissiveColor**: [`Color3`](Color3.md)

Emissivie color used to self-illuminate the model.

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[emissiveColor](PBRBaseSimpleMaterial.md#emissivecolor)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseSimpleMaterial.ts:62

___

### emissiveTexture

• **emissiveTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Emissivie texture used to self-illuminate the model.

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[emissiveTexture](PBRBaseSimpleMaterial.md#emissivetexture)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseSimpleMaterial.ts:69

___

### environmentTexture

• **environmentTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Environment Texture used in the material (this is use for both reflection and environment lighting).

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[environmentTexture](PBRBaseSimpleMaterial.md#environmenttexture)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseSimpleMaterial.ts:34

___

### forceDepthWrite

• **forceDepthWrite**: `boolean` = `false`

Specifies if depth writing should be forced

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[forceDepthWrite](PBRBaseSimpleMaterial.md#forcedepthwrite)

#### Defined in

packages/dev/core/src/Materials/material.ts:578

___

### getRenderTargetTextures

• **getRenderTargetTextures**: [`Nullable`](../modules.md#nullable)() => [`SmartArray`](SmartArray.md)[`RenderTargetTexture`](RenderTargetTexture.md) = `null`

Callback triggered to get the render target textures

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[getRenderTargetTextures](PBRBaseSimpleMaterial.md#getrendertargettextures)

#### Defined in

packages/dev/core/src/Materials/material.ts:391

___

### glossiness

• **glossiness**: `number`

Specifies the glossiness of the material. This indicates "how sharp is the reflection".

#### Defined in

packages/dev/core/src/Materials/PBR/pbrSpecularGlossinessMaterial.ts:43

___

### id

• **id**: `string`

The ID of the material

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[id](PBRBaseSimpleMaterial.md#id)

#### Defined in

packages/dev/core/src/Materials/material.ts:233

___

### inspectableCustomProperties

• **inspectableCustomProperties**: [`IInspectable`](../interfaces/IInspectable.md)[]

List of inspectable custom properties (used by the Inspector)

**`See`**

https://doc.babylonjs.com/how_to/debug_layer#extensibility

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[inspectableCustomProperties](PBRBaseSimpleMaterial.md#inspectablecustomproperties)

#### Defined in

packages/dev/core/src/Materials/material.ts:298

___

### invertNormalMapX

• **invertNormalMapX**: `boolean` = `false`

If sets to true, x component of normal map value will invert (x = 1.0 - x).

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[invertNormalMapX](PBRBaseSimpleMaterial.md#invertnormalmapx)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseSimpleMaterial.ts:41

___

### invertNormalMapY

• **invertNormalMapY**: `boolean` = `false`

If sets to true, y component of normal map value will invert (y = 1.0 - y).

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[invertNormalMapY](PBRBaseSimpleMaterial.md#invertnormalmapy)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseSimpleMaterial.ts:48

___

### iridescence

• `Readonly` **iridescence**: [`PBRIridescenceConfiguration`](PBRIridescenceConfiguration.md)

Defines the iridescence layer parameters for the material.

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[iridescence](PBRBaseSimpleMaterial.md#iridescence)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:856

___

### lightmapTexture

• **lightmapTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Stores the pre-calculated light information of a mesh in a texture.

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[lightmapTexture](PBRBaseSimpleMaterial.md#lightmaptexture)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseSimpleMaterial.ts:116

___

### maxSimultaneousLights

• **maxSimultaneousLights**: `number` = `4`

Number of Simultaneous lights allowed on the material.

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[maxSimultaneousLights](PBRBaseSimpleMaterial.md#maxsimultaneouslights)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseSimpleMaterial.ts:20

___

### metadata

• **metadata**: `any` = `null`

Gets or sets user defined metadata

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[metadata](PBRBaseSimpleMaterial.md#metadata)

#### Defined in

packages/dev/core/src/Materials/material.ts:254

___

### name

• **name**: `string`

The name of the material

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[name](PBRBaseSimpleMaterial.md#name)

#### Defined in

packages/dev/core/src/Materials/material.ts:248

___

### normalTexture

• **normalTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Normal map used in the model.

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[normalTexture](PBRBaseSimpleMaterial.md#normaltexture)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseSimpleMaterial.ts:55

___

### occlusionStrength

• **occlusionStrength**: `number` = `1.0`

Occlusion Channel Strength.

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[occlusionStrength](PBRBaseSimpleMaterial.md#occlusionstrength)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseSimpleMaterial.ts:76

___

### occlusionTexture

• **occlusionTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Occlusion Texture of the material (adding extra occlusion effects).

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[occlusionTexture](PBRBaseSimpleMaterial.md#occlusiontexture)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseSimpleMaterial.ts:83

___

### onCompiled

• **onCompiled**: [`Nullable`](../modules.md#nullable)(`effect`: [`Effect`](Effect.md)) => `void` = `null`

Callback triggered when the material is compiled

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[onCompiled](PBRBaseSimpleMaterial.md#oncompiled)

#### Defined in

packages/dev/core/src/Materials/material.ts:381

___

### onDisposeObservable

• **onDisposeObservable**: [`Observable`](Observable.md)[`Material`](Material.md)

An event triggered when the material is disposed

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[onDisposeObservable](PBRBaseSimpleMaterial.md#ondisposeobservable)

#### Defined in

packages/dev/core/src/Materials/material.ts:420

___

### onError

• **onError**: [`Nullable`](../modules.md#nullable)(`effect`: [`Effect`](Effect.md), `errors`: `string`) => `void` = `null`

Callback triggered when an error occurs

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[onError](PBRBaseSimpleMaterial.md#onerror)

#### Defined in

packages/dev/core/src/Materials/material.ts:386

___

### pluginManager

• `Optional` **pluginManager**: [`MaterialPluginManager`](MaterialPluginManager.md)

Plugin manager for this material

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[pluginManager](PBRBaseSimpleMaterial.md#pluginmanager)

#### Defined in

packages/dev/core/src/Materials/materialPluginManager.ts:30

___

### pointSize

• **pointSize**: `number` = `1.0`

Stores the size of points

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[pointSize](PBRBaseSimpleMaterial.md#pointsize)

#### Defined in

packages/dev/core/src/Materials/material.ts:620

___

### prePassConfiguration

• `Readonly` **prePassConfiguration**: `PrePassConfiguration`

Defines additional PrePass parameters for the material.

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[prePassConfiguration](PBRBaseSimpleMaterial.md#prepassconfiguration)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:881

___

### reservedDataStore

• **reservedDataStore**: `any` = `null`

For internal use only. Please do not use.

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[reservedDataStore](PBRBaseSimpleMaterial.md#reserveddatastore)

#### Defined in

packages/dev/core/src/Materials/material.ts:259

___

### separateCullingPass

• **separateCullingPass**: `boolean` = `false`

Specifies if there should be a separate pass for culling

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[separateCullingPass](PBRBaseSimpleMaterial.md#separatecullingpass)

#### Defined in

packages/dev/core/src/Materials/material.ts:590

___

### shadowDepthWrapper

• **shadowDepthWrapper**: [`Nullable`](../modules.md#nullable)[`ShadowDepthWrapper`](ShadowDepthWrapper.md) = `null`

Custom shadow depth material to use for shadow rendering instead of the in-built one

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[shadowDepthWrapper](PBRBaseSimpleMaterial.md#shadowdepthwrapper)

#### Defined in

packages/dev/core/src/Materials/material.ts:220

___

### sheen

• `Readonly` **sheen**: [`PBRSheenConfiguration`](PBRSheenConfiguration.md)

Defines the Sheen parameters for the material.

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[sheen](PBRBaseSimpleMaterial.md#sheen)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:871

___

### sideOrientation

• **sideOrientation**: `number`

Stores the value for side orientation

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[sideOrientation](PBRBaseSimpleMaterial.md#sideorientation)

#### Defined in

packages/dev/core/src/Materials/material.ts:376

___

### specularColor

• **specularColor**: [`Color3`](Color3.md)

Specifies the specular color of the material. This indicates how reflective is the material (none to mirror).

#### Defined in

packages/dev/core/src/Materials/PBR/pbrSpecularGlossinessMaterial.ts:36

___

### specularGlossinessTexture

• **specularGlossinessTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Specifies both the specular color RGB and the glossiness A of the material per pixels.

#### Defined in

packages/dev/core/src/Materials/PBR/pbrSpecularGlossinessMaterial.ts:50

___

### state

• **state**: `string` = `""`

The state of the material

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[state](PBRBaseSimpleMaterial.md#state)

#### Defined in

packages/dev/core/src/Materials/material.ts:277

___

### stencil

• `Readonly` **stencil**: `MaterialStencilState`

Gives access to the stencil properties of the material

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[stencil](PBRBaseSimpleMaterial.md#stencil)

#### Defined in

packages/dev/core/src/Materials/material.ts:697

___

### subSurface

• `Readonly` **subSurface**: [`PBRSubSurfaceConfiguration`](PBRSubSurfaceConfiguration.md)

Defines the SubSurface parameters for the material.

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[subSurface](PBRBaseSimpleMaterial.md#subsurface)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:876

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the material

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[uniqueId](PBRBaseSimpleMaterial.md#uniqueid)

#### Defined in

packages/dev/core/src/Materials/material.ts:239

___

### useLightmapAsShadowmap

• **useLightmapAsShadowmap**: `boolean` = `false`

If true, the light map contains occlusion information instead of lighting info.

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[useLightmapAsShadowmap](PBRBaseSimpleMaterial.md#uselightmapasshadowmap)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseSimpleMaterial.ts:123

___

### zOffset

• **zOffset**: `number` = `0`

Stores the z offset Factor value

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[zOffset](PBRBaseSimpleMaterial.md#zoffset)

#### Defined in

packages/dev/core/src/Materials/material.ts:626

___

### zOffsetUnits

• **zOffsetUnits**: `number` = `0`

Stores the z offset Units value

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[zOffsetUnits](PBRBaseSimpleMaterial.md#zoffsetunits)

#### Defined in

packages/dev/core/src/Materials/material.ts:632

___

### AllDirtyFlag

▪ `Static` `Readonly` **AllDirtyFlag**: ``63``

The all dirty flag value

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[AllDirtyFlag](PBRBaseSimpleMaterial.md#alldirtyflag)

#### Defined in

packages/dev/core/src/Materials/material.ts:164

___

### AttributesDirtyFlag

▪ `Static` `Readonly` **AttributesDirtyFlag**: ``8``

The dirty attribute flag value

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[AttributesDirtyFlag](PBRBaseSimpleMaterial.md#attributesdirtyflag)

#### Defined in

packages/dev/core/src/Materials/material.ts:149

___

### ClockWiseSideOrientation

▪ `Static` `Readonly` **ClockWiseSideOrientation**: ``0``

Stores the clock-wise side orientation

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[ClockWiseSideOrientation](PBRBaseSimpleMaterial.md#clockwisesideorientation)

#### Defined in

packages/dev/core/src/Materials/material.ts:124

___

### CounterClockWiseSideOrientation

▪ `Static` `Readonly` **CounterClockWiseSideOrientation**: ``1``

Stores the counter clock-wise side orientation

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[CounterClockWiseSideOrientation](PBRBaseSimpleMaterial.md#counterclockwisesideorientation)

#### Defined in

packages/dev/core/src/Materials/material.ts:129

___

### DEFAULT\_AO\_ON\_ANALYTICAL\_LIGHTS

▪ `Static` **DEFAULT\_AO\_ON\_ANALYTICAL\_LIGHTS**: `number` = `0`

Defines the default value of how much AO map is occluding the analytical lights
(point spot...).

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[DEFAULT_AO_ON_ANALYTICAL_LIGHTS](PBRBaseSimpleMaterial.md#default_ao_on_analytical_lights)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:301

___

### FresnelDirtyFlag

▪ `Static` `Readonly` **FresnelDirtyFlag**: ``4``

The dirty fresnel flag value

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[FresnelDirtyFlag](PBRBaseSimpleMaterial.md#fresneldirtyflag)

#### Defined in

packages/dev/core/src/Materials/material.ts:144

___

### LIGHTFALLOFF\_GLTF

▪ `Static` `Readonly` **LIGHTFALLOFF\_GLTF**: ``1``

PBRMaterialLightFalloff gltf: light is falling off as described in the gltf moving to PBR document
to enhance interoperability with other engines.

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[LIGHTFALLOFF_GLTF](PBRBaseSimpleMaterial.md#lightfalloff_gltf)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:312

___

### LIGHTFALLOFF\_PHYSICAL

▪ `Static` `Readonly` **LIGHTFALLOFF\_PHYSICAL**: ``0``

PBRMaterialLightFalloff Physical: light is falling off following the inverse squared distance law.

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[LIGHTFALLOFF_PHYSICAL](PBRBaseSimpleMaterial.md#lightfalloff_physical)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:306

___

### LIGHTFALLOFF\_STANDARD

▪ `Static` `Readonly` **LIGHTFALLOFF\_STANDARD**: ``2``

PBRMaterialLightFalloff Standard: light is falling off like in the standard material
to enhance interoperability with other materials.

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[LIGHTFALLOFF_STANDARD](PBRBaseSimpleMaterial.md#lightfalloff_standard)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:318

___

### LightDirtyFlag

▪ `Static` `Readonly` **LightDirtyFlag**: ``2``

The dirty light flag value

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[LightDirtyFlag](PBRBaseSimpleMaterial.md#lightdirtyflag)

#### Defined in

packages/dev/core/src/Materials/material.ts:139

___

### LineListDrawMode

▪ `Static` `Readonly` **LineListDrawMode**: ``4``

Returns the line list draw mode

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[LineListDrawMode](PBRBaseSimpleMaterial.md#linelistdrawmode)

#### Defined in

packages/dev/core/src/Materials/material.ts:103

___

### LineLoopDrawMode

▪ `Static` `Readonly` **LineLoopDrawMode**: ``5``

Returns the line loop draw mode

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[LineLoopDrawMode](PBRBaseSimpleMaterial.md#lineloopdrawmode)

#### Defined in

packages/dev/core/src/Materials/material.ts:107

___

### LineStripDrawMode

▪ `Static` `Readonly` **LineStripDrawMode**: ``6``

Returns the line strip draw mode

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[LineStripDrawMode](PBRBaseSimpleMaterial.md#linestripdrawmode)

#### Defined in

packages/dev/core/src/Materials/material.ts:111

___

### MATERIAL\_ALPHABLEND

▪ `Static` `Readonly` **MATERIAL\_ALPHABLEND**: ``2``

MaterialTransparencyMode: Pixels are blended (according to the alpha mode) with the already drawn pixels in the current frame buffer.

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[MATERIAL_ALPHABLEND](PBRBaseSimpleMaterial.md#material_alphablend)

#### Defined in

packages/dev/core/src/Materials/material.ts:179

___

### MATERIAL\_ALPHATEST

▪ `Static` `Readonly` **MATERIAL\_ALPHATEST**: ``1``

MaterialTransparencyMode: Alpha Test mode, pixel are discarded below a certain threshold defined by the alpha cutoff value.

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[MATERIAL_ALPHATEST](PBRBaseSimpleMaterial.md#material_alphatest)

#### Defined in

packages/dev/core/src/Materials/material.ts:174

___

### MATERIAL\_ALPHATESTANDBLEND

▪ `Static` `Readonly` **MATERIAL\_ALPHATESTANDBLEND**: ``3``

MaterialTransparencyMode: Pixels are blended (according to the alpha mode) with the already drawn pixels in the current frame buffer.
They are also discarded below the alpha cutoff threshold to improve performances.

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[MATERIAL_ALPHATESTANDBLEND](PBRBaseSimpleMaterial.md#material_alphatestandblend)

#### Defined in

packages/dev/core/src/Materials/material.ts:185

___

### MATERIAL\_NORMALBLENDMETHOD\_RNM

▪ `Static` `Readonly` **MATERIAL\_NORMALBLENDMETHOD\_RNM**: ``1``

The Reoriented Normal Mapping method is used to blend normals.
Details of the algorithm can be found here: https://blog.selfshadow.com/publications/blending-in-detail/

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[MATERIAL_NORMALBLENDMETHOD_RNM](PBRBaseSimpleMaterial.md#material_normalblendmethod_rnm)

#### Defined in

packages/dev/core/src/Materials/material.ts:197

___

### MATERIAL\_NORMALBLENDMETHOD\_WHITEOUT

▪ `Static` `Readonly` **MATERIAL\_NORMALBLENDMETHOD\_WHITEOUT**: ``0``

The Whiteout method is used to blend normals.
Details of the algorithm can be found here: https://blog.selfshadow.com/publications/blending-in-detail/

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[MATERIAL_NORMALBLENDMETHOD_WHITEOUT](PBRBaseSimpleMaterial.md#material_normalblendmethod_whiteout)

#### Defined in

packages/dev/core/src/Materials/material.ts:191

___

### MATERIAL\_OPAQUE

▪ `Static` `Readonly` **MATERIAL\_OPAQUE**: ``0``

MaterialTransparencyMode: No transparency mode, Alpha channel is not use.

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[MATERIAL_OPAQUE](PBRBaseSimpleMaterial.md#material_opaque)

#### Defined in

packages/dev/core/src/Materials/material.ts:169

___

### MiscDirtyFlag

▪ `Static` `Readonly` **MiscDirtyFlag**: ``16``

The dirty misc flag value

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[MiscDirtyFlag](PBRBaseSimpleMaterial.md#miscdirtyflag)

#### Defined in

packages/dev/core/src/Materials/material.ts:154

___

### OnEventObservable

▪ `Static` **OnEventObservable**: [`Observable`](Observable.md)[`Material`](Material.md)

Event observable which raises global events common to all materials (like MaterialPluginEvent.Created)

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[OnEventObservable](PBRBaseSimpleMaterial.md#oneventobservable)

#### Defined in

packages/dev/core/src/Materials/material.ts:202

___

### PBRMATERIAL\_ALPHABLEND

▪ `Static` `Readonly` **PBRMATERIAL\_ALPHABLEND**: ``2``

PBRMaterialTransparencyMode: Pixels are blended (according to the alpha mode) with the already drawn pixels in the current frame buffer.

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[PBRMATERIAL_ALPHABLEND](PBRBaseSimpleMaterial.md#pbrmaterial_alphablend)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:289

___

### PBRMATERIAL\_ALPHATEST

▪ `Static` `Readonly` **PBRMATERIAL\_ALPHATEST**: ``1``

PBRMaterialTransparencyMode: Alpha Test mode, pixel are discarded below a certain threshold defined by the alpha cutoff value.

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[PBRMATERIAL_ALPHATEST](PBRBaseSimpleMaterial.md#pbrmaterial_alphatest)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:284

___

### PBRMATERIAL\_ALPHATESTANDBLEND

▪ `Static` `Readonly` **PBRMATERIAL\_ALPHATESTANDBLEND**: ``3``

PBRMaterialTransparencyMode: Pixels are blended (according to the alpha mode) with the already drawn pixels in the current frame buffer.
They are also discarded below the alpha cutoff threshold to improve performances.

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[PBRMATERIAL_ALPHATESTANDBLEND](PBRBaseSimpleMaterial.md#pbrmaterial_alphatestandblend)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:295

___

### PBRMATERIAL\_OPAQUE

▪ `Static` `Readonly` **PBRMATERIAL\_OPAQUE**: ``0``

PBRMaterialTransparencyMode: No transparency mode, Alpha channel is not use.

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[PBRMATERIAL_OPAQUE](PBRBaseSimpleMaterial.md#pbrmaterial_opaque)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:279

___

### PointFillMode

▪ `Static` `Readonly` **PointFillMode**: ``2``

Returns the point fill mode

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[PointFillMode](PBRBaseSimpleMaterial.md#pointfillmode)

#### Defined in

packages/dev/core/src/Materials/material.ts:95

___

### PointListDrawMode

▪ `Static` `Readonly` **PointListDrawMode**: ``3``

Returns the point list draw mode

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[PointListDrawMode](PBRBaseSimpleMaterial.md#pointlistdrawmode)

#### Defined in

packages/dev/core/src/Materials/material.ts:99

___

### PrePassDirtyFlag

▪ `Static` `Readonly` **PrePassDirtyFlag**: ``32``

The dirty prepass flag value

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[PrePassDirtyFlag](PBRBaseSimpleMaterial.md#prepassdirtyflag)

#### Defined in

packages/dev/core/src/Materials/material.ts:159

___

### TextureDirtyFlag

▪ `Static` `Readonly` **TextureDirtyFlag**: ``1``

The dirty texture flag value

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[TextureDirtyFlag](PBRBaseSimpleMaterial.md#texturedirtyflag)

#### Defined in

packages/dev/core/src/Materials/material.ts:134

___

### TriangleFanDrawMode

▪ `Static` `Readonly` **TriangleFanDrawMode**: ``8``

Returns the triangle fan draw mode

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[TriangleFanDrawMode](PBRBaseSimpleMaterial.md#trianglefandrawmode)

#### Defined in

packages/dev/core/src/Materials/material.ts:119

___

### TriangleFillMode

▪ `Static` `Readonly` **TriangleFillMode**: ``0``

Returns the triangle fill mode

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[TriangleFillMode](PBRBaseSimpleMaterial.md#trianglefillmode)

#### Defined in

packages/dev/core/src/Materials/material.ts:87

___

### TriangleStripDrawMode

▪ `Static` `Readonly` **TriangleStripDrawMode**: ``7``

Returns the triangle strip draw mode

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[TriangleStripDrawMode](PBRBaseSimpleMaterial.md#trianglestripdrawmode)

#### Defined in

packages/dev/core/src/Materials/material.ts:115

___

### WireFrameFillMode

▪ `Static` `Readonly` **WireFrameFillMode**: ``1``

Returns the wireframe mode

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[WireFrameFillMode](PBRBaseSimpleMaterial.md#wireframefillmode)

#### Defined in

packages/dev/core/src/Materials/material.ts:91

## Accessors

### \_disableAlphaBlending

• `Protected` `get` **_disableAlphaBlending**(): `boolean`

Returns true if alpha blending should be disabled.

#### Returns

`boolean`

#### Inherited from

PBRBaseSimpleMaterial.\_disableAlphaBlending

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:970

___

### alpha

• `get` **alpha**(): `number`

Gets the alpha value of the material

#### Returns

`number`

#### Inherited from

PBRBaseSimpleMaterial.alpha

#### Defined in

packages/dev/core/src/Materials/material.ts:320

• `set` **alpha**(`value`): `void`

Sets the alpha value of the material

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

PBRBaseSimpleMaterial.alpha

#### Defined in

packages/dev/core/src/Materials/material.ts:303

___

### alphaMode

• `get` **alphaMode**(): `number`

Gets the value of the alpha mode

#### Returns

`number`

#### Inherited from

PBRBaseSimpleMaterial.alphaMode

#### Defined in

packages/dev/core/src/Materials/material.ts:525

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

PBRBaseSimpleMaterial.alphaMode

#### Defined in

packages/dev/core/src/Materials/material.ts:514

___

### backFaceCulling

• `get` **backFaceCulling**(): `boolean`

Gets the culling state

#### Returns

`boolean`

#### Inherited from

PBRBaseSimpleMaterial.backFaceCulling

#### Defined in

packages/dev/core/src/Materials/material.ts:344

• `set` **backFaceCulling**(`value`): `void`

Sets the culling state (true to enable culling, false to disable)

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

PBRBaseSimpleMaterial.backFaceCulling

#### Defined in

packages/dev/core/src/Materials/material.ts:333

___

### canRenderToMRT

• `get` **canRenderToMRT**(): `boolean`

Can this material render to several textures at once

#### Returns

`boolean`

#### Inherited from

PBRBaseSimpleMaterial.canRenderToMRT

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:742

___

### cullBackFaces

• `get` **cullBackFaces**(): `boolean`

Gets the type of faces that should be culled

#### Returns

`boolean`

#### Inherited from

PBRBaseSimpleMaterial.cullBackFaces

#### Defined in

packages/dev/core/src/Materials/material.ts:368

• `set` **cullBackFaces**(`value`): `void`

Sets the type of faces that should be culled (true for back faces, false for front faces)

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

PBRBaseSimpleMaterial.cullBackFaces

#### Defined in

packages/dev/core/src/Materials/material.ts:357

___

### doubleSided

• `get` **doubleSided**(): `boolean`

Gets the current double sided mode.

#### Returns

`boolean`

#### Inherited from

PBRBaseSimpleMaterial.doubleSided

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseSimpleMaterial.ts:95

• `set` **doubleSided**(`value`): `void`

If sets to true and backfaceCulling is false, normals will be flipped on the backside.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

PBRBaseSimpleMaterial.doubleSided

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseSimpleMaterial.ts:102

___

### fillMode

• `get` **fillMode**(): `number`

Gets the material fill mode

#### Returns

`number`

#### Inherited from

PBRBaseSimpleMaterial.fillMode

#### Defined in

packages/dev/core/src/Materials/material.ts:677

• `set` **fillMode**(`value`): `void`

Sets the material fill mode

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

PBRBaseSimpleMaterial.fillMode

#### Defined in

packages/dev/core/src/Materials/material.ts:685

___

### fogEnabled

• `get` **fogEnabled**(): `boolean`

Gets the value of the fog enabled state

#### Returns

`boolean`

#### Inherited from

PBRBaseSimpleMaterial.fogEnabled

#### Defined in

packages/dev/core/src/Materials/material.ts:612

• `set` **fogEnabled**(`value`): `void`

Sets the state for enabling fog

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

PBRBaseSimpleMaterial.fogEnabled

#### Defined in

packages/dev/core/src/Materials/material.ts:601

___

### hasRenderTargetTextures

• `get` **hasRenderTargetTextures**(): `boolean`

Gets a boolean indicating that current material needs to register RTT

#### Returns

`boolean`

#### Inherited from

PBRBaseSimpleMaterial.hasRenderTargetTextures

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:930

___

### isFrozen

• `get` **isFrozen**(): `boolean`

Specifies if updates for the material been locked

#### Returns

`boolean`

#### Inherited from

PBRBaseSimpleMaterial.isFrozen

#### Defined in

packages/dev/core/src/Materials/material.ts:883

___

### isPrePassCapable

• `get` **isPrePassCapable**(): `boolean`

Can this material render to prepass

#### Returns

`boolean`

#### Inherited from

PBRBaseSimpleMaterial.isPrePassCapable

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:941

___

### needDepthPrePass

• `get` **needDepthPrePass**(): `boolean`

Gets the depth pre-pass value

#### Returns

`boolean`

#### Inherited from

PBRBaseSimpleMaterial.needDepthPrePass

#### Defined in

packages/dev/core/src/Materials/material.ts:551

• `set` **needDepthPrePass**(`value`): `void`

Sets the need depth pre-pass value

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

PBRBaseSimpleMaterial.needDepthPrePass

#### Defined in

packages/dev/core/src/Materials/material.ts:538

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

PBRBaseSimpleMaterial.onBind

#### Defined in

packages/dev/core/src/Materials/material.ts:459

___

### onBindObservable

• `get` **onBindObservable**(): [`Observable`](Observable.md)[`AbstractMesh`](AbstractMesh.md)

An event triggered when the material is bound

#### Returns

[`Observable`](Observable.md)[`AbstractMesh`](AbstractMesh.md)

#### Inherited from

PBRBaseSimpleMaterial.onBindObservable

#### Defined in

packages/dev/core/src/Materials/material.ts:443

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

PBRBaseSimpleMaterial.onDispose

#### Defined in

packages/dev/core/src/Materials/material.ts:431

___

### onEffectCreatedObservable

• `get` **onEffectCreatedObservable**(): [`Observable`](Observable.md){ `effect`: [`Effect`](Effect.md) ; `subMesh`: [`Nullable`](../modules.md#nullable)[`SubMesh`](SubMesh.md)  }

An event triggered when the effect is (re)created

#### Returns

[`Observable`](Observable.md){ `effect`: [`Effect`](Effect.md) ; `subMesh`: [`Nullable`](../modules.md#nullable)[`SubMesh`](SubMesh.md)  }

#### Inherited from

PBRBaseSimpleMaterial.onEffectCreatedObservable

#### Defined in

packages/dev/core/src/Materials/material.ts:482

___

### onUnBindObservable

• `get` **onUnBindObservable**(): [`Observable`](Observable.md)[`Material`](Material.md)

An event triggered when the material is unbound

#### Returns

[`Observable`](Observable.md)[`Material`](Material.md)

#### Inherited from

PBRBaseSimpleMaterial.onUnBindObservable

#### Defined in

packages/dev/core/src/Materials/material.ts:469

___

### pointsCloud

• `get` **pointsCloud**(): `boolean`

Gets the value specifying if point clouds are enabled

#### Returns

`boolean`

#### Inherited from

PBRBaseSimpleMaterial.pointsCloud

#### Defined in

packages/dev/core/src/Materials/material.ts:656

• `set` **pointsCloud**(`value`): `void`

Sets the state of point cloud mode

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

PBRBaseSimpleMaterial.pointsCloud

#### Defined in

packages/dev/core/src/Materials/material.ts:670

___

### realTimeFiltering

• `get` **realTimeFiltering**(): `boolean`

Enables realtime filtering on the texture.

#### Returns

`boolean`

#### Inherited from

PBRBaseSimpleMaterial.realTimeFiltering

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:719

• `set` **realTimeFiltering**(`b`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `b` | `boolean` |

#### Returns

`void`

#### Inherited from

PBRBaseSimpleMaterial.realTimeFiltering

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:722

___

### realTimeFilteringQuality

• `get` **realTimeFilteringQuality**(): `number`

Quality switch for realtime filtering

#### Returns

`number`

#### Inherited from

PBRBaseSimpleMaterial.realTimeFilteringQuality

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:731

• `set` **realTimeFilteringQuality**(`n`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `n` | `number` |

#### Returns

`void`

#### Inherited from

PBRBaseSimpleMaterial.realTimeFilteringQuality

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:734

___

### transparencyMode

• `get` **transparencyMode**(): [`Nullable`](../modules.md#nullable)`number`

Gets the current transparency mode.

#### Returns

[`Nullable`](../modules.md#nullable)`number`

#### Inherited from

PBRBaseSimpleMaterial.transparencyMode

#### Defined in

packages/dev/core/src/Materials/material.ts:964

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

PBRBaseSimpleMaterial.transparencyMode

#### Defined in

packages/dev/core/src/Materials/material.ts:980

___

### useLogarithmicDepth

• `get` **useLogarithmicDepth**(): `boolean`

Enabled the use of logarithmic depth buffers, which is good for wide depth buffers.

#### Returns

`boolean`

#### Inherited from

PBRBaseSimpleMaterial.useLogarithmicDepth

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:955

• `set` **useLogarithmicDepth**(`value`): `void`

Enabled the use of logarithmic depth buffers, which is good for wide depth buffers.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

PBRBaseSimpleMaterial.useLogarithmicDepth

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:963

___

### useMicroSurfaceFromReflectivityMapAlpha

• `get` **useMicroSurfaceFromReflectivityMapAlpha**(): `boolean`

Specifies if the reflectivity texture contains the glossiness information in its alpha channel.

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Materials/PBR/pbrSpecularGlossinessMaterial.ts:55

___

### wireframe

• `get` **wireframe**(): `boolean`

#### Returns

`boolean`

#### Inherited from

PBRBaseSimpleMaterial.wireframe

#### Defined in

packages/dev/core/src/Materials/material.ts:634

• `set` **wireframe**(`value`): `void`

Sets the state of wireframe mode

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

PBRBaseSimpleMaterial.wireframe

#### Defined in

packages/dev/core/src/Materials/material.ts:649

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

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[_afterBind](PBRBaseSimpleMaterial.md#_afterbind)

#### Defined in

packages/dev/core/src/Materials/pushMaterial.ts:80

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

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[_attachImageProcessingConfiguration](PBRBaseSimpleMaterial.md#_attachimageprocessingconfiguration)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:775

___

### \_hasAlphaChannel

▸ `Protected` **_hasAlphaChannel**(): `boolean`

Specifies whether or not there is a usable alpha channel for transparency.

#### Returns

`boolean`

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[_hasAlphaChannel](PBRBaseSimpleMaterial.md#_hasalphachannel)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:1014

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

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[_isReadyForSubMesh](PBRBaseSimpleMaterial.md#_isreadyforsubmesh)

#### Defined in

packages/dev/core/src/Materials/pushMaterial.ts:43

___

### \_markAllSubMeshesAsAllDirty

▸ `Protected` **_markAllSubMeshesAsAllDirty**(): `void`

Indicates that we need to re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[_markAllSubMeshesAsAllDirty](PBRBaseSimpleMaterial.md#_markallsubmeshesasalldirty)

#### Defined in

packages/dev/core/src/Materials/material.ts:1543

___

### \_markAllSubMeshesAsAttributesDirty

▸ `Protected` **_markAllSubMeshesAsAttributesDirty**(): `void`

Indicates that attributes need to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[_markAllSubMeshesAsAttributesDirty](PBRBaseSimpleMaterial.md#_markallsubmeshesasattributesdirty)

#### Defined in

packages/dev/core/src/Materials/material.ts:1585

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

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[_markAllSubMeshesAsDirty](PBRBaseSimpleMaterial.md#_markallsubmeshesasdirty)

#### Defined in

packages/dev/core/src/Materials/material.ts:1498

___

### \_markAllSubMeshesAsFresnelAndMiscDirty

▸ `Protected` **_markAllSubMeshesAsFresnelAndMiscDirty**(): `void`

Indicates that fresnel and misc need to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[_markAllSubMeshesAsFresnelAndMiscDirty](PBRBaseSimpleMaterial.md#_markallsubmeshesasfresnelandmiscdirty)

#### Defined in

packages/dev/core/src/Materials/material.ts:1571

___

### \_markAllSubMeshesAsFresnelDirty

▸ `Protected` **_markAllSubMeshesAsFresnelDirty**(): `void`

Indicates that fresnel needs to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[_markAllSubMeshesAsFresnelDirty](PBRBaseSimpleMaterial.md#_markallsubmeshesasfresneldirty)

#### Defined in

packages/dev/core/src/Materials/material.ts:1564

___

### \_markAllSubMeshesAsImageProcessingDirty

▸ `Protected` **_markAllSubMeshesAsImageProcessingDirty**(): `void`

Indicates that image processing needs to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[_markAllSubMeshesAsImageProcessingDirty](PBRBaseSimpleMaterial.md#_markallsubmeshesasimageprocessingdirty)

#### Defined in

packages/dev/core/src/Materials/material.ts:1550

___

### \_markAllSubMeshesAsLightsDirty

▸ `Protected` **_markAllSubMeshesAsLightsDirty**(): `void`

Indicates that lights need to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[_markAllSubMeshesAsLightsDirty](PBRBaseSimpleMaterial.md#_markallsubmeshesaslightsdirty)

#### Defined in

packages/dev/core/src/Materials/material.ts:1578

___

### \_markAllSubMeshesAsMiscDirty

▸ `Protected` **_markAllSubMeshesAsMiscDirty**(): `void`

Indicates that misc needs to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[_markAllSubMeshesAsMiscDirty](PBRBaseSimpleMaterial.md#_markallsubmeshesasmiscdirty)

#### Defined in

packages/dev/core/src/Materials/material.ts:1592

___

### \_markAllSubMeshesAsPrePassDirty

▸ `Protected` **_markAllSubMeshesAsPrePassDirty**(): `void`

Indicates that prepass needs to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[_markAllSubMeshesAsPrePassDirty](PBRBaseSimpleMaterial.md#_markallsubmeshesasprepassdirty)

#### Defined in

packages/dev/core/src/Materials/material.ts:1599

___

### \_markAllSubMeshesAsTexturesAndMiscDirty

▸ `Protected` **_markAllSubMeshesAsTexturesAndMiscDirty**(): `void`

Indicates that textures and misc need to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[_markAllSubMeshesAsTexturesAndMiscDirty](PBRBaseSimpleMaterial.md#_markallsubmeshesastexturesandmiscdirty)

#### Defined in

packages/dev/core/src/Materials/material.ts:1606

___

### \_markAllSubMeshesAsTexturesDirty

▸ `Protected` **_markAllSubMeshesAsTexturesDirty**(): `void`

Indicates that textures need to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[_markAllSubMeshesAsTexturesDirty](PBRBaseSimpleMaterial.md#_markallsubmeshesastexturesdirty)

#### Defined in

packages/dev/core/src/Materials/material.ts:1557

___

### \_markScenePrePassDirty

▸ `Protected` **_markScenePrePassDirty**(): `void`

Indicates that the scene should check if the rendering now needs a prepass

#### Returns

`void`

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[_markScenePrePassDirty](PBRBaseSimpleMaterial.md#_marksceneprepassdirty)

#### Defined in

packages/dev/core/src/Materials/material.ts:1529

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

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[_mustRebind](PBRBaseSimpleMaterial.md#_mustrebind)

#### Defined in

packages/dev/core/src/Materials/pushMaterial.ts:85

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

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[_shouldTurnAlphaTestOn](PBRBaseSimpleMaterial.md#_shouldturnalphateston)

#### Defined in

packages/dev/core/src/Materials/material.ts:1040

___

### \_shouldUseAlphaFromAlbedoTexture

▸ `Protected` **_shouldUseAlphaFromAlbedoTexture**(): `boolean`

Specifies whether or not the alpha value of the albedo texture should be used for alpha blending.

#### Returns

`boolean`

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[_shouldUseAlphaFromAlbedoTexture](PBRBaseSimpleMaterial.md#_shouldusealphafromalbedotexture)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:1007

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

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[bind](PBRBaseSimpleMaterial.md#bind)

#### Defined in

packages/dev/core/src/Materials/pushMaterial.ts:72

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

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[bindEyePosition](PBRBaseSimpleMaterial.md#bindeyeposition)

#### Defined in

packages/dev/core/src/Materials/material.ts:1168

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

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[bindForSubMesh](PBRBaseSimpleMaterial.md#bindforsubmesh)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:1956

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

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[bindOnlyNormalMatrix](PBRBaseSimpleMaterial.md#bindonlynormalmatrix)

#### Defined in

packages/dev/core/src/Materials/pushMaterial.ts:68

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

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[bindOnlyWorldMatrix](PBRBaseSimpleMaterial.md#bindonlyworldmatrix)

#### Defined in

packages/dev/core/src/Materials/pushMaterial.ts:59

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

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[bindView](PBRBaseSimpleMaterial.md#bindview)

#### Defined in

packages/dev/core/src/Materials/material.ts:1142

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

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[bindViewProjection](PBRBaseSimpleMaterial.md#bindviewprojection)

#### Defined in

packages/dev/core/src/Materials/material.ts:1154

___

### buildUniformLayout

▸ **buildUniformLayout**(): `void`

Initializes the uniform buffer layout for the shader.

#### Returns

`void`

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[buildUniformLayout](PBRBaseSimpleMaterial.md#builduniformlayout)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:1883

___

### clone

▸ **clone**(`name`): [`PBRSpecularGlossinessMaterial`](PBRSpecularGlossinessMaterial.md)

Makes a duplicate of the current material.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | name to use for the new material. |

#### Returns

[`PBRSpecularGlossinessMaterial`](PBRSpecularGlossinessMaterial.md)

#### Overrides

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[clone](PBRBaseSimpleMaterial.md#clone)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrSpecularGlossinessMaterial.ts:81

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

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[dispose](PBRBaseSimpleMaterial.md#dispose)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:2496

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

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[forceCompilation](PBRBaseSimpleMaterial.md#forcecompilation)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:1848

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

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[forceCompilationAsync](PBRBaseSimpleMaterial.md#forcecompilationasync)

#### Defined in

packages/dev/core/src/Materials/material.ts:1392

___

### freeze

▸ **freeze**(): `void`

Locks updates for the material

#### Returns

`void`

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[freeze](PBRBaseSimpleMaterial.md#freeze)

#### Defined in

packages/dev/core/src/Materials/material.ts:890

___

### getActiveTextures

▸ **getActiveTextures**(): [`BaseTexture`](BaseTexture.md)[]

Returns an array of the actively used textures.

#### Returns

[`BaseTexture`](BaseTexture.md)[]

- Array of BaseTextures

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[getActiveTextures](PBRBaseSimpleMaterial.md#getactivetextures)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:2364

___

### getAlphaTestTexture

▸ **getAlphaTestTexture**(): [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Gets the texture used for the alpha test.

#### Returns

[`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[getAlphaTestTexture](PBRBaseSimpleMaterial.md#getalphatesttexture)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:1021

___

### getAnimatables

▸ **getAnimatables**(): [`IAnimatable`](../interfaces/IAnimatable.md)[]

Returns the animatable textures.

#### Returns

[`IAnimatable`](../interfaces/IAnimatable.md)[]

- Array of animatable textures.

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[getAnimatables](PBRBaseSimpleMaterial.md#getanimatables)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:2308

___

### getBindedMeshes

▸ **getBindedMeshes**(): [`AbstractMesh`](AbstractMesh.md)[]

Gets the meshes bound to the material

#### Returns

[`AbstractMesh`](AbstractMesh.md)[]

an array of meshes bound to the material

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[getBindedMeshes](PBRBaseSimpleMaterial.md#getbindedmeshes)

#### Defined in

packages/dev/core/src/Materials/material.ts:1289

___

### getClassName

▸ **getClassName**(): `string`

Return the current class name of the material.

#### Returns

`string`

#### Overrides

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[getClassName](PBRBaseSimpleMaterial.md#getclassname)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrSpecularGlossinessMaterial.ts:73

___

### getEffect

▸ **getEffect**(): [`Effect`](Effect.md)

#### Returns

[`Effect`](Effect.md)

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[getEffect](PBRBaseSimpleMaterial.md#geteffect)

#### Defined in

packages/dev/core/src/Materials/pushMaterial.ts:23

___

### getScene

▸ **getScene**(): [`Scene`](Scene.md)

Returns the current scene

#### Returns

[`Scene`](Scene.md)

a Scene

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[getScene](PBRBaseSimpleMaterial.md#getscene)

#### Defined in

packages/dev/core/src/Materials/material.ts:947

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

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[hasTexture](PBRBaseSimpleMaterial.md#hastexture)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:2423

___

### isMetallicWorkflow

▸ **isMetallicWorkflow**(): `boolean`

Specifies if the material uses metallic roughness workflow.

#### Returns

`boolean`

boolean specifying if the material uses metallic roughness workflow.

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[isMetallicWorkflow](PBRBaseSimpleMaterial.md#ismetallicworkflow)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:1208

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

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[isReady](PBRBaseSimpleMaterial.md#isready)

#### Defined in

packages/dev/core/src/Materials/pushMaterial.ts:27

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

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[isReadyForSubMesh](PBRBaseSimpleMaterial.md#isreadyforsubmesh)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:1032

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

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[markAsDirty](PBRBaseSimpleMaterial.md#markasdirty)

#### Defined in

packages/dev/core/src/Materials/material.ts:1437

___

### markDirty

▸ **markDirty**(): `void`

Marks the material to indicate that it needs to be re-calculated

#### Returns

`void`

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[markDirty](PBRBaseSimpleMaterial.md#markdirty)

#### Defined in

packages/dev/core/src/Materials/material.ts:1055

___

### needAlphaBlending

▸ **needAlphaBlending**(): `boolean`

Specifies whether or not this material should be rendered in alpha blend mode.

#### Returns

`boolean`

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[needAlphaBlending](PBRBaseSimpleMaterial.md#needalphablending)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:981

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

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[needAlphaBlendingForMesh](PBRBaseSimpleMaterial.md#needalphablendingformesh)

#### Defined in

packages/dev/core/src/Materials/material.ts:1016

___

### needAlphaTesting

▸ **needAlphaTesting**(): `boolean`

Specifies whether or not this material should be rendered in alpha test mode.

#### Returns

`boolean`

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[needAlphaTesting](PBRBaseSimpleMaterial.md#needalphatesting)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:992

___

### resetDrawCache

▸ **resetDrawCache**(): `void`

Resets the draw wrappers cache for all submeshes that are using this material

#### Returns

`void`

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[resetDrawCache](PBRBaseSimpleMaterial.md#resetdrawcache)

#### Defined in

packages/dev/core/src/Materials/material.ts:1478

___

### serialize

▸ **serialize**(): `any`

Serialize the material to a parsable JSON object.

#### Returns

`any`

#### Overrides

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[serialize](PBRBaseSimpleMaterial.md#serialize)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrSpecularGlossinessMaterial.ts:99

___

### setPrePassRenderer

▸ **setPrePassRenderer**(): `boolean`

Sets the required values to the prepass renderer.

#### Returns

`boolean`

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[setPrePassRenderer](PBRBaseSimpleMaterial.md#setprepassrenderer)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrBaseMaterial.ts:2478

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

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[toString](PBRBaseSimpleMaterial.md#tostring)

#### Defined in

packages/dev/core/src/Materials/material.ts:867

___

### unbind

▸ **unbind**(): `void`

Unbinds the material from the mesh

#### Returns

`void`

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[unbind](PBRBaseSimpleMaterial.md#unbind)

#### Defined in

packages/dev/core/src/Materials/material.ts:1222

___

### unfreeze

▸ **unfreeze**(): `void`

Unlocks updates for the material

#### Returns

`void`

#### Inherited from

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[unfreeze](PBRBaseSimpleMaterial.md#unfreeze)

#### Defined in

packages/dev/core/src/Materials/material.ts:898

___

### Parse

▸ `Static` **Parse**(`source`, `scene`, `rootUrl`): [`PBRSpecularGlossinessMaterial`](PBRSpecularGlossinessMaterial.md)

Parses a JSON object corresponding to the serialize function.

#### Parameters

| Name | Type |
| :------ | :------ |
| `source` | `any` |
| `scene` | [`Scene`](Scene.md) |
| `rootUrl` | `string` |

#### Returns

[`PBRSpecularGlossinessMaterial`](PBRSpecularGlossinessMaterial.md)

#### Overrides

[PBRBaseSimpleMaterial](PBRBaseSimpleMaterial.md).[Parse](PBRBaseSimpleMaterial.md#parse)

#### Defined in

packages/dev/core/src/Materials/PBR/pbrSpecularGlossinessMaterial.ts:119
