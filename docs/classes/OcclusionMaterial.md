[@dev/core](../README.md) / [Exports](../modules.md) / OcclusionMaterial

# Class: OcclusionMaterial

A material to use for fast depth-only rendering.

**`Since`**

5.0.0

## Hierarchy

- [`ShaderMaterial`](ShaderMaterial.md)

  ↳ **`OcclusionMaterial`**

## Table of contents

### Constructors

- [constructor](OcclusionMaterial.md#constructor)

### Properties

- [\_activeEffect](OcclusionMaterial.md#_activeeffect)
- [\_alpha](OcclusionMaterial.md#_alpha)
- [\_backFaceCulling](OcclusionMaterial.md#_backfaceculling)
- [\_cullBackFaces](OcclusionMaterial.md#_cullbackfaces)
- [\_drawWrapper](OcclusionMaterial.md#_drawwrapper)
- [\_eventInfo](OcclusionMaterial.md#_eventinfo)
- [\_forceAlphaTest](OcclusionMaterial.md#_forcealphatest)
- [\_needToBindSceneUbo](OcclusionMaterial.md#_needtobindsceneubo)
- [\_normalMatrix](OcclusionMaterial.md#_normalmatrix)
- [\_onEffectCreatedObservable](OcclusionMaterial.md#_oneffectcreatedobservable)
- [\_transparencyMode](OcclusionMaterial.md#_transparencymode)
- [allowShaderHotSwapping](OcclusionMaterial.md#allowshaderhotswapping)
- [animations](OcclusionMaterial.md#animations)
- [checkReadyOnEveryCall](OcclusionMaterial.md#checkreadyoneverycall)
- [checkReadyOnlyOnce](OcclusionMaterial.md#checkreadyonlyonce)
- [customShaderNameResolve](OcclusionMaterial.md#customshadernameresolve)
- [depthFunction](OcclusionMaterial.md#depthfunction)
- [disableColorWrite](OcclusionMaterial.md#disablecolorwrite)
- [disableDepthWrite](OcclusionMaterial.md#disabledepthwrite)
- [doNotSerialize](OcclusionMaterial.md#donotserialize)
- [forceDepthWrite](OcclusionMaterial.md#forcedepthwrite)
- [getRenderTargetTextures](OcclusionMaterial.md#getrendertargettextures)
- [id](OcclusionMaterial.md#id)
- [inspectableCustomProperties](OcclusionMaterial.md#inspectablecustomproperties)
- [metadata](OcclusionMaterial.md#metadata)
- [name](OcclusionMaterial.md#name)
- [onCompiled](OcclusionMaterial.md#oncompiled)
- [onDisposeObservable](OcclusionMaterial.md#ondisposeobservable)
- [onError](OcclusionMaterial.md#onerror)
- [pluginManager](OcclusionMaterial.md#pluginmanager)
- [pointSize](OcclusionMaterial.md#pointsize)
- [reservedDataStore](OcclusionMaterial.md#reserveddatastore)
- [separateCullingPass](OcclusionMaterial.md#separatecullingpass)
- [shadowDepthWrapper](OcclusionMaterial.md#shadowdepthwrapper)
- [sideOrientation](OcclusionMaterial.md#sideorientation)
- [snippetId](OcclusionMaterial.md#snippetid)
- [state](OcclusionMaterial.md#state)
- [stencil](OcclusionMaterial.md#stencil)
- [uniqueId](OcclusionMaterial.md#uniqueid)
- [zOffset](OcclusionMaterial.md#zoffset)
- [zOffsetUnits](OcclusionMaterial.md#zoffsetunits)
- [AllDirtyFlag](OcclusionMaterial.md#alldirtyflag)
- [AttributesDirtyFlag](OcclusionMaterial.md#attributesdirtyflag)
- [ClockWiseSideOrientation](OcclusionMaterial.md#clockwisesideorientation)
- [CounterClockWiseSideOrientation](OcclusionMaterial.md#counterclockwisesideorientation)
- [CreateFromSnippetAsync](OcclusionMaterial.md#createfromsnippetasync)
- [FresnelDirtyFlag](OcclusionMaterial.md#fresneldirtyflag)
- [LightDirtyFlag](OcclusionMaterial.md#lightdirtyflag)
- [LineListDrawMode](OcclusionMaterial.md#linelistdrawmode)
- [LineLoopDrawMode](OcclusionMaterial.md#lineloopdrawmode)
- [LineStripDrawMode](OcclusionMaterial.md#linestripdrawmode)
- [MATERIAL\_ALPHABLEND](OcclusionMaterial.md#material_alphablend)
- [MATERIAL\_ALPHATEST](OcclusionMaterial.md#material_alphatest)
- [MATERIAL\_ALPHATESTANDBLEND](OcclusionMaterial.md#material_alphatestandblend)
- [MATERIAL\_NORMALBLENDMETHOD\_RNM](OcclusionMaterial.md#material_normalblendmethod_rnm)
- [MATERIAL\_NORMALBLENDMETHOD\_WHITEOUT](OcclusionMaterial.md#material_normalblendmethod_whiteout)
- [MATERIAL\_OPAQUE](OcclusionMaterial.md#material_opaque)
- [MiscDirtyFlag](OcclusionMaterial.md#miscdirtyflag)
- [OnEventObservable](OcclusionMaterial.md#oneventobservable)
- [PointFillMode](OcclusionMaterial.md#pointfillmode)
- [PointListDrawMode](OcclusionMaterial.md#pointlistdrawmode)
- [PrePassDirtyFlag](OcclusionMaterial.md#prepassdirtyflag)
- [SnippetUrl](OcclusionMaterial.md#snippeturl)
- [TextureDirtyFlag](OcclusionMaterial.md#texturedirtyflag)
- [TriangleFanDrawMode](OcclusionMaterial.md#trianglefandrawmode)
- [TriangleFillMode](OcclusionMaterial.md#trianglefillmode)
- [TriangleStripDrawMode](OcclusionMaterial.md#trianglestripdrawmode)
- [WireFrameFillMode](OcclusionMaterial.md#wireframefillmode)

### Accessors

- [\_disableAlphaBlending](OcclusionMaterial.md#_disablealphablending)
- [alpha](OcclusionMaterial.md#alpha)
- [alphaMode](OcclusionMaterial.md#alphamode)
- [backFaceCulling](OcclusionMaterial.md#backfaceculling)
- [canRenderToMRT](OcclusionMaterial.md#canrendertomrt)
- [cullBackFaces](OcclusionMaterial.md#cullbackfaces)
- [fillMode](OcclusionMaterial.md#fillmode)
- [fogEnabled](OcclusionMaterial.md#fogenabled)
- [hasRenderTargetTextures](OcclusionMaterial.md#hasrendertargettextures)
- [isFrozen](OcclusionMaterial.md#isfrozen)
- [isPrePassCapable](OcclusionMaterial.md#isprepasscapable)
- [needDepthPrePass](OcclusionMaterial.md#needdepthprepass)
- [onBind](OcclusionMaterial.md#onbind)
- [onBindObservable](OcclusionMaterial.md#onbindobservable)
- [onDispose](OcclusionMaterial.md#ondispose)
- [onEffectCreatedObservable](OcclusionMaterial.md#oneffectcreatedobservable)
- [onUnBindObservable](OcclusionMaterial.md#onunbindobservable)
- [options](OcclusionMaterial.md#options)
- [pointsCloud](OcclusionMaterial.md#pointscloud)
- [shaderPath](OcclusionMaterial.md#shaderpath)
- [transparencyMode](OcclusionMaterial.md#transparencymode)
- [wireframe](OcclusionMaterial.md#wireframe)

### Methods

- [\_afterBind](OcclusionMaterial.md#_afterbind)
- [\_isReadyForSubMesh](OcclusionMaterial.md#_isreadyforsubmesh)
- [\_markAllSubMeshesAsAllDirty](OcclusionMaterial.md#_markallsubmeshesasalldirty)
- [\_markAllSubMeshesAsAttributesDirty](OcclusionMaterial.md#_markallsubmeshesasattributesdirty)
- [\_markAllSubMeshesAsDirty](OcclusionMaterial.md#_markallsubmeshesasdirty)
- [\_markAllSubMeshesAsFresnelAndMiscDirty](OcclusionMaterial.md#_markallsubmeshesasfresnelandmiscdirty)
- [\_markAllSubMeshesAsFresnelDirty](OcclusionMaterial.md#_markallsubmeshesasfresneldirty)
- [\_markAllSubMeshesAsImageProcessingDirty](OcclusionMaterial.md#_markallsubmeshesasimageprocessingdirty)
- [\_markAllSubMeshesAsLightsDirty](OcclusionMaterial.md#_markallsubmeshesaslightsdirty)
- [\_markAllSubMeshesAsMiscDirty](OcclusionMaterial.md#_markallsubmeshesasmiscdirty)
- [\_markAllSubMeshesAsPrePassDirty](OcclusionMaterial.md#_markallsubmeshesasprepassdirty)
- [\_markAllSubMeshesAsTexturesAndMiscDirty](OcclusionMaterial.md#_markallsubmeshesastexturesandmiscdirty)
- [\_markAllSubMeshesAsTexturesDirty](OcclusionMaterial.md#_markallsubmeshesastexturesdirty)
- [\_markScenePrePassDirty](OcclusionMaterial.md#_marksceneprepassdirty)
- [\_mustRebind](OcclusionMaterial.md#_mustrebind)
- [\_shouldTurnAlphaTestOn](OcclusionMaterial.md#_shouldturnalphateston)
- [bind](OcclusionMaterial.md#bind)
- [bindEyePosition](OcclusionMaterial.md#bindeyeposition)
- [bindForSubMesh](OcclusionMaterial.md#bindforsubmesh)
- [bindOnlyNormalMatrix](OcclusionMaterial.md#bindonlynormalmatrix)
- [bindOnlyWorldMatrix](OcclusionMaterial.md#bindonlyworldmatrix)
- [bindView](OcclusionMaterial.md#bindview)
- [bindViewProjection](OcclusionMaterial.md#bindviewprojection)
- [buildUniformLayout](OcclusionMaterial.md#builduniformlayout)
- [clone](OcclusionMaterial.md#clone)
- [dispose](OcclusionMaterial.md#dispose)
- [forceCompilation](OcclusionMaterial.md#forcecompilation)
- [forceCompilationAsync](OcclusionMaterial.md#forcecompilationasync)
- [freeze](OcclusionMaterial.md#freeze)
- [getActiveTextures](OcclusionMaterial.md#getactivetextures)
- [getAlphaTestTexture](OcclusionMaterial.md#getalphatesttexture)
- [getAnimatables](OcclusionMaterial.md#getanimatables)
- [getBindedMeshes](OcclusionMaterial.md#getbindedmeshes)
- [getClassName](OcclusionMaterial.md#getclassname)
- [getEffect](OcclusionMaterial.md#geteffect)
- [getScene](OcclusionMaterial.md#getscene)
- [hasTexture](OcclusionMaterial.md#hastexture)
- [isReady](OcclusionMaterial.md#isready)
- [isReadyForSubMesh](OcclusionMaterial.md#isreadyforsubmesh)
- [markAsDirty](OcclusionMaterial.md#markasdirty)
- [markDirty](OcclusionMaterial.md#markdirty)
- [needAlphaBlending](OcclusionMaterial.md#needalphablending)
- [needAlphaBlendingForMesh](OcclusionMaterial.md#needalphablendingformesh)
- [needAlphaTesting](OcclusionMaterial.md#needalphatesting)
- [resetDrawCache](OcclusionMaterial.md#resetdrawcache)
- [serialize](OcclusionMaterial.md#serialize)
- [setArray2](OcclusionMaterial.md#setarray2)
- [setArray3](OcclusionMaterial.md#setarray3)
- [setArray4](OcclusionMaterial.md#setarray4)
- [setColor3](OcclusionMaterial.md#setcolor3)
- [setColor3Array](OcclusionMaterial.md#setcolor3array)
- [setColor4](OcclusionMaterial.md#setcolor4)
- [setColor4Array](OcclusionMaterial.md#setcolor4array)
- [setExternalTexture](OcclusionMaterial.md#setexternaltexture)
- [setFloat](OcclusionMaterial.md#setfloat)
- [setFloats](OcclusionMaterial.md#setfloats)
- [setInt](OcclusionMaterial.md#setint)
- [setMatrices](OcclusionMaterial.md#setmatrices)
- [setMatrix](OcclusionMaterial.md#setmatrix)
- [setMatrix2x2](OcclusionMaterial.md#setmatrix2x2)
- [setMatrix3x3](OcclusionMaterial.md#setmatrix3x3)
- [setPrePassRenderer](OcclusionMaterial.md#setprepassrenderer)
- [setQuaternion](OcclusionMaterial.md#setquaternion)
- [setQuaternionArray](OcclusionMaterial.md#setquaternionarray)
- [setStorageBuffer](OcclusionMaterial.md#setstoragebuffer)
- [setTexture](OcclusionMaterial.md#settexture)
- [setTextureArray](OcclusionMaterial.md#settexturearray)
- [setTextureSampler](OcclusionMaterial.md#settexturesampler)
- [setUniformBuffer](OcclusionMaterial.md#setuniformbuffer)
- [setVector2](OcclusionMaterial.md#setvector2)
- [setVector3](OcclusionMaterial.md#setvector3)
- [setVector4](OcclusionMaterial.md#setvector4)
- [toString](OcclusionMaterial.md#tostring)
- [unbind](OcclusionMaterial.md#unbind)
- [unfreeze](OcclusionMaterial.md#unfreeze)
- [Parse](OcclusionMaterial.md#parse)
- [ParseFromFileAsync](OcclusionMaterial.md#parsefromfileasync)
- [ParseFromSnippetAsync](OcclusionMaterial.md#parsefromsnippetasync)

## Constructors

### constructor

• **new OcclusionMaterial**(`name`, `scene`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `scene` | [`Scene`](Scene.md) |

#### Overrides

[ShaderMaterial](ShaderMaterial.md).[constructor](ShaderMaterial.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Occlusion/occlusionMaterial.ts:13

## Properties

### \_activeEffect

• `Protected` **\_activeEffect**: [`Effect`](Effect.md)

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[_activeEffect](ShaderMaterial.md#_activeeffect)

#### Defined in

https://github.com/babylon.js/core/src/Materials/pushMaterial.ts:14

___

### \_alpha

• `Protected` **\_alpha**: `number` = `1.0`

The alpha value of the material

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[_alpha](ShaderMaterial.md#_alpha)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:292

___

### \_backFaceCulling

• `Protected` **\_backFaceCulling**: `boolean` = `true`

Specifies if back face culling is enabled

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[_backFaceCulling](ShaderMaterial.md#_backfaceculling)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:328

___

### \_cullBackFaces

• `Protected` **\_cullBackFaces**: `boolean` = `true`

Specifies if back or front faces should be culled (when culling is enabled)

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[_cullBackFaces](ShaderMaterial.md#_cullbackfaces)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:352

___

### \_drawWrapper

• `Protected` **\_drawWrapper**: `DrawWrapper`

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[_drawWrapper](ShaderMaterial.md#_drawwrapper)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:705

___

### \_eventInfo

• `Protected` **\_eventInfo**: `MaterialPluginDisposed` & `MaterialPluginHasTexture` & `MaterialPluginIsReadyForSubMesh` & `MaterialPluginGetDefineNames` & `MaterialPluginPrepareEffect` & `MaterialPluginPrepareDefines` & `MaterialPluginPrepareUniformBuffer` & `MaterialPluginBindForSubMesh` & `MaterialPluginGetAnimatables` & `MaterialPluginGetActiveTextures` & `MaterialPluginFillRenderTargetTextures` & `MaterialPluginHasRenderTargetTextures` & `MaterialPluginHardBindForSubMesh`

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[_eventInfo](ShaderMaterial.md#_eventinfo)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:770

___

### \_forceAlphaTest

• `Protected` **\_forceAlphaTest**: `boolean` = `false`

Enforces alpha test in opaque or blend mode in order to improve the performances of some situations.

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[_forceAlphaTest](ShaderMaterial.md#_forcealphatest)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:954

___

### \_needToBindSceneUbo

• `Protected` **\_needToBindSceneUbo**: `boolean`

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[_needToBindSceneUbo](ShaderMaterial.md#_needtobindsceneubo)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:727

___

### \_normalMatrix

• `Protected` **\_normalMatrix**: [`Matrix`](Matrix.md)

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[_normalMatrix](ShaderMaterial.md#_normalmatrix)

#### Defined in

https://github.com/babylon.js/core/src/Materials/pushMaterial.ts:16

___

### \_onEffectCreatedObservable

• `Protected` **\_onEffectCreatedObservable**: [`Nullable`](../modules.md#nullable)[`Observable`](Observable.md){ `effect`: [`Effect`](Effect.md) ; `subMesh`: [`Nullable`](../modules.md#nullable)[`SubMesh`](SubMesh.md)  }

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[_onEffectCreatedObservable](ShaderMaterial.md#_oneffectcreatedobservable)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:477

___

### \_transparencyMode

• `Protected` **\_transparencyMode**: [`Nullable`](../modules.md#nullable)`number` = `null`

The transparency mode of the material.

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[_transparencyMode](ShaderMaterial.md#_transparencymode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:959

___

### allowShaderHotSwapping

• **allowShaderHotSwapping**: `boolean` = `true`

Gets or sets a boolean indicating that the material is allowed (if supported) to do shader hot swapping.
This means that the material can keep using a previous shader while a new one is being compiled.
This is mostly used when shader parallel compilation is supported (true by default)

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[allowShaderHotSwapping](ShaderMaterial.md#allowshaderhotswapping)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:227

___

### animations

• **animations**: [`Nullable`](../modules.md#nullable)[`Animation`](Animation.md)[] = `null`

Stores the animations for the material

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[animations](ShaderMaterial.md#animations)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:415

___

### checkReadyOnEveryCall

• **checkReadyOnEveryCall**: `boolean` = `false`

Specifies if the ready state should be checked on each call

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[checkReadyOnEveryCall](ShaderMaterial.md#checkreadyoneverycall)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:265

___

### checkReadyOnlyOnce

• **checkReadyOnlyOnce**: `boolean` = `false`

Specifies if the ready state should be checked once

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[checkReadyOnlyOnce](ShaderMaterial.md#checkreadyonlyonce)

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

[ShaderMaterial](ShaderMaterial.md).[customShaderNameResolve](ShaderMaterial.md#customshadernameresolve)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:207

___

### depthFunction

• **depthFunction**: `number` = `0`

Specifies the depth function that should be used. 0 means the default engine function

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[depthFunction](ShaderMaterial.md#depthfunction)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:584

___

### disableColorWrite

• **disableColorWrite**: `boolean` = `false`

Specifies if color writing should be disabled

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[disableColorWrite](ShaderMaterial.md#disablecolorwrite)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:572

___

### disableDepthWrite

• **disableDepthWrite**: `boolean` = `false`

Specifies if depth writing should be disabled

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[disableDepthWrite](ShaderMaterial.md#disabledepthwrite)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:566

___

### doNotSerialize

• **doNotSerialize**: `boolean` = `false`

Specifies if the material should be serialized

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[doNotSerialize](ShaderMaterial.md#donotserialize)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:405

___

### forceDepthWrite

• **forceDepthWrite**: `boolean` = `false`

Specifies if depth writing should be forced

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[forceDepthWrite](ShaderMaterial.md#forcedepthwrite)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:578

___

### getRenderTargetTextures

• **getRenderTargetTextures**: [`Nullable`](../modules.md#nullable)() => [`SmartArray`](SmartArray.md)[`RenderTargetTexture`](RenderTargetTexture.md) = `null`

Callback triggered to get the render target textures

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[getRenderTargetTextures](ShaderMaterial.md#getrendertargettextures)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:391

___

### id

• **id**: `string`

The ID of the material

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[id](ShaderMaterial.md#id)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:233

___

### inspectableCustomProperties

• **inspectableCustomProperties**: [`IInspectable`](../interfaces/IInspectable.md)[]

List of inspectable custom properties (used by the Inspector)

**`See`**

https://doc.babylonjs.com/how_to/debug_layer#extensibility

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[inspectableCustomProperties](ShaderMaterial.md#inspectablecustomproperties)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:298

___

### metadata

• **metadata**: `any` = `null`

Gets or sets user defined metadata

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[metadata](ShaderMaterial.md#metadata)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:254

___

### name

• **name**: `string`

The name of the material

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[name](ShaderMaterial.md#name)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:248

___

### onCompiled

• **onCompiled**: [`Nullable`](../modules.md#nullable)(`effect`: [`Effect`](Effect.md)) => `void` = `null`

Callback triggered when the material is compiled

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[onCompiled](ShaderMaterial.md#oncompiled)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:381

___

### onDisposeObservable

• **onDisposeObservable**: [`Observable`](Observable.md)[`Material`](Material.md)

An event triggered when the material is disposed

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[onDisposeObservable](ShaderMaterial.md#ondisposeobservable)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:420

___

### onError

• **onError**: [`Nullable`](../modules.md#nullable)(`effect`: [`Effect`](Effect.md), `errors`: `string`) => `void` = `null`

Callback triggered when an error occurs

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[onError](ShaderMaterial.md#onerror)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:386

___

### pluginManager

• `Optional` **pluginManager**: [`MaterialPluginManager`](MaterialPluginManager.md)

Plugin manager for this material

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[pluginManager](ShaderMaterial.md#pluginmanager)

#### Defined in

https://github.com/babylon.js/core/src/Materials/materialPluginManager.ts:30

___

### pointSize

• **pointSize**: `number` = `1.0`

Stores the size of points

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[pointSize](ShaderMaterial.md#pointsize)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:620

___

### reservedDataStore

• **reservedDataStore**: `any` = `null`

For internal use only. Please do not use.

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[reservedDataStore](ShaderMaterial.md#reserveddatastore)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:259

___

### separateCullingPass

• **separateCullingPass**: `boolean` = `false`

Specifies if there should be a separate pass for culling

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[separateCullingPass](ShaderMaterial.md#separatecullingpass)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:590

___

### shadowDepthWrapper

• **shadowDepthWrapper**: [`Nullable`](../modules.md#nullable)[`ShadowDepthWrapper`](ShadowDepthWrapper.md) = `null`

Custom shadow depth material to use for shadow rendering instead of the in-built one

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[shadowDepthWrapper](ShaderMaterial.md#shadowdepthwrapper)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:220

___

### sideOrientation

• **sideOrientation**: `number`

Stores the value for side orientation

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[sideOrientation](ShaderMaterial.md#sideorientation)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:376

___

### snippetId

• **snippetId**: `string`

Snippet ID if the material was created from the snippet server

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[snippetId](ShaderMaterial.md#snippetid)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:137

___

### state

• **state**: `string` = `""`

The state of the material

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[state](ShaderMaterial.md#state)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:277

___

### stencil

• `Readonly` **stencil**: `MaterialStencilState`

Gives access to the stencil properties of the material

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[stencil](ShaderMaterial.md#stencil)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:697

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the material

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[uniqueId](ShaderMaterial.md#uniqueid)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:239

___

### zOffset

• **zOffset**: `number` = `0`

Stores the z offset Factor value

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[zOffset](ShaderMaterial.md#zoffset)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:626

___

### zOffsetUnits

• **zOffsetUnits**: `number` = `0`

Stores the z offset Units value

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[zOffsetUnits](ShaderMaterial.md#zoffsetunits)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:632

___

### AllDirtyFlag

▪ `Static` `Readonly` **AllDirtyFlag**: ``63``

The all dirty flag value

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[AllDirtyFlag](ShaderMaterial.md#alldirtyflag)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:164

___

### AttributesDirtyFlag

▪ `Static` `Readonly` **AttributesDirtyFlag**: ``8``

The dirty attribute flag value

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[AttributesDirtyFlag](ShaderMaterial.md#attributesdirtyflag)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:149

___

### ClockWiseSideOrientation

▪ `Static` `Readonly` **ClockWiseSideOrientation**: ``0``

Stores the clock-wise side orientation

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[ClockWiseSideOrientation](ShaderMaterial.md#clockwisesideorientation)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:124

___

### CounterClockWiseSideOrientation

▪ `Static` `Readonly` **CounterClockWiseSideOrientation**: ``1``

Stores the counter clock-wise side orientation

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[CounterClockWiseSideOrientation](ShaderMaterial.md#counterclockwisesideorientation)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:129

___

### CreateFromSnippetAsync

▪ `Static` **CreateFromSnippetAsync**: (`snippetId`: `string`, `scene`: [`Scene`](Scene.md), `rootUrl`: `string`) => `Promise`[`ShaderMaterial`](ShaderMaterial.md) = `ShaderMaterial.ParseFromSnippetAsync`

#### Type declaration

▸ (`snippetId`, `scene`, `rootUrl?`): `Promise`[`ShaderMaterial`](ShaderMaterial.md)

Creates a ShaderMaterial from a snippet saved by the Inspector

##### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `snippetId` | `string` | `undefined` | defines the snippet to load |
| `scene` | [`Scene`](Scene.md) | `undefined` | defines the hosting scene |
| `rootUrl` | `string` | `""` | defines the root URL to use to load textures and relative dependencies |

##### Returns

`Promise`[`ShaderMaterial`](ShaderMaterial.md)

a promise that will resolve to the new ShaderMaterial

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[CreateFromSnippetAsync](ShaderMaterial.md#createfromsnippetasync)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:1765

___

### FresnelDirtyFlag

▪ `Static` `Readonly` **FresnelDirtyFlag**: ``4``

The dirty fresnel flag value

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[FresnelDirtyFlag](ShaderMaterial.md#fresneldirtyflag)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:144

___

### LightDirtyFlag

▪ `Static` `Readonly` **LightDirtyFlag**: ``2``

The dirty light flag value

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[LightDirtyFlag](ShaderMaterial.md#lightdirtyflag)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:139

___

### LineListDrawMode

▪ `Static` `Readonly` **LineListDrawMode**: ``4``

Returns the line list draw mode

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[LineListDrawMode](ShaderMaterial.md#linelistdrawmode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:103

___

### LineLoopDrawMode

▪ `Static` `Readonly` **LineLoopDrawMode**: ``5``

Returns the line loop draw mode

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[LineLoopDrawMode](ShaderMaterial.md#lineloopdrawmode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:107

___

### LineStripDrawMode

▪ `Static` `Readonly` **LineStripDrawMode**: ``6``

Returns the line strip draw mode

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[LineStripDrawMode](ShaderMaterial.md#linestripdrawmode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:111

___

### MATERIAL\_ALPHABLEND

▪ `Static` `Readonly` **MATERIAL\_ALPHABLEND**: ``2``

MaterialTransparencyMode: Pixels are blended (according to the alpha mode) with the already drawn pixels in the current frame buffer.

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[MATERIAL_ALPHABLEND](ShaderMaterial.md#material_alphablend)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:179

___

### MATERIAL\_ALPHATEST

▪ `Static` `Readonly` **MATERIAL\_ALPHATEST**: ``1``

MaterialTransparencyMode: Alpha Test mode, pixel are discarded below a certain threshold defined by the alpha cutoff value.

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[MATERIAL_ALPHATEST](ShaderMaterial.md#material_alphatest)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:174

___

### MATERIAL\_ALPHATESTANDBLEND

▪ `Static` `Readonly` **MATERIAL\_ALPHATESTANDBLEND**: ``3``

MaterialTransparencyMode: Pixels are blended (according to the alpha mode) with the already drawn pixels in the current frame buffer.
They are also discarded below the alpha cutoff threshold to improve performances.

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[MATERIAL_ALPHATESTANDBLEND](ShaderMaterial.md#material_alphatestandblend)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:185

___

### MATERIAL\_NORMALBLENDMETHOD\_RNM

▪ `Static` `Readonly` **MATERIAL\_NORMALBLENDMETHOD\_RNM**: ``1``

The Reoriented Normal Mapping method is used to blend normals.
Details of the algorithm can be found here: https://blog.selfshadow.com/publications/blending-in-detail/

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[MATERIAL_NORMALBLENDMETHOD_RNM](ShaderMaterial.md#material_normalblendmethod_rnm)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:197

___

### MATERIAL\_NORMALBLENDMETHOD\_WHITEOUT

▪ `Static` `Readonly` **MATERIAL\_NORMALBLENDMETHOD\_WHITEOUT**: ``0``

The Whiteout method is used to blend normals.
Details of the algorithm can be found here: https://blog.selfshadow.com/publications/blending-in-detail/

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[MATERIAL_NORMALBLENDMETHOD_WHITEOUT](ShaderMaterial.md#material_normalblendmethod_whiteout)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:191

___

### MATERIAL\_OPAQUE

▪ `Static` `Readonly` **MATERIAL\_OPAQUE**: ``0``

MaterialTransparencyMode: No transparency mode, Alpha channel is not use.

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[MATERIAL_OPAQUE](ShaderMaterial.md#material_opaque)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:169

___

### MiscDirtyFlag

▪ `Static` `Readonly` **MiscDirtyFlag**: ``16``

The dirty misc flag value

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[MiscDirtyFlag](ShaderMaterial.md#miscdirtyflag)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:154

___

### OnEventObservable

▪ `Static` **OnEventObservable**: [`Observable`](Observable.md)[`Material`](Material.md)

Event observable which raises global events common to all materials (like MaterialPluginEvent.Created)

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[OnEventObservable](ShaderMaterial.md#oneventobservable)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:202

___

### PointFillMode

▪ `Static` `Readonly` **PointFillMode**: ``2``

Returns the point fill mode

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[PointFillMode](ShaderMaterial.md#pointfillmode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:95

___

### PointListDrawMode

▪ `Static` `Readonly` **PointListDrawMode**: ``3``

Returns the point list draw mode

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[PointListDrawMode](ShaderMaterial.md#pointlistdrawmode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:99

___

### PrePassDirtyFlag

▪ `Static` `Readonly` **PrePassDirtyFlag**: ``32``

The dirty prepass flag value

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[PrePassDirtyFlag](ShaderMaterial.md#prepassdirtyflag)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:159

___

### SnippetUrl

▪ `Static` **SnippetUrl**: `string` = `Constants.SnippetUrl`

Define the Url to load snippets

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[SnippetUrl](ShaderMaterial.md#snippeturl)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:134

___

### TextureDirtyFlag

▪ `Static` `Readonly` **TextureDirtyFlag**: ``1``

The dirty texture flag value

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[TextureDirtyFlag](ShaderMaterial.md#texturedirtyflag)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:134

___

### TriangleFanDrawMode

▪ `Static` `Readonly` **TriangleFanDrawMode**: ``8``

Returns the triangle fan draw mode

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[TriangleFanDrawMode](ShaderMaterial.md#trianglefandrawmode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:119

___

### TriangleFillMode

▪ `Static` `Readonly` **TriangleFillMode**: ``0``

Returns the triangle fill mode

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[TriangleFillMode](ShaderMaterial.md#trianglefillmode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:87

___

### TriangleStripDrawMode

▪ `Static` `Readonly` **TriangleStripDrawMode**: ``7``

Returns the triangle strip draw mode

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[TriangleStripDrawMode](ShaderMaterial.md#trianglestripdrawmode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:115

___

### WireFrameFillMode

▪ `Static` `Readonly` **WireFrameFillMode**: ``1``

Returns the wireframe mode

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[WireFrameFillMode](ShaderMaterial.md#wireframefillmode)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:91

## Accessors

### \_disableAlphaBlending

• `Protected` `get` **_disableAlphaBlending**(): `boolean`

Returns true if alpha blending should be disabled.

#### Returns

`boolean`

#### Inherited from

ShaderMaterial.\_disableAlphaBlending

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:995

___

### alpha

• `get` **alpha**(): `number`

Gets the alpha value of the material

#### Returns

`number`

#### Inherited from

ShaderMaterial.alpha

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

ShaderMaterial.alpha

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:303

___

### alphaMode

• `get` **alphaMode**(): `number`

Gets the value of the alpha mode

#### Returns

`number`

#### Inherited from

ShaderMaterial.alphaMode

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

ShaderMaterial.alphaMode

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:514

___

### backFaceCulling

• `get` **backFaceCulling**(): `boolean`

Gets the culling state

#### Returns

`boolean`

#### Inherited from

ShaderMaterial.backFaceCulling

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

ShaderMaterial.backFaceCulling

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:333

___

### canRenderToMRT

• `get` **canRenderToMRT**(): `boolean`

If the material can be rendered to several textures with MRT extension

#### Returns

`boolean`

#### Inherited from

ShaderMaterial.canRenderToMRT

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:282

___

### cullBackFaces

• `get` **cullBackFaces**(): `boolean`

Gets the type of faces that should be culled

#### Returns

`boolean`

#### Inherited from

ShaderMaterial.cullBackFaces

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

ShaderMaterial.cullBackFaces

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:357

___

### fillMode

• `get` **fillMode**(): `number`

Gets the material fill mode

#### Returns

`number`

#### Inherited from

ShaderMaterial.fillMode

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

ShaderMaterial.fillMode

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:685

___

### fogEnabled

• `get` **fogEnabled**(): `boolean`

Gets the value of the fog enabled state

#### Returns

`boolean`

#### Inherited from

ShaderMaterial.fogEnabled

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

ShaderMaterial.fogEnabled

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:601

___

### hasRenderTargetTextures

• `get` **hasRenderTargetTextures**(): `boolean`

Gets a boolean indicating that current material needs to register RTT

#### Returns

`boolean`

#### Inherited from

ShaderMaterial.hasRenderTargetTextures

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:396

___

### isFrozen

• `get` **isFrozen**(): `boolean`

Specifies if updates for the material been locked

#### Returns

`boolean`

#### Inherited from

ShaderMaterial.isFrozen

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:883

___

### isPrePassCapable

• `get` **isPrePassCapable**(): `boolean`

Can this material render to prepass

#### Returns

`boolean`

#### Inherited from

ShaderMaterial.isPrePassCapable

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:558

___

### needDepthPrePass

• `get` **needDepthPrePass**(): `boolean`

Gets the depth pre-pass value

#### Returns

`boolean`

#### Inherited from

ShaderMaterial.needDepthPrePass

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

ShaderMaterial.needDepthPrePass

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

ShaderMaterial.onBind

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:459

___

### onBindObservable

• `get` **onBindObservable**(): [`Observable`](Observable.md)[`AbstractMesh`](AbstractMesh.md)

An event triggered when the material is bound

#### Returns

[`Observable`](Observable.md)[`AbstractMesh`](AbstractMesh.md)

#### Inherited from

ShaderMaterial.onBindObservable

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

ShaderMaterial.onDispose

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:431

___

### onEffectCreatedObservable

• `get` **onEffectCreatedObservable**(): [`Observable`](Observable.md){ `effect`: [`Effect`](Effect.md) ; `subMesh`: [`Nullable`](../modules.md#nullable)[`SubMesh`](SubMesh.md)  }

An event triggered when the effect is (re)created

#### Returns

[`Observable`](Observable.md){ `effect`: [`Effect`](Effect.md) ; `subMesh`: [`Nullable`](../modules.md#nullable)[`SubMesh`](SubMesh.md)  }

#### Inherited from

ShaderMaterial.onEffectCreatedObservable

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:482

___

### onUnBindObservable

• `get` **onUnBindObservable**(): [`Observable`](Observable.md)[`Material`](Material.md)

An event triggered when the material is unbound

#### Returns

[`Observable`](Observable.md)[`Material`](Material.md)

#### Inherited from

ShaderMaterial.onUnBindObservable

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:469

___

### options

• `get` **options**(): [`IShaderMaterialOptions`](../interfaces/IShaderMaterialOptions.md)

Gets the options used to compile the shader.
They can be modified to trigger a new compilation

#### Returns

[`IShaderMaterialOptions`](../interfaces/IShaderMaterialOptions.md)

#### Inherited from

ShaderMaterial.options

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:194

___

### pointsCloud

• `get` **pointsCloud**(): `boolean`

Gets the value specifying if point clouds are enabled

#### Returns

`boolean`

#### Inherited from

ShaderMaterial.pointsCloud

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

ShaderMaterial.pointsCloud

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:670

___

### shaderPath

• `get` **shaderPath**(): `any`

Gets the shader path used to define the shader code
It can be modified to trigger a new compilation

#### Returns

`any`

#### Inherited from

ShaderMaterial.shaderPath

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:178

• `set` **shaderPath**(`shaderPath`): `void`

Sets the shader path used to define the shader code
It can be modified to trigger a new compilation

#### Parameters

| Name | Type |
| :------ | :------ |
| `shaderPath` | `any` |

#### Returns

`void`

#### Inherited from

ShaderMaterial.shaderPath

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:186

___

### transparencyMode

• `get` **transparencyMode**(): [`Nullable`](../modules.md#nullable)`number`

Gets the current transparency mode.

#### Returns

[`Nullable`](../modules.md#nullable)`number`

#### Inherited from

ShaderMaterial.transparencyMode

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

ShaderMaterial.transparencyMode

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:980

___

### wireframe

• `get` **wireframe**(): `boolean`

#### Returns

`boolean`

#### Inherited from

ShaderMaterial.wireframe

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

ShaderMaterial.wireframe

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

[ShaderMaterial](ShaderMaterial.md).[_afterBind](ShaderMaterial.md#_afterbind)

#### Defined in

https://github.com/babylon.js/core/src/Materials/pushMaterial.ts:80

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

[ShaderMaterial](ShaderMaterial.md).[_isReadyForSubMesh](ShaderMaterial.md#_isreadyforsubmesh)

#### Defined in

https://github.com/babylon.js/core/src/Materials/pushMaterial.ts:43

___

### \_markAllSubMeshesAsAllDirty

▸ `Protected` **_markAllSubMeshesAsAllDirty**(): `void`

Indicates that we need to re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[_markAllSubMeshesAsAllDirty](ShaderMaterial.md#_markallsubmeshesasalldirty)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1543

___

### \_markAllSubMeshesAsAttributesDirty

▸ `Protected` **_markAllSubMeshesAsAttributesDirty**(): `void`

Indicates that attributes need to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[_markAllSubMeshesAsAttributesDirty](ShaderMaterial.md#_markallsubmeshesasattributesdirty)

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

[ShaderMaterial](ShaderMaterial.md).[_markAllSubMeshesAsDirty](ShaderMaterial.md#_markallsubmeshesasdirty)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1498

___

### \_markAllSubMeshesAsFresnelAndMiscDirty

▸ `Protected` **_markAllSubMeshesAsFresnelAndMiscDirty**(): `void`

Indicates that fresnel and misc need to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[_markAllSubMeshesAsFresnelAndMiscDirty](ShaderMaterial.md#_markallsubmeshesasfresnelandmiscdirty)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1571

___

### \_markAllSubMeshesAsFresnelDirty

▸ `Protected` **_markAllSubMeshesAsFresnelDirty**(): `void`

Indicates that fresnel needs to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[_markAllSubMeshesAsFresnelDirty](ShaderMaterial.md#_markallsubmeshesasfresneldirty)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1564

___

### \_markAllSubMeshesAsImageProcessingDirty

▸ `Protected` **_markAllSubMeshesAsImageProcessingDirty**(): `void`

Indicates that image processing needs to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[_markAllSubMeshesAsImageProcessingDirty](ShaderMaterial.md#_markallsubmeshesasimageprocessingdirty)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1550

___

### \_markAllSubMeshesAsLightsDirty

▸ `Protected` **_markAllSubMeshesAsLightsDirty**(): `void`

Indicates that lights need to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[_markAllSubMeshesAsLightsDirty](ShaderMaterial.md#_markallsubmeshesaslightsdirty)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1578

___

### \_markAllSubMeshesAsMiscDirty

▸ `Protected` **_markAllSubMeshesAsMiscDirty**(): `void`

Indicates that misc needs to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[_markAllSubMeshesAsMiscDirty](ShaderMaterial.md#_markallsubmeshesasmiscdirty)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1592

___

### \_markAllSubMeshesAsPrePassDirty

▸ `Protected` **_markAllSubMeshesAsPrePassDirty**(): `void`

Indicates that prepass needs to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[_markAllSubMeshesAsPrePassDirty](ShaderMaterial.md#_markallsubmeshesasprepassdirty)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1599

___

### \_markAllSubMeshesAsTexturesAndMiscDirty

▸ `Protected` **_markAllSubMeshesAsTexturesAndMiscDirty**(): `void`

Indicates that textures and misc need to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[_markAllSubMeshesAsTexturesAndMiscDirty](ShaderMaterial.md#_markallsubmeshesastexturesandmiscdirty)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1606

___

### \_markAllSubMeshesAsTexturesDirty

▸ `Protected` **_markAllSubMeshesAsTexturesDirty**(): `void`

Indicates that textures need to be re-calculated for all submeshes

#### Returns

`void`

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[_markAllSubMeshesAsTexturesDirty](ShaderMaterial.md#_markallsubmeshesastexturesdirty)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1557

___

### \_markScenePrePassDirty

▸ `Protected` **_markScenePrePassDirty**(): `void`

Indicates that the scene should check if the rendering now needs a prepass

#### Returns

`void`

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[_markScenePrePassDirty](ShaderMaterial.md#_marksceneprepassdirty)

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

[ShaderMaterial](ShaderMaterial.md).[_mustRebind](ShaderMaterial.md#_mustrebind)

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

[ShaderMaterial](ShaderMaterial.md).[_shouldTurnAlphaTestOn](ShaderMaterial.md#_shouldturnalphateston)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1040

___

### bind

▸ **bind**(`world`, `mesh?`, `effectOverride?`, `subMesh?`): `void`

Binds the material to the mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `world` | [`Matrix`](Matrix.md) | defines the world transformation matrix |
| `mesh?` | [`Mesh`](Mesh.md) | defines the mesh to bind the material to |
| `effectOverride?` | [`Nullable`](../modules.md#nullable)[`Effect`](Effect.md) | If provided, use this effect instead of internal effect |
| `subMesh?` | [`SubMesh`](SubMesh.md) | defines the submesh to bind the material to |

#### Returns

`void`

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[bind](ShaderMaterial.md#bind)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:942

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

[ShaderMaterial](ShaderMaterial.md).[bindEyePosition](ShaderMaterial.md#bindeyeposition)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1168

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

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[bindForSubMesh](ShaderMaterial.md#bindforsubmesh)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:931

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

[ShaderMaterial](ShaderMaterial.md).[bindOnlyNormalMatrix](ShaderMaterial.md#bindonlynormalmatrix)

#### Defined in

https://github.com/babylon.js/core/src/Materials/pushMaterial.ts:68

___

### bindOnlyWorldMatrix

▸ **bindOnlyWorldMatrix**(`world`, `effectOverride?`): `void`

Binds the world matrix to the material

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `world` | [`Matrix`](Matrix.md) | defines the world transformation matrix |
| `effectOverride?` | [`Nullable`](../modules.md#nullable)[`Effect`](Effect.md) | If provided, use this effect instead of internal effect |

#### Returns

`void`

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[bindOnlyWorldMatrix](ShaderMaterial.md#bindonlyworldmatrix)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:901

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

[ShaderMaterial](ShaderMaterial.md).[bindView](ShaderMaterial.md#bindview)

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

[ShaderMaterial](ShaderMaterial.md).[bindViewProjection](ShaderMaterial.md#bindviewprojection)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1154

___

### buildUniformLayout

▸ **buildUniformLayout**(): `void`

Initializes the uniform buffer layout for the shader.

#### Returns

`void`

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[buildUniformLayout](ShaderMaterial.md#builduniformlayout)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1104

___

### clone

▸ **clone**(`name`): [`ShaderMaterial`](ShaderMaterial.md)

Makes a duplicate of the material, and gives it a new name

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the new name for the duplicated material |

#### Returns

[`ShaderMaterial`](ShaderMaterial.md)

the cloned material

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[clone](ShaderMaterial.md#clone)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:1208

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

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[dispose](ShaderMaterial.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:1366

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

[ShaderMaterial](ShaderMaterial.md).[forceCompilation](ShaderMaterial.md#forcecompilation)

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

[ShaderMaterial](ShaderMaterial.md).[forceCompilationAsync](ShaderMaterial.md#forcecompilationasync)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1392

___

### freeze

▸ **freeze**(): `void`

Locks updates for the material

#### Returns

`void`

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[freeze](ShaderMaterial.md#freeze)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:890

___

### getActiveTextures

▸ **getActiveTextures**(): [`BaseTexture`](BaseTexture.md)[]

Gets the active textures from the material

#### Returns

[`BaseTexture`](BaseTexture.md)[]

an array of textures

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[getActiveTextures](ShaderMaterial.md#getactivetextures)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:1158

___

### getAlphaTestTexture

▸ **getAlphaTestTexture**(): [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Gets the texture used for the alpha test

#### Returns

[`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

the texture to use for alpha testing

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[getAlphaTestTexture](ShaderMaterial.md#getalphatesttexture)

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

[ShaderMaterial](ShaderMaterial.md).[getAnimatables](ShaderMaterial.md#getanimatables)

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

[ShaderMaterial](ShaderMaterial.md).[getBindedMeshes](ShaderMaterial.md#getbindedmeshes)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1289

___

### getClassName

▸ **getClassName**(): `string`

Gets the current class name of the material e.g. "ShaderMaterial"
Mainly use in serialization.

#### Returns

`string`

the class name

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[getClassName](ShaderMaterial.md#getclassname)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:203

___

### getEffect

▸ **getEffect**(): [`Effect`](Effect.md)

#### Returns

[`Effect`](Effect.md)

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[getEffect](ShaderMaterial.md#geteffect)

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

[ShaderMaterial](ShaderMaterial.md).[getScene](ShaderMaterial.md#getscene)

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

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[hasTexture](ShaderMaterial.md#hastexture)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:1180

___

### isReady

▸ **isReady**(`mesh?`, `useInstances?`, `subMesh?`): `boolean`

Checks if the material is ready to render the requested mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh?` | [`AbstractMesh`](AbstractMesh.md) | Define the mesh to render |
| `useInstances?` | `boolean` | Define whether or not the material is used with instances |
| `subMesh?` | [`SubMesh`](SubMesh.md) | defines which submesh to render |

#### Returns

`boolean`

true if ready, otherwise false

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[isReady](ShaderMaterial.md#isready)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:602

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

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[isReadyForSubMesh](ShaderMaterial.md#isreadyforsubmesh)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:591

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

[ShaderMaterial](ShaderMaterial.md).[markAsDirty](ShaderMaterial.md#markasdirty)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1437

___

### markDirty

▸ **markDirty**(): `void`

Marks the material to indicate that it needs to be re-calculated

#### Returns

`void`

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[markDirty](ShaderMaterial.md#markdirty)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1055

___

### needAlphaBlending

▸ **needAlphaBlending**(): `boolean`

Specifies if the material will require alpha blending

#### Returns

`boolean`

a boolean specifying if alpha blending is needed

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[needAlphaBlending](ShaderMaterial.md#needalphablending)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:211

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

[ShaderMaterial](ShaderMaterial.md).[needAlphaBlendingForMesh](ShaderMaterial.md#needalphablendingformesh)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1016

___

### needAlphaTesting

▸ **needAlphaTesting**(): `boolean`

Specifies if this material should be rendered in alpha test mode

#### Returns

`boolean`

a boolean specifying if an alpha test is needed.

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[needAlphaTesting](ShaderMaterial.md#needalphatesting)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:219

___

### resetDrawCache

▸ **resetDrawCache**(): `void`

Resets the draw wrappers cache for all submeshes that are using this material

#### Returns

`void`

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[resetDrawCache](ShaderMaterial.md#resetdrawcache)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1478

___

### serialize

▸ **serialize**(): `any`

Serializes this material in a JSON representation

#### Returns

`any`

the serialized material object

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[serialize](ShaderMaterial.md#serialize)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:1390

___

### setArray2

▸ **setArray2**(`name`, `value`): [`ShaderMaterial`](ShaderMaterial.md)

Set a vec2 array in the shader from a number array.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Define the name of the uniform as defined in the shader |
| `value` | `number`[] | Define the value to give to the uniform |

#### Returns

[`ShaderMaterial`](ShaderMaterial.md)

the material itself allowing "fluent" like uniform updates

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[setArray2](ShaderMaterial.md#setarray2)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:506

___

### setArray3

▸ **setArray3**(`name`, `value`): [`ShaderMaterial`](ShaderMaterial.md)

Set a vec3 array in the shader from a number array.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Define the name of the uniform as defined in the shader |
| `value` | `number`[] | Define the value to give to the uniform |

#### Returns

[`ShaderMaterial`](ShaderMaterial.md)

the material itself allowing "fluent" like uniform updates

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[setArray3](ShaderMaterial.md#setarray3)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:519

___

### setArray4

▸ **setArray4**(`name`, `value`): [`ShaderMaterial`](ShaderMaterial.md)

Set a vec4 array in the shader from a number array.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Define the name of the uniform as defined in the shader |
| `value` | `number`[] | Define the value to give to the uniform |

#### Returns

[`ShaderMaterial`](ShaderMaterial.md)

the material itself allowing "fluent" like uniform updates

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[setArray4](ShaderMaterial.md#setarray4)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:532

___

### setColor3

▸ **setColor3**(`name`, `value`): [`ShaderMaterial`](ShaderMaterial.md)

Set a vec3 in the shader from a Color3.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Define the name of the uniform as defined in the shader |
| `value` | [`Color3`](Color3.md) | Define the value to give to the uniform |

#### Returns

[`ShaderMaterial`](ShaderMaterial.md)

the material itself allowing "fluent" like uniform updates

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[setColor3](ShaderMaterial.md#setcolor3)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:322

___

### setColor3Array

▸ **setColor3Array**(`name`, `value`): [`ShaderMaterial`](ShaderMaterial.md)

Set a vec3 array in the shader from a Color3 array.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Define the name of the uniform as defined in the shader |
| `value` | [`Color3`](Color3.md)[] | Define the value to give to the uniform |

#### Returns

[`ShaderMaterial`](ShaderMaterial.md)

the material itself allowing "fluent" like uniform updates

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[setColor3Array](ShaderMaterial.md#setcolor3array)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:335

___

### setColor4

▸ **setColor4**(`name`, `value`): [`ShaderMaterial`](ShaderMaterial.md)

Set a vec4 in the shader from a Color4.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Define the name of the uniform as defined in the shader |
| `value` | [`Color4`](Color4.md) | Define the value to give to the uniform |

#### Returns

[`ShaderMaterial`](ShaderMaterial.md)

the material itself allowing "fluent" like uniform updates

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[setColor4](ShaderMaterial.md#setcolor4)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:350

___

### setColor4Array

▸ **setColor4Array**(`name`, `value`): [`ShaderMaterial`](ShaderMaterial.md)

Set a vec4 array in the shader from a Color4 array.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Define the name of the uniform as defined in the shader |
| `value` | [`Color4`](Color4.md)[] | Define the value to give to the uniform |

#### Returns

[`ShaderMaterial`](ShaderMaterial.md)

the material itself allowing "fluent" like uniform updates

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[setColor4Array](ShaderMaterial.md#setcolor4array)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:363

___

### setExternalTexture

▸ **setExternalTexture**(`name`, `texture`): [`ShaderMaterial`](ShaderMaterial.md)

Set an internal texture in the shader.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Define the name of the uniform samplers as defined in the shader |
| `texture` | [`ExternalTexture`](ExternalTexture.md) | Define the texture to bind to this sampler |

#### Returns

[`ShaderMaterial`](ShaderMaterial.md)

the material itself allowing "fluent" like uniform updates

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[setExternalTexture](ShaderMaterial.md#setexternaltexture)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:268

___

### setFloat

▸ **setFloat**(`name`, `value`): [`ShaderMaterial`](ShaderMaterial.md)

Set a float in the shader.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Define the name of the uniform as defined in the shader |
| `value` | `number` | Define the value to give to the uniform |

#### Returns

[`ShaderMaterial`](ShaderMaterial.md)

the material itself allowing "fluent" like uniform updates

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[setFloat](ShaderMaterial.md#setfloat)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:283

___

### setFloats

▸ **setFloats**(`name`, `value`): [`ShaderMaterial`](ShaderMaterial.md)

Set an array of floats in the shader.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Define the name of the uniform as defined in the shader |
| `value` | `number`[] | Define the value to give to the uniform |

#### Returns

[`ShaderMaterial`](ShaderMaterial.md)

the material itself allowing "fluent" like uniform updates

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[setFloats](ShaderMaterial.md#setfloats)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:309

___

### setInt

▸ **setInt**(`name`, `value`): [`ShaderMaterial`](ShaderMaterial.md)

Set a int in the shader.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Define the name of the uniform as defined in the shader |
| `value` | `number` | Define the value to give to the uniform |

#### Returns

[`ShaderMaterial`](ShaderMaterial.md)

the material itself allowing "fluent" like uniform updates

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[setInt](ShaderMaterial.md#setint)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:296

___

### setMatrices

▸ **setMatrices**(`name`, `value`): [`ShaderMaterial`](ShaderMaterial.md)

Set a float32Array in the shader from a matrix array.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Define the name of the uniform as defined in the shader |
| `value` | [`Matrix`](Matrix.md)[] | Define the value to give to the uniform |

#### Returns

[`ShaderMaterial`](ShaderMaterial.md)

the material itself allowing "fluent" like uniform updates

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[setMatrices](ShaderMaterial.md#setmatrices)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:458

___

### setMatrix

▸ **setMatrix**(`name`, `value`): [`ShaderMaterial`](ShaderMaterial.md)

Set a mat4 in the shader from a Matrix.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Define the name of the uniform as defined in the shader |
| `value` | [`Matrix`](Matrix.md) | Define the value to give to the uniform |

#### Returns

[`ShaderMaterial`](ShaderMaterial.md)

the material itself allowing "fluent" like uniform updates

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[setMatrix](ShaderMaterial.md#setmatrix)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:445

___

### setMatrix2x2

▸ **setMatrix2x2**(`name`, `value`): [`ShaderMaterial`](ShaderMaterial.md)

Set a mat2 in the shader from a Float32Array.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Define the name of the uniform as defined in the shader |
| `value` | `number`[] \| `Float32Array` | Define the value to give to the uniform |

#### Returns

[`ShaderMaterial`](ShaderMaterial.md)

the material itself allowing "fluent" like uniform updates

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[setMatrix2x2](ShaderMaterial.md#setmatrix2x2)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:493

___

### setMatrix3x3

▸ **setMatrix3x3**(`name`, `value`): [`ShaderMaterial`](ShaderMaterial.md)

Set a mat3 in the shader from a Float32Array.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Define the name of the uniform as defined in the shader |
| `value` | `number`[] \| `Float32Array` | Define the value to give to the uniform |

#### Returns

[`ShaderMaterial`](ShaderMaterial.md)

the material itself allowing "fluent" like uniform updates

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[setMatrix3x3](ShaderMaterial.md#setmatrix3x3)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:480

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

[ShaderMaterial](ShaderMaterial.md).[setPrePassRenderer](ShaderMaterial.md#setprepassrenderer)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1616

___

### setQuaternion

▸ **setQuaternion**(`name`, `value`): [`ShaderMaterial`](ShaderMaterial.md)

Set a vec4 in the shader from a Quaternion.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Define the name of the uniform as defined in the shader |
| `value` | [`Quaternion`](Quaternion.md) | Define the value to give to the uniform |

#### Returns

[`ShaderMaterial`](ShaderMaterial.md)

the material itself allowing "fluent" like uniform updates

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[setQuaternion](ShaderMaterial.md#setquaternion)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:417

___

### setQuaternionArray

▸ **setQuaternionArray**(`name`, `value`): [`ShaderMaterial`](ShaderMaterial.md)

Set a vec4 array in the shader from a Quaternion array.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Define the name of the uniform as defined in the shader |
| `value` | [`Quaternion`](Quaternion.md)[] | Define the value to give to the uniform |

#### Returns

[`ShaderMaterial`](ShaderMaterial.md)

the material itself allowing "fluent" like uniform updates

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[setQuaternionArray](ShaderMaterial.md#setquaternionarray)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:430

___

### setStorageBuffer

▸ **setStorageBuffer**(`name`, `buffer`): [`ShaderMaterial`](ShaderMaterial.md)

Set a storage buffer in the shader

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Define the name of the storage buffer as defined in the shader |
| `buffer` | [`StorageBuffer`](StorageBuffer.md) | Define the value to give to the uniform |

#### Returns

[`ShaderMaterial`](ShaderMaterial.md)

the material itself allowing "fluent" like uniform updates

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[setStorageBuffer](ShaderMaterial.md#setstoragebuffer)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:575

___

### setTexture

▸ **setTexture**(`name`, `texture`): [`ShaderMaterial`](ShaderMaterial.md)

Set a texture in the shader.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Define the name of the uniform samplers as defined in the shader |
| `texture` | [`BaseTexture`](BaseTexture.md) | Define the texture to bind to this sampler |

#### Returns

[`ShaderMaterial`](ShaderMaterial.md)

the material itself allowing "fluent" like uniform updates

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[setTexture](ShaderMaterial.md#settexture)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:235

___

### setTextureArray

▸ **setTextureArray**(`name`, `textures`): [`ShaderMaterial`](ShaderMaterial.md)

Set a texture array in the shader.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Define the name of the uniform sampler array as defined in the shader |
| `textures` | [`BaseTexture`](BaseTexture.md)[] | Define the list of textures to bind to this sampler |

#### Returns

[`ShaderMaterial`](ShaderMaterial.md)

the material itself allowing "fluent" like uniform updates

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[setTextureArray](ShaderMaterial.md#settexturearray)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:250

___

### setTextureSampler

▸ **setTextureSampler**(`name`, `sampler`): [`ShaderMaterial`](ShaderMaterial.md)

Set a texture sampler in the shader

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Define the name of the uniform as defined in the shader |
| `sampler` | [`TextureSampler`](TextureSampler.md) | Define the value to give to the uniform |

#### Returns

[`ShaderMaterial`](ShaderMaterial.md)

the material itself allowing "fluent" like uniform updates

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[setTextureSampler](ShaderMaterial.md#settexturesampler)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:560

___

### setUniformBuffer

▸ **setUniformBuffer**(`name`, `buffer`): [`ShaderMaterial`](ShaderMaterial.md)

Set a uniform buffer in the shader

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Define the name of the uniform as defined in the shader |
| `buffer` | [`UniformBuffer`](UniformBuffer.md) | Define the value to give to the uniform |

#### Returns

[`ShaderMaterial`](ShaderMaterial.md)

the material itself allowing "fluent" like uniform updates

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[setUniformBuffer](ShaderMaterial.md#setuniformbuffer)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:545

___

### setVector2

▸ **setVector2**(`name`, `value`): [`ShaderMaterial`](ShaderMaterial.md)

Set a vec2 in the shader from a Vector2.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Define the name of the uniform as defined in the shader |
| `value` | [`Vector2`](Vector2.md) | Define the value to give to the uniform |

#### Returns

[`ShaderMaterial`](ShaderMaterial.md)

the material itself allowing "fluent" like uniform updates

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[setVector2](ShaderMaterial.md#setvector2)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:378

___

### setVector3

▸ **setVector3**(`name`, `value`): [`ShaderMaterial`](ShaderMaterial.md)

Set a vec3 in the shader from a Vector3.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Define the name of the uniform as defined in the shader |
| `value` | [`Vector3`](Vector3.md) | Define the value to give to the uniform |

#### Returns

[`ShaderMaterial`](ShaderMaterial.md)

the material itself allowing "fluent" like uniform updates

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[setVector3](ShaderMaterial.md#setvector3)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:391

___

### setVector4

▸ **setVector4**(`name`, `value`): [`ShaderMaterial`](ShaderMaterial.md)

Set a vec4 in the shader from a Vector4.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Define the name of the uniform as defined in the shader |
| `value` | [`Vector4`](Vector4.md) | Define the value to give to the uniform |

#### Returns

[`ShaderMaterial`](ShaderMaterial.md)

the material itself allowing "fluent" like uniform updates

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[setVector4](ShaderMaterial.md#setvector4)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:404

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

[ShaderMaterial](ShaderMaterial.md).[toString](ShaderMaterial.md#tostring)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:867

___

### unbind

▸ **unbind**(): `void`

Unbinds the material from the mesh

#### Returns

`void`

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[unbind](ShaderMaterial.md#unbind)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1222

___

### unfreeze

▸ **unfreeze**(): `void`

Unlocks updates for the material

#### Returns

`void`

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[unfreeze](ShaderMaterial.md#unfreeze)

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:898

___

### Parse

▸ `Static` **Parse**(`source`, `scene`, `rootUrl`): [`ShaderMaterial`](ShaderMaterial.md)

Creates a shader material from parsed shader material data

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | `any` | defines the JSON representation of the material |
| `scene` | [`Scene`](Scene.md) | defines the hosting scene |
| `rootUrl` | `string` | defines the root URL to use to load textures and relative dependencies |

#### Returns

[`ShaderMaterial`](ShaderMaterial.md)

a new material

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[Parse](ShaderMaterial.md#parse)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:1544

___

### ParseFromFileAsync

▸ `Static` **ParseFromFileAsync**(`name`, `url`, `scene`, `rootUrl?`): `Promise`[`ShaderMaterial`](ShaderMaterial.md)

Creates a new ShaderMaterial from a snippet saved in a remote file

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | [`Nullable`](../modules.md#nullable)`string` | `undefined` | defines the name of the ShaderMaterial to create (can be null or empty to use the one from the json data) |
| `url` | `string` | `undefined` | defines the url to load from |
| `scene` | [`Scene`](Scene.md) | `undefined` | defines the hosting scene |
| `rootUrl` | `string` | `""` | defines the root URL to use to load textures and relative dependencies |

#### Returns

`Promise`[`ShaderMaterial`](ShaderMaterial.md)

a promise that will resolve to the new ShaderMaterial

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[ParseFromFileAsync](ShaderMaterial.md#parsefromfileasync)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:1701

___

### ParseFromSnippetAsync

▸ `Static` **ParseFromSnippetAsync**(`snippetId`, `scene`, `rootUrl?`): `Promise`[`ShaderMaterial`](ShaderMaterial.md)

Creates a ShaderMaterial from a snippet saved by the Inspector

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `snippetId` | `string` | `undefined` | defines the snippet to load |
| `scene` | [`Scene`](Scene.md) | `undefined` | defines the hosting scene |
| `rootUrl` | `string` | `""` | defines the root URL to use to load textures and relative dependencies |

#### Returns

`Promise`[`ShaderMaterial`](ShaderMaterial.md)

a promise that will resolve to the new ShaderMaterial

#### Inherited from

[ShaderMaterial](ShaderMaterial.md).[ParseFromSnippetAsync](ShaderMaterial.md#parsefromsnippetasync)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:1733
