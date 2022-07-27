[@dev/core](../README.md) / [Exports](../modules.md) / PBRBaseSimpleMaterial

# Class: PBRBaseSimpleMaterial

The Physically based simple base material of BJS.

This enables better naming and convention enforcements on top of the pbrMaterial.
It is used as the base class for both the specGloss and metalRough conventions.

## Hierarchy

- [`PBRBaseMaterial`](PBRBaseMaterial.md)

  ↳ **`PBRBaseSimpleMaterial`**

  ↳↳ [`PBRMetallicRoughnessMaterial`](PBRMetallicRoughnessMaterial.md)

  ↳↳ [`PBRSpecularGlossinessMaterial`](PBRSpecularGlossinessMaterial.md)

## Table of contents

### Constructors

- [constructor](PBRBaseSimpleMaterial.md#constructor)

### Properties

- [\_activeEffect](PBRBaseSimpleMaterial.md#_activeeffect)
- [\_alpha](PBRBaseSimpleMaterial.md#_alpha)
- [\_backFaceCulling](PBRBaseSimpleMaterial.md#_backfaceculling)
- [\_cacheHasRenderTargetTextures](PBRBaseSimpleMaterial.md#_cachehasrendertargettextures)
- [\_cullBackFaces](PBRBaseSimpleMaterial.md#_cullbackfaces)
- [\_drawWrapper](PBRBaseSimpleMaterial.md#_drawwrapper)
- [\_eventInfo](PBRBaseSimpleMaterial.md#_eventinfo)
- [\_imageProcessingConfiguration](PBRBaseSimpleMaterial.md#_imageprocessingconfiguration)
- [\_needToBindSceneUbo](PBRBaseSimpleMaterial.md#_needtobindsceneubo)
- [\_normalMatrix](PBRBaseSimpleMaterial.md#_normalmatrix)
- [\_onEffectCreatedObservable](PBRBaseSimpleMaterial.md#_oneffectcreatedobservable)
- [\_transparencyMode](PBRBaseSimpleMaterial.md#_transparencymode)
- [allowShaderHotSwapping](PBRBaseSimpleMaterial.md#allowshaderhotswapping)
- [alphaCutOff](PBRBaseSimpleMaterial.md#alphacutoff)
- [animations](PBRBaseSimpleMaterial.md#animations)
- [anisotropy](PBRBaseSimpleMaterial.md#anisotropy)
- [brdf](PBRBaseSimpleMaterial.md#brdf)
- [checkReadyOnEveryCall](PBRBaseSimpleMaterial.md#checkreadyoneverycall)
- [checkReadyOnlyOnce](PBRBaseSimpleMaterial.md#checkreadyonlyonce)
- [clearCoat](PBRBaseSimpleMaterial.md#clearcoat)
- [customShaderNameResolve](PBRBaseSimpleMaterial.md#customshadernameresolve)
- [depthFunction](PBRBaseSimpleMaterial.md#depthfunction)
- [detailMap](PBRBaseSimpleMaterial.md#detailmap)
- [disableColorWrite](PBRBaseSimpleMaterial.md#disablecolorwrite)
- [disableDepthWrite](PBRBaseSimpleMaterial.md#disabledepthwrite)
- [disableLighting](PBRBaseSimpleMaterial.md#disablelighting)
- [doNotSerialize](PBRBaseSimpleMaterial.md#donotserialize)
- [emissiveColor](PBRBaseSimpleMaterial.md#emissivecolor)
- [emissiveTexture](PBRBaseSimpleMaterial.md#emissivetexture)
- [environmentTexture](PBRBaseSimpleMaterial.md#environmenttexture)
- [forceDepthWrite](PBRBaseSimpleMaterial.md#forcedepthwrite)
- [getRenderTargetTextures](PBRBaseSimpleMaterial.md#getrendertargettextures)
- [id](PBRBaseSimpleMaterial.md#id)
- [inspectableCustomProperties](PBRBaseSimpleMaterial.md#inspectablecustomproperties)
- [invertNormalMapX](PBRBaseSimpleMaterial.md#invertnormalmapx)
- [invertNormalMapY](PBRBaseSimpleMaterial.md#invertnormalmapy)
- [iridescence](PBRBaseSimpleMaterial.md#iridescence)
- [lightmapTexture](PBRBaseSimpleMaterial.md#lightmaptexture)
- [maxSimultaneousLights](PBRBaseSimpleMaterial.md#maxsimultaneouslights)
- [metadata](PBRBaseSimpleMaterial.md#metadata)
- [name](PBRBaseSimpleMaterial.md#name)
- [normalTexture](PBRBaseSimpleMaterial.md#normaltexture)
- [occlusionStrength](PBRBaseSimpleMaterial.md#occlusionstrength)
- [occlusionTexture](PBRBaseSimpleMaterial.md#occlusiontexture)
- [onCompiled](PBRBaseSimpleMaterial.md#oncompiled)
- [onDisposeObservable](PBRBaseSimpleMaterial.md#ondisposeobservable)
- [onError](PBRBaseSimpleMaterial.md#onerror)
- [pluginManager](PBRBaseSimpleMaterial.md#pluginmanager)
- [pointSize](PBRBaseSimpleMaterial.md#pointsize)
- [prePassConfiguration](PBRBaseSimpleMaterial.md#prepassconfiguration)
- [reservedDataStore](PBRBaseSimpleMaterial.md#reserveddatastore)
- [separateCullingPass](PBRBaseSimpleMaterial.md#separatecullingpass)
- [shadowDepthWrapper](PBRBaseSimpleMaterial.md#shadowdepthwrapper)
- [sheen](PBRBaseSimpleMaterial.md#sheen)
- [sideOrientation](PBRBaseSimpleMaterial.md#sideorientation)
- [state](PBRBaseSimpleMaterial.md#state)
- [stencil](PBRBaseSimpleMaterial.md#stencil)
- [subSurface](PBRBaseSimpleMaterial.md#subsurface)
- [uniqueId](PBRBaseSimpleMaterial.md#uniqueid)
- [useLightmapAsShadowmap](PBRBaseSimpleMaterial.md#uselightmapasshadowmap)
- [zOffset](PBRBaseSimpleMaterial.md#zoffset)
- [zOffsetUnits](PBRBaseSimpleMaterial.md#zoffsetunits)
- [AllDirtyFlag](PBRBaseSimpleMaterial.md#alldirtyflag)
- [AttributesDirtyFlag](PBRBaseSimpleMaterial.md#attributesdirtyflag)
- [ClockWiseSideOrientation](PBRBaseSimpleMaterial.md#clockwisesideorientation)
- [CounterClockWiseSideOrientation](PBRBaseSimpleMaterial.md#counterclockwisesideorientation)
- [DEFAULT\_AO\_ON\_ANALYTICAL\_LIGHTS](PBRBaseSimpleMaterial.md#default_ao_on_analytical_lights)
- [FresnelDirtyFlag](PBRBaseSimpleMaterial.md#fresneldirtyflag)
- [LIGHTFALLOFF\_GLTF](PBRBaseSimpleMaterial.md#lightfalloff_gltf)
- [LIGHTFALLOFF\_PHYSICAL](PBRBaseSimpleMaterial.md#lightfalloff_physical)
- [LIGHTFALLOFF\_STANDARD](PBRBaseSimpleMaterial.md#lightfalloff_standard)
- [LightDirtyFlag](PBRBaseSimpleMaterial.md#lightdirtyflag)
- [LineListDrawMode](PBRBaseSimpleMaterial.md#linelistdrawmode)
- [LineLoopDrawMode](PBRBaseSimpleMaterial.md#lineloopdrawmode)
- [LineStripDrawMode](PBRBaseSimpleMaterial.md#linestripdrawmode)
- [MATERIAL\_ALPHABLEND](PBRBaseSimpleMaterial.md#material_alphablend)
- [MATERIAL\_ALPHATEST](PBRBaseSimpleMaterial.md#material_alphatest)
- [MATERIAL\_ALPHATESTANDBLEND](PBRBaseSimpleMaterial.md#material_alphatestandblend)
- [MATERIAL\_NORMALBLENDMETHOD\_RNM](PBRBaseSimpleMaterial.md#material_normalblendmethod_rnm)
- [MATERIAL\_NORMALBLENDMETHOD\_WHITEOUT](PBRBaseSimpleMaterial.md#material_normalblendmethod_whiteout)
- [MATERIAL\_OPAQUE](PBRBaseSimpleMaterial.md#material_opaque)
- [MiscDirtyFlag](PBRBaseSimpleMaterial.md#miscdirtyflag)
- [OnEventObservable](PBRBaseSimpleMaterial.md#oneventobservable)
- [PBRMATERIAL\_ALPHABLEND](PBRBaseSimpleMaterial.md#pbrmaterial_alphablend)
- [PBRMATERIAL\_ALPHATEST](PBRBaseSimpleMaterial.md#pbrmaterial_alphatest)
- [PBRMATERIAL\_ALPHATESTANDBLEND](PBRBaseSimpleMaterial.md#pbrmaterial_alphatestandblend)
- [PBRMATERIAL\_OPAQUE](PBRBaseSimpleMaterial.md#pbrmaterial_opaque)
- [PointFillMode](PBRBaseSimpleMaterial.md#pointfillmode)
- [PointListDrawMode](PBRBaseSimpleMaterial.md#pointlistdrawmode)
- [PrePassDirtyFlag](PBRBaseSimpleMaterial.md#prepassdirtyflag)
- [TextureDirtyFlag](PBRBaseSimpleMaterial.md#texturedirtyflag)
- [TriangleFanDrawMode](PBRBaseSimpleMaterial.md#trianglefandrawmode)
- [TriangleFillMode](PBRBaseSimpleMaterial.md#trianglefillmode)
- [TriangleStripDrawMode](PBRBaseSimpleMaterial.md#trianglestripdrawmode)
- [WireFrameFillMode](PBRBaseSimpleMaterial.md#wireframefillmode)

### Accessors

- [\_disableAlphaBlending](PBRBaseSimpleMaterial.md#_disablealphablending)
- [alpha](PBRBaseSimpleMaterial.md#alpha)
- [alphaMode](PBRBaseSimpleMaterial.md#alphamode)
- [backFaceCulling](PBRBaseSimpleMaterial.md#backfaceculling)
- [canRenderToMRT](PBRBaseSimpleMaterial.md#canrendertomrt)
- [cullBackFaces](PBRBaseSimpleMaterial.md#cullbackfaces)
- [doubleSided](PBRBaseSimpleMaterial.md#doublesided)
- [fillMode](PBRBaseSimpleMaterial.md#fillmode)
- [fogEnabled](PBRBaseSimpleMaterial.md#fogenabled)
- [hasRenderTargetTextures](PBRBaseSimpleMaterial.md#hasrendertargettextures)
- [isFrozen](PBRBaseSimpleMaterial.md#isfrozen)
- [isPrePassCapable](PBRBaseSimpleMaterial.md#isprepasscapable)
- [needDepthPrePass](PBRBaseSimpleMaterial.md#needdepthprepass)
- [onBind](PBRBaseSimpleMaterial.md#onbind)
- [onBindObservable](PBRBaseSimpleMaterial.md#onbindobservable)
- [onDispose](PBRBaseSimpleMaterial.md#ondispose)
- [onEffectCreatedObservable](PBRBaseSimpleMaterial.md#oneffectcreatedobservable)
- [onUnBindObservable](PBRBaseSimpleMaterial.md#onunbindobservable)
- [pointsCloud](PBRBaseSimpleMaterial.md#pointscloud)
- [realTimeFiltering](PBRBaseSimpleMaterial.md#realtimefiltering)
- [realTimeFilteringQuality](PBRBaseSimpleMaterial.md#realtimefilteringquality)
- [transparencyMode](PBRBaseSimpleMaterial.md#transparencymode)
- [useLogarithmicDepth](PBRBaseSimpleMaterial.md#uselogarithmicdepth)
- [wireframe](PBRBaseSimpleMaterial.md#wireframe)

### Methods

- [\_afterBind](PBRBaseSimpleMaterial.md#_afterbind)
- [\_attachImageProcessingConfiguration](PBRBaseSimpleMaterial.md#_attachimageprocessingconfiguration)
- [\_hasAlphaChannel](PBRBaseSimpleMaterial.md#_hasalphachannel)
- [\_isReadyForSubMesh](PBRBaseSimpleMaterial.md#_isreadyforsubmesh)
- [\_markAllSubMeshesAsAllDirty](PBRBaseSimpleMaterial.md#_markallsubmeshesasalldirty)
- [\_markAllSubMeshesAsAttributesDirty](PBRBaseSimpleMaterial.md#_markallsubmeshesasattributesdirty)
- [\_markAllSubMeshesAsDirty](PBRBaseSimpleMaterial.md#_markallsubmeshesasdirty)
- [\_markAllSubMeshesAsFresnelAndMiscDirty](PBRBaseSimpleMaterial.md#_markallsubmeshesasfresnelandmiscdirty)
- [\_markAllSubMeshesAsFresnelDirty](PBRBaseSimpleMaterial.md#_markallsubmeshesasfresneldirty)
- [\_markAllSubMeshesAsImageProcessingDirty](PBRBaseSimpleMaterial.md#_markallsubmeshesasimageprocessingdirty)
- [\_markAllSubMeshesAsLightsDirty](PBRBaseSimpleMaterial.md#_markallsubmeshesaslightsdirty)
- [\_markAllSubMeshesAsMiscDirty](PBRBaseSimpleMaterial.md#_markallsubmeshesasmiscdirty)
- [\_markAllSubMeshesAsPrePassDirty](PBRBaseSimpleMaterial.md#_markallsubmeshesasprepassdirty)
- [\_markAllSubMeshesAsTexturesAndMiscDirty](PBRBaseSimpleMaterial.md#_markallsubmeshesastexturesandmiscdirty)
- [\_markAllSubMeshesAsTexturesDirty](PBRBaseSimpleMaterial.md#_markallsubmeshesastexturesdirty)
- [\_markScenePrePassDirty](PBRBaseSimpleMaterial.md#_marksceneprepassdirty)
- [\_mustRebind](PBRBaseSimpleMaterial.md#_mustrebind)
- [\_shouldTurnAlphaTestOn](PBRBaseSimpleMaterial.md#_shouldturnalphateston)
- [\_shouldUseAlphaFromAlbedoTexture](PBRBaseSimpleMaterial.md#_shouldusealphafromalbedotexture)
- [bind](PBRBaseSimpleMaterial.md#bind)
- [bindEyePosition](PBRBaseSimpleMaterial.md#bindeyeposition)
- [bindForSubMesh](PBRBaseSimpleMaterial.md#bindforsubmesh)
- [bindOnlyNormalMatrix](PBRBaseSimpleMaterial.md#bindonlynormalmatrix)
- [bindOnlyWorldMatrix](PBRBaseSimpleMaterial.md#bindonlyworldmatrix)
- [bindView](PBRBaseSimpleMaterial.md#bindview)
- [bindViewProjection](PBRBaseSimpleMaterial.md#bindviewprojection)
- [buildUniformLayout](PBRBaseSimpleMaterial.md#builduniformlayout)
- [clone](PBRBaseSimpleMaterial.md#clone)
- [dispose](PBRBaseSimpleMaterial.md#dispose)
- [forceCompilation](PBRBaseSimpleMaterial.md#forcecompilation)
- [forceCompilationAsync](PBRBaseSimpleMaterial.md#forcecompilationasync)
- [freeze](PBRBaseSimpleMaterial.md#freeze)
- [getActiveTextures](PBRBaseSimpleMaterial.md#getactivetextures)
- [getAlphaTestTexture](PBRBaseSimpleMaterial.md#getalphatesttexture)
- [getAnimatables](PBRBaseSimpleMaterial.md#getanimatables)
- [getBindedMeshes](PBRBaseSimpleMaterial.md#getbindedmeshes)
- [getClassName](PBRBaseSimpleMaterial.md#getclassname)
- [getEffect](PBRBaseSimpleMaterial.md#geteffect)
- [getScene](PBRBaseSimpleMaterial.md#getscene)
- [hasTexture](PBRBaseSimpleMaterial.md#hastexture)
- [isMetallicWorkflow](PBRBaseSimpleMaterial.md#ismetallicworkflow)
- [isReady](PBRBaseSimpleMaterial.md#isready)
- [isReadyForSubMesh](PBRBaseSimpleMaterial.md#isreadyforsubmesh)
- [markAsDirty](PBRBaseSimpleMaterial.md#markasdirty)
- [markDirty](PBRBaseSimpleMaterial.md#markdirty)
- [needAlphaBlending](PBRBaseSimpleMaterial.md#needalphablending)
- [needAlphaBlendingForMesh](PBRBaseSimpleMaterial.md#needalphablendingformesh)
- [needAlphaTesting](PBRBaseSimpleMaterial.md#needalphatesting)
- [resetDrawCache](PBRBaseSimpleMaterial.md#resetdrawcache)
- [serialize](PBRBaseSimpleMaterial.md#serialize)
- [setPrePassRenderer](PBRBaseSimpleMaterial.md#setprepassrenderer)
- [toString](PBRBaseSimpleMaterial.md#tostring)
- [unbind](PBRBaseSimpleMaterial.md#unbind)
- [unfreeze](PBRBaseSimpleMaterial.md#unfreeze)
- [Parse](PBRBaseSimpleMaterial.md#parse)

## Constructors

### constructor

• **new PBRBaseSimpleMaterial**(`name`, `scene?`)

Instantiates a new PBRMaterial instance.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | The material name |
| `scene?` | [`Scene`](Scene.md) | The scene the material will be use in. |

#### Overrides

[PBRBaseMaterial](PBRBaseMaterial.md).[constructor](PBRBaseMaterial.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseSimpleMaterial.ts:131

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

• **alphaCutOff**: `number`

Defines the alpha limits in alpha test mode.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseSimpleMaterial.ts:90

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

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseSimpleMaterial.ts:27

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

Emissivie color used to self-illuminate the model.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseSimpleMaterial.ts:62

___

### emissiveTexture

• **emissiveTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Emissivie texture used to self-illuminate the model.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseSimpleMaterial.ts:69

___

### environmentTexture

• **environmentTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Environment Texture used in the material (this is use for both reflection and environment lighting).

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseSimpleMaterial.ts:34

___

### forceDepthWrite

• **forceDepthWrite**: `boolean` = `false`

Specifies if depth writing should be forced

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[forceDepthWrite](PBRBaseMaterial.md#forcedepthwrite)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:578

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

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseSimpleMaterial.ts:41

___

### invertNormalMapY

• **invertNormalMapY**: `boolean` = `false`

If sets to true, y component of normal map value will invert (y = 1.0 - y).

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseSimpleMaterial.ts:48

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

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseSimpleMaterial.ts:116

___

### maxSimultaneousLights

• **maxSimultaneousLights**: `number` = `4`

Number of Simultaneous lights allowed on the material.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseSimpleMaterial.ts:20

___

### metadata

• **metadata**: `any` = `null`

Gets or sets user defined metadata

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[metadata](PBRBaseMaterial.md#metadata)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:254

___

### name

• **name**: `string`

The name of the material

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[name](PBRBaseMaterial.md#name)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:248

___

### normalTexture

• **normalTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Normal map used in the model.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseSimpleMaterial.ts:55

___

### occlusionStrength

• **occlusionStrength**: `number` = `1.0`

Occlusion Channel Strength.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseSimpleMaterial.ts:76

___

### occlusionTexture

• **occlusionTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Occlusion Texture of the material (adding extra occlusion effects).

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseSimpleMaterial.ts:83

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

### reservedDataStore

• **reservedDataStore**: `any` = `null`

For internal use only. Please do not use.

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[reservedDataStore](PBRBaseMaterial.md#reserveddatastore)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:259

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

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the material

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[uniqueId](PBRBaseMaterial.md#uniqueid)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:239

___

### useLightmapAsShadowmap

• **useLightmapAsShadowmap**: `boolean` = `false`

If true, the light map contains occlusion information instead of lighting info.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseSimpleMaterial.ts:123

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

▪ `Static` **DEFAULT\_AO\_ON\_ANALYTICAL\_LIGHTS**: `number` = `0`

Defines the default value of how much AO map is occluding the analytical lights
(point spot...).

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[DEFAULT_AO_ON_ANALYTICAL_LIGHTS](PBRBaseMaterial.md#default_ao_on_analytical_lights)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:301

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

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[PBRMATERIAL_ALPHABLEND](PBRBaseMaterial.md#pbrmaterial_alphablend)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:289

___

### PBRMATERIAL\_ALPHATEST

▪ `Static` `Readonly` **PBRMATERIAL\_ALPHATEST**: ``1``

PBRMaterialTransparencyMode: Alpha Test mode, pixel are discarded below a certain threshold defined by the alpha cutoff value.

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[PBRMATERIAL_ALPHATEST](PBRBaseMaterial.md#pbrmaterial_alphatest)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:284

___

### PBRMATERIAL\_ALPHATESTANDBLEND

▪ `Static` `Readonly` **PBRMATERIAL\_ALPHATESTANDBLEND**: ``3``

PBRMaterialTransparencyMode: Pixels are blended (according to the alpha mode) with the already drawn pixels in the current frame buffer.
They are also discarded below the alpha cutoff threshold to improve performances.

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[PBRMATERIAL_ALPHATESTANDBLEND](PBRBaseMaterial.md#pbrmaterial_alphatestandblend)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:295

___

### PBRMATERIAL\_OPAQUE

▪ `Static` `Readonly` **PBRMATERIAL\_OPAQUE**: ``0``

PBRMaterialTransparencyMode: No transparency mode, Alpha channel is not use.

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[PBRMATERIAL_OPAQUE](PBRBaseMaterial.md#pbrmaterial_opaque)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:279

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

### doubleSided

• `get` **doubleSided**(): `boolean`

Gets the current double sided mode.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseSimpleMaterial.ts:95

• `set` **doubleSided**(`value`): `void`

If sets to true and backfaceCulling is false, normals will be flipped on the backside.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseSimpleMaterial.ts:102

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

▸ **clone**(`name`): [`Nullable`](../modules.md#nullable)[`Material`](Material.md)

Makes a duplicate of the material, and gives it a new name

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the new name for the duplicated material |

#### Returns

[`Nullable`](../modules.md#nullable)[`Material`](Material.md)

the cloned material

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[clone](PBRBaseMaterial.md#clone)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1281

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

Gets the name of the material class.

#### Returns

`string`

#### Overrides

[PBRBaseMaterial](PBRBaseMaterial.md).[getClassName](PBRBaseMaterial.md#getclassname)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseSimpleMaterial.ts:138

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

Serializes this material

#### Returns

`any`

the serialized material object

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[serialize](PBRBaseMaterial.md#serialize)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1724

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

▸ `Static` **Parse**(`parsedMaterial`, `scene`, `rootUrl`): [`Nullable`](../modules.md#nullable)[`Material`](Material.md)

Creates a material from parsed material data

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `parsedMaterial` | `any` | defines parsed material data |
| `scene` | [`Scene`](Scene.md) | defines the hosting scene |
| `rootUrl` | `string` | defines the root URL to use to load textures |

#### Returns

[`Nullable`](../modules.md#nullable)[`Material`](Material.md)

a new material

#### Inherited from

[PBRBaseMaterial](PBRBaseMaterial.md).[Parse](PBRBaseMaterial.md#parse)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1739
