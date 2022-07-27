[@dev/core](../README.md) / [Exports](../modules.md) / NodeMaterial

# Class: NodeMaterial

Class used to create a node based material built by assembling shader blocks

## Hierarchy

- `PushMaterial`

  ↳ **`NodeMaterial`**

## Table of contents

### Constructors

- [constructor](NodeMaterial.md#constructor)

### Properties

- [BJSNODEMATERIALEDITOR](NodeMaterial.md#bjsnodematerialeditor)
- [\_activeEffect](NodeMaterial.md#_activeeffect)
- [\_alpha](NodeMaterial.md#_alpha)
- [\_animationFrame](NodeMaterial.md#_animationframe)
- [\_backFaceCulling](NodeMaterial.md#_backfaceculling)
- [\_buildId](NodeMaterial.md#_buildid)
- [\_buildWasSuccessful](NodeMaterial.md#_buildwassuccessful)
- [\_cachedWorldViewMatrix](NodeMaterial.md#_cachedworldviewmatrix)
- [\_cachedWorldViewProjectionMatrix](NodeMaterial.md#_cachedworldviewprojectionmatrix)
- [\_cullBackFaces](NodeMaterial.md#_cullbackfaces)
- [\_drawWrapper](NodeMaterial.md#_drawwrapper)
- [\_eventInfo](NodeMaterial.md#_eventinfo)
- [\_forceAlphaTest](NodeMaterial.md#_forcealphatest)
- [\_fragmentCompilationState](NodeMaterial.md#_fragmentcompilationstate)
- [\_fragmentOutputNodes](NodeMaterial.md#_fragmentoutputnodes)
- [\_imageProcessingConfiguration](NodeMaterial.md#_imageprocessingconfiguration)
- [\_imageProcessingObserver](NodeMaterial.md#_imageprocessingobserver)
- [\_needToBindSceneUbo](NodeMaterial.md#_needtobindsceneubo)
- [\_normalMatrix](NodeMaterial.md#_normalmatrix)
- [\_onEffectCreatedObservable](NodeMaterial.md#_oneffectcreatedobservable)
- [\_optimizers](NodeMaterial.md#_optimizers)
- [\_options](NodeMaterial.md#_options)
- [\_sharedData](NodeMaterial.md#_shareddata)
- [\_transparencyMode](NodeMaterial.md#_transparencymode)
- [\_vertexCompilationState](NodeMaterial.md#_vertexcompilationstate)
- [\_vertexOutputNodes](NodeMaterial.md#_vertexoutputnodes)
- [allowShaderHotSwapping](NodeMaterial.md#allowshaderhotswapping)
- [animations](NodeMaterial.md#animations)
- [attachedBlocks](NodeMaterial.md#attachedblocks)
- [checkReadyOnEveryCall](NodeMaterial.md#checkreadyoneverycall)
- [checkReadyOnlyOnce](NodeMaterial.md#checkreadyonlyonce)
- [comment](NodeMaterial.md#comment)
- [customShaderNameResolve](NodeMaterial.md#customshadernameresolve)
- [depthFunction](NodeMaterial.md#depthfunction)
- [disableColorWrite](NodeMaterial.md#disablecolorwrite)
- [disableDepthWrite](NodeMaterial.md#disabledepthwrite)
- [doNotSerialize](NodeMaterial.md#donotserialize)
- [editorData](NodeMaterial.md#editordata)
- [forceAlphaBlending](NodeMaterial.md#forcealphablending)
- [forceDepthWrite](NodeMaterial.md#forcedepthwrite)
- [getRenderTargetTextures](NodeMaterial.md#getrendertargettextures)
- [id](NodeMaterial.md#id)
- [ignoreAlpha](NodeMaterial.md#ignorealpha)
- [inspectableCustomProperties](NodeMaterial.md#inspectablecustomproperties)
- [maxSimultaneousLights](NodeMaterial.md#maxsimultaneouslights)
- [metadata](NodeMaterial.md#metadata)
- [name](NodeMaterial.md#name)
- [onBuildObservable](NodeMaterial.md#onbuildobservable)
- [onCompiled](NodeMaterial.md#oncompiled)
- [onDisposeObservable](NodeMaterial.md#ondisposeobservable)
- [onError](NodeMaterial.md#onerror)
- [pluginManager](NodeMaterial.md#pluginmanager)
- [pointSize](NodeMaterial.md#pointsize)
- [reservedDataStore](NodeMaterial.md#reserveddatastore)
- [separateCullingPass](NodeMaterial.md#separatecullingpass)
- [shadowDepthWrapper](NodeMaterial.md#shadowdepthwrapper)
- [sideOrientation](NodeMaterial.md#sideorientation)
- [snippetId](NodeMaterial.md#snippetid)
- [state](NodeMaterial.md#state)
- [stencil](NodeMaterial.md#stencil)
- [uniqueId](NodeMaterial.md#uniqueid)
- [zOffset](NodeMaterial.md#zoffset)
- [zOffsetUnits](NodeMaterial.md#zoffsetunits)
- [AllDirtyFlag](NodeMaterial.md#alldirtyflag)
- [AttributesDirtyFlag](NodeMaterial.md#attributesdirtyflag)
- [ClockWiseSideOrientation](NodeMaterial.md#clockwisesideorientation)
- [CounterClockWiseSideOrientation](NodeMaterial.md#counterclockwisesideorientation)
- [EditorURL](NodeMaterial.md#editorurl)
- [FresnelDirtyFlag](NodeMaterial.md#fresneldirtyflag)
- [IgnoreTexturesAtLoadTime](NodeMaterial.md#ignoretexturesatloadtime)
- [LightDirtyFlag](NodeMaterial.md#lightdirtyflag)
- [LineListDrawMode](NodeMaterial.md#linelistdrawmode)
- [LineLoopDrawMode](NodeMaterial.md#lineloopdrawmode)
- [LineStripDrawMode](NodeMaterial.md#linestripdrawmode)
- [MATERIAL\_ALPHABLEND](NodeMaterial.md#material_alphablend)
- [MATERIAL\_ALPHATEST](NodeMaterial.md#material_alphatest)
- [MATERIAL\_ALPHATESTANDBLEND](NodeMaterial.md#material_alphatestandblend)
- [MATERIAL\_NORMALBLENDMETHOD\_RNM](NodeMaterial.md#material_normalblendmethod_rnm)
- [MATERIAL\_NORMALBLENDMETHOD\_WHITEOUT](NodeMaterial.md#material_normalblendmethod_whiteout)
- [MATERIAL\_OPAQUE](NodeMaterial.md#material_opaque)
- [MiscDirtyFlag](NodeMaterial.md#miscdirtyflag)
- [OnEventObservable](NodeMaterial.md#oneventobservable)
- [PointFillMode](NodeMaterial.md#pointfillmode)
- [PointListDrawMode](NodeMaterial.md#pointlistdrawmode)
- [PrePassDirtyFlag](NodeMaterial.md#prepassdirtyflag)
- [SnippetUrl](NodeMaterial.md#snippeturl)
- [TextureDirtyFlag](NodeMaterial.md#texturedirtyflag)
- [TriangleFanDrawMode](NodeMaterial.md#trianglefandrawmode)
- [TriangleFillMode](NodeMaterial.md#trianglefillmode)
- [TriangleStripDrawMode](NodeMaterial.md#trianglestripdrawmode)
- [WireFrameFillMode](NodeMaterial.md#wireframefillmode)
- [\_BuildIdGenerator](NodeMaterial.md#_buildidgenerator)

### Accessors

- [\_disableAlphaBlending](NodeMaterial.md#_disablealphablending)
- [alpha](NodeMaterial.md#alpha)
- [alphaMode](NodeMaterial.md#alphamode)
- [backFaceCulling](NodeMaterial.md#backfaceculling)
- [buildId](NodeMaterial.md#buildid)
- [canRenderToMRT](NodeMaterial.md#canrendertomrt)
- [compiledShaders](NodeMaterial.md#compiledshaders)
- [cullBackFaces](NodeMaterial.md#cullbackfaces)
- [fillMode](NodeMaterial.md#fillmode)
- [fogEnabled](NodeMaterial.md#fogenabled)
- [hasRenderTargetTextures](NodeMaterial.md#hasrendertargettextures)
- [imageProcessingConfiguration](NodeMaterial.md#imageprocessingconfiguration)
- [isFrozen](NodeMaterial.md#isfrozen)
- [isPrePassCapable](NodeMaterial.md#isprepasscapable)
- [mode](NodeMaterial.md#mode)
- [needDepthPrePass](NodeMaterial.md#needdepthprepass)
- [onBind](NodeMaterial.md#onbind)
- [onBindObservable](NodeMaterial.md#onbindobservable)
- [onDispose](NodeMaterial.md#ondispose)
- [onEffectCreatedObservable](NodeMaterial.md#oneffectcreatedobservable)
- [onUnBindObservable](NodeMaterial.md#onunbindobservable)
- [options](NodeMaterial.md#options)
- [pointsCloud](NodeMaterial.md#pointscloud)
- [transparencyMode](NodeMaterial.md#transparencymode)
- [wireframe](NodeMaterial.md#wireframe)

### Methods

- [\_addFragmentOutputNode](NodeMaterial.md#_addfragmentoutputnode)
- [\_addVertexOutputNode](NodeMaterial.md#_addvertexoutputnode)
- [\_afterBind](NodeMaterial.md#_afterbind)
- [\_attachImageProcessingConfiguration](NodeMaterial.md#_attachimageprocessingconfiguration)
- [\_checkInternals](NodeMaterial.md#_checkinternals)
- [\_createEffectForParticles](NodeMaterial.md#_createeffectforparticles)
- [\_createEffectForPostProcess](NodeMaterial.md#_createeffectforpostprocess)
- [\_createNodeEditor](NodeMaterial.md#_createnodeeditor)
- [\_gatherBlocks](NodeMaterial.md#_gatherblocks)
- [\_getGlobalNodeMaterialEditor](NodeMaterial.md#_getglobalnodematerialeditor)
- [\_initializeBlock](NodeMaterial.md#_initializeblock)
- [\_isReadyForSubMesh](NodeMaterial.md#_isreadyforsubmesh)
- [\_markAllSubMeshesAsAllDirty](NodeMaterial.md#_markallsubmeshesasalldirty)
- [\_markAllSubMeshesAsAttributesDirty](NodeMaterial.md#_markallsubmeshesasattributesdirty)
- [\_markAllSubMeshesAsDirty](NodeMaterial.md#_markallsubmeshesasdirty)
- [\_markAllSubMeshesAsFresnelAndMiscDirty](NodeMaterial.md#_markallsubmeshesasfresnelandmiscdirty)
- [\_markAllSubMeshesAsFresnelDirty](NodeMaterial.md#_markallsubmeshesasfresneldirty)
- [\_markAllSubMeshesAsImageProcessingDirty](NodeMaterial.md#_markallsubmeshesasimageprocessingdirty)
- [\_markAllSubMeshesAsLightsDirty](NodeMaterial.md#_markallsubmeshesaslightsdirty)
- [\_markAllSubMeshesAsMiscDirty](NodeMaterial.md#_markallsubmeshesasmiscdirty)
- [\_markAllSubMeshesAsPrePassDirty](NodeMaterial.md#_markallsubmeshesasprepassdirty)
- [\_markAllSubMeshesAsTexturesAndMiscDirty](NodeMaterial.md#_markallsubmeshesastexturesandmiscdirty)
- [\_markAllSubMeshesAsTexturesDirty](NodeMaterial.md#_markallsubmeshesastexturesdirty)
- [\_markScenePrePassDirty](NodeMaterial.md#_marksceneprepassdirty)
- [\_mustRebind](NodeMaterial.md#_mustrebind)
- [\_prepareDefinesForAttributes](NodeMaterial.md#_preparedefinesforattributes)
- [\_processDefines](NodeMaterial.md#_processdefines)
- [\_removeFragmentOutputNode](NodeMaterial.md#_removefragmentoutputnode)
- [\_removeVertexOutputNode](NodeMaterial.md#_removevertexoutputnode)
- [\_resetDualBlocks](NodeMaterial.md#_resetdualblocks)
- [\_restoreConnections](NodeMaterial.md#_restoreconnections)
- [\_shouldTurnAlphaTestOn](NodeMaterial.md#_shouldturnalphateston)
- [addOutputNode](NodeMaterial.md#addoutputnode)
- [bind](NodeMaterial.md#bind)
- [bindEyePosition](NodeMaterial.md#bindeyeposition)
- [bindForSubMesh](NodeMaterial.md#bindforsubmesh)
- [bindOnlyNormalMatrix](NodeMaterial.md#bindonlynormalmatrix)
- [bindOnlyWorldMatrix](NodeMaterial.md#bindonlyworldmatrix)
- [bindView](NodeMaterial.md#bindview)
- [bindViewProjection](NodeMaterial.md#bindviewprojection)
- [build](NodeMaterial.md#build)
- [buildUniformLayout](NodeMaterial.md#builduniformlayout)
- [clear](NodeMaterial.md#clear)
- [clone](NodeMaterial.md#clone)
- [createEffectForParticles](NodeMaterial.md#createeffectforparticles)
- [createEffectForPostProcess](NodeMaterial.md#createeffectforpostprocess)
- [createPostProcess](NodeMaterial.md#createpostprocess)
- [createProceduralTexture](NodeMaterial.md#createproceduraltexture)
- [dispose](NodeMaterial.md#dispose)
- [edit](NodeMaterial.md#edit)
- [forceCompilation](NodeMaterial.md#forcecompilation)
- [forceCompilationAsync](NodeMaterial.md#forcecompilationasync)
- [freeze](NodeMaterial.md#freeze)
- [generateCode](NodeMaterial.md#generatecode)
- [getActiveTextures](NodeMaterial.md#getactivetextures)
- [getAlphaTestTexture](NodeMaterial.md#getalphatesttexture)
- [getAnimatables](NodeMaterial.md#getanimatables)
- [getBindedMeshes](NodeMaterial.md#getbindedmeshes)
- [getBlockByName](NodeMaterial.md#getblockbyname)
- [getBlockByPredicate](NodeMaterial.md#getblockbypredicate)
- [getClassName](NodeMaterial.md#getclassname)
- [getEffect](NodeMaterial.md#geteffect)
- [getInputBlockByPredicate](NodeMaterial.md#getinputblockbypredicate)
- [getInputBlocks](NodeMaterial.md#getinputblocks)
- [getScene](NodeMaterial.md#getscene)
- [getTextureBlocks](NodeMaterial.md#gettextureblocks)
- [hasTexture](NodeMaterial.md#hastexture)
- [isReady](NodeMaterial.md#isready)
- [isReadyForSubMesh](NodeMaterial.md#isreadyforsubmesh)
- [loadAsync](NodeMaterial.md#loadasync)
- [loadFromSerialization](NodeMaterial.md#loadfromserialization)
- [markAsDirty](NodeMaterial.md#markasdirty)
- [markDirty](NodeMaterial.md#markdirty)
- [needAlphaBlending](NodeMaterial.md#needalphablending)
- [needAlphaBlendingForMesh](NodeMaterial.md#needalphablendingformesh)
- [needAlphaTesting](NodeMaterial.md#needalphatesting)
- [optimize](NodeMaterial.md#optimize)
- [parseSerializedObject](NodeMaterial.md#parseserializedobject)
- [registerOptimizer](NodeMaterial.md#registeroptimizer)
- [removeBlock](NodeMaterial.md#removeblock)
- [removeOutputNode](NodeMaterial.md#removeoutputnode)
- [resetDrawCache](NodeMaterial.md#resetdrawcache)
- [serialize](NodeMaterial.md#serialize)
- [setPrePassRenderer](NodeMaterial.md#setprepassrenderer)
- [setToDefault](NodeMaterial.md#settodefault)
- [setToDefaultParticle](NodeMaterial.md#settodefaultparticle)
- [setToDefaultPostProcess](NodeMaterial.md#settodefaultpostprocess)
- [setToDefaultProceduralTexture](NodeMaterial.md#settodefaultproceduraltexture)
- [toString](NodeMaterial.md#tostring)
- [unbind](NodeMaterial.md#unbind)
- [unfreeze](NodeMaterial.md#unfreeze)
- [unregisterOptimizer](NodeMaterial.md#unregisteroptimizer)
- [CreateDefault](NodeMaterial.md#createdefault)
- [Parse](NodeMaterial.md#parse)
- [ParseFromFileAsync](NodeMaterial.md#parsefromfileasync)
- [ParseFromSnippetAsync](NodeMaterial.md#parsefromsnippetasync)

## Constructors

### constructor

• **new NodeMaterial**(`name`, `scene?`, `options?`)

Create a new node based material

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the material name |
| `scene?` | [`Scene`](Scene.md) | defines the hosting scene |
| `options` | `Partial`[`INodeMaterialOptions`](../interfaces/INodeMaterialOptions.md) | defines creation option |

#### Overrides

PushMaterial.constructor

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:304

## Properties

### BJSNODEMATERIALEDITOR

• `Private` **BJSNODEMATERIALEDITOR**: `any`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:172

___

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

### \_animationFrame

• `Private` **\_animationFrame**: `number` = `-1`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:161

___

### \_backFaceCulling

• `Protected` **\_backFaceCulling**: `boolean` = `true`

Specifies if back face culling is enabled

#### Inherited from

PushMaterial.\_backFaceCulling

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:328

___

### \_buildId

• `Private` **\_buildId**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:156

___

### \_buildWasSuccessful

• `Private` **\_buildWasSuccessful**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:157

___

### \_cachedWorldViewMatrix

• `Private` **\_cachedWorldViewMatrix**: [`Matrix`](Matrix.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:158

___

### \_cachedWorldViewProjectionMatrix

• `Private` **\_cachedWorldViewProjectionMatrix**: [`Matrix`](Matrix.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:159

___

### \_cullBackFaces

• `Protected` **\_cullBackFaces**: `boolean` = `true`

Specifies if back or front faces should be culled (when culling is enabled)

#### Inherited from

PushMaterial.\_cullBackFaces

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:352

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

### \_forceAlphaTest

• `Protected` **\_forceAlphaTest**: `boolean` = `false`

Enforces alpha test in opaque or blend mode in order to improve the performances of some situations.

#### Inherited from

PushMaterial.\_forceAlphaTest

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:954

___

### \_fragmentCompilationState

• `Private` **\_fragmentCompilationState**: `NodeMaterialBuildState`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:154

___

### \_fragmentOutputNodes

• **\_fragmentOutputNodes**: [`NodeMaterialBlock`](NodeMaterialBlock.md)[]

Gets or sets the root nodes of the material fragment (pixel) shader

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:225

___

### \_imageProcessingConfiguration

• `Protected` **\_imageProcessingConfiguration**: [`ImageProcessingConfiguration`](ImageProcessingConfiguration.md)

Default configuration related to image processing available in the standard Material.

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:239

___

### \_imageProcessingObserver

• `Private` **\_imageProcessingObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`ImageProcessingConfiguration`](ImageProcessingConfiguration.md)

Keep track of the image processing observer to allow dispose and replace.

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:327

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

### \_optimizers

• `Private` **\_optimizers**: [`NodeMaterialOptimizer`](NodeMaterialOptimizer.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:160

___

### \_options

• `Private` **\_options**: [`INodeMaterialOptions`](../interfaces/INodeMaterialOptions.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:152

___

### \_sharedData

• `Private` **\_sharedData**: `NodeMaterialBuildStateSharedData`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:155

___

### \_transparencyMode

• `Protected` **\_transparencyMode**: [`Nullable`](../modules.md#nullable)`number` = `null`

The transparency mode of the material.

#### Inherited from

PushMaterial.\_transparencyMode

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:959

___

### \_vertexCompilationState

• `Private` **\_vertexCompilationState**: `NodeMaterialBuildState`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:153

___

### \_vertexOutputNodes

• **\_vertexOutputNodes**: [`NodeMaterialBlock`](NodeMaterialBlock.md)[]

Gets or sets the root nodes of the material vertex shader

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:220

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

### attachedBlocks

• **attachedBlocks**: [`NodeMaterialBlock`](NodeMaterialBlock.md)[]

Gets an array of blocks that needs to be serialized even if they are not yet connected

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:263

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

### comment

• **comment**: `string`

A free comment about the material

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:296

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

### editorData

• **editorData**: `any` = `null`

Gets or sets data used by visual editor

**`See`**

https://nme.babylonjs.com

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:198

___

### forceAlphaBlending

• **forceAlphaBlending**: `boolean` = `false`

Gets or sets a boolean indicating that alpha blending must be enabled no matter what alpha value or alpha channel of the FragmentBlock are

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:548

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

### ignoreAlpha

• **ignoreAlpha**: `boolean` = `false`

Gets or sets a boolean indicating that alpha value must be ignored (This will turn alpha blending off even if an alpha value is produced by the material)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:204

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

### maxSimultaneousLights

• **maxSimultaneousLights**: `number` = `4`

Defines the maximum number of lights that can be used in the material

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:210

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

### onBuildObservable

• **onBuildObservable**: [`Observable`](Observable.md)[`NodeMaterial`](NodeMaterial.md)

Observable raised when the material is built

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:215

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

### sideOrientation

• **sideOrientation**: `number`

Stores the value for side orientation

#### Inherited from

PushMaterial.sideOrientation

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:376

___

### snippetId

• **snippetId**: `string`

Snippet ID if the material was created from the snippet server

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:192

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

### EditorURL

▪ `Static` **EditorURL**: `string`

Define the Url to load node editor script

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:164

___

### FresnelDirtyFlag

▪ `Static` `Readonly` **FresnelDirtyFlag**: ``4``

The dirty fresnel flag value

#### Inherited from

PushMaterial.FresnelDirtyFlag

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:144

___

### IgnoreTexturesAtLoadTime

▪ `Static` **IgnoreTexturesAtLoadTime**: `boolean` = `false`

Gets or sets a boolean indicating that node materials should not deserialize textures from json / snippet content

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:170

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

### SnippetUrl

▪ `Static` **SnippetUrl**: `string` = `Constants.SnippetUrl`

Define the Url to load snippets

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:167

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

___

### \_BuildIdGenerator

▪ `Static` `Private` **\_BuildIdGenerator**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:151

## Accessors

### \_disableAlphaBlending

• `Protected` `get` **_disableAlphaBlending**(): `boolean`

Returns true if alpha blending should be disabled.

#### Returns

`boolean`

#### Inherited from

PushMaterial.\_disableAlphaBlending

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:995

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

### buildId

• `get` **buildId**(): `number`

Gets or sets the unique identifier used to identified the effect associated with the material

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:284

• `set` **buildId**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:288

___

### canRenderToMRT

• `get` **canRenderToMRT**(): `boolean`

If the material can be rendered to several textures with MRT extension

#### Returns

`boolean`

#### Inherited from

PushMaterial.canRenderToMRT

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:282

___

### compiledShaders

• `get` **compiledShaders**(): `string`

Get a string representing the shaders built by the current node graph

#### Returns

`string`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:1342

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

#### Inherited from

PushMaterial.hasRenderTargetTextures

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:396

___

### imageProcessingConfiguration

• `get` **imageProcessingConfiguration**(): [`ImageProcessingConfiguration`](ImageProcessingConfiguration.md)

Gets the image processing configuration used either in this material.

#### Returns

[`ImageProcessingConfiguration`](ImageProcessingConfiguration.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:244

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

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:253

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

#### Inherited from

PushMaterial.isPrePassCapable

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:558

___

### mode

• `get` **mode**(): [`NodeMaterialModes`](../enums/NodeMaterialModes.md)

Gets or sets the mode property

#### Returns

[`NodeMaterialModes`](../enums/NodeMaterialModes.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:275

• `set` **mode**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`NodeMaterialModes`](../enums/NodeMaterialModes.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:279

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

### options

• `get` **options**(): [`INodeMaterialOptions`](../interfaces/INodeMaterialOptions.md)

Gets or sets options to control the node material overall behavior

#### Returns

[`INodeMaterialOptions`](../interfaces/INodeMaterialOptions.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:228

• `set` **options**(`options`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `options` | [`INodeMaterialOptions`](../interfaces/INodeMaterialOptions.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:232

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

### \_addFragmentOutputNode

▸ `Private` **_addFragmentOutputNode**(`node`): `undefined` \| [`NodeMaterial`](NodeMaterial.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `node` | [`NodeMaterialBlock`](NodeMaterialBlock.md) |

#### Returns

`undefined` \| [`NodeMaterial`](NodeMaterial.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:522

___

### \_addVertexOutputNode

▸ `Private` **_addVertexOutputNode**(`node`): `undefined` \| [`NodeMaterial`](NodeMaterial.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `node` | [`NodeMaterialBlock`](NodeMaterialBlock.md) |

#### Returns

`undefined` \| [`NodeMaterial`](NodeMaterial.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:500

___

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

Attaches a new image processing configuration to the Standard Material.

#### Parameters

| Name | Type |
| :------ | :------ |
| `configuration` | [`Nullable`](../modules.md#nullable)[`ImageProcessingConfiguration`](ImageProcessingConfiguration.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:333

___

### \_checkInternals

▸ `Private` **_checkInternals**(`effect`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `effect` | [`Effect`](Effect.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:1103

___

### \_createEffectForParticles

▸ `Private` **_createEffectForParticles**(`particleSystem`, `blendMode`, `onCompiled?`, `onError?`, `effect?`, `defines?`, `dummyMesh?`, `particleSystemDefinesJoined?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `particleSystem` | [`IParticleSystem`](../interfaces/IParticleSystem.md) | `undefined` |
| `blendMode` | `number` | `undefined` |
| `onCompiled?` | (`effect`: [`Effect`](Effect.md)) => `void` | `undefined` |
| `onError?` | (`effect`: [`Effect`](Effect.md), `errors`: `string`) => `void` | `undefined` |
| `effect?` | [`Effect`](Effect.md) | `undefined` |
| `defines?` | `NodeMaterialDefines` | `undefined` |
| `dummyMesh?` | [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md) | `undefined` |
| `particleSystemDefinesJoined` | `string` | `""` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:999

___

### \_createEffectForPostProcess

▸ `Private` **_createEffectForPostProcess**(`postProcess`, `camera?`, `options?`, `samplingMode?`, `engine?`, `reusable?`, `textureType?`, `textureFormat?`): [`PostProcess`](PostProcess.md)

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `postProcess` | [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md) | `undefined` |
| `camera?` | [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md) | `undefined` |
| `options` | `number` \| [`PostProcessOptions`](../modules.md#postprocessoptions) | `1` |
| `samplingMode` | `number` | `Constants.TEXTURE_NEAREST_SAMPLINGMODE` |
| `engine?` | [`Engine`](Engine.md) | `undefined` |
| `reusable?` | `boolean` | `undefined` |
| `textureType` | `number` | `Constants.TEXTURETYPE_UNSIGNED_INT` |
| `textureFormat` | `number` | `Constants.TEXTUREFORMAT_RGBA` |

#### Returns

[`PostProcess`](PostProcess.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:824

___

### \_createNodeEditor

▸ `Private` **_createNodeEditor**(): `void`

Creates the node editor window.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:1500

___

### \_gatherBlocks

▸ `Private` **_gatherBlocks**(`rootNode`, `list`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `rootNode` | [`NodeMaterialBlock`](NodeMaterialBlock.md) |
| `list` | [`NodeMaterialBlock`](NodeMaterialBlock.md)[] |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:1741

___

### \_getGlobalNodeMaterialEditor

▸ `Private` **_getGlobalNodeMaterialEditor**(): `any`

Get the inspector from bundle or global

#### Returns

`any`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:175

___

### \_initializeBlock

▸ `Private` **_initializeBlock**(`node`, `state`, `nodesToProcessForOtherBuildState`, `autoConfigure?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `node` | [`NodeMaterialBlock`](NodeMaterialBlock.md) | `undefined` |
| `state` | `NodeMaterialBuildState` | `undefined` |
| `nodesToProcessForOtherBuildState` | [`NodeMaterialBlock`](NodeMaterialBlock.md)[] | `undefined` |
| `autoConfigure` | `boolean` | `true` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:569

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

### \_prepareDefinesForAttributes

▸ `Private` **_prepareDefinesForAttributes**(`mesh`, `defines`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) |
| `defines` | `NodeMaterialDefines` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:769

___

### \_processDefines

▸ `Private` **_processDefines**(`mesh`, `defines`, `useInstances?`, `subMesh?`): [`Nullable`](../modules.md#nullable){ `fallbacks`: [`EffectFallbacks`](EffectFallbacks.md) ; `lightDisposed`: `boolean` ; `mergedSamplers`: `string`[] ; `mergedUniforms`: `string`[] ; `uniformBuffers`: `string`[]  }

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | `undefined` |
| `defines` | `NodeMaterialDefines` | `undefined` |
| `useInstances` | `boolean` | `false` |
| `subMesh?` | [`SubMesh`](SubMesh.md) | `undefined` |

#### Returns

[`Nullable`](../modules.md#nullable){ `fallbacks`: [`EffectFallbacks`](EffectFallbacks.md) ; `lightDisposed`: `boolean` ; `mergedSamplers`: `string`[] ; `mergedUniforms`: `string`[] ; `uniformBuffers`: `string`[]  }

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:1146

___

### \_removeFragmentOutputNode

▸ `Private` **_removeFragmentOutputNode**(`node`): `undefined` \| [`NodeMaterial`](NodeMaterial.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `node` | [`NodeMaterialBlock`](NodeMaterialBlock.md) |

#### Returns

`undefined` \| [`NodeMaterial`](NodeMaterial.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:533

___

### \_removeVertexOutputNode

▸ `Private` **_removeVertexOutputNode**(`node`): `undefined` \| [`NodeMaterial`](NodeMaterial.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `node` | [`NodeMaterialBlock`](NodeMaterialBlock.md) |

#### Returns

`undefined` \| [`NodeMaterial`](NodeMaterial.md)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:511

___

### \_resetDualBlocks

▸ `Private` **_resetDualBlocks**(`node`, `id`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `node` | [`NodeMaterialBlock`](NodeMaterialBlock.md) |
| `id` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:611

___

### \_restoreConnections

▸ `Private` **_restoreConnections**(`block`, `source`, `map`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `block` | [`NodeMaterialBlock`](NodeMaterialBlock.md) |
| `source` | `any` |
| `map` | `Object` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:1867

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

### addOutputNode

▸ **addOutputNode**(`node`): [`NodeMaterial`](NodeMaterial.md)

Add a new block to the list of output nodes

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `node` | [`NodeMaterialBlock`](NodeMaterialBlock.md) | defines the node to add |

#### Returns

[`NodeMaterial`](NodeMaterial.md)

the current material

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:463

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

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:1379

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

Binds the world matrix to the material

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `world` | [`Matrix`](Matrix.md) | defines the world transformation matrix |

#### Returns

`void`

#### Overrides

PushMaterial.bindOnlyWorldMatrix

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:1350

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

### build

▸ **build**(`verbose?`, `updateBuildId?`, `autoConfigure?`): `void`

Build the material and generates the inner effect

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `verbose` | `boolean` | `false` | defines if the build should log activity |
| `updateBuildId` | `boolean` | `true` | defines if the internal build Id should be updated (default is true) |
| `autoConfigure` | `boolean` | `true` | defines if the autoConfigure method should be called when initializing blocks (default is true) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:648

___

### buildUniformLayout

▸ **buildUniformLayout**(): `void`

Initializes the uniform buffer layout for the shader.

#### Returns

`void`

#### Inherited from

PushMaterial.buildUniformLayout

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:1104

___

### clear

▸ **clear**(): `void`

Clear the current material

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:1534

___

### clone

▸ **clone**(`name`, `shareEffect?`): [`NodeMaterial`](NodeMaterial.md)

Makes a duplicate of the current material.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | defines the name to use for the new material |
| `shareEffect` | `boolean` | `false` | defines if the clone material should share the same effect (default is false) |

#### Returns

[`NodeMaterial`](NodeMaterial.md)

#### Overrides

PushMaterial.clone

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:2002

___

### createEffectForParticles

▸ **createEffectForParticles**(`particleSystem`, `onCompiled?`, `onError?`): `void`

Create the effect to be used as the custom effect for a particle system

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `particleSystem` | [`IParticleSystem`](../interfaces/IParticleSystem.md) | Particle system to create the effect for |
| `onCompiled?` | (`effect`: [`Effect`](Effect.md)) => `void` | defines a function to call when the effect creation is successful |
| `onError?` | (`effect`: [`Effect`](Effect.md), `errors`: `string`) => `void` | defines a function to call when the effect creation has failed |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:1136

___

### createEffectForPostProcess

▸ **createEffectForPostProcess**(`postProcess`): `void`

Create the post process effect from the material

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `postProcess` | [`PostProcess`](PostProcess.md) | The post process to create the effect for |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:820

___

### createPostProcess

▸ **createPostProcess**(`camera`, `options?`, `samplingMode?`, `engine?`, `reusable?`, `textureType?`, `textureFormat?`): [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)

Create a post process from the material

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `camera` | [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md) | `undefined` | The camera to apply the render pass to. |
| `options` | `number` \| [`PostProcessOptions`](../modules.md#postprocessoptions) | `1` | The required width/height ratio to downsize to before computing the render pass. (Use 1.0 for full size) |
| `samplingMode` | `number` | `Constants.TEXTURE_NEAREST_SAMPLINGMODE` | The sampling mode to be used when computing the pass. (default: 0) |
| `engine?` | [`Engine`](Engine.md) | `undefined` | The engine which the post process will be applied. (default: current engine) |
| `reusable?` | `boolean` | `undefined` | If the post process can be reused on the same frame. (default: false) |
| `textureType` | `number` | `Constants.TEXTURETYPE_UNSIGNED_INT` | Type of textures used when performing the post process. (default: 0) |
| `textureFormat` | `number` | `Constants.TEXTUREFORMAT_RGBA` | Format of textures used when performing the post process. (default: TEXTUREFORMAT_RGBA) |

#### Returns

[`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)

the post process created

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:800

___

### createProceduralTexture

▸ **createProceduralTexture**(`size`, `scene`): [`Nullable`](../modules.md#nullable)[`ProceduralTexture`](ProceduralTexture.md)

Create a new procedural texture based on this node material

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `size` | `number` \| { `height`: `number` ; `layers?`: `number` ; `width`: `number`  } | defines the size of the texture |
| `scene` | [`Scene`](Scene.md) | defines the hosting scene |

#### Returns

[`Nullable`](../modules.md#nullable)[`ProceduralTexture`](ProceduralTexture.md)

the new procedural texture attached to this node material

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:922

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

#### Overrides

PushMaterial.dispose

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:1471

___

### edit

▸ **edit**(`config?`): `Promise``void`

Launch the node material editor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `config?` | [`INodeMaterialEditorOptions`](../interfaces/INodeMaterialEditorOptions.md) | Define the configuration of the editor |

#### Returns

`Promise``void`

a promise fulfilled when the node editor is visible

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:1511

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

### generateCode

▸ **generateCode**(): `string`

Generate a string containing the code declaration required to create an equivalent of this material

#### Returns

`string`

a string

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:1762

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

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:1420

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

https://github.com/babylon.js/core/src/Materials/material.ts:1048

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

https://github.com/babylon.js/core/src/Materials/material.ts:1247

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

### getBlockByName

▸ **getBlockByName**(`name`): ``null`` \| [`NodeMaterialBlock`](NodeMaterialBlock.md)

Get a block by its name

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the name of the block to retrieve |

#### Returns

``null`` \| [`NodeMaterialBlock`](NodeMaterialBlock.md)

the required block or null if not found

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:363

___

### getBlockByPredicate

▸ **getBlockByPredicate**(`predicate`): ``null`` \| [`NodeMaterialBlock`](NodeMaterialBlock.md)

Get a block by its name

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `predicate` | (`block`: [`NodeMaterialBlock`](NodeMaterialBlock.md)) => `boolean` | defines the predicate used to find the good candidate |

#### Returns

``null`` \| [`NodeMaterialBlock`](NodeMaterialBlock.md)

the required block or null if not found

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:384

___

### getClassName

▸ **getClassName**(): `string`

Gets the current class name of the material e.g. "NodeMaterial"

#### Returns

`string`

the class name

#### Overrides

PushMaterial.getClassName

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:320

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

### getInputBlockByPredicate

▸ **getInputBlockByPredicate**(`predicate`): [`Nullable`](../modules.md#nullable)[`InputBlock`](InputBlock.md)

Get an input block by its name

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `predicate` | (`block`: [`InputBlock`](InputBlock.md)) => `boolean` | defines the predicate used to find the good candidate |

#### Returns

[`Nullable`](../modules.md#nullable)[`InputBlock`](InputBlock.md)

the required input block or null if not found

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:399

___

### getInputBlocks

▸ **getInputBlocks**(): [`InputBlock`](InputBlock.md)[]

Gets the list of input blocks attached to this material

#### Returns

[`InputBlock`](InputBlock.md)[]

an array of InputBlocks

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:413

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

### getTextureBlocks

▸ **getTextureBlocks**(): ([`TextureBlock`](TextureBlock.md) \| `ReflectionTextureBaseBlock` \| [`RefractionBlock`](RefractionBlock.md) \| [`CurrentScreenBlock`](CurrentScreenBlock.md) \| [`ParticleTextureBlock`](ParticleTextureBlock.md) \| [`ImageSourceBlock`](ImageSourceBlock.md))[]

Gets the list of texture blocks

#### Returns

([`TextureBlock`](TextureBlock.md) \| `ReflectionTextureBaseBlock` \| [`RefractionBlock`](RefractionBlock.md) \| [`CurrentScreenBlock`](CurrentScreenBlock.md) \| [`ParticleTextureBlock`](ParticleTextureBlock.md) \| [`ImageSourceBlock`](ImageSourceBlock.md))[]

an array of texture blocks

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:1434

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

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:1447

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

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:1235

___

### loadAsync

▸ **loadAsync**(`url`, `rootUrl?`): `Promise`[`NodeMaterial`](NodeMaterial.md)

Loads the current Node Material from a url pointing to a file save by the Node Material Editor

**`Deprecated`**

Please use NodeMaterial.ParseFromFileAsync instead

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `url` | `string` | `undefined` | defines the url to load from |
| `rootUrl` | `string` | `""` | defines the root URL for nested url in the node material |

#### Returns

`Promise`[`NodeMaterial`](NodeMaterial.md)

a promise that will fulfil when the material is fully loaded

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:1737

___

### loadFromSerialization

▸ **loadFromSerialization**(`source`, `rootUrl?`, `merge?`): `void`

Clear the current graph and load a new one from a serialization object

**`Deprecated`**

Please use the parseSerializedObject method instead

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `source` | `any` | `undefined` | defines the JSON representation of the material |
| `rootUrl` | `string` | `""` | defines the root URL to use to load textures and relative dependencies |
| `merge` | `boolean` | `false` | defines whether or not the source must be merged or replace the current content |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:1993

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

Specifies if the material will require alpha blending

#### Returns

`boolean`

a boolean specifying if alpha blending is needed

#### Overrides

PushMaterial.needAlphaBlending

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:554

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

Specifies if this material should be rendered in alpha test mode

#### Returns

`boolean`

a boolean specifying if an alpha test is needed.

#### Overrides

PushMaterial.needAlphaTesting

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:565

___

### optimize

▸ **optimize**(): `void`

Runs an otpimization phase to try to improve the shader code

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:763

___

### parseSerializedObject

▸ **parseSerializedObject**(`source`, `rootUrl?`, `merge?`): `void`

Clear the current graph and load a new one from a serialization object

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `source` | `any` | `undefined` | defines the JSON representation of the material |
| `rootUrl` | `string` | `""` | defines the root URL to use to load textures and relative dependencies |
| `merge` | `boolean` | `false` | defines whether or not the source must be merged or replace the current content |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:1898

___

### registerOptimizer

▸ **registerOptimizer**(`optimizer`): `undefined` \| [`NodeMaterial`](NodeMaterial.md)

Adds a new optimizer to the list of optimizers

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `optimizer` | [`NodeMaterialOptimizer`](NodeMaterialOptimizer.md) | defines the optimizers to add |

#### Returns

`undefined` \| [`NodeMaterial`](NodeMaterial.md)

the current material

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:429

___

### removeBlock

▸ **removeBlock**(`block`): `void`

Remove a block from the current node material

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `block` | [`NodeMaterialBlock`](NodeMaterialBlock.md) | defines the block to remove |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:631

___

### removeOutputNode

▸ **removeOutputNode**(`node`): [`NodeMaterial`](NodeMaterial.md)

Remove a block from the list of root nodes

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `node` | [`NodeMaterialBlock`](NodeMaterialBlock.md) | defines the node to remove |

#### Returns

[`NodeMaterial`](NodeMaterial.md)

the current material

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:484

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

▸ **serialize**(`selectedBlocks?`): `any`

Serializes this material in a JSON representation

#### Parameters

| Name | Type |
| :------ | :------ |
| `selectedBlocks?` | [`NodeMaterialBlock`](NodeMaterialBlock.md)[] |

#### Returns

`any`

the serialized material object

#### Overrides

PushMaterial.serialize

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:1821

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

https://github.com/babylon.js/core/src/Materials/material.ts:1616

___

### setToDefault

▸ **setToDefault**(): `void`

Clear the current material and set it to a default state

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:1543

___

### setToDefaultParticle

▸ **setToDefaultParticle**(): `void`

Clear the current material and set it to a default state for particle

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:1691

___

### setToDefaultPostProcess

▸ **setToDefaultPostProcess**(): `void`

Clear the current material and set it to a default state for post process

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:1585

___

### setToDefaultProceduralTexture

▸ **setToDefaultProceduralTexture**(): `void`

Clear the current material and set it to a default state for procedural texture

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:1635

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

### unregisterOptimizer

▸ **unregisterOptimizer**(`optimizer`): `undefined` \| [`NodeMaterial`](NodeMaterial.md)

Remove an optimizer from the list of optimizers

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `optimizer` | [`NodeMaterialOptimizer`](NodeMaterialOptimizer.md) | defines the optimizers to remove |

#### Returns

`undefined` \| [`NodeMaterial`](NodeMaterial.md)

the current material

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:446

___

### CreateDefault

▸ `Static` **CreateDefault**(`name`, `scene?`): [`NodeMaterial`](NodeMaterial.md)

Creates a new node material set to default basic configuration

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the name of the material |
| `scene?` | [`Scene`](Scene.md) | defines the hosting scene |

#### Returns

[`NodeMaterial`](NodeMaterial.md)

a new NodeMaterial

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:2114

___

### Parse

▸ `Static` **Parse**(`source`, `scene`, `rootUrl?`): [`NodeMaterial`](NodeMaterial.md)

Creates a node material from parsed material data

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `source` | `any` | `undefined` | defines the JSON representation of the material |
| `scene` | [`Scene`](Scene.md) | `undefined` | defines the hosting scene |
| `rootUrl` | `string` | `""` | defines the root URL to use to load textures and relative dependencies |

#### Returns

[`NodeMaterial`](NodeMaterial.md)

a new node material

#### Overrides

PushMaterial.Parse

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:2023

___

### ParseFromFileAsync

▸ `Static` **ParseFromFileAsync**(`name`, `url`, `scene`, `rootUrl?`, `skipBuild?`): `Promise`[`NodeMaterial`](NodeMaterial.md)

Creates a node material from a snippet saved in a remote file

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | defines the name of the material to create |
| `url` | `string` | `undefined` | defines the url to load from |
| `scene` | [`Scene`](Scene.md) | `undefined` | defines the hosting scene |
| `rootUrl` | `string` | `""` | defines the root URL for nested url in the node material |
| `skipBuild` | `boolean` | `false` | defines whether to build the node material |

#### Returns

`Promise`[`NodeMaterial`](NodeMaterial.md)

a promise that will resolve to the new node material

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:2041

___

### ParseFromSnippetAsync

▸ `Static` **ParseFromSnippetAsync**(`snippetId`, `scene?`, `rootUrl?`, `nodeMaterial?`, `skipBuild?`): `Promise`[`NodeMaterial`](NodeMaterial.md)

Creates a node material from a snippet saved by the node material editor

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `snippetId` | `string` | `undefined` | defines the snippet to load |
| `scene` | [`Scene`](Scene.md) | `undefined` | defines the hosting scene |
| `rootUrl` | `string` | `""` | defines the root URL to use to load textures and relative dependencies |
| `nodeMaterial?` | [`NodeMaterial`](NodeMaterial.md) | `undefined` | defines a node material to update (instead of creating a new one) |
| `skipBuild` | `boolean` | `false` | defines whether to build the node material |

#### Returns

`Promise`[`NodeMaterial`](NodeMaterial.md)

a promise that will resolve to the new node material

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterial.ts:2062
