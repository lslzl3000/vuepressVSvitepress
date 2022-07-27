[@dev/core](../README.md) / [Exports](../modules.md) / MultiMaterial

# Class: MultiMaterial

A multi-material is used to apply different materials to different parts of the same object without the need of
separate meshes. This can be use to improve performances.

**`See`**

https://doc.babylonjs.com/how_to/multi_materials

## Hierarchy

- [`Material`](Material.md)

  ↳ **`MultiMaterial`**

## Table of contents

### Constructors

- [constructor](MultiMaterial.md#constructor)

### Properties

- [\_alpha](MultiMaterial.md#_alpha)
- [\_backFaceCulling](MultiMaterial.md#_backfaceculling)
- [\_cullBackFaces](MultiMaterial.md#_cullbackfaces)
- [\_drawWrapper](MultiMaterial.md#_drawwrapper)
- [\_eventInfo](MultiMaterial.md#_eventinfo)
- [\_forceAlphaTest](MultiMaterial.md#_forcealphatest)
- [\_needToBindSceneUbo](MultiMaterial.md#_needtobindsceneubo)
- [\_onEffectCreatedObservable](MultiMaterial.md#_oneffectcreatedobservable)
- [\_subMaterials](MultiMaterial.md#_submaterials)
- [\_transparencyMode](MultiMaterial.md#_transparencymode)
- [allowShaderHotSwapping](MultiMaterial.md#allowshaderhotswapping)
- [animations](MultiMaterial.md#animations)
- [checkReadyOnEveryCall](MultiMaterial.md#checkreadyoneverycall)
- [checkReadyOnlyOnce](MultiMaterial.md#checkreadyonlyonce)
- [customShaderNameResolve](MultiMaterial.md#customshadernameresolve)
- [depthFunction](MultiMaterial.md#depthfunction)
- [disableColorWrite](MultiMaterial.md#disablecolorwrite)
- [disableDepthWrite](MultiMaterial.md#disabledepthwrite)
- [doNotSerialize](MultiMaterial.md#donotserialize)
- [forceDepthWrite](MultiMaterial.md#forcedepthwrite)
- [getRenderTargetTextures](MultiMaterial.md#getrendertargettextures)
- [id](MultiMaterial.md#id)
- [inspectableCustomProperties](MultiMaterial.md#inspectablecustomproperties)
- [metadata](MultiMaterial.md#metadata)
- [name](MultiMaterial.md#name)
- [onCompiled](MultiMaterial.md#oncompiled)
- [onDisposeObservable](MultiMaterial.md#ondisposeobservable)
- [onError](MultiMaterial.md#onerror)
- [pluginManager](MultiMaterial.md#pluginmanager)
- [pointSize](MultiMaterial.md#pointsize)
- [reservedDataStore](MultiMaterial.md#reserveddatastore)
- [separateCullingPass](MultiMaterial.md#separatecullingpass)
- [shadowDepthWrapper](MultiMaterial.md#shadowdepthwrapper)
- [sideOrientation](MultiMaterial.md#sideorientation)
- [state](MultiMaterial.md#state)
- [stencil](MultiMaterial.md#stencil)
- [uniqueId](MultiMaterial.md#uniqueid)
- [zOffset](MultiMaterial.md#zoffset)
- [zOffsetUnits](MultiMaterial.md#zoffsetunits)
- [AllDirtyFlag](MultiMaterial.md#alldirtyflag)
- [AttributesDirtyFlag](MultiMaterial.md#attributesdirtyflag)
- [ClockWiseSideOrientation](MultiMaterial.md#clockwisesideorientation)
- [CounterClockWiseSideOrientation](MultiMaterial.md#counterclockwisesideorientation)
- [FresnelDirtyFlag](MultiMaterial.md#fresneldirtyflag)
- [LightDirtyFlag](MultiMaterial.md#lightdirtyflag)
- [LineListDrawMode](MultiMaterial.md#linelistdrawmode)
- [LineLoopDrawMode](MultiMaterial.md#lineloopdrawmode)
- [LineStripDrawMode](MultiMaterial.md#linestripdrawmode)
- [MATERIAL\_ALPHABLEND](MultiMaterial.md#material_alphablend)
- [MATERIAL\_ALPHATEST](MultiMaterial.md#material_alphatest)
- [MATERIAL\_ALPHATESTANDBLEND](MultiMaterial.md#material_alphatestandblend)
- [MATERIAL\_NORMALBLENDMETHOD\_RNM](MultiMaterial.md#material_normalblendmethod_rnm)
- [MATERIAL\_NORMALBLENDMETHOD\_WHITEOUT](MultiMaterial.md#material_normalblendmethod_whiteout)
- [MATERIAL\_OPAQUE](MultiMaterial.md#material_opaque)
- [MiscDirtyFlag](MultiMaterial.md#miscdirtyflag)
- [OnEventObservable](MultiMaterial.md#oneventobservable)
- [PointFillMode](MultiMaterial.md#pointfillmode)
- [PointListDrawMode](MultiMaterial.md#pointlistdrawmode)
- [PrePassDirtyFlag](MultiMaterial.md#prepassdirtyflag)
- [TextureDirtyFlag](MultiMaterial.md#texturedirtyflag)
- [TriangleFanDrawMode](MultiMaterial.md#trianglefandrawmode)
- [TriangleFillMode](MultiMaterial.md#trianglefillmode)
- [TriangleStripDrawMode](MultiMaterial.md#trianglestripdrawmode)
- [WireFrameFillMode](MultiMaterial.md#wireframefillmode)

### Accessors

- [\_disableAlphaBlending](MultiMaterial.md#_disablealphablending)
- [alpha](MultiMaterial.md#alpha)
- [alphaMode](MultiMaterial.md#alphamode)
- [backFaceCulling](MultiMaterial.md#backfaceculling)
- [canRenderToMRT](MultiMaterial.md#canrendertomrt)
- [cullBackFaces](MultiMaterial.md#cullbackfaces)
- [fillMode](MultiMaterial.md#fillmode)
- [fogEnabled](MultiMaterial.md#fogenabled)
- [hasRenderTargetTextures](MultiMaterial.md#hasrendertargettextures)
- [isFrozen](MultiMaterial.md#isfrozen)
- [isPrePassCapable](MultiMaterial.md#isprepasscapable)
- [needDepthPrePass](MultiMaterial.md#needdepthprepass)
- [onBind](MultiMaterial.md#onbind)
- [onBindObservable](MultiMaterial.md#onbindobservable)
- [onDispose](MultiMaterial.md#ondispose)
- [onEffectCreatedObservable](MultiMaterial.md#oneffectcreatedobservable)
- [onUnBindObservable](MultiMaterial.md#onunbindobservable)
- [pointsCloud](MultiMaterial.md#pointscloud)
- [subMaterials](MultiMaterial.md#submaterials)
- [transparencyMode](MultiMaterial.md#transparencymode)
- [wireframe](MultiMaterial.md#wireframe)

### Methods

- [\_afterBind](MultiMaterial.md#_afterbind)
- [\_hookArray](MultiMaterial.md#_hookarray)
- [\_markAllSubMeshesAsAllDirty](MultiMaterial.md#_markallsubmeshesasalldirty)
- [\_markAllSubMeshesAsAttributesDirty](MultiMaterial.md#_markallsubmeshesasattributesdirty)
- [\_markAllSubMeshesAsDirty](MultiMaterial.md#_markallsubmeshesasdirty)
- [\_markAllSubMeshesAsFresnelAndMiscDirty](MultiMaterial.md#_markallsubmeshesasfresnelandmiscdirty)
- [\_markAllSubMeshesAsFresnelDirty](MultiMaterial.md#_markallsubmeshesasfresneldirty)
- [\_markAllSubMeshesAsImageProcessingDirty](MultiMaterial.md#_markallsubmeshesasimageprocessingdirty)
- [\_markAllSubMeshesAsLightsDirty](MultiMaterial.md#_markallsubmeshesaslightsdirty)
- [\_markAllSubMeshesAsMiscDirty](MultiMaterial.md#_markallsubmeshesasmiscdirty)
- [\_markAllSubMeshesAsPrePassDirty](MultiMaterial.md#_markallsubmeshesasprepassdirty)
- [\_markAllSubMeshesAsTexturesAndMiscDirty](MultiMaterial.md#_markallsubmeshesastexturesandmiscdirty)
- [\_markAllSubMeshesAsTexturesDirty](MultiMaterial.md#_markallsubmeshesastexturesdirty)
- [\_markScenePrePassDirty](MultiMaterial.md#_marksceneprepassdirty)
- [\_shouldTurnAlphaTestOn](MultiMaterial.md#_shouldturnalphateston)
- [bind](MultiMaterial.md#bind)
- [bindEyePosition](MultiMaterial.md#bindeyeposition)
- [bindForSubMesh](MultiMaterial.md#bindforsubmesh)
- [bindOnlyWorldMatrix](MultiMaterial.md#bindonlyworldmatrix)
- [bindView](MultiMaterial.md#bindview)
- [bindViewProjection](MultiMaterial.md#bindviewprojection)
- [buildUniformLayout](MultiMaterial.md#builduniformlayout)
- [clone](MultiMaterial.md#clone)
- [dispose](MultiMaterial.md#dispose)
- [forceCompilation](MultiMaterial.md#forcecompilation)
- [forceCompilationAsync](MultiMaterial.md#forcecompilationasync)
- [freeze](MultiMaterial.md#freeze)
- [getActiveTextures](MultiMaterial.md#getactivetextures)
- [getAlphaTestTexture](MultiMaterial.md#getalphatesttexture)
- [getAnimatables](MultiMaterial.md#getanimatables)
- [getBindedMeshes](MultiMaterial.md#getbindedmeshes)
- [getChildren](MultiMaterial.md#getchildren)
- [getClassName](MultiMaterial.md#getclassname)
- [getEffect](MultiMaterial.md#geteffect)
- [getScene](MultiMaterial.md#getscene)
- [getSubMaterial](MultiMaterial.md#getsubmaterial)
- [hasTexture](MultiMaterial.md#hastexture)
- [isReady](MultiMaterial.md#isready)
- [isReadyForSubMesh](MultiMaterial.md#isreadyforsubmesh)
- [markAsDirty](MultiMaterial.md#markasdirty)
- [markDirty](MultiMaterial.md#markdirty)
- [needAlphaBlending](MultiMaterial.md#needalphablending)
- [needAlphaBlendingForMesh](MultiMaterial.md#needalphablendingformesh)
- [needAlphaTesting](MultiMaterial.md#needalphatesting)
- [resetDrawCache](MultiMaterial.md#resetdrawcache)
- [serialize](MultiMaterial.md#serialize)
- [setPrePassRenderer](MultiMaterial.md#setprepassrenderer)
- [toString](MultiMaterial.md#tostring)
- [unbind](MultiMaterial.md#unbind)
- [unfreeze](MultiMaterial.md#unfreeze)
- [Parse](MultiMaterial.md#parse)
- [ParseMultiMaterial](MultiMaterial.md#parsemultimaterial)

## Constructors

### constructor

• **new MultiMaterial**(`name`, `scene?`)

Instantiates a new Multi Material
A multi-material is used to apply different materials to different parts of the same object without the need of
separate meshes. This can be use to improve performances.

**`See`**

https://doc.babylonjs.com/how_to/multi_materials

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Define the name in the scene |
| `scene?` | [`Scene`](Scene.md) | Define the scene the material belongs to |

#### Overrides

[Material](Material.md).[constructor](Material.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Materials/multiMaterial.ts:49

## Properties

### \_alpha

• `Protected` **\_alpha**: `number` = `1.0`

The alpha value of the material

#### Inherited from

[Material](Material.md).[_alpha](Material.md#_alpha)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:292

___

### \_backFaceCulling

• `Protected` **\_backFaceCulling**: `boolean` = `true`

Specifies if back face culling is enabled

#### Inherited from

[Material](Material.md).[_backFaceCulling](Material.md#_backfaceculling)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:328

___

### \_cullBackFaces

• `Protected` **\_cullBackFaces**: `boolean` = `true`

Specifies if back or front faces should be culled (when culling is enabled)

#### Inherited from

[Material](Material.md).[_cullBackFaces](Material.md#_cullbackfaces)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:352

___

### \_drawWrapper

• `Protected` **\_drawWrapper**: `DrawWrapper`

#### Inherited from

[Material](Material.md).[_drawWrapper](Material.md#_drawwrapper)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:705

___

### \_eventInfo

• `Protected` **\_eventInfo**: `MaterialPluginDisposed` & `MaterialPluginHasTexture` & `MaterialPluginIsReadyForSubMesh` & `MaterialPluginGetDefineNames` & `MaterialPluginPrepareEffect` & `MaterialPluginPrepareDefines` & `MaterialPluginPrepareUniformBuffer` & `MaterialPluginBindForSubMesh` & `MaterialPluginGetAnimatables` & `MaterialPluginGetActiveTextures` & `MaterialPluginFillRenderTargetTextures` & `MaterialPluginHasRenderTargetTextures` & `MaterialPluginHardBindForSubMesh`

#### Inherited from

[Material](Material.md).[_eventInfo](Material.md#_eventinfo)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:770

___

### \_forceAlphaTest

• `Protected` **\_forceAlphaTest**: `boolean` = `false`

Enforces alpha test in opaque or blend mode in order to improve the performances of some situations.

#### Inherited from

[Material](Material.md).[_forceAlphaTest](Material.md#_forcealphatest)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:954

___

### \_needToBindSceneUbo

• `Protected` **\_needToBindSceneUbo**: `boolean`

#### Inherited from

[Material](Material.md).[_needToBindSceneUbo](Material.md#_needtobindsceneubo)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:727

___

### \_onEffectCreatedObservable

• `Protected` **\_onEffectCreatedObservable**: [`Nullable`](../modules.md#nullable)[`Observable`](Observable.md){ `effect`: [`Effect`](Effect.md) ; `subMesh`: [`Nullable`](../modules.md#nullable)[`SubMesh`](SubMesh.md)  }

#### Inherited from

[Material](Material.md).[_onEffectCreatedObservable](Material.md#_oneffectcreatedobservable)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:477

___

### \_subMaterials

• `Private` **\_subMaterials**: [`Nullable`](../modules.md#nullable)[`Material`](Material.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Materials/multiMaterial.ts:16

___

### \_transparencyMode

• `Protected` **\_transparencyMode**: [`Nullable`](../modules.md#nullable)`number` = `null`

The transparency mode of the material.

#### Inherited from

[Material](Material.md).[_transparencyMode](Material.md#_transparencymode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:959

___

### allowShaderHotSwapping

• **allowShaderHotSwapping**: `boolean` = `true`

Gets or sets a boolean indicating that the material is allowed (if supported) to do shader hot swapping.
This means that the material can keep using a previous shader while a new one is being compiled.
This is mostly used when shader parallel compilation is supported (true by default)

#### Inherited from

[Material](Material.md).[allowShaderHotSwapping](Material.md#allowshaderhotswapping)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:227

___

### animations

• **animations**: [`Nullable`](../modules.md#nullable)[`Animation`](Animation.md)[] = `null`

Stores the animations for the material

#### Inherited from

[Material](Material.md).[animations](Material.md#animations)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:415

___

### checkReadyOnEveryCall

• **checkReadyOnEveryCall**: `boolean` = `false`

Specifies if the ready state should be checked on each call

#### Inherited from

[Material](Material.md).[checkReadyOnEveryCall](Material.md#checkreadyoneverycall)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:265

___

### checkReadyOnlyOnce

• **checkReadyOnlyOnce**: `boolean` = `false`

Specifies if the ready state should be checked once

#### Inherited from

[Material](Material.md).[checkReadyOnlyOnce](Material.md#checkreadyonlyonce)

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

#### Inherited from

[Material](Material.md).[customShaderNameResolve](Material.md#customshadernameresolve)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:207

___

### depthFunction

• **depthFunction**: `number` = `0`

Specifies the depth function that should be used. 0 means the default engine function

#### Inherited from

[Material](Material.md).[depthFunction](Material.md#depthfunction)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:584

___

### disableColorWrite

• **disableColorWrite**: `boolean` = `false`

Specifies if color writing should be disabled

#### Inherited from

[Material](Material.md).[disableColorWrite](Material.md#disablecolorwrite)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:572

___

### disableDepthWrite

• **disableDepthWrite**: `boolean` = `false`

Specifies if depth writing should be disabled

#### Inherited from

[Material](Material.md).[disableDepthWrite](Material.md#disabledepthwrite)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:566

___

### doNotSerialize

• **doNotSerialize**: `boolean` = `false`

Specifies if the material should be serialized

#### Inherited from

[Material](Material.md).[doNotSerialize](Material.md#donotserialize)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:405

___

### forceDepthWrite

• **forceDepthWrite**: `boolean` = `false`

Specifies if depth writing should be forced

#### Inherited from

[Material](Material.md).[forceDepthWrite](Material.md#forcedepthwrite)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:578

___

### getRenderTargetTextures

• **getRenderTargetTextures**: [`Nullable`](../modules.md#nullable)() => [`SmartArray`](SmartArray.md)[`RenderTargetTexture`](RenderTargetTexture.md) = `null`

Callback triggered to get the render target textures

#### Inherited from

[Material](Material.md).[getRenderTargetTextures](Material.md#getrendertargettextures)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:391

___

### id

• **id**: `string`

The ID of the material

#### Inherited from

[Material](Material.md).[id](Material.md#id)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:233

___

### inspectableCustomProperties

• **inspectableCustomProperties**: [`IInspectable`](../interfaces/IInspectable.md)[]

List of inspectable custom properties (used by the Inspector)

**`See`**

https://doc.babylonjs.com/how_to/debug_layer#extensibility

#### Inherited from

[Material](Material.md).[inspectableCustomProperties](Material.md#inspectablecustomproperties)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:298

___

### metadata

• **metadata**: `any` = `null`

Gets or sets user defined metadata

#### Inherited from

[Material](Material.md).[metadata](Material.md#metadata)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:254

___

### name

• **name**: `string`

The name of the material

#### Inherited from

[Material](Material.md).[name](Material.md#name)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:248

___

### onCompiled

• **onCompiled**: [`Nullable`](../modules.md#nullable)(`effect`: [`Effect`](Effect.md)) => `void` = `null`

Callback triggered when the material is compiled

#### Inherited from

[Material](Material.md).[onCompiled](Material.md#oncompiled)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:381

___

### onDisposeObservable

• **onDisposeObservable**: [`Observable`](Observable.md)[`Material`](Material.md)

An event triggered when the material is disposed

#### Inherited from

[Material](Material.md).[onDisposeObservable](Material.md#ondisposeobservable)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:420

___

### onError

• **onError**: [`Nullable`](../modules.md#nullable)(`effect`: [`Effect`](Effect.md), `errors`: `string`) => `void` = `null`

Callback triggered when an error occurs

#### Inherited from

[Material](Material.md).[onError](Material.md#onerror)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:386

___

### pluginManager

• `Optional` **pluginManager**: [`MaterialPluginManager`](MaterialPluginManager.md)

Plugin manager for this material

#### Inherited from

[Material](Material.md).[pluginManager](Material.md#pluginmanager)

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginManager.ts:30

___

### pointSize

• **pointSize**: `number` = `1.0`

Stores the size of points

#### Inherited from

[Material](Material.md).[pointSize](Material.md#pointsize)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:620

___

### reservedDataStore

• **reservedDataStore**: `any` = `null`

For internal use only. Please do not use.

#### Inherited from

[Material](Material.md).[reservedDataStore](Material.md#reserveddatastore)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:259

___

### separateCullingPass

• **separateCullingPass**: `boolean` = `false`

Specifies if there should be a separate pass for culling

#### Inherited from

[Material](Material.md).[separateCullingPass](Material.md#separatecullingpass)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:590

___

### shadowDepthWrapper

• **shadowDepthWrapper**: [`Nullable`](../modules.md#nullable)[`ShadowDepthWrapper`](ShadowDepthWrapper.md) = `null`

Custom shadow depth material to use for shadow rendering instead of the in-built one

#### Inherited from

[Material](Material.md).[shadowDepthWrapper](Material.md#shadowdepthwrapper)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:220

___

### sideOrientation

• **sideOrientation**: `number`

Stores the value for side orientation

#### Inherited from

[Material](Material.md).[sideOrientation](Material.md#sideorientation)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:376

___

### state

• **state**: `string` = `""`

The state of the material

#### Inherited from

[Material](Material.md).[state](Material.md#state)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:277

___

### stencil

• `Readonly` **stencil**: `MaterialStencilState`

Gives access to the stencil properties of the material

#### Inherited from

[Material](Material.md).[stencil](Material.md#stencil)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:697

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the material

#### Inherited from

[Material](Material.md).[uniqueId](Material.md#uniqueid)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:239

___

### zOffset

• **zOffset**: `number` = `0`

Stores the z offset Factor value

#### Inherited from

[Material](Material.md).[zOffset](Material.md#zoffset)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:626

___

### zOffsetUnits

• **zOffsetUnits**: `number` = `0`

Stores the z offset Units value

#### Inherited from

[Material](Material.md).[zOffsetUnits](Material.md#zoffsetunits)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:632

___

### AllDirtyFlag

▪ `Static` `Readonly` **AllDirtyFlag**: ``63``

The all dirty flag value

#### Inherited from

[Material](Material.md).[AllDirtyFlag](Material.md#alldirtyflag)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:164

___

### AttributesDirtyFlag

▪ `Static` `Readonly` **AttributesDirtyFlag**: ``8``

The dirty attribute flag value

#### Inherited from

[Material](Material.md).[AttributesDirtyFlag](Material.md#attributesdirtyflag)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:149

___

### ClockWiseSideOrientation

▪ `Static` `Readonly` **ClockWiseSideOrientation**: ``0``

Stores the clock-wise side orientation

#### Inherited from

[Material](Material.md).[ClockWiseSideOrientation](Material.md#clockwisesideorientation)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:124

___

### CounterClockWiseSideOrientation

▪ `Static` `Readonly` **CounterClockWiseSideOrientation**: ``1``

Stores the counter clock-wise side orientation

#### Inherited from

[Material](Material.md).[CounterClockWiseSideOrientation](Material.md#counterclockwisesideorientation)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:129

___

### FresnelDirtyFlag

▪ `Static` `Readonly` **FresnelDirtyFlag**: ``4``

The dirty fresnel flag value

#### Inherited from

[Material](Material.md).[FresnelDirtyFlag](Material.md#fresneldirtyflag)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:144

___

### LightDirtyFlag

▪ `Static` `Readonly` **LightDirtyFlag**: ``2``

The dirty light flag value

#### Inherited from

[Material](Material.md).[LightDirtyFlag](Material.md#lightdirtyflag)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:139

___

### LineListDrawMode

▪ `Static` `Readonly` **LineListDrawMode**: ``4``

Returns the line list draw mode

#### Inherited from

[Material](Material.md).[LineListDrawMode](Material.md#linelistdrawmode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:103

___

### LineLoopDrawMode

▪ `Static` `Readonly` **LineLoopDrawMode**: ``5``

Returns the line loop draw mode

#### Inherited from

[Material](Material.md).[LineLoopDrawMode](Material.md#lineloopdrawmode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:107

___

### LineStripDrawMode

▪ `Static` `Readonly` **LineStripDrawMode**: ``6``

Returns the line strip draw mode

#### Inherited from

[Material](Material.md).[LineStripDrawMode](Material.md#linestripdrawmode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:111

___

### MATERIAL\_ALPHABLEND

▪ `Static` `Readonly` **MATERIAL\_ALPHABLEND**: ``2``

MaterialTransparencyMode: Pixels are blended (according to the alpha mode) with the already drawn pixels in the current frame buffer.

#### Inherited from

[Material](Material.md).[MATERIAL_ALPHABLEND](Material.md#material_alphablend)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:179

___

### MATERIAL\_ALPHATEST

▪ `Static` `Readonly` **MATERIAL\_ALPHATEST**: ``1``

MaterialTransparencyMode: Alpha Test mode, pixel are discarded below a certain threshold defined by the alpha cutoff value.

#### Inherited from

[Material](Material.md).[MATERIAL_ALPHATEST](Material.md#material_alphatest)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:174

___

### MATERIAL\_ALPHATESTANDBLEND

▪ `Static` `Readonly` **MATERIAL\_ALPHATESTANDBLEND**: ``3``

MaterialTransparencyMode: Pixels are blended (according to the alpha mode) with the already drawn pixels in the current frame buffer.
They are also discarded below the alpha cutoff threshold to improve performances.

#### Inherited from

[Material](Material.md).[MATERIAL_ALPHATESTANDBLEND](Material.md#material_alphatestandblend)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:185

___

### MATERIAL\_NORMALBLENDMETHOD\_RNM

▪ `Static` `Readonly` **MATERIAL\_NORMALBLENDMETHOD\_RNM**: ``1``

The Reoriented Normal Mapping method is used to blend normals.
Details of the algorithm can be found here: https://blog.selfshadow.com/publications/blending-in-detail/

#### Inherited from

[Material](Material.md).[MATERIAL_NORMALBLENDMETHOD_RNM](Material.md#material_normalblendmethod_rnm)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:197

___

### MATERIAL\_NORMALBLENDMETHOD\_WHITEOUT

▪ `Static` `Readonly` **MATERIAL\_NORMALBLENDMETHOD\_WHITEOUT**: ``0``

The Whiteout method is used to blend normals.
Details of the algorithm can be found here: https://blog.selfshadow.com/publications/blending-in-detail/

#### Inherited from

[Material](Material.md).[MATERIAL_NORMALBLENDMETHOD_WHITEOUT](Material.md#material_normalblendmethod_whiteout)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:191

___

### MATERIAL\_OPAQUE

▪ `Static` `Readonly` **MATERIAL\_OPAQUE**: ``0``

MaterialTransparencyMode: No transparency mode, Alpha channel is not use.

#### Inherited from

[Material](Material.md).[MATERIAL_OPAQUE](Material.md#material_opaque)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:169

___

### MiscDirtyFlag

▪ `Static` `Readonly` **MiscDirtyFlag**: ``16``

The dirty misc flag value

#### Inherited from

[Material](Material.md).[MiscDirtyFlag](Material.md#miscdirtyflag)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:154

___

### OnEventObservable

▪ `Static` **OnEventObservable**: [`Observable`](Observable.md)[`Material`](Material.md)

Event observable which raises global events common to all materials (like MaterialPluginEvent.Created)

#### Inherited from

[Material](Material.md).[OnEventObservable](Material.md#oneventobservable)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:202

___

### PointFillMode

▪ `Static` `Readonly` **PointFillMode**: ``2``

Returns the point fill mode

#### Inherited from

[Material](Material.md).[PointFillMode](Material.md#pointfillmode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:95

___

### PointListDrawMode

▪ `Static` `Readonly` **PointListDrawMode**: ``3``

Returns the point list draw mode

#### Inherited from

[Material](Material.md).[PointListDrawMode](Material.md#pointlistdrawmode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:99

___

### PrePassDirtyFlag

▪ `Static` `Readonly` **PrePassDirtyFlag**: ``32``

The dirty prepass flag value

#### Inherited from

[Material](Material.md).[PrePassDirtyFlag](Material.md#prepassdirtyflag)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:159

___

### TextureDirtyFlag

▪ `Static` `Readonly` **TextureDirtyFlag**: ``1``

The dirty texture flag value

#### Inherited from

[Material](Material.md).[TextureDirtyFlag](Material.md#texturedirtyflag)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:134

___

### TriangleFanDrawMode

▪ `Static` `Readonly` **TriangleFanDrawMode**: ``8``

Returns the triangle fan draw mode

#### Inherited from

[Material](Material.md).[TriangleFanDrawMode](Material.md#trianglefandrawmode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:119

___

### TriangleFillMode

▪ `Static` `Readonly` **TriangleFillMode**: ``0``

Returns the triangle fill mode

#### Inherited from

[Material](Material.md).[TriangleFillMode](Material.md#trianglefillmode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:87

___

### TriangleStripDrawMode

▪ `Static` `Readonly` **TriangleStripDrawMode**: ``7``

Returns the triangle strip draw mode

#### Inherited from

[Material](Material.md).[TriangleStripDrawMode](Material.md#trianglestripdrawmode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:115

___

### WireFrameFillMode

▪ `Static` `Readonly` **WireFrameFillMode**: ``1``

Returns the wireframe mode

#### Inherited from

[Material](Material.md).[WireFrameFillMode](Material.md#wireframefillmode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:91

## Accessors

### \_disableAlphaBlending

• `Protected` `get` **_disableAlphaBlending**(): `boolean`

Returns true if alpha blending should be disabled.

#### Returns

`boolean`

#### Inherited from

Material.\_disableAlphaBlending

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:995

___

### alpha

• `get` **alpha**(): `number`

Gets the alpha value of the material

#### Returns

`number`

#### Inherited from

Material.alpha

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

Material.alpha

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:303

___

### alphaMode

• `get` **alphaMode**(): `number`

Gets the value of the alpha mode

#### Returns

`number`

#### Inherited from

Material.alphaMode

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

Material.alphaMode

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:514

___

### backFaceCulling

• `get` **backFaceCulling**(): `boolean`

Gets the culling state

#### Returns

`boolean`

#### Inherited from

Material.backFaceCulling

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

Material.backFaceCulling

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:333

___

### canRenderToMRT

• `get` **canRenderToMRT**(): `boolean`

If the material can be rendered to several textures with MRT extension

#### Returns

`boolean`

#### Inherited from

Material.canRenderToMRT

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:282

___

### cullBackFaces

• `get` **cullBackFaces**(): `boolean`

Gets the type of faces that should be culled

#### Returns

`boolean`

#### Inherited from

Material.cullBackFaces

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

Material.cullBackFaces

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:357

___

### fillMode

• `get` **fillMode**(): `number`

Gets the material fill mode

#### Returns

`number`

#### Inherited from

Material.fillMode

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

Material.fillMode

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:685

___

### fogEnabled

• `get` **fogEnabled**(): `boolean`

Gets the value of the fog enabled state

#### Returns

`boolean`

#### Inherited from

Material.fogEnabled

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

Material.fogEnabled

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:601

___

### hasRenderTargetTextures

• `get` **hasRenderTargetTextures**(): `boolean`

Gets a boolean indicating that current material needs to register RTT

#### Returns

`boolean`

#### Inherited from

Material.hasRenderTargetTextures

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:396

___

### isFrozen

• `get` **isFrozen**(): `boolean`

Specifies if updates for the material been locked

#### Returns

`boolean`

#### Inherited from

Material.isFrozen

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:883

___

### isPrePassCapable

• `get` **isPrePassCapable**(): `boolean`

Can this material render to prepass

#### Returns

`boolean`

#### Inherited from

Material.isPrePassCapable

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:558

___

### needDepthPrePass

• `get` **needDepthPrePass**(): `boolean`

Gets the depth pre-pass value

#### Returns

`boolean`

#### Inherited from

Material.needDepthPrePass

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

Material.needDepthPrePass

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

Material.onBind

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:459

___

### onBindObservable

• `get` **onBindObservable**(): [`Observable`](Observable.md)[`AbstractMesh`](AbstractMesh.md)

An event triggered when the material is bound

#### Returns

[`Observable`](Observable.md)[`AbstractMesh`](AbstractMesh.md)

#### Inherited from

Material.onBindObservable

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

Material.onDispose

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:431

___

### onEffectCreatedObservable

• `get` **onEffectCreatedObservable**(): [`Observable`](Observable.md){ `effect`: [`Effect`](Effect.md) ; `subMesh`: [`Nullable`](../modules.md#nullable)[`SubMesh`](SubMesh.md)  }

An event triggered when the effect is (re)created

#### Returns

[`Observable`](Observable.md){ `effect`: [`Effect`](Effect.md) ; `subMesh`: [`Nullable`](../modules.md#nullable)[`SubMesh`](SubMesh.md)  }

#### Inherited from

Material.onEffectCreatedObservable

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:482

___

### onUnBindObservable

• `get` **onUnBindObservable**(): [`Observable`](Observable.md)[`Material`](Material.md)

An event triggered when the material is unbound

#### Returns

[`Observable`](Observable.md)[`Material`](Material.md)

#### Inherited from

Material.onUnBindObservable

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:469

___

### pointsCloud

• `get` **pointsCloud**(): `boolean`

Gets the value specifying if point clouds are enabled

#### Returns

`boolean`

#### Inherited from

Material.pointsCloud

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

Material.pointsCloud

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:670

___

### subMaterials

• `get` **subMaterials**(): [`Nullable`](../modules.md#nullable)[`Material`](Material.md)[]

Gets or Sets the list of Materials used within the multi material.
They need to be ordered according to the submeshes order in the associated mesh

#### Returns

[`Nullable`](../modules.md#nullable)[`Material`](Material.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Materials/multiMaterial.ts:24

• `set` **subMaterials**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`Material`](Material.md)[] |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/multiMaterial.ts:28

___

### transparencyMode

• `get` **transparencyMode**(): [`Nullable`](../modules.md#nullable)`number`

Gets the current transparency mode.

#### Returns

[`Nullable`](../modules.md#nullable)`number`

#### Inherited from

Material.transparencyMode

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

Material.transparencyMode

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:980

___

### wireframe

• `get` **wireframe**(): `boolean`

#### Returns

`boolean`

#### Inherited from

Material.wireframe

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

Material.wireframe

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

#### Inherited from

[Material](Material.md).[_afterBind](Material.md#_afterbind)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1181

___

### \_hookArray

▸ `Private` **_hookArray**(`array`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `array` | [`Nullable`](../modules.md#nullable)[`Material`](Material.md)[] |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/multiMaterial.ts:59

___

### \_markAllSubMeshesAsAllDirty

▸ `Protected` **_markAllSubMeshesAsAllDirty**(): `void`

Indicates that we need to re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

[Material](Material.md).[_markAllSubMeshesAsAllDirty](Material.md#_markallsubmeshesasalldirty)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1543

___

### \_markAllSubMeshesAsAttributesDirty

▸ `Protected` **_markAllSubMeshesAsAttributesDirty**(): `void`

Indicates that attributes need to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

[Material](Material.md).[_markAllSubMeshesAsAttributesDirty](Material.md#_markallsubmeshesasattributesdirty)

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

[Material](Material.md).[_markAllSubMeshesAsDirty](Material.md#_markallsubmeshesasdirty)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1498

___

### \_markAllSubMeshesAsFresnelAndMiscDirty

▸ `Protected` **_markAllSubMeshesAsFresnelAndMiscDirty**(): `void`

Indicates that fresnel and misc need to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

[Material](Material.md).[_markAllSubMeshesAsFresnelAndMiscDirty](Material.md#_markallsubmeshesasfresnelandmiscdirty)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1571

___

### \_markAllSubMeshesAsFresnelDirty

▸ `Protected` **_markAllSubMeshesAsFresnelDirty**(): `void`

Indicates that fresnel needs to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

[Material](Material.md).[_markAllSubMeshesAsFresnelDirty](Material.md#_markallsubmeshesasfresneldirty)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1564

___

### \_markAllSubMeshesAsImageProcessingDirty

▸ `Protected` **_markAllSubMeshesAsImageProcessingDirty**(): `void`

Indicates that image processing needs to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

[Material](Material.md).[_markAllSubMeshesAsImageProcessingDirty](Material.md#_markallsubmeshesasimageprocessingdirty)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1550

___

### \_markAllSubMeshesAsLightsDirty

▸ `Protected` **_markAllSubMeshesAsLightsDirty**(): `void`

Indicates that lights need to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

[Material](Material.md).[_markAllSubMeshesAsLightsDirty](Material.md#_markallsubmeshesaslightsdirty)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1578

___

### \_markAllSubMeshesAsMiscDirty

▸ `Protected` **_markAllSubMeshesAsMiscDirty**(): `void`

Indicates that misc needs to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

[Material](Material.md).[_markAllSubMeshesAsMiscDirty](Material.md#_markallsubmeshesasmiscdirty)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1592

___

### \_markAllSubMeshesAsPrePassDirty

▸ `Protected` **_markAllSubMeshesAsPrePassDirty**(): `void`

Indicates that prepass needs to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

[Material](Material.md).[_markAllSubMeshesAsPrePassDirty](Material.md#_markallsubmeshesasprepassdirty)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1599

___

### \_markAllSubMeshesAsTexturesAndMiscDirty

▸ `Protected` **_markAllSubMeshesAsTexturesAndMiscDirty**(): `void`

Indicates that textures and misc need to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

[Material](Material.md).[_markAllSubMeshesAsTexturesAndMiscDirty](Material.md#_markallsubmeshesastexturesandmiscdirty)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1606

___

### \_markAllSubMeshesAsTexturesDirty

▸ `Protected` **_markAllSubMeshesAsTexturesDirty**(): `void`

Indicates that textures need to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

[Material](Material.md).[_markAllSubMeshesAsTexturesDirty](Material.md#_markallsubmeshesastexturesdirty)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1557

___

### \_markScenePrePassDirty

▸ `Protected` **_markScenePrePassDirty**(): `void`

Indicates that the scene should check if the rendering now needs a prepass

#### Returns

`void`

#### Inherited from

[Material](Material.md).[_markScenePrePassDirty](Material.md#_marksceneprepassdirty)

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

#### Inherited from

[Material](Material.md).[_shouldTurnAlphaTestOn](Material.md#_shouldturnalphateston)

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

#### Inherited from

[Material](Material.md).[bind](Material.md#bind)

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

#### Inherited from

[Material](Material.md).[bindEyePosition](Material.md#bindeyeposition)

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

#### Inherited from

[Material](Material.md).[bindForSubMesh](Material.md#bindforsubmesh)

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

#### Inherited from

[Material](Material.md).[bindOnlyWorldMatrix](Material.md#bindonlyworldmatrix)

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

#### Inherited from

[Material](Material.md).[bindView](Material.md#bindview)

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

[Material](Material.md).[bindViewProjection](Material.md#bindviewprojection)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1154

___

### buildUniformLayout

▸ **buildUniformLayout**(): `void`

Initializes the uniform buffer layout for the shader.

#### Returns

`void`

#### Inherited from

[Material](Material.md).[buildUniformLayout](Material.md#builduniformlayout)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1104

___

### clone

▸ **clone**(`name`, `cloneChildren?`): [`MultiMaterial`](MultiMaterial.md)

Clones the current material and its related sub materials

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Define the name of the newly cloned material |
| `cloneChildren?` | `boolean` | Define if submaterial will be cloned or shared with the parent instance |

#### Returns

[`MultiMaterial`](MultiMaterial.md)

the cloned material

#### Overrides

[Material](Material.md).[clone](Material.md#clone)

#### Defined in

https://github.com/babylon.js/core/src/Materials/multiMaterial.ts:169

___

### dispose

▸ **dispose**(`forceDisposeEffect?`, `forceDisposeTextures?`, `forceDisposeChildren?`): `void`

Dispose the material and release its associated resources

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `forceDisposeEffect?` | `boolean` | Define if we want to force disposing the associated effect (if false the shader is not released and could be reuse later on) |
| `forceDisposeTextures?` | `boolean` | Define if we want to force disposing the associated textures (if false, they will not be disposed and can still be use elsewhere in the app) |
| `forceDisposeChildren?` | `boolean` | Define if we want to force disposing the associated submaterials (if false, they will not be disposed and can still be use elsewhere in the app) |

#### Returns

`void`

#### Overrides

[Material](Material.md).[dispose](Material.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Materials/multiMaterial.ts:223

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

[Material](Material.md).[forceCompilation](Material.md#forcecompilation)

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

#### Inherited from

[Material](Material.md).[forceCompilationAsync](Material.md#forcecompilationasync)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1392

___

### freeze

▸ **freeze**(): `void`

Locks updates for the material

#### Returns

`void`

#### Inherited from

[Material](Material.md).[freeze](Material.md#freeze)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:890

___

### getActiveTextures

▸ **getActiveTextures**(): [`BaseTexture`](BaseTexture.md)[]

Get the list of active textures for the whole sub materials list.

#### Returns

[`BaseTexture`](BaseTexture.md)[]

All the textures that will be used during the rendering

#### Overrides

[Material](Material.md).[getActiveTextures](Material.md#getactivetextures)

#### Defined in

https://github.com/babylon.js/core/src/Materials/multiMaterial.ts:96

___

### getAlphaTestTexture

▸ **getAlphaTestTexture**(): [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Gets the texture used for the alpha test

#### Returns

[`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

the texture to use for alpha testing

#### Inherited from

[Material](Material.md).[getAlphaTestTexture](Material.md#getalphatesttexture)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1048

___

### getAnimatables

▸ **getAnimatables**(): [`IAnimatable`](../interfaces/IAnimatable.md)[]

Returns the animatable textures.

#### Returns

[`IAnimatable`](../interfaces/IAnimatable.md)[]

- Array of animatable textures.

#### Inherited from

[Material](Material.md).[getAnimatables](Material.md#getanimatables)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1247

___

### getBindedMeshes

▸ **getBindedMeshes**(): [`AbstractMesh`](AbstractMesh.md)[]

Gets the meshes bound to the material

#### Returns

[`AbstractMesh`](AbstractMesh.md)[]

an array of meshes bound to the material

#### Inherited from

[Material](Material.md).[getBindedMeshes](Material.md#getbindedmeshes)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1289

___

### getChildren

▸ **getChildren**(): [`Nullable`](../modules.md#nullable)[`Material`](Material.md)[]

Function used to align with Node.getChildren()

#### Returns

[`Nullable`](../modules.md#nullable)[`Material`](Material.md)[]

the list of Materials used within the multi material

#### Defined in

https://github.com/babylon.js/core/src/Materials/multiMaterial.ts:37

___

### getClassName

▸ **getClassName**(): `string`

Gets the current class name of the material e.g. "MultiMaterial"
Mainly use in serialization.

#### Returns

`string`

the class name

#### Overrides

[Material](Material.md).[getClassName](Material.md#getclassname)

#### Defined in

https://github.com/babylon.js/core/src/Materials/multiMaterial.ts:132

___

### getEffect

▸ **getEffect**(): [`Nullable`](../modules.md#nullable)[`Effect`](Effect.md)

Returns the material effect

#### Returns

[`Nullable`](../modules.md#nullable)[`Effect`](Effect.md)

the effect associated with the material

#### Inherited from

[Material](Material.md).[getEffect](Material.md#geteffect)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:939

___

### getScene

▸ **getScene**(): [`Scene`](Scene.md)

Returns the current scene

#### Returns

[`Scene`](Scene.md)

a Scene

#### Inherited from

[Material](Material.md).[getScene](Material.md#getscene)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:947

___

### getSubMaterial

▸ **getSubMaterial**(`index`): [`Nullable`](../modules.md#nullable)[`Material`](Material.md)

Get one of the submaterial by its index in the submaterials array

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | The index to look the sub material at |

#### Returns

[`Nullable`](../modules.md#nullable)[`Material`](Material.md)

The Material if the index has been defined

#### Defined in

https://github.com/babylon.js/core/src/Materials/multiMaterial.ts:84

___

### hasTexture

▸ **hasTexture**(`texture`): `boolean`

Specifies if any sub-materials of this multi-material use a given texture.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `texture` | [`BaseTexture`](BaseTexture.md) | Defines the texture to check against this multi-material's sub-materials. |

#### Returns

`boolean`

A boolean specifying if any sub-material of this multi-material uses the texture.

#### Overrides

[Material](Material.md).[hasTexture](Material.md#hastexture)

#### Defined in

https://github.com/babylon.js/core/src/Materials/multiMaterial.ts:113

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

#### Inherited from

[Material](Material.md).[isReady](Material.md#isready)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:910

___

### isReadyForSubMesh

▸ **isReadyForSubMesh**(`mesh`, `subMesh`, `useInstances?`): `boolean`

Checks if the material is ready to render the requested sub mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | Define the mesh the submesh belongs to |
| `subMesh` | [`SubMesh`](SubMesh.md) | Define the sub mesh to look readiness for |
| `useInstances?` | `boolean` | Define whether or not the material is used with instances |

#### Returns

`boolean`

true if ready, otherwise false

#### Overrides

[Material](Material.md).[isReadyForSubMesh](Material.md#isreadyforsubmesh)

#### Defined in

https://github.com/babylon.js/core/src/Materials/multiMaterial.ts:143

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

[Material](Material.md).[markAsDirty](Material.md#markasdirty)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1437

___

### markDirty

▸ **markDirty**(): `void`

Marks the material to indicate that it needs to be re-calculated

#### Returns

`void`

#### Inherited from

[Material](Material.md).[markDirty](Material.md#markdirty)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1055

___

### needAlphaBlending

▸ **needAlphaBlending**(): `boolean`

Specifies whether or not this material should be rendered in alpha blend mode.

#### Returns

`boolean`

a boolean specifying if alpha blending is needed

#### Inherited from

[Material](Material.md).[needAlphaBlending](Material.md#needalphablending)

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

#### Inherited from

[Material](Material.md).[needAlphaBlendingForMesh](Material.md#needalphablendingformesh)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1016

___

### needAlphaTesting

▸ **needAlphaTesting**(): `boolean`

Specifies whether or not this material should be rendered in alpha test mode.

#### Returns

`boolean`

a boolean specifying if an alpha test is needed.

#### Inherited from

[Material](Material.md).[needAlphaTesting](Material.md#needalphatesting)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1028

___

### resetDrawCache

▸ **resetDrawCache**(): `void`

Resets the draw wrappers cache for all submeshes that are using this material

#### Returns

`void`

#### Inherited from

[Material](Material.md).[resetDrawCache](Material.md#resetdrawcache)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1478

___

### serialize

▸ **serialize**(): `any`

Serializes the materials into a JSON representation.

#### Returns

`any`

the JSON representation

#### Overrides

[Material](Material.md).[serialize](Material.md#serialize)

#### Defined in

https://github.com/babylon.js/core/src/Materials/multiMaterial.ts:190

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

[Material](Material.md).[setPrePassRenderer](Material.md#setprepassrenderer)

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

#### Inherited from

[Material](Material.md).[toString](Material.md#tostring)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:867

___

### unbind

▸ **unbind**(): `void`

Unbinds the material from the mesh

#### Returns

`void`

#### Inherited from

[Material](Material.md).[unbind](Material.md#unbind)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1222

___

### unfreeze

▸ **unfreeze**(): `void`

Unlocks updates for the material

#### Returns

`void`

#### Inherited from

[Material](Material.md).[unfreeze](Material.md#unfreeze)

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

[Material](Material.md).[Parse](Material.md#parse)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1739

___

### ParseMultiMaterial

▸ `Static` **ParseMultiMaterial**(`parsedMultiMaterial`, `scene`): [`MultiMaterial`](MultiMaterial.md)

Creates a MultiMaterial from parsed MultiMaterial data.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `parsedMultiMaterial` | `any` | defines parsed MultiMaterial data. |
| `scene` | [`Scene`](Scene.md) | defines the hosting scene |

#### Returns

[`MultiMaterial`](MultiMaterial.md)

a new MultiMaterial

#### Defined in

https://github.com/babylon.js/core/src/Materials/multiMaterial.ts:252
