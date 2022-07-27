[@dev/core](../README.md) / [Exports](../modules.md) / PBRBaseMaterial

# Class: PBRBaseMaterial

The Physically based material base class of BJS.

This offers the main features of a standard PBR material.
For more information, please refer to the documentation :
https://doc.babylonjs.com/how_to/physically_based_rendering

## Hierarchy

- `PushMaterial`

  ↳ **`PBRBaseMaterial`**

  ↳↳ [`PBRBaseSimpleMaterial`](PBRBaseSimpleMaterial.md)

  ↳↳ [`PBRMaterial`](PBRMaterial.md)

## Table of contents

### Constructors

- [constructor](PBRBaseMaterial.md#constructor)

### Properties

- [\_activeEffect](PBRBaseMaterial.md#_activeeffect)
- [\_alpha](PBRBaseMaterial.md#_alpha)
- [\_backFaceCulling](PBRBaseMaterial.md#_backfaceculling)
- [\_cacheHasRenderTargetTextures](PBRBaseMaterial.md#_cachehasrendertargettextures)
- [\_cullBackFaces](PBRBaseMaterial.md#_cullbackfaces)
- [\_debugMode](PBRBaseMaterial.md#_debugmode)
- [\_drawWrapper](PBRBaseMaterial.md#_drawwrapper)
- [\_eventInfo](PBRBaseMaterial.md#_eventinfo)
- [\_globalAmbientColor](PBRBaseMaterial.md#_globalambientcolor)
- [\_imageProcessingConfiguration](PBRBaseMaterial.md#_imageprocessingconfiguration)
- [\_imageProcessingObserver](PBRBaseMaterial.md#_imageprocessingobserver)
- [\_lightingInfos](PBRBaseMaterial.md#_lightinginfos)
- [\_needToBindSceneUbo](PBRBaseMaterial.md#_needtobindsceneubo)
- [\_normalMatrix](PBRBaseMaterial.md#_normalmatrix)
- [\_onEffectCreatedObservable](PBRBaseMaterial.md#_oneffectcreatedobservable)
- [\_realTimeFiltering](PBRBaseMaterial.md#_realtimefiltering)
- [\_realTimeFilteringQuality](PBRBaseMaterial.md#_realtimefilteringquality)
- [\_renderTargets](PBRBaseMaterial.md#_rendertargets)
- [\_transparencyMode](PBRBaseMaterial.md#_transparencymode)
- [\_unlit](PBRBaseMaterial.md#_unlit)
- [\_useLogarithmicDepth](PBRBaseMaterial.md#_uselogarithmicdepth)
- [allowShaderHotSwapping](PBRBaseMaterial.md#allowshaderhotswapping)
- [animations](PBRBaseMaterial.md#animations)
- [anisotropy](PBRBaseMaterial.md#anisotropy)
- [brdf](PBRBaseMaterial.md#brdf)
- [checkReadyOnEveryCall](PBRBaseMaterial.md#checkreadyoneverycall)
- [checkReadyOnlyOnce](PBRBaseMaterial.md#checkreadyonlyonce)
- [clearCoat](PBRBaseMaterial.md#clearcoat)
- [customShaderNameResolve](PBRBaseMaterial.md#customshadernameresolve)
- [depthFunction](PBRBaseMaterial.md#depthfunction)
- [detailMap](PBRBaseMaterial.md#detailmap)
- [disableColorWrite](PBRBaseMaterial.md#disablecolorwrite)
- [disableDepthWrite](PBRBaseMaterial.md#disabledepthwrite)
- [doNotSerialize](PBRBaseMaterial.md#donotserialize)
- [forceDepthWrite](PBRBaseMaterial.md#forcedepthwrite)
- [getRenderTargetTextures](PBRBaseMaterial.md#getrendertargettextures)
- [id](PBRBaseMaterial.md#id)
- [inspectableCustomProperties](PBRBaseMaterial.md#inspectablecustomproperties)
- [iridescence](PBRBaseMaterial.md#iridescence)
- [metadata](PBRBaseMaterial.md#metadata)
- [name](PBRBaseMaterial.md#name)
- [onCompiled](PBRBaseMaterial.md#oncompiled)
- [onDisposeObservable](PBRBaseMaterial.md#ondisposeobservable)
- [onError](PBRBaseMaterial.md#onerror)
- [pluginManager](PBRBaseMaterial.md#pluginmanager)
- [pointSize](PBRBaseMaterial.md#pointsize)
- [prePassConfiguration](PBRBaseMaterial.md#prepassconfiguration)
- [reservedDataStore](PBRBaseMaterial.md#reserveddatastore)
- [separateCullingPass](PBRBaseMaterial.md#separatecullingpass)
- [shadowDepthWrapper](PBRBaseMaterial.md#shadowdepthwrapper)
- [sheen](PBRBaseMaterial.md#sheen)
- [sideOrientation](PBRBaseMaterial.md#sideorientation)
- [state](PBRBaseMaterial.md#state)
- [stencil](PBRBaseMaterial.md#stencil)
- [subSurface](PBRBaseMaterial.md#subsurface)
- [uniqueId](PBRBaseMaterial.md#uniqueid)
- [zOffset](PBRBaseMaterial.md#zoffset)
- [zOffsetUnits](PBRBaseMaterial.md#zoffsetunits)
- [AllDirtyFlag](PBRBaseMaterial.md#alldirtyflag)
- [AttributesDirtyFlag](PBRBaseMaterial.md#attributesdirtyflag)
- [ClockWiseSideOrientation](PBRBaseMaterial.md#clockwisesideorientation)
- [CounterClockWiseSideOrientation](PBRBaseMaterial.md#counterclockwisesideorientation)
- [DEFAULT\_AO\_ON\_ANALYTICAL\_LIGHTS](PBRBaseMaterial.md#default_ao_on_analytical_lights)
- [FresnelDirtyFlag](PBRBaseMaterial.md#fresneldirtyflag)
- [LIGHTFALLOFF\_GLTF](PBRBaseMaterial.md#lightfalloff_gltf)
- [LIGHTFALLOFF\_PHYSICAL](PBRBaseMaterial.md#lightfalloff_physical)
- [LIGHTFALLOFF\_STANDARD](PBRBaseMaterial.md#lightfalloff_standard)
- [LightDirtyFlag](PBRBaseMaterial.md#lightdirtyflag)
- [LineListDrawMode](PBRBaseMaterial.md#linelistdrawmode)
- [LineLoopDrawMode](PBRBaseMaterial.md#lineloopdrawmode)
- [LineStripDrawMode](PBRBaseMaterial.md#linestripdrawmode)
- [MATERIAL\_ALPHABLEND](PBRBaseMaterial.md#material_alphablend)
- [MATERIAL\_ALPHATEST](PBRBaseMaterial.md#material_alphatest)
- [MATERIAL\_ALPHATESTANDBLEND](PBRBaseMaterial.md#material_alphatestandblend)
- [MATERIAL\_NORMALBLENDMETHOD\_RNM](PBRBaseMaterial.md#material_normalblendmethod_rnm)
- [MATERIAL\_NORMALBLENDMETHOD\_WHITEOUT](PBRBaseMaterial.md#material_normalblendmethod_whiteout)
- [MATERIAL\_OPAQUE](PBRBaseMaterial.md#material_opaque)
- [MiscDirtyFlag](PBRBaseMaterial.md#miscdirtyflag)
- [OnEventObservable](PBRBaseMaterial.md#oneventobservable)
- [PBRMATERIAL\_ALPHABLEND](PBRBaseMaterial.md#pbrmaterial_alphablend)
- [PBRMATERIAL\_ALPHATEST](PBRBaseMaterial.md#pbrmaterial_alphatest)
- [PBRMATERIAL\_ALPHATESTANDBLEND](PBRBaseMaterial.md#pbrmaterial_alphatestandblend)
- [PBRMATERIAL\_OPAQUE](PBRBaseMaterial.md#pbrmaterial_opaque)
- [PointFillMode](PBRBaseMaterial.md#pointfillmode)
- [PointListDrawMode](PBRBaseMaterial.md#pointlistdrawmode)
- [PrePassDirtyFlag](PBRBaseMaterial.md#prepassdirtyflag)
- [TextureDirtyFlag](PBRBaseMaterial.md#texturedirtyflag)
- [TriangleFanDrawMode](PBRBaseMaterial.md#trianglefandrawmode)
- [TriangleFillMode](PBRBaseMaterial.md#trianglefillmode)
- [TriangleStripDrawMode](PBRBaseMaterial.md#trianglestripdrawmode)
- [WireFrameFillMode](PBRBaseMaterial.md#wireframefillmode)

### Accessors

- [\_disableAlphaBlending](PBRBaseMaterial.md#_disablealphablending)
- [alpha](PBRBaseMaterial.md#alpha)
- [alphaMode](PBRBaseMaterial.md#alphamode)
- [backFaceCulling](PBRBaseMaterial.md#backfaceculling)
- [canRenderToMRT](PBRBaseMaterial.md#canrendertomrt)
- [cullBackFaces](PBRBaseMaterial.md#cullbackfaces)
- [fillMode](PBRBaseMaterial.md#fillmode)
- [fogEnabled](PBRBaseMaterial.md#fogenabled)
- [hasRenderTargetTextures](PBRBaseMaterial.md#hasrendertargettextures)
- [isFrozen](PBRBaseMaterial.md#isfrozen)
- [isPrePassCapable](PBRBaseMaterial.md#isprepasscapable)
- [needDepthPrePass](PBRBaseMaterial.md#needdepthprepass)
- [onBind](PBRBaseMaterial.md#onbind)
- [onBindObservable](PBRBaseMaterial.md#onbindobservable)
- [onDispose](PBRBaseMaterial.md#ondispose)
- [onEffectCreatedObservable](PBRBaseMaterial.md#oneffectcreatedobservable)
- [onUnBindObservable](PBRBaseMaterial.md#onunbindobservable)
- [pointsCloud](PBRBaseMaterial.md#pointscloud)
- [realTimeFiltering](PBRBaseMaterial.md#realtimefiltering)
- [realTimeFilteringQuality](PBRBaseMaterial.md#realtimefilteringquality)
- [transparencyMode](PBRBaseMaterial.md#transparencymode)
- [useLogarithmicDepth](PBRBaseMaterial.md#uselogarithmicdepth)
- [wireframe](PBRBaseMaterial.md#wireframe)

### Methods

- [\_afterBind](PBRBaseMaterial.md#_afterbind)
- [\_attachImageProcessingConfiguration](PBRBaseMaterial.md#_attachimageprocessingconfiguration)
- [\_getReflectionTexture](PBRBaseMaterial.md#_getreflectiontexture)
- [\_hasAlphaChannel](PBRBaseMaterial.md#_hasalphachannel)
- [\_isReadyForSubMesh](PBRBaseMaterial.md#_isreadyforsubmesh)
- [\_markAllSubMeshesAsAllDirty](PBRBaseMaterial.md#_markallsubmeshesasalldirty)
- [\_markAllSubMeshesAsAttributesDirty](PBRBaseMaterial.md#_markallsubmeshesasattributesdirty)
- [\_markAllSubMeshesAsDirty](PBRBaseMaterial.md#_markallsubmeshesasdirty)
- [\_markAllSubMeshesAsFresnelAndMiscDirty](PBRBaseMaterial.md#_markallsubmeshesasfresnelandmiscdirty)
- [\_markAllSubMeshesAsFresnelDirty](PBRBaseMaterial.md#_markallsubmeshesasfresneldirty)
- [\_markAllSubMeshesAsImageProcessingDirty](PBRBaseMaterial.md#_markallsubmeshesasimageprocessingdirty)
- [\_markAllSubMeshesAsLightsDirty](PBRBaseMaterial.md#_markallsubmeshesaslightsdirty)
- [\_markAllSubMeshesAsMiscDirty](PBRBaseMaterial.md#_markallsubmeshesasmiscdirty)
- [\_markAllSubMeshesAsPrePassDirty](PBRBaseMaterial.md#_markallsubmeshesasprepassdirty)
- [\_markAllSubMeshesAsTexturesAndMiscDirty](PBRBaseMaterial.md#_markallsubmeshesastexturesandmiscdirty)
- [\_markAllSubMeshesAsTexturesDirty](PBRBaseMaterial.md#_markallsubmeshesastexturesdirty)
- [\_markScenePrePassDirty](PBRBaseMaterial.md#_marksceneprepassdirty)
- [\_mustRebind](PBRBaseMaterial.md#_mustrebind)
- [\_prepareDefines](PBRBaseMaterial.md#_preparedefines)
- [\_prepareEffect](PBRBaseMaterial.md#_prepareeffect)
- [\_shouldTurnAlphaTestOn](PBRBaseMaterial.md#_shouldturnalphateston)
- [\_shouldUseAlphaFromAlbedoTexture](PBRBaseMaterial.md#_shouldusealphafromalbedotexture)
- [bind](PBRBaseMaterial.md#bind)
- [bindEyePosition](PBRBaseMaterial.md#bindeyeposition)
- [bindForSubMesh](PBRBaseMaterial.md#bindforsubmesh)
- [bindOnlyNormalMatrix](PBRBaseMaterial.md#bindonlynormalmatrix)
- [bindOnlyWorldMatrix](PBRBaseMaterial.md#bindonlyworldmatrix)
- [bindView](PBRBaseMaterial.md#bindview)
- [bindViewProjection](PBRBaseMaterial.md#bindviewprojection)
- [buildUniformLayout](PBRBaseMaterial.md#builduniformlayout)
- [clone](PBRBaseMaterial.md#clone)
- [dispose](PBRBaseMaterial.md#dispose)
- [forceCompilation](PBRBaseMaterial.md#forcecompilation)
- [forceCompilationAsync](PBRBaseMaterial.md#forcecompilationasync)
- [freeze](PBRBaseMaterial.md#freeze)
- [getActiveTextures](PBRBaseMaterial.md#getactivetextures)
- [getAlphaTestTexture](PBRBaseMaterial.md#getalphatesttexture)
- [getAnimatables](PBRBaseMaterial.md#getanimatables)
- [getBindedMeshes](PBRBaseMaterial.md#getbindedmeshes)
- [getClassName](PBRBaseMaterial.md#getclassname)
- [getEffect](PBRBaseMaterial.md#geteffect)
- [getScene](PBRBaseMaterial.md#getscene)
- [hasTexture](PBRBaseMaterial.md#hastexture)
- [isMetallicWorkflow](PBRBaseMaterial.md#ismetallicworkflow)
- [isReady](PBRBaseMaterial.md#isready)
- [isReadyForSubMesh](PBRBaseMaterial.md#isreadyforsubmesh)
- [markAsDirty](PBRBaseMaterial.md#markasdirty)
- [markDirty](PBRBaseMaterial.md#markdirty)
- [needAlphaBlending](PBRBaseMaterial.md#needalphablending)
- [needAlphaBlendingForMesh](PBRBaseMaterial.md#needalphablendingformesh)
- [needAlphaTesting](PBRBaseMaterial.md#needalphatesting)
- [resetDrawCache](PBRBaseMaterial.md#resetdrawcache)
- [serialize](PBRBaseMaterial.md#serialize)
- [setPrePassRenderer](PBRBaseMaterial.md#setprepassrenderer)
- [toString](PBRBaseMaterial.md#tostring)
- [unbind](PBRBaseMaterial.md#unbind)
- [unfreeze](PBRBaseMaterial.md#unfreeze)
- [Parse](PBRBaseMaterial.md#parse)

## Constructors

### constructor

• **new PBRBaseMaterial**(`name`, `scene?`)

Instantiates a new PBRMaterial instance.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | The material name |
| `scene?` | [`Scene`](Scene.md) | The scene the material will be use in. |

#### Overrides

PushMaterial.constructor

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:896

## Properties

### \_activeEffect

• `Protected` **\_activeEffect**: [`Effect`](Effect.md)

#### Inherited from

PushMaterial.\_activeEffect

#### Defined in

https://github.com/babylon.js/core/src/Materials/pushMaterial.ts:14

___

### \_alpha

• `Protected` **\_alpha**: `number` = `1.0`

The alpha value of the material

#### Inherited from

PushMaterial.\_alpha

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:292

___

### \_backFaceCulling

• `Protected` **\_backFaceCulling**: `boolean` = `true`

Specifies if back face culling is enabled

#### Inherited from

PushMaterial.\_backFaceCulling

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:328

___

### \_cacheHasRenderTargetTextures

• `Protected` **\_cacheHasRenderTargetTextures**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:888

___

### \_cullBackFaces

• `Protected` **\_cullBackFaces**: `boolean` = `true`

Specifies if back or front faces should be culled (when culling is enabled)

#### Inherited from

PushMaterial.\_cullBackFaces

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:352

___

### \_debugMode

• `Private` **\_debugMode**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:820

___

### \_drawWrapper

• `Protected` **\_drawWrapper**: `DrawWrapper`

#### Inherited from

PushMaterial.\_drawWrapper

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:705

___

### \_eventInfo

• `Protected` **\_eventInfo**: `MaterialPluginDisposed` & `MaterialPluginHasTexture` & `MaterialPluginIsReadyForSubMesh` & `MaterialPluginGetDefineNames` & `MaterialPluginPrepareEffect` & `MaterialPluginPrepareDefines` & `MaterialPluginPrepareUniformBuffer` & `MaterialPluginBindForSubMesh` & `MaterialPluginGetAnimatables` & `MaterialPluginGetActiveTextures` & `MaterialPluginFillRenderTargetTextures` & `MaterialPluginHasRenderTargetTextures` & `MaterialPluginHardBindForSubMesh`

#### Inherited from

PushMaterial.\_eventInfo

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:770

___

### \_globalAmbientColor

• `Private` **\_globalAmbientColor**: [`Color3`](Color3.md)

Sets the global ambient color for the material used in lighting calculations.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:808

___

### \_imageProcessingConfiguration

• `Protected` **\_imageProcessingConfiguration**: [`ImageProcessingConfiguration`](ImageProcessingConfiguration.md)

Default configuration related to image processing available in the PBR Material.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:764

___

### \_imageProcessingObserver

• `Private` **\_imageProcessingObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`ImageProcessingConfiguration`](ImageProcessingConfiguration.md) = `null`

Keep track of the image processing observer to allow dispose and replace.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:769

___

### \_lightingInfos

• `Private` **\_lightingInfos**: [`Vector4`](Vector4.md)

This stores the direct, emissive, environment, and specular light intensities into a Vector4.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:351

___

### \_needToBindSceneUbo

• `Protected` **\_needToBindSceneUbo**: `boolean`

#### Inherited from

PushMaterial.\_needToBindSceneUbo

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:727

___

### \_normalMatrix

• `Protected` **\_normalMatrix**: [`Matrix`](Matrix.md)

#### Inherited from

PushMaterial.\_normalMatrix

#### Defined in

https://github.com/babylon.js/core/src/Materials/pushMaterial.ts:16

___

### \_onEffectCreatedObservable

• `Protected` **\_onEffectCreatedObservable**: [`Nullable`](../modules.md#nullable)[`Observable`](Observable.md){ `effect`: [`Effect`](Effect.md) ; `subMesh`: [`Nullable`](../modules.md#nullable)[`SubMesh`](SubMesh.md)  }

#### Inherited from

PushMaterial.\_onEffectCreatedObservable

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:477

___

### \_realTimeFiltering

• `Private` **\_realTimeFiltering**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:715

___

### \_realTimeFilteringQuality

• `Private` **\_realTimeFilteringQuality**: `number` = `Constants.TEXTURE_FILTERING_QUALITY_LOW`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:727

___

### \_renderTargets

• `Private` **\_renderTargets**: [`SmartArray`](SmartArray.md)[`RenderTargetTexture`](RenderTargetTexture.md)

Stores the available render targets.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:803

___

### \_transparencyMode

• `Protected` **\_transparencyMode**: [`Nullable`](../modules.md#nullable)`number` = `null`

The transparency mode of the material.

#### Inherited from

PushMaterial.\_transparencyMode

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:959

___

### \_unlit

• `Private` **\_unlit**: `boolean` = `false`

If set to true, no lighting calculations will be applied.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:818

___

### \_useLogarithmicDepth

• `Private` **\_useLogarithmicDepth**: `boolean` = `false`

Enables the use of logarithmic depth buffers, which is good for wide depth buffers.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:813

___

### allowShaderHotSwapping

• **allowShaderHotSwapping**: `boolean` = `true`

Gets or sets a boolean indicating that the material is allowed (if supported) to do shader hot swapping.
This means that the material can keep using a previous shader while a new one is being compiled.
This is mostly used when shader parallel compilation is supported (true by default)

#### Inherited from

PushMaterial.allowShaderHotSwapping

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:227

___

### animations

• **animations**: [`Nullable`](../modules.md#nullable)[`Animation`](Animation.md)[] = `null`

Stores the animations for the material

#### Inherited from

PushMaterial.animations

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:415

___

### anisotropy

• `Readonly` **anisotropy**: [`PBRAnisotropicConfiguration`](PBRAnisotropicConfiguration.md)

Defines the anisotropic parameters for the material.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:861

___

### brdf

• `Readonly` **brdf**: `PBRBRDFConfiguration`

Defines the BRDF parameters for the material.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:866

___

### checkReadyOnEveryCall

• **checkReadyOnEveryCall**: `boolean` = `false`

Specifies if the ready state should be checked on each call

#### Inherited from

PushMaterial.checkReadyOnEveryCall

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:265

___

### checkReadyOnlyOnce

• **checkReadyOnlyOnce**: `boolean` = `false`

Specifies if the ready state should be checked once

#### Inherited from

PushMaterial.checkReadyOnlyOnce

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:271

___

### clearCoat

• `Readonly` **clearCoat**: [`PBRClearCoatConfiguration`](PBRClearCoatConfiguration.md)

Defines the clear coat layer parameters for the material.

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

PushMaterial.customShaderNameResolve

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:207

___

### depthFunction

• **depthFunction**: `number` = `0`

Specifies the depth function that should be used. 0 means the default engine function

#### Inherited from

PushMaterial.depthFunction

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:584

___

### detailMap

• `Readonly` **detailMap**: [`DetailMapConfiguration`](DetailMapConfiguration.md)

Defines the detail map parameters for the material.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:886

___

### disableColorWrite

• **disableColorWrite**: `boolean` = `false`

Specifies if color writing should be disabled

#### Inherited from

PushMaterial.disableColorWrite

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:572

___

### disableDepthWrite

• **disableDepthWrite**: `boolean` = `false`

Specifies if depth writing should be disabled

#### Inherited from

PushMaterial.disableDepthWrite

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:566

___

### doNotSerialize

• **doNotSerialize**: `boolean` = `false`

Specifies if the material should be serialized

#### Inherited from

PushMaterial.doNotSerialize

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:405

___

### forceDepthWrite

• **forceDepthWrite**: `boolean` = `false`

Specifies if depth writing should be forced

#### Inherited from

PushMaterial.forceDepthWrite

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:578

___

### getRenderTargetTextures

• **getRenderTargetTextures**: [`Nullable`](../modules.md#nullable)() => [`SmartArray`](SmartArray.md)[`RenderTargetTexture`](RenderTargetTexture.md) = `null`

Callback triggered to get the render target textures

#### Inherited from

PushMaterial.getRenderTargetTextures

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:391

___

### id

• **id**: `string`

The ID of the material

#### Inherited from

PushMaterial.id

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:233

___

### inspectableCustomProperties

• **inspectableCustomProperties**: [`IInspectable`](../interfaces/IInspectable.md)[]

List of inspectable custom properties (used by the Inspector)

**`See`**

https://doc.babylonjs.com/how_to/debug_layer#extensibility

#### Inherited from

PushMaterial.inspectableCustomProperties

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:298

___

### iridescence

• `Readonly` **iridescence**: [`PBRIridescenceConfiguration`](PBRIridescenceConfiguration.md)

Defines the iridescence layer parameters for the material.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:856

___

### metadata

• **metadata**: `any` = `null`

Gets or sets user defined metadata

#### Inherited from

PushMaterial.metadata

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:254

___

### name

• **name**: `string`

The name of the material

#### Inherited from

PushMaterial.name

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:248

___

### onCompiled

• **onCompiled**: [`Nullable`](../modules.md#nullable)(`effect`: [`Effect`](Effect.md)) => `void` = `null`

Callback triggered when the material is compiled

#### Inherited from

PushMaterial.onCompiled

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:381

___

### onDisposeObservable

• **onDisposeObservable**: [`Observable`](Observable.md)[`Material`](Material.md)

An event triggered when the material is disposed

#### Inherited from

PushMaterial.onDisposeObservable

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:420

___

### onError

• **onError**: [`Nullable`](../modules.md#nullable)(`effect`: [`Effect`](Effect.md), `errors`: `string`) => `void` = `null`

Callback triggered when an error occurs

#### Inherited from

PushMaterial.onError

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:386

___

### pluginManager

• `Optional` **pluginManager**: [`MaterialPluginManager`](MaterialPluginManager.md)

Plugin manager for this material

#### Inherited from

PushMaterial.pluginManager

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginManager.ts:30

___

### pointSize

• **pointSize**: `number` = `1.0`

Stores the size of points

#### Inherited from

PushMaterial.pointSize

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:620

___

### prePassConfiguration

• `Readonly` **prePassConfiguration**: `PrePassConfiguration`

Defines additional PrePass parameters for the material.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:881

___

### reservedDataStore

• **reservedDataStore**: `any` = `null`

For internal use only. Please do not use.

#### Inherited from

PushMaterial.reservedDataStore

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:259

___

### separateCullingPass

• **separateCullingPass**: `boolean` = `false`

Specifies if there should be a separate pass for culling

#### Inherited from

PushMaterial.separateCullingPass

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:590

___

### shadowDepthWrapper

• **shadowDepthWrapper**: [`Nullable`](../modules.md#nullable)[`ShadowDepthWrapper`](ShadowDepthWrapper.md) = `null`

Custom shadow depth material to use for shadow rendering instead of the in-built one

#### Inherited from

PushMaterial.shadowDepthWrapper

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:220

___

### sheen

• `Readonly` **sheen**: [`PBRSheenConfiguration`](PBRSheenConfiguration.md)

Defines the Sheen parameters for the material.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:871

___

### sideOrientation

• **sideOrientation**: `number`

Stores the value for side orientation

#### Inherited from

PushMaterial.sideOrientation

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:376

___

### state

• **state**: `string` = `""`

The state of the material

#### Inherited from

PushMaterial.state

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:277

___

### stencil

• `Readonly` **stencil**: `MaterialStencilState`

Gives access to the stencil properties of the material

#### Inherited from

PushMaterial.stencil

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:697

___

### subSurface

• `Readonly` **subSurface**: [`PBRSubSurfaceConfiguration`](PBRSubSurfaceConfiguration.md)

Defines the SubSurface parameters for the material.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:876

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the material

#### Inherited from

PushMaterial.uniqueId

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:239

___

### zOffset

• **zOffset**: `number` = `0`

Stores the z offset Factor value

#### Inherited from

PushMaterial.zOffset

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:626

___

### zOffsetUnits

• **zOffsetUnits**: `number` = `0`

Stores the z offset Units value

#### Inherited from

PushMaterial.zOffsetUnits

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:632

___

### AllDirtyFlag

▪ `Static` `Readonly` **AllDirtyFlag**: ``63``

The all dirty flag value

#### Inherited from

PushMaterial.AllDirtyFlag

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:164

___

### AttributesDirtyFlag

▪ `Static` `Readonly` **AttributesDirtyFlag**: ``8``

The dirty attribute flag value

#### Inherited from

PushMaterial.AttributesDirtyFlag

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:149

___

### ClockWiseSideOrientation

▪ `Static` `Readonly` **ClockWiseSideOrientation**: ``0``

Stores the clock-wise side orientation

#### Inherited from

PushMaterial.ClockWiseSideOrientation

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:124

___

### CounterClockWiseSideOrientation

▪ `Static` `Readonly` **CounterClockWiseSideOrientation**: ``1``

Stores the counter clock-wise side orientation

#### Inherited from

PushMaterial.CounterClockWiseSideOrientation

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:129

___

### DEFAULT\_AO\_ON\_ANALYTICAL\_LIGHTS

▪ `Static` **DEFAULT\_AO\_ON\_ANALYTICAL\_LIGHTS**: `number` = `0`

Defines the default value of how much AO map is occluding the analytical lights
(point spot...).

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:301

___

### FresnelDirtyFlag

▪ `Static` `Readonly` **FresnelDirtyFlag**: ``4``

The dirty fresnel flag value

#### Inherited from

PushMaterial.FresnelDirtyFlag

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:144

___

### LIGHTFALLOFF\_GLTF

▪ `Static` `Readonly` **LIGHTFALLOFF\_GLTF**: ``1``

PBRMaterialLightFalloff gltf: light is falling off as described in the gltf moving to PBR document
to enhance interoperability with other engines.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:312

___

### LIGHTFALLOFF\_PHYSICAL

▪ `Static` `Readonly` **LIGHTFALLOFF\_PHYSICAL**: ``0``

PBRMaterialLightFalloff Physical: light is falling off following the inverse squared distance law.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:306

___

### LIGHTFALLOFF\_STANDARD

▪ `Static` `Readonly` **LIGHTFALLOFF\_STANDARD**: ``2``

PBRMaterialLightFalloff Standard: light is falling off like in the standard material
to enhance interoperability with other materials.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:318

___

### LightDirtyFlag

▪ `Static` `Readonly` **LightDirtyFlag**: ``2``

The dirty light flag value

#### Inherited from

PushMaterial.LightDirtyFlag

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:139

___

### LineListDrawMode

▪ `Static` `Readonly` **LineListDrawMode**: ``4``

Returns the line list draw mode

#### Inherited from

PushMaterial.LineListDrawMode

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:103

___

### LineLoopDrawMode

▪ `Static` `Readonly` **LineLoopDrawMode**: ``5``

Returns the line loop draw mode

#### Inherited from

PushMaterial.LineLoopDrawMode

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:107

___

### LineStripDrawMode

▪ `Static` `Readonly` **LineStripDrawMode**: ``6``

Returns the line strip draw mode

#### Inherited from

PushMaterial.LineStripDrawMode

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:111

___

### MATERIAL\_ALPHABLEND

▪ `Static` `Readonly` **MATERIAL\_ALPHABLEND**: ``2``

MaterialTransparencyMode: Pixels are blended (according to the alpha mode) with the already drawn pixels in the current frame buffer.

#### Inherited from

PushMaterial.MATERIAL\_ALPHABLEND

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:179

___

### MATERIAL\_ALPHATEST

▪ `Static` `Readonly` **MATERIAL\_ALPHATEST**: ``1``

MaterialTransparencyMode: Alpha Test mode, pixel are discarded below a certain threshold defined by the alpha cutoff value.

#### Inherited from

PushMaterial.MATERIAL\_ALPHATEST

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:174

___

### MATERIAL\_ALPHATESTANDBLEND

▪ `Static` `Readonly` **MATERIAL\_ALPHATESTANDBLEND**: ``3``

MaterialTransparencyMode: Pixels are blended (according to the alpha mode) with the already drawn pixels in the current frame buffer.
They are also discarded below the alpha cutoff threshold to improve performances.

#### Inherited from

PushMaterial.MATERIAL\_ALPHATESTANDBLEND

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:185

___

### MATERIAL\_NORMALBLENDMETHOD\_RNM

▪ `Static` `Readonly` **MATERIAL\_NORMALBLENDMETHOD\_RNM**: ``1``

The Reoriented Normal Mapping method is used to blend normals.
Details of the algorithm can be found here: https://blog.selfshadow.com/publications/blending-in-detail/

#### Inherited from

PushMaterial.MATERIAL\_NORMALBLENDMETHOD\_RNM

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:197

___

### MATERIAL\_NORMALBLENDMETHOD\_WHITEOUT

▪ `Static` `Readonly` **MATERIAL\_NORMALBLENDMETHOD\_WHITEOUT**: ``0``

The Whiteout method is used to blend normals.
Details of the algorithm can be found here: https://blog.selfshadow.com/publications/blending-in-detail/

#### Inherited from

PushMaterial.MATERIAL\_NORMALBLENDMETHOD\_WHITEOUT

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:191

___

### MATERIAL\_OPAQUE

▪ `Static` `Readonly` **MATERIAL\_OPAQUE**: ``0``

MaterialTransparencyMode: No transparency mode, Alpha channel is not use.

#### Inherited from

PushMaterial.MATERIAL\_OPAQUE

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:169

___

### MiscDirtyFlag

▪ `Static` `Readonly` **MiscDirtyFlag**: ``16``

The dirty misc flag value

#### Inherited from

PushMaterial.MiscDirtyFlag

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:154

___

### OnEventObservable

▪ `Static` **OnEventObservable**: [`Observable`](Observable.md)[`Material`](Material.md)

Event observable which raises global events common to all materials (like MaterialPluginEvent.Created)

#### Inherited from

PushMaterial.OnEventObservable

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:202

___

### PBRMATERIAL\_ALPHABLEND

▪ `Static` `Readonly` **PBRMATERIAL\_ALPHABLEND**: ``2``

PBRMaterialTransparencyMode: Pixels are blended (according to the alpha mode) with the already drawn pixels in the current frame buffer.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:289

___

### PBRMATERIAL\_ALPHATEST

▪ `Static` `Readonly` **PBRMATERIAL\_ALPHATEST**: ``1``

PBRMaterialTransparencyMode: Alpha Test mode, pixel are discarded below a certain threshold defined by the alpha cutoff value.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:284

___

### PBRMATERIAL\_ALPHATESTANDBLEND

▪ `Static` `Readonly` **PBRMATERIAL\_ALPHATESTANDBLEND**: ``3``

PBRMaterialTransparencyMode: Pixels are blended (according to the alpha mode) with the already drawn pixels in the current frame buffer.
They are also discarded below the alpha cutoff threshold to improve performances.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:295

___

### PBRMATERIAL\_OPAQUE

▪ `Static` `Readonly` **PBRMATERIAL\_OPAQUE**: ``0``

PBRMaterialTransparencyMode: No transparency mode, Alpha channel is not use.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:279

___

### PointFillMode

▪ `Static` `Readonly` **PointFillMode**: ``2``

Returns the point fill mode

#### Inherited from

PushMaterial.PointFillMode

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:95

___

### PointListDrawMode

▪ `Static` `Readonly` **PointListDrawMode**: ``3``

Returns the point list draw mode

#### Inherited from

PushMaterial.PointListDrawMode

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:99

___

### PrePassDirtyFlag

▪ `Static` `Readonly` **PrePassDirtyFlag**: ``32``

The dirty prepass flag value

#### Inherited from

PushMaterial.PrePassDirtyFlag

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:159

___

### TextureDirtyFlag

▪ `Static` `Readonly` **TextureDirtyFlag**: ``1``

The dirty texture flag value

#### Inherited from

PushMaterial.TextureDirtyFlag

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:134

___

### TriangleFanDrawMode

▪ `Static` `Readonly` **TriangleFanDrawMode**: ``8``

Returns the triangle fan draw mode

#### Inherited from

PushMaterial.TriangleFanDrawMode

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:119

___

### TriangleFillMode

▪ `Static` `Readonly` **TriangleFillMode**: ``0``

Returns the triangle fill mode

#### Inherited from

PushMaterial.TriangleFillMode

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:87

___

### TriangleStripDrawMode

▪ `Static` `Readonly` **TriangleStripDrawMode**: ``7``

Returns the triangle strip draw mode

#### Inherited from

PushMaterial.TriangleStripDrawMode

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:115

___

### WireFrameFillMode

▪ `Static` `Readonly` **WireFrameFillMode**: ``1``

Returns the wireframe mode

#### Inherited from

PushMaterial.WireFrameFillMode

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:91

## Accessors

### \_disableAlphaBlending

• `Protected` `get` **_disableAlphaBlending**(): `boolean`

Returns true if alpha blending should be disabled.

#### Returns

`boolean`

#### Overrides

PushMaterial.\_disableAlphaBlending

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:970

___

### alpha

• `get` **alpha**(): `number`

Gets the alpha value of the material

#### Returns

`number`

#### Inherited from

PushMaterial.alpha

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

PushMaterial.alpha

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:303

___

### alphaMode

• `get` **alphaMode**(): `number`

Gets the value of the alpha mode

#### Returns

`number`

#### Inherited from

PushMaterial.alphaMode

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

PushMaterial.alphaMode

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:514

___

### backFaceCulling

• `get` **backFaceCulling**(): `boolean`

Gets the culling state

#### Returns

`boolean`

#### Inherited from

PushMaterial.backFaceCulling

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

PushMaterial.backFaceCulling

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:333

___

### canRenderToMRT

• `get` **canRenderToMRT**(): `boolean`

Can this material render to several textures at once

#### Returns

`boolean`

#### Overrides

PushMaterial.canRenderToMRT

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:742

___

### cullBackFaces

• `get` **cullBackFaces**(): `boolean`

Gets the type of faces that should be culled

#### Returns

`boolean`

#### Inherited from

PushMaterial.cullBackFaces

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

PushMaterial.cullBackFaces

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:357

___

### fillMode

• `get` **fillMode**(): `number`

Gets the material fill mode

#### Returns

`number`

#### Inherited from

PushMaterial.fillMode

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

PushMaterial.fillMode

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:685

___

### fogEnabled

• `get` **fogEnabled**(): `boolean`

Gets the value of the fog enabled state

#### Returns

`boolean`

#### Inherited from

PushMaterial.fogEnabled

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

PushMaterial.fogEnabled

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:601

___

### hasRenderTargetTextures

• `get` **hasRenderTargetTextures**(): `boolean`

Gets a boolean indicating that current material needs to register RTT

#### Returns

`boolean`

#### Overrides

PushMaterial.hasRenderTargetTextures

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:930

___

### isFrozen

• `get` **isFrozen**(): `boolean`

Specifies if updates for the material been locked

#### Returns

`boolean`

#### Inherited from

PushMaterial.isFrozen

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:883

___

### isPrePassCapable

• `get` **isPrePassCapable**(): `boolean`

Can this material render to prepass

#### Returns

`boolean`

#### Overrides

PushMaterial.isPrePassCapable

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:941

___

### needDepthPrePass

• `get` **needDepthPrePass**(): `boolean`

Gets the depth pre-pass value

#### Returns

`boolean`

#### Inherited from

PushMaterial.needDepthPrePass

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

PushMaterial.needDepthPrePass

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

PushMaterial.onBind

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:459

___

### onBindObservable

• `get` **onBindObservable**(): [`Observable`](Observable.md)[`AbstractMesh`](AbstractMesh.md)

An event triggered when the material is bound

#### Returns

[`Observable`](Observable.md)[`AbstractMesh`](AbstractMesh.md)

#### Inherited from

PushMaterial.onBindObservable

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

PushMaterial.onDispose

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:431

___

### onEffectCreatedObservable

• `get` **onEffectCreatedObservable**(): [`Observable`](Observable.md){ `effect`: [`Effect`](Effect.md) ; `subMesh`: [`Nullable`](../modules.md#nullable)[`SubMesh`](SubMesh.md)  }

An event triggered when the effect is (re)created

#### Returns

[`Observable`](Observable.md){ `effect`: [`Effect`](Effect.md) ; `subMesh`: [`Nullable`](../modules.md#nullable)[`SubMesh`](SubMesh.md)  }

#### Inherited from

PushMaterial.onEffectCreatedObservable

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:482

___

### onUnBindObservable

• `get` **onUnBindObservable**(): [`Observable`](Observable.md)[`Material`](Material.md)

An event triggered when the material is unbound

#### Returns

[`Observable`](Observable.md)[`Material`](Material.md)

#### Inherited from

PushMaterial.onUnBindObservable

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:469

___

### pointsCloud

• `get` **pointsCloud**(): `boolean`

Gets the value specifying if point clouds are enabled

#### Returns

`boolean`

#### Inherited from

PushMaterial.pointsCloud

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

PushMaterial.pointsCloud

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:670

___

### realTimeFiltering

• `get` **realTimeFiltering**(): `boolean`

Enables realtime filtering on the texture.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:719

• `set` **realTimeFiltering**(`b`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `b` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:722

___

### realTimeFilteringQuality

• `get` **realTimeFilteringQuality**(): `number`

Quality switch for realtime filtering

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:731

• `set` **realTimeFilteringQuality**(`n`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `n` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:734

___

### transparencyMode

• `get` **transparencyMode**(): [`Nullable`](../modules.md#nullable)`number`

Gets the current transparency mode.

#### Returns

[`Nullable`](../modules.md#nullable)`number`

#### Inherited from

PushMaterial.transparencyMode

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

PushMaterial.transparencyMode

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:980

___

### useLogarithmicDepth

• `get` **useLogarithmicDepth**(): `boolean`

Enabled the use of logarithmic depth buffers, which is good for wide depth buffers.

#### Returns

`boolean`

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:963

___

### wireframe

• `get` **wireframe**(): `boolean`

#### Returns

`boolean`

#### Inherited from

PushMaterial.wireframe

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

PushMaterial.wireframe

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

PushMaterial.\_afterBind

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:775

___

### \_getReflectionTexture

▸ `Private` **_getReflectionTexture**(): [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Returns the texture used for reflections.

#### Returns

[`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

- Reflection texture if present.  Otherwise, returns the environment texture.

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:2352

___

### \_hasAlphaChannel

▸ `Protected` **_hasAlphaChannel**(): `boolean`

Specifies whether or not there is a usable alpha channel for transparency.

#### Returns

`boolean`

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

PushMaterial.\_isReadyForSubMesh

#### Defined in

https://github.com/babylon.js/core/src/Materials/pushMaterial.ts:43

___

### \_markAllSubMeshesAsAllDirty

▸ `Protected` **_markAllSubMeshesAsAllDirty**(): `void`

Indicates that we need to re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

PushMaterial.\_markAllSubMeshesAsAllDirty

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1543

___

### \_markAllSubMeshesAsAttributesDirty

▸ `Protected` **_markAllSubMeshesAsAttributesDirty**(): `void`

Indicates that attributes need to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

PushMaterial.\_markAllSubMeshesAsAttributesDirty

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

PushMaterial.\_markAllSubMeshesAsDirty

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1498

___

### \_markAllSubMeshesAsFresnelAndMiscDirty

▸ `Protected` **_markAllSubMeshesAsFresnelAndMiscDirty**(): `void`

Indicates that fresnel and misc need to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

PushMaterial.\_markAllSubMeshesAsFresnelAndMiscDirty

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1571

___

### \_markAllSubMeshesAsFresnelDirty

▸ `Protected` **_markAllSubMeshesAsFresnelDirty**(): `void`

Indicates that fresnel needs to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

PushMaterial.\_markAllSubMeshesAsFresnelDirty

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1564

___

### \_markAllSubMeshesAsImageProcessingDirty

▸ `Protected` **_markAllSubMeshesAsImageProcessingDirty**(): `void`

Indicates that image processing needs to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

PushMaterial.\_markAllSubMeshesAsImageProcessingDirty

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1550

___

### \_markAllSubMeshesAsLightsDirty

▸ `Protected` **_markAllSubMeshesAsLightsDirty**(): `void`

Indicates that lights need to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

PushMaterial.\_markAllSubMeshesAsLightsDirty

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1578

___

### \_markAllSubMeshesAsMiscDirty

▸ `Protected` **_markAllSubMeshesAsMiscDirty**(): `void`

Indicates that misc needs to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

PushMaterial.\_markAllSubMeshesAsMiscDirty

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1592

___

### \_markAllSubMeshesAsPrePassDirty

▸ `Protected` **_markAllSubMeshesAsPrePassDirty**(): `void`

Indicates that prepass needs to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

PushMaterial.\_markAllSubMeshesAsPrePassDirty

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1599

___

### \_markAllSubMeshesAsTexturesAndMiscDirty

▸ `Protected` **_markAllSubMeshesAsTexturesAndMiscDirty**(): `void`

Indicates that textures and misc need to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

PushMaterial.\_markAllSubMeshesAsTexturesAndMiscDirty

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1606

___

### \_markAllSubMeshesAsTexturesDirty

▸ `Protected` **_markAllSubMeshesAsTexturesDirty**(): `void`

Indicates that textures need to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

PushMaterial.\_markAllSubMeshesAsTexturesDirty

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1557

___

### \_markScenePrePassDirty

▸ `Protected` **_markScenePrePassDirty**(): `void`

Indicates that the scene should check if the rendering now needs a prepass

#### Returns

`void`

#### Inherited from

PushMaterial.\_markScenePrePassDirty

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

PushMaterial.\_mustRebind

#### Defined in

https://github.com/babylon.js/core/src/Materials/pushMaterial.ts:85

___

### \_prepareDefines

▸ `Private` **_prepareDefines**(`mesh`, `defines`, `useInstances?`, `useClipPlane?`, `useThinInstances?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | `undefined` |
| `defines` | `PBRMaterialDefines` | `undefined` |
| `useInstances` | [`Nullable`](../modules.md#nullable)`boolean` | `null` |
| `useClipPlane` | [`Nullable`](../modules.md#nullable)`boolean` | `null` |
| `useThinInstances` | `boolean` | `false` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:1503

___

### \_prepareEffect

▸ `Private` **_prepareEffect**(`mesh`, `defines`, `onCompiled?`, `onError?`, `useInstances?`, `useClipPlane?`, `useThinInstances`): [`Nullable`](../modules.md#nullable)[`Effect`](Effect.md)

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | `undefined` |
| `defines` | `PBRMaterialDefines` | `undefined` |
| `onCompiled` | [`Nullable`](../modules.md#nullable)(`effect`: [`Effect`](Effect.md)) => `void` | `null` |
| `onError` | [`Nullable`](../modules.md#nullable)(`effect`: [`Effect`](Effect.md), `errors`: `string`) => `void` | `null` |
| `useInstances` | [`Nullable`](../modules.md#nullable)`boolean` | `null` |
| `useClipPlane` | [`Nullable`](../modules.md#nullable)`boolean` | `null` |
| `useThinInstances` | `boolean` | `undefined` |

#### Returns

[`Nullable`](../modules.md#nullable)[`Effect`](Effect.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:1216

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

https://github.com/babylon.js/core/src/Materials/material.ts:1040

___

### \_shouldUseAlphaFromAlbedoTexture

▸ `Protected` **_shouldUseAlphaFromAlbedoTexture**(): `boolean`

Specifies whether or not the alpha value of the albedo texture should be used for alpha blending.

#### Returns

`boolean`

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

PushMaterial.bind

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

PushMaterial.bindEyePosition

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

#### Overrides

PushMaterial.bindForSubMesh

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

PushMaterial.bindOnlyNormalMatrix

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

PushMaterial.bindOnlyWorldMatrix

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

PushMaterial.bindView

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

PushMaterial.bindViewProjection

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1154

___

### buildUniformLayout

▸ **buildUniformLayout**(): `void`

Initializes the uniform buffer layout for the shader.

#### Returns

`void`

#### Overrides

PushMaterial.buildUniformLayout

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

PushMaterial.clone

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

#### Overrides

PushMaterial.dispose

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

#### Overrides

PushMaterial.forceCompilation

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

PushMaterial.forceCompilationAsync

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1392

___

### freeze

▸ **freeze**(): `void`

Locks updates for the material

#### Returns

`void`

#### Inherited from

PushMaterial.freeze

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:890

___

### getActiveTextures

▸ **getActiveTextures**(): [`BaseTexture`](BaseTexture.md)[]

Returns an array of the actively used textures.

#### Returns

[`BaseTexture`](BaseTexture.md)[]

- Array of BaseTextures

#### Overrides

PushMaterial.getActiveTextures

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:2364

___

### getAlphaTestTexture

▸ **getAlphaTestTexture**(): [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Gets the texture used for the alpha test.

#### Returns

[`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

#### Overrides

PushMaterial.getAlphaTestTexture

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:1021

___

### getAnimatables

▸ **getAnimatables**(): [`IAnimatable`](../interfaces/IAnimatable.md)[]

Returns the animatable textures.

#### Returns

[`IAnimatable`](../interfaces/IAnimatable.md)[]

- Array of animatable textures.

#### Overrides

PushMaterial.getAnimatables

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

PushMaterial.getBindedMeshes

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1289

___

### getClassName

▸ **getClassName**(): `string`

Gets the name of the material class.

#### Returns

`string`

#### Overrides

PushMaterial.getClassName

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:948

___

### getEffect

▸ **getEffect**(): [`Effect`](Effect.md)

#### Returns

[`Effect`](Effect.md)

#### Inherited from

PushMaterial.getEffect

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

PushMaterial.getScene

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

#### Overrides

PushMaterial.hasTexture

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:2423

___

### isMetallicWorkflow

▸ **isMetallicWorkflow**(): `boolean`

Specifies if the material uses metallic roughness workflow.

#### Returns

`boolean`

boolean specifying if the material uses metallic roughness workflow.

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

PushMaterial.isReady

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

#### Overrides

PushMaterial.isReadyForSubMesh

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

PushMaterial.markAsDirty

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1437

___

### markDirty

▸ **markDirty**(): `void`

Marks the material to indicate that it needs to be re-calculated

#### Returns

`void`

#### Inherited from

PushMaterial.markDirty

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1055

___

### needAlphaBlending

▸ **needAlphaBlending**(): `boolean`

Specifies whether or not this material should be rendered in alpha blend mode.

#### Returns

`boolean`

#### Overrides

PushMaterial.needAlphaBlending

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

PushMaterial.needAlphaBlendingForMesh

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1016

___

### needAlphaTesting

▸ **needAlphaTesting**(): `boolean`

Specifies whether or not this material should be rendered in alpha test mode.

#### Returns

`boolean`

#### Overrides

PushMaterial.needAlphaTesting

#### Defined in

https://github.com/babylon.js/core/src/Materials/PBR/pbrBaseMaterial.ts:992

___

### resetDrawCache

▸ **resetDrawCache**(): `void`

Resets the draw wrappers cache for all submeshes that are using this material

#### Returns

`void`

#### Inherited from

PushMaterial.resetDrawCache

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

PushMaterial.serialize

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1724

___

### setPrePassRenderer

▸ **setPrePassRenderer**(): `boolean`

Sets the required values to the prepass renderer.

#### Returns

`boolean`

#### Overrides

PushMaterial.setPrePassRenderer

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

PushMaterial.toString

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:867

___

### unbind

▸ **unbind**(): `void`

Unbinds the material from the mesh

#### Returns

`void`

#### Inherited from

PushMaterial.unbind

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1222

___

### unfreeze

▸ **unfreeze**(): `void`

Unlocks updates for the material

#### Returns

`void`

#### Inherited from

PushMaterial.unfreeze

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

PushMaterial.Parse

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1739
