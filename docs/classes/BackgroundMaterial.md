[@dev/core](../README.md) / [Exports](../modules.md) / BackgroundMaterial

# Class: BackgroundMaterial

Background material used to create an efficient environment around your scene.

## Hierarchy

- `PushMaterial`

  ↳ **`BackgroundMaterial`**

## Table of contents

### Constructors

- [constructor](BackgroundMaterial.md#constructor)

### Properties

- [\_\_perceptualColor](BackgroundMaterial.md#__perceptualcolor)
- [\_activeEffect](BackgroundMaterial.md#_activeeffect)
- [\_alpha](BackgroundMaterial.md#_alpha)
- [\_backFaceCulling](BackgroundMaterial.md#_backfaceculling)
- [\_cullBackFaces](BackgroundMaterial.md#_cullbackfaces)
- [\_diffuseTexture](BackgroundMaterial.md#_diffusetexture)
- [\_drawWrapper](BackgroundMaterial.md#_drawwrapper)
- [\_enableNoise](BackgroundMaterial.md#_enablenoise)
- [\_eventInfo](BackgroundMaterial.md#_eventinfo)
- [\_forceAlphaTest](BackgroundMaterial.md#_forcealphatest)
- [\_fovMultiplier](BackgroundMaterial.md#_fovmultiplier)
- [\_imageProcessingConfiguration](BackgroundMaterial.md#_imageprocessingconfiguration)
- [\_imageProcessingObserver](BackgroundMaterial.md#_imageprocessingobserver)
- [\_maxSimultaneousLights](BackgroundMaterial.md#_maxsimultaneouslights)
- [\_needToBindSceneUbo](BackgroundMaterial.md#_needtobindsceneubo)
- [\_normalMatrix](BackgroundMaterial.md#_normalmatrix)
- [\_onEffectCreatedObservable](BackgroundMaterial.md#_oneffectcreatedobservable)
- [\_opacityFresnel](BackgroundMaterial.md#_opacityfresnel)
- [\_primaryColor](BackgroundMaterial.md#_primarycolor)
- [\_primaryColorHighlightLevel](BackgroundMaterial.md#_primarycolorhighlightlevel)
- [\_primaryColorShadowLevel](BackgroundMaterial.md#_primarycolorshadowlevel)
- [\_primaryHighlightColor](BackgroundMaterial.md#_primaryhighlightcolor)
- [\_primaryShadowColor](BackgroundMaterial.md#_primaryshadowcolor)
- [\_reflectionAmount](BackgroundMaterial.md#_reflectionamount)
- [\_reflectionBlur](BackgroundMaterial.md#_reflectionblur)
- [\_reflectionControls](BackgroundMaterial.md#_reflectioncontrols)
- [\_reflectionFalloffDistance](BackgroundMaterial.md#_reflectionfalloffdistance)
- [\_reflectionFresnel](BackgroundMaterial.md#_reflectionfresnel)
- [\_reflectionReflectance0](BackgroundMaterial.md#_reflectionreflectance0)
- [\_reflectionReflectance90](BackgroundMaterial.md#_reflectionreflectance90)
- [\_reflectionTexture](BackgroundMaterial.md#_reflectiontexture)
- [\_renderTargets](BackgroundMaterial.md#_rendertargets)
- [\_sceneCenter](BackgroundMaterial.md#_scenecenter)
- [\_shadowLevel](BackgroundMaterial.md#_shadowlevel)
- [\_shadowLights](BackgroundMaterial.md#_shadowlights)
- [\_shadowOnly](BackgroundMaterial.md#_shadowonly)
- [\_transparencyMode](BackgroundMaterial.md#_transparencymode)
- [\_useRGBColor](BackgroundMaterial.md#_usergbcolor)
- [\_white](BackgroundMaterial.md#_white)
- [allowShaderHotSwapping](BackgroundMaterial.md#allowshaderhotswapping)
- [animations](BackgroundMaterial.md#animations)
- [checkReadyOnEveryCall](BackgroundMaterial.md#checkreadyoneverycall)
- [checkReadyOnlyOnce](BackgroundMaterial.md#checkreadyonlyonce)
- [customShaderNameResolve](BackgroundMaterial.md#customshadernameresolve)
- [depthFunction](BackgroundMaterial.md#depthfunction)
- [diffuseTexture](BackgroundMaterial.md#diffusetexture)
- [disableColorWrite](BackgroundMaterial.md#disablecolorwrite)
- [disableDepthWrite](BackgroundMaterial.md#disabledepthwrite)
- [doNotSerialize](BackgroundMaterial.md#donotserialize)
- [enableNoise](BackgroundMaterial.md#enablenoise)
- [forceDepthWrite](BackgroundMaterial.md#forcedepthwrite)
- [getRenderTargetTextures](BackgroundMaterial.md#getrendertargettextures)
- [id](BackgroundMaterial.md#id)
- [inspectableCustomProperties](BackgroundMaterial.md#inspectablecustomproperties)
- [maxSimultaneousLights](BackgroundMaterial.md#maxsimultaneouslights)
- [metadata](BackgroundMaterial.md#metadata)
- [name](BackgroundMaterial.md#name)
- [onCompiled](BackgroundMaterial.md#oncompiled)
- [onDisposeObservable](BackgroundMaterial.md#ondisposeobservable)
- [onError](BackgroundMaterial.md#onerror)
- [opacityFresnel](BackgroundMaterial.md#opacityfresnel)
- [pluginManager](BackgroundMaterial.md#pluginmanager)
- [pointSize](BackgroundMaterial.md#pointsize)
- [primaryColor](BackgroundMaterial.md#primarycolor)
- [reflectionAmount](BackgroundMaterial.md#reflectionamount)
- [reflectionBlur](BackgroundMaterial.md#reflectionblur)
- [reflectionFalloffDistance](BackgroundMaterial.md#reflectionfalloffdistance)
- [reflectionFresnel](BackgroundMaterial.md#reflectionfresnel)
- [reflectionReflectance0](BackgroundMaterial.md#reflectionreflectance0)
- [reflectionReflectance90](BackgroundMaterial.md#reflectionreflectance90)
- [reflectionTexture](BackgroundMaterial.md#reflectiontexture)
- [reservedDataStore](BackgroundMaterial.md#reserveddatastore)
- [sceneCenter](BackgroundMaterial.md#scenecenter)
- [separateCullingPass](BackgroundMaterial.md#separatecullingpass)
- [shadowDepthWrapper](BackgroundMaterial.md#shadowdepthwrapper)
- [shadowLevel](BackgroundMaterial.md#shadowlevel)
- [shadowLights](BackgroundMaterial.md#shadowlights)
- [shadowOnly](BackgroundMaterial.md#shadowonly)
- [sideOrientation](BackgroundMaterial.md#sideorientation)
- [state](BackgroundMaterial.md#state)
- [stencil](BackgroundMaterial.md#stencil)
- [switchToBGR](BackgroundMaterial.md#switchtobgr)
- [uniqueId](BackgroundMaterial.md#uniqueid)
- [useEquirectangularFOV](BackgroundMaterial.md#useequirectangularfov)
- [useRGBColor](BackgroundMaterial.md#usergbcolor)
- [zOffset](BackgroundMaterial.md#zoffset)
- [zOffsetUnits](BackgroundMaterial.md#zoffsetunits)
- [AllDirtyFlag](BackgroundMaterial.md#alldirtyflag)
- [AttributesDirtyFlag](BackgroundMaterial.md#attributesdirtyflag)
- [ClockWiseSideOrientation](BackgroundMaterial.md#clockwisesideorientation)
- [CounterClockWiseSideOrientation](BackgroundMaterial.md#counterclockwisesideorientation)
- [FresnelDirtyFlag](BackgroundMaterial.md#fresneldirtyflag)
- [LightDirtyFlag](BackgroundMaterial.md#lightdirtyflag)
- [LineListDrawMode](BackgroundMaterial.md#linelistdrawmode)
- [LineLoopDrawMode](BackgroundMaterial.md#lineloopdrawmode)
- [LineStripDrawMode](BackgroundMaterial.md#linestripdrawmode)
- [MATERIAL\_ALPHABLEND](BackgroundMaterial.md#material_alphablend)
- [MATERIAL\_ALPHATEST](BackgroundMaterial.md#material_alphatest)
- [MATERIAL\_ALPHATESTANDBLEND](BackgroundMaterial.md#material_alphatestandblend)
- [MATERIAL\_NORMALBLENDMETHOD\_RNM](BackgroundMaterial.md#material_normalblendmethod_rnm)
- [MATERIAL\_NORMALBLENDMETHOD\_WHITEOUT](BackgroundMaterial.md#material_normalblendmethod_whiteout)
- [MATERIAL\_OPAQUE](BackgroundMaterial.md#material_opaque)
- [MiscDirtyFlag](BackgroundMaterial.md#miscdirtyflag)
- [OnEventObservable](BackgroundMaterial.md#oneventobservable)
- [PointFillMode](BackgroundMaterial.md#pointfillmode)
- [PointListDrawMode](BackgroundMaterial.md#pointlistdrawmode)
- [PrePassDirtyFlag](BackgroundMaterial.md#prepassdirtyflag)
- [StandardReflectance0](BackgroundMaterial.md#standardreflectance0)
- [StandardReflectance90](BackgroundMaterial.md#standardreflectance90)
- [TextureDirtyFlag](BackgroundMaterial.md#texturedirtyflag)
- [TriangleFanDrawMode](BackgroundMaterial.md#trianglefandrawmode)
- [TriangleFillMode](BackgroundMaterial.md#trianglefillmode)
- [TriangleStripDrawMode](BackgroundMaterial.md#trianglestripdrawmode)
- [WireFrameFillMode](BackgroundMaterial.md#wireframefillmode)

### Accessors

- [\_disableAlphaBlending](BackgroundMaterial.md#_disablealphablending)
- [\_perceptualColor](BackgroundMaterial.md#_perceptualcolor)
- [alpha](BackgroundMaterial.md#alpha)
- [alphaMode](BackgroundMaterial.md#alphamode)
- [backFaceCulling](BackgroundMaterial.md#backfaceculling)
- [cameraColorCurves](BackgroundMaterial.md#cameracolorcurves)
- [cameraColorCurvesEnabled](BackgroundMaterial.md#cameracolorcurvesenabled)
- [cameraColorGradingEnabled](BackgroundMaterial.md#cameracolorgradingenabled)
- [cameraColorGradingTexture](BackgroundMaterial.md#cameracolorgradingtexture)
- [cameraContrast](BackgroundMaterial.md#cameracontrast)
- [cameraExposure](BackgroundMaterial.md#cameraexposure)
- [cameraToneMappingEnabled](BackgroundMaterial.md#cameratonemappingenabled)
- [canRenderToMRT](BackgroundMaterial.md#canrendertomrt)
- [cullBackFaces](BackgroundMaterial.md#cullbackfaces)
- [fillMode](BackgroundMaterial.md#fillmode)
- [fogEnabled](BackgroundMaterial.md#fogenabled)
- [fovMultiplier](BackgroundMaterial.md#fovmultiplier)
- [hasRenderTargetTextures](BackgroundMaterial.md#hasrendertargettextures)
- [imageProcessingConfiguration](BackgroundMaterial.md#imageprocessingconfiguration)
- [isFrozen](BackgroundMaterial.md#isfrozen)
- [isPrePassCapable](BackgroundMaterial.md#isprepasscapable)
- [needDepthPrePass](BackgroundMaterial.md#needdepthprepass)
- [onBind](BackgroundMaterial.md#onbind)
- [onBindObservable](BackgroundMaterial.md#onbindobservable)
- [onDispose](BackgroundMaterial.md#ondispose)
- [onEffectCreatedObservable](BackgroundMaterial.md#oneffectcreatedobservable)
- [onUnBindObservable](BackgroundMaterial.md#onunbindobservable)
- [pointsCloud](BackgroundMaterial.md#pointscloud)
- [primaryColorHighlightLevel](BackgroundMaterial.md#primarycolorhighlightlevel)
- [primaryColorShadowLevel](BackgroundMaterial.md#primarycolorshadowlevel)
- [reflectionStandardFresnelWeight](BackgroundMaterial.md#reflectionstandardfresnelweight)
- [transparencyMode](BackgroundMaterial.md#transparencymode)
- [wireframe](BackgroundMaterial.md#wireframe)

### Methods

- [\_afterBind](BackgroundMaterial.md#_afterbind)
- [\_attachImageProcessingConfiguration](BackgroundMaterial.md#_attachimageprocessingconfiguration)
- [\_computePrimaryColorFromPerceptualColor](BackgroundMaterial.md#_computeprimarycolorfromperceptualcolor)
- [\_computePrimaryColors](BackgroundMaterial.md#_computeprimarycolors)
- [\_isReadyForSubMesh](BackgroundMaterial.md#_isreadyforsubmesh)
- [\_markAllSubMeshesAsAllDirty](BackgroundMaterial.md#_markallsubmeshesasalldirty)
- [\_markAllSubMeshesAsAttributesDirty](BackgroundMaterial.md#_markallsubmeshesasattributesdirty)
- [\_markAllSubMeshesAsDirty](BackgroundMaterial.md#_markallsubmeshesasdirty)
- [\_markAllSubMeshesAsFresnelAndMiscDirty](BackgroundMaterial.md#_markallsubmeshesasfresnelandmiscdirty)
- [\_markAllSubMeshesAsFresnelDirty](BackgroundMaterial.md#_markallsubmeshesasfresneldirty)
- [\_markAllSubMeshesAsImageProcessingDirty](BackgroundMaterial.md#_markallsubmeshesasimageprocessingdirty)
- [\_markAllSubMeshesAsLightsDirty](BackgroundMaterial.md#_markallsubmeshesaslightsdirty)
- [\_markAllSubMeshesAsMiscDirty](BackgroundMaterial.md#_markallsubmeshesasmiscdirty)
- [\_markAllSubMeshesAsPrePassDirty](BackgroundMaterial.md#_markallsubmeshesasprepassdirty)
- [\_markAllSubMeshesAsTexturesAndMiscDirty](BackgroundMaterial.md#_markallsubmeshesastexturesandmiscdirty)
- [\_markAllSubMeshesAsTexturesDirty](BackgroundMaterial.md#_markallsubmeshesastexturesdirty)
- [\_markScenePrePassDirty](BackgroundMaterial.md#_marksceneprepassdirty)
- [\_mustRebind](BackgroundMaterial.md#_mustrebind)
- [\_shouldTurnAlphaTestOn](BackgroundMaterial.md#_shouldturnalphateston)
- [bind](BackgroundMaterial.md#bind)
- [bindEyePosition](BackgroundMaterial.md#bindeyeposition)
- [bindForSubMesh](BackgroundMaterial.md#bindforsubmesh)
- [bindOnlyNormalMatrix](BackgroundMaterial.md#bindonlynormalmatrix)
- [bindOnlyWorldMatrix](BackgroundMaterial.md#bindonlyworldmatrix)
- [bindView](BackgroundMaterial.md#bindview)
- [bindViewProjection](BackgroundMaterial.md#bindviewprojection)
- [buildUniformLayout](BackgroundMaterial.md#builduniformlayout)
- [clone](BackgroundMaterial.md#clone)
- [dispose](BackgroundMaterial.md#dispose)
- [forceCompilation](BackgroundMaterial.md#forcecompilation)
- [forceCompilationAsync](BackgroundMaterial.md#forcecompilationasync)
- [freeze](BackgroundMaterial.md#freeze)
- [getActiveTextures](BackgroundMaterial.md#getactivetextures)
- [getAlphaTestTexture](BackgroundMaterial.md#getalphatesttexture)
- [getAnimatables](BackgroundMaterial.md#getanimatables)
- [getBindedMeshes](BackgroundMaterial.md#getbindedmeshes)
- [getClassName](BackgroundMaterial.md#getclassname)
- [getEffect](BackgroundMaterial.md#geteffect)
- [getScene](BackgroundMaterial.md#getscene)
- [hasTexture](BackgroundMaterial.md#hastexture)
- [isReady](BackgroundMaterial.md#isready)
- [isReadyForSubMesh](BackgroundMaterial.md#isreadyforsubmesh)
- [markAsDirty](BackgroundMaterial.md#markasdirty)
- [markDirty](BackgroundMaterial.md#markdirty)
- [needAlphaBlending](BackgroundMaterial.md#needalphablending)
- [needAlphaBlendingForMesh](BackgroundMaterial.md#needalphablendingformesh)
- [needAlphaTesting](BackgroundMaterial.md#needalphatesting)
- [resetDrawCache](BackgroundMaterial.md#resetdrawcache)
- [serialize](BackgroundMaterial.md#serialize)
- [setPrePassRenderer](BackgroundMaterial.md#setprepassrenderer)
- [toString](BackgroundMaterial.md#tostring)
- [unbind](BackgroundMaterial.md#unbind)
- [unfreeze](BackgroundMaterial.md#unfreeze)
- [Parse](BackgroundMaterial.md#parse)

## Constructors

### constructor

• **new BackgroundMaterial**(`name`, `scene?`)

Instantiates a Background Material in the given scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | The friendly name of the material |
| `scene?` | [`Scene`](Scene.md) | The scene to add the material to |

#### Overrides

PushMaterial.constructor

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:622

## Properties

### \_\_perceptualColor

• `Protected` **\_\_perceptualColor**: [`Nullable`](../modules.md#nullable)[`Color3`](Color3.md)

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:214

___

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

### \_backFaceCulling

• `Protected` **\_backFaceCulling**: `boolean` = `true`

Specifies if back face culling is enabled

#### Inherited from

PushMaterial.\_backFaceCulling

#### Defined in

packages/dev/core/src/Materials/material.ts:328

___

### \_cullBackFaces

• `Protected` **\_cullBackFaces**: `boolean` = `true`

Specifies if back or front faces should be culled (when culling is enabled)

#### Inherited from

PushMaterial.\_cullBackFaces

#### Defined in

packages/dev/core/src/Materials/material.ts:352

___

### \_diffuseTexture

• `Protected` **\_diffuseTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:286

___

### \_drawWrapper

• `Protected` **\_drawWrapper**: `DrawWrapper`

#### Inherited from

PushMaterial.\_drawWrapper

#### Defined in

packages/dev/core/src/Materials/material.ts:705

___

### \_enableNoise

• `Protected` **\_enableNoise**: `boolean`

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:398

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

### \_fovMultiplier

• `Private` **\_fovMultiplier**: `number` = `1.0`

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:419

___

### \_imageProcessingConfiguration

• `Protected` **\_imageProcessingConfiguration**: [`ImageProcessingConfiguration`](ImageProcessingConfiguration.md)

Default configuration related to image processing available in the Background Material.

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:446

___

### \_imageProcessingObserver

• `Private` **\_imageProcessingObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`ImageProcessingConfiguration`](ImageProcessingConfiguration.md) = `null`

Keep track of the image processing observer to allow dispose and replace.

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:451

___

### \_maxSimultaneousLights

• `Private` **\_maxSimultaneousLights**: `number` = `4`

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:427

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

### \_opacityFresnel

• `Protected` **\_opacityFresnel**: `boolean`

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:321

___

### \_primaryColor

• `Protected` **\_primaryColor**: [`Color3`](Color3.md)

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:206

___

### \_primaryColorHighlightLevel

• `Protected` **\_primaryColorHighlightLevel**: `number` = `0`

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:250

___

### \_primaryColorShadowLevel

• `Protected` **\_primaryColorShadowLevel**: `number` = `0`

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:235

___

### \_primaryHighlightColor

• `Private` **\_primaryHighlightColor**: [`Color3`](Color3.md)

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:615

___

### \_primaryShadowColor

• `Private` **\_primaryShadowColor**: [`Color3`](Color3.md)

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:614

___

### \_reflectionAmount

• `Protected` **\_reflectionAmount**: `number`

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:348

___

### \_reflectionBlur

• `Protected` **\_reflectionBlur**: `number`

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:275

___

### \_reflectionControls

• `Private` **\_reflectionControls**: [`Vector4`](Vector4.md)

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:612

___

### \_reflectionFalloffDistance

• `Protected` **\_reflectionFalloffDistance**: `number`

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:339

___

### \_reflectionFresnel

• `Protected` **\_reflectionFresnel**: `boolean`

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:330

___

### \_reflectionReflectance0

• `Protected` **\_reflectionReflectance0**: `number`

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:356

___

### \_reflectionReflectance90

• `Protected` **\_reflectionReflectance90**: `number`

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:364

___

### \_reflectionTexture

• `Protected` **\_reflectionTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:266

___

### \_renderTargets

• `Private` **\_renderTargets**: [`SmartArray`](SmartArray.md)[`RenderTargetTexture`](RenderTargetTexture.md)

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:611

___

### \_sceneCenter

• `Protected` **\_sceneCenter**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:312

___

### \_shadowLevel

• `Protected` **\_shadowLevel**: `number`

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:303

___

### \_shadowLights

• `Protected` **\_shadowLights**: [`Nullable`](../modules.md#nullable)[`IShadowLight`](../interfaces/IShadowLight.md)[] = `null`

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:294

___

### \_shadowOnly

• `Private` **\_shadowOnly**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:435

___

### \_transparencyMode

• `Protected` **\_transparencyMode**: [`Nullable`](../modules.md#nullable)`number` = `null`

The transparency mode of the material.

#### Inherited from

PushMaterial.\_transparencyMode

#### Defined in

packages/dev/core/src/Materials/material.ts:959

___

### \_useRGBColor

• `Protected` **\_useRGBColor**: `boolean`

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:390

___

### \_white

• `Private` **\_white**: [`Color3`](Color3.md)

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:613

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

### animations

• **animations**: [`Nullable`](../modules.md#nullable)[`Animation`](Animation.md)[] = `null`

Stores the animations for the material

#### Inherited from

PushMaterial.animations

#### Defined in

packages/dev/core/src/Materials/material.ts:415

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

### diffuseTexture

• **diffuseTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) = `null`

Diffuse Texture used in the material.
Should be author in a specific way for the best result (refer to the documentation).

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:292

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

### doNotSerialize

• **doNotSerialize**: `boolean` = `false`

Specifies if the material should be serialized

#### Inherited from

PushMaterial.doNotSerialize

#### Defined in

packages/dev/core/src/Materials/material.ts:405

___

### enableNoise

• **enableNoise**: `boolean` = `false`

This helps reducing the banding effect that could occur on the background.

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:403

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

### maxSimultaneousLights

• **maxSimultaneousLights**: `number` = `4`

Number of Simultaneous lights allowed on the material.

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:432

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

### opacityFresnel

• **opacityFresnel**: `boolean` = `true`

This helps specifying that the material is falling off to the sky box at grazing angle.
This helps ensuring a nice transition when the camera goes under the ground.

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:327

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

### primaryColor

• **primaryColor**: [`Color3`](Color3.md)

Key light Color (multiply against the environment texture)

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:211

___

### reflectionAmount

• **reflectionAmount**: `number` = `1.0`

This specifies the weight of the reflection against the background in case of reflection Fresnel.

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:353

___

### reflectionBlur

• **reflectionBlur**: `number` = `0`

Reflection Texture level of blur.

Can be use to reuse an existing HDR Texture and target a specific LOD to prevent authoring the
texture twice.

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:283

___

### reflectionFalloffDistance

• **reflectionFalloffDistance**: `number` = `0.0`

This helps specifying the falloff radius off the reflection texture from the sceneCenter.
This helps adding a nice falloff effect to the reflection if used as a mirror for instance.

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:345

___

### reflectionFresnel

• **reflectionFresnel**: `boolean` = `false`

This helps specifying that the material is falling off from diffuse to the reflection texture at grazing angle.
This helps adding a mirror texture on the ground.

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:336

___

### reflectionReflectance0

• **reflectionReflectance0**: `number` = `0.05`

This specifies the weight of the reflection at grazing angle.

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:361

___

### reflectionReflectance90

• **reflectionReflectance90**: `number` = `0.5`

This specifies the weight of the reflection at a perpendicular point of view.

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:369

___

### reflectionTexture

• **reflectionTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) = `null`

Reflection Texture used in the material.
Should be author in a specific way for the best result (refer to the documentation).

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:272

___

### reservedDataStore

• **reservedDataStore**: `any` = `null`

For internal use only. Please do not use.

#### Inherited from

PushMaterial.reservedDataStore

#### Defined in

packages/dev/core/src/Materials/material.ts:259

___

### sceneCenter

• **sceneCenter**: [`Vector3`](Vector3.md)

In case of opacity Fresnel or reflection falloff, this is use as a scene center.
It is usually zero but might be interesting to modify according to your setup.

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:318

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

### shadowLevel

• **shadowLevel**: `number` = `0`

Helps adjusting the shadow to a softer level if required.
0 means black shadows and 1 means no shadows.

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:309

___

### shadowLights

• **shadowLights**: [`Nullable`](../modules.md#nullable)[`IShadowLight`](../interfaces/IShadowLight.md)[] = `null`

Specify the list of lights casting shadow on the material.
All scene shadow lights will be included if null.

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:300

___

### shadowOnly

• **shadowOnly**: `boolean` = `false`

Make the material only render shadows

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:440

___

### sideOrientation

• **sideOrientation**: `number`

Stores the value for side orientation

#### Inherited from

PushMaterial.sideOrientation

#### Defined in

packages/dev/core/src/Materials/material.ts:376

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

### switchToBGR

• **switchToBGR**: `boolean` = `false`

Due to a bug in iOS10, video tags (which are using the background material) are in BGR and not RGB.
Setting this flag to true (not done automatically!) will convert it back to RGB.

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:608

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the material

#### Inherited from

PushMaterial.uniqueId

#### Defined in

packages/dev/core/src/Materials/material.ts:239

___

### useEquirectangularFOV

• **useEquirectangularFOV**: `boolean` = `false`

Enable the FOV adjustment feature controlled by fovMultiplier.

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:424

___

### useRGBColor

• **useRGBColor**: `boolean` = `true`

Helps to directly use the maps channels instead of their level.

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:395

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

### StandardReflectance0

▪ `Static` **StandardReflectance0**: `number` = `0.05`

Standard reflectance value at parallel view angle.

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:198

___

### StandardReflectance90

▪ `Static` **StandardReflectance90**: `number` = `0.5`

Standard reflectance value at grazing angle.

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:203

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

### \_perceptualColor

• `get` **_perceptualColor**(): [`Nullable`](../modules.md#nullable)[`Color3`](Color3.md)

Experimental Internal Use Only.

Key light Color in "perceptual value" meaning the color you would like to see on screen.
This acts as a helper to set the primary color to a more "human friendly" value.
Conversion to linear space as well as exposure and tone mapping correction will be applied to keep the
output color as close as possible from the chosen value.
(This does not account for contrast color grading and color curves as they are considered post effect and not directly
part of lighting setup.)

#### Returns

[`Nullable`](../modules.md#nullable)[`Color3`](Color3.md)

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:225

• `set` **_perceptualColor**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`Color3`](Color3.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:228

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

The color grading curves provide additional color adjustment that is applied after any color grading transform (3D LUT).
They allow basic adjustment of saturation and small exposure adjustments, along with color filter tinting to provide white balance adjustment or more stylistic effects.
These are similar to controls found in many professional imaging or colorist software. The global controls are applied to the entire image. For advanced tuning, extra controls are provided to adjust the shadow, midtone and highlight areas of the image;
corresponding to low luminance, medium luminance, and high luminance areas respectively.

#### Returns

[`Nullable`](../modules.md#nullable)[`ColorCurves`](ColorCurves.md)

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:591

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

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:600

___

### cameraColorCurvesEnabled

• `get` **cameraColorCurvesEnabled**(): `boolean`

Gets whether the color curves effect is enabled.

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:505

• `set` **cameraColorCurvesEnabled**(`value`): `void`

Sets whether the color curves effect is enabled.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:511

___

### cameraColorGradingEnabled

• `get` **cameraColorGradingEnabled**(): `boolean`

Gets whether the color grading effect is enabled.

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:518

• `set` **cameraColorGradingEnabled**(`value`): `void`

Gets whether the color grading effect is enabled.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:524

___

### cameraColorGradingTexture

• `get` **cameraColorGradingTexture**(): [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Gets the Color Grading 2D Lookup Texture.

#### Returns

[`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:575

• `set` **cameraColorGradingTexture**(`value`): `void`

Sets the Color Grading 2D Lookup Texture.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:581

___

### cameraContrast

• `get` **cameraContrast**(): `number`

Gets The camera contrast used on this material.

#### Returns

`number`

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:561

• `set` **cameraContrast**(`value`): `void`

Sets The camera contrast used on this material.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:568

___

### cameraExposure

• `get` **cameraExposure**(): `number`

The camera exposure used on this material.
This property is here and not in the camera to allow controlling exposure without full screen post process.
This corresponds to a photographic exposure.

#### Returns

`number`

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:546

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

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:554

___

### cameraToneMappingEnabled

• `get` **cameraToneMappingEnabled**(): `boolean`

Gets whether tonemapping is enabled or not.

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:531

• `set` **cameraToneMappingEnabled**(`value`): `void`

Sets whether tonemapping is enabled or not

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:537

___

### canRenderToMRT

• `get` **canRenderToMRT**(): `boolean`

If the material can be rendered to several textures with MRT extension

#### Returns

`boolean`

#### Inherited from

PushMaterial.canRenderToMRT

#### Defined in

packages/dev/core/src/Materials/material.ts:282

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

### fovMultiplier

• `get` **fovMultiplier**(): `number`

The current fov(field of view) multiplier, 0.0 - 2.0. Defaults to 1.0. Lower values "zoom in" and higher values "zoom out".
Best used when trying to implement visual zoom effects like fish-eye or binoculars while not adjusting camera fov.
Recommended to be keep at 1.0 except for special cases.

#### Returns

`number`

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:410

• `set` **fovMultiplier**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:413

___

### hasRenderTargetTextures

• `get` **hasRenderTargetTextures**(): `boolean`

Gets a boolean indicating that current material needs to register RTT

#### Returns

`boolean`

#### Overrides

PushMaterial.hasRenderTargetTextures

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:646

___

### imageProcessingConfiguration

• `get` **imageProcessingConfiguration**(): [`Nullable`](../modules.md#nullable)[`ImageProcessingConfiguration`](ImageProcessingConfiguration.md)

Gets the image processing configuration used either in this material.

#### Returns

[`Nullable`](../modules.md#nullable)[`ImageProcessingConfiguration`](ImageProcessingConfiguration.md)

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:486

• `set` **imageProcessingConfiguration**(`value`): `void`

Sets the Default image processing configuration used either in the this material.

If sets to null, the scene one is in use.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`ImageProcessingConfiguration`](ImageProcessingConfiguration.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:495

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

#### Inherited from

PushMaterial.isPrePassCapable

#### Defined in

packages/dev/core/src/Materials/material.ts:558

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

### primaryColorHighlightLevel

• `get` **primaryColorHighlightLevel**(): `number`

Defines the level of the highlights (highlight area of the reflection map) in order to help scaling the colors.
The primary color is used at the level chosen to define what the white area would look.

#### Returns

`number`

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:255

• `set` **primaryColorHighlightLevel**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:259

___

### primaryColorShadowLevel

• `get` **primaryColorShadowLevel**(): `number`

Defines the level of the shadows (dark area of the reflection map) in order to help scaling the colors.
The color opposite to the primary color is used at the level chosen to define what the black area would look.

#### Returns

`number`

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:240

• `set` **primaryColorShadowLevel**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:243

___

### reflectionStandardFresnelWeight

• `set` **reflectionStandardFresnelWeight**(`value`): `void`

Sets the reflection reflectance fresnel values according to the default standard
empirically know to work well :-)

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:375

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

Attaches a new image processing configuration to the PBR Material.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `configuration` | [`Nullable`](../modules.md#nullable)[`ImageProcessingConfiguration`](ImageProcessingConfiguration.md) | (if null the scene configuration will be use) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:457

___

### \_computePrimaryColorFromPerceptualColor

▸ `Private` **_computePrimaryColorFromPerceptualColor**(): `void`

Compute the primary color according to the chosen perceptual color.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:978

___

### \_computePrimaryColors

▸ `Private` **_computePrimaryColors**(): `void`

Compute the highlights and shadow colors according to their chosen levels.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:1000

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

Bind the material for a dedicated submeh (every used meshes will be considered opaque).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `world` | [`Matrix`](Matrix.md) | The world matrix to bind. |
| `mesh` | [`Mesh`](Mesh.md) |  |
| `subMesh` | [`SubMesh`](SubMesh.md) | The submesh to bind for. |

#### Returns

`void`

#### Overrides

PushMaterial.bindForSubMesh

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:1066

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

Bind only the world matrix to the material.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `world` | [`Matrix`](Matrix.md) | The world matrix to bind. |

#### Returns

`void`

#### Overrides

PushMaterial.bindOnlyWorldMatrix

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:1056

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

Build the uniform buffer used in the material.

#### Returns

`void`

#### Overrides

PushMaterial.buildUniformLayout

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:1018

___

### clone

▸ **clone**(`name`): [`BackgroundMaterial`](BackgroundMaterial.md)

Clones the material.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | The cloned name. |

#### Returns

[`BackgroundMaterial`](BackgroundMaterial.md)

The cloned material.

#### Overrides

PushMaterial.clone

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:1245

___

### dispose

▸ **dispose**(`forceDisposeEffect?`, `forceDisposeTextures?`): `void`

Dispose the material.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `forceDisposeEffect` | `boolean` | `false` | Force disposal of the associated effect. |
| `forceDisposeTextures` | `boolean` | `false` | Force disposal of the associated textures. |

#### Returns

`void`

#### Overrides

PushMaterial.dispose

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:1221

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

#### Inherited from

PushMaterial.getActiveTextures

#### Defined in

packages/dev/core/src/Materials/material.ts:1257

___

### getAlphaTestTexture

▸ **getAlphaTestTexture**(): [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Gets the texture used for the alpha test

#### Returns

[`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

the texture to use for alpha testing

#### Inherited from

PushMaterial.getAlphaTestTexture

#### Defined in

packages/dev/core/src/Materials/material.ts:1048

___

### getAnimatables

▸ **getAnimatables**(): [`IAnimatable`](../interfaces/IAnimatable.md)[]

Returns the animatable textures.

#### Returns

[`IAnimatable`](../interfaces/IAnimatable.md)[]

- Array of animatable textures.

#### Inherited from

PushMaterial.getAnimatables

#### Defined in

packages/dev/core/src/Materials/material.ts:1247

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

Gets the class name of the material

#### Returns

`string`

"BackgroundMaterial"

#### Overrides

PushMaterial.getClassName

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:1263

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

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:1200

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

Checks whether the material is ready to be rendered for a given mesh.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | `undefined` | The mesh to render |
| `subMesh` | [`SubMesh`](SubMesh.md) | `undefined` | The submesh to check against |
| `useInstances` | `boolean` | `false` | Specify wether or not the material is used with instances |

#### Returns

`boolean`

true if all the dependencies are ready (Textures, Effects...)

#### Overrides

PushMaterial.isReadyForSubMesh

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:681

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

The entire material has been created in order to prevent overdraw.

#### Returns

`boolean`

true if blending is enable

#### Overrides

PushMaterial.needAlphaBlending

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:670

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

The entire material has been created in order to prevent overdraw.

#### Returns

`boolean`

false

#### Overrides

PushMaterial.needAlphaTesting

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:662

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

Serializes the current material to its JSON representation.

#### Returns

`any`

The JSON representation.

#### Overrides

PushMaterial.serialize

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:1253

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

Unbind the material.

#### Returns

`void`

#### Overrides

PushMaterial.unbind

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:1040

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

▸ `Static` **Parse**(`source`, `scene`, `rootUrl`): [`BackgroundMaterial`](BackgroundMaterial.md)

Parse a JSON input to create back a background material.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | `any` | The JSON data to parse |
| `scene` | [`Scene`](Scene.md) | The scene to create the parsed material in |
| `rootUrl` | `string` | The root url of the assets the material depends upon |

#### Returns

[`BackgroundMaterial`](BackgroundMaterial.md)

the instantiated BackgroundMaterial.

#### Overrides

PushMaterial.Parse

#### Defined in

packages/dev/core/src/Materials/Background/backgroundMaterial.ts:1274
