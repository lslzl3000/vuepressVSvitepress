[@dev/core](../README.md) / [Exports](../modules.md) / StandardMaterial

# Class: StandardMaterial

This is the default material used in Babylon. It is the best trade off between quality
and performances.

**`See`**

https://doc.babylonjs.com/babylon101/materials

## Hierarchy

- `PushMaterial`

  ↳ **`StandardMaterial`**

## Table of contents

### Constructors

- [constructor](StandardMaterial.md#constructor)

### Properties

- [\_activeEffect](StandardMaterial.md#_activeeffect)
- [\_alpha](StandardMaterial.md#_alpha)
- [\_ambientTexture](StandardMaterial.md#_ambienttexture)
- [\_backFaceCulling](StandardMaterial.md#_backfaceculling)
- [\_bumpTexture](StandardMaterial.md#_bumptexture)
- [\_cacheHasRenderTargetTextures](StandardMaterial.md#_cachehasrendertargettextures)
- [\_cullBackFaces](StandardMaterial.md#_cullbackfaces)
- [\_diffuseFresnelParameters](StandardMaterial.md#_diffusefresnelparameters)
- [\_diffuseTexture](StandardMaterial.md#_diffusetexture)
- [\_disableLighting](StandardMaterial.md#_disablelighting)
- [\_drawWrapper](StandardMaterial.md#_drawwrapper)
- [\_emissiveFresnelParameters](StandardMaterial.md#_emissivefresnelparameters)
- [\_emissiveTexture](StandardMaterial.md#_emissivetexture)
- [\_eventInfo](StandardMaterial.md#_eventinfo)
- [\_forceAlphaTest](StandardMaterial.md#_forcealphatest)
- [\_globalAmbientColor](StandardMaterial.md#_globalambientcolor)
- [\_imageProcessingConfiguration](StandardMaterial.md#_imageprocessingconfiguration)
- [\_imageProcessingObserver](StandardMaterial.md#_imageprocessingobserver)
- [\_invertNormalMapX](StandardMaterial.md#_invertnormalmapx)
- [\_invertNormalMapY](StandardMaterial.md#_invertnormalmapy)
- [\_lightmapTexture](StandardMaterial.md#_lightmaptexture)
- [\_linkEmissiveWithDiffuse](StandardMaterial.md#_linkemissivewithdiffuse)
- [\_maxSimultaneousLights](StandardMaterial.md#_maxsimultaneouslights)
- [\_needToBindSceneUbo](StandardMaterial.md#_needtobindsceneubo)
- [\_normalMatrix](StandardMaterial.md#_normalmatrix)
- [\_onEffectCreatedObservable](StandardMaterial.md#_oneffectcreatedobservable)
- [\_opacityFresnelParameters](StandardMaterial.md#_opacityfresnelparameters)
- [\_opacityTexture](StandardMaterial.md#_opacitytexture)
- [\_reflectionFresnelParameters](StandardMaterial.md#_reflectionfresnelparameters)
- [\_reflectionTexture](StandardMaterial.md#_reflectiontexture)
- [\_refractionFresnelParameters](StandardMaterial.md#_refractionfresnelparameters)
- [\_refractionTexture](StandardMaterial.md#_refractiontexture)
- [\_renderTargets](StandardMaterial.md#_rendertargets)
- [\_roughness](StandardMaterial.md#_roughness)
- [\_specularTexture](StandardMaterial.md#_speculartexture)
- [\_transparencyMode](StandardMaterial.md#_transparencymode)
- [\_twoSidedLighting](StandardMaterial.md#_twosidedlighting)
- [\_useAlphaFromDiffuseTexture](StandardMaterial.md#_usealphafromdiffusetexture)
- [\_useEmissiveAsIllumination](StandardMaterial.md#_useemissiveasillumination)
- [\_useGlossinessFromSpecularMapAlpha](StandardMaterial.md#_useglossinessfromspecularmapalpha)
- [\_useLightmapAsShadowmap](StandardMaterial.md#_uselightmapasshadowmap)
- [\_useLogarithmicDepth](StandardMaterial.md#_uselogarithmicdepth)
- [\_useObjectSpaceNormalMap](StandardMaterial.md#_useobjectspacenormalmap)
- [\_useParallax](StandardMaterial.md#_useparallax)
- [\_useParallaxOcclusion](StandardMaterial.md#_useparallaxocclusion)
- [\_useReflectionFresnelFromSpecular](StandardMaterial.md#_usereflectionfresnelfromspecular)
- [\_useReflectionOverAlpha](StandardMaterial.md#_usereflectionoveralpha)
- [\_useSpecularOverAlpha](StandardMaterial.md#_usespecularoveralpha)
- [\_worldViewProjectionMatrix](StandardMaterial.md#_worldviewprojectionmatrix)
- [allowShaderHotSwapping](StandardMaterial.md#allowshaderhotswapping)
- [alphaCutOff](StandardMaterial.md#alphacutoff)
- [ambientColor](StandardMaterial.md#ambientcolor)
- [ambientTexture](StandardMaterial.md#ambienttexture)
- [animations](StandardMaterial.md#animations)
- [bumpTexture](StandardMaterial.md#bumptexture)
- [checkReadyOnEveryCall](StandardMaterial.md#checkreadyoneverycall)
- [checkReadyOnlyOnce](StandardMaterial.md#checkreadyonlyonce)
- [customShaderNameResolve](StandardMaterial.md#customshadernameresolve)
- [depthFunction](StandardMaterial.md#depthfunction)
- [detailMap](StandardMaterial.md#detailmap)
- [diffuseColor](StandardMaterial.md#diffusecolor)
- [diffuseFresnelParameters](StandardMaterial.md#diffusefresnelparameters)
- [diffuseTexture](StandardMaterial.md#diffusetexture)
- [disableColorWrite](StandardMaterial.md#disablecolorwrite)
- [disableDepthWrite](StandardMaterial.md#disabledepthwrite)
- [disableLighting](StandardMaterial.md#disablelighting)
- [doNotSerialize](StandardMaterial.md#donotserialize)
- [emissiveColor](StandardMaterial.md#emissivecolor)
- [emissiveFresnelParameters](StandardMaterial.md#emissivefresnelparameters)
- [emissiveTexture](StandardMaterial.md#emissivetexture)
- [forceDepthWrite](StandardMaterial.md#forcedepthwrite)
- [getRenderTargetTextures](StandardMaterial.md#getrendertargettextures)
- [id](StandardMaterial.md#id)
- [indexOfRefraction](StandardMaterial.md#indexofrefraction)
- [inspectableCustomProperties](StandardMaterial.md#inspectablecustomproperties)
- [invertNormalMapX](StandardMaterial.md#invertnormalmapx)
- [invertNormalMapY](StandardMaterial.md#invertnormalmapy)
- [invertRefractionY](StandardMaterial.md#invertrefractiony)
- [lightmapTexture](StandardMaterial.md#lightmaptexture)
- [linkEmissiveWithDiffuse](StandardMaterial.md#linkemissivewithdiffuse)
- [maxSimultaneousLights](StandardMaterial.md#maxsimultaneouslights)
- [metadata](StandardMaterial.md#metadata)
- [name](StandardMaterial.md#name)
- [onCompiled](StandardMaterial.md#oncompiled)
- [onDisposeObservable](StandardMaterial.md#ondisposeobservable)
- [onError](StandardMaterial.md#onerror)
- [opacityFresnelParameters](StandardMaterial.md#opacityfresnelparameters)
- [opacityTexture](StandardMaterial.md#opacitytexture)
- [parallaxScaleBias](StandardMaterial.md#parallaxscalebias)
- [pluginManager](StandardMaterial.md#pluginmanager)
- [pointSize](StandardMaterial.md#pointsize)
- [prePassConfiguration](StandardMaterial.md#prepassconfiguration)
- [reflectionFresnelParameters](StandardMaterial.md#reflectionfresnelparameters)
- [reflectionTexture](StandardMaterial.md#reflectiontexture)
- [refractionFresnelParameters](StandardMaterial.md#refractionfresnelparameters)
- [refractionTexture](StandardMaterial.md#refractiontexture)
- [reservedDataStore](StandardMaterial.md#reserveddatastore)
- [roughness](StandardMaterial.md#roughness)
- [separateCullingPass](StandardMaterial.md#separatecullingpass)
- [shadowDepthWrapper](StandardMaterial.md#shadowdepthwrapper)
- [sideOrientation](StandardMaterial.md#sideorientation)
- [specularColor](StandardMaterial.md#specularcolor)
- [specularPower](StandardMaterial.md#specularpower)
- [specularTexture](StandardMaterial.md#speculartexture)
- [state](StandardMaterial.md#state)
- [stencil](StandardMaterial.md#stencil)
- [twoSidedLighting](StandardMaterial.md#twosidedlighting)
- [uniqueId](StandardMaterial.md#uniqueid)
- [useAlphaFromDiffuseTexture](StandardMaterial.md#usealphafromdiffusetexture)
- [useEmissiveAsIllumination](StandardMaterial.md#useemissiveasillumination)
- [useGlossinessFromSpecularMapAlpha](StandardMaterial.md#useglossinessfromspecularmapalpha)
- [useLightmapAsShadowmap](StandardMaterial.md#uselightmapasshadowmap)
- [useObjectSpaceNormalMap](StandardMaterial.md#useobjectspacenormalmap)
- [useParallax](StandardMaterial.md#useparallax)
- [useParallaxOcclusion](StandardMaterial.md#useparallaxocclusion)
- [useReflectionFresnelFromSpecular](StandardMaterial.md#usereflectionfresnelfromspecular)
- [useReflectionOverAlpha](StandardMaterial.md#usereflectionoveralpha)
- [useSpecularOverAlpha](StandardMaterial.md#usespecularoveralpha)
- [zOffset](StandardMaterial.md#zoffset)
- [zOffsetUnits](StandardMaterial.md#zoffsetunits)
- [AllDirtyFlag](StandardMaterial.md#alldirtyflag)
- [AttributesDirtyFlag](StandardMaterial.md#attributesdirtyflag)
- [ClockWiseSideOrientation](StandardMaterial.md#clockwisesideorientation)
- [CounterClockWiseSideOrientation](StandardMaterial.md#counterclockwisesideorientation)
- [FresnelDirtyFlag](StandardMaterial.md#fresneldirtyflag)
- [LightDirtyFlag](StandardMaterial.md#lightdirtyflag)
- [LineListDrawMode](StandardMaterial.md#linelistdrawmode)
- [LineLoopDrawMode](StandardMaterial.md#lineloopdrawmode)
- [LineStripDrawMode](StandardMaterial.md#linestripdrawmode)
- [MATERIAL\_ALPHABLEND](StandardMaterial.md#material_alphablend)
- [MATERIAL\_ALPHATEST](StandardMaterial.md#material_alphatest)
- [MATERIAL\_ALPHATESTANDBLEND](StandardMaterial.md#material_alphatestandblend)
- [MATERIAL\_NORMALBLENDMETHOD\_RNM](StandardMaterial.md#material_normalblendmethod_rnm)
- [MATERIAL\_NORMALBLENDMETHOD\_WHITEOUT](StandardMaterial.md#material_normalblendmethod_whiteout)
- [MATERIAL\_OPAQUE](StandardMaterial.md#material_opaque)
- [MiscDirtyFlag](StandardMaterial.md#miscdirtyflag)
- [OnEventObservable](StandardMaterial.md#oneventobservable)
- [PointFillMode](StandardMaterial.md#pointfillmode)
- [PointListDrawMode](StandardMaterial.md#pointlistdrawmode)
- [PrePassDirtyFlag](StandardMaterial.md#prepassdirtyflag)
- [TextureDirtyFlag](StandardMaterial.md#texturedirtyflag)
- [TriangleFanDrawMode](StandardMaterial.md#trianglefandrawmode)
- [TriangleFillMode](StandardMaterial.md#trianglefillmode)
- [TriangleStripDrawMode](StandardMaterial.md#trianglestripdrawmode)
- [WireFrameFillMode](StandardMaterial.md#wireframefillmode)

### Accessors

- [\_disableAlphaBlending](StandardMaterial.md#_disablealphablending)
- [alpha](StandardMaterial.md#alpha)
- [alphaMode](StandardMaterial.md#alphamode)
- [backFaceCulling](StandardMaterial.md#backfaceculling)
- [cameraColorCurves](StandardMaterial.md#cameracolorcurves)
- [cameraColorCurvesEnabled](StandardMaterial.md#cameracolorcurvesenabled)
- [cameraColorGradingEnabled](StandardMaterial.md#cameracolorgradingenabled)
- [cameraColorGradingTexture](StandardMaterial.md#cameracolorgradingtexture)
- [cameraContrast](StandardMaterial.md#cameracontrast)
- [cameraExposure](StandardMaterial.md#cameraexposure)
- [cameraToneMappingEnabled](StandardMaterial.md#cameratonemappingenabled)
- [canRenderToMRT](StandardMaterial.md#canrendertomrt)
- [cullBackFaces](StandardMaterial.md#cullbackfaces)
- [fillMode](StandardMaterial.md#fillmode)
- [fogEnabled](StandardMaterial.md#fogenabled)
- [hasRenderTargetTextures](StandardMaterial.md#hasrendertargettextures)
- [imageProcessingConfiguration](StandardMaterial.md#imageprocessingconfiguration)
- [isFrozen](StandardMaterial.md#isfrozen)
- [isPrePassCapable](StandardMaterial.md#isprepasscapable)
- [needDepthPrePass](StandardMaterial.md#needdepthprepass)
- [onBind](StandardMaterial.md#onbind)
- [onBindObservable](StandardMaterial.md#onbindobservable)
- [onDispose](StandardMaterial.md#ondispose)
- [onEffectCreatedObservable](StandardMaterial.md#oneffectcreatedobservable)
- [onUnBindObservable](StandardMaterial.md#onunbindobservable)
- [pointsCloud](StandardMaterial.md#pointscloud)
- [transparencyMode](StandardMaterial.md#transparencymode)
- [useLogarithmicDepth](StandardMaterial.md#uselogarithmicdepth)
- [wireframe](StandardMaterial.md#wireframe)
- [AmbientTextureEnabled](StandardMaterial.md#ambienttextureenabled)
- [BumpTextureEnabled](StandardMaterial.md#bumptextureenabled)
- [ColorGradingTextureEnabled](StandardMaterial.md#colorgradingtextureenabled)
- [DetailTextureEnabled](StandardMaterial.md#detailtextureenabled)
- [DiffuseTextureEnabled](StandardMaterial.md#diffusetextureenabled)
- [EmissiveTextureEnabled](StandardMaterial.md#emissivetextureenabled)
- [FresnelEnabled](StandardMaterial.md#fresnelenabled)
- [LightmapTextureEnabled](StandardMaterial.md#lightmaptextureenabled)
- [OpacityTextureEnabled](StandardMaterial.md#opacitytextureenabled)
- [ReflectionTextureEnabled](StandardMaterial.md#reflectiontextureenabled)
- [RefractionTextureEnabled](StandardMaterial.md#refractiontextureenabled)
- [SpecularTextureEnabled](StandardMaterial.md#speculartextureenabled)

### Methods

- [\_afterBind](StandardMaterial.md#_afterbind)
- [\_attachImageProcessingConfiguration](StandardMaterial.md#_attachimageprocessingconfiguration)
- [\_hasAlphaChannel](StandardMaterial.md#_hasalphachannel)
- [\_isReadyForSubMesh](StandardMaterial.md#_isreadyforsubmesh)
- [\_markAllSubMeshesAsAllDirty](StandardMaterial.md#_markallsubmeshesasalldirty)
- [\_markAllSubMeshesAsAttributesDirty](StandardMaterial.md#_markallsubmeshesasattributesdirty)
- [\_markAllSubMeshesAsDirty](StandardMaterial.md#_markallsubmeshesasdirty)
- [\_markAllSubMeshesAsFresnelAndMiscDirty](StandardMaterial.md#_markallsubmeshesasfresnelandmiscdirty)
- [\_markAllSubMeshesAsFresnelDirty](StandardMaterial.md#_markallsubmeshesasfresneldirty)
- [\_markAllSubMeshesAsImageProcessingDirty](StandardMaterial.md#_markallsubmeshesasimageprocessingdirty)
- [\_markAllSubMeshesAsLightsDirty](StandardMaterial.md#_markallsubmeshesaslightsdirty)
- [\_markAllSubMeshesAsMiscDirty](StandardMaterial.md#_markallsubmeshesasmiscdirty)
- [\_markAllSubMeshesAsPrePassDirty](StandardMaterial.md#_markallsubmeshesasprepassdirty)
- [\_markAllSubMeshesAsTexturesAndMiscDirty](StandardMaterial.md#_markallsubmeshesastexturesandmiscdirty)
- [\_markAllSubMeshesAsTexturesDirty](StandardMaterial.md#_markallsubmeshesastexturesdirty)
- [\_markScenePrePassDirty](StandardMaterial.md#_marksceneprepassdirty)
- [\_mustRebind](StandardMaterial.md#_mustrebind)
- [\_shouldTurnAlphaTestOn](StandardMaterial.md#_shouldturnalphateston)
- [\_shouldUseAlphaFromDiffuseTexture](StandardMaterial.md#_shouldusealphafromdiffusetexture)
- [bind](StandardMaterial.md#bind)
- [bindEyePosition](StandardMaterial.md#bindeyeposition)
- [bindForSubMesh](StandardMaterial.md#bindforsubmesh)
- [bindOnlyNormalMatrix](StandardMaterial.md#bindonlynormalmatrix)
- [bindOnlyWorldMatrix](StandardMaterial.md#bindonlyworldmatrix)
- [bindView](StandardMaterial.md#bindview)
- [bindViewProjection](StandardMaterial.md#bindviewprojection)
- [buildUniformLayout](StandardMaterial.md#builduniformlayout)
- [clone](StandardMaterial.md#clone)
- [dispose](StandardMaterial.md#dispose)
- [forceCompilation](StandardMaterial.md#forcecompilation)
- [forceCompilationAsync](StandardMaterial.md#forcecompilationasync)
- [freeze](StandardMaterial.md#freeze)
- [getActiveTextures](StandardMaterial.md#getactivetextures)
- [getAlphaTestTexture](StandardMaterial.md#getalphatesttexture)
- [getAnimatables](StandardMaterial.md#getanimatables)
- [getBindedMeshes](StandardMaterial.md#getbindedmeshes)
- [getClassName](StandardMaterial.md#getclassname)
- [getEffect](StandardMaterial.md#geteffect)
- [getScene](StandardMaterial.md#getscene)
- [hasTexture](StandardMaterial.md#hastexture)
- [isReady](StandardMaterial.md#isready)
- [isReadyForSubMesh](StandardMaterial.md#isreadyforsubmesh)
- [markAsDirty](StandardMaterial.md#markasdirty)
- [markDirty](StandardMaterial.md#markdirty)
- [needAlphaBlending](StandardMaterial.md#needalphablending)
- [needAlphaBlendingForMesh](StandardMaterial.md#needalphablendingformesh)
- [needAlphaTesting](StandardMaterial.md#needalphatesting)
- [resetDrawCache](StandardMaterial.md#resetdrawcache)
- [serialize](StandardMaterial.md#serialize)
- [setPrePassRenderer](StandardMaterial.md#setprepassrenderer)
- [toString](StandardMaterial.md#tostring)
- [unbind](StandardMaterial.md#unbind)
- [unfreeze](StandardMaterial.md#unfreeze)
- [Parse](StandardMaterial.md#parse)

## Constructors

### constructor

• **new StandardMaterial**(`name`, `scene?`)

Instantiates a new standard material.
This is the default material used in Babylon. It is the best trade off between quality
and performances.

**`See`**

https://doc.babylonjs.com/babylon101/materials

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Define the name of the material in the scene |
| `scene?` | [`Scene`](Scene.md) | Define the scene the material belong to |

#### Overrides

PushMaterial.constructor

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:761

## Properties

### \_activeEffect

• `Protected` **\_activeEffect**: [`Effect`](Effect.md)

#### Inherited from

PushMaterial.\_activeEffect

#### Defined in

packages/dev/core/src/Materials/pushMaterial.ts:14

___

### \_alpha

• `Protected` **\_alpha**: `number` = `1.0`

The alpha value of the material

#### Inherited from

PushMaterial.\_alpha

#### Defined in

packages/dev/core/src/Materials/material.ts:292

___

### \_ambientTexture

• `Private` **\_ambientTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) = `null`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:240

___

### \_backFaceCulling

• `Protected` **\_backFaceCulling**: `boolean` = `true`

Specifies if back face culling is enabled

#### Inherited from

PushMaterial.\_backFaceCulling

#### Defined in

packages/dev/core/src/Materials/material.ts:328

___

### \_bumpTexture

• `Private` **\_bumpTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) = `null`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:284

___

### \_cacheHasRenderTargetTextures

• `Protected` **\_cacheHasRenderTargetTextures**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:751

___

### \_cullBackFaces

• `Protected` **\_cullBackFaces**: `boolean` = `true`

Specifies if back or front faces should be culled (when culling is enabled)

#### Inherited from

PushMaterial.\_cullBackFaces

#### Defined in

packages/dev/core/src/Materials/material.ts:352

___

### \_diffuseFresnelParameters

• `Private` **\_diffuseFresnelParameters**: [`FresnelParameters`](FresnelParameters.md)

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:470

___

### \_diffuseTexture

• `Private` **\_diffuseTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) = `null`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:232

___

### \_disableLighting

• `Private` **\_disableLighting**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:390

___

### \_drawWrapper

• `Protected` **\_drawWrapper**: `DrawWrapper`

#### Inherited from

PushMaterial.\_drawWrapper

#### Defined in

packages/dev/core/src/Materials/material.ts:705

___

### \_emissiveFresnelParameters

• `Private` **\_emissiveFresnelParameters**: [`FresnelParameters`](FresnelParameters.md)

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:506

___

### \_emissiveTexture

• `Private` **\_emissiveTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) = `null`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:267

___

### \_eventInfo

• `Protected` **\_eventInfo**: `MaterialPluginDisposed` & `MaterialPluginHasTexture` & `MaterialPluginIsReadyForSubMesh` & `MaterialPluginGetDefineNames` & `MaterialPluginPrepareEffect` & `MaterialPluginPrepareDefines` & `MaterialPluginPrepareUniformBuffer` & `MaterialPluginBindForSubMesh` & `MaterialPluginGetAnimatables` & `MaterialPluginGetActiveTextures` & `MaterialPluginFillRenderTargetTextures` & `MaterialPluginHasRenderTargetTextures` & `MaterialPluginHardBindForSubMesh`

#### Inherited from

PushMaterial.\_eventInfo

#### Defined in

packages/dev/core/src/Materials/material.ts:770

___

### \_forceAlphaTest

• `Protected` **\_forceAlphaTest**: `boolean` = `false`

Enforces alpha test in opaque or blend mode in order to improve the performances of some situations.

#### Inherited from

PushMaterial.\_forceAlphaTest

#### Defined in

packages/dev/core/src/Materials/material.ts:954

___

### \_globalAmbientColor

• `Protected` **\_globalAmbientColor**: [`Color3`](Color3.md)

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:749

___

### \_imageProcessingConfiguration

• `Protected` **\_imageProcessingConfiguration**: [`ImageProcessingConfiguration`](ImageProcessingConfiguration.md)

Default configuration related to image processing available in the standard Material.

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:566

___

### \_imageProcessingObserver

• `Private` **\_imageProcessingObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`ImageProcessingConfiguration`](ImageProcessingConfiguration.md)

Keep track of the image processing observer to allow dispose and replace.

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:590

___

### \_invertNormalMapX

• `Private` **\_invertNormalMapX**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:540

___

### \_invertNormalMapY

• `Private` **\_invertNormalMapY**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:548

___

### \_lightmapTexture

• `Private` **\_lightmapTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) = `null`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:294

___

### \_linkEmissiveWithDiffuse

• `Private` **\_linkEmissiveWithDiffuse**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:363

___

### \_maxSimultaneousLights

• `Private` **\_maxSimultaneousLights**: `number` = `4`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:532

___

### \_needToBindSceneUbo

• `Protected` **\_needToBindSceneUbo**: `boolean`

#### Inherited from

PushMaterial.\_needToBindSceneUbo

#### Defined in

packages/dev/core/src/Materials/material.ts:727

___

### \_normalMatrix

• `Protected` **\_normalMatrix**: [`Matrix`](Matrix.md)

#### Inherited from

PushMaterial.\_normalMatrix

#### Defined in

packages/dev/core/src/Materials/pushMaterial.ts:16

___

### \_onEffectCreatedObservable

• `Protected` **\_onEffectCreatedObservable**: [`Nullable`](../modules.md#nullable)[`Observable`](Observable.md){ `effect`: [`Effect`](Effect.md) ; `subMesh`: [`Nullable`](../modules.md#nullable)[`SubMesh`](SubMesh.md)  }

#### Inherited from

PushMaterial.\_onEffectCreatedObservable

#### Defined in

packages/dev/core/src/Materials/material.ts:477

___

### \_opacityFresnelParameters

• `Private` **\_opacityFresnelParameters**: [`FresnelParameters`](FresnelParameters.md)

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:479

___

### \_opacityTexture

• `Private` **\_opacityTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) = `null`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:248

___

### \_reflectionFresnelParameters

• `Private` **\_reflectionFresnelParameters**: [`FresnelParameters`](FresnelParameters.md)

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:488

___

### \_reflectionTexture

• `Private` **\_reflectionTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) = `null`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:258

___

### \_refractionFresnelParameters

• `Private` **\_refractionFresnelParameters**: [`FresnelParameters`](FresnelParameters.md)

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:497

___

### \_refractionTexture

• `Private` **\_refractionTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) = `null`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:304

___

### \_renderTargets

• `Protected` **\_renderTargets**: [`SmartArray`](SmartArray.md)[`RenderTargetTexture`](RenderTargetTexture.md)

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:747

___

### \_roughness

• `Private` **\_roughness**: `number` = `0`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:432

___

### \_specularTexture

• `Private` **\_specularTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) = `null`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:276

___

### \_transparencyMode

• `Protected` **\_transparencyMode**: [`Nullable`](../modules.md#nullable)`number` = `null`

The transparency mode of the material.

#### Inherited from

PushMaterial.\_transparencyMode

#### Defined in

packages/dev/core/src/Materials/material.ts:959

___

### \_twoSidedLighting

• `Private` **\_twoSidedLighting**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:556

___

### \_useAlphaFromDiffuseTexture

• `Private` **\_useAlphaFromDiffuseTexture**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:347

___

### \_useEmissiveAsIllumination

• `Private` **\_useEmissiveAsIllumination**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:355

___

### \_useGlossinessFromSpecularMapAlpha

• `Private` **\_useGlossinessFromSpecularMapAlpha**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:524

___

### \_useLightmapAsShadowmap

• `Private` **\_useLightmapAsShadowmap**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:461

___

### \_useLogarithmicDepth

• `Protected` **\_useLogarithmicDepth**: `boolean`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:750

___

### \_useObjectSpaceNormalMap

• `Private` **\_useObjectSpaceNormalMap**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:399

___

### \_useParallax

• `Private` **\_useParallax**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:407

___

### \_useParallaxOcclusion

• `Private` **\_useParallaxOcclusion**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:416

___

### \_useReflectionFresnelFromSpecular

• `Private` **\_useReflectionFresnelFromSpecular**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:515

___

### \_useReflectionOverAlpha

• `Private` **\_useReflectionOverAlpha**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:381

___

### \_useSpecularOverAlpha

• `Private` **\_useSpecularOverAlpha**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:372

___

### \_worldViewProjectionMatrix

• `Protected` **\_worldViewProjectionMatrix**: [`Matrix`](Matrix.md)

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:748

___

### allowShaderHotSwapping

• **allowShaderHotSwapping**: `boolean` = `true`

Gets or sets a boolean indicating that the material is allowed (if supported) to do shader hot swapping.
This means that the material can keep using a previous shader while a new one is being compiled.
This is mostly used when shader parallel compilation is supported (true by default)

#### Inherited from

PushMaterial.allowShaderHotSwapping

#### Defined in

packages/dev/core/src/Materials/material.ts:227

___

### alphaCutOff

• **alphaCutOff**: `number` = `0.4`

Defines the alpha limits in alpha test mode.

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:458

___

### ambientColor

• **ambientColor**: [`Color3`](Color3.md)

The color of the material lit by the environmental background lighting.

**`See`**

https://doc.babylonjs.com/babylon101/materials#ambient-color-example

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:317

___

### ambientTexture

• **ambientTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

AKA Occlusion Texture in other nomenclature, it helps adding baked shadows into your material.

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:245

___

### animations

• **animations**: [`Nullable`](../modules.md#nullable)[`Animation`](Animation.md)[] = `null`

Stores the animations for the material

#### Inherited from

PushMaterial.animations

#### Defined in

packages/dev/core/src/Materials/material.ts:415

___

### bumpTexture

• **bumpTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Bump mapping is a technique to simulate bump and dents on a rendered surface.
These are made by creating a normal map from an image. The means to do this can be found on the web, a search for 'normal map generator' will bring up free and paid for methods of doing this.

**`See`**

https://doc.babylonjs.com/how_to/more_materials#bump-map

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:291

___

### checkReadyOnEveryCall

• **checkReadyOnEveryCall**: `boolean` = `false`

Specifies if the ready state should be checked on each call

#### Inherited from

PushMaterial.checkReadyOnEveryCall

#### Defined in

packages/dev/core/src/Materials/material.ts:265

___

### checkReadyOnlyOnce

• **checkReadyOnlyOnce**: `boolean` = `false`

Specifies if the ready state should be checked once

#### Inherited from

PushMaterial.checkReadyOnlyOnce

#### Defined in

packages/dev/core/src/Materials/material.ts:271

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

PushMaterial.customShaderNameResolve

#### Defined in

packages/dev/core/src/Materials/material.ts:207

___

### depthFunction

• **depthFunction**: `number` = `0`

Specifies the depth function that should be used. 0 means the default engine function

#### Inherited from

PushMaterial.depthFunction

#### Defined in

packages/dev/core/src/Materials/material.ts:584

___

### detailMap

• `Readonly` **detailMap**: [`DetailMapConfiguration`](DetailMapConfiguration.md)

Defines the detail map parameters for the material.

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:745

___

### diffuseColor

• **diffuseColor**: [`Color3`](Color3.md)

The basic color of the material as viewed under a light.

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:323

___

### diffuseFresnelParameters

• **diffuseFresnelParameters**: [`FresnelParameters`](FresnelParameters.md)

Define the diffuse fresnel parameters of the material.

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_fresnelparameters

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:476

___

### diffuseTexture

• **diffuseTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

The basic texture of the material as viewed under a light.

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:237

___

### disableColorWrite

• **disableColorWrite**: `boolean` = `false`

Specifies if color writing should be disabled

#### Inherited from

PushMaterial.disableColorWrite

#### Defined in

packages/dev/core/src/Materials/material.ts:572

___

### disableDepthWrite

• **disableDepthWrite**: `boolean` = `false`

Specifies if depth writing should be disabled

#### Inherited from

PushMaterial.disableDepthWrite

#### Defined in

packages/dev/core/src/Materials/material.ts:566

___

### disableLighting

• **disableLighting**: `boolean`

Does lights from the scene impacts this material.
It can be a nice trick for performance to disable lighting on a fully emissive material.

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:396

___

### doNotSerialize

• **doNotSerialize**: `boolean` = `false`

Specifies if the material should be serialized

#### Inherited from

PushMaterial.doNotSerialize

#### Defined in

packages/dev/core/src/Materials/material.ts:405

___

### emissiveColor

• **emissiveColor**: [`Color3`](Color3.md)

Define the color of the material as if self lit.
This will be mixed in the final result even in the absence of light.

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:336

___

### emissiveFresnelParameters

• **emissiveFresnelParameters**: [`FresnelParameters`](FresnelParameters.md)

Define the emissive fresnel parameters of the material.

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_fresnelparameters

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:512

___

### emissiveTexture

• **emissiveTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Define texture of the material as if self lit.
This will be mixed in the final result even in the absence of light.

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:273

___

### forceDepthWrite

• **forceDepthWrite**: `boolean` = `false`

Specifies if depth writing should be forced

#### Inherited from

PushMaterial.forceDepthWrite

#### Defined in

packages/dev/core/src/Materials/material.ts:578

___

### getRenderTargetTextures

• **getRenderTargetTextures**: [`Nullable`](../modules.md#nullable)() => [`SmartArray`](SmartArray.md)[`RenderTargetTexture`](RenderTargetTexture.md) = `null`

Callback triggered to get the render target textures

#### Inherited from

PushMaterial.getRenderTargetTextures

#### Defined in

packages/dev/core/src/Materials/material.ts:391

___

### id

• **id**: `string`

The ID of the material

#### Inherited from

PushMaterial.id

#### Defined in

packages/dev/core/src/Materials/material.ts:233

___

### indexOfRefraction

• **indexOfRefraction**: `number` = `0.98`

In case of refraction, define the value of the index of refraction.

**`See`**

https://doc.babylonjs.com/how_to/reflect#how-to-obtain-reflections-and-refractions

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:444

___

### inspectableCustomProperties

• **inspectableCustomProperties**: [`IInspectable`](../interfaces/IInspectable.md)[]

List of inspectable custom properties (used by the Inspector)

**`See`**

https://doc.babylonjs.com/how_to/debug_layer#extensibility

#### Inherited from

PushMaterial.inspectableCustomProperties

#### Defined in

packages/dev/core/src/Materials/material.ts:298

___

### invertNormalMapX

• **invertNormalMapX**: `boolean`

If sets to true, x component of normal map value will invert (x = 1.0 - x).

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:545

___

### invertNormalMapY

• **invertNormalMapY**: `boolean`

If sets to true, y component of normal map value will invert (y = 1.0 - y).

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:553

___

### invertRefractionY

• **invertRefractionY**: `boolean` = `true`

Invert the refraction texture alongside the y axis.
It can be useful with procedural textures or probe for instance.

**`See`**

https://doc.babylonjs.com/how_to/reflect#how-to-obtain-reflections-and-refractions

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:452

___

### lightmapTexture

• **lightmapTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Complex lighting can be computationally expensive to compute at runtime.
To save on computation, lightmaps may be used to store calculated lighting in a texture which will be applied to a given mesh.

**`See`**

https://doc.babylonjs.com/babylon101/lights#lightmaps

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:301

___

### linkEmissiveWithDiffuse

• **linkEmissiveWithDiffuse**: `boolean`

If true, some kind of energy conservation will prevent the end result to be more than 1 by reducing
the emissive level when the final color is close to one.

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:369

___

### maxSimultaneousLights

• **maxSimultaneousLights**: `number`

Defines the maximum number of lights that can be used in the material

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:537

___

### metadata

• **metadata**: `any` = `null`

Gets or sets user defined metadata

#### Inherited from

PushMaterial.metadata

#### Defined in

packages/dev/core/src/Materials/material.ts:254

___

### name

• **name**: `string`

The name of the material

#### Inherited from

PushMaterial.name

#### Defined in

packages/dev/core/src/Materials/material.ts:248

___

### onCompiled

• **onCompiled**: [`Nullable`](../modules.md#nullable)(`effect`: [`Effect`](Effect.md)) => `void` = `null`

Callback triggered when the material is compiled

#### Inherited from

PushMaterial.onCompiled

#### Defined in

packages/dev/core/src/Materials/material.ts:381

___

### onDisposeObservable

• **onDisposeObservable**: [`Observable`](Observable.md)[`Material`](Material.md)

An event triggered when the material is disposed

#### Inherited from

PushMaterial.onDisposeObservable

#### Defined in

packages/dev/core/src/Materials/material.ts:420

___

### onError

• **onError**: [`Nullable`](../modules.md#nullable)(`effect`: [`Effect`](Effect.md), `errors`: `string`) => `void` = `null`

Callback triggered when an error occurs

#### Inherited from

PushMaterial.onError

#### Defined in

packages/dev/core/src/Materials/material.ts:386

___

### opacityFresnelParameters

• **opacityFresnelParameters**: [`FresnelParameters`](FresnelParameters.md)

Define the opacity fresnel parameters of the material.

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_fresnelparameters

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:485

___

### opacityTexture

• **opacityTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Define the transparency of the material from a texture.
The final alpha value can be read either from the red channel (if texture.getAlphaFromRGB is false)
or from the luminance or the current texel (if texture.getAlphaFromRGB is true)

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:255

___

### parallaxScaleBias

• **parallaxScaleBias**: `number` = `0.05`

Apply a scaling factor that determine which "depth" the height map should reprensent. A value between 0.05 and 0.1 is reasonnable in Parallax, you can reach 0.2 using Parallax Occlusion.

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:429

___

### pluginManager

• `Optional` **pluginManager**: [`MaterialPluginManager`](MaterialPluginManager.md)

Plugin manager for this material

#### Inherited from

PushMaterial.pluginManager

#### Defined in

packages/dev/core/src/Materials/materialPluginManager.ts:30

___

### pointSize

• **pointSize**: `number` = `1.0`

Stores the size of points

#### Inherited from

PushMaterial.pointSize

#### Defined in

packages/dev/core/src/Materials/material.ts:620

___

### prePassConfiguration

• `Readonly` **prePassConfiguration**: `PrePassConfiguration`

Defines additional PrePass parameters for the material.

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:624

___

### reflectionFresnelParameters

• **reflectionFresnelParameters**: [`FresnelParameters`](FresnelParameters.md)

Define the reflection fresnel parameters of the material.

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_fresnelparameters

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:494

___

### reflectionTexture

• **reflectionTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Define the texture used to display the reflection.

**`See`**

https://doc.babylonjs.com/how_to/reflect#how-to-obtain-reflections-and-refractions

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:264

___

### refractionFresnelParameters

• **refractionFresnelParameters**: [`FresnelParameters`](FresnelParameters.md)

Define the refraction fresnel parameters of the material.

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_fresnelparameters

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:503

___

### refractionTexture

• **refractionTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Define the texture used to display the refraction.

**`See`**

https://doc.babylonjs.com/how_to/reflect#how-to-obtain-reflections-and-refractions

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:310

___

### reservedDataStore

• **reservedDataStore**: `any` = `null`

For internal use only. Please do not use.

#### Inherited from

PushMaterial.reservedDataStore

#### Defined in

packages/dev/core/src/Materials/material.ts:259

___

### roughness

• **roughness**: `number`

Helps to define how blurry the reflections should appears in the material.

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:437

___

### separateCullingPass

• **separateCullingPass**: `boolean` = `false`

Specifies if there should be a separate pass for culling

#### Inherited from

PushMaterial.separateCullingPass

#### Defined in

packages/dev/core/src/Materials/material.ts:590

___

### shadowDepthWrapper

• **shadowDepthWrapper**: [`Nullable`](../modules.md#nullable)[`ShadowDepthWrapper`](ShadowDepthWrapper.md) = `null`

Custom shadow depth material to use for shadow rendering instead of the in-built one

#### Inherited from

PushMaterial.shadowDepthWrapper

#### Defined in

packages/dev/core/src/Materials/material.ts:220

___

### sideOrientation

• **sideOrientation**: `number`

Stores the value for side orientation

#### Inherited from

PushMaterial.sideOrientation

#### Defined in

packages/dev/core/src/Materials/material.ts:376

___

### specularColor

• **specularColor**: [`Color3`](Color3.md)

Define how the color and intensity of the highlight given by the light in the material.

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:329

___

### specularPower

• **specularPower**: `number` = `64`

Defines how sharp are the highlights in the material.
The bigger the value the sharper giving a more glossy feeling to the result.
Reversely, the smaller the value the blurrier giving a more rough feeling to the result.

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:344

___

### specularTexture

• **specularTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Define how the color and intensity of the highlight given by the light in the material.

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:281

___

### state

• **state**: `string` = `""`

The state of the material

#### Inherited from

PushMaterial.state

#### Defined in

packages/dev/core/src/Materials/material.ts:277

___

### stencil

• `Readonly` **stencil**: `MaterialStencilState`

Gives access to the stencil properties of the material

#### Inherited from

PushMaterial.stencil

#### Defined in

packages/dev/core/src/Materials/material.ts:697

___

### twoSidedLighting

• **twoSidedLighting**: `boolean`

If sets to true and backfaceCulling is false, normals will be flipped on the backside.

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:561

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the material

#### Inherited from

PushMaterial.uniqueId

#### Defined in

packages/dev/core/src/Materials/material.ts:239

___

### useAlphaFromDiffuseTexture

• **useAlphaFromDiffuseTexture**: `boolean`

Does the transparency come from the diffuse texture alpha channel.

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:352

___

### useEmissiveAsIllumination

• **useEmissiveAsIllumination**: `boolean`

If true, the emissive value is added into the end result, otherwise it is multiplied in.

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:360

___

### useGlossinessFromSpecularMapAlpha

• **useGlossinessFromSpecularMapAlpha**: `boolean`

Defines if the glossiness/roughness of the material should be read from the specular map alpha channel

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:529

___

### useLightmapAsShadowmap

• **useLightmapAsShadowmap**: `boolean`

In case of light mapping, define whether the map contains light or shadow informations.

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:466

___

### useObjectSpaceNormalMap

• **useObjectSpaceNormalMap**: `boolean`

Allows using an object space normal map (instead of tangent space).

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:404

___

### useParallax

• **useParallax**: `boolean`

Is parallax enabled or not.

**`See`**

https://doc.babylonjs.com/how_to/using_parallax_mapping

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:413

___

### useParallaxOcclusion

• **useParallaxOcclusion**: `boolean`

Is parallax occlusion enabled or not.
If true, the outcome is way more realistic than traditional Parallax but you can expect a performance hit that worthes consideration.

**`See`**

https://doc.babylonjs.com/how_to/using_parallax_mapping

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:423

___

### useReflectionFresnelFromSpecular

• **useReflectionFresnelFromSpecular**: `boolean`

If true automatically deducts the fresnels values from the material specularity.

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_fresnelparameters

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:521

___

### useReflectionOverAlpha

• **useReflectionOverAlpha**: `boolean`

Specifies that the material will keeps the reflection highlights over a transparent surface (only the most luminous ones).
A car glass is a good exemple of that. When the street lights reflects on it you can not see what is behind.

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:387

___

### useSpecularOverAlpha

• **useSpecularOverAlpha**: `boolean`

Specifies that the material will keep the specular highlights over a transparent surface (only the most luminous ones).
A car glass is a good exemple of that. When sun reflects on it you can not see what is behind.

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:378

___

### zOffset

• **zOffset**: `number` = `0`

Stores the z offset Factor value

#### Inherited from

PushMaterial.zOffset

#### Defined in

packages/dev/core/src/Materials/material.ts:626

___

### zOffsetUnits

• **zOffsetUnits**: `number` = `0`

Stores the z offset Units value

#### Inherited from

PushMaterial.zOffsetUnits

#### Defined in

packages/dev/core/src/Materials/material.ts:632

___

### AllDirtyFlag

▪ `Static` `Readonly` **AllDirtyFlag**: ``63``

The all dirty flag value

#### Inherited from

PushMaterial.AllDirtyFlag

#### Defined in

packages/dev/core/src/Materials/material.ts:164

___

### AttributesDirtyFlag

▪ `Static` `Readonly` **AttributesDirtyFlag**: ``8``

The dirty attribute flag value

#### Inherited from

PushMaterial.AttributesDirtyFlag

#### Defined in

packages/dev/core/src/Materials/material.ts:149

___

### ClockWiseSideOrientation

▪ `Static` `Readonly` **ClockWiseSideOrientation**: ``0``

Stores the clock-wise side orientation

#### Inherited from

PushMaterial.ClockWiseSideOrientation

#### Defined in

packages/dev/core/src/Materials/material.ts:124

___

### CounterClockWiseSideOrientation

▪ `Static` `Readonly` **CounterClockWiseSideOrientation**: ``1``

Stores the counter clock-wise side orientation

#### Inherited from

PushMaterial.CounterClockWiseSideOrientation

#### Defined in

packages/dev/core/src/Materials/material.ts:129

___

### FresnelDirtyFlag

▪ `Static` `Readonly` **FresnelDirtyFlag**: ``4``

The dirty fresnel flag value

#### Inherited from

PushMaterial.FresnelDirtyFlag

#### Defined in

packages/dev/core/src/Materials/material.ts:144

___

### LightDirtyFlag

▪ `Static` `Readonly` **LightDirtyFlag**: ``2``

The dirty light flag value

#### Inherited from

PushMaterial.LightDirtyFlag

#### Defined in

packages/dev/core/src/Materials/material.ts:139

___

### LineListDrawMode

▪ `Static` `Readonly` **LineListDrawMode**: ``4``

Returns the line list draw mode

#### Inherited from

PushMaterial.LineListDrawMode

#### Defined in

packages/dev/core/src/Materials/material.ts:103

___

### LineLoopDrawMode

▪ `Static` `Readonly` **LineLoopDrawMode**: ``5``

Returns the line loop draw mode

#### Inherited from

PushMaterial.LineLoopDrawMode

#### Defined in

packages/dev/core/src/Materials/material.ts:107

___

### LineStripDrawMode

▪ `Static` `Readonly` **LineStripDrawMode**: ``6``

Returns the line strip draw mode

#### Inherited from

PushMaterial.LineStripDrawMode

#### Defined in

packages/dev/core/src/Materials/material.ts:111

___

### MATERIAL\_ALPHABLEND

▪ `Static` `Readonly` **MATERIAL\_ALPHABLEND**: ``2``

MaterialTransparencyMode: Pixels are blended (according to the alpha mode) with the already drawn pixels in the current frame buffer.

#### Inherited from

PushMaterial.MATERIAL\_ALPHABLEND

#### Defined in

packages/dev/core/src/Materials/material.ts:179

___

### MATERIAL\_ALPHATEST

▪ `Static` `Readonly` **MATERIAL\_ALPHATEST**: ``1``

MaterialTransparencyMode: Alpha Test mode, pixel are discarded below a certain threshold defined by the alpha cutoff value.

#### Inherited from

PushMaterial.MATERIAL\_ALPHATEST

#### Defined in

packages/dev/core/src/Materials/material.ts:174

___

### MATERIAL\_ALPHATESTANDBLEND

▪ `Static` `Readonly` **MATERIAL\_ALPHATESTANDBLEND**: ``3``

MaterialTransparencyMode: Pixels are blended (according to the alpha mode) with the already drawn pixels in the current frame buffer.
They are also discarded below the alpha cutoff threshold to improve performances.

#### Inherited from

PushMaterial.MATERIAL\_ALPHATESTANDBLEND

#### Defined in

packages/dev/core/src/Materials/material.ts:185

___

### MATERIAL\_NORMALBLENDMETHOD\_RNM

▪ `Static` `Readonly` **MATERIAL\_NORMALBLENDMETHOD\_RNM**: ``1``

The Reoriented Normal Mapping method is used to blend normals.
Details of the algorithm can be found here: https://blog.selfshadow.com/publications/blending-in-detail/

#### Inherited from

PushMaterial.MATERIAL\_NORMALBLENDMETHOD\_RNM

#### Defined in

packages/dev/core/src/Materials/material.ts:197

___

### MATERIAL\_NORMALBLENDMETHOD\_WHITEOUT

▪ `Static` `Readonly` **MATERIAL\_NORMALBLENDMETHOD\_WHITEOUT**: ``0``

The Whiteout method is used to blend normals.
Details of the algorithm can be found here: https://blog.selfshadow.com/publications/blending-in-detail/

#### Inherited from

PushMaterial.MATERIAL\_NORMALBLENDMETHOD\_WHITEOUT

#### Defined in

packages/dev/core/src/Materials/material.ts:191

___

### MATERIAL\_OPAQUE

▪ `Static` `Readonly` **MATERIAL\_OPAQUE**: ``0``

MaterialTransparencyMode: No transparency mode, Alpha channel is not use.

#### Inherited from

PushMaterial.MATERIAL\_OPAQUE

#### Defined in

packages/dev/core/src/Materials/material.ts:169

___

### MiscDirtyFlag

▪ `Static` `Readonly` **MiscDirtyFlag**: ``16``

The dirty misc flag value

#### Inherited from

PushMaterial.MiscDirtyFlag

#### Defined in

packages/dev/core/src/Materials/material.ts:154

___

### OnEventObservable

▪ `Static` **OnEventObservable**: [`Observable`](Observable.md)[`Material`](Material.md)

Event observable which raises global events common to all materials (like MaterialPluginEvent.Created)

#### Inherited from

PushMaterial.OnEventObservable

#### Defined in

packages/dev/core/src/Materials/material.ts:202

___

### PointFillMode

▪ `Static` `Readonly` **PointFillMode**: ``2``

Returns the point fill mode

#### Inherited from

PushMaterial.PointFillMode

#### Defined in

packages/dev/core/src/Materials/material.ts:95

___

### PointListDrawMode

▪ `Static` `Readonly` **PointListDrawMode**: ``3``

Returns the point list draw mode

#### Inherited from

PushMaterial.PointListDrawMode

#### Defined in

packages/dev/core/src/Materials/material.ts:99

___

### PrePassDirtyFlag

▪ `Static` `Readonly` **PrePassDirtyFlag**: ``32``

The dirty prepass flag value

#### Inherited from

PushMaterial.PrePassDirtyFlag

#### Defined in

packages/dev/core/src/Materials/material.ts:159

___

### TextureDirtyFlag

▪ `Static` `Readonly` **TextureDirtyFlag**: ``1``

The dirty texture flag value

#### Inherited from

PushMaterial.TextureDirtyFlag

#### Defined in

packages/dev/core/src/Materials/material.ts:134

___

### TriangleFanDrawMode

▪ `Static` `Readonly` **TriangleFanDrawMode**: ``8``

Returns the triangle fan draw mode

#### Inherited from

PushMaterial.TriangleFanDrawMode

#### Defined in

packages/dev/core/src/Materials/material.ts:119

___

### TriangleFillMode

▪ `Static` `Readonly` **TriangleFillMode**: ``0``

Returns the triangle fill mode

#### Inherited from

PushMaterial.TriangleFillMode

#### Defined in

packages/dev/core/src/Materials/material.ts:87

___

### TriangleStripDrawMode

▪ `Static` `Readonly` **TriangleStripDrawMode**: ``7``

Returns the triangle strip draw mode

#### Inherited from

PushMaterial.TriangleStripDrawMode

#### Defined in

packages/dev/core/src/Materials/material.ts:115

___

### WireFrameFillMode

▪ `Static` `Readonly` **WireFrameFillMode**: ``1``

Returns the wireframe mode

#### Inherited from

PushMaterial.WireFrameFillMode

#### Defined in

packages/dev/core/src/Materials/material.ts:91

## Accessors

### \_disableAlphaBlending

• `Protected` `get` **_disableAlphaBlending**(): `boolean`

Returns true if alpha blending should be disabled.

#### Returns

`boolean`

#### Inherited from

PushMaterial.\_disableAlphaBlending

#### Defined in

packages/dev/core/src/Materials/material.ts:995

___

### alpha

• `get` **alpha**(): `number`

Gets the alpha value of the material

#### Returns

`number`

#### Inherited from

PushMaterial.alpha

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

PushMaterial.alpha

#### Defined in

packages/dev/core/src/Materials/material.ts:303

___

### alphaMode

• `get` **alphaMode**(): `number`

Gets the value of the alpha mode

#### Returns

`number`

#### Inherited from

PushMaterial.alphaMode

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

PushMaterial.alphaMode

#### Defined in

packages/dev/core/src/Materials/material.ts:514

___

### backFaceCulling

• `get` **backFaceCulling**(): `boolean`

Gets the culling state

#### Returns

`boolean`

#### Inherited from

PushMaterial.backFaceCulling

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

PushMaterial.backFaceCulling

#### Defined in

packages/dev/core/src/Materials/material.ts:333

___

### cameraColorCurves

• `get` **cameraColorCurves**(): [`Nullable`](../modules.md#nullable)[`ColorCurves`](ColorCurves.md)

The color grading curves provide additional color adjustmnent that is applied after any color grading transform (3D LUT).
They allow basic adjustment of saturation and small exposure adjustments, along with color filter tinting to provide white balance adjustment or more stylistic effects.
These are similar to controls found in many professional imaging or colorist software. The global controls are applied to the entire image. For advanced tuning, extra controls are provided to adjust the shadow, midtone and highlight areas of the image;
corresponding to low luminance, medium luminance, and high luminance areas respectively.

#### Returns

[`Nullable`](../modules.md#nullable)[`ColorCurves`](ColorCurves.md)

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:722

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

packages/dev/core/src/Materials/standardMaterial.ts:731

___

### cameraColorCurvesEnabled

• `get` **cameraColorCurvesEnabled**(): `boolean`

Gets whether the color curves effect is enabled.

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:636

• `set` **cameraColorCurvesEnabled**(`value`): `void`

Sets whether the color curves effect is enabled.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:642

___

### cameraColorGradingEnabled

• `get` **cameraColorGradingEnabled**(): `boolean`

Gets whether the color grading effect is enabled.

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:649

• `set` **cameraColorGradingEnabled**(`value`): `void`

Gets whether the color grading effect is enabled.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:655

___

### cameraColorGradingTexture

• `get` **cameraColorGradingTexture**(): [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Gets the Color Grading 2D Lookup Texture.

#### Returns

[`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:706

• `set` **cameraColorGradingTexture**(`value`): `void`

Sets the Color Grading 2D Lookup Texture.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:712

___

### cameraContrast

• `get` **cameraContrast**(): `number`

Gets The camera contrast used on this material.

#### Returns

`number`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:692

• `set` **cameraContrast**(`value`): `void`

Sets The camera contrast used on this material.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:699

___

### cameraExposure

• `get` **cameraExposure**(): `number`

The camera exposure used on this material.
This property is here and not in the camera to allow controlling exposure without full screen post process.
This corresponds to a photographic exposure.

#### Returns

`number`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:677

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

packages/dev/core/src/Materials/standardMaterial.ts:685

___

### cameraToneMappingEnabled

• `get` **cameraToneMappingEnabled**(): `boolean`

Gets whether tonemapping is enabled or not.

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:662

• `set` **cameraToneMappingEnabled**(`value`): `void`

Sets whether tonemapping is enabled or not

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:668

___

### canRenderToMRT

• `get` **canRenderToMRT**(): `boolean`

Can this material render to several textures at once

#### Returns

`boolean`

#### Overrides

PushMaterial.canRenderToMRT

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:738

___

### cullBackFaces

• `get` **cullBackFaces**(): `boolean`

Gets the type of faces that should be culled

#### Returns

`boolean`

#### Inherited from

PushMaterial.cullBackFaces

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

PushMaterial.cullBackFaces

#### Defined in

packages/dev/core/src/Materials/material.ts:357

___

### fillMode

• `get` **fillMode**(): `number`

Gets the material fill mode

#### Returns

`number`

#### Inherited from

PushMaterial.fillMode

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

PushMaterial.fillMode

#### Defined in

packages/dev/core/src/Materials/material.ts:685

___

### fogEnabled

• `get` **fogEnabled**(): `boolean`

Gets the value of the fog enabled state

#### Returns

`boolean`

#### Inherited from

PushMaterial.fogEnabled

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

PushMaterial.fogEnabled

#### Defined in

packages/dev/core/src/Materials/material.ts:601

___

### hasRenderTargetTextures

• `get` **hasRenderTargetTextures**(): `boolean`

Gets a boolean indicating that current material needs to register RTT

#### Returns

`boolean`

#### Overrides

PushMaterial.hasRenderTargetTextures

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:791

___

### imageProcessingConfiguration

• `get` **imageProcessingConfiguration**(): [`ImageProcessingConfiguration`](ImageProcessingConfiguration.md)

Gets the image processing configuration used either in this material.

#### Returns

[`ImageProcessingConfiguration`](ImageProcessingConfiguration.md)

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:571

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

packages/dev/core/src/Materials/standardMaterial.ts:580

___

### isFrozen

• `get` **isFrozen**(): `boolean`

Specifies if updates for the material been locked

#### Returns

`boolean`

#### Inherited from

PushMaterial.isFrozen

#### Defined in

packages/dev/core/src/Materials/material.ts:883

___

### isPrePassCapable

• `get` **isPrePassCapable**(): `boolean`

Can this material render to prepass

#### Returns

`boolean`

#### Overrides

PushMaterial.isPrePassCapable

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:629

___

### needDepthPrePass

• `get` **needDepthPrePass**(): `boolean`

Gets the depth pre-pass value

#### Returns

`boolean`

#### Inherited from

PushMaterial.needDepthPrePass

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

PushMaterial.needDepthPrePass

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

PushMaterial.onBind

#### Defined in

packages/dev/core/src/Materials/material.ts:459

___

### onBindObservable

• `get` **onBindObservable**(): [`Observable`](Observable.md)[`AbstractMesh`](AbstractMesh.md)

An event triggered when the material is bound

#### Returns

[`Observable`](Observable.md)[`AbstractMesh`](AbstractMesh.md)

#### Inherited from

PushMaterial.onBindObservable

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

PushMaterial.onDispose

#### Defined in

packages/dev/core/src/Materials/material.ts:431

___

### onEffectCreatedObservable

• `get` **onEffectCreatedObservable**(): [`Observable`](Observable.md){ `effect`: [`Effect`](Effect.md) ; `subMesh`: [`Nullable`](../modules.md#nullable)[`SubMesh`](SubMesh.md)  }

An event triggered when the effect is (re)created

#### Returns

[`Observable`](Observable.md){ `effect`: [`Effect`](Effect.md) ; `subMesh`: [`Nullable`](../modules.md#nullable)[`SubMesh`](SubMesh.md)  }

#### Inherited from

PushMaterial.onEffectCreatedObservable

#### Defined in

packages/dev/core/src/Materials/material.ts:482

___

### onUnBindObservable

• `get` **onUnBindObservable**(): [`Observable`](Observable.md)[`Material`](Material.md)

An event triggered when the material is unbound

#### Returns

[`Observable`](Observable.md)[`Material`](Material.md)

#### Inherited from

PushMaterial.onUnBindObservable

#### Defined in

packages/dev/core/src/Materials/material.ts:469

___

### pointsCloud

• `get` **pointsCloud**(): `boolean`

Gets the value specifying if point clouds are enabled

#### Returns

`boolean`

#### Inherited from

PushMaterial.pointsCloud

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

PushMaterial.pointsCloud

#### Defined in

packages/dev/core/src/Materials/material.ts:670

___

### transparencyMode

• `get` **transparencyMode**(): [`Nullable`](../modules.md#nullable)`number`

Gets the current transparency mode.

#### Returns

[`Nullable`](../modules.md#nullable)`number`

#### Inherited from

PushMaterial.transparencyMode

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

PushMaterial.transparencyMode

#### Defined in

packages/dev/core/src/Materials/material.ts:980

___

### useLogarithmicDepth

• `get` **useLogarithmicDepth**(): `boolean`

In case the depth buffer does not allow enough depth precision for your scene (might be the case in large scenes)
You can try switching to logarithmic depth.

**`See`**

https://doc.babylonjs.com/how_to/using_logarithmic_depth_buffer

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:817

• `set` **useLogarithmicDepth**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:822

___

### wireframe

• `get` **wireframe**(): `boolean`

#### Returns

`boolean`

#### Inherited from

PushMaterial.wireframe

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

PushMaterial.wireframe

#### Defined in

packages/dev/core/src/Materials/material.ts:649

___

### AmbientTextureEnabled

• `Static` `get` **AmbientTextureEnabled**(): `boolean`

Are ambient textures enabled in the application.

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:2016

• `Static` `set` **AmbientTextureEnabled**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:2019

___

### BumpTextureEnabled

• `Static` `get` **BumpTextureEnabled**(): `boolean`

Are bump textures enabled in the application.

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:2066

• `Static` `set` **BumpTextureEnabled**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:2069

___

### ColorGradingTextureEnabled

• `Static` `get` **ColorGradingTextureEnabled**(): `boolean`

Are color grading textures enabled in the application.

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:2096

• `Static` `set` **ColorGradingTextureEnabled**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:2099

___

### DetailTextureEnabled

• `Static` `get` **DetailTextureEnabled**(): `boolean`

Are detail textures enabled in the application.

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:2006

• `Static` `set` **DetailTextureEnabled**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:2009

___

### DiffuseTextureEnabled

• `Static` `get` **DiffuseTextureEnabled**(): `boolean`

Are diffuse textures enabled in the application.

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:1996

• `Static` `set` **DiffuseTextureEnabled**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:1999

___

### EmissiveTextureEnabled

• `Static` `get` **EmissiveTextureEnabled**(): `boolean`

Are emissive textures enabled in the application.

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:2046

• `Static` `set` **EmissiveTextureEnabled**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:2049

___

### FresnelEnabled

• `Static` `get` **FresnelEnabled**(): `boolean`

Are fresnels enabled in the application.

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:2106

• `Static` `set` **FresnelEnabled**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:2109

___

### LightmapTextureEnabled

• `Static` `get` **LightmapTextureEnabled**(): `boolean`

Are lightmap textures enabled in the application.

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:2076

• `Static` `set` **LightmapTextureEnabled**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:2079

___

### OpacityTextureEnabled

• `Static` `get` **OpacityTextureEnabled**(): `boolean`

Are opacity textures enabled in the application.

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:2026

• `Static` `set` **OpacityTextureEnabled**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:2029

___

### ReflectionTextureEnabled

• `Static` `get` **ReflectionTextureEnabled**(): `boolean`

Are reflection textures enabled in the application.

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:2036

• `Static` `set` **ReflectionTextureEnabled**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:2039

___

### RefractionTextureEnabled

• `Static` `get` **RefractionTextureEnabled**(): `boolean`

Are refraction textures enabled in the application.

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:2086

• `Static` `set` **RefractionTextureEnabled**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:2089

___

### SpecularTextureEnabled

• `Static` `get` **SpecularTextureEnabled**(): `boolean`

Are specular textures enabled in the application.

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:2056

• `Static` `set` **SpecularTextureEnabled**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:2059

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

PushMaterial.\_afterBind

#### Defined in

packages/dev/core/src/Materials/pushMaterial.ts:80

___

### \_attachImageProcessingConfiguration

▸ `Protected` **_attachImageProcessingConfiguration**(`configuration`): `void`

Attaches a new image processing configuration to the Standard Material.

#### Parameters

| Name | Type |
| :------ | :------ |
| `configuration` | [`Nullable`](../modules.md#nullable)[`ImageProcessingConfiguration`](ImageProcessingConfiguration.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:596

___

### \_hasAlphaChannel

▸ `Protected` **_hasAlphaChannel**(): `boolean`

Specifies whether or not there is a usable alpha channel for transparency.

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:867

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

PushMaterial.\_isReadyForSubMesh

#### Defined in

packages/dev/core/src/Materials/pushMaterial.ts:43

___

### \_markAllSubMeshesAsAllDirty

▸ `Protected` **_markAllSubMeshesAsAllDirty**(): `void`

Indicates that we need to re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

PushMaterial.\_markAllSubMeshesAsAllDirty

#### Defined in

packages/dev/core/src/Materials/material.ts:1543

___

### \_markAllSubMeshesAsAttributesDirty

▸ `Protected` **_markAllSubMeshesAsAttributesDirty**(): `void`

Indicates that attributes need to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

PushMaterial.\_markAllSubMeshesAsAttributesDirty

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

PushMaterial.\_markAllSubMeshesAsDirty

#### Defined in

packages/dev/core/src/Materials/material.ts:1498

___

### \_markAllSubMeshesAsFresnelAndMiscDirty

▸ `Protected` **_markAllSubMeshesAsFresnelAndMiscDirty**(): `void`

Indicates that fresnel and misc need to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

PushMaterial.\_markAllSubMeshesAsFresnelAndMiscDirty

#### Defined in

packages/dev/core/src/Materials/material.ts:1571

___

### \_markAllSubMeshesAsFresnelDirty

▸ `Protected` **_markAllSubMeshesAsFresnelDirty**(): `void`

Indicates that fresnel needs to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

PushMaterial.\_markAllSubMeshesAsFresnelDirty

#### Defined in

packages/dev/core/src/Materials/material.ts:1564

___

### \_markAllSubMeshesAsImageProcessingDirty

▸ `Protected` **_markAllSubMeshesAsImageProcessingDirty**(): `void`

Indicates that image processing needs to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

PushMaterial.\_markAllSubMeshesAsImageProcessingDirty

#### Defined in

packages/dev/core/src/Materials/material.ts:1550

___

### \_markAllSubMeshesAsLightsDirty

▸ `Protected` **_markAllSubMeshesAsLightsDirty**(): `void`

Indicates that lights need to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

PushMaterial.\_markAllSubMeshesAsLightsDirty

#### Defined in

packages/dev/core/src/Materials/material.ts:1578

___

### \_markAllSubMeshesAsMiscDirty

▸ `Protected` **_markAllSubMeshesAsMiscDirty**(): `void`

Indicates that misc needs to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

PushMaterial.\_markAllSubMeshesAsMiscDirty

#### Defined in

packages/dev/core/src/Materials/material.ts:1592

___

### \_markAllSubMeshesAsPrePassDirty

▸ `Protected` **_markAllSubMeshesAsPrePassDirty**(): `void`

Indicates that prepass needs to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

PushMaterial.\_markAllSubMeshesAsPrePassDirty

#### Defined in

packages/dev/core/src/Materials/material.ts:1599

___

### \_markAllSubMeshesAsTexturesAndMiscDirty

▸ `Protected` **_markAllSubMeshesAsTexturesAndMiscDirty**(): `void`

Indicates that textures and misc need to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

PushMaterial.\_markAllSubMeshesAsTexturesAndMiscDirty

#### Defined in

packages/dev/core/src/Materials/material.ts:1606

___

### \_markAllSubMeshesAsTexturesDirty

▸ `Protected` **_markAllSubMeshesAsTexturesDirty**(): `void`

Indicates that textures need to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

PushMaterial.\_markAllSubMeshesAsTexturesDirty

#### Defined in

packages/dev/core/src/Materials/material.ts:1557

___

### \_markScenePrePassDirty

▸ `Protected` **_markScenePrePassDirty**(): `void`

Indicates that the scene should check if the rendering now needs a prepass

#### Returns

`void`

#### Inherited from

PushMaterial.\_markScenePrePassDirty

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

PushMaterial.\_mustRebind

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

PushMaterial.\_shouldTurnAlphaTestOn

#### Defined in

packages/dev/core/src/Materials/material.ts:1040

___

### \_shouldUseAlphaFromDiffuseTexture

▸ `Protected` **_shouldUseAlphaFromDiffuseTexture**(): `boolean`

Specifies whether or not the alpha value of the diffuse texture should be used for alpha blending.

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:860

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

PushMaterial.bind

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

PushMaterial.bindEyePosition

#### Defined in

packages/dev/core/src/Materials/material.ts:1168

___

### bindForSubMesh

▸ **bindForSubMesh**(`world`, `mesh`, `subMesh`): `void`

Binds the submesh to this material by preparing the effect and shader to draw

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `world` | [`Matrix`](Matrix.md) | defines the world transformation matrix |
| `mesh` | [`Mesh`](Mesh.md) | defines the mesh containing the submesh |
| `subMesh` | [`SubMesh`](SubMesh.md) | defines the submesh to bind the material to |

#### Returns

`void`

#### Overrides

PushMaterial.bindForSubMesh

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:1515

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

PushMaterial.bindOnlyNormalMatrix

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

PushMaterial.bindOnlyWorldMatrix

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

PushMaterial.bindView

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

PushMaterial.bindViewProjection

#### Defined in

packages/dev/core/src/Materials/material.ts:1154

___

### buildUniformLayout

▸ **buildUniformLayout**(): `void`

Builds the material UBO layouts.
Used internally during the effect preparation.

#### Returns

`void`

#### Overrides

PushMaterial.buildUniformLayout

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:1462

___

### clone

▸ **clone**(`name`): [`StandardMaterial`](StandardMaterial.md)

Makes a duplicate of the material, and gives it a new name

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the new name for the duplicated material |

#### Returns

[`StandardMaterial`](StandardMaterial.md)

the cloned material

#### Overrides

PushMaterial.clone

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:1964

___

### dispose

▸ **dispose**(`forceDisposeEffect?`, `forceDisposeTextures?`): `void`

Disposes the material

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `forceDisposeEffect?` | `boolean` | specifies if effects should be forcefully disposed |
| `forceDisposeTextures?` | `boolean` | specifies if textures should be forcefully disposed |

#### Returns

`void`

#### Overrides

PushMaterial.dispose

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:1939

___

### forceCompilation

▸ **forceCompilation**(`mesh`, `onCompiled?`, `options?`, `onError?`): `void`

Force shader compilation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | defines the mesh associated with this material |
| `onCompiled?` | (`material`: [`Material`](Material.md)) => `void` | defines a function to execute once the material is compiled |
| `options?` | `Partial`[`IMaterialCompilationOptions`](../interfaces/IMaterialCompilationOptions.md) | defines the options to configure the compilation |
| `onError?` | (`reason`: `string`) => `void` | defines a function to execute if the material fails compiling |

#### Returns

`void`

#### Inherited from

PushMaterial.forceCompilation

#### Defined in

packages/dev/core/src/Materials/material.ts:1312

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

PushMaterial.forceCompilationAsync

#### Defined in

packages/dev/core/src/Materials/material.ts:1392

___

### freeze

▸ **freeze**(): `void`

Locks updates for the material

#### Returns

`void`

#### Inherited from

PushMaterial.freeze

#### Defined in

packages/dev/core/src/Materials/material.ts:890

___

### getActiveTextures

▸ **getActiveTextures**(): [`BaseTexture`](BaseTexture.md)[]

Gets the active textures from the material

#### Returns

[`BaseTexture`](BaseTexture.md)[]

an array of textures

#### Overrides

PushMaterial.getActiveTextures

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:1843

___

### getAlphaTestTexture

▸ **getAlphaTestTexture**(): [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Get the texture used for alpha test purpose.

#### Returns

[`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

the diffuse texture in case of the standard material.

#### Overrides

PushMaterial.getAlphaTestTexture

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:875

___

### getAnimatables

▸ **getAnimatables**(): [`IAnimatable`](../interfaces/IAnimatable.md)[]

Get the list of animatables in the material.

#### Returns

[`IAnimatable`](../interfaces/IAnimatable.md)[]

the list of animatables object used in the material

#### Overrides

PushMaterial.getAnimatables

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:1797

___

### getBindedMeshes

▸ **getBindedMeshes**(): [`AbstractMesh`](AbstractMesh.md)[]

Gets the meshes bound to the material

#### Returns

[`AbstractMesh`](AbstractMesh.md)[]

an array of meshes bound to the material

#### Inherited from

PushMaterial.getBindedMeshes

#### Defined in

packages/dev/core/src/Materials/material.ts:1289

___

### getClassName

▸ **getClassName**(): `string`

Gets the current class name of the material e.g. "StandardMaterial"
Mainly use in serialization.

#### Returns

`string`

the class name

#### Overrides

PushMaterial.getClassName

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:808

___

### getEffect

▸ **getEffect**(): [`Effect`](Effect.md)

#### Returns

[`Effect`](Effect.md)

#### Inherited from

PushMaterial.getEffect

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

PushMaterial.getScene

#### Defined in

packages/dev/core/src/Materials/material.ts:947

___

### hasTexture

▸ **hasTexture**(`texture`): `boolean`

Specifies if the material uses a texture

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `texture` | [`BaseTexture`](BaseTexture.md) | defines the texture to check against the material |

#### Returns

`boolean`

a boolean specifying if the material uses the texture

#### Overrides

PushMaterial.hasTexture

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:1890

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

PushMaterial.isReady

#### Defined in

packages/dev/core/src/Materials/pushMaterial.ts:27

___

### isReadyForSubMesh

▸ **isReadyForSubMesh**(`mesh`, `subMesh`, `useInstances?`): `boolean`

Get if the submesh is ready to be used and all its information available.
Child classes can use it to update shaders

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | `undefined` | defines the mesh to check |
| `subMesh` | [`SubMesh`](SubMesh.md) | `undefined` | defines which submesh to check |
| `useInstances` | `boolean` | `false` | specifies that instances should be used |

#### Returns

`boolean`

a boolean indicating that the submesh is ready or not

#### Overrides

PushMaterial.isReadyForSubMesh

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:887

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

PushMaterial.markAsDirty

#### Defined in

packages/dev/core/src/Materials/material.ts:1437

___

### markDirty

▸ **markDirty**(): `void`

Marks the material to indicate that it needs to be re-calculated

#### Returns

`void`

#### Inherited from

PushMaterial.markDirty

#### Defined in

packages/dev/core/src/Materials/material.ts:1055

___

### needAlphaBlending

▸ **needAlphaBlending**(): `boolean`

Specifies if the material will require alpha blending

#### Returns

`boolean`

a boolean specifying if alpha blending is needed

#### Overrides

PushMaterial.needAlphaBlending

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:832

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

PushMaterial.needAlphaBlendingForMesh

#### Defined in

packages/dev/core/src/Materials/material.ts:1016

___

### needAlphaTesting

▸ **needAlphaTesting**(): `boolean`

Specifies if this material should be rendered in alpha test mode

#### Returns

`boolean`

a boolean specifying if an alpha test is needed.

#### Overrides

PushMaterial.needAlphaTesting

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:849

___

### resetDrawCache

▸ **resetDrawCache**(): `void`

Resets the draw wrappers cache for all submeshes that are using this material

#### Returns

`void`

#### Inherited from

PushMaterial.resetDrawCache

#### Defined in

packages/dev/core/src/Materials/material.ts:1478

___

### serialize

▸ **serialize**(): `any`

Serializes this material

#### Returns

`any`

the serialized material object

#### Inherited from

PushMaterial.serialize

#### Defined in

packages/dev/core/src/Materials/material.ts:1724

___

### setPrePassRenderer

▸ **setPrePassRenderer**(`prePassRenderer`): `boolean`

Sets the required values to the prepass renderer.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `prePassRenderer` | [`PrePassRenderer`](PrePassRenderer.md) | defines the prepass renderer to setup. |

#### Returns

`boolean`

true if the pre pass is needed.

#### Inherited from

PushMaterial.setPrePassRenderer

#### Defined in

packages/dev/core/src/Materials/material.ts:1616

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

PushMaterial.toString

#### Defined in

packages/dev/core/src/Materials/material.ts:867

___

### unbind

▸ **unbind**(): `void`

Unbinds the material from the mesh

#### Returns

`void`

#### Inherited from

PushMaterial.unbind

#### Defined in

packages/dev/core/src/Materials/material.ts:1222

___

### unfreeze

▸ **unfreeze**(): `void`

Unlocks updates for the material

#### Returns

`void`

#### Inherited from

PushMaterial.unfreeze

#### Defined in

packages/dev/core/src/Materials/material.ts:898

___

### Parse

▸ `Static` **Parse**(`source`, `scene`, `rootUrl`): [`StandardMaterial`](StandardMaterial.md)

Creates a standard material from parsed material data

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | `any` | defines the JSON representation of the material |
| `scene` | [`Scene`](Scene.md) | defines the hosting scene |
| `rootUrl` | `string` | defines the root URL to use to load textures and relative dependencies |

#### Returns

[`StandardMaterial`](StandardMaterial.md)

a new standard material

#### Overrides

PushMaterial.Parse

#### Defined in

packages/dev/core/src/Materials/standardMaterial.ts:1982
