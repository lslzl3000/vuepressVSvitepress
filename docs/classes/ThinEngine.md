[@dev/core](../README.md) / [Exports](../modules.md) / ThinEngine

# Class: ThinEngine

The base engine class (root of all engines)

## Hierarchy

- **`ThinEngine`**

  ↳ [`Engine`](Engine.md)

## Table of contents

### Constructors

- [constructor](ThinEngine.md#constructor)

### Properties

- [\_activeRenderLoops](ThinEngine.md#_activerenderloops)
- [\_activeRequests](ThinEngine.md#_activerequests)
- [\_audioContext](ThinEngine.md#_audiocontext)
- [\_audioDestination](ThinEngine.md#_audiodestination)
- [\_boundUniforms](ThinEngine.md#_bounduniforms)
- [\_cachedVertexArrayObject](ThinEngine.md#_cachedvertexarrayobject)
- [\_checkForMobile](ThinEngine.md#_checkformobile)
- [\_compiledEffects](ThinEngine.md#_compiledeffects)
- [\_contextWasLost](ThinEngine.md#_contextwaslost)
- [\_creationOptions](ThinEngine.md#_creationoptions)
- [\_currentBoundBuffer](ThinEngine.md#_currentboundbuffer)
- [\_currentBufferPointers](ThinEngine.md#_currentbufferpointers)
- [\_currentEffect](ThinEngine.md#_currenteffect)
- [\_currentInstanceBuffers](ThinEngine.md#_currentinstancebuffers)
- [\_currentInstanceLocations](ThinEngine.md#_currentinstancelocations)
- [\_currentTextureChannel](ThinEngine.md#_currenttexturechannel)
- [\_emptyCubeTexture](ThinEngine.md#_emptycubetexture)
- [\_emptyTexture](ThinEngine.md#_emptytexture)
- [\_emptyTexture2DArray](ThinEngine.md#_emptytexture2darray)
- [\_emptyTexture3D](ThinEngine.md#_emptytexture3d)
- [\_frameId](ThinEngine.md#_frameid)
- [\_framebufferDimensionsObject](ThinEngine.md#_framebufferdimensionsobject)
- [\_glRenderer](ThinEngine.md#_glrenderer)
- [\_glVendor](ThinEngine.md#_glvendor)
- [\_glVersion](ThinEngine.md#_glversion)
- [\_highPrecisionShadersAllowed](ThinEngine.md#_highprecisionshadersallowed)
- [\_isStencilEnable](ThinEngine.md#_isstencilenable)
- [\_maxMSAASamplesOverride](ThinEngine.md#_maxmsaasamplesoverride)
- [\_maxSimultaneousTextures](ThinEngine.md#_maxsimultaneoustextures)
- [\_mustWipeVertexAttributes](ThinEngine.md#_mustwipevertexattributes)
- [\_nextFreeTextureSlots](ThinEngine.md#_nextfreetextureslots)
- [\_onContextLost](ThinEngine.md#_oncontextlost)
- [\_onContextRestored](ThinEngine.md#_oncontextrestored)
- [\_renderingCanvas](ThinEngine.md#_renderingcanvas)
- [\_renderingQueueLaunched](ThinEngine.md#_renderingqueuelaunched)
- [\_shaderProcessor](ThinEngine.md#_shaderprocessor)
- [\_snapshotRenderingMode](ThinEngine.md#_snapshotrenderingmode)
- [\_textureUnits](ThinEngine.md#_textureunits)
- [\_uintIndicesCurrentlySet](ThinEngine.md#_uintindicescurrentlyset)
- [\_unpackFlipYCached](ThinEngine.md#_unpackflipycached)
- [\_useExactSrgbConversions](ThinEngine.md#_useexactsrgbconversions)
- [\_useReverseDepthBuffer](ThinEngine.md#_usereversedepthbuffer)
- [\_vaoRecordInProgress](ThinEngine.md#_vaorecordinprogress)
- [\_vertexAttribArraysEnabled](ThinEngine.md#_vertexattribarraysenabled)
- [\_viewportCached](ThinEngine.md#_viewportcached)
- [\_windowIsBackground](ThinEngine.md#_windowisbackground)
- [adaptToDeviceRatio](ThinEngine.md#adapttodeviceratio)
- [cullBackFaces](ThinEngine.md#cullbackfaces)
- [disableUniformBuffers](ThinEngine.md#disableuniformbuffers)
- [disableVertexArrayObjects](ThinEngine.md#disablevertexarrayobjects)
- [enableUnpackFlipYCached](ThinEngine.md#enableunpackflipycached)
- [forcePOTTextures](ThinEngine.md#forcepottextures)
- [hasOriginBottomLeft](ThinEngine.md#hasoriginbottomleft)
- [hostInformation](ThinEngine.md#hostinformation)
- [isFullscreen](ThinEngine.md#isfullscreen)
- [isNDCHalfZRange](ThinEngine.md#isndchalfzrange)
- [onBeforeTextureInitObservable](ThinEngine.md#onbeforetextureinitobservable)
- [onContextLostObservable](ThinEngine.md#oncontextlostobservable)
- [onContextRestoredObservable](ThinEngine.md#oncontextrestoredobservable)
- [onDisposeObservable](ThinEngine.md#ondisposeobservable)
- [premultipliedAlpha](ThinEngine.md#premultipliedalpha)
- [preventCacheWipeBetweenFrames](ThinEngine.md#preventcachewipebetweenframes)
- [renderEvenInBackground](ThinEngine.md#rendereveninbackground)
- [validateShaderPrograms](ThinEngine.md#validateshaderprograms)
- [CollisionsEpsilon](ThinEngine.md#collisionsepsilon)
- [ExceptionList](ThinEngine.md#exceptionlist)
- [\_HasMajorPerformanceCaveat](ThinEngine.md#_hasmajorperformancecaveat)
- [\_IsSupported](ThinEngine.md#_issupported)

### Accessors

- [\_supportsHardwareTextureRescaling](ThinEngine.md#_supportshardwaretexturerescaling)
- [activeRenderLoops](ThinEngine.md#activerenderloops)
- [alphaState](ThinEngine.md#alphastate)
- [currentViewport](ThinEngine.md#currentviewport)
- [depthCullingState](ThinEngine.md#depthcullingstate)
- [description](ThinEngine.md#description)
- [doNotHandleContextLost](ThinEngine.md#donothandlecontextlost)
- [emptyCubeTexture](ThinEngine.md#emptycubetexture)
- [emptyTexture](ThinEngine.md#emptytexture)
- [emptyTexture2DArray](ThinEngine.md#emptytexture2darray)
- [emptyTexture3D](ThinEngine.md#emptytexture3d)
- [frameId](ThinEngine.md#frameid)
- [framebufferDimensionsObject](ThinEngine.md#framebufferdimensionsobject)
- [isStencilEnable](ThinEngine.md#isstencilenable)
- [isWebGPU](ThinEngine.md#iswebgpu)
- [name](ThinEngine.md#name)
- [needPOTTextures](ThinEngine.md#needpottextures)
- [shaderPlatformName](ThinEngine.md#shaderplatformname)
- [snapshotRendering](ThinEngine.md#snapshotrendering)
- [snapshotRenderingMode](ThinEngine.md#snapshotrenderingmode)
- [stencilState](ThinEngine.md#stencilstate)
- [stencilStateComposer](ThinEngine.md#stencilstatecomposer)
- [supportsUniformBuffers](ThinEngine.md#supportsuniformbuffers)
- [useExactSrgbConversions](ThinEngine.md#useexactsrgbconversions)
- [useReverseDepthBuffer](ThinEngine.md#usereversedepthbuffer)
- [version](ThinEngine.md#version)
- [webGLVersion](ThinEngine.md#webglversion)
- [HasMajorPerformanceCaveat](ThinEngine.md#hasmajorperformancecaveat)
- [IsSupported](ThinEngine.md#issupported)
- [IsSupportedAsync](ThinEngine.md#issupportedasync)
- [NpmPackage](ThinEngine.md#npmpackage)
- [ShadersRepository](ThinEngine.md#shadersrepository)
- [Version](ThinEngine.md#version-1)

### Methods

- [\_activateCurrentTexture](ThinEngine.md#_activatecurrenttexture)
- [\_bindBuffer](ThinEngine.md#_bindbuffer)
- [\_bindSamplerUniformToChannel](ThinEngine.md#_bindsampleruniformtochannel)
- [\_bindVertexBuffersAttributes](ThinEngine.md#_bindvertexbuffersattributes)
- [\_canRenderToFloatFramebuffer](ThinEngine.md#_canrendertofloatframebuffer)
- [\_canRenderToFramebuffer](ThinEngine.md#_canrendertoframebuffer)
- [\_canRenderToHalfFloatFramebuffer](ThinEngine.md#_canrendertohalffloatframebuffer)
- [\_compileRawShader](ThinEngine.md#_compilerawshader)
- [\_compileShader](ThinEngine.md#_compileshader)
- [\_createDepthStencilCubeTexture](ThinEngine.md#_createdepthstencilcubetexture)
- [\_createShaderProgram](ThinEngine.md#_createshaderprogram)
- [\_createTextureBase](ThinEngine.md#_createtexturebase)
- [\_createVertexBuffer](ThinEngine.md#_createvertexbuffer)
- [\_deleteBuffer](ThinEngine.md#_deletebuffer)
- [\_deleteTexture](ThinEngine.md#_deletetexture)
- [\_drawMode](ThinEngine.md#_drawmode)
- [\_finalizePipelineContext](ThinEngine.md#_finalizepipelinecontext)
- [\_getTextureTarget](ThinEngine.md#_gettexturetarget)
- [\_getTextureWrapMode](ThinEngine.md#_gettexturewrapmode)
- [\_initFeatures](ThinEngine.md#_initfeatures)
- [\_initGLContext](ThinEngine.md#_initglcontext)
- [\_normalizeIndexData](ThinEngine.md#_normalizeindexdata)
- [\_prepareWebGLTexture](ThinEngine.md#_preparewebgltexture)
- [\_prepareWebGLTextureContinuation](ThinEngine.md#_preparewebgltexturecontinuation)
- [\_rebuildBuffers](ThinEngine.md#_rebuildbuffers)
- [\_rebuildEffects](ThinEngine.md#_rebuildeffects)
- [\_rebuildInternalTextures](ThinEngine.md#_rebuildinternaltextures)
- [\_rebuildRenderTargetWrappers](ThinEngine.md#_rebuildrendertargetwrappers)
- [\_resetIndexBufferBinding](ThinEngine.md#_resetindexbufferbinding)
- [\_restoreEngineAfterContextLost](ThinEngine.md#_restoreengineaftercontextlost)
- [\_setProgram](ThinEngine.md#_setprogram)
- [\_setTexture](ThinEngine.md#_settexture)
- [\_setTextureParameterFloat](ThinEngine.md#_settextureparameterfloat)
- [\_setTextureParameterInteger](ThinEngine.md#_settextureparameterinteger)
- [\_sharedInit](ThinEngine.md#_sharedinit)
- [\_unbindVertexArrayObject](ThinEngine.md#_unbindvertexarrayobject)
- [\_vertexAttribPointer](ThinEngine.md#_vertexattribpointer)
- [applyStates](ThinEngine.md#applystates)
- [areAllComputeEffectsReady](ThinEngine.md#areallcomputeeffectsready)
- [areAllEffectsReady](ThinEngine.md#arealleffectsready)
- [attachContextLostEvent](ThinEngine.md#attachcontextlostevent)
- [attachContextRestoredEvent](ThinEngine.md#attachcontextrestoredevent)
- [beginFrame](ThinEngine.md#beginframe)
- [bindArrayBuffer](ThinEngine.md#bindarraybuffer)
- [bindAttachments](ThinEngine.md#bindattachments)
- [bindBuffers](ThinEngine.md#bindbuffers)
- [bindBuffersDirectly](ThinEngine.md#bindbuffersdirectly)
- [bindFramebuffer](ThinEngine.md#bindframebuffer)
- [bindIndexBuffer](ThinEngine.md#bindindexbuffer)
- [bindInstancesBuffer](ThinEngine.md#bindinstancesbuffer)
- [bindSamplers](ThinEngine.md#bindsamplers)
- [bindUniformBlock](ThinEngine.md#binduniformblock)
- [bindUniformBuffer](ThinEngine.md#binduniformbuffer)
- [bindUniformBufferBase](ThinEngine.md#binduniformbufferbase)
- [bindVertexArrayObject](ThinEngine.md#bindvertexarrayobject)
- [buildTextureLayout](ThinEngine.md#buildtexturelayout)
- [clear](ThinEngine.md#clear)
- [clearInternalTexturesCache](ThinEngine.md#clearinternaltexturescache)
- [computeDispatch](ThinEngine.md#computedispatch)
- [createCanvas](ThinEngine.md#createcanvas)
- [createCanvasImage](ThinEngine.md#createcanvasimage)
- [createComputeContext](ThinEngine.md#createcomputecontext)
- [createComputeEffect](ThinEngine.md#createcomputeeffect)
- [createComputePipelineContext](ThinEngine.md#createcomputepipelinecontext)
- [createCubeTexture](ThinEngine.md#createcubetexture)
- [createDepthStencilTexture](ThinEngine.md#createdepthstenciltexture)
- [createDrawContext](ThinEngine.md#createdrawcontext)
- [createDynamicTexture](ThinEngine.md#createdynamictexture)
- [createDynamicUniformBuffer](ThinEngine.md#createdynamicuniformbuffer)
- [createDynamicVertexBuffer](ThinEngine.md#createdynamicvertexbuffer)
- [createEffect](ThinEngine.md#createeffect)
- [createExternalTexture](ThinEngine.md#createexternaltexture)
- [createIndexBuffer](ThinEngine.md#createindexbuffer)
- [createMaterialContext](ThinEngine.md#creatematerialcontext)
- [createMultipleRenderTarget](ThinEngine.md#createmultiplerendertarget)
- [createPipelineContext](ThinEngine.md#createpipelinecontext)
- [createPrefilteredCubeTexture](ThinEngine.md#createprefilteredcubetexture)
- [createRawCubeTexture](ThinEngine.md#createrawcubetexture)
- [createRawCubeTextureFromUrl](ThinEngine.md#createrawcubetexturefromurl)
- [createRawShaderProgram](ThinEngine.md#createrawshaderprogram)
- [createRawTexture](ThinEngine.md#createrawtexture)
- [createRawTexture2DArray](ThinEngine.md#createrawtexture2darray)
- [createRawTexture3D](ThinEngine.md#createrawtexture3d)
- [createRenderTargetCubeTexture](ThinEngine.md#createrendertargetcubetexture)
- [createRenderTargetTexture](ThinEngine.md#createrendertargettexture)
- [createShaderProgram](ThinEngine.md#createshaderprogram)
- [createStorageBuffer](ThinEngine.md#createstoragebuffer)
- [createTexture](ThinEngine.md#createtexture)
- [createUniformBuffer](ThinEngine.md#createuniformbuffer)
- [createVertexBuffer](ThinEngine.md#createvertexbuffer)
- [disableAttributeByIndex](ThinEngine.md#disableattributebyindex)
- [disableInstanceAttribute](ThinEngine.md#disableinstanceattribute)
- [disableInstanceAttributeByName](ThinEngine.md#disableinstanceattributebyname)
- [dispose](ThinEngine.md#dispose)
- [draw](ThinEngine.md#draw)
- [drawArraysType](ThinEngine.md#drawarraystype)
- [drawElementsType](ThinEngine.md#drawelementstype)
- [drawPointClouds](ThinEngine.md#drawpointclouds)
- [drawUnIndexed](ThinEngine.md#drawunindexed)
- [enableEffect](ThinEngine.md#enableeffect)
- [endFrame](ThinEngine.md#endframe)
- [flushFramebuffer](ThinEngine.md#flushframebuffer)
- [generateMipmaps](ThinEngine.md#generatemipmaps)
- [getAlphaEquation](ThinEngine.md#getalphaequation)
- [getAlphaMode](ThinEngine.md#getalphamode)
- [getAttributes](ThinEngine.md#getattributes)
- [getAudioContext](ThinEngine.md#getaudiocontext)
- [getAudioDestination](ThinEngine.md#getaudiodestination)
- [getCaps](ThinEngine.md#getcaps)
- [getClassName](ThinEngine.md#getclassname)
- [getColorWrite](ThinEngine.md#getcolorwrite)
- [getCreationOptions](ThinEngine.md#getcreationoptions)
- [getDepthBuffer](ThinEngine.md#getdepthbuffer)
- [getError](ThinEngine.md#geterror)
- [getGlInfo](ThinEngine.md#getglinfo)
- [getHardwareScalingLevel](ThinEngine.md#gethardwarescalinglevel)
- [getHostDocument](ThinEngine.md#gethostdocument)
- [getHostWindow](ThinEngine.md#gethostwindow)
- [getInfo](ThinEngine.md#getinfo)
- [getLoadedTexturesCache](ThinEngine.md#getloadedtexturescache)
- [getRenderHeight](ThinEngine.md#getrenderheight)
- [getRenderWidth](ThinEngine.md#getrenderwidth)
- [getRenderingCanvas](ThinEngine.md#getrenderingcanvas)
- [getUniforms](ThinEngine.md#getuniforms)
- [getZOffset](ThinEngine.md#getzoffset)
- [getZOffsetUnits](ThinEngine.md#getzoffsetunits)
- [inlineShaderCode](ThinEngine.md#inlineshadercode)
- [readFromStorageBuffer](ThinEngine.md#readfromstoragebuffer)
- [readPixels](ThinEngine.md#readpixels)
- [recordVertexArrayObject](ThinEngine.md#recordvertexarrayobject)
- [releaseComputeEffects](ThinEngine.md#releasecomputeeffects)
- [releaseEffects](ThinEngine.md#releaseeffects)
- [releaseVertexArrayObject](ThinEngine.md#releasevertexarrayobject)
- [resetTextureCache](ThinEngine.md#resettexturecache)
- [resize](ThinEngine.md#resize)
- [restoreDefaultFramebuffer](ThinEngine.md#restoredefaultframebuffer)
- [restoreSingleAttachment](ThinEngine.md#restoresingleattachment)
- [restoreSingleAttachmentForRenderTarget](ThinEngine.md#restoresingleattachmentforrendertarget)
- [runRenderLoop](ThinEngine.md#runrenderloop)
- [setAlphaConstants](ThinEngine.md#setalphaconstants)
- [setAlphaEquation](ThinEngine.md#setalphaequation)
- [setAlphaMode](ThinEngine.md#setalphamode)
- [setArray](ThinEngine.md#setarray)
- [setArray2](ThinEngine.md#setarray2)
- [setArray3](ThinEngine.md#setarray3)
- [setArray4](ThinEngine.md#setarray4)
- [setColorWrite](ThinEngine.md#setcolorwrite)
- [setDepthBuffer](ThinEngine.md#setdepthbuffer)
- [setExternalTexture](ThinEngine.md#setexternaltexture)
- [setFloat](ThinEngine.md#setfloat)
- [setFloat2](ThinEngine.md#setfloat2)
- [setFloat3](ThinEngine.md#setfloat3)
- [setFloat4](ThinEngine.md#setfloat4)
- [setHardwareScalingLevel](ThinEngine.md#sethardwarescalinglevel)
- [setInt](ThinEngine.md#setint)
- [setInt2](ThinEngine.md#setint2)
- [setInt3](ThinEngine.md#setint3)
- [setInt4](ThinEngine.md#setint4)
- [setIntArray](ThinEngine.md#setintarray)
- [setIntArray2](ThinEngine.md#setintarray2)
- [setIntArray3](ThinEngine.md#setintarray3)
- [setIntArray4](ThinEngine.md#setintarray4)
- [setMatrices](ThinEngine.md#setmatrices)
- [setMatrix2x2](ThinEngine.md#setmatrix2x2)
- [setMatrix3x3](ThinEngine.md#setmatrix3x3)
- [setSize](ThinEngine.md#setsize)
- [setState](ThinEngine.md#setstate)
- [setStorageBuffer](ThinEngine.md#setstoragebuffer)
- [setTexture](ThinEngine.md#settexture)
- [setTextureArray](ThinEngine.md#settexturearray)
- [setTextureSampler](ThinEngine.md#settexturesampler)
- [setViewport](ThinEngine.md#setviewport)
- [setZOffset](ThinEngine.md#setzoffset)
- [setZOffsetUnits](ThinEngine.md#setzoffsetunits)
- [snapshotRenderingReset](ThinEngine.md#snapshotrenderingreset)
- [stopRenderLoop](ThinEngine.md#stoprenderloop)
- [unBindFramebuffer](ThinEngine.md#unbindframebuffer)
- [unBindMultiColorAttachmentFramebuffer](ThinEngine.md#unbindmulticolorattachmentframebuffer)
- [unbindAllAttributes](ThinEngine.md#unbindallattributes)
- [unbindAllTextures](ThinEngine.md#unbindalltextures)
- [unbindInstanceAttributes](ThinEngine.md#unbindinstanceattributes)
- [updateAndBindInstancesBuffer](ThinEngine.md#updateandbindinstancesbuffer)
- [updateArrayBuffer](ThinEngine.md#updatearraybuffer)
- [updateDynamicIndexBuffer](ThinEngine.md#updatedynamicindexbuffer)
- [updateDynamicTexture](ThinEngine.md#updatedynamictexture)
- [updateDynamicVertexBuffer](ThinEngine.md#updatedynamicvertexbuffer)
- [updateMultipleRenderTargetTextureSampleCount](ThinEngine.md#updatemultiplerendertargettexturesamplecount)
- [updateRawCubeTexture](ThinEngine.md#updaterawcubetexture)
- [updateRawTexture](ThinEngine.md#updaterawtexture)
- [updateRawTexture2DArray](ThinEngine.md#updaterawtexture2darray)
- [updateRawTexture3D](ThinEngine.md#updaterawtexture3d)
- [updateRenderTargetTextureSampleCount](ThinEngine.md#updaterendertargettexturesamplecount)
- [updateStorageBuffer](ThinEngine.md#updatestoragebuffer)
- [updateTextureData](ThinEngine.md#updatetexturedata)
- [updateTextureDimensions](ThinEngine.md#updatetexturedimensions)
- [updateTextureSamplingMode](ThinEngine.md#updatetexturesamplingmode)
- [updateTextureWrappingMode](ThinEngine.md#updatetexturewrappingmode)
- [updateUniformBuffer](ThinEngine.md#updateuniformbuffer)
- [updateVideoTexture](ThinEngine.md#updatevideotexture)
- [wipeCaches](ThinEngine.md#wipecaches)
- [CeilingPOT](ThinEngine.md#ceilingpot)
- [FloorPOT](ThinEngine.md#floorpot)
- [GetExponentOfTwo](ThinEngine.md#getexponentoftwo)
- [NearestPOT](ThinEngine.md#nearestpot)
- [QueueNewFrame](ThinEngine.md#queuenewframe)
- [\_ConcatenateShader](ThinEngine.md#_concatenateshader)
- [\_CreateCanvas](ThinEngine.md#_createcanvas)
- [isSupported](ThinEngine.md#issupported-1)

## Constructors

### constructor

• **new ThinEngine**(`canvasOrContext`, `antialias?`, `options?`, `adaptToDeviceRatio?`)

Creates a new engine

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `canvasOrContext` | [`Nullable`](../modules.md#nullable)`HTMLCanvasElement` \| `WebGLRenderingContext` \| `OffscreenCanvas` \| `WebGL2RenderingContext` | defines the canvas or WebGL context to use for rendering. If you provide a WebGL context, Babylon.js will not hook events on the canvas (like pointers, keyboards, etc...) so no event observables will be available. This is mostly used when Babylon.js is used as a plugin on a system which already used the WebGL context |
| `antialias?` | `boolean` | defines enable antialiasing (default: false) |
| `options?` | [`EngineOptions`](../interfaces/EngineOptions.md) | defines further options to be sent to the getContext() function |
| `adaptToDeviceRatio?` | `boolean` | defines whether to adapt to the device's viewport characteristics (default: false) |

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:758

## Properties

### \_activeRenderLoops

• `Protected` **\_activeRenderLoops**: () => `void`[]

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:424

___

### \_activeRequests

• `Private` **\_activeRequests**: [`IFileRequest`](../interfaces/IFileRequest.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:550

___

### \_audioContext

• `Protected` **\_audioContext**: [`Nullable`](../modules.md#nullable)`AudioContext`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:377

___

### \_audioDestination

• `Protected` **\_audioDestination**: [`Nullable`](../modules.md#nullable)`AudioDestinationNode` \| `MediaStreamAudioDestinationNode`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:378

___

### \_boundUniforms

• `Protected` **\_boundUniforms**: `Object` = `{}`

#### Index signature

▪ [key: `number`]: `WebGLUniformLocation`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:4916

___

### \_cachedVertexArrayObject

• `Private` **\_cachedVertexArrayObject**: [`Nullable`](../modules.md#nullable)`WebGLVertexArrayObject`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:506

___

### \_checkForMobile

• `Private` **\_checkForMobile**: () => `void`

#### Type declaration

▸ (): `void`

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:721

___

### \_compiledEffects

• `Protected` **\_compiledEffects**: `Object` = `{}`

#### Index signature

▪ [key: `string`]: [`Effect`](Effect.md)

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:502

___

### \_contextWasLost

• `Protected` **\_contextWasLost**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:445

___

### \_creationOptions

• `Protected` **\_creationOptions**: [`EngineOptions`](../interfaces/EngineOptions.md)

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:376

___

### \_currentBoundBuffer

• `Protected` **\_currentBoundBuffer**: [`Nullable`](../modules.md#nullable)`WebGLBuffer`[]

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:517

___

### \_currentBufferPointers

• `Private` **\_currentBufferPointers**: `BufferPointer`[]

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:522

___

### \_currentEffect

• `Protected` **\_currentEffect**: [`Nullable`](../modules.md#nullable)[`Effect`](Effect.md)

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:495

___

### \_currentInstanceBuffers

• `Private` **\_currentInstanceBuffers**: [`DataBuffer`](DataBuffer.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:524

___

### \_currentInstanceLocations

• `Private` **\_currentInstanceLocations**: `number`[]

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:523

___

### \_currentTextureChannel

• `Private` **\_currentTextureChannel**: `number` = `-1`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:492

___

### \_emptyCubeTexture

• `Private` **\_emptyCubeTexture**: [`Nullable`](../modules.md#nullable)[`InternalTexture`](InternalTexture.md)

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:539

___

### \_emptyTexture

• `Private` **\_emptyTexture**: [`Nullable`](../modules.md#nullable)[`InternalTexture`](InternalTexture.md)

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:538

___

### \_emptyTexture2DArray

• `Private` **\_emptyTexture2DArray**: [`Nullable`](../modules.md#nullable)[`InternalTexture`](InternalTexture.md)

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:541

___

### \_emptyTexture3D

• `Private` **\_emptyTexture3D**: [`Nullable`](../modules.md#nullable)[`InternalTexture`](InternalTexture.md)

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:540

___

### \_frameId

• `Private` **\_frameId**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:347

___

### \_framebufferDimensionsObject

• `Private` **\_framebufferDimensionsObject**: [`Nullable`](../modules.md#nullable){ `framebufferHeight`: `number` ; `framebufferWidth`: `number`  }

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:573

___

### \_glRenderer

• `Private` **\_glRenderer**: `string`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:417

___

### \_glVendor

• `Private` **\_glVendor**: `string`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:418

___

### \_glVersion

• `Private` **\_glVersion**: `string`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:416

___

### \_highPrecisionShadersAllowed

• `Protected` **\_highPrecisionShadersAllowed**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:388

___

### \_isStencilEnable

• `Protected` **\_isStencilEnable**: `boolean`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:414

___

### \_maxMSAASamplesOverride

• `Private` **\_maxMSAASamplesOverride**: [`Nullable`](../modules.md#nullable)`number` = `null`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:548

___

### \_maxSimultaneousTextures

• `Private` **\_maxSimultaneousTextures**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:547

___

### \_mustWipeVertexAttributes

• `Private` **\_mustWipeVertexAttributes**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:536

___

### \_nextFreeTextureSlots

• `Private` **\_nextFreeTextureSlots**: `number`[]

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:546

___

### \_onContextLost

• `Private` **\_onContextLost**: (`evt`: `Event`) => `void`

#### Type declaration

▸ (`evt`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `evt` | `Event` |

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:443

___

### \_onContextRestored

• `Private` **\_onContextRestored**: (`evt`: `Event`) => `void`

#### Type declaration

▸ (`evt`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `evt` | `Event` |

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:444

___

### \_renderingCanvas

• `Protected` **\_renderingCanvas**: [`Nullable`](../modules.md#nullable)`HTMLCanvasElement`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:374

___

### \_renderingQueueLaunched

• `Protected` **\_renderingQueueLaunched**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:423

___

### \_shaderProcessor

• `Protected` **\_shaderProcessor**: [`Nullable`](../modules.md#nullable)`IShaderProcessor`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:265

___

### \_snapshotRenderingMode

• `Protected` **\_snapshotRenderingMode**: `number` = `Constants.SNAPSHOTRENDERING_STANDARD`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:694

___

### \_textureUnits

• `Private` **\_textureUnits**: `Int32Array`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:525

___

### \_uintIndicesCurrentlySet

• `Private` **\_uintIndicesCurrentlySet**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:516

___

### \_unpackFlipYCached

• `Private` **\_unpackFlipYCached**: [`Nullable`](../modules.md#nullable)`boolean` = `null`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:4362

___

### \_useExactSrgbConversions

• `Protected` **\_useExactSrgbConversions**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:706

___

### \_useReverseDepthBuffer

• `Private` **\_useReverseDepthBuffer**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:304

___

### \_vaoRecordInProgress

• `Private` **\_vaoRecordInProgress**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:535

___

### \_vertexAttribArraysEnabled

• `Private` **\_vertexAttribArraysEnabled**: `boolean`[] = `[]`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:503

___

### \_viewportCached

• `Protected` **\_viewportCached**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `w` | `number` |
| `x` | `number` |
| `y` | `number` |
| `z` | `number` |

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1692

___

### \_windowIsBackground

• `Protected` **\_windowIsBackground**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:375

___

### adaptToDeviceRatio

• **adaptToDeviceRatio**: `boolean` = `false`

If set to true zooming in and out in the browser will rescale the hardware-scaling correctly.

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:555

___

### cullBackFaces

• **cullBackFaces**: [`Nullable`](../modules.md#nullable)`boolean` = `null`

Gets or sets a boolean indicating if back faces must be culled. If false, front faces are culled instead (true by default)
If non null, this takes precedence over the value from the material

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:289

___

### disableUniformBuffers

• **disableUniformBuffers**: `boolean` = `false`

Gets or sets a boolean indicating that uniform buffers must be disabled even if they are supported

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:340

___

### disableVertexArrayObjects

• **disableVertexArrayObjects**: `boolean` = `false`

Gets or sets a boolean indicating that vertex array object must be disabled even if they are supported

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:465

___

### enableUnpackFlipYCached

• **enableUnpackFlipYCached**: `boolean` = `true`

In case you are sharing the context with other applications, it might
be interested to not cache the unpack flip y state to ensure a consistent
value would be set.

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:4369

___

### forcePOTTextures

• **forcePOTTextures**: `boolean` = `false`

Gets or sets a boolean that indicates if textures must be forced to power of 2 size even if not required

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:278

___

### hasOriginBottomLeft

• `Readonly` **hasOriginBottomLeft**: ``true``

Indicates that the origin of the texture/framebuffer space is the bottom left corner. If false, the origin is top left

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:335

___

### hostInformation

• **hostInformation**: [`HostInformation`](../interfaces/HostInformation.md)

Gets information about the current host

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:565

___

### isFullscreen

• **isFullscreen**: `boolean` = `false`

Gets a boolean indicating if the engine is currently rendering in fullscreen mode

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:283

___

### isNDCHalfZRange

• `Readonly` **isNDCHalfZRange**: ``false``

Indicates if the z range in NDC space is 0..1 (value: true) or -1..1 (value: false)

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:330

___

### onBeforeTextureInitObservable

• **onBeforeTextureInitObservable**: [`Observable`](Observable.md)[`Texture`](Texture.md)

Observable event triggered before each texture is initialized

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:662

___

### onContextLostObservable

• **onContextLostObservable**: [`Observable`](Observable.md)[`ThinEngine`](ThinEngine.md)

Observable signaled when a context lost event is raised

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:438

___

### onContextRestoredObservable

• **onContextRestoredObservable**: [`Observable`](Observable.md)[`ThinEngine`](ThinEngine.md)

Observable signaled when a context restored event is raised

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:442

___

### onDisposeObservable

• `Readonly` **onDisposeObservable**: [`Observable`](Observable.md)[`ThinEngine`](ThinEngine.md)

An event triggered when the engine is disposed.

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:345

___

### premultipliedAlpha

• **premultipliedAlpha**: `boolean` = `true`

Defines whether the engine has been created with the premultipliedAlpha option on or not.

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:657

___

### preventCacheWipeBetweenFrames

• **preventCacheWipeBetweenFrames**: `boolean` = `false`

Gets or sets a boolean indicating that cache can be kept between frames

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:299

___

### renderEvenInBackground

• **renderEvenInBackground**: `boolean` = `true`

Gets or sets a boolean indicating if the engine must keep rendering even if the window is not in foreground

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:294

___

### validateShaderPrograms

• **validateShaderPrograms**: `boolean` = `false`

Gets or sets a boolean indicating if the engine should validate programs after compilation

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:302

___

### CollisionsEpsilon

▪ `Static` **CollisionsEpsilon**: `number` = `0.001`

Gets or sets the epsilon value used by collision engine

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:253

___

### ExceptionList

▪ `Static` **ExceptionList**: ({ `capture`: `string` = "63\\.0\\.3239\\.(\\d+)"; `captureConstraint`: `number` = 108; `key`: `string` = "Chrome/63.0"; `targets`: `string`[]  } \| { `capture`: ``null`` = null; `captureConstraint`: ``null`` = null; `key`: `string` = "Firefox/58"; `targets`: `string`[]  })[]

Use this array to turn off some WebGL2 features on known buggy browsers version

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:180

___

### \_HasMajorPerformanceCaveat

▪ `Static` `Private` **\_HasMajorPerformanceCaveat**: [`Nullable`](../modules.md#nullable)`boolean` = `null`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:5789

___

### \_IsSupported

▪ `Static` `Private` **\_IsSupported**: [`Nullable`](../modules.md#nullable)`boolean` = `null`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:5788

## Accessors

### \_supportsHardwareTextureRescaling

• `Protected` `get` **_supportsHardwareTextureRescaling**(): `boolean`

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:569

___

### activeRenderLoops

• `get` **activeRenderLoops**(): () => `void`[]

Gets the list of current active render loop functions

#### Returns

() => `void`[]

an array with the current render loop functions

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:430

___

### alphaState

• `get` **alphaState**(): `AlphaState`

Gets the alpha state manager

#### Returns

`AlphaState`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:3553

___

### currentViewport

• `get` **currentViewport**(): [`Nullable`](../modules.md#nullable)`IViewportLike`

Gets the current viewport

#### Returns

[`Nullable`](../modules.md#nullable)`IViewportLike`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:587

___

### depthCullingState

• `get` **depthCullingState**(): `DepthCullingState`

Gets the depth culling state manager

#### Returns

`DepthCullingState`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:3546

___

### description

• `get` **description**(): `string`

Returns a string describing the current engine

#### Returns

`string`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:217

___

### doNotHandleContextLost

• `get` **doNotHandleContextLost**(): `boolean`

Gets or sets a boolean indicating if resources should be retained to be able to handle context lost events

**`See`**

https://doc.babylonjs.com/how_to/optimizing_your_scene#handling-webgl-context-lost

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:454

• `set` **doNotHandleContextLost**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:458

___

### emptyCubeTexture

• `get` **emptyCubeTexture**(): [`InternalTexture`](InternalTexture.md)

Gets the default empty cube texture

#### Returns

[`InternalTexture`](InternalTexture.md)

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:636

___

### emptyTexture

• `get` **emptyTexture**(): [`InternalTexture`](InternalTexture.md)

Gets the default empty texture

#### Returns

[`InternalTexture`](InternalTexture.md)

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:594

___

### emptyTexture2DArray

• `get` **emptyTexture2DArray**(): [`InternalTexture`](InternalTexture.md)

Gets the default empty 2D array texture

#### Returns

[`InternalTexture`](InternalTexture.md)

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:616

___

### emptyTexture3D

• `get` **emptyTexture3D**(): [`InternalTexture`](InternalTexture.md)

Gets the default empty 3D texture

#### Returns

[`InternalTexture`](InternalTexture.md)

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:605

___

### frameId

• `get` **frameId**(): `number`

Gets the current frame id

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:351

___

### framebufferDimensionsObject

• `set` **framebufferDimensionsObject**(`dimensions`): `void`

sets the object from which width and height will be taken from when getting render width and height
Will fallback to the gl object

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `dimensions` | [`Nullable`](../modules.md#nullable){ `framebufferHeight`: `number` ; `framebufferWidth`: `number`  } | the framebuffer width and height that will be used. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:580

___

### isStencilEnable

• `get` **isStencilEnable**(): `boolean`

Returns true if the stencil buffer has been enabled through the creation option of the context.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1425

___

### isWebGPU

• `get` **isWebGPU**(): `boolean`

Gets a boolean indicating if the engine runs in WebGPU or not.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:669

___

### name

• `get` **name**(): `string`

Gets or sets the name of the engine

#### Returns

`string`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:233

• `set` **name**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `string` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:237

___

### needPOTTextures

• `get` **needPOTTextures**(): `boolean`

Gets a boolean indicating that only power of 2 textures are supported
Please note that you can still use non power of 2 textures but in this case the engine will forcefully convert them

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:398

___

### shaderPlatformName

• `get` **shaderPlatformName**(): `string`

Gets the shader platform name used by the effects.

#### Returns

`string`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:678

___

### snapshotRendering

• `get` **snapshotRendering**(): `boolean`

Enables or disables the snapshot rendering mode
Note that the WebGL engine does not support snapshot rendering so setting the value won't have any effect for this engine

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:686

• `set` **snapshotRendering**(`activate`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `activate` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:690

___

### snapshotRenderingMode

• `get` **snapshotRenderingMode**(): `number`

Gets or sets the snapshot rendering mode

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:698

• `set` **snapshotRenderingMode**(`mode`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `mode` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:702

___

### stencilState

• `get` **stencilState**(): `StencilState`

Gets the stencil state manager

#### Returns

`StencilState`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:3560

___

### stencilStateComposer

• `get` **stencilStateComposer**(): `StencilStateComposer`

Gets the stencil state composer

#### Returns

`StencilStateComposer`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:3567

___

### supportsUniformBuffers

• `get` **supportsUniformBuffers**(): `boolean`

Gets a boolean indicating that the engine supports uniform buffers

**`See`**

https://doc.babylonjs.com/features/webgl2#uniform-buffer-objets

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:364

___

### useExactSrgbConversions

• `get` **useExactSrgbConversions**(): `boolean`

Gets a boolean indicating if the exact sRGB conversions or faster approximations are used for converting to and from linear space.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:710

___

### useReverseDepthBuffer

• `get` **useReverseDepthBuffer**(): `boolean`

Gets or sets a boolean indicating if depth buffer should be reverse, going from far to near.
This can provide greater z depth for distant objects.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:309

• `set` **useReverseDepthBuffer**(`useReverse`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `useReverse` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:313

___

### version

• `get` **version**(): `number`

Returns the version of the engine

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:244

___

### webGLVersion

• `get` **webGLVersion**(): `number`

Gets version of the current webGL context
Keep it for back compat - use version instead

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1410

___

### HasMajorPerformanceCaveat

• `Static` `get` **HasMajorPerformanceCaveat**(): `boolean`

Gets a boolean indicating if the engine can be instantiated on a performant device (ie. if a webGL context can be found and it does not use a slow implementation)

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:5833

___

### IsSupported

• `Static` `get` **IsSupported**(): `boolean`

Gets a boolean indicating if the engine can be instantiated (ie. if a webGL context can be found)

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:5801

___

### IsSupportedAsync

• `Static` `get` **IsSupportedAsync**(): `Promise``boolean`

Gets a Promise indicating if the engine can be instantiated (ie. if a webGL context can be found)

#### Returns

`Promise``boolean`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:5794

___

### NpmPackage

• `Static` `get` **NpmPackage**(): `string`

Returns the current npm package of the sdk

#### Returns

`string`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:203

___

### ShadersRepository

• `Static` `get` **ShadersRepository**(): `string`

Gets or sets the relative url used to load shaders if using the engine in non-minified mode

#### Returns

`string`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:258

• `Static` `set` **ShadersRepository**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `string` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:261

___

### Version

• `Static` `get` **Version**(): `string`

Returns the current version of the framework

#### Returns

`string`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:210

## Methods

### \_activateCurrentTexture

▸ `Private` **_activateCurrentTexture**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:4936

___

### \_bindBuffer

▸ `Private` **_bindBuffer**(`buffer`, `target`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `buffer` | [`Nullable`](../modules.md#nullable)[`DataBuffer`](DataBuffer.md) |
| `target` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2180

___

### \_bindSamplerUniformToChannel

▸ `Private` **_bindSamplerUniformToChannel**(`sourceSlot`, `destination`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `sourceSlot` | `number` |
| `destination` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:5041

___

### \_bindVertexBuffersAttributes

▸ `Private` **_bindVertexBuffersAttributes**(`vertexBuffers`, `effect`, `overrideVertexBuffers?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `vertexBuffers` | `Object` |
| `effect` | [`Effect`](Effect.md) |
| `overrideVertexBuffers?` | `Object` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2260

___

### \_canRenderToFloatFramebuffer

▸ `Private` **_canRenderToFloatFramebuffer**(): `boolean`

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:5352

___

### \_canRenderToFramebuffer

▸ `Private` **_canRenderToFramebuffer**(`type`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `type` | `number` |

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:5367

___

### \_canRenderToHalfFloatFramebuffer

▸ `Private` **_canRenderToHalfFloatFramebuffer**(): `boolean`

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:5359

___

### \_compileRawShader

▸ `Private` **_compileRawShader**(`source`, `type`): `WebGLShader`

#### Parameters

| Name | Type |
| :------ | :------ |
| `source` | `string` |
| `type` | `string` |

#### Returns

`WebGLShader`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2845

___

### \_compileShader

▸ `Private` **_compileShader**(`source`, `type`, `defines`, `shaderVersion`): `WebGLShader`

#### Parameters

| Name | Type |
| :------ | :------ |
| `source` | `string` |
| `type` | `string` |
| `defines` | [`Nullable`](../modules.md#nullable)`string` |
| `shaderVersion` | `string` |

#### Returns

`WebGLShader`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2841

___

### \_createDepthStencilCubeTexture

▸ **_createDepthStencilCubeTexture**(`size`, `options`, `rtWrapper`): [`InternalTexture`](InternalTexture.md)

Creates a depth stencil cube texture.
This is only available in WebGL 2.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `size` | `number` | The size of face edge in the cube texture. |
| `options` | `DepthTextureCreationOptions` | The options defining the cube texture. |
| `rtWrapper` | [`RenderTargetWrapper`](RenderTargetWrapper.md) | The render target wrapper for which the depth/stencil texture must be created |

#### Returns

[`InternalTexture`](InternalTexture.md)

The cube texture

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.cubeTexture.ts:24

___

### \_createShaderProgram

▸ `Protected` **_createShaderProgram**(`pipelineContext`, `vertexShader`, `fragmentShader`, `context`, `transformFeedbackVaryings?`): `WebGLProgram`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `pipelineContext` | `WebGLPipelineContext` | `undefined` |
| `vertexShader` | `WebGLShader` | `undefined` |
| `fragmentShader` | `WebGLShader` | `undefined` |
| `context` | `WebGLRenderingContext` | `undefined` |
| `transformFeedbackVaryings` | [`Nullable`](../modules.md#nullable)`string`[] | `null` |

#### Returns

`WebGLProgram`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2969

___

### \_createTextureBase

▸ `Protected` **_createTextureBase**(`url`, `noMipmap`, `invertY`, `scene`, `samplingMode?`, `onLoad?`, `onError?`, `prepareTexture`, `prepareTextureProcessFunction`, `buffer?`, `fallback?`, `format?`, `forcedExtension?`, `mimeType?`, `loaderOptions?`, `useSRGBBuffer?`): [`InternalTexture`](InternalTexture.md)

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `url` | [`Nullable`](../modules.md#nullable)`string` | `undefined` |
| `noMipmap` | `boolean` | `undefined` |
| `invertY` | `boolean` | `undefined` |
| `scene` | [`Nullable`](../modules.md#nullable)`ISceneLike` | `undefined` |
| `samplingMode` | `number` | `Constants.TEXTURE_TRILINEAR_SAMPLINGMODE` |
| `onLoad` | [`Nullable`](../modules.md#nullable)(`texture`: [`InternalTexture`](InternalTexture.md)) => `void` | `null` |
| `onError` | [`Nullable`](../modules.md#nullable)(`message`: `string`, `exception`: `any`) => `void` | `null` |
| `prepareTexture` | (`texture`: [`InternalTexture`](InternalTexture.md), `extension`: `string`, `scene`: [`Nullable`](../modules.md#nullable)`ISceneLike`, `img`: `HTMLImageElement` \| `ImageBitmap` \| { `height`: `number` ; `width`: `number`  }, `invertY`: `boolean`, `noMipmap`: `boolean`, `isCompressed`: `boolean`, `processFunction`: (`width`: `number`, `height`: `number`, `img`: `HTMLImageElement` \| `ImageBitmap` \| { `height`: `number` ; `width`: `number`  }, `extension`: `string`, `texture`: [`InternalTexture`](InternalTexture.md), `continuationCallback`: () => `void`) => `boolean`, `samplingMode`: `number`) => `void` | `undefined` |
| `prepareTextureProcessFunction` | (`width`: `number`, `height`: `number`, `img`: `HTMLImageElement` \| `ImageBitmap` \| { `height`: `number` ; `width`: `number`  }, `extension`: `string`, `texture`: [`InternalTexture`](InternalTexture.md), `continuationCallback`: () => `void`) => `boolean` | `undefined` |
| `buffer` | [`Nullable`](../modules.md#nullable)`string` \| `ArrayBuffer` \| `ArrayBufferView` \| `Blob` \| `HTMLImageElement` \| `ImageBitmap` | `null` |
| `fallback` | [`Nullable`](../modules.md#nullable)[`InternalTexture`](InternalTexture.md) | `null` |
| `format` | [`Nullable`](../modules.md#nullable)`number` | `null` |
| `forcedExtension` | [`Nullable`](../modules.md#nullable)`string` | `null` |
| `mimeType?` | `string` | `undefined` |
| `loaderOptions?` | `any` | `undefined` |
| `useSRGBBuffer?` | `boolean` | `undefined` |

#### Returns

[`InternalTexture`](InternalTexture.md)

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:3851

___

### \_createVertexBuffer

▸ `Private` **_createVertexBuffer**(`data`, `usage`): [`DataBuffer`](DataBuffer.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `data` | [`DataArray`](../modules.md#dataarray) |
| `usage` | `number` |

#### Returns

[`DataBuffer`](DataBuffer.md)

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2061

___

### \_deleteBuffer

▸ `Protected` **_deleteBuffer**(`buffer`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `buffer` | [`DataBuffer`](DataBuffer.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2474

___

### \_deleteTexture

▸ `Protected` **_deleteTexture**(`texture`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `texture` | [`Nullable`](../modules.md#nullable)`WebGLTexture` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:4903

___

### \_drawMode

▸ `Private` **_drawMode**(`fillMode`): `number`

#### Parameters

| Name | Type |
| :------ | :------ |
| `fillMode` | `number` |

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2670

___

### \_finalizePipelineContext

▸ `Protected` **_finalizePipelineContext**(`pipelineContext`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `pipelineContext` | `WebGLPipelineContext` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2999

___

### \_getTextureTarget

▸ `Private` **_getTextureTarget**(`texture`): `number`

#### Parameters

| Name | Type |
| :------ | :------ |
| `texture` | [`InternalTexture`](InternalTexture.md) |

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:4390

___

### \_getTextureWrapMode

▸ `Private` **_getTextureWrapMode**(`mode`): `number`

#### Parameters

| Name | Type |
| :------ | :------ |
| `mode` | `number` |

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:5050

___

### \_initFeatures

▸ `Protected` **_initFeatures**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1378

___

### \_initGLContext

▸ `Protected` **_initGLContext**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1130

___

### \_normalizeIndexData

▸ `Protected` **_normalizeIndexData**(`indices`): `Uint32Array` \| `Uint16Array`

#### Parameters

| Name | Type |
| :------ | :------ |
| `indices` | [`IndicesArray`](../modules.md#indicesarray) |

#### Returns

`Uint32Array` \| `Uint16Array`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2121

___

### \_prepareWebGLTexture

▸ `Private` **_prepareWebGLTexture**(`texture`, `extension`, `scene`, `img`, `invertY`, `noMipmap`, `isCompressed`, `processFunction`, `samplingMode?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `texture` | [`InternalTexture`](InternalTexture.md) | `undefined` |
| `extension` | `string` | `undefined` |
| `scene` | [`Nullable`](../modules.md#nullable)`ISceneLike` | `undefined` |
| `img` | `HTMLImageElement` \| `ImageBitmap` \| { `height`: `number` ; `width`: `number`  } | `undefined` |
| `invertY` | `boolean` | `undefined` |
| `noMipmap` | `boolean` | `undefined` |
| `isCompressed` | `boolean` | `undefined` |
| `processFunction` | (`width`: `number`, `height`: `number`, `img`: `HTMLImageElement` \| `ImageBitmap` \| { `height`: `number` ; `width`: `number`  }, `extension`: `string`, `texture`: [`InternalTexture`](InternalTexture.md), `continuationCallback`: () => `void`) => `boolean` | `undefined` |
| `samplingMode` | `number` | `Constants.TEXTURE_TRILINEAR_SAMPLINGMODE` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:4728

___

### \_prepareWebGLTextureContinuation

▸ `Protected` **_prepareWebGLTextureContinuation**(`texture`, `scene`, `noMipmap`, `isCompressed`, `samplingMode`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `texture` | [`InternalTexture`](InternalTexture.md) |
| `scene` | [`Nullable`](../modules.md#nullable)`ISceneLike` |
| `noMipmap` | `boolean` |
| `isCompressed` | `boolean` |
| `samplingMode` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:4702

___

### \_rebuildBuffers

▸ `Protected` **_rebuildBuffers**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1119

___

### \_rebuildEffects

▸ `Private` **_rebuildEffects**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1091

___

### \_rebuildInternalTextures

▸ `Private` **_rebuildInternalTextures**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1075

___

### \_rebuildRenderTargetWrappers

▸ `Private` **_rebuildRenderTargetWrappers**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1083

___

### \_resetIndexBufferBinding

▸ `Protected` **_resetIndexBufferBinding**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2092

___

### \_restoreEngineAfterContextLost

▸ `Protected` **_restoreEngineAfterContextLost**(`initEngine`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `initEngine` | () => `void` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1022

___

### \_setProgram

▸ `Protected` **_setProgram**(`program`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `program` | `WebGLProgram` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:4909

___

### \_setTexture

▸ `Protected` **_setTexture**(`channel`, `texture`, `isPartOfTextureArray?`, `depthStencilTexture?`, `name?`): `boolean`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `channel` | `number` | `undefined` |
| `texture` | [`Nullable`](../modules.md#nullable)[`ThinTexture`](ThinTexture.md) | `undefined` |
| `isPartOfTextureArray` | `boolean` | `false` |
| `depthStencilTexture` | `boolean` | `false` |
| `name` | `string` | `""` |

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:5062

___

### \_setTextureParameterFloat

▸ `Private` **_setTextureParameterFloat**(`target`, `parameter`, `value`, `texture`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `target` | `number` |
| `parameter` | `number` |
| `value` | `number` |
| `texture` | [`InternalTexture`](InternalTexture.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:5214

___

### \_setTextureParameterInteger

▸ `Private` **_setTextureParameterInteger**(`target`, `parameter`, `value`, `texture?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `target` | `number` |
| `parameter` | `number` |
| `value` | `number` |
| `texture?` | [`InternalTexture`](InternalTexture.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:5219

___

### \_sharedInit

▸ `Protected` **_sharedInit**(`canvas`, `doNotHandleTouchAction`, `audioEngine`): `void`

Shared initialization across engines types.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `canvas` | `HTMLCanvasElement` | The canvas associated with this instance of the engine. |
| `doNotHandleTouchAction` | `boolean` | Defines that engine should ignore modifying touch action attribute and style |
| `audioEngine` | `boolean` | Defines if an audio engine should be created by default |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1063

___

### \_unbindVertexArrayObject

▸ `Private` **_unbindVertexArrayObject**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2401

___

### \_vertexAttribPointer

▸ `Private` **_vertexAttribPointer**(`buffer`, `indx`, `size`, `type`, `normalized`, `stride`, `offset`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `buffer` | [`DataBuffer`](DataBuffer.md) |
| `indx` | `number` |
| `size` | `number` |
| `type` | `number` |
| `normalized` | `boolean` |
| `stride` | `number` |
| `offset` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2195

___

### applyStates

▸ **applyStates**(): `void`

Apply all cached states (depth, culling, stencil and alpha)

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:3512

___

### areAllComputeEffectsReady

▸ **areAllComputeEffectsReady**(): `boolean`

Gets a boolean indicating if all created compute effects are ready

#### Returns

`boolean`

true if all effects are ready

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.computeShader.ts:79

___

### areAllEffectsReady

▸ **areAllEffectsReady**(): `boolean`

Gets a boolean indicating if all created effects are ready

#### Returns

`boolean`

true if all effects are ready

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1107

___

### attachContextLostEvent

▸ **attachContextLostEvent**(`callback`): `void`

Attach a new callback raised when context lost event is fired

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callback` | (`event`: `WebGLContextEvent`) => `void` | defines the callback to call |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:5327

___

### attachContextRestoredEvent

▸ **attachContextRestoredEvent**(`callback`): `void`

Attach a new callback raised when context restored event is fired

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callback` | (`event`: `WebGLContextEvent`) => `void` | defines the callback to call |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:5337

___

### beginFrame

▸ **beginFrame**(): `void`

Begin a new frame

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1732

___

### bindArrayBuffer

▸ **bindArrayBuffer**(`buffer`): `void`

Bind a webGL buffer to the webGL context

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `buffer` | [`Nullable`](../modules.md#nullable)[`DataBuffer`](DataBuffer.md) | defines the buffer to bind |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2151

___

### bindAttachments

▸ **bindAttachments**(`attachments`): `void`

Select a subsets of attachments to draw to.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `attachments` | `number`[] | gl attachments |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.multiRender.ts:47

___

### bindBuffers

▸ **bindBuffers**(`vertexBuffers`, `indexBuffer`, `effect`, `overrideVertexBuffers?`): `void`

Bind a list of vertex buffers to the webGL context

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vertexBuffers` | `Object` | defines the list of vertex buffers to bind |
| `indexBuffer` | [`Nullable`](../modules.md#nullable)[`DataBuffer`](DataBuffer.md) | defines the index buffer to bind |
| `effect` | [`Effect`](Effect.md) | defines the effect associated with the vertex buffers |
| `overrideVertexBuffers?` | `Object` | defines optional list of avertex buffers that overrides the entries in vertexBuffers |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2417

___

### bindBuffersDirectly

▸ **bindBuffersDirectly**(`vertexBuffer`, `indexBuffer`, `vertexDeclaration`, `vertexStrideSize`, `effect`): `void`

Bind webGl buffers directly to the webGL context

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vertexBuffer` | [`DataBuffer`](DataBuffer.md) | defines the vertex buffer to bind |
| `indexBuffer` | [`DataBuffer`](DataBuffer.md) | defines the index buffer to bind |
| `vertexDeclaration` | `number`[] | defines the vertex declaration to use with the vertex buffer |
| `vertexStrideSize` | `number` | defines the vertex stride of the vertex buffer |
| `effect` | [`Effect`](Effect.md) | defines the effect associated with the vertex buffer |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2372

___

### bindFramebuffer

▸ **bindFramebuffer**(`texture`, `faceIndex?`, `requiredWidth?`, `requiredHeight?`, `forceFullscreenViewport?`, `lodLevel?`, `layer?`): `void`

Binds the frame buffer to the specified texture.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `texture` | [`RenderTargetWrapper`](RenderTargetWrapper.md) | `undefined` | The render target wrapper to render to |
| `faceIndex` | `number` | `0` | The face of the texture to render to in case of cube texture |
| `requiredWidth?` | `number` | `undefined` | The width of the target to render to |
| `requiredHeight?` | `number` | `undefined` | The height of the target to render to |
| `forceFullscreenViewport?` | `boolean` | `undefined` | Forces the viewport to be the entire texture/screen if true |
| `lodLevel` | `number` | `0` | defines the lod level to bind to the frame buffer |
| `layer` | `number` | `0` | defines the 2d array index to bind to frame buffer to |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1807

___

### bindIndexBuffer

▸ `Protected` **bindIndexBuffer**(`buffer`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `buffer` | [`Nullable`](../modules.md#nullable)[`DataBuffer`](DataBuffer.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2173

___

### bindInstancesBuffer

▸ **bindInstancesBuffer**(`instancesBuffer`, `attributesInfo`, `computeStride?`): `void`

Bind the content of a webGL buffer used with instantiation

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `instancesBuffer` | [`DataBuffer`](DataBuffer.md) | `undefined` | defines the webGL buffer to bind |
| `attributesInfo` | [`InstancingAttributeInfo`](../interfaces/InstancingAttributeInfo.md)[] | `undefined` | defines the offsets or attributes information used to determine where data must be stored in the buffer |
| `computeStride` | `boolean` | `true` | defines Whether to compute the strides from the info or use the default 0 |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2515

___

### bindSamplers

▸ **bindSamplers**(`effect`): `void`

Binds an effect to the webGL context

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `effect` | [`Effect`](Effect.md) | defines the effect to bind |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:4922

___

### bindUniformBlock

▸ **bindUniformBlock**(`pipelineContext`, `blockName`, `index`): `void`

Bind a specific block at a given index in a specific shader program

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `pipelineContext` | [`IPipelineContext`](../interfaces/IPipelineContext.md) | defines the pipeline context to use |
| `blockName` | `string` | defines the block name |
| `index` | `number` | defines the index where to bind the block |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2164

▸ **bindUniformBlock**(`pipelineContext`, `blockName`, `index`): `void`

Bind a specific block at a given index in a specific shader program

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `pipelineContext` | [`IPipelineContext`](../interfaces/IPipelineContext.md) | defines the pipeline context to use |
| `blockName` | `string` | defines the block name |
| `index` | `number` | defines the index where to bind the block |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.uniformBuffer.ts:56

___

### bindUniformBuffer

▸ **bindUniformBuffer**(`buffer`): `void`

Bind an uniform buffer to the current webGL context

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `buffer` | [`Nullable`](../modules.md#nullable)[`DataBuffer`](DataBuffer.md) | defines the buffer to bind |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.uniformBuffer.ts:40

___

### bindUniformBufferBase

▸ **bindUniformBufferBase**(`buffer`, `location`, `name`): `void`

Bind a buffer to the current webGL context at a given location

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `buffer` | [`DataBuffer`](DataBuffer.md) | defines the buffer to bind |
| `location` | `number` | defines the index where to bind the buffer |
| `name` | `string` | Name of the uniform variable to bind |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.uniformBuffer.ts:48

___

### bindVertexArrayObject

▸ **bindVertexArrayObject**(`vertexArrayObject`, `indexBuffer`): `void`

Bind a specific vertex array object

**`See`**

https://doc.babylonjs.com/features/webgl2#vertex-array-objects

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vertexArrayObject` | `WebGLVertexArrayObject` | defines the vertex array object to bind |
| `indexBuffer` | [`Nullable`](../modules.md#nullable)[`DataBuffer`](DataBuffer.md) | defines the index buffer to bind |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2351

___

### buildTextureLayout

▸ **buildTextureLayout**(`textureStatus`): `number`[]

Creates a layout object to draw/clear on specific textures in a MRT

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `textureStatus` | `boolean`[] | textureStatus[i] indicates if the i-th is active |

#### Returns

`number`[]

A layout to be fed to the engine, calling `bindAttachments`.

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.multiRender.ts:54

___

### clear

▸ **clear**(`color`, `backBuffer`, `depth`, `stencil?`): `void`

Clear the current render buffer or the current render target (if any is set up)

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `color` | [`Nullable`](../modules.md#nullable)`IColor4Like` | `undefined` | defines the color to use |
| `backBuffer` | `boolean` | `undefined` | defines if the back buffer must be cleared |
| `depth` | `boolean` | `undefined` | defines if the depth buffer must be cleared |
| `stencil` | `boolean` | `false` | defines if the stencil buffer must be cleared |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1662

___

### clearInternalTexturesCache

▸ **clearInternalTexturesCache**(): `void`

Clears the list of texture accessible through engine.
This can help preventing texture load conflict due to name collision.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:3577

___

### computeDispatch

▸ **computeDispatch**(`effect`, `context`, `bindings`, `x`, `y?`, `z?`, `bindingsMapping?`): `void`

Dispatches a compute shader

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `effect` | [`ComputeEffect`](ComputeEffect.md) | The compute effect |
| `context` | `IComputeContext` | The compute context |
| `bindings` | `ComputeBindingList` | The list of resources to bind to the shader |
| `x` | `number` | The number of workgroups to execute on the X dimension |
| `y?` | `number` | The number of workgroups to execute on the Y dimension |
| `z?` | `number` | The number of workgroups to execute on the Z dimension |
| `bindingsMapping?` | [`ComputeBindingMapping`](../modules.md#computebindingmapping) | list of bindings mapping (key is property name, value is binding location) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.computeShader.ts:65

___

### createCanvas

▸ **createCanvas**(`width`, `height`): [`ICanvas`](../interfaces/ICanvas.md)

Create a canvas. This method is overridden by other engines

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `width` | `number` | width |
| `height` | `number` | height |

#### Returns

[`ICanvas`](../interfaces/ICanvas.md)

ICanvas interface

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:739

___

### createCanvasImage

▸ **createCanvasImage**(): [`IImage`](../interfaces/IImage.md)

Create an image to use with canvas

#### Returns

[`IImage`](../interfaces/IImage.md)

IImage interface

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:747

___

### createComputeContext

▸ **createComputeContext**(): `undefined` \| `IComputeContext`

Creates a new compute context

#### Returns

`undefined` \| `IComputeContext`

the new context

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.computeShader.ts:53

___

### createComputeEffect

▸ **createComputeEffect**(`baseName`, `options`): [`ComputeEffect`](ComputeEffect.md)

Creates a new compute effect

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `baseName` | `any` | Name of the effect |
| `options` | [`IComputeEffectCreationOptions`](../interfaces/IComputeEffectCreationOptions.md) | Options used to create the effect |

#### Returns

[`ComputeEffect`](ComputeEffect.md)

The new compute effect

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.computeShader.ts:41

___

### createComputePipelineContext

▸ **createComputePipelineContext**(): `IComputePipelineContext`

Creates a new compute pipeline context

#### Returns

`IComputePipelineContext`

the new pipeline

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.computeShader.ts:47

___

### createCubeTexture

▸ **createCubeTexture**(`rootUrl`, `scene`, `files`, `noMipmap`, `onLoad`, `onError`, `format`, `forcedExtension`, `createPolynomials`, `lodScale`, `lodOffset`, `fallback`, `loaderOptions`, `useSRGBBuffer`): [`InternalTexture`](InternalTexture.md)

Creates a cube texture

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `rootUrl` | `string` | defines the url where the files to load is located |
| `scene` | [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) | defines the current scene |
| `files` | [`Nullable`](../modules.md#nullable)`string`[] | defines the list of files to load (1 per face) |
| `noMipmap` | `undefined` \| `boolean` | defines a boolean indicating that no mipmaps shall be generated (false by default) |
| `onLoad` | [`Nullable`](../modules.md#nullable)(`data?`: `any`) => `void` | defines an optional callback raised when the texture is loaded |
| `onError` | [`Nullable`](../modules.md#nullable)(`message?`: `string`, `exception?`: `any`) => `void` | defines an optional callback raised if there is an issue to load the texture |
| `format` | `undefined` \| `number` | defines the format of the data |
| `forcedExtension` | `any` | defines the extension to use to pick the right loader |
| `createPolynomials` | `boolean` | if a polynomial sphere should be created for the cube texture |
| `lodScale` | `number` | defines the scale applied to environment texture. This manages the range of LOD level used for IBL according to the roughness |
| `lodOffset` | `number` | defines the offset applied to environment texture. This manages first LOD level used for IBL according to the roughness |
| `fallback` | [`Nullable`](../modules.md#nullable)[`InternalTexture`](InternalTexture.md) | defines texture to use while falling back when (compressed) texture file not found. |
| `loaderOptions` | `any` | options to be passed to the loader |
| `useSRGBBuffer` | `boolean` | defines if the texture must be loaded in a sRGB GPU buffer (if supported by the GPU). |

#### Returns

[`InternalTexture`](InternalTexture.md)

the cube texture as an InternalTexture

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.cubeTexture.ts:44

▸ **createCubeTexture**(`rootUrl`, `scene`, `files`, `noMipmap`, `onLoad`, `onError`, `format`, `forcedExtension`): [`InternalTexture`](InternalTexture.md)

Creates a cube texture

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `rootUrl` | `string` | defines the url where the files to load is located |
| `scene` | [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) | defines the current scene |
| `files` | [`Nullable`](../modules.md#nullable)`string`[] | defines the list of files to load (1 per face) |
| `noMipmap` | `boolean` | defines a boolean indicating that no mipmaps shall be generated (false by default) |
| `onLoad` | [`Nullable`](../modules.md#nullable)(`data?`: `any`) => `void` | defines an optional callback raised when the texture is loaded |
| `onError` | [`Nullable`](../modules.md#nullable)(`message?`: `string`, `exception?`: `any`) => `void` | defines an optional callback raised if there is an issue to load the texture |
| `format` | `undefined` \| `number` | defines the format of the data |
| `forcedExtension` | `any` | defines the extension to use to pick the right loader |

#### Returns

[`InternalTexture`](InternalTexture.md)

the cube texture as an InternalTexture

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.cubeTexture.ts:73

▸ **createCubeTexture**(`rootUrl`, `scene`, `files`, `noMipmap`, `onLoad`, `onError`, `format`, `forcedExtension`, `createPolynomials`, `lodScale`, `lodOffset`): [`InternalTexture`](InternalTexture.md)

Creates a cube texture

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `rootUrl` | `string` | defines the url where the files to load is located |
| `scene` | [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) | defines the current scene |
| `files` | [`Nullable`](../modules.md#nullable)`string`[] | defines the list of files to load (1 per face) |
| `noMipmap` | `boolean` | defines a boolean indicating that no mipmaps shall be generated (false by default) |
| `onLoad` | [`Nullable`](../modules.md#nullable)(`data?`: `any`) => `void` | defines an optional callback raised when the texture is loaded |
| `onError` | [`Nullable`](../modules.md#nullable)(`message?`: `string`, `exception?`: `any`) => `void` | defines an optional callback raised if there is an issue to load the texture |
| `format` | `undefined` \| `number` | defines the format of the data |
| `forcedExtension` | `any` | defines the extension to use to pick the right loader |
| `createPolynomials` | `boolean` | if a polynomial sphere should be created for the cube texture |
| `lodScale` | `number` | defines the scale applied to environment texture. This manages the range of LOD level used for IBL according to the roughness |
| `lodOffset` | `number` | defines the offset applied to environment texture. This manages first LOD level used for IBL according to the roughness |

#### Returns

[`InternalTexture`](InternalTexture.md)

the cube texture as an InternalTexture

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.cubeTexture.ts:99

___

### createDepthStencilTexture

▸ **createDepthStencilTexture**(`size`, `options`, `rtWrapper`): [`InternalTexture`](InternalTexture.md)

Creates a depth stencil texture.
This is only available in WebGL 2 or with the depth texture extension available.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `size` | `TextureSize` | The size of face edge in the texture. |
| `options` | `DepthTextureCreationOptions` | The options defining the texture. |
| `rtWrapper` | [`RenderTargetWrapper`](RenderTargetWrapper.md) | The render target wrapper for which the depth/stencil texture must be created |

#### Returns

[`InternalTexture`](InternalTexture.md)

The texture

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.renderTarget.ts:36

___

### createDrawContext

▸ **createDrawContext**(): `undefined` \| `IDrawContext`

Creates a new draw context

#### Returns

`undefined` \| `IDrawContext`

the new context

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2965

___

### createDynamicTexture

▸ **createDynamicTexture**(`width`, `height`, `generateMipMaps`, `samplingMode`): [`InternalTexture`](InternalTexture.md)

Creates a dynamic texture

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `width` | `number` | defines the width of the texture |
| `height` | `number` | defines the height of the texture |
| `generateMipMaps` | `boolean` | defines if the engine should generate the mip levels |
| `samplingMode` | `number` | defines the required sampling mode (Texture.NEAREST_SAMPLINGMODE by default) |

#### Returns

[`InternalTexture`](InternalTexture.md)

the dynamic texture inside an InternalTexture

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.dynamicTexture.ts:16

___

### createDynamicUniformBuffer

▸ **createDynamicUniformBuffer**(`elements`): [`DataBuffer`](DataBuffer.md)

Create a dynamic uniform buffer

**`See`**

https://doc.babylonjs.com/features/webgl2#uniform-buffer-objets

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `elements` | [`FloatArray`](../modules.md#floatarray) | defines the content of the uniform buffer |

#### Returns

[`DataBuffer`](DataBuffer.md)

the webGL uniform buffer

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.uniformBuffer.ts:24

___

### createDynamicVertexBuffer

▸ **createDynamicVertexBuffer**(`data`): [`DataBuffer`](DataBuffer.md)

Creates a dynamic vertex buffer

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | [`DataArray`](../modules.md#dataarray) | the data for the dynamic vertex buffer |

#### Returns

[`DataBuffer`](DataBuffer.md)

the new WebGL dynamic buffer

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2088

___

### createEffect

▸ **createEffect**(`baseName`, `attributesNamesOrOptions`, `uniformsNamesOrEngine`, `samplers?`, `defines?`, `fallbacks?`, `onCompiled?`, `onError?`, `indexParameters?`, `shaderLanguage?`): [`Effect`](Effect.md)

Create a new effect (used to store vertex/fragment shaders)

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `baseName` | `any` | `undefined` | defines the base name of the effect (The name of file without .fragment.fx or .vertex.fx) |
| `attributesNamesOrOptions` | `string`[] \| [`IEffectCreationOptions`](../interfaces/IEffectCreationOptions.md) | `undefined` | defines either a list of attribute names or an IEffectCreationOptions object |
| `uniformsNamesOrEngine` | `string`[] \| [`ThinEngine`](ThinEngine.md) | `undefined` | defines either a list of uniform names or the engine to use |
| `samplers?` | `string`[] | `undefined` | defines an array of string used to represent textures |
| `defines?` | `string` | `undefined` | defines the string containing the defines to use to compile the shaders |
| `fallbacks?` | [`IEffectFallbacks`](../interfaces/IEffectFallbacks.md) | `undefined` | defines the list of potential fallbacks to use if shader compilation fails |
| `onCompiled?` | [`Nullable`](../modules.md#nullable)(`effect`: [`Effect`](Effect.md)) => `void` | `undefined` | defines a function to call when the effect creation is successful |
| `onError?` | [`Nullable`](../modules.md#nullable)(`effect`: [`Effect`](Effect.md), `errors`: `string`) => `void` | `undefined` | defines a function to call when the effect creation has failed |
| `indexParameters?` | `any` | `undefined` | defines an object containing the index values to use to compile shaders (like the maximum number of simultaneous lights) |
| `shaderLanguage` | [`ShaderLanguage`](../enums/ShaderLanguage.md) | `ShaderLanguage.GLSL` | the language the shader is written in (default: GLSL) |

#### Returns

[`Effect`](Effect.md)

the new Effect

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2786

___

### createExternalTexture

▸ **createExternalTexture**(`video`): [`Nullable`](../modules.md#nullable)[`ExternalTexture`](ExternalTexture.md)

Creates an external texture

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `video` | `HTMLVideoElement` | video element |

#### Returns

[`Nullable`](../modules.md#nullable)[`ExternalTexture`](ExternalTexture.md)

the external texture, or null if external textures are not supported by the engine

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.externalTexture.ts:12

___

### createIndexBuffer

▸ **createIndexBuffer**(`indices`, `updatable?`): [`DataBuffer`](DataBuffer.md)

Creates a new index buffer

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `indices` | [`IndicesArray`](../modules.md#indicesarray) | defines the content of the index buffer |
| `updatable?` | `boolean` | defines if the index buffer must be updatable |

#### Returns

[`DataBuffer`](DataBuffer.md)

a new webGL buffer

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2103

___

### createMaterialContext

▸ **createMaterialContext**(): `undefined` \| `IMaterialContext`

Creates a new material context

#### Returns

`undefined` \| `IMaterialContext`

the new context

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2957

___

### createMultipleRenderTarget

▸ **createMultipleRenderTarget**(`size`, `options`, `initializeBuffers?`): [`RenderTargetWrapper`](RenderTargetWrapper.md)

Create a multi render target texture

**`See`**

https://doc.babylonjs.com/features/webgl2#multiple-render-target

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `size` | `TextureSize` | defines the size of the texture |
| `options` | [`IMultiRenderTargetOptions`](../interfaces/IMultiRenderTargetOptions.md) | defines the creation options |
| `initializeBuffers?` | `boolean` | if set to true, the engine will make an initializing call of drawBuffers |

#### Returns

[`RenderTargetWrapper`](RenderTargetWrapper.md)

a new render target wrapper ready to render textures

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.multiRender.ts:31

___

### createPipelineContext

▸ **createPipelineContext**(`shaderProcessingContext`): [`IPipelineContext`](../interfaces/IPipelineContext.md)

Creates a new pipeline context

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `shaderProcessingContext` | [`Nullable`](../modules.md#nullable)`ShaderProcessingContext` | defines the shader processing context used during the processing if available |

#### Returns

[`IPipelineContext`](../interfaces/IPipelineContext.md)

the new pipeline

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2942

___

### createPrefilteredCubeTexture

▸ **createPrefilteredCubeTexture**(`rootUrl`, `scene`, `lodScale`, `lodOffset`, `onLoad?`, `onError?`, `format?`, `forcedExtension?`, `createPolynomials?`): [`InternalTexture`](InternalTexture.md)

Create a cube texture from prefiltered data (ie. the mipmaps contain ready to use data for PBR reflection)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `rootUrl` | `string` | defines the url where the file to load is located |
| `scene` | [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) | defines the current scene |
| `lodScale` | `number` | defines scale to apply to the mip map selection |
| `lodOffset` | `number` | defines offset to apply to the mip map selection |
| `onLoad?` | [`Nullable`](../modules.md#nullable)(`internalTexture`: [`Nullable`](../modules.md#nullable)[`InternalTexture`](InternalTexture.md)) => `void` | defines an optional callback raised when the texture is loaded |
| `onError?` | [`Nullable`](../modules.md#nullable)(`message?`: `string`, `exception?`: `any`) => `void` | defines an optional callback raised if there is an issue to load the texture |
| `format?` | `number` | defines the format of the data |
| `forcedExtension?` | `any` | defines the extension to use to pick the right loader |
| `createPolynomials?` | `boolean` | defines wheter or not to create polynomails harmonics for the texture |

#### Returns

[`InternalTexture`](InternalTexture.md)

the cube texture as an InternalTexture

#### Defined in

https://github.com/babylon.js/core/src/Misc/dds.ts:733

___

### createRawCubeTexture

▸ **createRawCubeTexture**(`data`, `size`, `format`, `type`, `generateMipMaps`, `invertY`, `samplingMode`, `compression?`): [`InternalTexture`](InternalTexture.md)

Creates a new raw cube texture

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `data` | [`Nullable`](../modules.md#nullable)`ArrayBufferView`[] | `undefined` | defines the array of data to use to create each face |
| `size` | `number` | `undefined` | defines the size of the textures |
| `format` | `number` | `undefined` | defines the format of the data |
| `type` | `number` | `undefined` | defines the type of the data (like Engine.TEXTURETYPE_UNSIGNED_INT) |
| `generateMipMaps` | `boolean` | `undefined` | defines if the engine should generate the mip levels |
| `invertY` | `boolean` | `undefined` | defines if data must be stored with Y axis inverted |
| `samplingMode` | `number` | `undefined` | defines the required sampling mode (like Texture.NEAREST_SAMPLINGMODE) |
| `compression` | [`Nullable`](../modules.md#nullable)`string` | `null` | defines the compression used (null by default) |

#### Returns

[`InternalTexture`](InternalTexture.md)

the cube texture as an InternalTexture

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:4291

▸ **createRawCubeTexture**(`data`, `size`, `format`, `type`, `generateMipMaps`, `invertY`, `samplingMode`, `compression`): [`InternalTexture`](InternalTexture.md)

Creates a new raw cube texture

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | [`Nullable`](../modules.md#nullable)`ArrayBufferView`[] | defines the array of data to use to create each face |
| `size` | `number` | defines the size of the textures |
| `format` | `number` | defines the format of the data |
| `type` | `number` | defines the type of the data (like Engine.TEXTURETYPE_UNSIGNED_INT) |
| `generateMipMaps` | `boolean` | defines if the engine should generate the mip levels |
| `invertY` | `boolean` | defines if data must be stored with Y axis inverted |
| `samplingMode` | `number` | defines the required sampling mode (like Texture.NEAREST_SAMPLINGMODE) |
| `compression` | [`Nullable`](../modules.md#nullable)`string` | defines the compression used (null by default) |

#### Returns

[`InternalTexture`](InternalTexture.md)

the cube texture as an InternalTexture

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.rawTexture.ts:82

___

### createRawCubeTextureFromUrl

▸ **createRawCubeTextureFromUrl**(`url`, `scene`, `size`, `format`, `type`, `noMipmap`, `callback`, `mipmapGenerator`, `onLoad`, `onError`): [`InternalTexture`](InternalTexture.md)

Creates a new raw cube texture from a specified url

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `url` | `string` | defines the url where the data is located |
| `scene` | [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) | defines the current scene |
| `size` | `number` | defines the size of the textures |
| `format` | `number` | defines the format of the data |
| `type` | `number` | defines the type fo the data (like Engine.TEXTURETYPE_UNSIGNED_INT) |
| `noMipmap` | `boolean` | defines if the engine should avoid generating the mip levels |
| `callback` | (`ArrayBuffer`: `ArrayBuffer`) => [`Nullable`](../modules.md#nullable)`ArrayBufferView`[] | defines a callback used to extract texture data from loaded data |
| `mipmapGenerator` | [`Nullable`](../modules.md#nullable)(`faces`: `ArrayBufferView`[]) => `ArrayBufferView`[][] | defines to provide an optional tool to generate mip levels |
| `onLoad` | [`Nullable`](../modules.md#nullable)() => `void` | defines a callback called when texture is loaded |
| `onError` | [`Nullable`](../modules.md#nullable)(`message?`: `string`, `exception?`: `any`) => `void` | defines a callback called if there is an error |

#### Returns

[`InternalTexture`](InternalTexture.md)

the cube texture as an InternalTexture

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.rawTexture.ts:140

▸ **createRawCubeTextureFromUrl**(`url`, `scene`, `size`, `format`, `type`, `noMipmap`, `callback`, `mipmapGenerator`, `onLoad`, `onError`, `samplingMode`, `invertY`): [`InternalTexture`](InternalTexture.md)

Creates a new raw cube texture from a specified url

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `url` | `string` | defines the url where the data is located |
| `scene` | [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) | defines the current scene |
| `size` | `number` | defines the size of the textures |
| `format` | `number` | defines the format of the data |
| `type` | `number` | defines the type fo the data (like Engine.TEXTURETYPE_UNSIGNED_INT) |
| `noMipmap` | `boolean` | defines if the engine should avoid generating the mip levels |
| `callback` | (`ArrayBuffer`: `ArrayBuffer`) => [`Nullable`](../modules.md#nullable)`ArrayBufferView`[] | defines a callback used to extract texture data from loaded data |
| `mipmapGenerator` | [`Nullable`](../modules.md#nullable)(`faces`: `ArrayBufferView`[]) => `ArrayBufferView`[][] | defines to provide an optional tool to generate mip levels |
| `onLoad` | [`Nullable`](../modules.md#nullable)() => `void` | defines a callback called when texture is loaded |
| `onError` | [`Nullable`](../modules.md#nullable)(`message?`: `string`, `exception?`: `any`) => `void` | defines a callback called if there is an error |
| `samplingMode` | `number` | defines the required sampling mode (like Texture.NEAREST_SAMPLINGMODE) |
| `invertY` | `boolean` | defines if data must be stored with Y axis inverted |

#### Returns

[`InternalTexture`](InternalTexture.md)

the cube texture as an InternalTexture

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.rawTexture.ts:169

___

### createRawShaderProgram

▸ **createRawShaderProgram**(`pipelineContext`, `vertexCode`, `fragmentCode`, `context?`, `transformFeedbackVaryings?`): `WebGLProgram`

Directly creates a webGL program

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `pipelineContext` | [`IPipelineContext`](../interfaces/IPipelineContext.md) | `undefined` | defines the pipeline context to attach to |
| `vertexCode` | `string` | `undefined` | defines the vertex shader code to use |
| `fragmentCode` | `string` | `undefined` | defines the fragment shader code to use |
| `context?` | `WebGLRenderingContext` | `undefined` | defines the webGL context to use (if not set, the current one will be used) |
| `transformFeedbackVaryings` | [`Nullable`](../modules.md#nullable)`string`[] | `null` | defines the list of transform feedback varyings to use |

#### Returns

`WebGLProgram`

the new webGL program

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2885

___

### createRawTexture

▸ **createRawTexture**(`data`, `width`, `height`, `format`, `generateMipMaps`, `invertY`, `samplingMode`, `compression?`, `type?`, `creationFlags?`, `useSRGBBuffer?`): [`InternalTexture`](InternalTexture.md)

Creates a raw texture

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `data` | [`Nullable`](../modules.md#nullable)`ArrayBufferView` | `undefined` | defines the data to store in the texture |
| `width` | `number` | `undefined` | defines the width of the texture |
| `height` | `number` | `undefined` | defines the height of the texture |
| `format` | `number` | `undefined` | defines the format of the data |
| `generateMipMaps` | `boolean` | `undefined` | defines if the engine should generate the mip levels |
| `invertY` | `boolean` | `undefined` | defines if data must be stored with Y axis inverted |
| `samplingMode` | `number` | `undefined` | defines the required sampling mode (Texture.NEAREST_SAMPLINGMODE by default) |
| `compression` | [`Nullable`](../modules.md#nullable)`string` | `null` | defines the compression used (null by default) |
| `type` | `number` | `Constants.TEXTURETYPE_UNSIGNED_INT` | defines the type fo the data (Engine.TEXTURETYPE_UNSIGNED_INT by default) |
| `creationFlags` | `number` | `0` | specific flags to use when creating the texture (Constants.TEXTURE_CREATIONFLAG_STORAGE for storage textures, for eg) |
| `useSRGBBuffer` | `boolean` | `false` | defines if the texture must be loaded in a sRGB GPU buffer (if supported by the GPU). |

#### Returns

[`InternalTexture`](InternalTexture.md)

the raw texture inside an InternalTexture

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:4263

▸ **createRawTexture**(`data`, `width`, `height`, `format`, `generateMipMaps`, `invertY`, `samplingMode`, `compression`, `type`, `creationFlags?`, `useSRGBBuffer?`): [`InternalTexture`](InternalTexture.md)

Creates a raw texture

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | [`Nullable`](../modules.md#nullable)`ArrayBufferView` | defines the data to store in the texture |
| `width` | `number` | defines the width of the texture |
| `height` | `number` | defines the height of the texture |
| `format` | `number` | defines the format of the data |
| `generateMipMaps` | `boolean` | defines if the engine should generate the mip levels |
| `invertY` | `boolean` | defines if data must be stored with Y axis inverted |
| `samplingMode` | `number` | defines the required sampling mode (Texture.NEAREST_SAMPLINGMODE by default) |
| `compression` | [`Nullable`](../modules.md#nullable)`string` | defines the compression used (null by default) |
| `type` | `number` | defines the type fo the data (Engine.TEXTURETYPE_UNSIGNED_INT by default) |
| `creationFlags?` | `number` | specific flags to use when creating the texture (Constants.TEXTURE_CREATIONFLAG_STORAGE for storage textures, for eg) |
| `useSRGBBuffer?` | `boolean` | defines if the texture must be loaded in a sRGB GPU buffer (if supported by the GPU). |

#### Returns

[`InternalTexture`](InternalTexture.md)

the raw texture inside an InternalTexture

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.rawTexture.ts:27

___

### createRawTexture2DArray

▸ **createRawTexture2DArray**(`data`, `width`, `height`, `depth`, `format`, `generateMipMaps`, `invertY`, `samplingMode`, `compression?`, `textureType?`): [`InternalTexture`](InternalTexture.md)

Creates a new raw 2D array texture

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `data` | [`Nullable`](../modules.md#nullable)`ArrayBufferView` | `undefined` | defines the data used to create the texture |
| `width` | `number` | `undefined` | defines the width of the texture |
| `height` | `number` | `undefined` | defines the height of the texture |
| `depth` | `number` | `undefined` | defines the number of layers of the texture |
| `format` | `number` | `undefined` | defines the format of the texture |
| `generateMipMaps` | `boolean` | `undefined` | defines if the engine must generate mip levels |
| `invertY` | `boolean` | `undefined` | defines if data must be stored with Y axis inverted |
| `samplingMode` | `number` | `undefined` | defines the required sampling mode (like Texture.NEAREST_SAMPLINGMODE) |
| `compression` | [`Nullable`](../modules.md#nullable)`string` | `null` | defines the compressed used (can be null) |
| `textureType` | `number` | `Constants.TEXTURETYPE_UNSIGNED_INT` | defines the compressed used (can be null) |

#### Returns

[`InternalTexture`](InternalTexture.md)

a new raw 2D array texture (stored in an InternalTexture)

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:4347

▸ **createRawTexture2DArray**(`data`, `width`, `height`, `depth`, `format`, `generateMipMaps`, `invertY`, `samplingMode`, `compression`, `textureType`, `creationFlags?`): [`InternalTexture`](InternalTexture.md)

Creates a new raw 2D array texture

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | [`Nullable`](../modules.md#nullable)`ArrayBufferView` | defines the data used to create the texture |
| `width` | `number` | defines the width of the texture |
| `height` | `number` | defines the height of the texture |
| `depth` | `number` | defines the number of layers of the texture |
| `format` | `number` | defines the format of the texture |
| `generateMipMaps` | `boolean` | defines if the engine must generate mip levels |
| `invertY` | `boolean` | defines if data must be stored with Y axis inverted |
| `samplingMode` | `number` | defines the required sampling mode (like Texture.NEAREST_SAMPLINGMODE) |
| `compression` | [`Nullable`](../modules.md#nullable)`string` | defines the compressed used (can be null) |
| `textureType` | `number` | defines the compressed used (can be null) |
| `creationFlags?` | `number` | specific flags to use when creating the texture (Constants.TEXTURE_CREATIONFLAG_STORAGE for storage textures, for eg) |

#### Returns

[`InternalTexture`](InternalTexture.md)

a new raw 2D array texture (stored in an InternalTexture)

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.rawTexture.ts:248

___

### createRawTexture3D

▸ **createRawTexture3D**(`data`, `width`, `height`, `depth`, `format`, `generateMipMaps`, `invertY`, `samplingMode`, `compression?`, `textureType?`): [`InternalTexture`](InternalTexture.md)

Creates a new raw 3D texture

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `data` | [`Nullable`](../modules.md#nullable)`ArrayBufferView` | `undefined` | defines the data used to create the texture |
| `width` | `number` | `undefined` | defines the width of the texture |
| `height` | `number` | `undefined` | defines the height of the texture |
| `depth` | `number` | `undefined` | defines the depth of the texture |
| `format` | `number` | `undefined` | defines the format of the texture |
| `generateMipMaps` | `boolean` | `undefined` | defines if the engine must generate mip levels |
| `invertY` | `boolean` | `undefined` | defines if data must be stored with Y axis inverted |
| `samplingMode` | `number` | `undefined` | defines the required sampling mode (like Texture.NEAREST_SAMPLINGMODE) |
| `compression` | [`Nullable`](../modules.md#nullable)`string` | `null` | defines the compressed used (can be null) |
| `textureType` | `number` | `Constants.TEXTURETYPE_UNSIGNED_INT` | defines the compressed used (can be null) |

#### Returns

[`InternalTexture`](InternalTexture.md)

a new raw 3D texture (stored in an InternalTexture)

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:4318

▸ **createRawTexture3D**(`data`, `width`, `height`, `depth`, `format`, `generateMipMaps`, `invertY`, `samplingMode`, `compression`, `textureType`, `creationFlags?`): [`InternalTexture`](InternalTexture.md)

Creates a new raw 3D texture

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | [`Nullable`](../modules.md#nullable)`ArrayBufferView` | defines the data used to create the texture |
| `width` | `number` | defines the width of the texture |
| `height` | `number` | defines the height of the texture |
| `depth` | `number` | defines the depth of the texture |
| `format` | `number` | defines the format of the texture |
| `generateMipMaps` | `boolean` | defines if the engine must generate mip levels |
| `invertY` | `boolean` | defines if data must be stored with Y axis inverted |
| `samplingMode` | `number` | defines the required sampling mode (like Texture.NEAREST_SAMPLINGMODE) |
| `compression` | [`Nullable`](../modules.md#nullable)`string` | defines the compressed used (can be null) |
| `textureType` | `number` | defines the compressed used (can be null) |
| `creationFlags?` | `number` | specific flags to use when creating the texture (Constants.TEXTURE_CREATIONFLAG_STORAGE for storage textures, for eg) |

#### Returns

[`InternalTexture`](InternalTexture.md)

a new raw 3D texture (stored in an InternalTexture)

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.rawTexture.ts:199

___

### createRenderTargetCubeTexture

▸ **createRenderTargetCubeTexture**(`size`, `options?`): [`RenderTargetWrapper`](RenderTargetWrapper.md)

Creates a new render target cube wrapper

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `size` | `number` | defines the size of the texture |
| `options?` | `Partial``RenderTargetCreationOptions` | defines the options used to create the texture |

#### Returns

[`RenderTargetWrapper`](RenderTargetWrapper.md)

a new render target cube wrapper

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.renderTargetCube.ts:17

___

### createRenderTargetTexture

▸ **createRenderTargetTexture**(`size`, `options`): [`RenderTargetWrapper`](RenderTargetWrapper.md)

Creates a new render target texture

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `size` | `TextureSize` | defines the size of the texture |
| `options` | `boolean` \| `RenderTargetCreationOptions` | defines the options used to create the texture |

#### Returns

[`RenderTargetWrapper`](RenderTargetWrapper.md)

a new render target wrapper ready to render texture

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.renderTarget.ts:26

___

### createShaderProgram

▸ **createShaderProgram**(`pipelineContext`, `vertexCode`, `fragmentCode`, `defines`, `context?`, `transformFeedbackVaryings?`): `WebGLProgram`

Creates a webGL program

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `pipelineContext` | [`IPipelineContext`](../interfaces/IPipelineContext.md) | `undefined` | defines the pipeline context to attach to |
| `vertexCode` | `string` | `undefined` | defines the vertex shader code to use |
| `fragmentCode` | `string` | `undefined` | defines the fragment shader code to use |
| `defines` | [`Nullable`](../modules.md#nullable)`string` | `undefined` | defines the string containing the defines to use to compile the shaders |
| `context?` | `WebGLRenderingContext` | `undefined` | defines the webGL context to use (if not set, the current one will be used) |
| `transformFeedbackVaryings` | [`Nullable`](../modules.md#nullable)`string`[] | `null` | defines the list of transform feedback varyings to use |

#### Returns

`WebGLProgram`

the new webGL program

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2910

___

### createStorageBuffer

▸ **createStorageBuffer**(`data`, `creationFlags`): [`DataBuffer`](DataBuffer.md)

Creates a storage buffer

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `number` \| [`DataArray`](../modules.md#dataarray) | the data for the storage buffer or the size of the buffer |
| `creationFlags` | `number` | flags to use when creating the buffer (see Constants.BUFFER_CREATIONFLAG_XXX). The BUFFER_CREATIONFLAG_STORAGE flag will be automatically added |

#### Returns

[`DataBuffer`](DataBuffer.md)

the new buffer

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.storageBuffer.ts:15

___

### createTexture

▸ **createTexture**(`url`, `noMipmap`, `invertY`, `scene`, `samplingMode?`, `onLoad?`, `onError?`, `buffer?`, `fallback?`, `format?`, `forcedExtension?`, `mimeType?`, `loaderOptions?`, `creationFlags?`, `useSRGBBuffer?`): [`InternalTexture`](InternalTexture.md)

Usually called from Texture.ts.
Passed information to create a WebGLTexture

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `url` | [`Nullable`](../modules.md#nullable)`string` | `undefined` | defines a value which contains one of the following:  * A conventional http URL, e.g. 'http://...' or 'file://...'  * A base64 string of in-line texture data, e.g. 'data:image/jpg;base64,/...'  * An indicator that data being passed using the buffer parameter, e.g. 'data:mytexture.jpg' |
| `noMipmap` | `boolean` | `undefined` | defines a boolean indicating that no mipmaps shall be generated.  Ignored for compressed textures.  They must be in the file |
| `invertY` | `boolean` | `undefined` | when true, image is flipped when loaded.  You probably want true. Certain compressed textures may invert this if their default is inverted (eg. ktx) |
| `scene` | [`Nullable`](../modules.md#nullable)`ISceneLike` | `undefined` | needed for loading to the correct scene |
| `samplingMode` | `number` | `Constants.TEXTURE_TRILINEAR_SAMPLINGMODE` | mode with should be used sample / access the texture (Default: Texture.TRILINEAR_SAMPLINGMODE) |
| `onLoad` | [`Nullable`](../modules.md#nullable)(`texture`: [`InternalTexture`](InternalTexture.md)) => `void` | `null` | optional callback to be called upon successful completion |
| `onError` | [`Nullable`](../modules.md#nullable)(`message`: `string`, `exception`: `any`) => `void` | `null` | optional callback to be called upon failure |
| `buffer` | [`Nullable`](../modules.md#nullable)`string` \| `ArrayBuffer` \| `ArrayBufferView` \| `Blob` \| `HTMLImageElement` \| `ImageBitmap` | `null` | a source of a file previously fetched as either a base64 string, an ArrayBuffer (compressed or image format), HTMLImageElement (image format), or a Blob |
| `fallback` | [`Nullable`](../modules.md#nullable)[`InternalTexture`](InternalTexture.md) | `null` | an internal argument in case the function must be called again, due to etc1 not having alpha capabilities |
| `format` | [`Nullable`](../modules.md#nullable)`number` | `null` | internal format.  Default: RGB when extension is '.jpg' else RGBA.  Ignored for compressed textures |
| `forcedExtension` | [`Nullable`](../modules.md#nullable)`string` | `null` | defines the extension to use to pick the right loader |
| `mimeType?` | `string` | `undefined` | defines an optional mime type |
| `loaderOptions?` | `any` | `undefined` | options to be passed to the loader |
| `creationFlags?` | `number` | `undefined` | specific flags to use when creating the texture (Constants.TEXTURE_CREATIONFLAG_STORAGE for storage textures, for eg) |
| `useSRGBBuffer?` | `boolean` | `undefined` | defines if the texture must be loaded in a sRGB GPU buffer (if supported by the GPU). |

#### Returns

[`InternalTexture`](InternalTexture.md)

a InternalTexture for assignment back into BABYLON.Texture

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:4124

___

### createUniformBuffer

▸ **createUniformBuffer**(`elements`): [`DataBuffer`](DataBuffer.md)

Create an uniform buffer

**`See`**

https://doc.babylonjs.com/features/webgl2#uniform-buffer-objets

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `elements` | [`FloatArray`](../modules.md#floatarray) | defines the content of the uniform buffer |

#### Returns

[`DataBuffer`](DataBuffer.md)

the webGL uniform buffer

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.uniformBuffer.ts:16

___

### createVertexBuffer

▸ **createVertexBuffer**(`data`): [`DataBuffer`](DataBuffer.md)

Creates a vertex buffer

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | [`DataArray`](../modules.md#dataarray) | the data for the vertex buffer |

#### Returns

[`DataBuffer`](DataBuffer.md)

the new WebGL static buffer

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2057

___

### disableAttributeByIndex

▸ **disableAttributeByIndex**(`attributeLocation`): `void`

Disable the attribute corresponding to the location in parameter

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `attributeLocation` | `number` | defines the attribute location of the attribute to disable |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2586

___

### disableInstanceAttribute

▸ **disableInstanceAttribute**(`attributeLocation`): `void`

Disable the instance attribute corresponding to the location in parameter

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `attributeLocation` | `number` | defines the attribute location of the attribute to disable |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2565

___

### disableInstanceAttributeByName

▸ **disableInstanceAttributeByName**(`name`): `void`

Disable the instance attribute corresponding to the name in parameter

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the name of the attribute to disable |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2552

___

### dispose

▸ **dispose**(): `void`

Dispose and release all associated resources

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:5263

___

### draw

▸ **draw**(`useTriangles`, `indexStart`, `indexCount`, `instancesCount?`): `void`

Send a draw order

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `useTriangles` | `boolean` | defines if triangles must be used to draw (else wireframe will be used) |
| `indexStart` | `number` | defines the starting index |
| `indexCount` | `number` | defines the number of index to draw |
| `instancesCount?` | `number` | defines the number of instances to draw (if instantiation is enabled) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2599

___

### drawArraysType

▸ **drawArraysType**(`fillMode`, `verticesStart`, `verticesCount`, `instancesCount?`): `void`

Draw a list of unindexed primitives

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fillMode` | `number` | defines the primitive to use |
| `verticesStart` | `number` | defines the index of first vertex to draw |
| `verticesCount` | `number` | defines the count of vertices to draw |
| `instancesCount?` | `number` | defines the number of instances to draw (if instantiation is enabled) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2656

___

### drawElementsType

▸ **drawElementsType**(`fillMode`, `indexStart`, `indexCount`, `instancesCount?`): `void`

Draw a list of indexed primitives

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fillMode` | `number` | defines the primitive to use |
| `indexStart` | `number` | defines the starting index |
| `indexCount` | `number` | defines the number of index to draw |
| `instancesCount?` | `number` | defines the number of instances to draw (if instantiation is enabled) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2631

___

### drawPointClouds

▸ **drawPointClouds**(`verticesStart`, `verticesCount`, `instancesCount?`): `void`

Draw a list of points

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `verticesStart` | `number` | defines the index of first vertex to draw |
| `verticesCount` | `number` | defines the count of vertices to draw |
| `instancesCount?` | `number` | defines the number of instances to draw (if instantiation is enabled) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2609

___

### drawUnIndexed

▸ **drawUnIndexed**(`useTriangles`, `verticesStart`, `verticesCount`, `instancesCount?`): `void`

Draw a list of unindexed primitives

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `useTriangles` | `boolean` | defines if triangles must be used to draw (else wireframe will be used) |
| `verticesStart` | `number` | defines the index of first vertex to draw |
| `verticesCount` | `number` | defines the count of vertices to draw |
| `instancesCount?` | `number` | defines the number of instances to draw (if instantiation is enabled) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2620

___

### enableEffect

▸ **enableEffect**(`effect`): `void`

Activates an effect, making it the current one (ie. the one used for rendering)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `effect` | [`Nullable`](../modules.md#nullable)[`Effect`](Effect.md) \| `DrawWrapper` | defines the effect to activate |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:3174

___

### endFrame

▸ **endFrame**(): `void`

Enf the current frame

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1737

___

### flushFramebuffer

▸ **flushFramebuffer**(): `void`

Force a webGL flush (ie. a flush of all waiting webGL commands)

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2024

___

### generateMipmaps

▸ **generateMipmaps**(`texture`): `void`

Generates the mipmaps for a texture

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `texture` | [`InternalTexture`](InternalTexture.md) | texture to generate the mipmaps for |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1976

___

### getAlphaEquation

▸ **getAlphaEquation**(): `number`

Gets the current alpha equation.

#### Returns

`number`

the current alpha equation

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.alpha.ts:40

___

### getAlphaMode

▸ **getAlphaMode**(): `number`

Gets the current alpha mode

**`See`**

https://doc.babylonjs.com/resources/transparency_and_how_meshes_are_rendered

#### Returns

`number`

the current alpha mode

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.alpha.ts:28

___

### getAttributes

▸ **getAttributes**(`pipelineContext`, `attributesNames`): `number`[]

Gets the list of active attributes for a given webGL program

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `pipelineContext` | [`IPipelineContext`](../interfaces/IPipelineContext.md) | defines the pipeline context to use |
| `attributesNames` | `string`[] | defines the list of attribute names to get |

#### Returns

`number`[]

an array of indices indicating the offset of each attribute

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:3155

___

### getAudioContext

▸ **getAudioContext**(): [`Nullable`](../modules.md#nullable)`AudioContext`

Gets the audio context specified in engine initialization options

#### Returns

[`Nullable`](../modules.md#nullable)`AudioContext`

an Audio Context

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1573

___

### getAudioDestination

▸ **getAudioDestination**(): [`Nullable`](../modules.md#nullable)`AudioDestinationNode` \| `MediaStreamAudioDestinationNode`

Gets the audio destination specified in engine initialization options

#### Returns

[`Nullable`](../modules.md#nullable)`AudioDestinationNode` \| `MediaStreamAudioDestinationNode`

an audio destination node

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1581

___

### getCaps

▸ **getCaps**(): [`EngineCapabilities`](../interfaces/EngineCapabilities.md)

Gets the object containing all engine capabilities

#### Returns

[`EngineCapabilities`](../interfaces/EngineCapabilities.md)

the EngineCapabilities object

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1510

___

### getClassName

▸ **getClassName**(): `string`

Gets a string identifying the name of the class

#### Returns

`string`

"Engine" string

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1418

___

### getColorWrite

▸ **getColorWrite**(): `boolean`

Gets a boolean indicating if color writing is enabled

#### Returns

`boolean`

the current color writing state

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:3539

___

### getCreationOptions

▸ **getCreationOptions**(): [`EngineOptions`](../interfaces/EngineOptions.md)

Gets the options used for engine creation

#### Returns

[`EngineOptions`](../interfaces/EngineOptions.md)

EngineOptions object

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:384

___

### getDepthBuffer

▸ **getDepthBuffer**(): `boolean`

Gets a boolean indicating if depth testing is enabled

#### Returns

`boolean`

the current state

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1910

___

### getError

▸ **getError**(): `number`

Get the current error code of the webGL context

**`See`**

https://developer.mozilla.org/en-US/docs/Web/API/WebGLRenderingContext/getError

#### Returns

`number`

the error code

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:5348

___

### getGlInfo

▸ **getGlInfo**(): `Object`

Gets an object containing information about the current webGL context

#### Returns

`Object`

an object containing the vendor, the renderer and the version of the current webGL context

| Name | Type |
| :------ | :------ |
| `renderer` | `string` |
| `vendor` | `string` |
| `version` | `string` |

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1469

___

### getHardwareScalingLevel

▸ **getHardwareScalingLevel**(): `number`

Gets the current hardware scaling level.
By default the hardware scaling level is computed from the window device ratio.
if level = 1 then the engine will render at the exact resolution of the canvas. If level = 0.5 then the engine will render at twice the size of the canvas.

#### Returns

`number`

a number indicating the current hardware scaling level

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1494

___

### getHostDocument

▸ **getHostDocument**(): [`Nullable`](../modules.md#nullable)`Document`

Gets host document

#### Returns

[`Nullable`](../modules.md#nullable)`Document`

the host document object

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:5957

___

### getHostWindow

▸ **getHostWindow**(): [`Nullable`](../modules.md#nullable)`Window`

Gets host window

#### Returns

[`Nullable`](../modules.md#nullable)`Window`

the host window object

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1589

___

### getInfo

▸ **getInfo**(): `Object`

Gets an object containing information about the current engine context

#### Returns

`Object`

an object containing the vendor, the renderer and the version of the current engine context

| Name | Type |
| :------ | :------ |
| `renderer` | `string` |
| `vendor` | `string` |
| `version` | `string` |

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1461

___

### getLoadedTexturesCache

▸ **getLoadedTexturesCache**(): [`InternalTexture`](InternalTexture.md)[]

Gets the list of loaded textures

#### Returns

[`InternalTexture`](InternalTexture.md)[]

an array containing all loaded textures

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1502

___

### getRenderHeight

▸ **getRenderHeight**(`useScreen?`): `number`

Gets the current render height

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `useScreen` | `boolean` | `false` | defines if screen size must be used (or the current render target if any) |

#### Returns

`number`

a number defining the current render height

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1619

___

### getRenderWidth

▸ **getRenderWidth**(`useScreen?`): `number`

Gets the current render width

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `useScreen` | `boolean` | `false` | defines if screen size must be used (or the current render target if any) |

#### Returns

`number`

a number defining the current render width

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1606

___

### getRenderingCanvas

▸ **getRenderingCanvas**(): [`Nullable`](../modules.md#nullable)`HTMLCanvasElement`

Gets the HTML canvas attached with the current webGL context

#### Returns

[`Nullable`](../modules.md#nullable)`HTMLCanvasElement`

a HTML canvas

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1565

___

### getUniforms

▸ **getUniforms**(`pipelineContext`, `uniformsNames`): [`Nullable`](../modules.md#nullable)`WebGLUniformLocation`[]

Gets the list of webGL uniform locations associated with a specific program based on a list of uniform names

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `pipelineContext` | [`IPipelineContext`](../interfaces/IPipelineContext.md) | defines the pipeline context to use |
| `uniformsNames` | `string`[] | defines the list of uniform names |

#### Returns

[`Nullable`](../modules.md#nullable)`WebGLUniformLocation`[]

an array of webGL uniform locations

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:3138

___

### getZOffset

▸ **getZOffset**(): `number`

Gets the current value of the zOffset Factor

#### Returns

`number`

the current zOffset Factor state

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1934

___

### getZOffsetUnits

▸ **getZOffsetUnits**(): `number`

Gets the current value of the zOffset Units

#### Returns

`number`

the current zOffset Units state

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1951

___

### inlineShaderCode

▸ **inlineShaderCode**(`code`): `string`

Inline functions in shader code that are marked to be inlined

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `code` | `string` | code to inline |

#### Returns

`string`

inlined code

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2932

___

### readFromStorageBuffer

▸ **readFromStorageBuffer**(`storageBuffer`, `offset?`, `size?`, `buffer?`): `Promise``ArrayBufferView`

Read data from a storage buffer

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `storageBuffer` | [`DataBuffer`](DataBuffer.md) | The storage buffer to read from |
| `offset?` | `number` | The offset in the storage buffer to start reading from (default: 0) |
| `size?` | `number` | The number of bytes to read from the storage buffer (default: capacity of the buffer) |
| `buffer?` | `ArrayBufferView` | The buffer to write the data we have read from the storage buffer to (optional) |

#### Returns

`Promise``ArrayBufferView`

If not undefined, returns the (promise) buffer (as provided by the 4th parameter) filled with the data, else it returns a (promise) Uint8Array with the data read from the storage buffer

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.storageBuffer.ts:34

___

### readPixels

▸ **readPixels**(`x`, `y`, `width`, `height`, `hasAlpha?`, `flushRenderer?`): `Promise``ArrayBufferView`

Reads pixels from the current frame buffer. Please note that this function can be slow

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `x` | `number` | `undefined` | defines the x coordinate of the rectangle where pixels must be read |
| `y` | `number` | `undefined` | defines the y coordinate of the rectangle where pixels must be read |
| `width` | `number` | `undefined` | defines the width of the rectangle where pixels must be read |
| `height` | `number` | `undefined` | defines the height of the rectangle where pixels must be read |
| `hasAlpha` | `boolean` | `true` | defines whether the output should have alpha or not (defaults to true) |
| `flushRenderer` | `boolean` | `true` | true to flush the renderer from the pending commands before reading the pixels |

#### Returns

`Promise``ArrayBufferView`

a ArrayBufferView promise (Uint8Array) containing RGBA colors

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:5775

___

### recordVertexArrayObject

▸ **recordVertexArrayObject**(`vertexBuffers`, `indexBuffer`, `effect`, `overrideVertexBuffers?`): `WebGLVertexArrayObject`

Records a vertex array object

**`See`**

https://doc.babylonjs.com/features/webgl2#vertex-array-objects

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vertexBuffers` | `Object` | defines the list of vertex buffers to store |
| `indexBuffer` | [`Nullable`](../modules.md#nullable)[`DataBuffer`](DataBuffer.md) | defines the index buffer to store |
| `effect` | [`Effect`](Effect.md) | defines the effect to store |
| `overrideVertexBuffers?` | `Object` | defines optional list of avertex buffers that overrides the entries in vertexBuffers |

#### Returns

`WebGLVertexArrayObject`

the new vertex array object

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2322

___

### releaseComputeEffects

▸ **releaseComputeEffects**(): `void`

Forces the engine to release all cached compute effects. This means that next effect compilation will have to be done completely even if a similar effect was already compiled

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.computeShader.ts:84

___

### releaseEffects

▸ **releaseEffects**(): `void`

Force the engine to release all cached effects. This means that next effect compilation will have to be done completely even if a similar effect was already compiled

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:5251

___

### releaseVertexArrayObject

▸ **releaseVertexArrayObject**(`vao`): `void`

Release and free the memory of a vertex array object

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vao` | `WebGLVertexArrayObject` | defines the vertex array object to delete |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2455

___

### resetTextureCache

▸ **resetTextureCache**(): `void`

Reset the texture cache to empty state

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1446

___

### resize

▸ **resize**(`forceSetSize?`): `void`

Resize the view according to the canvas' size

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `forceSetSize` | `boolean` | `false` | true to force setting the sizes of the underlying canvas |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1749

___

### restoreDefaultFramebuffer

▸ **restoreDefaultFramebuffer**(): `void`

Unbind the current render target and bind the default framebuffer

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2031

___

### restoreSingleAttachment

▸ **restoreSingleAttachment**(): `void`

Restores the webgl state to only draw on the main color attachment
when the frame buffer associated is the canvas frame buffer

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.multiRender.ts:60

___

### restoreSingleAttachmentForRenderTarget

▸ **restoreSingleAttachmentForRenderTarget**(): `void`

Restores the webgl state to only draw on the main color attachment
when the frame buffer associated is not the canvas frame buffer

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.multiRender.ts:66

___

### runRenderLoop

▸ **runRenderLoop**(`renderFunction`): `void`

Register and execute a render loop. The engine can have more than one render function

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `renderFunction` | () => `void` | defines the function to continuously execute |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1641

___

### setAlphaConstants

▸ **setAlphaConstants**(`r`, `g`, `b`, `a`): `void`

Sets alpha constants used by some alpha blending modes

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `r` | `number` | defines the red component |
| `g` | `number` | defines the green component |
| `b` | `number` | defines the blue component |
| `a` | `number` | defines the alpha component |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.alpha.ts:13

___

### setAlphaEquation

▸ **setAlphaEquation**(`equation`): `void`

Sets the current alpha equation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `equation` | `number` | defines the equation to use (one of the Engine.ALPHA_EQUATION_XXX) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.alpha.ts:34

___

### setAlphaMode

▸ **setAlphaMode**(`mode`, `noDepthWriteChange?`): `void`

Sets the current alpha mode

**`See`**

https://doc.babylonjs.com/resources/transparency_and_how_meshes_are_rendered

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mode` | `number` | defines the mode to use (one of the Engine.ALPHA_XXX) |
| `noDepthWriteChange?` | `boolean` | defines if depth writing state should remains unchanged (false by default) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.alpha.ts:21

___

### setArray

▸ **setArray**(`uniform`, `array`): `boolean`

Set the value of an uniform to an array of number

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniform` | [`Nullable`](../modules.md#nullable)`WebGLUniformLocation` | defines the webGL uniform location where to store the value |
| `array` | `number`[] \| `Float32Array` | defines the array of number to store |

#### Returns

`boolean`

true if the value was set

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:3335

___

### setArray2

▸ **setArray2**(`uniform`, `array`): `boolean`

Set the value of an uniform to an array of number (stored as vec2)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniform` | [`Nullable`](../modules.md#nullable)`WebGLUniformLocation` | defines the webGL uniform location where to store the value |
| `array` | `number`[] \| `Float32Array` | defines the array of number to store |

#### Returns

`boolean`

true if the value was set

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:3353

___

### setArray3

▸ **setArray3**(`uniform`, `array`): `boolean`

Set the value of an uniform to an array of number (stored as vec3)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniform` | [`Nullable`](../modules.md#nullable)`WebGLUniformLocation` | defines the webGL uniform location where to store the value |
| `array` | `number`[] \| `Float32Array` | defines the array of number to store |

#### Returns

`boolean`

true if the value was set

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:3368

___

### setArray4

▸ **setArray4**(`uniform`, `array`): `boolean`

Set the value of an uniform to an array of number (stored as vec4)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniform` | [`Nullable`](../modules.md#nullable)`WebGLUniformLocation` | defines the webGL uniform location where to store the value |
| `array` | `number`[] \| `Float32Array` | defines the array of number to store |

#### Returns

`boolean`

true if the value was set

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:3383

___

### setColorWrite

▸ **setColorWrite**(`enable`): `void`

Enable or disable color writing

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `enable` | `boolean` | defines the state to set |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:3528

___

### setDepthBuffer

▸ **setDepthBuffer**(`enable`): `void`

Enable or disable depth buffering

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `enable` | `boolean` | defines the state to set |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1918

___

### setExternalTexture

▸ **setExternalTexture**(`name`, `texture`): `void`

Sets an internal texture to the according uniform.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | The name of the uniform in the effect |
| `texture` | [`Nullable`](../modules.md#nullable)[`ExternalTexture`](ExternalTexture.md) | The texture to apply |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.externalTexture.ts:19

___

### setFloat

▸ **setFloat**(`uniform`, `value`): `boolean`

Set the value of an uniform to a number (float)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniform` | [`Nullable`](../modules.md#nullable)`WebGLUniformLocation` | defines the webGL uniform location where to store the value |
| `value` | `number` | defines the float number to store |

#### Returns

`boolean`

true if the value was transferred

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:3443

___

### setFloat2

▸ **setFloat2**(`uniform`, `x`, `y`): `boolean`

Set the value of an uniform to a vec2

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniform` | [`Nullable`](../modules.md#nullable)`WebGLUniformLocation` | defines the webGL uniform location where to store the value |
| `x` | `number` | defines the 1st component of the value |
| `y` | `number` | defines the 2nd component of the value |

#### Returns

`boolean`

true if the value was set

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:3460

___

### setFloat3

▸ **setFloat3**(`uniform`, `x`, `y`, `z`): `boolean`

Set the value of an uniform to a vec3

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniform` | [`Nullable`](../modules.md#nullable)`WebGLUniformLocation` | defines the webGL uniform location where to store the value |
| `x` | `number` | defines the 1st component of the value |
| `y` | `number` | defines the 2nd component of the value |
| `z` | `number` | defines the 3rd component of the value |

#### Returns

`boolean`

true if the value was set

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:3478

___

### setFloat4

▸ **setFloat4**(`uniform`, `x`, `y`, `z`, `w`): `boolean`

Set the value of an uniform to a vec4

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniform` | [`Nullable`](../modules.md#nullable)`WebGLUniformLocation` | defines the webGL uniform location where to store the value |
| `x` | `number` | defines the 1st component of the value |
| `y` | `number` | defines the 2nd component of the value |
| `z` | `number` | defines the 3rd component of the value |
| `w` | `number` | defines the 4th component of the value |

#### Returns

`boolean`

true if the value was set

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:3497

___

### setHardwareScalingLevel

▸ **setHardwareScalingLevel**(`level`): `void`

Defines the hardware scaling level.
By default the hardware scaling level is computed from the window device ratio.
if level = 1 then the engine will render at the exact resolution of the canvas. If level = 0.5 then the engine will render at twice the size of the canvas.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `level` | `number` | defines the level to use |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1483

___

### setInt

▸ **setInt**(`uniform`, `value`): `boolean`

Set the value of an uniform to a number (int)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniform` | [`Nullable`](../modules.md#nullable)`WebGLUniformLocation` | defines the webGL uniform location where to store the value |
| `value` | `number` | defines the int number to store |

#### Returns

`boolean`

true if the value was set

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:3204

___

### setInt2

▸ **setInt2**(`uniform`, `x`, `y`): `boolean`

Set the value of an uniform to a int2

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniform` | [`Nullable`](../modules.md#nullable)`WebGLUniformLocation` | defines the webGL uniform location where to store the value |
| `x` | `number` | defines the 1st component of the value |
| `y` | `number` | defines the 2nd component of the value |

#### Returns

`boolean`

true if the value was set

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:3221

___

### setInt3

▸ **setInt3**(`uniform`, `x`, `y`, `z`): `boolean`

Set the value of an uniform to a int3

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniform` | [`Nullable`](../modules.md#nullable)`WebGLUniformLocation` | defines the webGL uniform location where to store the value |
| `x` | `number` | defines the 1st component of the value |
| `y` | `number` | defines the 2nd component of the value |
| `z` | `number` | defines the 3rd component of the value |

#### Returns

`boolean`

true if the value was set

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:3239

___

### setInt4

▸ **setInt4**(`uniform`, `x`, `y`, `z`, `w`): `boolean`

Set the value of an uniform to a int4

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniform` | [`Nullable`](../modules.md#nullable)`WebGLUniformLocation` | defines the webGL uniform location where to store the value |
| `x` | `number` | defines the 1st component of the value |
| `y` | `number` | defines the 2nd component of the value |
| `z` | `number` | defines the 3rd component of the value |
| `w` | `number` | defines the 4th component of the value |

#### Returns

`boolean`

true if the value was set

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:3258

___

### setIntArray

▸ **setIntArray**(`uniform`, `array`): `boolean`

Set the value of an uniform to an array of int32

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniform` | [`Nullable`](../modules.md#nullable)`WebGLUniformLocation` | defines the webGL uniform location where to store the value |
| `array` | `Int32Array` | defines the array of int32 to store |

#### Returns

`boolean`

true if the value was set

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:3274

___

### setIntArray2

▸ **setIntArray2**(`uniform`, `array`): `boolean`

Set the value of an uniform to an array of int32 (stored as vec2)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniform` | [`Nullable`](../modules.md#nullable)`WebGLUniformLocation` | defines the webGL uniform location where to store the value |
| `array` | `Int32Array` | defines the array of int32 to store |

#### Returns

`boolean`

true if the value was set

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:3290

___

### setIntArray3

▸ **setIntArray3**(`uniform`, `array`): `boolean`

Set the value of an uniform to an array of int32 (stored as vec3)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniform` | [`Nullable`](../modules.md#nullable)`WebGLUniformLocation` | defines the webGL uniform location where to store the value |
| `array` | `Int32Array` | defines the array of int32 to store |

#### Returns

`boolean`

true if the value was set

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:3305

___

### setIntArray4

▸ **setIntArray4**(`uniform`, `array`): `boolean`

Set the value of an uniform to an array of int32 (stored as vec4)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniform` | [`Nullable`](../modules.md#nullable)`WebGLUniformLocation` | defines the webGL uniform location where to store the value |
| `array` | `Int32Array` | defines the array of int32 to store |

#### Returns

`boolean`

true if the value was set

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:3320

___

### setMatrices

▸ **setMatrices**(`uniform`, `matrices`): `boolean`

Set the value of an uniform to an array of float32 (stored as matrices)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniform` | [`Nullable`](../modules.md#nullable)`WebGLUniformLocation` | defines the webGL uniform location where to store the value |
| `matrices` | `Float32Array` | defines the array of float32 to store |

#### Returns

`boolean`

true if the value was set

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:3398

___

### setMatrix2x2

▸ **setMatrix2x2**(`uniform`, `matrix`): `boolean`

Set the value of an uniform to a matrix (2x2)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniform` | [`Nullable`](../modules.md#nullable)`WebGLUniformLocation` | defines the webGL uniform location where to store the value |
| `matrix` | `Float32Array` | defines the Float32Array representing the 2x2 matrix to store |

#### Returns

`boolean`

true if the value was set

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:3428

___

### setMatrix3x3

▸ **setMatrix3x3**(`uniform`, `matrix`): `boolean`

Set the value of an uniform to a matrix (3x3)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniform` | [`Nullable`](../modules.md#nullable)`WebGLUniformLocation` | defines the webGL uniform location where to store the value |
| `matrix` | `Float32Array` | defines the Float32Array representing the 3x3 matrix to store |

#### Returns

`boolean`

true if the value was set

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:3413

___

### setSize

▸ **setSize**(`width`, `height`, `forceSetSize?`): `boolean`

Force a specific size of the canvas

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `width` | `number` | `undefined` | defines the new canvas' width |
| `height` | `number` | `undefined` | defines the new canvas' height |
| `forceSetSize` | `boolean` | `false` | true to force setting the sizes of the underlying canvas |

#### Returns

`boolean`

true if the size was changed

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1779

___

### setState

▸ **setState**(`culling`, `zOffset?`, `force?`, `reverseSide?`, `cullBackFaces?`, `stencil?`, `zOffsetUnits?`): `void`

Set various states to the webGL context

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `culling` | `boolean` | `undefined` | defines culling state: true to enable culling, false to disable it |
| `zOffset` | `number` | `0` | defines the value to apply to zOffset (0 by default) |
| `force?` | `boolean` | `undefined` | defines if states must be applied even if cache is up to date |
| `reverseSide` | `boolean` | `false` | defines if culling must be reversed (CCW if false, CW if true) |
| `cullBackFaces?` | `boolean` | `undefined` | true to cull back faces, false to cull front faces (if culling is enabled) |
| `stencil?` | `IStencilState` | `undefined` | stencil states to set |
| `zOffsetUnits` | `number` | `0` | defines the value to apply to zOffsetUnits (0 by default) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1881

___

### setStorageBuffer

▸ **setStorageBuffer**(`name`, `buffer`): `void`

Sets a storage buffer in the shader

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Defines the name of the storage buffer as defined in the shader |
| `buffer` | [`Nullable`](../modules.md#nullable)[`StorageBuffer`](StorageBuffer.md) | Defines the value to give to the uniform |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.storageBuffer.ts:41

___

### setTexture

▸ **setTexture**(`channel`, `uniform`, `texture`, `name`): `void`

Sets a texture to the according uniform.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `channel` | `number` | The texture channel |
| `uniform` | [`Nullable`](../modules.md#nullable)`WebGLUniformLocation` | The uniform to set |
| `texture` | [`Nullable`](../modules.md#nullable)[`ThinTexture`](ThinTexture.md) | The texture to apply |
| `name` | `string` | The name of the uniform in the effect |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:5029

___

### setTextureArray

▸ **setTextureArray**(`channel`, `uniform`, `textures`, `name`): `void`

Sets an array of texture to the webGL context

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `channel` | `number` | defines the channel where the texture array must be set |
| `uniform` | [`Nullable`](../modules.md#nullable)`WebGLUniformLocation` | defines the associated uniform location |
| `textures` | [`ThinTexture`](ThinTexture.md)[] | defines the array of textures to bind |
| `name` | `string` | name of the channel |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:5162

___

### setTextureSampler

▸ **setTextureSampler**(`name`, `sampler`): `void`

Sets a texture sampler to the according uniform.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | The name of the uniform in the effect |
| `sampler` | [`Nullable`](../modules.md#nullable)[`TextureSampler`](TextureSampler.md) | The sampler to apply |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.textureSampler.ts:13

___

### setViewport

▸ **setViewport**(`viewport`, `requiredWidth?`, `requiredHeight?`): `void`

Set the WebGL's viewport

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `viewport` | `IViewportLike` | defines the viewport element to be used |
| `requiredWidth?` | `number` | defines the width required for rendering. If not provided the rendering canvas' width is used |
| `requiredHeight?` | `number` | defines the height required for rendering. If not provided the rendering canvas' height is used |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1718

___

### setZOffset

▸ **setZOffset**(`value`): `void`

Set the z offset Factor to apply to current rendering

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `number` | defines the offset to apply |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1926

___

### setZOffsetUnits

▸ **setZOffsetUnits**(`value`): `void`

Set the z offset Units to apply to current rendering

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `number` | defines the offset to apply |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1943

___

### snapshotRenderingReset

▸ **snapshotRenderingReset**(): `void`

Creates a new snapshot at the next frame using the current snapshotRenderingMode

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:717

___

### stopRenderLoop

▸ **stopRenderLoop**(`renderFunction?`): `void`

stop executing a render loop function and remove it from the execution array

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `renderFunction?` | () => `void` | defines the function to be removed. If not provided all functions will be removed. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1518

___

### unBindFramebuffer

▸ **unBindFramebuffer**(`texture`, `disableGenerateMipMaps?`, `onBeforeUnbind?`): `void`

Unbind the current render target texture from the webGL context

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `texture` | [`RenderTargetWrapper`](RenderTargetWrapper.md) | `undefined` | defines the render target wrapper to unbind |
| `disableGenerateMipMaps` | `boolean` | `false` | defines a boolean indicating that mipmaps must not be generated |
| `onBeforeUnbind?` | () => `void` | `undefined` | defines a function which will be called before the effective unbind |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:1988

___

### unBindMultiColorAttachmentFramebuffer

▸ **unBindMultiColorAttachmentFramebuffer**(`rtWrapper`, `disableGenerateMipMaps`, `onBeforeUnbind?`): `void`

Unbind a list of render target textures from the webGL context
This is used only when drawBuffer extension or webGL2 are active

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `rtWrapper` | [`RenderTargetWrapper`](RenderTargetWrapper.md) | defines the render target wrapper to unbind |
| `disableGenerateMipMaps` | `boolean` | defines a boolean indicating that mipmaps must not be generated |
| `onBeforeUnbind?` | () => `void` | defines a function which will be called before the effective unbind |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.multiRender.ts:21

___

### unbindAllAttributes

▸ **unbindAllAttributes**(): `void`

Unbind all vertex attributes from the webGL context

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:5229

___

### unbindAllTextures

▸ **unbindAllTextures**(): `void`

Unbind all textures from the webGL context

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:5010

___

### unbindInstanceAttributes

▸ **unbindInstanceAttributes**(): `void`

Unbind all instance attributes

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2436

___

### updateAndBindInstancesBuffer

▸ **updateAndBindInstancesBuffer**(`instancesBuffer`, `data`, `offsetLocations`): `void`

Update the content of a webGL buffer used with instantiation and bind it to the webGL context

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `instancesBuffer` | [`DataBuffer`](DataBuffer.md) | defines the webGL buffer to update and bind |
| `data` | `Float32Array` | defines the data to store in the buffer |
| `offsetLocations` | `number`[] \| [`InstancingAttributeInfo`](../interfaces/InstancingAttributeInfo.md)[] | defines the offsets or attributes information used to determine where data must be stored in the buffer |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2484

___

### updateArrayBuffer

▸ **updateArrayBuffer**(`data`): `void`

update the bound buffer with the given data

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `Float32Array` | defines the data to update |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2191

___

### updateDynamicIndexBuffer

▸ **updateDynamicIndexBuffer**(`indexBuffer`, `indices`, `offset?`): `void`

Update a dynamic index buffer

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `indexBuffer` | [`DataBuffer`](DataBuffer.md) | defines the target index buffer |
| `indices` | [`IndicesArray`](../modules.md#indicesarray) | defines the data to update |
| `offset?` | `number` | defines the offset in the target index buffer where update should start |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.dynamicBuffer.ts:13

___

### updateDynamicTexture

▸ **updateDynamicTexture**(`texture`, `source`, `invertY?`, `premulAlpha?`, `format?`, `forceBindTexture?`, `allowGPUOptimization?`): `void`

Update the content of a dynamic texture

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `texture` | [`Nullable`](../modules.md#nullable)[`InternalTexture`](InternalTexture.md) | defines the texture to update |
| `source` | `HTMLCanvasElement` \| [`ICanvas`](../interfaces/ICanvas.md) \| `HTMLImageElement` \| `ImageBitmap` \| `OffscreenCanvas` \| `HTMLVideoElement` \| `ImageData` | defines the source containing the data |
| `invertY?` | `boolean` | defines if data must be stored with Y axis inverted |
| `premulAlpha?` | `boolean` | defines if alpha is stored as premultiplied |
| `format?` | `number` | defines the format of the data |
| `forceBindTexture?` | `boolean` | if the texture should be forced to be bound eg. after a graphics context loss (Default: false) |
| `allowGPUOptimization?` | `boolean` | true to allow some specific GPU optimizations (subject to engine feature "allowGPUOptimizationsForGUI" being true) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.dynamicTexture.ts:28

___

### updateDynamicVertexBuffer

▸ **updateDynamicVertexBuffer**(`vertexBuffer`, `data`, `byteOffset?`, `byteLength?`): `void`

Updates a dynamic vertex buffer.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vertexBuffer` | [`DataBuffer`](DataBuffer.md) | the vertex buffer to update |
| `data` | [`DataArray`](../modules.md#dataarray) | the data used to update the vertex buffer |
| `byteOffset?` | `number` | the byte offset of the data |
| `byteLength?` | `number` | the byte length of the data |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.dynamicBuffer.ts:22

___

### updateMultipleRenderTargetTextureSampleCount

▸ **updateMultipleRenderTargetTextureSampleCount**(`rtWrapper`, `samples`, `initializeBuffers?`): `number`

Update the sample count for a given multiple render target texture

**`See`**

https://doc.babylonjs.com/features/webgl2#multisample-render-targets

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `rtWrapper` | [`Nullable`](../modules.md#nullable)[`RenderTargetWrapper`](RenderTargetWrapper.md) | defines the render target wrapper to update |
| `samples` | `number` | defines the sample count to set |
| `initializeBuffers?` | `boolean` | if set to true, the engine will make an initializing call of drawBuffers |

#### Returns

`number`

the effective sample count (could be 0 if multisample render targets are not supported)

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.multiRender.ts:41

___

### updateRawCubeTexture

▸ **updateRawCubeTexture**(`texture`, `data`, `format`, `type`, `invertY`): `void`

Update a raw cube texture

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `texture` | [`InternalTexture`](InternalTexture.md) | defines the texture to update |
| `data` | `ArrayBufferView`[] | defines the data to store |
| `format` | `number` | defines the data format |
| `type` | `number` | defines the type fo the data (Engine.TEXTURETYPE_UNSIGNED_INT by default) |
| `invertY` | `boolean` | defines if data must be stored with Y axis inverted |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.rawTexture.ts:101

▸ **updateRawCubeTexture**(`texture`, `data`, `format`, `type`, `invertY`, `compression`): `void`

Update a raw cube texture

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `texture` | [`InternalTexture`](InternalTexture.md) | defines the texture to update |
| `data` | `ArrayBufferView`[] | defines the data to store |
| `format` | `number` | defines the data format |
| `type` | `number` | defines the type fo the data (Engine.TEXTURETYPE_UNSIGNED_INT by default) |
| `invertY` | `boolean` | defines if data must be stored with Y axis inverted |
| `compression` | [`Nullable`](../modules.md#nullable)`string` | defines the compression used (null by default) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.rawTexture.ts:112

▸ **updateRawCubeTexture**(`texture`, `data`, `format`, `type`, `invertY`, `compression`, `level`): `void`

Update a raw cube texture

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `texture` | [`InternalTexture`](InternalTexture.md) | defines the texture to update |
| `data` | `ArrayBufferView`[] | defines the data to store |
| `format` | `number` | defines the data format |
| `type` | `number` | defines the type fo the data (Engine.TEXTURETYPE_UNSIGNED_INT by default) |
| `invertY` | `boolean` | defines if data must be stored with Y axis inverted |
| `compression` | [`Nullable`](../modules.md#nullable)`string` | defines the compression used (null by default) |
| `level` | `number` | defines which level of the texture to update |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.rawTexture.ts:124

___

### updateRawTexture

▸ **updateRawTexture**(`texture`, `data`, `format`, `invertY`): `void`

Update a raw texture

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `texture` | [`Nullable`](../modules.md#nullable)[`InternalTexture`](InternalTexture.md) | defines the texture to update |
| `data` | [`Nullable`](../modules.md#nullable)`ArrayBufferView` | defines the data to store in the texture |
| `format` | `number` | defines the format of the data |
| `invertY` | `boolean` | defines if data must be stored with Y axis inverted |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.rawTexture.ts:48

▸ **updateRawTexture**(`texture`, `data`, `format`, `invertY`, `compression`, `type`, `useSRGBBuffer`): `void`

Update a raw texture

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `texture` | [`Nullable`](../modules.md#nullable)[`InternalTexture`](InternalTexture.md) | defines the texture to update |
| `data` | [`Nullable`](../modules.md#nullable)`ArrayBufferView` | defines the data to store in the texture |
| `format` | `number` | defines the format of the data |
| `invertY` | `boolean` | defines if data must be stored with Y axis inverted |
| `compression` | [`Nullable`](../modules.md#nullable)`string` | defines the compression used (null by default) |
| `type` | `number` | defines the type fo the data (Engine.TEXTURETYPE_UNSIGNED_INT by default) |
| `useSRGBBuffer` | `boolean` | defines if the texture must be loaded in a sRGB GPU buffer (if supported by the GPU). |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.rawTexture.ts:60

___

### updateRawTexture2DArray

▸ **updateRawTexture2DArray**(`texture`, `data`, `format`, `invertY`): `void`

Update a raw 2D array texture

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `texture` | [`InternalTexture`](InternalTexture.md) | defines the texture to update |
| `data` | [`Nullable`](../modules.md#nullable)`ArrayBufferView` | defines the data to store |
| `format` | `number` | defines the data format |
| `invertY` | `boolean` | defines if data must be stored with Y axis inverted |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.rawTexture.ts:269

▸ **updateRawTexture2DArray**(`texture`, `data`, `format`, `invertY`, `compression`, `textureType`): `void`

Update a raw 2D array texture

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `texture` | [`InternalTexture`](InternalTexture.md) | defines the texture to update |
| `data` | [`Nullable`](../modules.md#nullable)`ArrayBufferView` | defines the data to store |
| `format` | `number` | defines the data format |
| `invertY` | `boolean` | defines if data must be stored with Y axis inverted |
| `compression` | [`Nullable`](../modules.md#nullable)`string` | defines the used compression (can be null) |
| `textureType` | `number` | defines the texture Type (Engine.TEXTURETYPE_UNSIGNED_INT, Engine.TEXTURETYPE_FLOAT...) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.rawTexture.ts:280

___

### updateRawTexture3D

▸ **updateRawTexture3D**(`texture`, `data`, `format`, `invertY`): `void`

Update a raw 3D texture

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `texture` | [`InternalTexture`](InternalTexture.md) | defines the texture to update |
| `data` | [`Nullable`](../modules.md#nullable)`ArrayBufferView` | defines the data to store |
| `format` | `number` | defines the data format |
| `invertY` | `boolean` | defines if data must be stored with Y axis inverted |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.rawTexture.ts:220

▸ **updateRawTexture3D**(`texture`, `data`, `format`, `invertY`, `compression`, `textureType`): `void`

Update a raw 3D texture

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `texture` | [`InternalTexture`](InternalTexture.md) | defines the texture to update |
| `data` | [`Nullable`](../modules.md#nullable)`ArrayBufferView` | defines the data to store |
| `format` | `number` | defines the data format |
| `invertY` | `boolean` | defines if data must be stored with Y axis inverted |
| `compression` | [`Nullable`](../modules.md#nullable)`string` | defines the used compression (can be null) |
| `textureType` | `number` | defines the texture Type (Engine.TEXTURETYPE_UNSIGNED_INT, Engine.TEXTURETYPE_FLOAT...) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.rawTexture.ts:231

___

### updateRenderTargetTextureSampleCount

▸ **updateRenderTargetTextureSampleCount**(`rtWrapper`, `samples`): `number`

Updates the sample count of a render target texture

**`See`**

https://doc.babylonjs.com/features/webgl2#multisample-render-targets

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `rtWrapper` | [`Nullable`](../modules.md#nullable)[`RenderTargetWrapper`](RenderTargetWrapper.md) | defines the render target wrapper to update |
| `samples` | `number` | defines the sample count to set |

#### Returns

`number`

the effective sample count (could be 0 if multisample render targets are not supported)

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.renderTarget.ts:45

___

### updateStorageBuffer

▸ **updateStorageBuffer**(`buffer`, `data`, `byteOffset?`, `byteLength?`): `void`

Updates a storage buffer

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `buffer` | [`DataBuffer`](DataBuffer.md) | the storage buffer to update |
| `data` | [`DataArray`](../modules.md#dataarray) | the data used to update the storage buffer |
| `byteOffset?` | `number` | the byte offset of the data |
| `byteLength?` | `number` | the byte length of the data |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.storageBuffer.ts:24

___

### updateTextureData

▸ **updateTextureData**(`texture`, `imageData`, `xOffset`, `yOffset`, `width`, `height`, `faceIndex?`, `lod?`, `generateMipMaps?`): `void`

Update a portion of an internal texture

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `texture` | [`InternalTexture`](InternalTexture.md) | `undefined` | defines the texture to update |
| `imageData` | `ArrayBufferView` | `undefined` | defines the data to store into the texture |
| `xOffset` | `number` | `undefined` | defines the x coordinates of the update rectangle |
| `yOffset` | `number` | `undefined` | defines the y coordinates of the update rectangle |
| `width` | `number` | `undefined` | defines the width of the update rectangle |
| `height` | `number` | `undefined` | defines the height of the update rectangle |
| `faceIndex` | `number` | `0` | defines the face index if texture is a cube (0 by default) |
| `lod` | `number` | `0` | defines the lod level to update (0 by default) |
| `generateMipMaps` | `boolean` | `false` | defines whether to generate mipmaps or not |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:4650

___

### updateTextureDimensions

▸ **updateTextureDimensions**(`texture`, `width`, `height`, `depth?`): `void`

Update the dimensions of a texture

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `texture` | [`InternalTexture`](InternalTexture.md) | `undefined` | texture to update |
| `width` | `number` | `undefined` | new width of the texture |
| `height` | `number` | `undefined` | new height of the texture |
| `depth` | `number` | `1` | new depth of the texture |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:4431

___

### updateTextureSamplingMode

▸ **updateTextureSamplingMode**(`samplingMode`, `texture`, `generateMipMaps?`): `void`

Update the sampling mode of a given texture

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `samplingMode` | `number` | `undefined` | defines the required sampling mode |
| `texture` | [`InternalTexture`](InternalTexture.md) | `undefined` | defines the texture to update |
| `generateMipMaps` | `boolean` | `false` | defines whether to generate mipmaps for the texture |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:4407

___

### updateTextureWrappingMode

▸ **updateTextureWrappingMode**(`texture`, `wrapU`, `wrapV?`, `wrapR?`): `void`

Update the sampling mode of a given texture

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `texture` | [`InternalTexture`](InternalTexture.md) | `undefined` | defines the texture to update |
| `wrapU` | [`Nullable`](../modules.md#nullable)`number` | `undefined` | defines the texture wrap mode of the u coordinates |
| `wrapV` | [`Nullable`](../modules.md#nullable)`number` | `null` | defines the texture wrap mode of the v coordinates |
| `wrapR` | [`Nullable`](../modules.md#nullable)`number` | `null` | defines the texture wrap mode of the r coordinates |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:4440

___

### updateUniformBuffer

▸ **updateUniformBuffer**(`uniformBuffer`, `elements`, `offset?`, `count?`): `void`

Update an existing uniform buffer

**`See`**

https://doc.babylonjs.com/features/webgl2#uniform-buffer-objets

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformBuffer` | [`DataBuffer`](DataBuffer.md) | defines the target uniform buffer |
| `elements` | [`FloatArray`](../modules.md#floatarray) | defines the content to update |
| `offset?` | `number` | defines the offset in the uniform buffer where update should start |
| `count?` | `number` | defines the size of the data to update |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.uniformBuffer.ts:34

___

### updateVideoTexture

▸ **updateVideoTexture**(`texture`, `video`, `invertY`): `void`

Update a video texture

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `texture` | [`Nullable`](../modules.md#nullable)[`InternalTexture`](InternalTexture.md) | defines the texture to update |
| `video` | `HTMLVideoElement` | defines the video element to use |
| `invertY` | `boolean` | defines if data must be stored with Y axis inverted |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.videoTexture.ts:13

___

### wipeCaches

▸ **wipeCaches**(`bruteForce?`): `void`

Force the entire cache to be cleared
You should not have to use this function unless your engine needs to share the webGL context with another engine

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `bruteForce?` | `boolean` | defines a boolean to force clearing ALL caches (including stencil, detoh and alpha states) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:3586

___

### CeilingPOT

▸ `Static` **CeilingPOT**(`x`): `number`

Find the next highest power of two.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | Number to start search from. |

#### Returns

`number`

Next highest power of two.

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:5855

___

### FloorPOT

▸ `Static` **FloorPOT**(`x`): `number`

Find the next lowest power of two.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | Number to start search from. |

#### Returns

`number`

Next lowest power of two.

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:5871

___

### GetExponentOfTwo

▸ `Static` **GetExponentOfTwo**(`value`, `max`, `mode?`): `number`

Get the closest exponent of two

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `value` | `number` | `undefined` | defines the value to approximate |
| `max` | `number` | `undefined` | defines the maximum value to return |
| `mode` | `number` | `Constants.SCALEMODE_NEAREST` | defines how to define the closest value |

#### Returns

`number`

closest exponent of two of the given value

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:5898

___

### NearestPOT

▸ `Static` **NearestPOT**(`x`): `number`

Find the nearest power of two.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | Number to start search from. |

#### Returns

`number`

Next nearest power of two.

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:5885

___

### QueueNewFrame

▸ `Static` **QueueNewFrame**(`func`, `requester?`): `number`

Queue a new function into the requested animation frame pool (ie. this function will be executed byt the browser for the next frame)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `func` | () => `void` | the function to be called |
| `requester?` | `any` | the object that will request the next frame. Falls back to window. |

#### Returns

`number`

frame number

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:5923

___

### \_ConcatenateShader

▸ `Static` `Protected` **_ConcatenateShader**(`source`, `defines`, `shaderVersion?`): `string`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `source` | `string` | `undefined` |
| `defines` | [`Nullable`](../modules.md#nullable)`string` | `undefined` |
| `shaderVersion` | `string` | `""` |

#### Returns

`string`

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:2837

___

### \_CreateCanvas

▸ `Static` `Private` **_CreateCanvas**(`width`, `height`): [`ICanvas`](../interfaces/ICanvas.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `width` | `number` |
| `height` | `number` |

#### Returns

[`ICanvas`](../interfaces/ICanvas.md)

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:723

___

### isSupported

▸ `Static` **isSupported**(): `boolean`

Gets a boolean indicating if the engine can be instantiated (ie. if a webGL context can be found)

**`Ignorenaming`**

#### Returns

`boolean`

true if the engine can be created

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:5811
