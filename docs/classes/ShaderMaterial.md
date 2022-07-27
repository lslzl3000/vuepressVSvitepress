[@dev/core](../README.md) / [Exports](../modules.md) / ShaderMaterial

# Class: ShaderMaterial

The ShaderMaterial object has the necessary methods to pass data from your scene to the Vertex and Fragment Shaders and returns a material that can be applied to any mesh.

This returned material effects how the mesh will look based on the code in the shaders.

**`See`**

https://doc.babylonjs.com/advanced_topics/shaders/shaderMaterial

## Hierarchy

- `PushMaterial`

  ↳ **`ShaderMaterial`**

  ↳↳ [`OcclusionMaterial`](OcclusionMaterial.md)

## Table of contents

### Constructors

- [constructor](ShaderMaterial.md#constructor)

### Properties

- [\_activeEffect](ShaderMaterial.md#_activeeffect)
- [\_alpha](ShaderMaterial.md#_alpha)
- [\_backFaceCulling](ShaderMaterial.md#_backfaceculling)
- [\_cachedWorldViewMatrix](ShaderMaterial.md#_cachedworldviewmatrix)
- [\_cachedWorldViewProjectionMatrix](ShaderMaterial.md#_cachedworldviewprojectionmatrix)
- [\_colors3](ShaderMaterial.md#_colors3)
- [\_colors3Arrays](ShaderMaterial.md#_colors3arrays)
- [\_colors4](ShaderMaterial.md#_colors4)
- [\_colors4Arrays](ShaderMaterial.md#_colors4arrays)
- [\_cullBackFaces](ShaderMaterial.md#_cullbackfaces)
- [\_drawWrapper](ShaderMaterial.md#_drawwrapper)
- [\_eventInfo](ShaderMaterial.md#_eventinfo)
- [\_externalTextures](ShaderMaterial.md#_externaltextures)
- [\_floats](ShaderMaterial.md#_floats)
- [\_floatsArrays](ShaderMaterial.md#_floatsarrays)
- [\_forceAlphaTest](ShaderMaterial.md#_forcealphatest)
- [\_ints](ShaderMaterial.md#_ints)
- [\_matrices](ShaderMaterial.md#_matrices)
- [\_matrices2x2](ShaderMaterial.md#_matrices2x2)
- [\_matrices3x3](ShaderMaterial.md#_matrices3x3)
- [\_matrixArrays](ShaderMaterial.md#_matrixarrays)
- [\_multiview](ShaderMaterial.md#_multiview)
- [\_needToBindSceneUbo](ShaderMaterial.md#_needtobindsceneubo)
- [\_normalMatrix](ShaderMaterial.md#_normalmatrix)
- [\_onEffectCreatedObservable](ShaderMaterial.md#_oneffectcreatedobservable)
- [\_options](ShaderMaterial.md#_options)
- [\_quaternions](ShaderMaterial.md#_quaternions)
- [\_quaternionsArrays](ShaderMaterial.md#_quaternionsarrays)
- [\_shaderPath](ShaderMaterial.md#_shaderpath)
- [\_storageBuffers](ShaderMaterial.md#_storagebuffers)
- [\_textureArrays](ShaderMaterial.md#_texturearrays)
- [\_textureSamplers](ShaderMaterial.md#_texturesamplers)
- [\_textures](ShaderMaterial.md#_textures)
- [\_transparencyMode](ShaderMaterial.md#_transparencymode)
- [\_uniformBuffers](ShaderMaterial.md#_uniformbuffers)
- [\_vectors2](ShaderMaterial.md#_vectors2)
- [\_vectors2Arrays](ShaderMaterial.md#_vectors2arrays)
- [\_vectors3](ShaderMaterial.md#_vectors3)
- [\_vectors3Arrays](ShaderMaterial.md#_vectors3arrays)
- [\_vectors4](ShaderMaterial.md#_vectors4)
- [\_vectors4Arrays](ShaderMaterial.md#_vectors4arrays)
- [allowShaderHotSwapping](ShaderMaterial.md#allowshaderhotswapping)
- [animations](ShaderMaterial.md#animations)
- [checkReadyOnEveryCall](ShaderMaterial.md#checkreadyoneverycall)
- [checkReadyOnlyOnce](ShaderMaterial.md#checkreadyonlyonce)
- [customShaderNameResolve](ShaderMaterial.md#customshadernameresolve)
- [depthFunction](ShaderMaterial.md#depthfunction)
- [disableColorWrite](ShaderMaterial.md#disablecolorwrite)
- [disableDepthWrite](ShaderMaterial.md#disabledepthwrite)
- [doNotSerialize](ShaderMaterial.md#donotserialize)
- [forceDepthWrite](ShaderMaterial.md#forcedepthwrite)
- [getRenderTargetTextures](ShaderMaterial.md#getrendertargettextures)
- [id](ShaderMaterial.md#id)
- [inspectableCustomProperties](ShaderMaterial.md#inspectablecustomproperties)
- [metadata](ShaderMaterial.md#metadata)
- [name](ShaderMaterial.md#name)
- [onCompiled](ShaderMaterial.md#oncompiled)
- [onDisposeObservable](ShaderMaterial.md#ondisposeobservable)
- [onError](ShaderMaterial.md#onerror)
- [pluginManager](ShaderMaterial.md#pluginmanager)
- [pointSize](ShaderMaterial.md#pointsize)
- [reservedDataStore](ShaderMaterial.md#reserveddatastore)
- [separateCullingPass](ShaderMaterial.md#separatecullingpass)
- [shadowDepthWrapper](ShaderMaterial.md#shadowdepthwrapper)
- [sideOrientation](ShaderMaterial.md#sideorientation)
- [snippetId](ShaderMaterial.md#snippetid)
- [state](ShaderMaterial.md#state)
- [stencil](ShaderMaterial.md#stencil)
- [uniqueId](ShaderMaterial.md#uniqueid)
- [zOffset](ShaderMaterial.md#zoffset)
- [zOffsetUnits](ShaderMaterial.md#zoffsetunits)
- [AllDirtyFlag](ShaderMaterial.md#alldirtyflag)
- [AttributesDirtyFlag](ShaderMaterial.md#attributesdirtyflag)
- [ClockWiseSideOrientation](ShaderMaterial.md#clockwisesideorientation)
- [CounterClockWiseSideOrientation](ShaderMaterial.md#counterclockwisesideorientation)
- [CreateFromSnippetAsync](ShaderMaterial.md#createfromsnippetasync)
- [FresnelDirtyFlag](ShaderMaterial.md#fresneldirtyflag)
- [LightDirtyFlag](ShaderMaterial.md#lightdirtyflag)
- [LineListDrawMode](ShaderMaterial.md#linelistdrawmode)
- [LineLoopDrawMode](ShaderMaterial.md#lineloopdrawmode)
- [LineStripDrawMode](ShaderMaterial.md#linestripdrawmode)
- [MATERIAL\_ALPHABLEND](ShaderMaterial.md#material_alphablend)
- [MATERIAL\_ALPHATEST](ShaderMaterial.md#material_alphatest)
- [MATERIAL\_ALPHATESTANDBLEND](ShaderMaterial.md#material_alphatestandblend)
- [MATERIAL\_NORMALBLENDMETHOD\_RNM](ShaderMaterial.md#material_normalblendmethod_rnm)
- [MATERIAL\_NORMALBLENDMETHOD\_WHITEOUT](ShaderMaterial.md#material_normalblendmethod_whiteout)
- [MATERIAL\_OPAQUE](ShaderMaterial.md#material_opaque)
- [MiscDirtyFlag](ShaderMaterial.md#miscdirtyflag)
- [OnEventObservable](ShaderMaterial.md#oneventobservable)
- [PointFillMode](ShaderMaterial.md#pointfillmode)
- [PointListDrawMode](ShaderMaterial.md#pointlistdrawmode)
- [PrePassDirtyFlag](ShaderMaterial.md#prepassdirtyflag)
- [SnippetUrl](ShaderMaterial.md#snippeturl)
- [TextureDirtyFlag](ShaderMaterial.md#texturedirtyflag)
- [TriangleFanDrawMode](ShaderMaterial.md#trianglefandrawmode)
- [TriangleFillMode](ShaderMaterial.md#trianglefillmode)
- [TriangleStripDrawMode](ShaderMaterial.md#trianglestripdrawmode)
- [WireFrameFillMode](ShaderMaterial.md#wireframefillmode)

### Accessors

- [\_disableAlphaBlending](ShaderMaterial.md#_disablealphablending)
- [alpha](ShaderMaterial.md#alpha)
- [alphaMode](ShaderMaterial.md#alphamode)
- [backFaceCulling](ShaderMaterial.md#backfaceculling)
- [canRenderToMRT](ShaderMaterial.md#canrendertomrt)
- [cullBackFaces](ShaderMaterial.md#cullbackfaces)
- [fillMode](ShaderMaterial.md#fillmode)
- [fogEnabled](ShaderMaterial.md#fogenabled)
- [hasRenderTargetTextures](ShaderMaterial.md#hasrendertargettextures)
- [isFrozen](ShaderMaterial.md#isfrozen)
- [isPrePassCapable](ShaderMaterial.md#isprepasscapable)
- [needDepthPrePass](ShaderMaterial.md#needdepthprepass)
- [onBind](ShaderMaterial.md#onbind)
- [onBindObservable](ShaderMaterial.md#onbindobservable)
- [onDispose](ShaderMaterial.md#ondispose)
- [onEffectCreatedObservable](ShaderMaterial.md#oneffectcreatedobservable)
- [onUnBindObservable](ShaderMaterial.md#onunbindobservable)
- [options](ShaderMaterial.md#options)
- [pointsCloud](ShaderMaterial.md#pointscloud)
- [shaderPath](ShaderMaterial.md#shaderpath)
- [transparencyMode](ShaderMaterial.md#transparencymode)
- [wireframe](ShaderMaterial.md#wireframe)

### Methods

- [\_afterBind](ShaderMaterial.md#_afterbind)
- [\_checkUniform](ShaderMaterial.md#_checkuniform)
- [\_isReadyForSubMesh](ShaderMaterial.md#_isreadyforsubmesh)
- [\_markAllSubMeshesAsAllDirty](ShaderMaterial.md#_markallsubmeshesasalldirty)
- [\_markAllSubMeshesAsAttributesDirty](ShaderMaterial.md#_markallsubmeshesasattributesdirty)
- [\_markAllSubMeshesAsDirty](ShaderMaterial.md#_markallsubmeshesasdirty)
- [\_markAllSubMeshesAsFresnelAndMiscDirty](ShaderMaterial.md#_markallsubmeshesasfresnelandmiscdirty)
- [\_markAllSubMeshesAsFresnelDirty](ShaderMaterial.md#_markallsubmeshesasfresneldirty)
- [\_markAllSubMeshesAsImageProcessingDirty](ShaderMaterial.md#_markallsubmeshesasimageprocessingdirty)
- [\_markAllSubMeshesAsLightsDirty](ShaderMaterial.md#_markallsubmeshesaslightsdirty)
- [\_markAllSubMeshesAsMiscDirty](ShaderMaterial.md#_markallsubmeshesasmiscdirty)
- [\_markAllSubMeshesAsPrePassDirty](ShaderMaterial.md#_markallsubmeshesasprepassdirty)
- [\_markAllSubMeshesAsTexturesAndMiscDirty](ShaderMaterial.md#_markallsubmeshesastexturesandmiscdirty)
- [\_markAllSubMeshesAsTexturesDirty](ShaderMaterial.md#_markallsubmeshesastexturesdirty)
- [\_markScenePrePassDirty](ShaderMaterial.md#_marksceneprepassdirty)
- [\_mustRebind](ShaderMaterial.md#_mustrebind)
- [\_shouldTurnAlphaTestOn](ShaderMaterial.md#_shouldturnalphateston)
- [bind](ShaderMaterial.md#bind)
- [bindEyePosition](ShaderMaterial.md#bindeyeposition)
- [bindForSubMesh](ShaderMaterial.md#bindforsubmesh)
- [bindOnlyNormalMatrix](ShaderMaterial.md#bindonlynormalmatrix)
- [bindOnlyWorldMatrix](ShaderMaterial.md#bindonlyworldmatrix)
- [bindView](ShaderMaterial.md#bindview)
- [bindViewProjection](ShaderMaterial.md#bindviewprojection)
- [buildUniformLayout](ShaderMaterial.md#builduniformlayout)
- [clone](ShaderMaterial.md#clone)
- [dispose](ShaderMaterial.md#dispose)
- [forceCompilation](ShaderMaterial.md#forcecompilation)
- [forceCompilationAsync](ShaderMaterial.md#forcecompilationasync)
- [freeze](ShaderMaterial.md#freeze)
- [getActiveTextures](ShaderMaterial.md#getactivetextures)
- [getAlphaTestTexture](ShaderMaterial.md#getalphatesttexture)
- [getAnimatables](ShaderMaterial.md#getanimatables)
- [getBindedMeshes](ShaderMaterial.md#getbindedmeshes)
- [getClassName](ShaderMaterial.md#getclassname)
- [getEffect](ShaderMaterial.md#geteffect)
- [getScene](ShaderMaterial.md#getscene)
- [hasTexture](ShaderMaterial.md#hastexture)
- [isReady](ShaderMaterial.md#isready)
- [isReadyForSubMesh](ShaderMaterial.md#isreadyforsubmesh)
- [markAsDirty](ShaderMaterial.md#markasdirty)
- [markDirty](ShaderMaterial.md#markdirty)
- [needAlphaBlending](ShaderMaterial.md#needalphablending)
- [needAlphaBlendingForMesh](ShaderMaterial.md#needalphablendingformesh)
- [needAlphaTesting](ShaderMaterial.md#needalphatesting)
- [resetDrawCache](ShaderMaterial.md#resetdrawcache)
- [serialize](ShaderMaterial.md#serialize)
- [setArray2](ShaderMaterial.md#setarray2)
- [setArray3](ShaderMaterial.md#setarray3)
- [setArray4](ShaderMaterial.md#setarray4)
- [setColor3](ShaderMaterial.md#setcolor3)
- [setColor3Array](ShaderMaterial.md#setcolor3array)
- [setColor4](ShaderMaterial.md#setcolor4)
- [setColor4Array](ShaderMaterial.md#setcolor4array)
- [setExternalTexture](ShaderMaterial.md#setexternaltexture)
- [setFloat](ShaderMaterial.md#setfloat)
- [setFloats](ShaderMaterial.md#setfloats)
- [setInt](ShaderMaterial.md#setint)
- [setMatrices](ShaderMaterial.md#setmatrices)
- [setMatrix](ShaderMaterial.md#setmatrix)
- [setMatrix2x2](ShaderMaterial.md#setmatrix2x2)
- [setMatrix3x3](ShaderMaterial.md#setmatrix3x3)
- [setPrePassRenderer](ShaderMaterial.md#setprepassrenderer)
- [setQuaternion](ShaderMaterial.md#setquaternion)
- [setQuaternionArray](ShaderMaterial.md#setquaternionarray)
- [setStorageBuffer](ShaderMaterial.md#setstoragebuffer)
- [setTexture](ShaderMaterial.md#settexture)
- [setTextureArray](ShaderMaterial.md#settexturearray)
- [setTextureSampler](ShaderMaterial.md#settexturesampler)
- [setUniformBuffer](ShaderMaterial.md#setuniformbuffer)
- [setVector2](ShaderMaterial.md#setvector2)
- [setVector3](ShaderMaterial.md#setvector3)
- [setVector4](ShaderMaterial.md#setvector4)
- [toString](ShaderMaterial.md#tostring)
- [unbind](ShaderMaterial.md#unbind)
- [unfreeze](ShaderMaterial.md#unfreeze)
- [Parse](ShaderMaterial.md#parse)
- [ParseFromFileAsync](ShaderMaterial.md#parsefromfileasync)
- [ParseFromSnippetAsync](ShaderMaterial.md#parsefromsnippetasync)

## Constructors

### constructor

• **new ShaderMaterial**(`name`, `scene`, `shaderPath`, `options?`, `storeEffectOnSubMeshes?`)

Instantiate a new shader material.
The ShaderMaterial object has the necessary methods to pass data from your scene to the Vertex and Fragment Shaders and returns a material that can be applied to any mesh.
This returned material effects how the mesh will look based on the code in the shaders.

**`See`**

https://doc.babylonjs.com/how_to/shader_material

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | Define the name of the material in the scene |
| `scene` | [`Scene`](Scene.md) | `undefined` | Define the scene the material belongs to |
| `shaderPath` | `any` | `undefined` | Defines  the route to the shader code in one of three ways:   * object: { vertex: "custom", fragment: "custom" }, used with Effect.ShadersStore["customVertexShader"] and Effect.ShadersStore["customFragmentShader"]   * object: { vertexElement: "vertexShaderCode", fragmentElement: "fragmentShaderCode" }, used with shader code in script tags   * object: { vertexSource: "vertex shader code string", fragmentSource: "fragment shader code string" } using with strings containing the shaders code   * string: "./COMMON_NAME", used with external files COMMON_NAME.vertex.fx and COMMON_NAME.fragment.fx in index.html folder. |
| `options` | `Partial`[`IShaderMaterialOptions`](../interfaces/IShaderMaterialOptions.md) | `{}` | Define the options used to create the shader |
| `storeEffectOnSubMeshes` | `boolean` | `true` | true to store effect on submeshes, false to store the effect directly in the material class. |

#### Overrides

PushMaterial.constructor

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:154

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

### \_backFaceCulling

• `Protected` **\_backFaceCulling**: `boolean` = `true`

Specifies if back face culling is enabled

#### Inherited from

PushMaterial.\_backFaceCulling

#### Defined in

packages/dev/core/src/Materials/material.ts:328

___

### \_cachedWorldViewMatrix

• `Private` **\_cachedWorldViewMatrix**: [`Matrix`](Matrix.md)

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:129

___

### \_cachedWorldViewProjectionMatrix

• `Private` **\_cachedWorldViewProjectionMatrix**: [`Matrix`](Matrix.md)

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:130

___

### \_colors3

• `Private` **\_colors3**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: [`Color3`](Color3.md)

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:110

___

### \_colors3Arrays

• `Private` **\_colors3Arrays**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: `number`[]

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:111

___

### \_colors4

• `Private` **\_colors4**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: [`Color4`](Color4.md)

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:112

___

### \_colors4Arrays

• `Private` **\_colors4Arrays**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: `number`[]

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:113

___

### \_cullBackFaces

• `Protected` **\_cullBackFaces**: `boolean` = `true`

Specifies if back or front faces should be culled (when culling is enabled)

#### Inherited from

PushMaterial.\_cullBackFaces

#### Defined in

packages/dev/core/src/Materials/material.ts:352

___

### \_drawWrapper

• `Protected` **\_drawWrapper**: `DrawWrapper`

#### Inherited from

PushMaterial.\_drawWrapper

#### Defined in

packages/dev/core/src/Materials/material.ts:705

___

### \_eventInfo

• `Protected` **\_eventInfo**: `MaterialPluginDisposed` & `MaterialPluginHasTexture` & `MaterialPluginIsReadyForSubMesh` & `MaterialPluginGetDefineNames` & `MaterialPluginPrepareEffect` & `MaterialPluginPrepareDefines` & `MaterialPluginPrepareUniformBuffer` & `MaterialPluginBindForSubMesh` & `MaterialPluginGetAnimatables` & `MaterialPluginGetActiveTextures` & `MaterialPluginFillRenderTargetTextures` & `MaterialPluginHasRenderTargetTextures` & `MaterialPluginHardBindForSubMesh`

#### Inherited from

PushMaterial.\_eventInfo

#### Defined in

packages/dev/core/src/Materials/material.ts:770

___

### \_externalTextures

• `Private` **\_externalTextures**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: `ExternalTexture`

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:106

___

### \_floats

• `Private` **\_floats**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: `number`

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:107

___

### \_floatsArrays

• `Private` **\_floatsArrays**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: `number`[]

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:109

___

### \_forceAlphaTest

• `Protected` **\_forceAlphaTest**: `boolean` = `false`

Enforces alpha test in opaque or blend mode in order to improve the performances of some situations.

#### Inherited from

PushMaterial.\_forceAlphaTest

#### Defined in

packages/dev/core/src/Materials/material.ts:954

___

### \_ints

• `Private` **\_ints**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: `number`

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:108

___

### \_matrices

• `Private` **\_matrices**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: [`Matrix`](Matrix.md)

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:119

___

### \_matrices2x2

• `Private` **\_matrices2x2**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: `Float32Array` \| `number`[]

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:122

___

### \_matrices3x3

• `Private` **\_matrices3x3**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: `Float32Array` \| `number`[]

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:121

___

### \_matrixArrays

• `Private` **\_matrixArrays**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: `Float32Array` \| `number`[]

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:120

___

### \_multiview

• `Private` **\_multiview**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:131

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

### \_options

• `Private` **\_options**: [`IShaderMaterialOptions`](../interfaces/IShaderMaterialOptions.md)

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:103

___

### \_quaternions

• `Private` **\_quaternions**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: [`Quaternion`](Quaternion.md)

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:117

___

### \_quaternionsArrays

• `Private` **\_quaternionsArrays**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: `number`[]

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:118

___

### \_shaderPath

• `Private` **\_shaderPath**: `any`

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:102

___

### \_storageBuffers

• `Private` **\_storageBuffers**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: [`StorageBuffer`](StorageBuffer.md)

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:128

___

### \_textureArrays

• `Private` **\_textureArrays**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: [`BaseTexture`](BaseTexture.md)[]

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:105

___

### \_textureSamplers

• `Private` **\_textureSamplers**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: [`TextureSampler`](TextureSampler.md)

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:127

___

### \_textures

• `Private` **\_textures**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: [`BaseTexture`](BaseTexture.md)

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:104

___

### \_transparencyMode

• `Protected` **\_transparencyMode**: [`Nullable`](../modules.md#nullable)`number` = `null`

The transparency mode of the material.

#### Inherited from

PushMaterial.\_transparencyMode

#### Defined in

packages/dev/core/src/Materials/material.ts:959

___

### \_uniformBuffers

• `Private` **\_uniformBuffers**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: [`UniformBuffer`](UniformBuffer.md)

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:126

___

### \_vectors2

• `Private` **\_vectors2**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: [`Vector2`](Vector2.md)

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:114

___

### \_vectors2Arrays

• `Private` **\_vectors2Arrays**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: `number`[]

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:123

___

### \_vectors3

• `Private` **\_vectors3**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:115

___

### \_vectors3Arrays

• `Private` **\_vectors3Arrays**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: `number`[]

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:124

___

### \_vectors4

• `Private` **\_vectors4**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: [`Vector4`](Vector4.md)

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:116

___

### \_vectors4Arrays

• `Private` **\_vectors4Arrays**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: `number`[]

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:125

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

### reservedDataStore

• **reservedDataStore**: `any` = `null`

For internal use only. Please do not use.

#### Inherited from

PushMaterial.reservedDataStore

#### Defined in

packages/dev/core/src/Materials/material.ts:259

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

### snippetId

• **snippetId**: `string`

Snippet ID if the material was created from the snippet server

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:137

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

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the material

#### Inherited from

PushMaterial.uniqueId

#### Defined in

packages/dev/core/src/Materials/material.ts:239

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

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:1765

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

### SnippetUrl

▪ `Static` **SnippetUrl**: `string` = `Constants.SnippetUrl`

Define the Url to load snippets

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:134

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

### hasRenderTargetTextures

• `get` **hasRenderTargetTextures**(): `boolean`

Gets a boolean indicating that current material needs to register RTT

#### Returns

`boolean`

#### Inherited from

PushMaterial.hasRenderTargetTextures

#### Defined in

packages/dev/core/src/Materials/material.ts:396

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

### options

• `get` **options**(): [`IShaderMaterialOptions`](../interfaces/IShaderMaterialOptions.md)

Gets the options used to compile the shader.
They can be modified to trigger a new compilation

#### Returns

[`IShaderMaterialOptions`](../interfaces/IShaderMaterialOptions.md)

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:194

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

### shaderPath

• `get` **shaderPath**(): `any`

Gets the shader path used to define the shader code
It can be modified to trigger a new compilation

#### Returns

`any`

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:178

• `set` **shaderPath**(`shaderPath`): `void`

Sets the shader path used to define the shader code
It can be modified to trigger a new compilation

#### Parameters

| Name | Type |
| :------ | :------ |
| `shaderPath` | `any` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:186

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

### \_checkUniform

▸ `Private` **_checkUniform**(`uniformName`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `uniformName` | `string` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:223

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

#### Overrides

PushMaterial.bind

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:942

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

packages/dev/core/src/Materials/shaderMaterial.ts:931

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

▸ **bindOnlyWorldMatrix**(`world`, `effectOverride?`): `void`

Binds the world matrix to the material

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `world` | [`Matrix`](Matrix.md) | defines the world transformation matrix |
| `effectOverride?` | [`Nullable`](../modules.md#nullable)[`Effect`](Effect.md) | If provided, use this effect instead of internal effect |

#### Returns

`void`

#### Overrides

PushMaterial.bindOnlyWorldMatrix

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:901

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

Initializes the uniform buffer layout for the shader.

#### Returns

`void`

#### Inherited from

PushMaterial.buildUniformLayout

#### Defined in

packages/dev/core/src/Materials/material.ts:1104

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

#### Overrides

PushMaterial.clone

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:1208

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

packages/dev/core/src/Materials/shaderMaterial.ts:1366

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

packages/dev/core/src/Materials/shaderMaterial.ts:1158

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

Gets the current class name of the material e.g. "ShaderMaterial"
Mainly use in serialization.

#### Returns

`string`

the class name

#### Overrides

PushMaterial.getClassName

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:203

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

packages/dev/core/src/Materials/shaderMaterial.ts:1180

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

#### Overrides

PushMaterial.isReady

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:602

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

#### Overrides

PushMaterial.isReadyForSubMesh

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:591

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

packages/dev/core/src/Materials/shaderMaterial.ts:211

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

packages/dev/core/src/Materials/shaderMaterial.ts:219

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

Serializes this material in a JSON representation

#### Returns

`any`

the serialized material object

#### Overrides

PushMaterial.serialize

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:1390

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

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:506

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

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:519

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

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:532

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

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:322

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

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:335

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

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:350

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

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:363

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

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:268

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

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:283

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

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:309

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

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:296

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

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:458

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

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:445

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

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:493

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

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:480

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

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:417

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

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:430

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

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:575

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

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:235

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

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:250

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

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:560

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

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:545

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

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:378

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

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:391

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

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:404

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

#### Overrides

PushMaterial.Parse

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:1544

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

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:1701

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

#### Defined in

packages/dev/core/src/Materials/shaderMaterial.ts:1733
