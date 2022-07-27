[@dev/core](../README.md) / [Exports](../modules.md) / Material

# Class: Material

Base class for the main features of a material in Babylon.js

## Hierarchy

- **`Material`**

  ↳ [`MultiMaterial`](MultiMaterial.md)

## Implements

- [`IAnimatable`](../interfaces/IAnimatable.md)

## Table of contents

### Constructors

- [constructor](Material.md#constructor)

### Properties

- [\_alpha](Material.md#_alpha)
- [\_alphaMode](Material.md#_alphamode)
- [\_backFaceCulling](Material.md#_backfaceculling)
- [\_cachedColorWriteState](Material.md#_cachedcolorwritestate)
- [\_cachedDepthFunctionState](Material.md#_cacheddepthfunctionstate)
- [\_cachedDepthWriteState](Material.md#_cacheddepthwritestate)
- [\_cullBackFaces](Material.md#_cullbackfaces)
- [\_drawWrapper](Material.md#_drawwrapper)
- [\_eventInfo](Material.md#_eventinfo)
- [\_fillMode](Material.md#_fillmode)
- [\_fogEnabled](Material.md#_fogenabled)
- [\_forceAlphaTest](Material.md#_forcealphatest)
- [\_needDepthPrePass](Material.md#_needdepthprepass)
- [\_needToBindSceneUbo](Material.md#_needtobindsceneubo)
- [\_onBindObservable](Material.md#_onbindobservable)
- [\_onBindObserver](Material.md#_onbindobserver)
- [\_onDisposeObserver](Material.md#_ondisposeobserver)
- [\_onEffectCreatedObservable](Material.md#_oneffectcreatedobservable)
- [\_onUnBindObservable](Material.md#_onunbindobservable)
- [\_scene](Material.md#_scene)
- [\_transparencyMode](Material.md#_transparencymode)
- [\_useUBO](Material.md#_useubo)
- [allowShaderHotSwapping](Material.md#allowshaderhotswapping)
- [animations](Material.md#animations)
- [checkReadyOnEveryCall](Material.md#checkreadyoneverycall)
- [checkReadyOnlyOnce](Material.md#checkreadyonlyonce)
- [customShaderNameResolve](Material.md#customshadernameresolve)
- [depthFunction](Material.md#depthfunction)
- [disableColorWrite](Material.md#disablecolorwrite)
- [disableDepthWrite](Material.md#disabledepthwrite)
- [doNotSerialize](Material.md#donotserialize)
- [forceDepthWrite](Material.md#forcedepthwrite)
- [getRenderTargetTextures](Material.md#getrendertargettextures)
- [id](Material.md#id)
- [inspectableCustomProperties](Material.md#inspectablecustomproperties)
- [metadata](Material.md#metadata)
- [name](Material.md#name)
- [onCompiled](Material.md#oncompiled)
- [onDisposeObservable](Material.md#ondisposeobservable)
- [onError](Material.md#onerror)
- [pluginManager](Material.md#pluginmanager)
- [pointSize](Material.md#pointsize)
- [reservedDataStore](Material.md#reserveddatastore)
- [separateCullingPass](Material.md#separatecullingpass)
- [shadowDepthWrapper](Material.md#shadowdepthwrapper)
- [sideOrientation](Material.md#sideorientation)
- [state](Material.md#state)
- [stencil](Material.md#stencil)
- [uniqueId](Material.md#uniqueid)
- [zOffset](Material.md#zoffset)
- [zOffsetUnits](Material.md#zoffsetunits)
- [AllDirtyFlag](Material.md#alldirtyflag)
- [AttributesDirtyFlag](Material.md#attributesdirtyflag)
- [ClockWiseSideOrientation](Material.md#clockwisesideorientation)
- [CounterClockWiseSideOrientation](Material.md#counterclockwisesideorientation)
- [FresnelDirtyFlag](Material.md#fresneldirtyflag)
- [LightDirtyFlag](Material.md#lightdirtyflag)
- [LineListDrawMode](Material.md#linelistdrawmode)
- [LineLoopDrawMode](Material.md#lineloopdrawmode)
- [LineStripDrawMode](Material.md#linestripdrawmode)
- [MATERIAL\_ALPHABLEND](Material.md#material_alphablend)
- [MATERIAL\_ALPHATEST](Material.md#material_alphatest)
- [MATERIAL\_ALPHATESTANDBLEND](Material.md#material_alphatestandblend)
- [MATERIAL\_NORMALBLENDMETHOD\_RNM](Material.md#material_normalblendmethod_rnm)
- [MATERIAL\_NORMALBLENDMETHOD\_WHITEOUT](Material.md#material_normalblendmethod_whiteout)
- [MATERIAL\_OPAQUE](Material.md#material_opaque)
- [MiscDirtyFlag](Material.md#miscdirtyflag)
- [OnEventObservable](Material.md#oneventobservable)
- [PointFillMode](Material.md#pointfillmode)
- [PointListDrawMode](Material.md#pointlistdrawmode)
- [PrePassDirtyFlag](Material.md#prepassdirtyflag)
- [TextureDirtyFlag](Material.md#texturedirtyflag)
- [TriangleFanDrawMode](Material.md#trianglefandrawmode)
- [TriangleFillMode](Material.md#trianglefillmode)
- [TriangleStripDrawMode](Material.md#trianglestripdrawmode)
- [WireFrameFillMode](Material.md#wireframefillmode)
- [\_DirtyCallbackArray](Material.md#_dirtycallbackarray)

### Accessors

- [\_disableAlphaBlending](Material.md#_disablealphablending)
- [alpha](Material.md#alpha)
- [alphaMode](Material.md#alphamode)
- [backFaceCulling](Material.md#backfaceculling)
- [canRenderToMRT](Material.md#canrendertomrt)
- [cullBackFaces](Material.md#cullbackfaces)
- [fillMode](Material.md#fillmode)
- [fogEnabled](Material.md#fogenabled)
- [hasRenderTargetTextures](Material.md#hasrendertargettextures)
- [isFrozen](Material.md#isfrozen)
- [isPrePassCapable](Material.md#isprepasscapable)
- [needDepthPrePass](Material.md#needdepthprepass)
- [onBind](Material.md#onbind)
- [onBindObservable](Material.md#onbindobservable)
- [onDispose](Material.md#ondispose)
- [onEffectCreatedObservable](Material.md#oneffectcreatedobservable)
- [onUnBindObservable](Material.md#onunbindobservable)
- [pointsCloud](Material.md#pointscloud)
- [transparencyMode](Material.md#transparencymode)
- [wireframe](Material.md#wireframe)

### Methods

- [\_afterBind](Material.md#_afterbind)
- [\_markAllSubMeshesAsAllDirty](Material.md#_markallsubmeshesasalldirty)
- [\_markAllSubMeshesAsAttributesDirty](Material.md#_markallsubmeshesasattributesdirty)
- [\_markAllSubMeshesAsDirty](Material.md#_markallsubmeshesasdirty)
- [\_markAllSubMeshesAsFresnelAndMiscDirty](Material.md#_markallsubmeshesasfresnelandmiscdirty)
- [\_markAllSubMeshesAsFresnelDirty](Material.md#_markallsubmeshesasfresneldirty)
- [\_markAllSubMeshesAsImageProcessingDirty](Material.md#_markallsubmeshesasimageprocessingdirty)
- [\_markAllSubMeshesAsLightsDirty](Material.md#_markallsubmeshesaslightsdirty)
- [\_markAllSubMeshesAsMiscDirty](Material.md#_markallsubmeshesasmiscdirty)
- [\_markAllSubMeshesAsPrePassDirty](Material.md#_markallsubmeshesasprepassdirty)
- [\_markAllSubMeshesAsTexturesAndMiscDirty](Material.md#_markallsubmeshesastexturesandmiscdirty)
- [\_markAllSubMeshesAsTexturesDirty](Material.md#_markallsubmeshesastexturesdirty)
- [\_markScenePrePassDirty](Material.md#_marksceneprepassdirty)
- [\_shouldTurnAlphaTestOn](Material.md#_shouldturnalphateston)
- [bind](Material.md#bind)
- [bindEyePosition](Material.md#bindeyeposition)
- [bindForSubMesh](Material.md#bindforsubmesh)
- [bindOnlyWorldMatrix](Material.md#bindonlyworldmatrix)
- [bindView](Material.md#bindview)
- [bindViewProjection](Material.md#bindviewprojection)
- [buildUniformLayout](Material.md#builduniformlayout)
- [clone](Material.md#clone)
- [dispose](Material.md#dispose)
- [forceCompilation](Material.md#forcecompilation)
- [forceCompilationAsync](Material.md#forcecompilationasync)
- [freeze](Material.md#freeze)
- [getActiveTextures](Material.md#getactivetextures)
- [getAlphaTestTexture](Material.md#getalphatesttexture)
- [getAnimatables](Material.md#getanimatables)
- [getBindedMeshes](Material.md#getbindedmeshes)
- [getClassName](Material.md#getclassname)
- [getEffect](Material.md#geteffect)
- [getScene](Material.md#getscene)
- [hasTexture](Material.md#hastexture)
- [isReady](Material.md#isready)
- [isReadyForSubMesh](Material.md#isreadyforsubmesh)
- [markAsDirty](Material.md#markasdirty)
- [markDirty](Material.md#markdirty)
- [needAlphaBlending](Material.md#needalphablending)
- [needAlphaBlendingForMesh](Material.md#needalphablendingformesh)
- [needAlphaTesting](Material.md#needalphatesting)
- [resetDrawCache](Material.md#resetdrawcache)
- [serialize](Material.md#serialize)
- [setPrePassRenderer](Material.md#setprepassrenderer)
- [toString](Material.md#tostring)
- [unbind](Material.md#unbind)
- [unfreeze](Material.md#unfreeze)
- [Parse](Material.md#parse)
- [\_AllDirtyCallBack](Material.md#_alldirtycallback)
- [\_AttributeDirtyCallBack](Material.md#_attributedirtycallback)
- [\_FresnelAndMiscDirtyCallBack](Material.md#_fresnelandmiscdirtycallback)
- [\_FresnelDirtyCallBack](Material.md#_fresneldirtycallback)
- [\_ImageProcessingDirtyCallBack](Material.md#_imageprocessingdirtycallback)
- [\_LightsDirtyCallBack](Material.md#_lightsdirtycallback)
- [\_MiscDirtyCallBack](Material.md#_miscdirtycallback)
- [\_PrePassDirtyCallBack](Material.md#_prepassdirtycallback)
- [\_RunDirtyCallBacks](Material.md#_rundirtycallbacks)
- [\_TextureAndMiscDirtyCallBack](Material.md#_textureandmiscdirtycallback)
- [\_TextureDirtyCallBack](Material.md#_texturedirtycallback)

## Constructors

### constructor

• **new Material**(`name`, `scene?`, `doNotAdd?`)

Creates a material instance

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the name of the material |
| `scene?` | [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) | defines the scene to reference |
| `doNotAdd?` | `boolean` | specifies if the material should be added to the scene |

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:818

## Properties

### \_alpha

• `Protected` **\_alpha**: `number` = `1.0`

The alpha value of the material

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:292

___

### \_alphaMode

• `Private` **\_alphaMode**: `number` = `Constants.ALPHA_COMBINE`

Stores the value of the alpha mode

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:494

___

### \_backFaceCulling

• `Protected` **\_backFaceCulling**: `boolean` = `true`

Specifies if back face culling is enabled

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:328

___

### \_cachedColorWriteState

• `Private` **\_cachedColorWriteState**: `boolean` = `false`

Specifies if the color write state should be cached

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:742

___

### \_cachedDepthFunctionState

• `Private` **\_cachedDepthFunctionState**: `number` = `0`

Specifies if the depth function state should be cached

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:747

___

### \_cachedDepthWriteState

• `Private` **\_cachedDepthWriteState**: `boolean` = `false`

Specifies if the depth write state should be cached

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:737

___

### \_cullBackFaces

• `Protected` **\_cullBackFaces**: `boolean` = `true`

Specifies if back or front faces should be culled (when culling is enabled)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:352

___

### \_drawWrapper

• `Protected` **\_drawWrapper**: `DrawWrapper`

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:705

___

### \_eventInfo

• `Protected` **\_eventInfo**: `MaterialPluginDisposed` & `MaterialPluginHasTexture` & `MaterialPluginIsReadyForSubMesh` & `MaterialPluginGetDefineNames` & `MaterialPluginPrepareEffect` & `MaterialPluginPrepareDefines` & `MaterialPluginPrepareUniformBuffer` & `MaterialPluginBindForSubMesh` & `MaterialPluginGetAnimatables` & `MaterialPluginGetActiveTextures` & `MaterialPluginFillRenderTargetTextures` & `MaterialPluginHasRenderTargetTextures` & `MaterialPluginHardBindForSubMesh`

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:770

___

### \_fillMode

• `Private` **\_fillMode**: `number` = `Material.TriangleFillMode`

Stores the fill mode state

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:732

___

### \_fogEnabled

• `Private` **\_fogEnabled**: `boolean` = `true`

Stores the state specifying if fog should be enabled

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:596

___

### \_forceAlphaTest

• `Protected` **\_forceAlphaTest**: `boolean` = `false`

Enforces alpha test in opaque or blend mode in order to improve the performances of some situations.

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:954

___

### \_needDepthPrePass

• `Private` **\_needDepthPrePass**: `boolean` = `false`

Stores the state of the need depth pre-pass value

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:533

___

### \_needToBindSceneUbo

• `Protected` **\_needToBindSceneUbo**: `boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:727

___

### \_onBindObservable

• `Private` **\_onBindObservable**: [`Nullable`](../modules.md#nullable)[`Observable`](Observable.md)[`AbstractMesh`](AbstractMesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:438

___

### \_onBindObserver

• `Private` **\_onBindObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`AbstractMesh`](AbstractMesh.md) = `null`

An observer which watches for bind events

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:454

___

### \_onDisposeObserver

• `Private` **\_onDisposeObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Material`](Material.md) = `null`

An observer which watches for dispose events

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:425

___

### \_onEffectCreatedObservable

• `Protected` **\_onEffectCreatedObservable**: [`Nullable`](../modules.md#nullable)[`Observable`](Observable.md){ `effect`: [`Effect`](Effect.md) ; `subMesh`: [`Nullable`](../modules.md#nullable)[`SubMesh`](SubMesh.md)  }

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:477

___

### \_onUnBindObservable

• `Private` **\_onUnBindObservable**: [`Nullable`](../modules.md#nullable)[`Observable`](Observable.md)[`Material`](Material.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:426

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

Stores a reference to the scene

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:726

___

### \_transparencyMode

• `Protected` **\_transparencyMode**: [`Nullable`](../modules.md#nullable)`number` = `null`

The transparency mode of the material.

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:959

___

### \_useUBO

• `Private` **\_useUBO**: `boolean` = `false`

Specifies if uniform buffers should be used

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:721

___

### allowShaderHotSwapping

• **allowShaderHotSwapping**: `boolean` = `true`

Gets or sets a boolean indicating that the material is allowed (if supported) to do shader hot swapping.
This means that the material can keep using a previous shader while a new one is being compiled.
This is mostly used when shader parallel compilation is supported (true by default)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:227

___

### animations

• **animations**: [`Nullable`](../modules.md#nullable)[`Animation`](Animation.md)[] = `null`

Stores the animations for the material

#### Implementation of

[IAnimatable](../interfaces/IAnimatable.md).[animations](../interfaces/IAnimatable.md#animations)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:415

___

### checkReadyOnEveryCall

• **checkReadyOnEveryCall**: `boolean` = `false`

Specifies if the ready state should be checked on each call

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:265

___

### checkReadyOnlyOnce

• **checkReadyOnlyOnce**: `boolean` = `false`

Specifies if the ready state should be checked once

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:271

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:207

___

### depthFunction

• **depthFunction**: `number` = `0`

Specifies the depth function that should be used. 0 means the default engine function

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:584

___

### disableColorWrite

• **disableColorWrite**: `boolean` = `false`

Specifies if color writing should be disabled

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:572

___

### disableDepthWrite

• **disableDepthWrite**: `boolean` = `false`

Specifies if depth writing should be disabled

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:566

___

### doNotSerialize

• **doNotSerialize**: `boolean` = `false`

Specifies if the material should be serialized

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:405

___

### forceDepthWrite

• **forceDepthWrite**: `boolean` = `false`

Specifies if depth writing should be forced

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:578

___

### getRenderTargetTextures

• **getRenderTargetTextures**: [`Nullable`](../modules.md#nullable)() => [`SmartArray`](SmartArray.md)[`RenderTargetTexture`](RenderTargetTexture.md) = `null`

Callback triggered to get the render target textures

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:391

___

### id

• **id**: `string`

The ID of the material

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:233

___

### inspectableCustomProperties

• **inspectableCustomProperties**: [`IInspectable`](../interfaces/IInspectable.md)[]

List of inspectable custom properties (used by the Inspector)

**`See`**

https://doc.babylonjs.com/how_to/debug_layer#extensibility

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:298

___

### metadata

• **metadata**: `any` = `null`

Gets or sets user defined metadata

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:254

___

### name

• **name**: `string`

The name of the material

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:248

___

### onCompiled

• **onCompiled**: [`Nullable`](../modules.md#nullable)(`effect`: [`Effect`](Effect.md)) => `void` = `null`

Callback triggered when the material is compiled

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:381

___

### onDisposeObservable

• **onDisposeObservable**: [`Observable`](Observable.md)[`Material`](Material.md)

An event triggered when the material is disposed

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:420

___

### onError

• **onError**: [`Nullable`](../modules.md#nullable)(`effect`: [`Effect`](Effect.md), `errors`: `string`) => `void` = `null`

Callback triggered when an error occurs

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:386

___

### pluginManager

• `Optional` **pluginManager**: [`MaterialPluginManager`](MaterialPluginManager.md)

Plugin manager for this material

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginManager.ts:30

___

### pointSize

• **pointSize**: `number` = `1.0`

Stores the size of points

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:620

___

### reservedDataStore

• **reservedDataStore**: `any` = `null`

For internal use only. Please do not use.

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:259

___

### separateCullingPass

• **separateCullingPass**: `boolean` = `false`

Specifies if there should be a separate pass for culling

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:590

___

### shadowDepthWrapper

• **shadowDepthWrapper**: [`Nullable`](../modules.md#nullable)[`ShadowDepthWrapper`](ShadowDepthWrapper.md) = `null`

Custom shadow depth material to use for shadow rendering instead of the in-built one

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:220

___

### sideOrientation

• **sideOrientation**: `number`

Stores the value for side orientation

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:376

___

### state

• **state**: `string` = `""`

The state of the material

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:277

___

### stencil

• `Readonly` **stencil**: `MaterialStencilState`

Gives access to the stencil properties of the material

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:697

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the material

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:239

___

### zOffset

• **zOffset**: `number` = `0`

Stores the z offset Factor value

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:626

___

### zOffsetUnits

• **zOffsetUnits**: `number` = `0`

Stores the z offset Units value

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:632

___

### AllDirtyFlag

▪ `Static` `Readonly` **AllDirtyFlag**: ``63``

The all dirty flag value

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:164

___

### AttributesDirtyFlag

▪ `Static` `Readonly` **AttributesDirtyFlag**: ``8``

The dirty attribute flag value

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:149

___

### ClockWiseSideOrientation

▪ `Static` `Readonly` **ClockWiseSideOrientation**: ``0``

Stores the clock-wise side orientation

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:124

___

### CounterClockWiseSideOrientation

▪ `Static` `Readonly` **CounterClockWiseSideOrientation**: ``1``

Stores the counter clock-wise side orientation

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:129

___

### FresnelDirtyFlag

▪ `Static` `Readonly` **FresnelDirtyFlag**: ``4``

The dirty fresnel flag value

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:144

___

### LightDirtyFlag

▪ `Static` `Readonly` **LightDirtyFlag**: ``2``

The dirty light flag value

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:139

___

### LineListDrawMode

▪ `Static` `Readonly` **LineListDrawMode**: ``4``

Returns the line list draw mode

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:103

___

### LineLoopDrawMode

▪ `Static` `Readonly` **LineLoopDrawMode**: ``5``

Returns the line loop draw mode

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:107

___

### LineStripDrawMode

▪ `Static` `Readonly` **LineStripDrawMode**: ``6``

Returns the line strip draw mode

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:111

___

### MATERIAL\_ALPHABLEND

▪ `Static` `Readonly` **MATERIAL\_ALPHABLEND**: ``2``

MaterialTransparencyMode: Pixels are blended (according to the alpha mode) with the already drawn pixels in the current frame buffer.

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:179

___

### MATERIAL\_ALPHATEST

▪ `Static` `Readonly` **MATERIAL\_ALPHATEST**: ``1``

MaterialTransparencyMode: Alpha Test mode, pixel are discarded below a certain threshold defined by the alpha cutoff value.

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:174

___

### MATERIAL\_ALPHATESTANDBLEND

▪ `Static` `Readonly` **MATERIAL\_ALPHATESTANDBLEND**: ``3``

MaterialTransparencyMode: Pixels are blended (according to the alpha mode) with the already drawn pixels in the current frame buffer.
They are also discarded below the alpha cutoff threshold to improve performances.

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:185

___

### MATERIAL\_NORMALBLENDMETHOD\_RNM

▪ `Static` `Readonly` **MATERIAL\_NORMALBLENDMETHOD\_RNM**: ``1``

The Reoriented Normal Mapping method is used to blend normals.
Details of the algorithm can be found here: https://blog.selfshadow.com/publications/blending-in-detail/

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:197

___

### MATERIAL\_NORMALBLENDMETHOD\_WHITEOUT

▪ `Static` `Readonly` **MATERIAL\_NORMALBLENDMETHOD\_WHITEOUT**: ``0``

The Whiteout method is used to blend normals.
Details of the algorithm can be found here: https://blog.selfshadow.com/publications/blending-in-detail/

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:191

___

### MATERIAL\_OPAQUE

▪ `Static` `Readonly` **MATERIAL\_OPAQUE**: ``0``

MaterialTransparencyMode: No transparency mode, Alpha channel is not use.

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:169

___

### MiscDirtyFlag

▪ `Static` `Readonly` **MiscDirtyFlag**: ``16``

The dirty misc flag value

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:154

___

### OnEventObservable

▪ `Static` **OnEventObservable**: [`Observable`](Observable.md)[`Material`](Material.md)

Event observable which raises global events common to all materials (like MaterialPluginEvent.Created)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:202

___

### PointFillMode

▪ `Static` `Readonly` **PointFillMode**: ``2``

Returns the point fill mode

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:95

___

### PointListDrawMode

▪ `Static` `Readonly` **PointListDrawMode**: ``3``

Returns the point list draw mode

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:99

___

### PrePassDirtyFlag

▪ `Static` `Readonly` **PrePassDirtyFlag**: ``32``

The dirty prepass flag value

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:159

___

### TextureDirtyFlag

▪ `Static` `Readonly` **TextureDirtyFlag**: ``1``

The dirty texture flag value

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:134

___

### TriangleFanDrawMode

▪ `Static` `Readonly` **TriangleFanDrawMode**: ``8``

Returns the triangle fan draw mode

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:119

___

### TriangleFillMode

▪ `Static` `Readonly` **TriangleFillMode**: ``0``

Returns the triangle fill mode

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:87

___

### TriangleStripDrawMode

▪ `Static` `Readonly` **TriangleStripDrawMode**: ``7``

Returns the triangle strip draw mode

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:115

___

### WireFrameFillMode

▪ `Static` `Readonly` **WireFrameFillMode**: ``1``

Returns the wireframe mode

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:91

___

### \_DirtyCallbackArray

▪ `Static` `Private` `Readonly` **\_DirtyCallbackArray**: (`defines`: [`MaterialDefines`](MaterialDefines.md)) => `void`[] = `[]`

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1426

## Accessors

### \_disableAlphaBlending

• `Protected` `get` **_disableAlphaBlending**(): `boolean`

Returns true if alpha blending should be disabled.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:995

___

### alpha

• `get` **alpha**(): `number`

Gets the alpha value of the material

#### Returns

`number`

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:303

___

### alphaMode

• `get` **alphaMode**(): `number`

Gets the value of the alpha mode

#### Returns

`number`

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:514

___

### backFaceCulling

• `get` **backFaceCulling**(): `boolean`

Gets the culling state

#### Returns

`boolean`

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:333

___

### canRenderToMRT

• `get` **canRenderToMRT**(): `boolean`

If the material can be rendered to several textures with MRT extension

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:282

___

### cullBackFaces

• `get` **cullBackFaces**(): `boolean`

Gets the type of faces that should be culled

#### Returns

`boolean`

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:357

___

### fillMode

• `get` **fillMode**(): `number`

Gets the material fill mode

#### Returns

`number`

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:685

___

### fogEnabled

• `get` **fogEnabled**(): `boolean`

Gets the value of the fog enabled state

#### Returns

`boolean`

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:601

___

### hasRenderTargetTextures

• `get` **hasRenderTargetTextures**(): `boolean`

Gets a boolean indicating that current material needs to register RTT

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:396

___

### isFrozen

• `get` **isFrozen**(): `boolean`

Specifies if updates for the material been locked

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:883

___

### isPrePassCapable

• `get` **isPrePassCapable**(): `boolean`

Can this material render to prepass

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:558

___

### needDepthPrePass

• `get` **needDepthPrePass**(): `boolean`

Gets the depth pre-pass value

#### Returns

`boolean`

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:459

___

### onBindObservable

• `get` **onBindObservable**(): [`Observable`](Observable.md)[`AbstractMesh`](AbstractMesh.md)

An event triggered when the material is bound

#### Returns

[`Observable`](Observable.md)[`AbstractMesh`](AbstractMesh.md)

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:431

___

### onEffectCreatedObservable

• `get` **onEffectCreatedObservable**(): [`Observable`](Observable.md){ `effect`: [`Effect`](Effect.md) ; `subMesh`: [`Nullable`](../modules.md#nullable)[`SubMesh`](SubMesh.md)  }

An event triggered when the effect is (re)created

#### Returns

[`Observable`](Observable.md){ `effect`: [`Effect`](Effect.md) ; `subMesh`: [`Nullable`](../modules.md#nullable)[`SubMesh`](SubMesh.md)  }

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:482

___

### onUnBindObservable

• `get` **onUnBindObservable**(): [`Observable`](Observable.md)[`Material`](Material.md)

An event triggered when the material is unbound

#### Returns

[`Observable`](Observable.md)[`Material`](Material.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:469

___

### pointsCloud

• `get` **pointsCloud**(): `boolean`

Gets the value specifying if point clouds are enabled

#### Returns

`boolean`

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:670

___

### transparencyMode

• `get` **transparencyMode**(): [`Nullable`](../modules.md#nullable)`number`

Gets the current transparency mode.

#### Returns

[`Nullable`](../modules.md#nullable)`number`

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:980

___

### wireframe

• `get` **wireframe**(): `boolean`

#### Returns

`boolean`

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:649

## Methods

### \_afterBind

▸ `Protected` **_afterBind**(`mesh?`, `effect?`): `void`

Processes to execute after binding the material to a mesh

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `mesh?` | [`Mesh`](Mesh.md) | `undefined` | defines the rendered mesh |
| `effect` | [`Nullable`](../modules.md#nullable)[`Effect`](Effect.md) | `null` |  |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1181

___

### \_markAllSubMeshesAsAllDirty

▸ `Protected` **_markAllSubMeshesAsAllDirty**(): `void`

Indicates that we need to re-calculated for all submeshes

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1543

___

### \_markAllSubMeshesAsAttributesDirty

▸ `Protected` **_markAllSubMeshesAsAttributesDirty**(): `void`

Indicates that attributes need to be re-calculated for all submeshes

#### Returns

`void`

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1498

___

### \_markAllSubMeshesAsFresnelAndMiscDirty

▸ `Protected` **_markAllSubMeshesAsFresnelAndMiscDirty**(): `void`

Indicates that fresnel and misc need to be re-calculated for all submeshes

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1571

___

### \_markAllSubMeshesAsFresnelDirty

▸ `Protected` **_markAllSubMeshesAsFresnelDirty**(): `void`

Indicates that fresnel needs to be re-calculated for all submeshes

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1564

___

### \_markAllSubMeshesAsImageProcessingDirty

▸ `Protected` **_markAllSubMeshesAsImageProcessingDirty**(): `void`

Indicates that image processing needs to be re-calculated for all submeshes

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1550

___

### \_markAllSubMeshesAsLightsDirty

▸ `Protected` **_markAllSubMeshesAsLightsDirty**(): `void`

Indicates that lights need to be re-calculated for all submeshes

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1578

___

### \_markAllSubMeshesAsMiscDirty

▸ `Protected` **_markAllSubMeshesAsMiscDirty**(): `void`

Indicates that misc needs to be re-calculated for all submeshes

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1592

___

### \_markAllSubMeshesAsPrePassDirty

▸ `Protected` **_markAllSubMeshesAsPrePassDirty**(): `void`

Indicates that prepass needs to be re-calculated for all submeshes

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1599

___

### \_markAllSubMeshesAsTexturesAndMiscDirty

▸ `Protected` **_markAllSubMeshesAsTexturesAndMiscDirty**(): `void`

Indicates that textures and misc need to be re-calculated for all submeshes

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1606

___

### \_markAllSubMeshesAsTexturesDirty

▸ `Protected` **_markAllSubMeshesAsTexturesDirty**(): `void`

Indicates that textures need to be re-calculated for all submeshes

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1557

___

### \_markScenePrePassDirty

▸ `Protected` **_markScenePrePassDirty**(): `void`

Indicates that the scene should check if the rendering now needs a prepass

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1529

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1040

___

### bind

▸ **bind**(`world`, `mesh?`): `void`

Binds the material to the mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `world` | [`Matrix`](Matrix.md) | defines the world transformation matrix |
| `mesh?` | [`Mesh`](Mesh.md) | defines the mesh to bind the material to |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1099

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1168

___

### bindForSubMesh

▸ **bindForSubMesh**(`world`, `mesh`, `subMesh`): `void`

Binds the submesh to the material

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `world` | [`Matrix`](Matrix.md) | defines the world transformation matrix |
| `mesh` | [`Mesh`](Mesh.md) | defines the mesh containing the submesh |
| `subMesh` | [`SubMesh`](SubMesh.md) | defines the submesh to bind the material to |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1121

___

### bindOnlyWorldMatrix

▸ **bindOnlyWorldMatrix**(`world`): `void`

Binds the world matrix to the material

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `world` | [`Matrix`](Matrix.md) | defines the world transformation matrix |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1136

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1154

___

### buildUniformLayout

▸ **buildUniformLayout**(): `void`

Initializes the uniform buffer layout for the shader.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1104

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1281

___

### dispose

▸ **dispose**(`forceDisposeEffect?`, `forceDisposeTextures?`, `notBoundToMesh?`): `void`

Disposes the material

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `forceDisposeEffect?` | `boolean` | specifies if effects should be forcefully disposed |
| `forceDisposeTextures?` | `boolean` | specifies if textures should be forcefully disposed |
| `notBoundToMesh?` | `boolean` | specifies if the material that is being disposed is known to be not bound to any mesh |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1627

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1312

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1392

___

### freeze

▸ **freeze**(): `void`

Locks updates for the material

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:890

___

### getActiveTextures

▸ **getActiveTextures**(): [`BaseTexture`](BaseTexture.md)[]

Gets the active textures from the material

#### Returns

[`BaseTexture`](BaseTexture.md)[]

an array of textures

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1257

___

### getAlphaTestTexture

▸ **getAlphaTestTexture**(): [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Gets the texture used for the alpha test

#### Returns

[`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

the texture to use for alpha testing

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1048

___

### getAnimatables

▸ **getAnimatables**(): [`IAnimatable`](../interfaces/IAnimatable.md)[]

Returns the animatable textures.

#### Returns

[`IAnimatable`](../interfaces/IAnimatable.md)[]

- Array of animatable textures.

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1247

___

### getBindedMeshes

▸ **getBindedMeshes**(): [`AbstractMesh`](AbstractMesh.md)[]

Gets the meshes bound to the material

#### Returns

[`AbstractMesh`](AbstractMesh.md)[]

an array of meshes bound to the material

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1289

___

### getClassName

▸ **getClassName**(): `string`

Gets the class name of the material

#### Returns

`string`

a string with the class name of the material

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:876

___

### getEffect

▸ **getEffect**(): [`Nullable`](../modules.md#nullable)[`Effect`](Effect.md)

Returns the material effect

#### Returns

[`Nullable`](../modules.md#nullable)[`Effect`](Effect.md)

the effect associated with the material

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:939

___

### getScene

▸ **getScene**(): [`Scene`](Scene.md)

Returns the current scene

#### Returns

[`Scene`](Scene.md)

a Scene

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:947

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1268

___

### isReady

▸ **isReady**(`mesh?`, `useInstances?`): `boolean`

Specifies if the material is ready to be used

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh?` | [`AbstractMesh`](AbstractMesh.md) | defines the mesh to check |
| `useInstances?` | `boolean` | specifies if instances should be used |

#### Returns

`boolean`

a boolean indicating if the material is ready to be used

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:910

___

### isReadyForSubMesh

▸ **isReadyForSubMesh**(`mesh`, `subMesh`, `useInstances?`): `boolean`

Specifies that the submesh is ready to be used

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | defines the mesh to check |
| `subMesh` | [`SubMesh`](SubMesh.md) | defines which submesh to check |
| `useInstances?` | `boolean` | specifies that instances should be used |

#### Returns

`boolean`

a boolean indicating that the submesh is ready or not

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:922

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1437

___

### markDirty

▸ **markDirty**(): `void`

Marks the material to indicate that it needs to be re-calculated

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1055

___

### needAlphaBlending

▸ **needAlphaBlending**(): `boolean`

Specifies whether or not this material should be rendered in alpha blend mode.

#### Returns

`boolean`

a boolean specifying if alpha blending is needed

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1003

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1016

___

### needAlphaTesting

▸ **needAlphaTesting**(): `boolean`

Specifies whether or not this material should be rendered in alpha test mode.

#### Returns

`boolean`

a boolean specifying if an alpha test is needed.

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1028

___

### resetDrawCache

▸ **resetDrawCache**(): `void`

Resets the draw wrappers cache for all submeshes that are using this material

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1478

___

### serialize

▸ **serialize**(): `any`

Serializes this material

#### Returns

`any`

the serialized material object

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1724

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1616

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:867

___

### unbind

▸ **unbind**(): `void`

Unbinds the material from the mesh

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1222

___

### unfreeze

▸ **unfreeze**(): `void`

Unlocks updates for the material

#### Returns

`void`

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

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1739

___

### \_AllDirtyCallBack

▸ `Static` `Private` `Readonly` **_AllDirtyCallBack**(`defines`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `defines` | [`MaterialDefines`](MaterialDefines.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1407

___

### \_AttributeDirtyCallBack

▸ `Static` `Private` `Readonly` **_AttributeDirtyCallBack**(`defines`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `defines` | [`MaterialDefines`](MaterialDefines.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1414

___

### \_FresnelAndMiscDirtyCallBack

▸ `Static` `Private` **_FresnelAndMiscDirtyCallBack**(`defines`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `defines` | [`MaterialDefines`](MaterialDefines.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1416

___

### \_FresnelDirtyCallBack

▸ `Static` `Private` `Readonly` **_FresnelDirtyCallBack**(`defines`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `defines` | [`MaterialDefines`](MaterialDefines.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1410

___

### \_ImageProcessingDirtyCallBack

▸ `Static` `Private` `Readonly` **_ImageProcessingDirtyCallBack**(`defines`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `defines` | [`MaterialDefines`](MaterialDefines.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1408

___

### \_LightsDirtyCallBack

▸ `Static` `Private` `Readonly` **_LightsDirtyCallBack**(`defines`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `defines` | [`MaterialDefines`](MaterialDefines.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1413

___

### \_MiscDirtyCallBack

▸ `Static` `Private` `Readonly` **_MiscDirtyCallBack**(`defines`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `defines` | [`MaterialDefines`](MaterialDefines.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1411

___

### \_PrePassDirtyCallBack

▸ `Static` `Private` `Readonly` **_PrePassDirtyCallBack**(`defines`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `defines` | [`MaterialDefines`](MaterialDefines.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1412

___

### \_RunDirtyCallBacks

▸ `Static` `Private` `Readonly` **_RunDirtyCallBacks**(`defines`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `defines` | [`MaterialDefines`](MaterialDefines.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1427

___

### \_TextureAndMiscDirtyCallBack

▸ `Static` `Private` **_TextureAndMiscDirtyCallBack**(`defines`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `defines` | [`MaterialDefines`](MaterialDefines.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1421

___

### \_TextureDirtyCallBack

▸ `Static` `Private` `Readonly` **_TextureDirtyCallBack**(`defines`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `defines` | [`MaterialDefines`](MaterialDefines.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1409
