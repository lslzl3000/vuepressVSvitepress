[@dev/core](../README.md) / [Exports](../modules.md) / NullEngine

# Class: NullEngine

The null engine class provides support for headless version of babylon.js.
This can be used in server side scenario or for testing purposes

## Hierarchy

- [`Engine`](Engine.md)

  ↳ **`NullEngine`**

## Table of contents

### Constructors

- [constructor](NullEngine.md#constructor)

### Properties

- [\_activeRenderLoops](NullEngine.md#_activerenderloops)
- [\_audioContext](NullEngine.md#_audiocontext)
- [\_audioDestination](NullEngine.md#_audiodestination)
- [\_boundUniforms](NullEngine.md#_bounduniforms)
- [\_compatibilityMode](NullEngine.md#_compatibilitymode)
- [\_compiledEffects](NullEngine.md#_compiledeffects)
- [\_contextWasLost](NullEngine.md#_contextwaslost)
- [\_creationOptions](NullEngine.md#_creationoptions)
- [\_currentBoundBuffer](NullEngine.md#_currentboundbuffer)
- [\_currentEffect](NullEngine.md#_currenteffect)
- [\_deterministicLockstep](NullEngine.md#_deterministiclockstep)
- [\_highPrecisionShadersAllowed](NullEngine.md#_highprecisionshadersallowed)
- [\_isStencilEnable](NullEngine.md#_isstencilenable)
- [\_lockstepMaxSteps](NullEngine.md#_lockstepmaxsteps)
- [\_options](NullEngine.md#_options)
- [\_renderingCanvas](NullEngine.md#_renderingcanvas)
- [\_renderingQueueLaunched](NullEngine.md#_renderingqueuelaunched)
- [\_shaderProcessor](NullEngine.md#_shaderprocessor)
- [\_snapshotRenderingMode](NullEngine.md#_snapshotrenderingmode)
- [\_timeStep](NullEngine.md#_timestep)
- [\_useExactSrgbConversions](NullEngine.md#_useexactsrgbconversions)
- [\_viewportCached](NullEngine.md#_viewportcached)
- [\_windowIsBackground](NullEngine.md#_windowisbackground)
- [activeView](NullEngine.md#activeview)
- [adaptToDeviceRatio](NullEngine.md#adapttodeviceratio)
- [canvasTabIndex](NullEngine.md#canvastabindex)
- [cullBackFaces](NullEngine.md#cullbackfaces)
- [currentRenderPassId](NullEngine.md#currentrenderpassid)
- [customAnimationFrameRequester](NullEngine.md#customanimationframerequester)
- [disableContextMenu](NullEngine.md#disablecontextmenu)
- [disableManifestCheck](NullEngine.md#disablemanifestcheck)
- [disablePerformanceMonitorInBackground](NullEngine.md#disableperformancemonitorinbackground)
- [disableUniformBuffers](NullEngine.md#disableuniformbuffers)
- [disableVertexArrayObjects](NullEngine.md#disablevertexarrayobjects)
- [enableOfflineSupport](NullEngine.md#enableofflinesupport)
- [enableUnpackFlipYCached](NullEngine.md#enableunpackflipycached)
- [forcePOTTextures](NullEngine.md#forcepottextures)
- [hasOriginBottomLeft](NullEngine.md#hasoriginbottomleft)
- [hostInformation](NullEngine.md#hostinformation)
- [inputElement](NullEngine.md#inputelement)
- [isFullscreen](NullEngine.md#isfullscreen)
- [isInVRExclusivePointerMode](NullEngine.md#isinvrexclusivepointermode)
- [isNDCHalfZRange](NullEngine.md#isndchalfzrange)
- [isPointerLock](NullEngine.md#ispointerlock)
- [onAfterShaderCompilationObservable](NullEngine.md#onaftershadercompilationobservable)
- [onBeforeShaderCompilationObservable](NullEngine.md#onbeforeshadercompilationobservable)
- [onBeforeTextureInitObservable](NullEngine.md#onbeforetextureinitobservable)
- [onBeginFrameObservable](NullEngine.md#onbeginframeobservable)
- [onCanvasBlurObservable](NullEngine.md#oncanvasblurobservable)
- [onCanvasFocusObservable](NullEngine.md#oncanvasfocusobservable)
- [onCanvasPointerOutObservable](NullEngine.md#oncanvaspointeroutobservable)
- [onContextLostObservable](NullEngine.md#oncontextlostobservable)
- [onContextRestoredObservable](NullEngine.md#oncontextrestoredobservable)
- [onDisposeObservable](NullEngine.md#ondisposeobservable)
- [onEndFrameObservable](NullEngine.md#onendframeobservable)
- [onNewSceneAddedObservable](NullEngine.md#onnewsceneaddedobservable)
- [onResizeObservable](NullEngine.md#onresizeobservable)
- [onVRDisplayChangedObservable](NullEngine.md#onvrdisplaychangedobservable)
- [onVRRequestPresentComplete](NullEngine.md#onvrrequestpresentcomplete)
- [onVRRequestPresentStart](NullEngine.md#onvrrequestpresentstart)
- [postProcesses](NullEngine.md#postprocesses)
- [premultipliedAlpha](NullEngine.md#premultipliedalpha)
- [preventCacheWipeBetweenFrames](NullEngine.md#preventcachewipebetweenframes)
- [renderEvenInBackground](NullEngine.md#rendereveninbackground)
- [scenes](NullEngine.md#scenes)
- [textureFormatInUse](NullEngine.md#textureformatinuse)
- [texturesSupported](NullEngine.md#texturessupported)
- [validateShaderPrograms](NullEngine.md#validateshaderprograms)
- [views](NullEngine.md#views)
- [vrPresentationAttributes](NullEngine.md#vrpresentationattributes)
- [ALPHA\_ADD](NullEngine.md#alpha_add)
- [ALPHA\_COMBINE](NullEngine.md#alpha_combine)
- [ALPHA\_DISABLE](NullEngine.md#alpha_disable)
- [ALPHA\_INTERPOLATE](NullEngine.md#alpha_interpolate)
- [ALPHA\_MAXIMIZED](NullEngine.md#alpha_maximized)
- [ALPHA\_MULTIPLY](NullEngine.md#alpha_multiply)
- [ALPHA\_ONEONE](NullEngine.md#alpha_oneone)
- [ALPHA\_PREMULTIPLIED](NullEngine.md#alpha_premultiplied)
- [ALPHA\_PREMULTIPLIED\_PORTERDUFF](NullEngine.md#alpha_premultiplied_porterduff)
- [ALPHA\_SCREENMODE](NullEngine.md#alpha_screenmode)
- [ALPHA\_SUBTRACT](NullEngine.md#alpha_subtract)
- [ALWAYS](NullEngine.md#always)
- [AudioEngineFactory](NullEngine.md#audioenginefactory)
- [CollisionsEpsilon](NullEngine.md#collisionsepsilon)
- [DECR](NullEngine.md#decr)
- [DECR\_WRAP](NullEngine.md#decr_wrap)
- [DELAYLOADSTATE\_LOADED](NullEngine.md#delayloadstate_loaded)
- [DELAYLOADSTATE\_LOADING](NullEngine.md#delayloadstate_loading)
- [DELAYLOADSTATE\_NONE](NullEngine.md#delayloadstate_none)
- [DELAYLOADSTATE\_NOTLOADED](NullEngine.md#delayloadstate_notloaded)
- [EQUAL](NullEngine.md#equal)
- [ExceptionList](NullEngine.md#exceptionlist)
- [GEQUAL](NullEngine.md#gequal)
- [GREATER](NullEngine.md#greater)
- [INCR](NullEngine.md#incr)
- [INCR\_WRAP](NullEngine.md#incr_wrap)
- [INVERT](NullEngine.md#invert)
- [KEEP](NullEngine.md#keep)
- [LEQUAL](NullEngine.md#lequal)
- [LESS](NullEngine.md#less)
- [NEVER](NullEngine.md#never)
- [NOTEQUAL](NullEngine.md#notequal)
- [OfflineProviderFactory](NullEngine.md#offlineproviderfactory)
- [REPLACE](NullEngine.md#replace)
- [SCALEMODE\_CEILING](NullEngine.md#scalemode_ceiling)
- [SCALEMODE\_FLOOR](NullEngine.md#scalemode_floor)
- [SCALEMODE\_NEAREST](NullEngine.md#scalemode_nearest)
- [TEXTUREFORMAT\_ALPHA](NullEngine.md#textureformat_alpha)
- [TEXTUREFORMAT\_LUMINANCE](NullEngine.md#textureformat_luminance)
- [TEXTUREFORMAT\_LUMINANCE\_ALPHA](NullEngine.md#textureformat_luminance_alpha)
- [TEXTUREFORMAT\_R](NullEngine.md#textureformat_r)
- [TEXTUREFORMAT\_RED](NullEngine.md#textureformat_red)
- [TEXTUREFORMAT\_RED\_INTEGER](NullEngine.md#textureformat_red_integer)
- [TEXTUREFORMAT\_RG](NullEngine.md#textureformat_rg)
- [TEXTUREFORMAT\_RGB](NullEngine.md#textureformat_rgb)
- [TEXTUREFORMAT\_RGBA](NullEngine.md#textureformat_rgba)
- [TEXTUREFORMAT\_RGBA\_INTEGER](NullEngine.md#textureformat_rgba_integer)
- [TEXTUREFORMAT\_RGB\_INTEGER](NullEngine.md#textureformat_rgb_integer)
- [TEXTUREFORMAT\_RG\_INTEGER](NullEngine.md#textureformat_rg_integer)
- [TEXTUREFORMAT\_R\_INTEGER](NullEngine.md#textureformat_r_integer)
- [TEXTURETYPE\_BYTE](NullEngine.md#texturetype_byte)
- [TEXTURETYPE\_FLOAT](NullEngine.md#texturetype_float)
- [TEXTURETYPE\_FLOAT\_32\_UNSIGNED\_INT\_24\_8\_REV](NullEngine.md#texturetype_float_32_unsigned_int_24_8_rev)
- [TEXTURETYPE\_HALF\_FLOAT](NullEngine.md#texturetype_half_float)
- [TEXTURETYPE\_INT](NullEngine.md#texturetype_int)
- [TEXTURETYPE\_SHORT](NullEngine.md#texturetype_short)
- [TEXTURETYPE\_UNSIGNED\_BYTE](NullEngine.md#texturetype_unsigned_byte)
- [TEXTURETYPE\_UNSIGNED\_INT](NullEngine.md#texturetype_unsigned_int)
- [TEXTURETYPE\_UNSIGNED\_INTEGER](NullEngine.md#texturetype_unsigned_integer)
- [TEXTURETYPE\_UNSIGNED\_INT\_10F\_11F\_11F\_REV](NullEngine.md#texturetype_unsigned_int_10f_11f_11f_rev)
- [TEXTURETYPE\_UNSIGNED\_INT\_24\_8](NullEngine.md#texturetype_unsigned_int_24_8)
- [TEXTURETYPE\_UNSIGNED\_INT\_2\_10\_10\_10\_REV](NullEngine.md#texturetype_unsigned_int_2_10_10_10_rev)
- [TEXTURETYPE\_UNSIGNED\_INT\_5\_9\_9\_9\_REV](NullEngine.md#texturetype_unsigned_int_5_9_9_9_rev)
- [TEXTURETYPE\_UNSIGNED\_SHORT](NullEngine.md#texturetype_unsigned_short)
- [TEXTURETYPE\_UNSIGNED\_SHORT\_4\_4\_4\_4](NullEngine.md#texturetype_unsigned_short_4_4_4_4)
- [TEXTURETYPE\_UNSIGNED\_SHORT\_5\_5\_5\_1](NullEngine.md#texturetype_unsigned_short_5_5_5_1)
- [TEXTURETYPE\_UNSIGNED\_SHORT\_5\_6\_5](NullEngine.md#texturetype_unsigned_short_5_6_5)
- [TEXTURE\_BILINEAR\_SAMPLINGMODE](NullEngine.md#texture_bilinear_samplingmode)
- [TEXTURE\_CLAMP\_ADDRESSMODE](NullEngine.md#texture_clamp_addressmode)
- [TEXTURE\_CUBIC\_MODE](NullEngine.md#texture_cubic_mode)
- [TEXTURE\_EQUIRECTANGULAR\_MODE](NullEngine.md#texture_equirectangular_mode)
- [TEXTURE\_EXPLICIT\_MODE](NullEngine.md#texture_explicit_mode)
- [TEXTURE\_FIXED\_EQUIRECTANGULAR\_MIRRORED\_MODE](NullEngine.md#texture_fixed_equirectangular_mirrored_mode)
- [TEXTURE\_FIXED\_EQUIRECTANGULAR\_MODE](NullEngine.md#texture_fixed_equirectangular_mode)
- [TEXTURE\_INVCUBIC\_MODE](NullEngine.md#texture_invcubic_mode)
- [TEXTURE\_LINEAR\_LINEAR](NullEngine.md#texture_linear_linear)
- [TEXTURE\_LINEAR\_LINEAR\_MIPLINEAR](NullEngine.md#texture_linear_linear_miplinear)
- [TEXTURE\_LINEAR\_LINEAR\_MIPNEAREST](NullEngine.md#texture_linear_linear_mipnearest)
- [TEXTURE\_LINEAR\_NEAREST](NullEngine.md#texture_linear_nearest)
- [TEXTURE\_LINEAR\_NEAREST\_MIPLINEAR](NullEngine.md#texture_linear_nearest_miplinear)
- [TEXTURE\_LINEAR\_NEAREST\_MIPNEAREST](NullEngine.md#texture_linear_nearest_mipnearest)
- [TEXTURE\_MIRROR\_ADDRESSMODE](NullEngine.md#texture_mirror_addressmode)
- [TEXTURE\_NEAREST\_LINEAR](NullEngine.md#texture_nearest_linear)
- [TEXTURE\_NEAREST\_LINEAR\_MIPLINEAR](NullEngine.md#texture_nearest_linear_miplinear)
- [TEXTURE\_NEAREST\_LINEAR\_MIPNEAREST](NullEngine.md#texture_nearest_linear_mipnearest)
- [TEXTURE\_NEAREST\_NEAREST](NullEngine.md#texture_nearest_nearest)
- [TEXTURE\_NEAREST\_NEAREST\_MIPLINEAR](NullEngine.md#texture_nearest_nearest_miplinear)
- [TEXTURE\_NEAREST\_NEAREST\_MIPNEAREST](NullEngine.md#texture_nearest_nearest_mipnearest)
- [TEXTURE\_NEAREST\_SAMPLINGMODE](NullEngine.md#texture_nearest_samplingmode)
- [TEXTURE\_PLANAR\_MODE](NullEngine.md#texture_planar_mode)
- [TEXTURE\_PROJECTION\_MODE](NullEngine.md#texture_projection_mode)
- [TEXTURE\_SKYBOX\_MODE](NullEngine.md#texture_skybox_mode)
- [TEXTURE\_SPHERICAL\_MODE](NullEngine.md#texture_spherical_mode)
- [TEXTURE\_TRILINEAR\_SAMPLINGMODE](NullEngine.md#texture_trilinear_samplingmode)
- [TEXTURE\_WRAP\_ADDRESSMODE](NullEngine.md#texture_wrap_addressmode)
- [\_RenderPassIdCounter](NullEngine.md#_renderpassidcounter)
- [\_RescalePostProcessFactory](NullEngine.md#_rescalepostprocessfactory)
- [audioEngine](NullEngine.md#audioengine)

### Accessors

- [\_supportsHardwareTextureRescaling](NullEngine.md#_supportshardwaretexturerescaling)
- [activeRenderLoops](NullEngine.md#activerenderloops)
- [alphaState](NullEngine.md#alphastate)
- [compatibilityMode](NullEngine.md#compatibilitymode)
- [currentViewport](NullEngine.md#currentviewport)
- [depthCullingState](NullEngine.md#depthcullingstate)
- [description](NullEngine.md#description)
- [doNotHandleContextLost](NullEngine.md#donothandlecontextlost)
- [emptyCubeTexture](NullEngine.md#emptycubetexture)
- [emptyTexture](NullEngine.md#emptytexture)
- [emptyTexture2DArray](NullEngine.md#emptytexture2darray)
- [emptyTexture3D](NullEngine.md#emptytexture3d)
- [frameId](NullEngine.md#frameid)
- [framebufferDimensionsObject](NullEngine.md#framebufferdimensionsobject)
- [isStencilEnable](NullEngine.md#isstencilenable)
- [isWebGPU](NullEngine.md#iswebgpu)
- [loadingScreen](NullEngine.md#loadingscreen)
- [loadingUIBackgroundColor](NullEngine.md#loadinguibackgroundcolor)
- [loadingUIText](NullEngine.md#loadinguitext)
- [name](NullEngine.md#name)
- [needPOTTextures](NullEngine.md#needpottextures)
- [performanceMonitor](NullEngine.md#performancemonitor)
- [shaderPlatformName](NullEngine.md#shaderplatformname)
- [snapshotRendering](NullEngine.md#snapshotrendering)
- [snapshotRenderingMode](NullEngine.md#snapshotrenderingmode)
- [stencilState](NullEngine.md#stencilstate)
- [stencilStateComposer](NullEngine.md#stencilstatecomposer)
- [supportsUniformBuffers](NullEngine.md#supportsuniformbuffers)
- [useExactSrgbConversions](NullEngine.md#useexactsrgbconversions)
- [useReverseDepthBuffer](NullEngine.md#usereversedepthbuffer)
- [version](NullEngine.md#version)
- [webGLVersion](NullEngine.md#webglversion)
- [HasMajorPerformanceCaveat](NullEngine.md#hasmajorperformancecaveat)
- [Instances](NullEngine.md#instances)
- [IsSupported](NullEngine.md#issupported)
- [IsSupportedAsync](NullEngine.md#issupportedasync)
- [LastCreatedEngine](NullEngine.md#lastcreatedengine)
- [LastCreatedScene](NullEngine.md#lastcreatedscene)
- [NpmPackage](NullEngine.md#npmpackage)
- [ShadersRepository](NullEngine.md#shadersrepository)
- [Version](NullEngine.md#version-1)

### Methods

- [\_createDepthStencilCubeTexture](NullEngine.md#_createdepthstencilcubetexture)
- [\_createImageBitmapFromSource](NullEngine.md#_createimagebitmapfromsource)
- [\_createShaderProgram](NullEngine.md#_createshaderprogram)
- [\_createTextureBase](NullEngine.md#_createtexturebase)
- [\_deleteBuffer](NullEngine.md#_deletebuffer)
- [\_deletePipelineContext](NullEngine.md#_deletepipelinecontext)
- [\_deleteTexture](NullEngine.md#_deletetexture)
- [\_finalizePipelineContext](NullEngine.md#_finalizepipelinecontext)
- [\_initFeatures](NullEngine.md#_initfeatures)
- [\_initGLContext](NullEngine.md#_initglcontext)
- [\_normalizeIndexData](NullEngine.md#_normalizeindexdata)
- [\_prepareWebGLTextureContinuation](NullEngine.md#_preparewebgltexturecontinuation)
- [\_rebuildBuffers](NullEngine.md#_rebuildbuffers)
- [\_renderLoop](NullEngine.md#_renderloop)
- [\_resetIndexBufferBinding](NullEngine.md#_resetindexbufferbinding)
- [\_restoreEngineAfterContextLost](NullEngine.md#_restoreengineaftercontextlost)
- [\_setProgram](NullEngine.md#_setprogram)
- [\_setTexture](NullEngine.md#_settexture)
- [\_sharedInit](NullEngine.md#_sharedinit)
- [applyStates](NullEngine.md#applystates)
- [areAllComputeEffectsReady](NullEngine.md#areallcomputeeffectsready)
- [areAllEffectsReady](NullEngine.md#arealleffectsready)
- [attachContextLostEvent](NullEngine.md#attachcontextlostevent)
- [attachContextRestoredEvent](NullEngine.md#attachcontextrestoredevent)
- [beginFrame](NullEngine.md#beginframe)
- [beginOcclusionQuery](NullEngine.md#beginocclusionquery)
- [beginTransformFeedback](NullEngine.md#begintransformfeedback)
- [bindArrayBuffer](NullEngine.md#bindarraybuffer)
- [bindAttachments](NullEngine.md#bindattachments)
- [bindBuffers](NullEngine.md#bindbuffers)
- [bindBuffersDirectly](NullEngine.md#bindbuffersdirectly)
- [bindFramebuffer](NullEngine.md#bindframebuffer)
- [bindIndexBuffer](NullEngine.md#bindindexbuffer)
- [bindInstancesBuffer](NullEngine.md#bindinstancesbuffer)
- [bindMultiviewFramebuffer](NullEngine.md#bindmultiviewframebuffer)
- [bindSamplers](NullEngine.md#bindsamplers)
- [bindTransformFeedback](NullEngine.md#bindtransformfeedback)
- [bindTransformFeedbackBuffer](NullEngine.md#bindtransformfeedbackbuffer)
- [bindUniformBlock](NullEngine.md#binduniformblock)
- [bindUniformBuffer](NullEngine.md#binduniformbuffer)
- [bindUniformBufferBase](NullEngine.md#binduniformbufferbase)
- [bindVertexArrayObject](NullEngine.md#bindvertexarrayobject)
- [buildTextureLayout](NullEngine.md#buildtexturelayout)
- [cacheStencilState](NullEngine.md#cachestencilstate)
- [captureGPUFrameTime](NullEngine.md#capturegpuframetime)
- [clear](NullEngine.md#clear)
- [clearInternalTexturesCache](NullEngine.md#clearinternaltexturescache)
- [computeDispatch](NullEngine.md#computedispatch)
- [createCanvas](NullEngine.md#createcanvas)
- [createCanvasImage](NullEngine.md#createcanvasimage)
- [createComputeContext](NullEngine.md#createcomputecontext)
- [createComputeEffect](NullEngine.md#createcomputeeffect)
- [createComputePipelineContext](NullEngine.md#createcomputepipelinecontext)
- [createCubeTexture](NullEngine.md#createcubetexture)
- [createDepthStencilTexture](NullEngine.md#createdepthstenciltexture)
- [createDrawContext](NullEngine.md#createdrawcontext)
- [createDynamicTexture](NullEngine.md#createdynamictexture)
- [createDynamicUniformBuffer](NullEngine.md#createdynamicuniformbuffer)
- [createDynamicVertexBuffer](NullEngine.md#createdynamicvertexbuffer)
- [createEffect](NullEngine.md#createeffect)
- [createEffectForParticles](NullEngine.md#createeffectforparticles)
- [createExternalTexture](NullEngine.md#createexternaltexture)
- [createImageBitmap](NullEngine.md#createimagebitmap)
- [createIndexBuffer](NullEngine.md#createindexbuffer)
- [createInstancesBuffer](NullEngine.md#createinstancesbuffer)
- [createMaterialContext](NullEngine.md#creatematerialcontext)
- [createMultipleRenderTarget](NullEngine.md#createmultiplerendertarget)
- [createMultiviewRenderTargetTexture](NullEngine.md#createmultiviewrendertargettexture)
- [createPipelineContext](NullEngine.md#createpipelinecontext)
- [createPrefilteredCubeTexture](NullEngine.md#createprefilteredcubetexture)
- [createQuery](NullEngine.md#createquery)
- [createRawCubeTexture](NullEngine.md#createrawcubetexture)
- [createRawCubeTextureFromUrl](NullEngine.md#createrawcubetexturefromurl)
- [createRawShaderProgram](NullEngine.md#createrawshaderprogram)
- [createRawTexture](NullEngine.md#createrawtexture)
- [createRawTexture2DArray](NullEngine.md#createrawtexture2darray)
- [createRawTexture3D](NullEngine.md#createrawtexture3d)
- [createRenderPassId](NullEngine.md#createrenderpassid)
- [createRenderTargetCubeTexture](NullEngine.md#createrendertargetcubetexture)
- [createRenderTargetTexture](NullEngine.md#createrendertargettexture)
- [createShaderProgram](NullEngine.md#createshaderprogram)
- [createStorageBuffer](NullEngine.md#createstoragebuffer)
- [createTexture](NullEngine.md#createtexture)
- [createTransformFeedback](NullEngine.md#createtransformfeedback)
- [createUniformBuffer](NullEngine.md#createuniformbuffer)
- [createVertexBuffer](NullEngine.md#createvertexbuffer)
- [createVideoElement](NullEngine.md#createvideoelement)
- [deleteInstancesBuffer](NullEngine.md#deleteinstancesbuffer)
- [deleteQuery](NullEngine.md#deletequery)
- [deleteTransformFeedback](NullEngine.md#deletetransformfeedback)
- [disableAttributeByIndex](NullEngine.md#disableattributebyindex)
- [disableInstanceAttribute](NullEngine.md#disableinstanceattribute)
- [disableInstanceAttributeByName](NullEngine.md#disableinstanceattributebyname)
- [disableScissor](NullEngine.md#disablescissor)
- [disableVR](NullEngine.md#disablevr)
- [displayLoadingUI](NullEngine.md#displayloadingui)
- [dispose](NullEngine.md#dispose)
- [draw](NullEngine.md#draw)
- [drawArraysType](NullEngine.md#drawarraystype)
- [drawElementsType](NullEngine.md#drawelementstype)
- [drawPointClouds](NullEngine.md#drawpointclouds)
- [drawUnIndexed](NullEngine.md#drawunindexed)
- [enableEffect](NullEngine.md#enableeffect)
- [enableScissor](NullEngine.md#enablescissor)
- [enableVR](NullEngine.md#enablevr)
- [endFrame](NullEngine.md#endframe)
- [endOcclusionQuery](NullEngine.md#endocclusionquery)
- [endTimeQuery](NullEngine.md#endtimequery)
- [endTransformFeedback](NullEngine.md#endtransformfeedback)
- [enterFullscreen](NullEngine.md#enterfullscreen)
- [enterPointerlock](NullEngine.md#enterpointerlock)
- [exitFullscreen](NullEngine.md#exitfullscreen)
- [exitPointerlock](NullEngine.md#exitpointerlock)
- [flushFramebuffer](NullEngine.md#flushframebuffer)
- [generateMipMapsForCubemap](NullEngine.md#generatemipmapsforcubemap)
- [generateMipmaps](NullEngine.md#generatemipmaps)
- [getAlphaEquation](NullEngine.md#getalphaequation)
- [getAlphaMode](NullEngine.md#getalphamode)
- [getAspectRatio](NullEngine.md#getaspectratio)
- [getAttributes](NullEngine.md#getattributes)
- [getAudioContext](NullEngine.md#getaudiocontext)
- [getAudioDestination](NullEngine.md#getaudiodestination)
- [getCaps](NullEngine.md#getcaps)
- [getClassName](NullEngine.md#getclassname)
- [getColorWrite](NullEngine.md#getcolorwrite)
- [getCreationOptions](NullEngine.md#getcreationoptions)
- [getCurrentRenderPassName](NullEngine.md#getcurrentrenderpassname)
- [getDeltaTime](NullEngine.md#getdeltatime)
- [getDepthBuffer](NullEngine.md#getdepthbuffer)
- [getDepthFunction](NullEngine.md#getdepthfunction)
- [getDepthWrite](NullEngine.md#getdepthwrite)
- [getFontOffset](NullEngine.md#getfontoffset)
- [getFps](NullEngine.md#getfps)
- [getFragmentShaderSource](NullEngine.md#getfragmentshadersource)
- [getGPUFrameTimeCounter](NullEngine.md#getgpuframetimecounter)
- [getGlInfo](NullEngine.md#getglinfo)
- [getHardwareScalingLevel](NullEngine.md#gethardwarescalinglevel)
- [getHostDocument](NullEngine.md#gethostdocument)
- [getHostWindow](NullEngine.md#gethostwindow)
- [getInfo](NullEngine.md#getinfo)
- [getInputElement](NullEngine.md#getinputelement)
- [getInputElementClientRect](NullEngine.md#getinputelementclientrect)
- [getLoadedTexturesCache](NullEngine.md#getloadedtexturescache)
- [getLockstepMaxSteps](NullEngine.md#getlockstepmaxsteps)
- [getQueryResult](NullEngine.md#getqueryresult)
- [getRenderHeight](NullEngine.md#getrenderheight)
- [getRenderPassNames](NullEngine.md#getrenderpassnames)
- [getRenderWidth](NullEngine.md#getrenderwidth)
- [getRenderingCanvas](NullEngine.md#getrenderingcanvas)
- [getRenderingCanvasClientRect](NullEngine.md#getrenderingcanvasclientrect)
- [getScreenAspectRatio](NullEngine.md#getscreenaspectratio)
- [getStencilBuffer](NullEngine.md#getstencilbuffer)
- [getStencilFunction](NullEngine.md#getstencilfunction)
- [getStencilFunctionMask](NullEngine.md#getstencilfunctionmask)
- [getStencilFunctionReference](NullEngine.md#getstencilfunctionreference)
- [getStencilMask](NullEngine.md#getstencilmask)
- [getStencilOperationDepthFail](NullEngine.md#getstenciloperationdepthfail)
- [getStencilOperationFail](NullEngine.md#getstenciloperationfail)
- [getStencilOperationPass](NullEngine.md#getstenciloperationpass)
- [getTimeStep](NullEngine.md#gettimestep)
- [getUniforms](NullEngine.md#getuniforms)
- [getVRDevice](NullEngine.md#getvrdevice)
- [getVertexShaderSource](NullEngine.md#getvertexshadersource)
- [getZOffset](NullEngine.md#getzoffset)
- [getZOffsetUnits](NullEngine.md#getzoffsetunits)
- [hideLoadingUI](NullEngine.md#hideloadingui)
- [initWebVR](NullEngine.md#initwebvr)
- [initWebVRAsync](NullEngine.md#initwebvrasync)
- [inlineShaderCode](NullEngine.md#inlineshadercode)
- [isDeterministicLockStep](NullEngine.md#isdeterministiclockstep)
- [isQueryResultAvailable](NullEngine.md#isqueryresultavailable)
- [isVRDevicePresent](NullEngine.md#isvrdevicepresent)
- [isVRPresenting](NullEngine.md#isvrpresenting)
- [readFromStorageBuffer](NullEngine.md#readfromstoragebuffer)
- [readPixels](NullEngine.md#readpixels)
- [recordVertexArrayObject](NullEngine.md#recordvertexarrayobject)
- [registerView](NullEngine.md#registerview)
- [releaseComputeEffects](NullEngine.md#releasecomputeeffects)
- [releaseEffects](NullEngine.md#releaseeffects)
- [releaseRenderPassId](NullEngine.md#releaserenderpassid)
- [releaseVertexArrayObject](NullEngine.md#releasevertexarrayobject)
- [resetTextureCache](NullEngine.md#resettexturecache)
- [resize](NullEngine.md#resize)
- [resizeImageBitmap](NullEngine.md#resizeimagebitmap)
- [restoreDefaultFramebuffer](NullEngine.md#restoredefaultframebuffer)
- [restoreSingleAttachment](NullEngine.md#restoresingleattachment)
- [restoreSingleAttachmentForRenderTarget](NullEngine.md#restoresingleattachmentforrendertarget)
- [restoreStencilState](NullEngine.md#restorestencilstate)
- [runRenderLoop](NullEngine.md#runrenderloop)
- [scissorClear](NullEngine.md#scissorclear)
- [setAlphaConstants](NullEngine.md#setalphaconstants)
- [setAlphaEquation](NullEngine.md#setalphaequation)
- [setAlphaMode](NullEngine.md#setalphamode)
- [setArray](NullEngine.md#setarray)
- [setArray2](NullEngine.md#setarray2)
- [setArray3](NullEngine.md#setarray3)
- [setArray4](NullEngine.md#setarray4)
- [setBool](NullEngine.md#setbool)
- [setColorWrite](NullEngine.md#setcolorwrite)
- [setCompressedTextureExclusions](NullEngine.md#setcompressedtextureexclusions)
- [setDepthBuffer](NullEngine.md#setdepthbuffer)
- [setDepthFunction](NullEngine.md#setdepthfunction)
- [setDepthFunctionToGreater](NullEngine.md#setdepthfunctiontogreater)
- [setDepthFunctionToGreaterOrEqual](NullEngine.md#setdepthfunctiontogreaterorequal)
- [setDepthFunctionToLess](NullEngine.md#setdepthfunctiontoless)
- [setDepthFunctionToLessOrEqual](NullEngine.md#setdepthfunctiontolessorequal)
- [setDepthStencilTexture](NullEngine.md#setdepthstenciltexture)
- [setDepthWrite](NullEngine.md#setdepthwrite)
- [setDirectViewport](NullEngine.md#setdirectviewport)
- [setDitheringState](NullEngine.md#setditheringstate)
- [setExternalTexture](NullEngine.md#setexternaltexture)
- [setFloat](NullEngine.md#setfloat)
- [setFloat2](NullEngine.md#setfloat2)
- [setFloat3](NullEngine.md#setfloat3)
- [setFloat4](NullEngine.md#setfloat4)
- [setFloatArray](NullEngine.md#setfloatarray)
- [setFloatArray2](NullEngine.md#setfloatarray2)
- [setFloatArray3](NullEngine.md#setfloatarray3)
- [setFloatArray4](NullEngine.md#setfloatarray4)
- [setHardwareScalingLevel](NullEngine.md#sethardwarescalinglevel)
- [setInt](NullEngine.md#setint)
- [setInt2](NullEngine.md#setint2)
- [setInt3](NullEngine.md#setint3)
- [setInt4](NullEngine.md#setint4)
- [setIntArray](NullEngine.md#setintarray)
- [setIntArray2](NullEngine.md#setintarray2)
- [setIntArray3](NullEngine.md#setintarray3)
- [setIntArray4](NullEngine.md#setintarray4)
- [setMatrices](NullEngine.md#setmatrices)
- [setMatrix2x2](NullEngine.md#setmatrix2x2)
- [setMatrix3x3](NullEngine.md#setmatrix3x3)
- [setRasterizerState](NullEngine.md#setrasterizerstate)
- [setSize](NullEngine.md#setsize)
- [setState](NullEngine.md#setstate)
- [setStencilBuffer](NullEngine.md#setstencilbuffer)
- [setStencilFunction](NullEngine.md#setstencilfunction)
- [setStencilFunctionMask](NullEngine.md#setstencilfunctionmask)
- [setStencilFunctionReference](NullEngine.md#setstencilfunctionreference)
- [setStencilMask](NullEngine.md#setstencilmask)
- [setStencilOperationDepthFail](NullEngine.md#setstenciloperationdepthfail)
- [setStencilOperationFail](NullEngine.md#setstenciloperationfail)
- [setStencilOperationPass](NullEngine.md#setstenciloperationpass)
- [setStorageBuffer](NullEngine.md#setstoragebuffer)
- [setTexture](NullEngine.md#settexture)
- [setTextureArray](NullEngine.md#settexturearray)
- [setTextureFormatToUse](NullEngine.md#settextureformattouse)
- [setTextureFromPostProcess](NullEngine.md#settexturefrompostprocess)
- [setTextureFromPostProcessOutput](NullEngine.md#settexturefrompostprocessoutput)
- [setTextureSampler](NullEngine.md#settexturesampler)
- [setTranformFeedbackVaryings](NullEngine.md#settranformfeedbackvaryings)
- [setViewport](NullEngine.md#setviewport)
- [setZOffset](NullEngine.md#setzoffset)
- [setZOffsetUnits](NullEngine.md#setzoffsetunits)
- [snapshotRenderingReset](NullEngine.md#snapshotrenderingreset)
- [startTimeQuery](NullEngine.md#starttimequery)
- [stopRenderLoop](NullEngine.md#stoprenderloop)
- [switchFullscreen](NullEngine.md#switchfullscreen)
- [unBindFramebuffer](NullEngine.md#unbindframebuffer)
- [unBindMultiColorAttachmentFramebuffer](NullEngine.md#unbindmulticolorattachmentframebuffer)
- [unRegisterView](NullEngine.md#unregisterview)
- [unbindAllAttributes](NullEngine.md#unbindallattributes)
- [unbindAllTextures](NullEngine.md#unbindalltextures)
- [unbindInstanceAttributes](NullEngine.md#unbindinstanceattributes)
- [updateAndBindInstancesBuffer](NullEngine.md#updateandbindinstancesbuffer)
- [updateArrayBuffer](NullEngine.md#updatearraybuffer)
- [updateDynamicIndexBuffer](NullEngine.md#updatedynamicindexbuffer)
- [updateDynamicTexture](NullEngine.md#updatedynamictexture)
- [updateDynamicVertexBuffer](NullEngine.md#updatedynamicvertexbuffer)
- [updateMultipleRenderTargetTextureSampleCount](NullEngine.md#updatemultiplerendertargettexturesamplecount)
- [updateRawCubeTexture](NullEngine.md#updaterawcubetexture)
- [updateRawTexture](NullEngine.md#updaterawtexture)
- [updateRawTexture2DArray](NullEngine.md#updaterawtexture2darray)
- [updateRawTexture3D](NullEngine.md#updaterawtexture3d)
- [updateRenderTargetTextureSampleCount](NullEngine.md#updaterendertargettexturesamplecount)
- [updateStorageBuffer](NullEngine.md#updatestoragebuffer)
- [updateTextureComparisonFunction](NullEngine.md#updatetexturecomparisonfunction)
- [updateTextureData](NullEngine.md#updatetexturedata)
- [updateTextureDimensions](NullEngine.md#updatetexturedimensions)
- [updateTextureSamplingMode](NullEngine.md#updatetexturesamplingmode)
- [updateTextureWrappingMode](NullEngine.md#updatetexturewrappingmode)
- [updateUniformBuffer](NullEngine.md#updateuniformbuffer)
- [updateVideoTexture](NullEngine.md#updatevideotexture)
- [wipeCaches](NullEngine.md#wipecaches)
- [wrapWebGLTexture](NullEngine.md#wrapwebgltexture)
- [CeilingPOT](NullEngine.md#ceilingpot)
- [DefaultLoadingScreenFactory](NullEngine.md#defaultloadingscreenfactory)
- [FloorPOT](NullEngine.md#floorpot)
- [GetExponentOfTwo](NullEngine.md#getexponentoftwo)
- [MarkAllMaterialsAsDirty](NullEngine.md#markallmaterialsasdirty)
- [NearestPOT](NullEngine.md#nearestpot)
- [QueueNewFrame](NullEngine.md#queuenewframe)
- [\_ConcatenateShader](NullEngine.md#_concatenateshader)
- [\_ExitFullscreen](NullEngine.md#_exitfullscreen)
- [\_ExitPointerlock](NullEngine.md#_exitpointerlock)
- [\_RequestFullscreen](NullEngine.md#_requestfullscreen)
- [\_RequestPointerlock](NullEngine.md#_requestpointerlock)
- [isSupported](NullEngine.md#issupported-1)

## Constructors

### constructor

• **new NullEngine**(`options?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `options` | [`NullEngineOptions`](NullEngineOptions.md) |

#### Overrides

[Engine](Engine.md).[constructor](Engine.md#constructor)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:92

## Properties

### \_activeRenderLoops

• `Protected` **\_activeRenderLoops**: () => `void`[]

#### Inherited from

[Engine](Engine.md).[_activeRenderLoops](Engine.md#_activerenderloops)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:424

___

### \_audioContext

• `Protected` **\_audioContext**: [`Nullable`](../modules.md#nullable)`AudioContext`

#### Inherited from

[Engine](Engine.md).[_audioContext](Engine.md#_audiocontext)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:377

___

### \_audioDestination

• `Protected` **\_audioDestination**: [`Nullable`](../modules.md#nullable)`AudioDestinationNode` \| `MediaStreamAudioDestinationNode`

#### Inherited from

[Engine](Engine.md).[_audioDestination](Engine.md#_audiodestination)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:378

___

### \_boundUniforms

• `Protected` **\_boundUniforms**: `Object` = `{}`

#### Index signature

▪ [key: `number`]: `WebGLUniformLocation`

#### Inherited from

[Engine](Engine.md).[_boundUniforms](Engine.md#_bounduniforms)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:4916

___

### \_compatibilityMode

• `Protected` **\_compatibilityMode**: `boolean` = `true`

#### Inherited from

[Engine](Engine.md).[_compatibilityMode](Engine.md#_compatibilitymode)

#### Defined in

packages/dev/core/src/Engines/engine.ts:545

___

### \_compiledEffects

• `Protected` **\_compiledEffects**: `Object` = `{}`

#### Index signature

▪ [key: `string`]: [`Effect`](Effect.md)

#### Inherited from

[Engine](Engine.md).[_compiledEffects](Engine.md#_compiledeffects)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:502

___

### \_contextWasLost

• `Protected` **\_contextWasLost**: `boolean` = `false`

#### Inherited from

[Engine](Engine.md).[_contextWasLost](Engine.md#_contextwaslost)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:445

___

### \_creationOptions

• `Protected` **\_creationOptions**: [`EngineOptions`](../interfaces/EngineOptions.md)

#### Inherited from

[Engine](Engine.md).[_creationOptions](Engine.md#_creationoptions)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:376

___

### \_currentBoundBuffer

• `Protected` **\_currentBoundBuffer**: [`Nullable`](../modules.md#nullable)`WebGLBuffer`[]

#### Inherited from

[Engine](Engine.md).[_currentBoundBuffer](Engine.md#_currentboundbuffer)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:517

___

### \_currentEffect

• `Protected` **\_currentEffect**: [`Nullable`](../modules.md#nullable)[`Effect`](Effect.md)

#### Inherited from

[Engine](Engine.md).[_currentEffect](Engine.md#_currenteffect)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:495

___

### \_deterministicLockstep

• `Protected` **\_deterministicLockstep**: `boolean` = `false`

#### Inherited from

[Engine](Engine.md).[_deterministicLockstep](Engine.md#_deterministiclockstep)

#### Defined in

packages/dev/core/src/Engines/engine.ts:502

___

### \_highPrecisionShadersAllowed

• `Protected` **\_highPrecisionShadersAllowed**: `boolean` = `true`

#### Inherited from

[Engine](Engine.md).[_highPrecisionShadersAllowed](Engine.md#_highprecisionshadersallowed)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:388

___

### \_isStencilEnable

• `Protected` **\_isStencilEnable**: `boolean`

#### Inherited from

[Engine](Engine.md).[_isStencilEnable](Engine.md#_isstencilenable)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:414

___

### \_lockstepMaxSteps

• `Protected` **\_lockstepMaxSteps**: `number` = `4`

#### Inherited from

[Engine](Engine.md).[_lockstepMaxSteps](Engine.md#_lockstepmaxsteps)

#### Defined in

packages/dev/core/src/Engines/engine.ts:503

___

### \_options

• `Private` **\_options**: [`NullEngineOptions`](NullEngineOptions.md)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:62

___

### \_renderingCanvas

• `Protected` **\_renderingCanvas**: [`Nullable`](../modules.md#nullable)`HTMLCanvasElement`

#### Inherited from

[Engine](Engine.md).[_renderingCanvas](Engine.md#_renderingcanvas)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:374

___

### \_renderingQueueLaunched

• `Protected` **\_renderingQueueLaunched**: `boolean` = `false`

#### Inherited from

[Engine](Engine.md).[_renderingQueueLaunched](Engine.md#_renderingqueuelaunched)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:423

___

### \_shaderProcessor

• `Protected` **\_shaderProcessor**: [`Nullable`](../modules.md#nullable)`IShaderProcessor`

#### Inherited from

[Engine](Engine.md).[_shaderProcessor](Engine.md#_shaderprocessor)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:265

___

### \_snapshotRenderingMode

• `Protected` **\_snapshotRenderingMode**: `number` = `Constants.SNAPSHOTRENDERING_STANDARD`

#### Inherited from

[Engine](Engine.md).[_snapshotRenderingMode](Engine.md#_snapshotrenderingmode)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:694

___

### \_timeStep

• `Protected` **\_timeStep**: `number`

#### Inherited from

[Engine](Engine.md).[_timeStep](Engine.md#_timestep)

#### Defined in

packages/dev/core/src/Engines/engine.ts:504

___

### \_useExactSrgbConversions

• `Protected` **\_useExactSrgbConversions**: `boolean` = `false`

#### Inherited from

[Engine](Engine.md).[_useExactSrgbConversions](Engine.md#_useexactsrgbconversions)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:706

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

#### Inherited from

[Engine](Engine.md).[_viewportCached](Engine.md#_viewportcached)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1692

___

### \_windowIsBackground

• `Protected` **\_windowIsBackground**: `boolean` = `false`

#### Inherited from

[Engine](Engine.md).[_windowIsBackground](Engine.md#_windowisbackground)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:375

___

### activeView

• **activeView**: [`Nullable`](../modules.md#nullable)[`EngineView`](EngineView.md)

Gets the current engine view

**`See`**

https://doc.babylonjs.com/how_to/multi_canvases

#### Inherited from

[Engine](Engine.md).[activeView](Engine.md#activeview)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.views.ts:43

___

### adaptToDeviceRatio

• **adaptToDeviceRatio**: `boolean` = `false`

If set to true zooming in and out in the browser will rescale the hardware-scaling correctly.

#### Inherited from

[Engine](Engine.md).[adaptToDeviceRatio](Engine.md#adapttodeviceratio)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:555

___

### canvasTabIndex

• **canvasTabIndex**: `number` = `1`

Gets or sets the tab index to set to the rendering canvas. 1 is the minimum value to set to be able to capture keyboard events

#### Inherited from

[Engine](Engine.md).[canvasTabIndex](Engine.md#canvastabindex)

#### Defined in

packages/dev/core/src/Engines/engine.ts:518

___

### cullBackFaces

• **cullBackFaces**: [`Nullable`](../modules.md#nullable)`boolean` = `null`

Gets or sets a boolean indicating if back faces must be culled. If false, front faces are culled instead (true by default)
If non null, this takes precedence over the value from the material

#### Inherited from

[Engine](Engine.md).[cullBackFaces](Engine.md#cullbackfaces)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:289

___

### currentRenderPassId

• **currentRenderPassId**: `number` = `Constants.RENDERPASS_MAIN`

Gets or sets the current render pass id

#### Inherited from

[Engine](Engine.md).[currentRenderPassId](Engine.md#currentrenderpassid)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1580

___

### customAnimationFrameRequester

• **customAnimationFrameRequester**: [`Nullable`](../modules.md#nullable)[`ICustomAnimationFrameRequester`](../interfaces/ICustomAnimationFrameRequester.md) = `null`

If set, will be used to request the next animation frame for the render loop

#### Inherited from

[Engine](Engine.md).[customAnimationFrameRequester](Engine.md#customanimationframerequester)

#### Defined in

packages/dev/core/src/Engines/engine.ts:456

___

### disableContextMenu

• **disableContextMenu**: `boolean` = `true`

Gets or sets a boolean to enable/disable the context menu (right-click) from appearing on the main canvas

#### Inherited from

[Engine](Engine.md).[disableContextMenu](Engine.md#disablecontextmenu)

#### Defined in

packages/dev/core/src/Engines/engine.ts:401

___

### disableManifestCheck

• **disableManifestCheck**: `boolean` = `false`

Gets or sets a boolean to enable/disable checking manifest if IndexedDB support is enabled (js will always consider the database is up to date)

#### Inherited from

[Engine](Engine.md).[disableManifestCheck](Engine.md#disablemanifestcheck)

#### Defined in

packages/dev/core/src/Engines/engine.ts:396

___

### disablePerformanceMonitorInBackground

• **disablePerformanceMonitorInBackground**: `boolean` = `false`

Turn this value on if you want to pause FPS computation when in background

#### Inherited from

[Engine](Engine.md).[disablePerformanceMonitorInBackground](Engine.md#disableperformancemonitorinbackground)

#### Defined in

packages/dev/core/src/Engines/engine.ts:523

___

### disableUniformBuffers

• **disableUniformBuffers**: `boolean` = `false`

Gets or sets a boolean indicating that uniform buffers must be disabled even if they are supported

#### Inherited from

[Engine](Engine.md).[disableUniformBuffers](Engine.md#disableuniformbuffers)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:340

___

### disableVertexArrayObjects

• **disableVertexArrayObjects**: `boolean` = `false`

Gets or sets a boolean indicating that vertex array object must be disabled even if they are supported

#### Inherited from

[Engine](Engine.md).[disableVertexArrayObjects](Engine.md#disablevertexarrayobjects)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:465

___

### enableOfflineSupport

• **enableOfflineSupport**: `boolean` = `false`

Gets or sets a boolean to enable/disable IndexedDB support and avoid XHR on .manifest

#### Inherited from

[Engine](Engine.md).[enableOfflineSupport](Engine.md#enableofflinesupport)

#### Defined in

packages/dev/core/src/Engines/engine.ts:391

___

### enableUnpackFlipYCached

• **enableUnpackFlipYCached**: `boolean` = `true`

In case you are sharing the context with other applications, it might
be interested to not cache the unpack flip y state to ensure a consistent
value would be set.

#### Inherited from

[Engine](Engine.md).[enableUnpackFlipYCached](Engine.md#enableunpackflipycached)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:4369

___

### forcePOTTextures

• **forcePOTTextures**: `boolean` = `false`

Gets or sets a boolean that indicates if textures must be forced to power of 2 size even if not required

#### Inherited from

[Engine](Engine.md).[forcePOTTextures](Engine.md#forcepottextures)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:278

___

### hasOriginBottomLeft

• `Readonly` **hasOriginBottomLeft**: ``true``

Indicates that the origin of the texture/framebuffer space is the bottom left corner. If false, the origin is top left

#### Inherited from

[Engine](Engine.md).[hasOriginBottomLeft](Engine.md#hasoriginbottomleft)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:335

___

### hostInformation

• **hostInformation**: [`HostInformation`](../interfaces/HostInformation.md)

Gets information about the current host

#### Inherited from

[Engine](Engine.md).[hostInformation](Engine.md#hostinformation)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:565

___

### inputElement

• **inputElement**: [`Nullable`](../modules.md#nullable)`HTMLElement`

Gets or sets the  HTML element to use for attaching events

#### Inherited from

[Engine](Engine.md).[inputElement](Engine.md#inputelement)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.views.ts:31

___

### isFullscreen

• **isFullscreen**: `boolean` = `false`

Gets a boolean indicating if the engine is currently rendering in fullscreen mode

#### Inherited from

[Engine](Engine.md).[isFullscreen](Engine.md#isfullscreen)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:283

___

### isInVRExclusivePointerMode

• **isInVRExclusivePointerMode**: `boolean`

Gets a boolean indicating that the engine is currently in VR exclusive mode for the pointers

**`See`**

https://docs.microsoft.com/en-us/microsoft-edge/webvr/essentials#mouse-input

#### Inherited from

[Engine](Engine.md).[isInVRExclusivePointerMode](Engine.md#isinvrexclusivepointermode)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.webVR.ts:68

___

### isNDCHalfZRange

• `Readonly` **isNDCHalfZRange**: ``false``

Indicates if the z range in NDC space is 0..1 (value: true) or -1..1 (value: false)

#### Inherited from

[Engine](Engine.md).[isNDCHalfZRange](Engine.md#isndchalfzrange)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:330

___

### isPointerLock

• **isPointerLock**: `boolean` = `false`

Gets a boolean indicating if the pointer is currently locked

#### Inherited from

[Engine](Engine.md).[isPointerLock](Engine.md#ispointerlock)

#### Defined in

packages/dev/core/src/Engines/engine.ts:424

___

### onAfterShaderCompilationObservable

• **onAfterShaderCompilationObservable**: [`Observable`](Observable.md)[`Engine`](Engine.md)

Observable raised when the engine has just compiled a shader

#### Inherited from

[Engine](Engine.md).[onAfterShaderCompilationObservable](Engine.md#onaftershadercompilationobservable)

#### Defined in

packages/dev/core/src/Engines/engine.ts:471

___

### onBeforeShaderCompilationObservable

• **onBeforeShaderCompilationObservable**: [`Observable`](Observable.md)[`Engine`](Engine.md)

Observable raised when the engine is about to compile a shader

#### Inherited from

[Engine](Engine.md).[onBeforeShaderCompilationObservable](Engine.md#onbeforeshadercompilationobservable)

#### Defined in

packages/dev/core/src/Engines/engine.ts:466

___

### onBeforeTextureInitObservable

• **onBeforeTextureInitObservable**: [`Observable`](Observable.md)[`Texture`](Texture.md)

Observable event triggered before each texture is initialized

#### Inherited from

[Engine](Engine.md).[onBeforeTextureInitObservable](Engine.md#onbeforetextureinitobservable)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:662

___

### onBeginFrameObservable

• **onBeginFrameObservable**: [`Observable`](Observable.md)[`Engine`](Engine.md)

Observable raised when the engine begins a new frame

#### Inherited from

[Engine](Engine.md).[onBeginFrameObservable](Engine.md#onbeginframeobservable)

#### Defined in

packages/dev/core/src/Engines/engine.ts:451

___

### onCanvasBlurObservable

• **onCanvasBlurObservable**: [`Observable`](Observable.md)[`Engine`](Engine.md)

Observable event triggered each time the canvas loses focus

#### Inherited from

[Engine](Engine.md).[onCanvasBlurObservable](Engine.md#oncanvasblurobservable)

#### Defined in

packages/dev/core/src/Engines/engine.ts:436

___

### onCanvasFocusObservable

• **onCanvasFocusObservable**: [`Observable`](Observable.md)[`Engine`](Engine.md)

Observable event triggered each time the canvas gains focus

#### Inherited from

[Engine](Engine.md).[onCanvasFocusObservable](Engine.md#oncanvasfocusobservable)

#### Defined in

packages/dev/core/src/Engines/engine.ts:441

___

### onCanvasPointerOutObservable

• **onCanvasPointerOutObservable**: [`Observable`](Observable.md)`PointerEvent`

Observable event triggered each time the canvas receives pointerout event

#### Inherited from

[Engine](Engine.md).[onCanvasPointerOutObservable](Engine.md#oncanvaspointeroutobservable)

#### Defined in

packages/dev/core/src/Engines/engine.ts:446

___

### onContextLostObservable

• **onContextLostObservable**: [`Observable`](Observable.md)[`ThinEngine`](ThinEngine.md)

Observable signaled when a context lost event is raised

#### Inherited from

[Engine](Engine.md).[onContextLostObservable](Engine.md#oncontextlostobservable)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:438

___

### onContextRestoredObservable

• **onContextRestoredObservable**: [`Observable`](Observable.md)[`ThinEngine`](ThinEngine.md)

Observable signaled when a context restored event is raised

#### Inherited from

[Engine](Engine.md).[onContextRestoredObservable](Engine.md#oncontextrestoredobservable)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:442

___

### onDisposeObservable

• `Readonly` **onDisposeObservable**: [`Observable`](Observable.md)[`ThinEngine`](ThinEngine.md)

An event triggered when the engine is disposed.

#### Inherited from

[Engine](Engine.md).[onDisposeObservable](Engine.md#ondisposeobservable)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:345

___

### onEndFrameObservable

• **onEndFrameObservable**: [`Observable`](Observable.md)[`Engine`](Engine.md)

Observable raised when the engine ends the current frame

#### Inherited from

[Engine](Engine.md).[onEndFrameObservable](Engine.md#onendframeobservable)

#### Defined in

packages/dev/core/src/Engines/engine.ts:461

___

### onNewSceneAddedObservable

• **onNewSceneAddedObservable**: [`Observable`](Observable.md)[`Scene`](Scene.md)

Event raised when a new scene is created

#### Inherited from

[Engine](Engine.md).[onNewSceneAddedObservable](Engine.md#onnewsceneaddedobservable)

#### Defined in

packages/dev/core/src/Engines/engine.ts:414

___

### onResizeObservable

• **onResizeObservable**: [`Observable`](Observable.md)[`Engine`](Engine.md)

Observable event triggered each time the rendering canvas is resized

#### Inherited from

[Engine](Engine.md).[onResizeObservable](Engine.md#onresizeobservable)

#### Defined in

packages/dev/core/src/Engines/engine.ts:431

___

### onVRDisplayChangedObservable

• **onVRDisplayChangedObservable**: [`Observable`](Observable.md)[`IDisplayChangedEventArgs`](../interfaces/IDisplayChangedEventArgs.md)

Observable signaled when VR display mode changes

#### Inherited from

[Engine](Engine.md).[onVRDisplayChangedObservable](Engine.md#onvrdisplaychangedobservable)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.webVR.ts:54

___

### onVRRequestPresentComplete

• **onVRRequestPresentComplete**: [`Observable`](Observable.md)`boolean`

Observable signaled when VR request present is complete

#### Inherited from

[Engine](Engine.md).[onVRRequestPresentComplete](Engine.md#onvrrequestpresentcomplete)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.webVR.ts:58

___

### onVRRequestPresentStart

• **onVRRequestPresentStart**: [`Observable`](Observable.md)[`Engine`](Engine.md)

Observable signaled when VR request present starts

#### Inherited from

[Engine](Engine.md).[onVRRequestPresentStart](Engine.md#onvrrequestpresentstart)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.webVR.ts:62

___

### postProcesses

• **postProcesses**: [`PostProcess`](PostProcess.md)[]

Gets the list of created postprocesses

#### Inherited from

[Engine](Engine.md).[postProcesses](Engine.md#postprocesses)

#### Defined in

packages/dev/core/src/Engines/engine.ts:419

___

### premultipliedAlpha

• **premultipliedAlpha**: `boolean` = `true`

Defines whether the engine has been created with the premultipliedAlpha option on or not.

#### Inherited from

[Engine](Engine.md).[premultipliedAlpha](Engine.md#premultipliedalpha)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:657

___

### preventCacheWipeBetweenFrames

• **preventCacheWipeBetweenFrames**: `boolean` = `false`

Gets or sets a boolean indicating that cache can be kept between frames

#### Inherited from

[Engine](Engine.md).[preventCacheWipeBetweenFrames](Engine.md#preventcachewipebetweenframes)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:299

___

### renderEvenInBackground

• **renderEvenInBackground**: `boolean` = `true`

Gets or sets a boolean indicating if the engine must keep rendering even if the window is not in foreground

#### Inherited from

[Engine](Engine.md).[renderEvenInBackground](Engine.md#rendereveninbackground)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:294

___

### scenes

• **scenes**: [`Scene`](Scene.md)[]

Gets the list of created scenes

#### Inherited from

[Engine](Engine.md).[scenes](Engine.md#scenes)

#### Defined in

packages/dev/core/src/Engines/engine.ts:406

___

### textureFormatInUse

• `Readonly` **textureFormatInUse**: [`Nullable`](../modules.md#nullable)`string`

Gets the texture format in use

#### Inherited from

[Engine](Engine.md).[textureFormatInUse](Engine.md#textureformatinuse)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.textureSelector.ts:20

___

### texturesSupported

• `Readonly` **texturesSupported**: `string`[]

Gets the list of texture formats supported

#### Inherited from

[Engine](Engine.md).[texturesSupported](Engine.md#texturessupported)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.textureSelector.ts:15

___

### validateShaderPrograms

• **validateShaderPrograms**: `boolean` = `false`

Gets or sets a boolean indicating if the engine should validate programs after compilation

#### Inherited from

[Engine](Engine.md).[validateShaderPrograms](Engine.md#validateshaderprograms)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:302

___

### views

• **views**: [`EngineView`](EngineView.md)[]

Gets or sets the list of views

#### Inherited from

[Engine](Engine.md).[views](Engine.md#views)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.views.ts:46

___

### vrPresentationAttributes

• `Optional` **vrPresentationAttributes**: [`IVRPresentationAttributes`](../interfaces/IVRPresentationAttributes.md)

Gets or sets the presentation attributes used to configure VR rendering

#### Inherited from

[Engine](Engine.md).[vrPresentationAttributes](Engine.md#vrpresentationattributes)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.webVR.ts:95

___

### ALPHA\_ADD

▪ `Static` `Readonly` **ALPHA\_ADD**: ``1``

Defines that alpha blending to SRC ALPHA * SRC + DEST

#### Inherited from

[Engine](Engine.md).[ALPHA_ADD](Engine.md#alpha_add)

#### Defined in

packages/dev/core/src/Engines/engine.ts:63

___

### ALPHA\_COMBINE

▪ `Static` `Readonly` **ALPHA\_COMBINE**: ``2``

Defines that alpha blending to SRC ALPHA * SRC + (1 - SRC ALPHA) * DEST

#### Inherited from

[Engine](Engine.md).[ALPHA_COMBINE](Engine.md#alpha_combine)

#### Defined in

packages/dev/core/src/Engines/engine.ts:65

___

### ALPHA\_DISABLE

▪ `Static` `Readonly` **ALPHA\_DISABLE**: ``0``

Defines that alpha blending is disabled

#### Inherited from

[Engine](Engine.md).[ALPHA_DISABLE](Engine.md#alpha_disable)

#### Defined in

packages/dev/core/src/Engines/engine.ts:61

___

### ALPHA\_INTERPOLATE

▪ `Static` `Readonly` **ALPHA\_INTERPOLATE**: ``9``

Defines that alpha blending to CST * SRC + (1 - CST) * DEST

#### Inherited from

[Engine](Engine.md).[ALPHA_INTERPOLATE](Engine.md#alpha_interpolate)

#### Defined in

packages/dev/core/src/Engines/engine.ts:82

___

### ALPHA\_MAXIMIZED

▪ `Static` `Readonly` **ALPHA\_MAXIMIZED**: ``5``

Defines that alpha blending to SRC ALPHA * SRC + (1 - SRC) * DEST

#### Inherited from

[Engine](Engine.md).[ALPHA_MAXIMIZED](Engine.md#alpha_maximized)

#### Defined in

packages/dev/core/src/Engines/engine.ts:71

___

### ALPHA\_MULTIPLY

▪ `Static` `Readonly` **ALPHA\_MULTIPLY**: ``4``

Defines that alpha blending to SRC * DEST

#### Inherited from

[Engine](Engine.md).[ALPHA_MULTIPLY](Engine.md#alpha_multiply)

#### Defined in

packages/dev/core/src/Engines/engine.ts:69

___

### ALPHA\_ONEONE

▪ `Static` `Readonly` **ALPHA\_ONEONE**: ``6``

Defines that alpha blending to SRC + DEST

#### Inherited from

[Engine](Engine.md).[ALPHA_ONEONE](Engine.md#alpha_oneone)

#### Defined in

packages/dev/core/src/Engines/engine.ts:73

___

### ALPHA\_PREMULTIPLIED

▪ `Static` `Readonly` **ALPHA\_PREMULTIPLIED**: ``7``

Defines that alpha blending to SRC + (1 - SRC ALPHA) * DEST

#### Inherited from

[Engine](Engine.md).[ALPHA_PREMULTIPLIED](Engine.md#alpha_premultiplied)

#### Defined in

packages/dev/core/src/Engines/engine.ts:75

___

### ALPHA\_PREMULTIPLIED\_PORTERDUFF

▪ `Static` `Readonly` **ALPHA\_PREMULTIPLIED\_PORTERDUFF**: ``8``

Defines that alpha blending to SRC + (1 - SRC ALPHA) * DEST
Alpha will be set to (1 - SRC ALPHA) * DEST ALPHA

#### Inherited from

[Engine](Engine.md).[ALPHA_PREMULTIPLIED_PORTERDUFF](Engine.md#alpha_premultiplied_porterduff)

#### Defined in

packages/dev/core/src/Engines/engine.ts:80

___

### ALPHA\_SCREENMODE

▪ `Static` `Readonly` **ALPHA\_SCREENMODE**: ``10``

Defines that alpha blending to SRC + (1 - SRC) * DEST
Alpha will be set to SRC ALPHA + (1 - SRC ALPHA) * DEST ALPHA

#### Inherited from

[Engine](Engine.md).[ALPHA_SCREENMODE](Engine.md#alpha_screenmode)

#### Defined in

packages/dev/core/src/Engines/engine.ts:87

___

### ALPHA\_SUBTRACT

▪ `Static` `Readonly` **ALPHA\_SUBTRACT**: ``3``

Defines that alpha blending to DEST - SRC * DEST

#### Inherited from

[Engine](Engine.md).[ALPHA_SUBTRACT](Engine.md#alpha_subtract)

#### Defined in

packages/dev/core/src/Engines/engine.ts:67

___

### ALWAYS

▪ `Static` `Readonly` **ALWAYS**: ``519``

Passed to depthFunction or stencilFunction to specify depth or stencil tests will always pass. i.e. Pixels will be drawn in the order they are drawn

#### Inherited from

[Engine](Engine.md).[ALWAYS](Engine.md#always)

#### Defined in

packages/dev/core/src/Engines/engine.ts:102

___

### AudioEngineFactory

▪ `Static` **AudioEngineFactory**: (`hostElement`: [`Nullable`](../modules.md#nullable)`HTMLElement`, `audioContext`: [`Nullable`](../modules.md#nullable)`AudioContext`, `audioDestination`: [`Nullable`](../modules.md#nullable)`AudioDestinationNode` \| `MediaStreamAudioDestinationNode`) => [`IAudioEngine`](../interfaces/IAudioEngine.md)

#### Type declaration

▸ (`hostElement`, `audioContext`, `audioDestination`): [`IAudioEngine`](../interfaces/IAudioEngine.md)

Default AudioEngine factory responsible of creating the Audio Engine.
By default, this will create a BabylonJS Audio Engine if the workload has been embedded.

##### Parameters

| Name | Type |
| :------ | :------ |
| `hostElement` | [`Nullable`](../modules.md#nullable)`HTMLElement` |
| `audioContext` | [`Nullable`](../modules.md#nullable)`AudioContext` |
| `audioDestination` | [`Nullable`](../modules.md#nullable)`AudioDestinationNode` \| `MediaStreamAudioDestinationNode` |

##### Returns

[`IAudioEngine`](../interfaces/IAudioEngine.md)

#### Inherited from

[Engine](Engine.md).[AudioEngineFactory](Engine.md#audioenginefactory)

#### Defined in

packages/dev/core/src/Engines/engine.ts:485

___

### CollisionsEpsilon

▪ `Static` **CollisionsEpsilon**: `number` = `0.001`

Gets or sets the epsilon value used by collision engine

#### Inherited from

[Engine](Engine.md).[CollisionsEpsilon](Engine.md#collisionsepsilon)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:253

___

### DECR

▪ `Static` `Readonly` **DECR**: ``7683``

Passed to stencilOperation to specify that stencil value must be decremented

#### Inherited from

[Engine](Engine.md).[DECR](Engine.md#decr)

#### Defined in

packages/dev/core/src/Engines/engine.ts:124

___

### DECR\_WRAP

▪ `Static` `Readonly` **DECR\_WRAP**: ``34056``

Passed to stencilOperation to specify that stencil value must be decremented with wrapping

#### Inherited from

[Engine](Engine.md).[DECR_WRAP](Engine.md#decr_wrap)

#### Defined in

packages/dev/core/src/Engines/engine.ts:130

___

### DELAYLOADSTATE\_LOADED

▪ `Static` `Readonly` **DELAYLOADSTATE\_LOADED**: ``1``

Defines that the resource was successfully delay loaded

#### Inherited from

[Engine](Engine.md).[DELAYLOADSTATE_LOADED](Engine.md#delayloadstate_loaded)

#### Defined in

packages/dev/core/src/Engines/engine.ts:92

___

### DELAYLOADSTATE\_LOADING

▪ `Static` `Readonly` **DELAYLOADSTATE\_LOADING**: ``2``

Defines that the resource is currently delay loading

#### Inherited from

[Engine](Engine.md).[DELAYLOADSTATE_LOADING](Engine.md#delayloadstate_loading)

#### Defined in

packages/dev/core/src/Engines/engine.ts:94

___

### DELAYLOADSTATE\_NONE

▪ `Static` `Readonly` **DELAYLOADSTATE\_NONE**: ``0``

Defines that the resource is not delayed

#### Inherited from

[Engine](Engine.md).[DELAYLOADSTATE_NONE](Engine.md#delayloadstate_none)

#### Defined in

packages/dev/core/src/Engines/engine.ts:90

___

### DELAYLOADSTATE\_NOTLOADED

▪ `Static` `Readonly` **DELAYLOADSTATE\_NOTLOADED**: ``4``

Defines that the resource is delayed and has not started loading

#### Inherited from

[Engine](Engine.md).[DELAYLOADSTATE_NOTLOADED](Engine.md#delayloadstate_notloaded)

#### Defined in

packages/dev/core/src/Engines/engine.ts:96

___

### EQUAL

▪ `Static` `Readonly` **EQUAL**: ``514``

Passed to depthFunction or stencilFunction to specify depth or stencil tests will pass if the new depth value is equals to the stored value

#### Inherited from

[Engine](Engine.md).[EQUAL](Engine.md#equal)

#### Defined in

packages/dev/core/src/Engines/engine.ts:106

___

### ExceptionList

▪ `Static` **ExceptionList**: ({ `capture`: `string` = "63\\.0\\.3239\\.(\\d+)"; `captureConstraint`: `number` = 108; `key`: `string` = "Chrome/63.0"; `targets`: `string`[]  } \| { `capture`: ``null`` = null; `captureConstraint`: ``null`` = null; `key`: `string` = "Firefox/58"; `targets`: `string`[]  })[]

Use this array to turn off some WebGL2 features on known buggy browsers version

#### Inherited from

[Engine](Engine.md).[ExceptionList](Engine.md#exceptionlist)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:180

___

### GEQUAL

▪ `Static` `Readonly` **GEQUAL**: ``518``

Passed to depthFunction or stencilFunction to specify depth or stencil tests will pass if the new depth value is greater than or equal to the stored value

#### Inherited from

[Engine](Engine.md).[GEQUAL](Engine.md#gequal)

#### Defined in

packages/dev/core/src/Engines/engine.ts:112

___

### GREATER

▪ `Static` `Readonly` **GREATER**: ``516``

Passed to depthFunction or stencilFunction to specify depth or stencil tests will pass if the new depth value is greater than the stored value

#### Inherited from

[Engine](Engine.md).[GREATER](Engine.md#greater)

#### Defined in

packages/dev/core/src/Engines/engine.ts:110

___

### INCR

▪ `Static` `Readonly` **INCR**: ``7682``

Passed to stencilOperation to specify that stencil value must be incremented

#### Inherited from

[Engine](Engine.md).[INCR](Engine.md#incr)

#### Defined in

packages/dev/core/src/Engines/engine.ts:122

___

### INCR\_WRAP

▪ `Static` `Readonly` **INCR\_WRAP**: ``34055``

Passed to stencilOperation to specify that stencil value must be incremented with wrapping

#### Inherited from

[Engine](Engine.md).[INCR_WRAP](Engine.md#incr_wrap)

#### Defined in

packages/dev/core/src/Engines/engine.ts:128

___

### INVERT

▪ `Static` `Readonly` **INVERT**: ``5386``

Passed to stencilOperation to specify that stencil value must be inverted

#### Inherited from

[Engine](Engine.md).[INVERT](Engine.md#invert)

#### Defined in

packages/dev/core/src/Engines/engine.ts:126

___

### KEEP

▪ `Static` `Readonly` **KEEP**: ``7680``

Passed to stencilOperation to specify that stencil value must be kept

#### Inherited from

[Engine](Engine.md).[KEEP](Engine.md#keep)

#### Defined in

packages/dev/core/src/Engines/engine.ts:118

___

### LEQUAL

▪ `Static` `Readonly` **LEQUAL**: ``515``

Passed to depthFunction or stencilFunction to specify depth or stencil tests will pass if the new depth value is less than or equal to the stored value

#### Inherited from

[Engine](Engine.md).[LEQUAL](Engine.md#lequal)

#### Defined in

packages/dev/core/src/Engines/engine.ts:108

___

### LESS

▪ `Static` `Readonly` **LESS**: ``513``

Passed to depthFunction or stencilFunction to specify depth or stencil tests will pass if the new depth value is less than the stored value

#### Inherited from

[Engine](Engine.md).[LESS](Engine.md#less)

#### Defined in

packages/dev/core/src/Engines/engine.ts:104

___

### NEVER

▪ `Static` `Readonly` **NEVER**: ``512``

Passed to depthFunction or stencilFunction to specify depth or stencil tests will never pass. i.e. Nothing will be drawn

#### Inherited from

[Engine](Engine.md).[NEVER](Engine.md#never)

#### Defined in

packages/dev/core/src/Engines/engine.ts:100

___

### NOTEQUAL

▪ `Static` `Readonly` **NOTEQUAL**: ``517``

Passed to depthFunction or stencilFunction to specify depth or stencil tests will pass if the new depth value is not equal to the stored value

#### Inherited from

[Engine](Engine.md).[NOTEQUAL](Engine.md#notequal)

#### Defined in

packages/dev/core/src/Engines/engine.ts:114

___

### OfflineProviderFactory

▪ `Static` **OfflineProviderFactory**: (`urlToScene`: `string`, `callbackManifestChecked`: (`checked`: `boolean`) => `any`, `disableManifestCheck`: `boolean`) => [`IOfflineProvider`](../interfaces/IOfflineProvider.md)

#### Type declaration

▸ (`urlToScene`, `callbackManifestChecked`, `disableManifestCheck`): [`IOfflineProvider`](../interfaces/IOfflineProvider.md)

Default offline support factory responsible of creating a tool used to store data locally.
By default, this will create a Database object if the workload has been embedded.

##### Parameters

| Name | Type |
| :------ | :------ |
| `urlToScene` | `string` |
| `callbackManifestChecked` | (`checked`: `boolean`) => `any` |
| `disableManifestCheck` | `boolean` |

##### Returns

[`IOfflineProvider`](../interfaces/IOfflineProvider.md)

#### Inherited from

[Engine](Engine.md).[OfflineProviderFactory](Engine.md#offlineproviderfactory)

#### Defined in

packages/dev/core/src/Engines/engine.ts:495

___

### REPLACE

▪ `Static` `Readonly` **REPLACE**: ``7681``

Passed to stencilOperation to specify that stencil value must be replaced

#### Inherited from

[Engine](Engine.md).[REPLACE](Engine.md#replace)

#### Defined in

packages/dev/core/src/Engines/engine.ts:120

___

### SCALEMODE\_CEILING

▪ `Static` `Readonly` **SCALEMODE\_CEILING**: ``3``

Defines that texture rescaling will use a ceil to find the closer power of 2 size

#### Inherited from

[Engine](Engine.md).[SCALEMODE_CEILING](Engine.md#scalemode_ceiling)

#### Defined in

packages/dev/core/src/Engines/engine.ts:259

___

### SCALEMODE\_FLOOR

▪ `Static` `Readonly` **SCALEMODE\_FLOOR**: ``1``

Defines that texture rescaling will use a floor to find the closer power of 2 size

#### Inherited from

[Engine](Engine.md).[SCALEMODE_FLOOR](Engine.md#scalemode_floor)

#### Defined in

packages/dev/core/src/Engines/engine.ts:255

___

### SCALEMODE\_NEAREST

▪ `Static` `Readonly` **SCALEMODE\_NEAREST**: ``2``

Defines that texture rescaling will look for the nearest power of 2 size

#### Inherited from

[Engine](Engine.md).[SCALEMODE_NEAREST](Engine.md#scalemode_nearest)

#### Defined in

packages/dev/core/src/Engines/engine.ts:257

___

### TEXTUREFORMAT\_ALPHA

▪ `Static` `Readonly` **TEXTUREFORMAT\_ALPHA**: ``0``

ALPHA

#### Inherited from

[Engine](Engine.md).[TEXTUREFORMAT_ALPHA](Engine.md#textureformat_alpha)

#### Defined in

packages/dev/core/src/Engines/engine.ts:140

___

### TEXTUREFORMAT\_LUMINANCE

▪ `Static` `Readonly` **TEXTUREFORMAT\_LUMINANCE**: ``1``

LUMINANCE

#### Inherited from

[Engine](Engine.md).[TEXTUREFORMAT_LUMINANCE](Engine.md#textureformat_luminance)

#### Defined in

packages/dev/core/src/Engines/engine.ts:142

___

### TEXTUREFORMAT\_LUMINANCE\_ALPHA

▪ `Static` `Readonly` **TEXTUREFORMAT\_LUMINANCE\_ALPHA**: ``2``

LUMINANCE_ALPHA

#### Inherited from

[Engine](Engine.md).[TEXTUREFORMAT_LUMINANCE_ALPHA](Engine.md#textureformat_luminance_alpha)

#### Defined in

packages/dev/core/src/Engines/engine.ts:144

___

### TEXTUREFORMAT\_R

▪ `Static` `Readonly` **TEXTUREFORMAT\_R**: ``6``

RED (2nd reference)

#### Inherited from

[Engine](Engine.md).[TEXTUREFORMAT_R](Engine.md#textureformat_r)

#### Defined in

packages/dev/core/src/Engines/engine.ts:152

___

### TEXTUREFORMAT\_RED

▪ `Static` `Readonly` **TEXTUREFORMAT\_RED**: ``6``

RED

#### Inherited from

[Engine](Engine.md).[TEXTUREFORMAT_RED](Engine.md#textureformat_red)

#### Defined in

packages/dev/core/src/Engines/engine.ts:150

___

### TEXTUREFORMAT\_RED\_INTEGER

▪ `Static` `Readonly` **TEXTUREFORMAT\_RED\_INTEGER**: ``8``

RED_INTEGER

#### Inherited from

[Engine](Engine.md).[TEXTUREFORMAT_RED_INTEGER](Engine.md#textureformat_red_integer)

#### Defined in

packages/dev/core/src/Engines/engine.ts:156

___

### TEXTUREFORMAT\_RG

▪ `Static` `Readonly` **TEXTUREFORMAT\_RG**: ``7``

RG

#### Inherited from

[Engine](Engine.md).[TEXTUREFORMAT_RG](Engine.md#textureformat_rg)

#### Defined in

packages/dev/core/src/Engines/engine.ts:154

___

### TEXTUREFORMAT\_RGB

▪ `Static` `Readonly` **TEXTUREFORMAT\_RGB**: ``4``

RGB

#### Inherited from

[Engine](Engine.md).[TEXTUREFORMAT_RGB](Engine.md#textureformat_rgb)

#### Defined in

packages/dev/core/src/Engines/engine.ts:146

___

### TEXTUREFORMAT\_RGBA

▪ `Static` `Readonly` **TEXTUREFORMAT\_RGBA**: ``5``

RGBA

#### Inherited from

[Engine](Engine.md).[TEXTUREFORMAT_RGBA](Engine.md#textureformat_rgba)

#### Defined in

packages/dev/core/src/Engines/engine.ts:148

___

### TEXTUREFORMAT\_RGBA\_INTEGER

▪ `Static` `Readonly` **TEXTUREFORMAT\_RGBA\_INTEGER**: ``11``

RGBA_INTEGER

#### Inherited from

[Engine](Engine.md).[TEXTUREFORMAT_RGBA_INTEGER](Engine.md#textureformat_rgba_integer)

#### Defined in

packages/dev/core/src/Engines/engine.ts:164

___

### TEXTUREFORMAT\_RGB\_INTEGER

▪ `Static` `Readonly` **TEXTUREFORMAT\_RGB\_INTEGER**: ``10``

RGB_INTEGER

#### Inherited from

[Engine](Engine.md).[TEXTUREFORMAT_RGB_INTEGER](Engine.md#textureformat_rgb_integer)

#### Defined in

packages/dev/core/src/Engines/engine.ts:162

___

### TEXTUREFORMAT\_RG\_INTEGER

▪ `Static` `Readonly` **TEXTUREFORMAT\_RG\_INTEGER**: ``9``

RG_INTEGER

#### Inherited from

[Engine](Engine.md).[TEXTUREFORMAT_RG_INTEGER](Engine.md#textureformat_rg_integer)

#### Defined in

packages/dev/core/src/Engines/engine.ts:160

___

### TEXTUREFORMAT\_R\_INTEGER

▪ `Static` `Readonly` **TEXTUREFORMAT\_R\_INTEGER**: ``8``

RED_INTEGER (2nd reference)

#### Inherited from

[Engine](Engine.md).[TEXTUREFORMAT_R_INTEGER](Engine.md#textureformat_r_integer)

#### Defined in

packages/dev/core/src/Engines/engine.ts:158

___

### TEXTURETYPE\_BYTE

▪ `Static` `Readonly` **TEXTURETYPE\_BYTE**: ``3``

BYTE

#### Inherited from

[Engine](Engine.md).[TEXTURETYPE_BYTE](Engine.md#texturetype_byte)

#### Defined in

packages/dev/core/src/Engines/engine.ts:175

___

### TEXTURETYPE\_FLOAT

▪ `Static` `Readonly` **TEXTURETYPE\_FLOAT**: ``1``

FLOAT

#### Inherited from

[Engine](Engine.md).[TEXTURETYPE_FLOAT](Engine.md#texturetype_float)

#### Defined in

packages/dev/core/src/Engines/engine.ts:171

___

### TEXTURETYPE\_FLOAT\_32\_UNSIGNED\_INT\_24\_8\_REV

▪ `Static` `Readonly` **TEXTURETYPE\_FLOAT\_32\_UNSIGNED\_INT\_24\_8\_REV**: ``15``

FLOAT_32_UNSIGNED_INT_24_8_REV

#### Inherited from

[Engine](Engine.md).[TEXTURETYPE_FLOAT_32_UNSIGNED_INT_24_8_REV](Engine.md#texturetype_float_32_unsigned_int_24_8_rev)

#### Defined in

packages/dev/core/src/Engines/engine.ts:199

___

### TEXTURETYPE\_HALF\_FLOAT

▪ `Static` `Readonly` **TEXTURETYPE\_HALF\_FLOAT**: ``2``

HALF_FLOAT

#### Inherited from

[Engine](Engine.md).[TEXTURETYPE_HALF_FLOAT](Engine.md#texturetype_half_float)

#### Defined in

packages/dev/core/src/Engines/engine.ts:173

___

### TEXTURETYPE\_INT

▪ `Static` `Readonly` **TEXTURETYPE\_INT**: ``6``

INT

#### Inherited from

[Engine](Engine.md).[TEXTURETYPE_INT](Engine.md#texturetype_int)

#### Defined in

packages/dev/core/src/Engines/engine.ts:181

___

### TEXTURETYPE\_SHORT

▪ `Static` `Readonly` **TEXTURETYPE\_SHORT**: ``4``

SHORT

#### Inherited from

[Engine](Engine.md).[TEXTURETYPE_SHORT](Engine.md#texturetype_short)

#### Defined in

packages/dev/core/src/Engines/engine.ts:177

___

### TEXTURETYPE\_UNSIGNED\_BYTE

▪ `Static` `Readonly` **TEXTURETYPE\_UNSIGNED\_BYTE**: ``0``

UNSIGNED_BYTE

#### Inherited from

[Engine](Engine.md).[TEXTURETYPE_UNSIGNED_BYTE](Engine.md#texturetype_unsigned_byte)

#### Defined in

packages/dev/core/src/Engines/engine.ts:167

___

### TEXTURETYPE\_UNSIGNED\_INT

▪ `Static` `Readonly` **TEXTURETYPE\_UNSIGNED\_INT**: ``0``

UNSIGNED_BYTE (2nd reference)

#### Inherited from

[Engine](Engine.md).[TEXTURETYPE_UNSIGNED_INT](Engine.md#texturetype_unsigned_int)

#### Defined in

packages/dev/core/src/Engines/engine.ts:169

___

### TEXTURETYPE\_UNSIGNED\_INTEGER

▪ `Static` `Readonly` **TEXTURETYPE\_UNSIGNED\_INTEGER**: ``7``

UNSIGNED_INT

#### Inherited from

[Engine](Engine.md).[TEXTURETYPE_UNSIGNED_INTEGER](Engine.md#texturetype_unsigned_integer)

#### Defined in

packages/dev/core/src/Engines/engine.ts:183

___

### TEXTURETYPE\_UNSIGNED\_INT\_10F\_11F\_11F\_REV

▪ `Static` `Readonly` **TEXTURETYPE\_UNSIGNED\_INT\_10F\_11F\_11F\_REV**: ``13``

UNSIGNED_INT_10F_11F_11F_REV

#### Inherited from

[Engine](Engine.md).[TEXTURETYPE_UNSIGNED_INT_10F_11F_11F_REV](Engine.md#texturetype_unsigned_int_10f_11f_11f_rev)

#### Defined in

packages/dev/core/src/Engines/engine.ts:195

___

### TEXTURETYPE\_UNSIGNED\_INT\_24\_8

▪ `Static` `Readonly` **TEXTURETYPE\_UNSIGNED\_INT\_24\_8**: ``12``

UNSIGNED_INT_24_8

#### Inherited from

[Engine](Engine.md).[TEXTURETYPE_UNSIGNED_INT_24_8](Engine.md#texturetype_unsigned_int_24_8)

#### Defined in

packages/dev/core/src/Engines/engine.ts:193

___

### TEXTURETYPE\_UNSIGNED\_INT\_2\_10\_10\_10\_REV

▪ `Static` `Readonly` **TEXTURETYPE\_UNSIGNED\_INT\_2\_10\_10\_10\_REV**: ``11``

UNSIGNED_INT_2_10_10_10_REV

#### Inherited from

[Engine](Engine.md).[TEXTURETYPE_UNSIGNED_INT_2_10_10_10_REV](Engine.md#texturetype_unsigned_int_2_10_10_10_rev)

#### Defined in

packages/dev/core/src/Engines/engine.ts:191

___

### TEXTURETYPE\_UNSIGNED\_INT\_5\_9\_9\_9\_REV

▪ `Static` `Readonly` **TEXTURETYPE\_UNSIGNED\_INT\_5\_9\_9\_9\_REV**: ``14``

UNSIGNED_INT_5_9_9_9_REV

#### Inherited from

[Engine](Engine.md).[TEXTURETYPE_UNSIGNED_INT_5_9_9_9_REV](Engine.md#texturetype_unsigned_int_5_9_9_9_rev)

#### Defined in

packages/dev/core/src/Engines/engine.ts:197

___

### TEXTURETYPE\_UNSIGNED\_SHORT

▪ `Static` `Readonly` **TEXTURETYPE\_UNSIGNED\_SHORT**: ``5``

UNSIGNED_SHORT

#### Inherited from

[Engine](Engine.md).[TEXTURETYPE_UNSIGNED_SHORT](Engine.md#texturetype_unsigned_short)

#### Defined in

packages/dev/core/src/Engines/engine.ts:179

___

### TEXTURETYPE\_UNSIGNED\_SHORT\_4\_4\_4\_4

▪ `Static` `Readonly` **TEXTURETYPE\_UNSIGNED\_SHORT\_4\_4\_4\_4**: ``8``

UNSIGNED_SHORT_4_4_4_4

#### Inherited from

[Engine](Engine.md).[TEXTURETYPE_UNSIGNED_SHORT_4_4_4_4](Engine.md#texturetype_unsigned_short_4_4_4_4)

#### Defined in

packages/dev/core/src/Engines/engine.ts:185

___

### TEXTURETYPE\_UNSIGNED\_SHORT\_5\_5\_5\_1

▪ `Static` `Readonly` **TEXTURETYPE\_UNSIGNED\_SHORT\_5\_5\_5\_1**: ``9``

UNSIGNED_SHORT_5_5_5_1

#### Inherited from

[Engine](Engine.md).[TEXTURETYPE_UNSIGNED_SHORT_5_5_5_1](Engine.md#texturetype_unsigned_short_5_5_5_1)

#### Defined in

packages/dev/core/src/Engines/engine.ts:187

___

### TEXTURETYPE\_UNSIGNED\_SHORT\_5\_6\_5

▪ `Static` `Readonly` **TEXTURETYPE\_UNSIGNED\_SHORT\_5\_6\_5**: ``10``

UNSIGNED_SHORT_5_6_5

#### Inherited from

[Engine](Engine.md).[TEXTURETYPE_UNSIGNED_SHORT_5_6_5](Engine.md#texturetype_unsigned_short_5_6_5)

#### Defined in

packages/dev/core/src/Engines/engine.ts:189

___

### TEXTURE\_BILINEAR\_SAMPLINGMODE

▪ `Static` `Readonly` **TEXTURE\_BILINEAR\_SAMPLINGMODE**: ``2``

Bilinear is mag = linear and min = linear and mip = nearest

#### Inherited from

[Engine](Engine.md).[TEXTURE_BILINEAR_SAMPLINGMODE](Engine.md#texture_bilinear_samplingmode)

#### Defined in

packages/dev/core/src/Engines/engine.ts:204

___

### TEXTURE\_CLAMP\_ADDRESSMODE

▪ `Static` `Readonly` **TEXTURE\_CLAMP\_ADDRESSMODE**: ``0``

Texture is not repeating outside of 0..1 UVs

#### Inherited from

[Engine](Engine.md).[TEXTURE_CLAMP_ADDRESSMODE](Engine.md#texture_clamp_addressmode)

#### Defined in

packages/dev/core/src/Engines/engine.ts:133

___

### TEXTURE\_CUBIC\_MODE

▪ `Static` `Readonly` **TEXTURE\_CUBIC\_MODE**: ``3``

Cubic coordinates mode

#### Inherited from

[Engine](Engine.md).[TEXTURE_CUBIC_MODE](Engine.md#texture_cubic_mode)

#### Defined in

packages/dev/core/src/Engines/engine.ts:239

___

### TEXTURE\_EQUIRECTANGULAR\_MODE

▪ `Static` `Readonly` **TEXTURE\_EQUIRECTANGULAR\_MODE**: ``7``

Equirectangular coordinates mode

#### Inherited from

[Engine](Engine.md).[TEXTURE_EQUIRECTANGULAR_MODE](Engine.md#texture_equirectangular_mode)

#### Defined in

packages/dev/core/src/Engines/engine.ts:247

___

### TEXTURE\_EXPLICIT\_MODE

▪ `Static` `Readonly` **TEXTURE\_EXPLICIT\_MODE**: ``0``

Explicit coordinates mode

#### Inherited from

[Engine](Engine.md).[TEXTURE_EXPLICIT_MODE](Engine.md#texture_explicit_mode)

#### Defined in

packages/dev/core/src/Engines/engine.ts:233

___

### TEXTURE\_FIXED\_EQUIRECTANGULAR\_MIRRORED\_MODE

▪ `Static` `Readonly` **TEXTURE\_FIXED\_EQUIRECTANGULAR\_MIRRORED\_MODE**: ``9``

Equirectangular Fixed Mirrored coordinates mode

#### Inherited from

[Engine](Engine.md).[TEXTURE_FIXED_EQUIRECTANGULAR_MIRRORED_MODE](Engine.md#texture_fixed_equirectangular_mirrored_mode)

#### Defined in

packages/dev/core/src/Engines/engine.ts:251

___

### TEXTURE\_FIXED\_EQUIRECTANGULAR\_MODE

▪ `Static` `Readonly` **TEXTURE\_FIXED\_EQUIRECTANGULAR\_MODE**: ``8``

Equirectangular Fixed coordinates mode

#### Inherited from

[Engine](Engine.md).[TEXTURE_FIXED_EQUIRECTANGULAR_MODE](Engine.md#texture_fixed_equirectangular_mode)

#### Defined in

packages/dev/core/src/Engines/engine.ts:249

___

### TEXTURE\_INVCUBIC\_MODE

▪ `Static` `Readonly` **TEXTURE\_INVCUBIC\_MODE**: ``6``

Inverse Cubic coordinates mode

#### Inherited from

[Engine](Engine.md).[TEXTURE_INVCUBIC_MODE](Engine.md#texture_invcubic_mode)

#### Defined in

packages/dev/core/src/Engines/engine.ts:245

___

### TEXTURE\_LINEAR\_LINEAR

▪ `Static` `Readonly` **TEXTURE\_LINEAR\_LINEAR**: ``2``

mag = linear and min = linear and mip = none

#### Inherited from

[Engine](Engine.md).[TEXTURE_LINEAR_LINEAR](Engine.md#texture_linear_linear)

#### Defined in

packages/dev/core/src/Engines/engine.ts:228

___

### TEXTURE\_LINEAR\_LINEAR\_MIPLINEAR

▪ `Static` `Readonly` **TEXTURE\_LINEAR\_LINEAR\_MIPLINEAR**: ``3``

Trilinear is mag = linear and min = linear and mip = linear

#### Inherited from

[Engine](Engine.md).[TEXTURE_LINEAR_LINEAR_MIPLINEAR](Engine.md#texture_linear_linear_miplinear)

#### Defined in

packages/dev/core/src/Engines/engine.ts:212

___

### TEXTURE\_LINEAR\_LINEAR\_MIPNEAREST

▪ `Static` `Readonly` **TEXTURE\_LINEAR\_LINEAR\_MIPNEAREST**: ``11``

Bilinear is mag = linear and min = linear and mip = nearest

#### Inherited from

[Engine](Engine.md).[TEXTURE_LINEAR_LINEAR_MIPNEAREST](Engine.md#texture_linear_linear_mipnearest)

#### Defined in

packages/dev/core/src/Engines/engine.ts:210

___

### TEXTURE\_LINEAR\_NEAREST

▪ `Static` `Readonly` **TEXTURE\_LINEAR\_NEAREST**: ``12``

mag = linear and min = nearest and mip = none

#### Inherited from

[Engine](Engine.md).[TEXTURE_LINEAR_NEAREST](Engine.md#texture_linear_nearest)

#### Defined in

packages/dev/core/src/Engines/engine.ts:230

___

### TEXTURE\_LINEAR\_NEAREST\_MIPLINEAR

▪ `Static` `Readonly` **TEXTURE\_LINEAR\_NEAREST\_MIPLINEAR**: ``10``

mag = linear and min = nearest and mip = linear

#### Inherited from

[Engine](Engine.md).[TEXTURE_LINEAR_NEAREST_MIPLINEAR](Engine.md#texture_linear_nearest_miplinear)

#### Defined in

packages/dev/core/src/Engines/engine.ts:226

___

### TEXTURE\_LINEAR\_NEAREST\_MIPNEAREST

▪ `Static` `Readonly` **TEXTURE\_LINEAR\_NEAREST\_MIPNEAREST**: ``9``

mag = linear and min = nearest and mip = nearest

#### Inherited from

[Engine](Engine.md).[TEXTURE_LINEAR_NEAREST_MIPNEAREST](Engine.md#texture_linear_nearest_mipnearest)

#### Defined in

packages/dev/core/src/Engines/engine.ts:224

___

### TEXTURE\_MIRROR\_ADDRESSMODE

▪ `Static` `Readonly` **TEXTURE\_MIRROR\_ADDRESSMODE**: ``2``

Texture is repeating and mirrored

#### Inherited from

[Engine](Engine.md).[TEXTURE_MIRROR_ADDRESSMODE](Engine.md#texture_mirror_addressmode)

#### Defined in

packages/dev/core/src/Engines/engine.ts:137

___

### TEXTURE\_NEAREST\_LINEAR

▪ `Static` `Readonly` **TEXTURE\_NEAREST\_LINEAR**: ``7``

mag = nearest and min = linear and mip = none

#### Inherited from

[Engine](Engine.md).[TEXTURE_NEAREST_LINEAR](Engine.md#texture_nearest_linear)

#### Defined in

packages/dev/core/src/Engines/engine.ts:220

___

### TEXTURE\_NEAREST\_LINEAR\_MIPLINEAR

▪ `Static` `Readonly` **TEXTURE\_NEAREST\_LINEAR\_MIPLINEAR**: ``6``

mag = nearest and min = linear and mip = linear

#### Inherited from

[Engine](Engine.md).[TEXTURE_NEAREST_LINEAR_MIPLINEAR](Engine.md#texture_nearest_linear_miplinear)

#### Defined in

packages/dev/core/src/Engines/engine.ts:218

___

### TEXTURE\_NEAREST\_LINEAR\_MIPNEAREST

▪ `Static` `Readonly` **TEXTURE\_NEAREST\_LINEAR\_MIPNEAREST**: ``5``

mag = nearest and min = linear and mip = nearest

#### Inherited from

[Engine](Engine.md).[TEXTURE_NEAREST_LINEAR_MIPNEAREST](Engine.md#texture_nearest_linear_mipnearest)

#### Defined in

packages/dev/core/src/Engines/engine.ts:216

___

### TEXTURE\_NEAREST\_NEAREST

▪ `Static` `Readonly` **TEXTURE\_NEAREST\_NEAREST**: ``1``

mag = nearest and min = nearest and mip = none

#### Inherited from

[Engine](Engine.md).[TEXTURE_NEAREST_NEAREST](Engine.md#texture_nearest_nearest)

#### Defined in

packages/dev/core/src/Engines/engine.ts:222

___

### TEXTURE\_NEAREST\_NEAREST\_MIPLINEAR

▪ `Static` `Readonly` **TEXTURE\_NEAREST\_NEAREST\_MIPLINEAR**: ``8``

nearest is mag = nearest and min = nearest and mip = linear

#### Inherited from

[Engine](Engine.md).[TEXTURE_NEAREST_NEAREST_MIPLINEAR](Engine.md#texture_nearest_nearest_miplinear)

#### Defined in

packages/dev/core/src/Engines/engine.ts:208

___

### TEXTURE\_NEAREST\_NEAREST\_MIPNEAREST

▪ `Static` `Readonly` **TEXTURE\_NEAREST\_NEAREST\_MIPNEAREST**: ``4``

mag = nearest and min = nearest and mip = nearest

#### Inherited from

[Engine](Engine.md).[TEXTURE_NEAREST_NEAREST_MIPNEAREST](Engine.md#texture_nearest_nearest_mipnearest)

#### Defined in

packages/dev/core/src/Engines/engine.ts:214

___

### TEXTURE\_NEAREST\_SAMPLINGMODE

▪ `Static` `Readonly` **TEXTURE\_NEAREST\_SAMPLINGMODE**: ``1``

nearest is mag = nearest and min = nearest and mip = none

#### Inherited from

[Engine](Engine.md).[TEXTURE_NEAREST_SAMPLINGMODE](Engine.md#texture_nearest_samplingmode)

#### Defined in

packages/dev/core/src/Engines/engine.ts:202

___

### TEXTURE\_PLANAR\_MODE

▪ `Static` `Readonly` **TEXTURE\_PLANAR\_MODE**: ``2``

Planar coordinates mode

#### Inherited from

[Engine](Engine.md).[TEXTURE_PLANAR_MODE](Engine.md#texture_planar_mode)

#### Defined in

packages/dev/core/src/Engines/engine.ts:237

___

### TEXTURE\_PROJECTION\_MODE

▪ `Static` `Readonly` **TEXTURE\_PROJECTION\_MODE**: ``4``

Projection coordinates mode

#### Inherited from

[Engine](Engine.md).[TEXTURE_PROJECTION_MODE](Engine.md#texture_projection_mode)

#### Defined in

packages/dev/core/src/Engines/engine.ts:241

___

### TEXTURE\_SKYBOX\_MODE

▪ `Static` `Readonly` **TEXTURE\_SKYBOX\_MODE**: ``5``

Skybox coordinates mode

#### Inherited from

[Engine](Engine.md).[TEXTURE_SKYBOX_MODE](Engine.md#texture_skybox_mode)

#### Defined in

packages/dev/core/src/Engines/engine.ts:243

___

### TEXTURE\_SPHERICAL\_MODE

▪ `Static` `Readonly` **TEXTURE\_SPHERICAL\_MODE**: ``1``

Spherical coordinates mode

#### Inherited from

[Engine](Engine.md).[TEXTURE_SPHERICAL_MODE](Engine.md#texture_spherical_mode)

#### Defined in

packages/dev/core/src/Engines/engine.ts:235

___

### TEXTURE\_TRILINEAR\_SAMPLINGMODE

▪ `Static` `Readonly` **TEXTURE\_TRILINEAR\_SAMPLINGMODE**: ``3``

Trilinear is mag = linear and min = linear and mip = linear

#### Inherited from

[Engine](Engine.md).[TEXTURE_TRILINEAR_SAMPLINGMODE](Engine.md#texture_trilinear_samplingmode)

#### Defined in

packages/dev/core/src/Engines/engine.ts:206

___

### TEXTURE\_WRAP\_ADDRESSMODE

▪ `Static` `Readonly` **TEXTURE\_WRAP\_ADDRESSMODE**: ``1``

Texture is repeating outside of 0..1 UVs

#### Inherited from

[Engine](Engine.md).[TEXTURE_WRAP_ADDRESSMODE](Engine.md#texture_wrap_addressmode)

#### Defined in

packages/dev/core/src/Engines/engine.ts:135

___

### \_RenderPassIdCounter

▪ `Static` `Protected` **\_RenderPassIdCounter**: `number` = `0`

#### Inherited from

[Engine](Engine.md).[_RenderPassIdCounter](Engine.md#_renderpassidcounter)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1576

___

### \_RescalePostProcessFactory

▪ `Static` **\_RescalePostProcessFactory**: [`Nullable`](../modules.md#nullable)(`engine`: [`Engine`](Engine.md)) => [`PostProcess`](PostProcess.md) = `null`

Method called to create the default rescale post process on each engine.

#### Inherited from

[Engine](Engine.md).[_RescalePostProcessFactory](Engine.md#_rescalepostprocessfactory)

#### Defined in

packages/dev/core/src/Engines/engine.ts:384

___

### audioEngine

▪ `Static` **audioEngine**: [`Nullable`](../modules.md#nullable)[`IAudioEngine`](../interfaces/IAudioEngine.md)

Gets the audio engine

**`See`**

https://doc.babylonjs.com/how_to/playing_sounds_and_music

**`Ignorenaming`**

#### Inherited from

[Engine](Engine.md).[audioEngine](Engine.md#audioengine)

#### Defined in

packages/dev/core/src/Engines/engine.ts:479

## Accessors

### \_supportsHardwareTextureRescaling

• `Protected` `get` **_supportsHardwareTextureRescaling**(): `boolean`

#### Returns

`boolean`

#### Inherited from

Engine.\_supportsHardwareTextureRescaling

#### Defined in

packages/dev/core/src/Engines/engine.ts:506

___

### activeRenderLoops

• `get` **activeRenderLoops**(): () => `void`[]

Gets the list of current active render loop functions

#### Returns

() => `void`[]

an array with the current render loop functions

#### Inherited from

Engine.activeRenderLoops

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:430

___

### alphaState

• `get` **alphaState**(): `AlphaState`

Gets the alpha state manager

#### Returns

`AlphaState`

#### Inherited from

Engine.alphaState

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:3553

___

### compatibilityMode

• `get` **compatibilityMode**(): `boolean`

(WebGPU only) True (default) to be in compatibility mode, meaning rendering all existing scenes without artifacts (same rendering than WebGL).
Setting the property to false will improve performances but may not work in some scenes if some precautions are not taken.
See https://doc.babylonjs.com/advanced_topics/webGPU/webGPUOptimization/webGPUNonCompatibilityMode for more details

#### Returns

`boolean`

#### Inherited from

Engine.compatibilityMode

#### Defined in

packages/dev/core/src/Engines/engine.ts:552

• `set` **compatibilityMode**(`mode`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `mode` | `boolean` |

#### Returns

`void`

#### Inherited from

Engine.compatibilityMode

#### Defined in

packages/dev/core/src/Engines/engine.ts:556

___

### currentViewport

• `get` **currentViewport**(): [`Nullable`](../modules.md#nullable)`IViewportLike`

Gets the current viewport

#### Returns

[`Nullable`](../modules.md#nullable)`IViewportLike`

#### Inherited from

Engine.currentViewport

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:587

___

### depthCullingState

• `get` **depthCullingState**(): `DepthCullingState`

Gets the depth culling state manager

#### Returns

`DepthCullingState`

#### Inherited from

Engine.depthCullingState

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:3546

___

### description

• `get` **description**(): `string`

Returns a string describing the current engine

#### Returns

`string`

#### Inherited from

Engine.description

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:217

___

### doNotHandleContextLost

• `get` **doNotHandleContextLost**(): `boolean`

Gets or sets a boolean indicating if resources should be retained to be able to handle context lost events

**`See`**

https://doc.babylonjs.com/how_to/optimizing_your_scene#handling-webgl-context-lost

#### Returns

`boolean`

#### Inherited from

Engine.doNotHandleContextLost

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:454

• `set` **doNotHandleContextLost**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

Engine.doNotHandleContextLost

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:458

___

### emptyCubeTexture

• `get` **emptyCubeTexture**(): [`InternalTexture`](InternalTexture.md)

Gets the default empty cube texture

#### Returns

[`InternalTexture`](InternalTexture.md)

#### Inherited from

Engine.emptyCubeTexture

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:636

___

### emptyTexture

• `get` **emptyTexture**(): [`InternalTexture`](InternalTexture.md)

Gets the default empty texture

#### Returns

[`InternalTexture`](InternalTexture.md)

#### Inherited from

Engine.emptyTexture

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:594

___

### emptyTexture2DArray

• `get` **emptyTexture2DArray**(): [`InternalTexture`](InternalTexture.md)

Gets the default empty 2D array texture

#### Returns

[`InternalTexture`](InternalTexture.md)

#### Inherited from

Engine.emptyTexture2DArray

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:616

___

### emptyTexture3D

• `get` **emptyTexture3D**(): [`InternalTexture`](InternalTexture.md)

Gets the default empty 3D texture

#### Returns

[`InternalTexture`](InternalTexture.md)

#### Inherited from

Engine.emptyTexture3D

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:605

___

### frameId

• `get` **frameId**(): `number`

Gets the current frame id

#### Returns

`number`

#### Inherited from

Engine.frameId

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:351

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

#### Inherited from

Engine.framebufferDimensionsObject

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:580

___

### isStencilEnable

• `get` **isStencilEnable**(): `boolean`

Returns true if the stencil buffer has been enabled through the creation option of the context.

#### Returns

`boolean`

#### Inherited from

Engine.isStencilEnable

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1425

___

### isWebGPU

• `get` **isWebGPU**(): `boolean`

Gets a boolean indicating if the engine runs in WebGPU or not.

#### Returns

`boolean`

#### Inherited from

Engine.isWebGPU

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:669

___

### loadingScreen

• `get` **loadingScreen**(): [`ILoadingScreen`](../interfaces/ILoadingScreen.md)

Gets the current loading screen object

**`See`**

https://doc.babylonjs.com/how_to/creating_a_custom_loading_screen

#### Returns

[`ILoadingScreen`](../interfaces/ILoadingScreen.md)

#### Inherited from

Engine.loadingScreen

#### Defined in

packages/dev/core/src/Engines/engine.ts:2011

• `set` **loadingScreen**(`loadingScreen`): `void`

Sets the current loading screen object

**`See`**

https://doc.babylonjs.com/how_to/creating_a_custom_loading_screen

#### Parameters

| Name | Type |
| :------ | :------ |
| `loadingScreen` | [`ILoadingScreen`](../interfaces/ILoadingScreen.md) |

#### Returns

`void`

#### Inherited from

Engine.loadingScreen

#### Defined in

packages/dev/core/src/Engines/engine.ts:2022

___

### loadingUIBackgroundColor

• `set` **loadingUIBackgroundColor**(`color`): `void`

Sets the current loading screen background color

**`See`**

https://doc.babylonjs.com/how_to/creating_a_custom_loading_screen

#### Parameters

| Name | Type |
| :------ | :------ |
| `color` | `string` |

#### Returns

`void`

#### Inherited from

Engine.loadingUIBackgroundColor

#### Defined in

packages/dev/core/src/Engines/engine.ts:2038

___

### loadingUIText

• `set` **loadingUIText**(`_`): `void`

Sets the current loading screen text

**`See`**

https://doc.babylonjs.com/how_to/creating_a_custom_loading_screen

#### Parameters

| Name | Type |
| :------ | :------ |
| `_` | `string` |

#### Returns

`void`

#### Overrides

Engine.loadingUIText

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:983

___

### name

• `get` **name**(): `string`

Gets or sets the name of the engine

#### Returns

`string`

#### Inherited from

Engine.name

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:233

• `set` **name**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `string` |

#### Returns

`void`

#### Inherited from

Engine.name

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:237

___

### needPOTTextures

• `get` **needPOTTextures**(): `boolean`

Gets a boolean indicating that only power of 2 textures are supported
Please note that you can still use non power of 2 textures but in this case the engine will forcefully convert them

#### Returns

`boolean`

#### Inherited from

Engine.needPOTTextures

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:398

___

### performanceMonitor

• `get` **performanceMonitor**(): [`PerformanceMonitor`](PerformanceMonitor.md)

Gets the performance monitor attached to this engine

**`See`**

https://doc.babylonjs.com/how_to/optimizing_your_scene#engineinstrumentation

#### Returns

[`PerformanceMonitor`](PerformanceMonitor.md)

#### Inherited from

Engine.performanceMonitor

#### Defined in

packages/dev/core/src/Engines/engine.ts:530

___

### shaderPlatformName

• `get` **shaderPlatformName**(): `string`

Gets the shader platform name used by the effects.

#### Returns

`string`

#### Inherited from

Engine.shaderPlatformName

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:678

___

### snapshotRendering

• `get` **snapshotRendering**(): `boolean`

Enables or disables the snapshot rendering mode
Note that the WebGL engine does not support snapshot rendering so setting the value won't have any effect for this engine

#### Returns

`boolean`

#### Inherited from

Engine.snapshotRendering

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:686

• `set` **snapshotRendering**(`activate`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `activate` | `boolean` |

#### Returns

`void`

#### Inherited from

Engine.snapshotRendering

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:690

___

### snapshotRenderingMode

• `get` **snapshotRenderingMode**(): `number`

Gets or sets the snapshot rendering mode

#### Returns

`number`

#### Inherited from

Engine.snapshotRenderingMode

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:698

• `set` **snapshotRenderingMode**(`mode`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `mode` | `number` |

#### Returns

`void`

#### Inherited from

Engine.snapshotRenderingMode

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:702

___

### stencilState

• `get` **stencilState**(): `StencilState`

Gets the stencil state manager

#### Returns

`StencilState`

#### Inherited from

Engine.stencilState

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:3560

___

### stencilStateComposer

• `get` **stencilStateComposer**(): `StencilStateComposer`

Gets the stencil state composer

#### Returns

`StencilStateComposer`

#### Inherited from

Engine.stencilStateComposer

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:3567

___

### supportsUniformBuffers

• `get` **supportsUniformBuffers**(): `boolean`

Gets a boolean indicating that the engine supports uniform buffers

**`See`**

https://doc.babylonjs.com/features/webgl2#uniform-buffer-objets

#### Returns

`boolean`

#### Inherited from

Engine.supportsUniformBuffers

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:364

___

### useExactSrgbConversions

• `get` **useExactSrgbConversions**(): `boolean`

Gets a boolean indicating if the exact sRGB conversions or faster approximations are used for converting to and from linear space.

#### Returns

`boolean`

#### Inherited from

Engine.useExactSrgbConversions

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:710

___

### useReverseDepthBuffer

• `get` **useReverseDepthBuffer**(): `boolean`

Gets or sets a boolean indicating if depth buffer should be reverse, going from far to near.
This can provide greater z depth for distant objects.

#### Returns

`boolean`

#### Inherited from

Engine.useReverseDepthBuffer

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:309

• `set` **useReverseDepthBuffer**(`useReverse`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `useReverse` | `boolean` |

#### Returns

`void`

#### Inherited from

Engine.useReverseDepthBuffer

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:313

___

### version

• `get` **version**(): `number`

Returns the version of the engine

#### Returns

`number`

#### Inherited from

Engine.version

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:244

___

### webGLVersion

• `get` **webGLVersion**(): `number`

Gets version of the current webGL context
Keep it for back compat - use version instead

#### Returns

`number`

#### Inherited from

Engine.webGLVersion

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1410

___

### HasMajorPerformanceCaveat

• `Static` `get` **HasMajorPerformanceCaveat**(): `boolean`

Gets a boolean indicating if the engine can be instantiated on a performant device (ie. if a webGL context can be found and it does not use a slow implementation)

#### Returns

`boolean`

#### Inherited from

Engine.HasMajorPerformanceCaveat

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:5833

___

### Instances

• `Static` `get` **Instances**(): [`Engine`](Engine.md)[]

Gets the list of created engines

#### Returns

[`Engine`](Engine.md)[]

#### Inherited from

Engine.Instances

#### Defined in

packages/dev/core/src/Engines/engine.ts:277

___

### IsSupported

• `Static` `get` **IsSupported**(): `boolean`

Gets a boolean indicating if the engine can be instantiated (ie. if a webGL context can be found)

#### Returns

`boolean`

#### Inherited from

Engine.IsSupported

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:5801

___

### IsSupportedAsync

• `Static` `get` **IsSupportedAsync**(): `Promise``boolean`

Gets a Promise indicating if the engine can be instantiated (ie. if a webGL context can be found)

#### Returns

`Promise``boolean`

#### Inherited from

Engine.IsSupportedAsync

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:5794

___

### LastCreatedEngine

• `Static` `get` **LastCreatedEngine**(): [`Nullable`](../modules.md#nullable)[`Engine`](Engine.md)

Gets the latest created engine

#### Returns

[`Nullable`](../modules.md#nullable)[`Engine`](Engine.md)

#### Inherited from

Engine.LastCreatedEngine

#### Defined in

packages/dev/core/src/Engines/engine.ts:284

___

### LastCreatedScene

• `Static` `get` **LastCreatedScene**(): [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md)

Gets the latest created scene

#### Returns

[`Nullable`](../modules.md#nullable)[`Scene`](Scene.md)

#### Inherited from

Engine.LastCreatedScene

#### Defined in

packages/dev/core/src/Engines/engine.ts:291

___

### NpmPackage

• `Static` `get` **NpmPackage**(): `string`

Returns the current npm package of the sdk

#### Returns

`string`

#### Inherited from

Engine.NpmPackage

#### Defined in

packages/dev/core/src/Engines/engine.ts:265

___

### ShadersRepository

• `Static` `get` **ShadersRepository**(): `string`

Gets or sets the relative url used to load shaders if using the engine in non-minified mode

#### Returns

`string`

#### Inherited from

Engine.ShadersRepository

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:258

• `Static` `set` **ShadersRepository**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `string` |

#### Returns

`void`

#### Inherited from

Engine.ShadersRepository

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:261

___

### Version

• `Static` `get` **Version**(): `string`

Returns the current version of the framework

#### Returns

`string`

#### Inherited from

Engine.Version

#### Defined in

packages/dev/core/src/Engines/engine.ts:272

## Methods

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

#### Inherited from

[Engine](Engine.md).[_createDepthStencilCubeTexture](Engine.md#_createdepthstencilcubetexture)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.cubeTexture.ts:24

___

### \_createImageBitmapFromSource

▸ **_createImageBitmapFromSource**(`imageSource`, `options?`): `Promise``ImageBitmap`

Engine abstraction for loading and creating an image bitmap from a given source string.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `imageSource` | `string` | source to load the image from. |
| `options?` | `ImageBitmapOptions` | An object that sets options for the image's extraction. |

#### Returns

`Promise``ImageBitmap`

ImageBitmap.

#### Inherited from

[Engine](Engine.md).[_createImageBitmapFromSource](Engine.md#_createimagebitmapfromsource)

#### Defined in

packages/dev/core/src/Engines/engine.ts:302

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

#### Inherited from

[Engine](Engine.md).[_createShaderProgram](Engine.md#_createshaderprogram)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1499

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

#### Inherited from

[Engine](Engine.md).[_createTextureBase](Engine.md#_createtexturebase)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:3851

___

### \_deleteBuffer

▸ `Protected` **_deleteBuffer**(`buffer`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `buffer` | `WebGLBuffer` |

#### Returns

`void`

#### Overrides

[Engine](Engine.md).[_deleteBuffer](Engine.md#_deletebuffer)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:972

___

### \_deletePipelineContext

▸ **_deletePipelineContext**(`pipelineContext`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `pipelineContext` | [`IPipelineContext`](../interfaces/IPipelineContext.md) |

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[_deletePipelineContext](Engine.md#_deletepipelinecontext)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1470

___

### \_deleteTexture

▸ `Protected` **_deleteTexture**(`texture`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `texture` | [`Nullable`](../modules.md#nullable)`WebGLTexture` |

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[_deleteTexture](Engine.md#_deletetexture)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:4903

___

### \_finalizePipelineContext

▸ `Protected` **_finalizePipelineContext**(`pipelineContext`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `pipelineContext` | `WebGLPipelineContext` |

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[_finalizePipelineContext](Engine.md#_finalizepipelinecontext)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:2999

___

### \_initFeatures

▸ `Protected` **_initFeatures**(): `void`

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[_initFeatures](Engine.md#_initfeatures)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1378

___

### \_initGLContext

▸ `Protected` **_initGLContext**(): `void`

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[_initGLContext](Engine.md#_initglcontext)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1130

___

### \_normalizeIndexData

▸ `Protected` **_normalizeIndexData**(`indices`): `Uint32Array` \| `Uint16Array`

#### Parameters

| Name | Type |
| :------ | :------ |
| `indices` | [`IndicesArray`](../modules.md#indicesarray) |

#### Returns

`Uint32Array` \| `Uint16Array`

#### Inherited from

[Engine](Engine.md).[_normalizeIndexData](Engine.md#_normalizeindexdata)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:2121

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

#### Inherited from

[Engine](Engine.md).[_prepareWebGLTextureContinuation](Engine.md#_preparewebgltexturecontinuation)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:4702

___

### \_rebuildBuffers

▸ `Protected` **_rebuildBuffers**(): `void`

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[_rebuildBuffers](Engine.md#_rebuildbuffers)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1281

___

### \_renderLoop

▸ **_renderLoop**(): `void`

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[_renderLoop](Engine.md#_renderloop)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1307

___

### \_resetIndexBufferBinding

▸ `Protected` **_resetIndexBufferBinding**(): `void`

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[_resetIndexBufferBinding](Engine.md#_resetindexbufferbinding)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:2092

___

### \_restoreEngineAfterContextLost

▸ `Protected` **_restoreEngineAfterContextLost**(`initEngine`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `initEngine` | () => `void` |

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[_restoreEngineAfterContextLost](Engine.md#_restoreengineaftercontextlost)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1022

___

### \_setProgram

▸ `Protected` **_setProgram**(`program`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `program` | `WebGLProgram` |

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[_setProgram](Engine.md#_setprogram)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:4909

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

#### Inherited from

[Engine](Engine.md).[_setTexture](Engine.md#_settexture)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:5062

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

#### Inherited from

[Engine](Engine.md).[_sharedInit](Engine.md#_sharedinit)

#### Defined in

packages/dev/core/src/Engines/engine.ts:669

___

### applyStates

▸ **applyStates**(): `void`

Apply all cached states (depth, culling, stencil and alpha)

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[applyStates](Engine.md#applystates)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:3512

___

### areAllComputeEffectsReady

▸ **areAllComputeEffectsReady**(): `boolean`

Gets a boolean indicating if all created compute effects are ready

#### Returns

`boolean`

true if all effects are ready

#### Inherited from

[Engine](Engine.md).[areAllComputeEffectsReady](Engine.md#areallcomputeeffectsready)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.computeShader.ts:79

___

### areAllEffectsReady

▸ **areAllEffectsReady**(): `boolean`

Gets a boolean indicating if all created effects are ready

#### Returns

`boolean`

true if all effects are ready

#### Overrides

[Engine](Engine.md).[areAllEffectsReady](Engine.md#arealleffectsready)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:904

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

#### Inherited from

[Engine](Engine.md).[attachContextLostEvent](Engine.md#attachcontextlostevent)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:5327

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

#### Inherited from

[Engine](Engine.md).[attachContextRestoredEvent](Engine.md#attachcontextrestoredevent)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:5337

___

### beginFrame

▸ **beginFrame**(): `void`

Begin a new frame

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[beginFrame](Engine.md#beginframe)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1405

___

### beginOcclusionQuery

▸ **beginOcclusionQuery**(`algorithmType`, `query`): `boolean`

Initiates an occlusion query

**`See`**

https://doc.babylonjs.com/features/occlusionquery

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `algorithmType` | `number` | defines the algorithm to use |
| `query` | `OcclusionQuery` | defines the query to use |

#### Returns

`boolean`

the current engine

#### Inherited from

[Engine](Engine.md).[beginOcclusionQuery](Engine.md#beginocclusionquery)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.query.ts:72

___

### beginTransformFeedback

▸ **beginTransformFeedback**(`usePoints`): `void`

Begins a transform feedback operation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `usePoints` | `boolean` | defines if points or triangles must be used |

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[beginTransformFeedback](Engine.md#begintransformfeedback)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.transformFeedback.ts:34

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

#### Inherited from

[Engine](Engine.md).[bindArrayBuffer](Engine.md#bindarraybuffer)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:2151

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

#### Inherited from

[Engine](Engine.md).[bindAttachments](Engine.md#bindattachments)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.multiRender.ts:47

___

### bindBuffers

▸ **bindBuffers**(`vertexBuffers`, `indexBuffer`, `effect`): `void`

Bind webGl buffers directly to the webGL context

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vertexBuffers` | `Object` | defines the vertex buffer to bind |
| `indexBuffer` | [`DataBuffer`](DataBuffer.md) | defines the index buffer to bind |
| `effect` | [`Effect`](Effect.md) | defines the effect associated with the vertex buffer |

#### Returns

`void`

#### Overrides

[Engine](Engine.md).[bindBuffers](Engine.md#bindbuffers)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:572

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

#### Inherited from

[Engine](Engine.md).[bindBuffersDirectly](Engine.md#bindbuffersdirectly)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:2372

___

### bindFramebuffer

▸ **bindFramebuffer**(`rtWrapper`, `faceIndex?`, `requiredWidth?`, `requiredHeight?`, `forceFullscreenViewport?`): `void`

Binds the frame buffer to the specified texture.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `rtWrapper` | [`RenderTargetWrapper`](RenderTargetWrapper.md) | The render target wrapper to render to |
| `faceIndex?` | `number` | The face of the texture to render to in case of cube texture |
| `requiredWidth?` | `number` | The width of the target to render to |
| `requiredHeight?` | `number` | The height of the target to render to |
| `forceFullscreenViewport?` | `boolean` | Forces the viewport to be the entire texture/screen if true |

#### Returns

`void`

#### Overrides

[Engine](Engine.md).[bindFramebuffer](Engine.md#bindframebuffer)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:852

___

### bindIndexBuffer

▸ `Protected` **bindIndexBuffer**(`buffer`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `buffer` | [`Nullable`](../modules.md#nullable)[`DataBuffer`](DataBuffer.md) |

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[bindIndexBuffer](Engine.md#bindindexbuffer)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:2173

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

#### Inherited from

[Engine](Engine.md).[bindInstancesBuffer](Engine.md#bindinstancesbuffer)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:2515

___

### bindMultiviewFramebuffer

▸ **bindMultiviewFramebuffer**(`multiviewTexture`): `void`

Binds a multiview render target wrapper to be drawn to

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `multiviewTexture` | [`RenderTargetWrapper`](RenderTargetWrapper.md) | render target wrapper to bind |

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[bindMultiviewFramebuffer](Engine.md#bindmultiviewframebuffer)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.multiview.ts:28

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

#### Overrides

[Engine](Engine.md).[bindSamplers](Engine.md#bindsamplers)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:297

___

### bindTransformFeedback

▸ **bindTransformFeedback**(`value`): `void`

Bind a webGL transform feedback object to the webgl context

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)`WebGLTransformFeedback` | defines the webGL transform feedback object to bind |

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[bindTransformFeedback](Engine.md#bindtransformfeedback)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.transformFeedback.ts:28

___

### bindTransformFeedbackBuffer

▸ **bindTransformFeedbackBuffer**(`value`): `void`

Bind a webGL buffer for a transform feedback operation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`DataBuffer`](DataBuffer.md) | defines the webGL buffer to bind |

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[bindTransformFeedbackBuffer](Engine.md#bindtransformfeedbackbuffer)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.transformFeedback.ts:52

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

#### Inherited from

[Engine](Engine.md).[bindUniformBlock](Engine.md#binduniformblock)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:2164

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

#### Inherited from

[Engine](Engine.md).[bindUniformBlock](Engine.md#binduniformblock)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.uniformBuffer.ts:56

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

#### Inherited from

[Engine](Engine.md).[bindUniformBuffer](Engine.md#binduniformbuffer)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.uniformBuffer.ts:40

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

#### Inherited from

[Engine](Engine.md).[bindUniformBufferBase](Engine.md#binduniformbufferbase)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.uniformBuffer.ts:48

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

#### Inherited from

[Engine](Engine.md).[bindVertexArrayObject](Engine.md#bindvertexarrayobject)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:2351

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

#### Inherited from

[Engine](Engine.md).[buildTextureLayout](Engine.md#buildtexturelayout)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.multiRender.ts:54

___

### cacheStencilState

▸ **cacheStencilState**(): `void`

Caches the the state of the stencil buffer

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[cacheStencilState](Engine.md#cachestencilstate)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1040

___

### captureGPUFrameTime

▸ **captureGPUFrameTime**(`value`): `void`

Enable or disable the GPU frame time capture

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `boolean` | True to enable, false to disable |

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[captureGPUFrameTime](Engine.md#capturegpuframetime)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.query.ts:106

___

### clear

▸ **clear**(`color`, `backBuffer`, `depth`, `stencil?`): `void`

Clear the current render buffer or the current render target (if any is set up)

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `color` | `IColor4Like` | `undefined` | defines the color to use |
| `backBuffer` | `boolean` | `undefined` | defines if the back buffer must be cleared |
| `depth` | `boolean` | `undefined` | defines if the depth buffer must be cleared |
| `stencil` | `boolean` | `false` | defines if the stencil buffer must be cleared |

#### Returns

`void`

#### Overrides

[Engine](Engine.md).[clear](Engine.md#clear)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:228

___

### clearInternalTexturesCache

▸ **clearInternalTexturesCache**(): `void`

Clears the list of texture accessible through engine.
This can help preventing texture load conflict due to name collision.

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[clearInternalTexturesCache](Engine.md#clearinternaltexturescache)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:3577

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

#### Inherited from

[Engine](Engine.md).[computeDispatch](Engine.md#computedispatch)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.computeShader.ts:65

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

#### Inherited from

[Engine](Engine.md).[createCanvas](Engine.md#createcanvas)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:739

___

### createCanvasImage

▸ **createCanvasImage**(): [`IImage`](../interfaces/IImage.md)

Create an image to use with canvas

#### Returns

[`IImage`](../interfaces/IImage.md)

IImage interface

#### Inherited from

[Engine](Engine.md).[createCanvasImage](Engine.md#createcanvasimage)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:747

___

### createComputeContext

▸ **createComputeContext**(): `undefined` \| `IComputeContext`

Creates a new compute context

#### Returns

`undefined` \| `IComputeContext`

the new context

#### Inherited from

[Engine](Engine.md).[createComputeContext](Engine.md#createcomputecontext)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.computeShader.ts:53

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

#### Inherited from

[Engine](Engine.md).[createComputeEffect](Engine.md#createcomputeeffect)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.computeShader.ts:41

___

### createComputePipelineContext

▸ **createComputePipelineContext**(): `IComputePipelineContext`

Creates a new compute pipeline context

#### Returns

`IComputePipelineContext`

the new pipeline

#### Inherited from

[Engine](Engine.md).[createComputePipelineContext](Engine.md#createcomputepipelinecontext)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.computeShader.ts:47

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

#### Inherited from

[Engine](Engine.md).[createCubeTexture](Engine.md#createcubetexture)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.cubeTexture.ts:44

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

#### Inherited from

[Engine](Engine.md).[createCubeTexture](Engine.md#createcubetexture)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.cubeTexture.ts:73

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

#### Inherited from

[Engine](Engine.md).[createCubeTexture](Engine.md#createcubetexture)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.cubeTexture.ts:99

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

#### Inherited from

[Engine](Engine.md).[createDepthStencilTexture](Engine.md#createdepthstenciltexture)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.renderTarget.ts:36

___

### createDrawContext

▸ **createDrawContext**(): `undefined` \| `IDrawContext`

Creates a new draw context

#### Returns

`undefined` \| `IDrawContext`

the new context

#### Inherited from

[Engine](Engine.md).[createDrawContext](Engine.md#createdrawcontext)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:2965

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

#### Inherited from

[Engine](Engine.md).[createDynamicTexture](Engine.md#createdynamictexture)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.dynamicTexture.ts:16

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

#### Inherited from

[Engine](Engine.md).[createDynamicUniformBuffer](Engine.md#createdynamicuniformbuffer)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.uniformBuffer.ts:24

___

### createDynamicVertexBuffer

▸ **createDynamicVertexBuffer**(`vertices`): [`DataBuffer`](DataBuffer.md)

Creates a dynamic vertex buffer

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vertices` | [`FloatArray`](../modules.md#floatarray) | the data for the dynamic vertex buffer |

#### Returns

[`DataBuffer`](DataBuffer.md)

the new WebGL dynamic buffer

#### Overrides

[Engine](Engine.md).[createDynamicVertexBuffer](Engine.md#createdynamicvertexbuffer)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:883

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

#### Inherited from

[Engine](Engine.md).[createEffect](Engine.md#createeffect)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:2786

___

### createEffectForParticles

▸ **createEffectForParticles**(`fragmentName`, `uniformsNames`, `samplers`, `defines`, `fallbacks?`, `onCompiled?`, `onError?`, `particleSystem?`): [`Effect`](Effect.md)

Create an effect to use with particle systems.
Please note that some parameters like animation sheets or not being billboard are not supported in this configuration, except if you pass
the particle system for which you want to create a custom effect in the last parameter

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fragmentName` | `string` | defines the base name of the effect (The name of file without .fragment.fx) |
| `uniformsNames` | `string`[] | defines a list of attribute names |
| `samplers` | `string`[] | defines an array of string used to represent textures |
| `defines` | `string` | defines the string containing the defines to use to compile the shaders |
| `fallbacks?` | [`EffectFallbacks`](EffectFallbacks.md) | defines the list of potential fallbacks to use if shader compilation fails |
| `onCompiled?` | (`effect`: [`Effect`](Effect.md)) => `void` | defines a function to call when the effect creation is successful |
| `onError?` | (`effect`: [`Effect`](Effect.md), `errors`: `string`) => `void` | defines a function to call when the effect creation has failed |
| `particleSystem?` | [`IParticleSystem`](../interfaces/IParticleSystem.md) | the particle system you want to create the effect for |

#### Returns

[`Effect`](Effect.md)

the new Effect

#### Inherited from

[Engine](Engine.md).[createEffectForParticles](Engine.md#createeffectforparticles)

#### Defined in

packages/dev/core/src/Particles/particleSystemComponent.ts:58

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

#### Inherited from

[Engine](Engine.md).[createExternalTexture](Engine.md#createexternaltexture)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.externalTexture.ts:12

___

### createImageBitmap

▸ **createImageBitmap**(`image`, `options?`): `Promise``ImageBitmap`

Engine abstraction for createImageBitmap

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `image` | `ImageBitmapSource` | source for image |
| `options?` | `ImageBitmapOptions` | An object that sets options for the image's extraction. |

#### Returns

`Promise``ImageBitmap`

ImageBitmap

#### Inherited from

[Engine](Engine.md).[createImageBitmap](Engine.md#createimagebitmap)

#### Defined in

packages/dev/core/src/Engines/engine.ts:328

___

### createIndexBuffer

▸ **createIndexBuffer**(`indices`): [`DataBuffer`](DataBuffer.md)

Creates a new index buffer

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `indices` | [`IndicesArray`](../modules.md#indicesarray) | defines the content of the index buffer |

#### Returns

[`DataBuffer`](DataBuffer.md)

a new webGL buffer

#### Overrides

[Engine](Engine.md).[createIndexBuffer](Engine.md#createindexbuffer)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:215

___

### createInstancesBuffer

▸ **createInstancesBuffer**(`capacity`): [`DataBuffer`](DataBuffer.md)

Creates a webGL buffer to use with instantiation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `capacity` | `number` | defines the size of the buffer |

#### Returns

[`DataBuffer`](DataBuffer.md)

the webGL buffer

#### Inherited from

[Engine](Engine.md).[createInstancesBuffer](Engine.md#createinstancesbuffer)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1804

___

### createMaterialContext

▸ **createMaterialContext**(): `undefined` \| `IMaterialContext`

Creates a new material context

#### Returns

`undefined` \| `IMaterialContext`

the new context

#### Inherited from

[Engine](Engine.md).[createMaterialContext](Engine.md#creatematerialcontext)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:2957

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

#### Inherited from

[Engine](Engine.md).[createMultipleRenderTarget](Engine.md#createmultiplerendertarget)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.multiRender.ts:31

___

### createMultiviewRenderTargetTexture

▸ **createMultiviewRenderTargetTexture**(`width`, `height`): [`RenderTargetWrapper`](RenderTargetWrapper.md)

Creates a new multiview render target

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `width` | `number` | defines the width of the texture |
| `height` | `number` | defines the height of the texture |

#### Returns

[`RenderTargetWrapper`](RenderTargetWrapper.md)

the created multiview render target wrapper

#### Inherited from

[Engine](Engine.md).[createMultiviewRenderTargetTexture](Engine.md#createmultiviewrendertargettexture)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.multiview.ts:22

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

#### Inherited from

[Engine](Engine.md).[createPipelineContext](Engine.md#createpipelinecontext)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:2942

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

#### Inherited from

[Engine](Engine.md).[createPrefilteredCubeTexture](Engine.md#createprefilteredcubetexture)

#### Defined in

packages/dev/core/src/Misc/dds.ts:733

___

### createQuery

▸ **createQuery**(): `OcclusionQuery`

Create a new webGL query (you must be sure that queries are supported by checking getCaps() function)

#### Returns

`OcclusionQuery`

the new query

#### Inherited from

[Engine](Engine.md).[createQuery](Engine.md#createquery)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.query.ts:42

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

#### Inherited from

[Engine](Engine.md).[createRawCubeTexture](Engine.md#createrawcubetexture)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:4291

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

#### Inherited from

[Engine](Engine.md).[createRawCubeTexture](Engine.md#createrawcubetexture)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.rawTexture.ts:82

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

#### Inherited from

[Engine](Engine.md).[createRawCubeTextureFromUrl](Engine.md#createrawcubetexturefromurl)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.rawTexture.ts:140

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

#### Inherited from

[Engine](Engine.md).[createRawCubeTextureFromUrl](Engine.md#createrawcubetexturefromurl)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.rawTexture.ts:169

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

#### Inherited from

[Engine](Engine.md).[createRawShaderProgram](Engine.md#createrawshaderprogram)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:2885

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

#### Overrides

[Engine](Engine.md).[createRawTexture](Engine.md#createrawtexture)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:782

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

#### Inherited from

[Engine](Engine.md).[createRawTexture2DArray](Engine.md#createrawtexture2darray)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:4347

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

#### Inherited from

[Engine](Engine.md).[createRawTexture2DArray](Engine.md#createrawtexture2darray)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.rawTexture.ts:248

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

#### Inherited from

[Engine](Engine.md).[createRawTexture3D](Engine.md#createrawtexture3d)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:4318

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

#### Inherited from

[Engine](Engine.md).[createRawTexture3D](Engine.md#createrawtexture3d)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.rawTexture.ts:199

___

### createRenderPassId

▸ **createRenderPassId**(`name?`): `number`

Creates a render pass id

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name?` | `string` | Name of the render pass (for debug purpose only) |

#### Returns

`number`

the id of the new render pass

#### Inherited from

[Engine](Engine.md).[createRenderPassId](Engine.md#createrenderpassid)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1604

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

#### Inherited from

[Engine](Engine.md).[createRenderTargetCubeTexture](Engine.md#createrendertargetcubetexture)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.renderTargetCube.ts:17

___

### createRenderTargetTexture

▸ **createRenderTargetTexture**(`size`, `options`): [`RenderTargetWrapper`](RenderTargetWrapper.md)

Creates a new render target wrapper

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `size` | `any` | defines the size of the texture |
| `options` | `boolean` \| `RenderTargetCreationOptions` | defines the options used to create the texture |

#### Returns

[`RenderTargetWrapper`](RenderTargetWrapper.md)

a new render target wrapper

#### Overrides

[Engine](Engine.md).[createRenderTargetTexture](Engine.md#createrendertargettexture)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:717

___

### createShaderProgram

▸ **createShaderProgram**(`pipelineContext`, `vertexCode`, `fragmentCode`, `defines`, `context?`): `WebGLProgram`

Creates a webGL program

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `pipelineContext` | [`IPipelineContext`](../interfaces/IPipelineContext.md) | defines the pipeline context to attach to |
| `vertexCode` | `string` | defines the vertex shader code to use |
| `fragmentCode` | `string` | defines the fragment shader code to use |
| `defines` | `string` | defines the string containing the defines to use to compile the shaders |
| `context?` | `WebGLRenderingContext` | defines the webGL context to use (if not set, the current one will be used) |

#### Returns

`WebGLProgram`

the new webGL program

#### Overrides

[Engine](Engine.md).[createShaderProgram](Engine.md#createshaderprogram)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:266

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

#### Inherited from

[Engine](Engine.md).[createStorageBuffer](Engine.md#createstoragebuffer)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.storageBuffer.ts:15

___

### createTexture

▸ **createTexture**(`urlArg`, `noMipmap`, `invertY`, `scene`, `samplingMode?`, `onLoad?`, `onError?`, `buffer?`, `fallback?`, `format?`, `forcedExtension?`, `mimeType?`): [`InternalTexture`](InternalTexture.md)

Usually called from Texture.ts.
Passed information to create a WebGLTexture

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `urlArg` | [`Nullable`](../modules.md#nullable)`string` | `undefined` | defines a value which contains one of the following:  * A conventional http URL, e.g. 'http://...' or 'file://...'  * A base64 string of in-line texture data, e.g. 'data:image/jpg;base64,/...'  * An indicator that data being passed using the buffer parameter, e.g. 'data:mytexture.jpg' |
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

#### Returns

[`InternalTexture`](InternalTexture.md)

a InternalTexture for assignment back into BABYLON.Texture

#### Overrides

[Engine](Engine.md).[createTexture](Engine.md#createtexture)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:657

___

### createTransformFeedback

▸ **createTransformFeedback**(): `WebGLTransformFeedback`

Creates a webGL transform feedback object
Please makes sure to check webGLVersion property to check if you are running webGL 2+

#### Returns

`WebGLTransformFeedback`

the webGL transform feedback object

#### Inherited from

[Engine](Engine.md).[createTransformFeedback](Engine.md#createtransformfeedback)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.transformFeedback.ts:16

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

#### Inherited from

[Engine](Engine.md).[createUniformBuffer](Engine.md#createuniformbuffer)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.uniformBuffer.ts:16

___

### createVertexBuffer

▸ **createVertexBuffer**(`vertices`): [`DataBuffer`](DataBuffer.md)

Creates a vertex buffer

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vertices` | [`FloatArray`](../modules.md#floatarray) | the data for the vertex buffer |

#### Returns

[`DataBuffer`](DataBuffer.md)

the new WebGL static buffer

#### Overrides

[Engine](Engine.md).[createVertexBuffer](Engine.md#createvertexbuffer)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:204

___

### createVideoElement

▸ **createVideoElement**(`constraints`): `any`

creates and returns a new video element

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `constraints` | `MediaTrackConstraints` | video constraints |

#### Returns

`any`

video element

#### Inherited from

[Engine](Engine.md).[createVideoElement](Engine.md#createvideoelement)

#### Defined in

packages/dev/core/src/Engines/engine.ts:2048

___

### deleteInstancesBuffer

▸ **deleteInstancesBuffer**(`buffer`): `void`

Delete a webGL buffer used with instantiation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `buffer` | `WebGLBuffer` | defines the webGL buffer to delete |

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[deleteInstancesBuffer](Engine.md#deleteinstancesbuffer)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1826

___

### deleteQuery

▸ **deleteQuery**(`query`): [`Engine`](Engine.md)

Delete and release a webGL query

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `query` | `OcclusionQuery` | defines the query to delete |

#### Returns

[`Engine`](Engine.md)

the current engine

#### Inherited from

[Engine](Engine.md).[deleteQuery](Engine.md#deletequery)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.query.ts:49

___

### deleteTransformFeedback

▸ **deleteTransformFeedback**(`value`): `void`

Delete a webGL transform feedback object

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `WebGLTransformFeedback` | defines the webGL transform feedback object to delete |

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[deleteTransformFeedback](Engine.md#deletetransformfeedback)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.transformFeedback.ts:22

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

#### Inherited from

[Engine](Engine.md).[disableAttributeByIndex](Engine.md#disableattributebyindex)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:2586

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

#### Inherited from

[Engine](Engine.md).[disableInstanceAttribute](Engine.md#disableinstanceattribute)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:2565

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

#### Inherited from

[Engine](Engine.md).[disableInstanceAttributeByName](Engine.md#disableinstanceattributebyname)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:2552

___

### disableScissor

▸ **disableScissor**(): `void`

Disable previously set scissor test rectangle

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[disableScissor](Engine.md#disablescissor)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1112

___

### disableVR

▸ **disableVR**(): `void`

Call this function to leave webVR mode
Will do nothing if webVR is not supported or if there is no webVR device

**`See`**

https://doc.babylonjs.com/how_to/webvr_camera

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[disableVR](Engine.md#disablevr)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1159

___

### displayLoadingUI

▸ **displayLoadingUI**(): `void`

Display the loading screen

**`See`**

https://doc.babylonjs.com/how_to/creating_a_custom_loading_screen

#### Returns

`void`

#### Overrides

[Engine](Engine.md).[displayLoadingUI](Engine.md#displayloadingui)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:979

___

### dispose

▸ **dispose**(): `void`

Dispose and release all associated resources

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[dispose](Engine.md#dispose)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1891

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

#### Overrides

[Engine](Engine.md).[draw](Engine.md#draw)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:606

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

#### Overrides

[Engine](Engine.md).[drawArraysType](Engine.md#drawarraystype)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:624

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

#### Overrides

[Engine](Engine.md).[drawElementsType](Engine.md#drawelementstype)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:615

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

#### Inherited from

[Engine](Engine.md).[drawPointClouds](Engine.md#drawpointclouds)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:2609

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

#### Inherited from

[Engine](Engine.md).[drawUnIndexed](Engine.md#drawunindexed)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:2620

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

#### Overrides

[Engine](Engine.md).[enableEffect](Engine.md#enableeffect)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:305

___

### enableScissor

▸ **enableScissor**(`x`, `y`, `width`, `height`): `void`

Enable scissor test on a specific rectangle (ie. render will only be executed on a specific portion of the screen)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | defines the x-coordinate of the bottom left corner of the clear rectangle |
| `y` | `number` | defines the y-coordinate of the corner of the clear rectangle |
| `width` | `number` | defines the width of the clear rectangle |
| `height` | `number` | defines the height of the clear rectangle |

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[enableScissor](Engine.md#enablescissor)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1101

___

### enableVR

▸ **enableVR**(`options`): `void`

Call this function to switch to webVR mode
Will do nothing if webVR is not supported or if there is no webVR device

**`See`**

https://doc.babylonjs.com/how_to/webvr_camera

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | [`WebVROptions`](../interfaces/WebVROptions.md) | the webvr options provided to the camera. mainly used for multiview |

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[enableVR](Engine.md#enablevr)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.webVR.ts:103

___

### endFrame

▸ **endFrame**(): `void`

End the current frame

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[endFrame](Engine.md#endframe)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1415

___

### endOcclusionQuery

▸ **endOcclusionQuery**(`algorithmType`): [`Engine`](Engine.md)

Ends an occlusion query

**`See`**

https://doc.babylonjs.com/features/occlusionquery

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `algorithmType` | `number` | defines the algorithm to use |

#### Returns

[`Engine`](Engine.md)

the current engine

#### Inherited from

[Engine](Engine.md).[endOcclusionQuery](Engine.md#endocclusionquery)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.query.ts:80

___

### endTimeQuery

▸ **endTimeQuery**(`token`): `number`

Ends a time query

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `token` | `_TimeToken` | defines the token used to measure the time span |

#### Returns

`number`

the time spent (in ns)

#### Inherited from

[Engine](Engine.md).[endTimeQuery](Engine.md#endtimequery)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.query.ts:94

___

### endTransformFeedback

▸ **endTransformFeedback**(): `void`

Ends a transform feedback operation

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[endTransformFeedback](Engine.md#endtransformfeedback)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.transformFeedback.ts:39

___

### enterFullscreen

▸ **enterFullscreen**(`requestPointerLock`): `void`

Enters full screen mode

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `requestPointerLock` | `boolean` | defines if a pointer lock should be requested from the user |

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[enterFullscreen](Engine.md#enterfullscreen)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1368

___

### enterPointerlock

▸ **enterPointerlock**(): `void`

Enters Pointerlock mode

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[enterPointerlock](Engine.md#enterpointerlock)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1389

___

### exitFullscreen

▸ **exitFullscreen**(): `void`

Exits full screen mode

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[exitFullscreen](Engine.md#exitfullscreen)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1380

___

### exitPointerlock

▸ **exitPointerlock**(): `void`

Exits Pointerlock mode

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[exitPointerlock](Engine.md#exitpointerlock)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1398

___

### flushFramebuffer

▸ **flushFramebuffer**(): `void`

Force a webGL flush (ie. a flush of all waiting webGL commands)

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[flushFramebuffer](Engine.md#flushframebuffer)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:2024

___

### generateMipMapsForCubemap

▸ **generateMipMapsForCubemap**(`texture`, `unbind?`): `void`

Force the mipmap generation for the given render target texture

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `texture` | [`InternalTexture`](InternalTexture.md) | `undefined` | defines the render target texture to use |
| `unbind` | `boolean` | `true` | defines whether or not to unbind the texture after generation. Defaults to true. |

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[generateMipMapsForCubemap](Engine.md#generatemipmapsforcubemap)

#### Defined in

packages/dev/core/src/Engines/engine.ts:804

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

#### Inherited from

[Engine](Engine.md).[generateMipmaps](Engine.md#generatemipmaps)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1976

___

### getAlphaEquation

▸ **getAlphaEquation**(): `number`

Gets the current alpha equation.

#### Returns

`number`

the current alpha equation

#### Inherited from

[Engine](Engine.md).[getAlphaEquation](Engine.md#getalphaequation)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.alpha.ts:40

___

### getAlphaMode

▸ **getAlphaMode**(): `number`

Gets the current alpha mode

**`See`**

https://doc.babylonjs.com/resources/transparency_and_how_meshes_are_rendered

#### Returns

`number`

the current alpha mode

#### Inherited from

[Engine](Engine.md).[getAlphaMode](Engine.md#getalphamode)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.alpha.ts:28

___

### getAspectRatio

▸ **getAspectRatio**(`viewportOwner`, `useScreen?`): `number`

Gets current aspect ratio

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `viewportOwner` | `IViewportOwnerLike` | `undefined` | defines the camera to use to get the aspect ratio |
| `useScreen` | `boolean` | `false` | defines if screen size must be used (or the current render target if any) |

#### Returns

`number`

a number defining the aspect ratio

#### Inherited from

[Engine](Engine.md).[getAspectRatio](Engine.md#getaspectratio)

#### Defined in

packages/dev/core/src/Engines/engine.ts:738

___

### getAttributes

▸ **getAttributes**(`pipelineContext`, `attributesNames`): `number`[]

Gets the lsit of active attributes for a given webGL program

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `pipelineContext` | [`IPipelineContext`](../interfaces/IPipelineContext.md) | defines the pipeline context to use |
| `attributesNames` | `string`[] | defines the list of attribute names to get |

#### Returns

`number`[]

an array of indices indicating the offset of each attribute

#### Overrides

[Engine](Engine.md).[getAttributes](Engine.md#getattributes)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:289

___

### getAudioContext

▸ **getAudioContext**(): [`Nullable`](../modules.md#nullable)`AudioContext`

Gets the audio context specified in engine initialization options

#### Returns

[`Nullable`](../modules.md#nullable)`AudioContext`

an Audio Context

#### Inherited from

[Engine](Engine.md).[getAudioContext](Engine.md#getaudiocontext)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1573

___

### getAudioDestination

▸ **getAudioDestination**(): [`Nullable`](../modules.md#nullable)`AudioDestinationNode` \| `MediaStreamAudioDestinationNode`

Gets the audio destination specified in engine initialization options

#### Returns

[`Nullable`](../modules.md#nullable)`AudioDestinationNode` \| `MediaStreamAudioDestinationNode`

an audio destination node

#### Inherited from

[Engine](Engine.md).[getAudioDestination](Engine.md#getaudiodestination)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1581

___

### getCaps

▸ **getCaps**(): [`EngineCapabilities`](../interfaces/EngineCapabilities.md)

Gets the object containing all engine capabilities

#### Returns

[`EngineCapabilities`](../interfaces/EngineCapabilities.md)

the EngineCapabilities object

#### Inherited from

[Engine](Engine.md).[getCaps](Engine.md#getcaps)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1510

___

### getClassName

▸ **getClassName**(): `string`

Gets a string identifying the name of the class

#### Returns

`string`

"Engine" string

#### Inherited from

[Engine](Engine.md).[getClassName](Engine.md#getclassname)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1418

___

### getColorWrite

▸ **getColorWrite**(): `boolean`

Gets a boolean indicating if color writing is enabled

#### Returns

`boolean`

the current color writing state

#### Inherited from

[Engine](Engine.md).[getColorWrite](Engine.md#getcolorwrite)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:3539

___

### getCreationOptions

▸ **getCreationOptions**(): [`EngineOptions`](../interfaces/EngineOptions.md)

Gets the options used for engine creation

#### Returns

[`EngineOptions`](../interfaces/EngineOptions.md)

EngineOptions object

#### Inherited from

[Engine](Engine.md).[getCreationOptions](Engine.md#getcreationoptions)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:384

___

### getCurrentRenderPassName

▸ **getCurrentRenderPassName**(): `string`

Gets the name of the current render pass

#### Returns

`string`

name of the current render pass

#### Inherited from

[Engine](Engine.md).[getCurrentRenderPassName](Engine.md#getcurrentrenderpassname)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1595

___

### getDeltaTime

▸ **getDeltaTime**(): `number`

Gets the time spent between current and previous frame

#### Returns

`number`

a number representing the delta time in ms

#### Inherited from

[Engine](Engine.md).[getDeltaTime](Engine.md#getdeltatime)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1704

___

### getDepthBuffer

▸ **getDepthBuffer**(): `boolean`

Gets a boolean indicating if depth testing is enabled

#### Returns

`boolean`

the current state

#### Inherited from

[Engine](Engine.md).[getDepthBuffer](Engine.md#getdepthbuffer)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1910

___

### getDepthFunction

▸ **getDepthFunction**(): [`Nullable`](../modules.md#nullable)`number`

Gets the current depth function

#### Returns

[`Nullable`](../modules.md#nullable)`number`

a number defining the depth function

#### Inherited from

[Engine](Engine.md).[getDepthFunction](Engine.md#getdepthfunction)

#### Defined in

packages/dev/core/src/Engines/engine.ts:989

___

### getDepthWrite

▸ **getDepthWrite**(): `boolean`

Gets a boolean indicating if depth writing is enabled

#### Returns

`boolean`

the current depth writing state

#### Inherited from

[Engine](Engine.md).[getDepthWrite](Engine.md#getdepthwrite)

#### Defined in

packages/dev/core/src/Engines/engine.ts:821

___

### getFontOffset

▸ **getFontOffset**(`font`): `Object`

Get Font size information

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `font` | `string` | font name |

#### Returns

`Object`

an object containing ascent, height and descent

| Name | Type |
| :------ | :------ |
| `ascent` | `number` |
| `descent` | `number` |
| `height` | `number` |

#### Inherited from

[Engine](Engine.md).[getFontOffset](Engine.md#getfontoffset)

#### Defined in

packages/dev/core/src/Engines/engine.ts:2113

___

### getFps

▸ **getFps**(): `number`

Gets the current framerate

#### Returns

`number`

a number representing the framerate

#### Inherited from

[Engine](Engine.md).[getFps](Engine.md#getfps)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1696

___

### getFragmentShaderSource

▸ **getFragmentShaderSource**(`program`): [`Nullable`](../modules.md#nullable)`string`

Gets the source code of the fragment shader associated with a specific webGL program

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `program` | `WebGLProgram` | defines the program to use |

#### Returns

[`Nullable`](../modules.md#nullable)`string`

a string containing the source code of the fragment shader associated with the program

#### Inherited from

[Engine](Engine.md).[getFragmentShaderSource](Engine.md#getfragmentshadersource)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1219

___

### getGPUFrameTimeCounter

▸ **getGPUFrameTimeCounter**(): [`PerfCounter`](PerfCounter.md)

Get the performance counter associated with the frame time computation

#### Returns

[`PerfCounter`](PerfCounter.md)

the perf counter

#### Inherited from

[Engine](Engine.md).[getGPUFrameTimeCounter](Engine.md#getgpuframetimecounter)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.query.ts:100

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

#### Inherited from

[Engine](Engine.md).[getGlInfo](Engine.md#getglinfo)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1469

___

### getHardwareScalingLevel

▸ **getHardwareScalingLevel**(): `number`

Gets the current hardware scaling level.
By default the hardware scaling level is computed from the window device ratio.
if level = 1 then the engine will render at the exact resolution of the canvas. If level = 0.5 then the engine will render at twice the size of the canvas.

#### Returns

`number`

a number indicating the current hardware scaling level

#### Overrides

[Engine](Engine.md).[getHardwareScalingLevel](Engine.md#gethardwarescalinglevel)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:88

___

### getHostDocument

▸ **getHostDocument**(): [`Nullable`](../modules.md#nullable)`Document`

Gets host document

#### Returns

[`Nullable`](../modules.md#nullable)`Document`

the host document object

#### Inherited from

[Engine](Engine.md).[getHostDocument](Engine.md#gethostdocument)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:5957

___

### getHostWindow

▸ **getHostWindow**(): [`Nullable`](../modules.md#nullable)`Window`

Gets host window

#### Returns

[`Nullable`](../modules.md#nullable)`Window`

the host window object

#### Inherited from

[Engine](Engine.md).[getHostWindow](Engine.md#gethostwindow)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1589

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

#### Inherited from

[Engine](Engine.md).[getInfo](Engine.md#getinfo)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1461

___

### getInputElement

▸ **getInputElement**(): [`Nullable`](../modules.md#nullable)`HTMLElement`

Gets the HTML element used to attach event listeners

#### Returns

[`Nullable`](../modules.md#nullable)`HTMLElement`

a HTML element

#### Inherited from

[Engine](Engine.md).[getInputElement](Engine.md#getinputelement)

#### Defined in

packages/dev/core/src/Engines/engine.ts:567

___

### getInputElementClientRect

▸ **getInputElementClientRect**(): [`Nullable`](../modules.md#nullable)`ClientRect`

Gets the client rect of the HTML element used for events

#### Returns

[`Nullable`](../modules.md#nullable)`ClientRect`

a client rectangle

#### Inherited from

[Engine](Engine.md).[getInputElementClientRect](Engine.md#getinputelementclientrect)

#### Defined in

packages/dev/core/src/Engines/engine.ts:766

___

### getLoadedTexturesCache

▸ **getLoadedTexturesCache**(): [`InternalTexture`](InternalTexture.md)[]

Gets the list of loaded textures

#### Returns

[`InternalTexture`](InternalTexture.md)[]

an array containing all loaded textures

#### Inherited from

[Engine](Engine.md).[getLoadedTexturesCache](Engine.md#getloadedtexturescache)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1502

___

### getLockstepMaxSteps

▸ **getLockstepMaxSteps**(): `number`

Gets the max steps when engine is running in deterministic lock step

**`See`**

https://doc.babylonjs.com/babylon101/animations#deterministic-lockstep

#### Returns

`number`

the max steps

#### Overrides

[Engine](Engine.md).[getLockstepMaxSteps](Engine.md#getlockstepmaxsteps)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:78

___

### getQueryResult

▸ **getQueryResult**(`query`): `number`

Gets the value of a given query

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `query` | `OcclusionQuery` | defines the query to check |

#### Returns

`number`

the value of the query

#### Inherited from

[Engine](Engine.md).[getQueryResult](Engine.md#getqueryresult)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.query.ts:63

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

#### Overrides

[Engine](Engine.md).[getRenderHeight](Engine.md#getrenderheight)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:248

___

### getRenderPassNames

▸ **getRenderPassNames**(): `string`[]

Gets the names of the render passes that are currently created

#### Returns

`string`[]

list of the render pass names

#### Inherited from

[Engine](Engine.md).[getRenderPassNames](Engine.md#getrenderpassnames)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1587

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

#### Overrides

[Engine](Engine.md).[getRenderWidth](Engine.md#getrenderwidth)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:235

___

### getRenderingCanvas

▸ **getRenderingCanvas**(): [`Nullable`](../modules.md#nullable)`HTMLCanvasElement`

Gets the HTML canvas attached with the current webGL context

#### Returns

[`Nullable`](../modules.md#nullable)`HTMLCanvasElement`

a HTML canvas

#### Inherited from

[Engine](Engine.md).[getRenderingCanvas](Engine.md#getrenderingcanvas)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1565

___

### getRenderingCanvasClientRect

▸ **getRenderingCanvasClientRect**(): [`Nullable`](../modules.md#nullable)`ClientRect`

Gets the client rect of the HTML canvas attached with the current webGL context

#### Returns

[`Nullable`](../modules.md#nullable)`ClientRect`

a client rectangle

#### Inherited from

[Engine](Engine.md).[getRenderingCanvasClientRect](Engine.md#getrenderingcanvasclientrect)

#### Defined in

packages/dev/core/src/Engines/engine.ts:755

___

### getScreenAspectRatio

▸ **getScreenAspectRatio**(): `number`

Gets current screen aspect ratio

#### Returns

`number`

a number defining the aspect ratio

#### Inherited from

[Engine](Engine.md).[getScreenAspectRatio](Engine.md#getscreenaspectratio)

#### Defined in

packages/dev/core/src/Engines/engine.ts:747

___

### getStencilBuffer

▸ **getStencilBuffer**(): `boolean`

Gets a boolean indicating if stencil buffer is enabled

#### Returns

`boolean`

the current stencil buffer state

#### Inherited from

[Engine](Engine.md).[getStencilBuffer](Engine.md#getstencilbuffer)

#### Defined in

packages/dev/core/src/Engines/engine.ts:837

___

### getStencilFunction

▸ **getStencilFunction**(): `number`

Gets the current stencil function

#### Returns

`number`

a number defining the stencil function to use

#### Inherited from

[Engine](Engine.md).[getStencilFunction](Engine.md#getstencilfunction)

#### Defined in

packages/dev/core/src/Engines/engine.ts:869

___

### getStencilFunctionMask

▸ **getStencilFunctionMask**(): `number`

Gets the current stencil mask

#### Returns

`number`

a number defining the stencil mask to use

#### Inherited from

[Engine](Engine.md).[getStencilFunctionMask](Engine.md#getstencilfunctionmask)

#### Defined in

packages/dev/core/src/Engines/engine.ts:885

___

### getStencilFunctionReference

▸ **getStencilFunctionReference**(): `number`

Gets the current stencil reference value

#### Returns

`number`

a number defining the stencil reference value to use

#### Inherited from

[Engine](Engine.md).[getStencilFunctionReference](Engine.md#getstencilfunctionreference)

#### Defined in

packages/dev/core/src/Engines/engine.ts:877

___

### getStencilMask

▸ **getStencilMask**(): `number`

Gets the current stencil mask

#### Returns

`number`

a number defining the new stencil mask to use

#### Inherited from

[Engine](Engine.md).[getStencilMask](Engine.md#getstencilmask)

#### Defined in

packages/dev/core/src/Engines/engine.ts:853

___

### getStencilOperationDepthFail

▸ **getStencilOperationDepthFail**(): `number`

Gets the current stencil operation when depth fails

#### Returns

`number`

a number defining stencil operation to use when depth fails

#### Inherited from

[Engine](Engine.md).[getStencilOperationDepthFail](Engine.md#getstenciloperationdepthfail)

#### Defined in

packages/dev/core/src/Engines/engine.ts:925

___

### getStencilOperationFail

▸ **getStencilOperationFail**(): `number`

Gets the current stencil operation when stencil fails

#### Returns

`number`

a number defining stencil operation to use when stencil fails

#### Inherited from

[Engine](Engine.md).[getStencilOperationFail](Engine.md#getstenciloperationfail)

#### Defined in

packages/dev/core/src/Engines/engine.ts:917

___

### getStencilOperationPass

▸ **getStencilOperationPass**(): `number`

Gets the current stencil operation when stencil passes

#### Returns

`number`

a number defining stencil operation to use when stencil passes

#### Inherited from

[Engine](Engine.md).[getStencilOperationPass](Engine.md#getstenciloperationpass)

#### Defined in

packages/dev/core/src/Engines/engine.ts:933

___

### getTimeStep

▸ **getTimeStep**(): `number`

Returns the time in ms between steps when using deterministic lock step.

#### Returns

`number`

time step in (ms)

#### Inherited from

[Engine](Engine.md).[getTimeStep](Engine.md#gettimestep)

#### Defined in

packages/dev/core/src/Engines/engine.ts:795

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

#### Overrides

[Engine](Engine.md).[getUniforms](Engine.md#getuniforms)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:279

___

### getVRDevice

▸ **getVRDevice**(): `any`

Gets the current webVR device

#### Returns

`any`

the current webVR device (or null)

#### Inherited from

[Engine](Engine.md).[getVRDevice](Engine.md#getvrdevice)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.webVR.ts:80

___

### getVertexShaderSource

▸ **getVertexShaderSource**(`program`): [`Nullable`](../modules.md#nullable)`string`

Gets the source code of the vertex shader associated with a specific webGL program

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `program` | `WebGLProgram` | defines the program to use |

#### Returns

[`Nullable`](../modules.md#nullable)`string`

a string containing the source code of the vertex shader associated with the program

#### Inherited from

[Engine](Engine.md).[getVertexShaderSource](Engine.md#getvertexshadersource)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1204

___

### getZOffset

▸ **getZOffset**(): `number`

Gets the current value of the zOffset Factor

#### Returns

`number`

the current zOffset Factor state

#### Inherited from

[Engine](Engine.md).[getZOffset](Engine.md#getzoffset)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1934

___

### getZOffsetUnits

▸ **getZOffsetUnits**(): `number`

Gets the current value of the zOffset Units

#### Returns

`number`

the current zOffset Units state

#### Inherited from

[Engine](Engine.md).[getZOffsetUnits](Engine.md#getzoffsetunits)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1951

___

### hideLoadingUI

▸ **hideLoadingUI**(): `void`

Hide the loading screen

**`See`**

https://doc.babylonjs.com/how_to/creating_a_custom_loading_screen

#### Returns

`void`

#### Overrides

[Engine](Engine.md).[hideLoadingUI](Engine.md#hideloadingui)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:981

___

### initWebVR

▸ **initWebVR**(): [`Observable`](Observable.md)[`IDisplayChangedEventArgs`](../interfaces/IDisplayChangedEventArgs.md)

Initializes a webVR display and starts listening to display change events
The onVRDisplayChangedObservable will be notified upon these changes

#### Returns

[`Observable`](Observable.md)[`IDisplayChangedEventArgs`](../interfaces/IDisplayChangedEventArgs.md)

The onVRDisplayChangedObservable

#### Inherited from

[Engine](Engine.md).[initWebVR](Engine.md#initwebvr)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1131

___

### initWebVRAsync

▸ **initWebVRAsync**(): `Promise`[`IDisplayChangedEventArgs`](../interfaces/IDisplayChangedEventArgs.md)

Initializes a webVR display and starts listening to display change events
The onVRDisplayChangedObservable will be notified upon these changes

#### Returns

`Promise`[`IDisplayChangedEventArgs`](../interfaces/IDisplayChangedEventArgs.md)

A promise containing a VRDisplay and if vr is supported

#### Inherited from

[Engine](Engine.md).[initWebVRAsync](Engine.md#initwebvrasync)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.webVR.ts:87

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

#### Inherited from

[Engine](Engine.md).[inlineShaderCode](Engine.md#inlineshadercode)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:2932

___

### isDeterministicLockStep

▸ **isDeterministicLockStep**(): `boolean`

Gets a boolean indicating that the engine is running in deterministic lock step mode

**`See`**

https://doc.babylonjs.com/babylon101/animations#deterministic-lockstep

#### Returns

`boolean`

true if engine is in deterministic lock step mode

#### Overrides

[Engine](Engine.md).[isDeterministicLockStep](Engine.md#isdeterministiclockstep)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:69

___

### isQueryResultAvailable

▸ **isQueryResultAvailable**(`query`): `boolean`

Check if a given query has resolved and got its value

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `query` | `OcclusionQuery` | defines the query to check |

#### Returns

`boolean`

true if the query got its value

#### Inherited from

[Engine](Engine.md).[isQueryResultAvailable](Engine.md#isqueryresultavailable)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.query.ts:56

___

### isVRDevicePresent

▸ **isVRDevicePresent**(): `boolean`

Gets a boolean indicating if a webVR device was detected

#### Returns

`boolean`

true if a webVR device was detected

#### Inherited from

[Engine](Engine.md).[isVRDevicePresent](Engine.md#isvrdevicepresent)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.webVR.ts:74

___

### isVRPresenting

▸ **isVRPresenting**(): `boolean`

Gets a boolean indicating that the system is in VR mode and is presenting

#### Returns

`boolean`

true if VR mode is engaged

#### Inherited from

[Engine](Engine.md).[isVRPresenting](Engine.md#isvrpresenting)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1167

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

#### Inherited from

[Engine](Engine.md).[readFromStorageBuffer](Engine.md#readfromstoragebuffer)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.storageBuffer.ts:34

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

#### Inherited from

[Engine](Engine.md).[readPixels](Engine.md#readpixels)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:5775

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

#### Inherited from

[Engine](Engine.md).[recordVertexArrayObject](Engine.md#recordvertexarrayobject)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:2322

___

### registerView

▸ **registerView**(`canvas`, `camera?`, `clearBeforeCopy?`): [`EngineView`](EngineView.md)

Register a new child canvas

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `canvas` | `HTMLCanvasElement` | defines the canvas to register |
| `camera?` | [`Camera`](Camera.md) | defines an optional camera to use with this canvas (it will overwrite the scene.camera for this view) |
| `clearBeforeCopy?` | `boolean` | Indicates if the destination view canvas should be cleared before copying the parent canvas. Can help if the scene clear color has alpha  1 |

#### Returns

[`EngineView`](EngineView.md)

the associated view

#### Inherited from

[Engine](Engine.md).[registerView](Engine.md#registerview)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.views.ts:55

___

### releaseComputeEffects

▸ **releaseComputeEffects**(): `void`

Forces the engine to release all cached compute effects. This means that next effect compilation will have to be done completely even if a similar effect was already compiled

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[releaseComputeEffects](Engine.md#releasecomputeeffects)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.computeShader.ts:84

___

### releaseEffects

▸ **releaseEffects**(): `void`

Force the engine to release all cached effects. This means that next effect compilation will have to be done completely even if a similar effect was already compiled

#### Returns

`void`

#### Overrides

[Engine](Engine.md).[releaseEffects](Engine.md#releaseeffects)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:977

___

### releaseRenderPassId

▸ **releaseRenderPassId**(`id`): `void`

Releases a render pass id

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `number` | id of the render pass to release |

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[releaseRenderPassId](Engine.md#releaserenderpassid)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1615

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

#### Inherited from

[Engine](Engine.md).[releaseVertexArrayObject](Engine.md#releasevertexarrayobject)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:2455

___

### resetTextureCache

▸ **resetTextureCache**(): `void`

Reset the texture cache to empty state

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[resetTextureCache](Engine.md#resettexturecache)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1446

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

#### Inherited from

[Engine](Engine.md).[resize](Engine.md#resize)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1426

___

### resizeImageBitmap

▸ **resizeImageBitmap**(`image`, `bufferWidth`, `bufferHeight`): `Uint8Array`

Resize an image and returns the image data as an uint8array

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `image` | `HTMLImageElement` \| `ImageBitmap` | image to resize |
| `bufferWidth` | `number` | destination buffer width |
| `bufferHeight` | `number` | destination buffer height |

#### Returns

`Uint8Array`

an uint8array containing RGBA values of bufferWidth * bufferHeight size

#### Inherited from

[Engine](Engine.md).[resizeImageBitmap](Engine.md#resizeimagebitmap)

#### Defined in

packages/dev/core/src/Engines/engine.ts:339

___

### restoreDefaultFramebuffer

▸ **restoreDefaultFramebuffer**(): `void`

Unbind the current render target and bind the default framebuffer

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[restoreDefaultFramebuffer](Engine.md#restoredefaultframebuffer)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:2031

___

### restoreSingleAttachment

▸ **restoreSingleAttachment**(): `void`

Restores the webgl state to only draw on the main color attachment
when the frame buffer associated is the canvas frame buffer

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[restoreSingleAttachment](Engine.md#restoresingleattachment)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.multiRender.ts:60

___

### restoreSingleAttachmentForRenderTarget

▸ **restoreSingleAttachmentForRenderTarget**(): `void`

Restores the webgl state to only draw on the main color attachment
when the frame buffer associated is not the canvas frame buffer

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[restoreSingleAttachmentForRenderTarget](Engine.md#restoresingleattachmentforrendertarget)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.multiRender.ts:66

___

### restoreStencilState

▸ **restoreStencilState**(): `void`

Restores the state of the stencil buffer

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[restoreStencilState](Engine.md#restorestencilstate)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1053

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

#### Inherited from

[Engine](Engine.md).[runRenderLoop](Engine.md#runrenderloop)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1641

___

### scissorClear

▸ **scissorClear**(`x`, `y`, `width`, `height`, `clearColor`): `void`

Executes a scissor clear (ie. a clear on a specific portion of the screen)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | defines the x-coordinate of the bottom left corner of the clear rectangle |
| `y` | `number` | defines the y-coordinate of the corner of the clear rectangle |
| `width` | `number` | defines the width of the clear rectangle |
| `height` | `number` | defines the height of the clear rectangle |
| `clearColor` | `IColor4Like` | defines the clear color |

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[scissorClear](Engine.md#scissorclear)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1088

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

#### Inherited from

[Engine](Engine.md).[setAlphaConstants](Engine.md#setalphaconstants)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.alpha.ts:13

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

#### Inherited from

[Engine](Engine.md).[setAlphaEquation](Engine.md#setalphaequation)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.alpha.ts:34

___

### setAlphaMode

▸ **setAlphaMode**(`mode`, `noDepthWriteChange?`): `void`

Sets the current alpha mode

**`See`**

https://doc.babylonjs.com/resources/transparency_and_how_meshes_are_rendered

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `mode` | `number` | `undefined` | defines the mode to use (one of the Engine.ALPHA_XXX) |
| `noDepthWriteChange` | `boolean` | `false` | defines if depth writing state should remains unchanged (false by default) |

#### Returns

`void`

#### Overrides

[Engine](Engine.md).[setAlphaMode](Engine.md#setalphamode)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:553

___

### setArray

▸ **setArray**(`uniform`, `array`): `boolean`

Set the value of an uniform to an array of number

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniform` | `WebGLUniformLocation` | defines the webGL uniform location where to store the value |
| `array` | `number`[] | defines the array of number to store |

#### Returns

`boolean`

true if value was set

#### Overrides

[Engine](Engine.md).[setArray](Engine.md#setarray)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:427

___

### setArray2

▸ **setArray2**(`uniform`, `array`): `boolean`

Set the value of an uniform to an array of number (stored as vec2)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniform` | `WebGLUniformLocation` | defines the webGL uniform location where to store the value |
| `array` | `number`[] | defines the array of number to store |

#### Returns

`boolean`

true if value was set

#### Overrides

[Engine](Engine.md).[setArray2](Engine.md#setarray2)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:437

___

### setArray3

▸ **setArray3**(`uniform`, `array`): `boolean`

Set the value of an uniform to an array of number (stored as vec3)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniform` | `WebGLUniformLocation` | defines the webGL uniform location where to store the value |
| `array` | `number`[] | defines the array of number to store |

#### Returns

`boolean`

true if value was set

#### Overrides

[Engine](Engine.md).[setArray3](Engine.md#setarray3)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:447

___

### setArray4

▸ **setArray4**(`uniform`, `array`): `boolean`

Set the value of an uniform to an array of number (stored as vec4)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniform` | `WebGLUniformLocation` | defines the webGL uniform location where to store the value |
| `array` | `number`[] | defines the array of number to store |

#### Returns

`boolean`

true if value was set

#### Overrides

[Engine](Engine.md).[setArray4](Engine.md#setarray4)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:457

___

### setBool

▸ **setBool**(`uniform`, `bool`): `boolean`

Set the value of an uniform to a boolean

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniform` | `WebGLUniformLocation` | defines the webGL uniform location where to store the value |
| `bool` | `number` | defines the boolean to store |

#### Returns

`boolean`

true if value was set

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:530

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

#### Inherited from

[Engine](Engine.md).[setColorWrite](Engine.md#setcolorwrite)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:3528

___

### setCompressedTextureExclusions

▸ **setCompressedTextureExclusions**(`skippedFiles`): `void`

Set the compressed texture extensions or file names to skip.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `skippedFiles` | `string`[] | defines the list of those texture files you want to skip  Example: [".dds", ".env", "myfile.png"] |

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[setCompressedTextureExclusions](Engine.md#setcompressedtextureexclusions)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.textureSelector.ts:28

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

#### Inherited from

[Engine](Engine.md).[setDepthBuffer](Engine.md#setdepthbuffer)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1918

___

### setDepthFunction

▸ **setDepthFunction**(`depthFunc`): `void`

Sets the current depth function

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `depthFunc` | `number` | defines the function to use |

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[setDepthFunction](Engine.md#setdepthfunction)

#### Defined in

packages/dev/core/src/Engines/engine.ts:997

___

### setDepthFunctionToGreater

▸ **setDepthFunctionToGreater**(): `void`

Sets the current depth function to GREATER

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[setDepthFunctionToGreater](Engine.md#setdepthfunctiontogreater)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1004

___

### setDepthFunctionToGreaterOrEqual

▸ **setDepthFunctionToGreaterOrEqual**(): `void`

Sets the current depth function to GEQUAL

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[setDepthFunctionToGreaterOrEqual](Engine.md#setdepthfunctiontogreaterorequal)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1011

___

### setDepthFunctionToLess

▸ **setDepthFunctionToLess**(): `void`

Sets the current depth function to LESS

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[setDepthFunctionToLess](Engine.md#setdepthfunctiontoless)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1018

___

### setDepthFunctionToLessOrEqual

▸ **setDepthFunctionToLessOrEqual**(): `void`

Sets the current depth function to LEQUAL

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[setDepthFunctionToLessOrEqual](Engine.md#setdepthfunctiontolessorequal)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1025

___

### setDepthStencilTexture

▸ **setDepthStencilTexture**(`channel`, `uniform`, `texture`, `name?`): `void`

Sets a depth stencil texture from a render target to the according uniform.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `channel` | `number` | The texture channel |
| `uniform` | [`Nullable`](../modules.md#nullable)`WebGLUniformLocation` | The uniform to set |
| `texture` | [`Nullable`](../modules.md#nullable)[`RenderTargetTexture`](RenderTargetTexture.md) | The render target texture containing the depth stencil texture to apply |
| `name?` | `string` | The texture name |

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[setDepthStencilTexture](Engine.md#setdepthstenciltexture)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1236

___

### setDepthWrite

▸ **setDepthWrite**(`enable`): `void`

Enable or disable depth writing

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `enable` | `boolean` | defines the state to set |

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[setDepthWrite](Engine.md#setdepthwrite)

#### Defined in

packages/dev/core/src/Engines/engine.ts:829

___

### setDirectViewport

▸ **setDirectViewport**(`x`, `y`, `width`, `height`): [`Nullable`](../modules.md#nullable)`IViewportLike`

Directly set the WebGL Viewport

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | defines the x coordinate of the viewport (in screen space) |
| `y` | `number` | defines the y coordinate of the viewport (in screen space) |
| `width` | `number` | defines the width of the viewport (in screen space) |
| `height` | `number` | defines the height of the viewport (in screen space) |

#### Returns

[`Nullable`](../modules.md#nullable)`IViewportLike`

the current viewport Object (if any) that is being replaced by this call. You can restore this viewport later on to go back to the original state

#### Inherited from

[Engine](Engine.md).[setDirectViewport](Engine.md#setdirectviewport)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1071

___

### setDitheringState

▸ **setDitheringState**(`value`): `void`

Sets a boolean indicating if the dithering state is enabled or disabled

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `boolean` | defines the dithering state |

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[setDitheringState](Engine.md#setditheringstate)

#### Defined in

packages/dev/core/src/Engines/engine.ts:965

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

#### Inherited from

[Engine](Engine.md).[setExternalTexture](Engine.md#setexternaltexture)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.externalTexture.ts:19

___

### setFloat

▸ **setFloat**(`uniform`, `value`): `boolean`

Set the value of an uniform to a number (float)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniform` | `WebGLUniformLocation` | defines the webGL uniform location where to store the value |
| `value` | `number` | defines the float number to store |

#### Returns

`boolean`

true if value was set

#### Overrides

[Engine](Engine.md).[setFloat](Engine.md#setfloat)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:497

___

### setFloat2

▸ **setFloat2**(`uniform`, `x`, `y`): `boolean`

Set the value of an uniform to a vec2

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniform` | `WebGLUniformLocation` | defines the webGL uniform location where to store the value |
| `x` | `number` | defines the 1st component of the value |
| `y` | `number` | defines the 2nd component of the value |

#### Returns

`boolean`

true if value was set

#### Overrides

[Engine](Engine.md).[setFloat2](Engine.md#setfloat2)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:508

___

### setFloat3

▸ **setFloat3**(`uniform`, `x`, `y`, `z`): `boolean`

Set the value of an uniform to a vec3

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniform` | `WebGLUniformLocation` | defines the webGL uniform location where to store the value |
| `x` | `number` | defines the 1st component of the value |
| `y` | `number` | defines the 2nd component of the value |
| `z` | `number` | defines the 3rd component of the value |

#### Returns

`boolean`

true if value was set

#### Overrides

[Engine](Engine.md).[setFloat3](Engine.md#setfloat3)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:520

___

### setFloat4

▸ **setFloat4**(`uniform`, `x`, `y`, `z`, `w`): `boolean`

Set the value of an uniform to a vec4

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniform` | `WebGLUniformLocation` | defines the webGL uniform location where to store the value |
| `x` | `number` | defines the 1st component of the value |
| `y` | `number` | defines the 2nd component of the value |
| `z` | `number` | defines the 3rd component of the value |
| `w` | `number` | defines the 4th component of the value |

#### Returns

`boolean`

true if value was set

#### Overrides

[Engine](Engine.md).[setFloat4](Engine.md#setfloat4)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:543

___

### setFloatArray

▸ **setFloatArray**(`uniform`, `array`): `boolean`

Set the value of an uniform to an array of float32

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniform` | `WebGLUniformLocation` | defines the webGL uniform location where to store the value |
| `array` | `Float32Array` | defines the array of float32 to store |

#### Returns

`boolean`

true if value was set

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:387

___

### setFloatArray2

▸ **setFloatArray2**(`uniform`, `array`): `boolean`

Set the value of an uniform to an array of float32 (stored as vec2)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniform` | `WebGLUniformLocation` | defines the webGL uniform location where to store the value |
| `array` | `Float32Array` | defines the array of float32 to store |

#### Returns

`boolean`

true if value was set

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:397

___

### setFloatArray3

▸ **setFloatArray3**(`uniform`, `array`): `boolean`

Set the value of an uniform to an array of float32 (stored as vec3)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniform` | `WebGLUniformLocation` | defines the webGL uniform location where to store the value |
| `array` | `Float32Array` | defines the array of float32 to store |

#### Returns

`boolean`

true if value was set

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:407

___

### setFloatArray4

▸ **setFloatArray4**(`uniform`, `array`): `boolean`

Set the value of an uniform to an array of float32 (stored as vec4)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniform` | `WebGLUniformLocation` | defines the webGL uniform location where to store the value |
| `array` | `Float32Array` | defines the array of float32 to store |

#### Returns

`boolean`

true if value was set

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:417

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

#### Inherited from

[Engine](Engine.md).[setHardwareScalingLevel](Engine.md#sethardwarescalinglevel)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1483

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

#### Inherited from

[Engine](Engine.md).[setInt](Engine.md#setint)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:3204

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

#### Inherited from

[Engine](Engine.md).[setInt2](Engine.md#setint2)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:3221

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

#### Inherited from

[Engine](Engine.md).[setInt3](Engine.md#setint3)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:3239

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

#### Inherited from

[Engine](Engine.md).[setInt4](Engine.md#setint4)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:3258

___

### setIntArray

▸ **setIntArray**(`uniform`, `array`): `boolean`

Set the value of an uniform to an array of int32

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniform` | `WebGLUniformLocation` | defines the webGL uniform location where to store the value |
| `array` | `Int32Array` | defines the array of int32 to store |

#### Returns

`boolean`

true if value was set

#### Overrides

[Engine](Engine.md).[setIntArray](Engine.md#setintarray)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:347

___

### setIntArray2

▸ **setIntArray2**(`uniform`, `array`): `boolean`

Set the value of an uniform to an array of int32 (stored as vec2)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniform` | `WebGLUniformLocation` | defines the webGL uniform location where to store the value |
| `array` | `Int32Array` | defines the array of int32 to store |

#### Returns

`boolean`

true if value was set

#### Overrides

[Engine](Engine.md).[setIntArray2](Engine.md#setintarray2)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:357

___

### setIntArray3

▸ **setIntArray3**(`uniform`, `array`): `boolean`

Set the value of an uniform to an array of int32 (stored as vec3)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniform` | `WebGLUniformLocation` | defines the webGL uniform location where to store the value |
| `array` | `Int32Array` | defines the array of int32 to store |

#### Returns

`boolean`

true if value was set

#### Overrides

[Engine](Engine.md).[setIntArray3](Engine.md#setintarray3)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:367

___

### setIntArray4

▸ **setIntArray4**(`uniform`, `array`): `boolean`

Set the value of an uniform to an array of int32 (stored as vec4)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniform` | `WebGLUniformLocation` | defines the webGL uniform location where to store the value |
| `array` | `Int32Array` | defines the array of int32 to store |

#### Returns

`boolean`

true if value was set

#### Overrides

[Engine](Engine.md).[setIntArray4](Engine.md#setintarray4)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:377

___

### setMatrices

▸ **setMatrices**(`uniform`, `matrices`): `boolean`

Set the value of an uniform to an array of float32 (stored as matrices)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniform` | `WebGLUniformLocation` | defines the webGL uniform location where to store the value |
| `matrices` | `Float32Array` | defines the array of float32 to store |

#### Returns

`boolean`

true if value was set

#### Overrides

[Engine](Engine.md).[setMatrices](Engine.md#setmatrices)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:467

___

### setMatrix2x2

▸ **setMatrix2x2**(`uniform`, `matrix`): `boolean`

Set the value of an uniform to a matrix (2x2)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniform` | `WebGLUniformLocation` | defines the webGL uniform location where to store the value |
| `matrix` | `Float32Array` | defines the Float32Array representing the 2x2 matrix to store |

#### Returns

`boolean`

true if value was set

#### Overrides

[Engine](Engine.md).[setMatrix2x2](Engine.md#setmatrix2x2)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:487

___

### setMatrix3x3

▸ **setMatrix3x3**(`uniform`, `matrix`): `boolean`

Set the value of an uniform to a matrix (3x3)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniform` | `WebGLUniformLocation` | defines the webGL uniform location where to store the value |
| `matrix` | `Float32Array` | defines the Float32Array representing the 3x3 matrix to store |

#### Returns

`boolean`

true if value was set

#### Overrides

[Engine](Engine.md).[setMatrix3x3](Engine.md#setmatrix3x3)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:477

___

### setRasterizerState

▸ **setRasterizerState**(`value`): `void`

Sets a boolean indicating if the rasterizer state is enabled or disabled

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `boolean` | defines the rasterizer state |

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[setRasterizerState](Engine.md#setrasterizerstate)

#### Defined in

packages/dev/core/src/Engines/engine.ts:977

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

#### Inherited from

[Engine](Engine.md).[setSize](Engine.md#setsize)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1442

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

#### Overrides

[Engine](Engine.md).[setState](Engine.md#setstate)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:331

___

### setStencilBuffer

▸ **setStencilBuffer**(`enable`): `void`

Enable or disable the stencil buffer

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `enable` | `boolean` | defines if the stencil buffer must be enabled or disabled |

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[setStencilBuffer](Engine.md#setstencilbuffer)

#### Defined in

packages/dev/core/src/Engines/engine.ts:845

___

### setStencilFunction

▸ **setStencilFunction**(`stencilFunc`): `void`

Sets the current stencil function

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `stencilFunc` | `number` | defines the new stencil function to use |

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[setStencilFunction](Engine.md#setstencilfunction)

#### Defined in

packages/dev/core/src/Engines/engine.ts:893

___

### setStencilFunctionMask

▸ **setStencilFunctionMask**(`mask`): `void`

Sets the current stencil mask

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mask` | `number` | defines the new stencil mask to use |

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[setStencilFunctionMask](Engine.md#setstencilfunctionmask)

#### Defined in

packages/dev/core/src/Engines/engine.ts:909

___

### setStencilFunctionReference

▸ **setStencilFunctionReference**(`reference`): `void`

Sets the current stencil reference

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `reference` | `number` | defines the new stencil reference to use |

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[setStencilFunctionReference](Engine.md#setstencilfunctionreference)

#### Defined in

packages/dev/core/src/Engines/engine.ts:901

___

### setStencilMask

▸ **setStencilMask**(`mask`): `void`

Sets the current stencil mask

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mask` | `number` | defines the new stencil mask to use |

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[setStencilMask](Engine.md#setstencilmask)

#### Defined in

packages/dev/core/src/Engines/engine.ts:861

___

### setStencilOperationDepthFail

▸ **setStencilOperationDepthFail**(`operation`): `void`

Sets the stencil operation to use when depth fails

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `operation` | `number` | defines the stencil operation to use when depth fails |

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[setStencilOperationDepthFail](Engine.md#setstenciloperationdepthfail)

#### Defined in

packages/dev/core/src/Engines/engine.ts:949

___

### setStencilOperationFail

▸ **setStencilOperationFail**(`operation`): `void`

Sets the stencil operation to use when stencil fails

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `operation` | `number` | defines the stencil operation to use when stencil fails |

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[setStencilOperationFail](Engine.md#setstenciloperationfail)

#### Defined in

packages/dev/core/src/Engines/engine.ts:941

___

### setStencilOperationPass

▸ **setStencilOperationPass**(`operation`): `void`

Sets the stencil operation to use when stencil passes

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `operation` | `number` | defines the stencil operation to use when stencil passes |

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[setStencilOperationPass](Engine.md#setstenciloperationpass)

#### Defined in

packages/dev/core/src/Engines/engine.ts:957

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

#### Inherited from

[Engine](Engine.md).[setStorageBuffer](Engine.md#setstoragebuffer)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.storageBuffer.ts:41

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

#### Inherited from

[Engine](Engine.md).[setTexture](Engine.md#settexture)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:5029

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

#### Inherited from

[Engine](Engine.md).[setTextureArray](Engine.md#settexturearray)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:5162

___

### setTextureFormatToUse

▸ **setTextureFormatToUse**(`formatsAvailable`): [`Nullable`](../modules.md#nullable)`string`

Set the compressed texture format to use, based on the formats you have, and the formats
supported by the hardware / browser.

Khronos Texture Container (.ktx) files are used to support this.  This format has the
advantage of being specifically designed for OpenGL.  Header elements directly correspond
to API arguments needed to compressed textures.  This puts the burden on the container
generator to house the arcane code for determining these for current & future formats.

for description see https://www.khronos.org/opengles/sdk/tools/KTX/
for file layout see https://www.khronos.org/opengles/sdk/tools/KTX/file_format_spec/

Note: The result of this call is not taken into account when a texture is base64.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `formatsAvailable` | `string`[] | defines the list of those format families you have created  on your server.  Syntax: '-' + format family + '.ktx'.  (Case and order do not matter.)    Current families are astc, dxt, pvrtc, etc2, & etc1. |

#### Returns

[`Nullable`](../modules.md#nullable)`string`

The extension selected.

#### Inherited from

[Engine](Engine.md).[setTextureFormatToUse](Engine.md#settextureformattouse)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.textureSelector.ts:50

___

### setTextureFromPostProcess

▸ **setTextureFromPostProcess**(`channel`, `postProcess`, `name`): `void`

Sets a texture to the webGL context from a postprocess

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `channel` | `number` | defines the channel to use |
| `postProcess` | [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md) | defines the source postprocess |
| `name` | `string` | name of the channel |

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[setTextureFromPostProcess](Engine.md#settexturefrompostprocess)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1258

___

### setTextureFromPostProcessOutput

▸ **setTextureFromPostProcessOutput**(`channel`, `postProcess`, `name`): `void`

Binds the output of the passed in post process to the texture channel specified

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `channel` | `number` | The channel the texture should be bound to |
| `postProcess` | [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md) | The post process which's output should be bound |
| `name` | `string` | name of the channel |

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[setTextureFromPostProcessOutput](Engine.md#settexturefrompostprocessoutput)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1277

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

#### Inherited from

[Engine](Engine.md).[setTextureSampler](Engine.md#settexturesampler)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.textureSampler.ts:13

___

### setTranformFeedbackVaryings

▸ **setTranformFeedbackVaryings**(`program`, `value`): `void`

Specify the varyings to use with transform feedback

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `program` | `WebGLProgram` | defines the associated webGL program |
| `value` | `string`[] | defines the list of strings representing the varying names |

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[setTranformFeedbackVaryings](Engine.md#settranformfeedbackvaryings)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.transformFeedback.ts:46

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

#### Overrides

[Engine](Engine.md).[setViewport](Engine.md#setviewport)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:262

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

#### Inherited from

[Engine](Engine.md).[setZOffset](Engine.md#setzoffset)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1926

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

#### Inherited from

[Engine](Engine.md).[setZOffsetUnits](Engine.md#setzoffsetunits)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1943

___

### snapshotRenderingReset

▸ **snapshotRenderingReset**(): `void`

Creates a new snapshot at the next frame using the current snapshotRenderingMode

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[snapshotRenderingReset](Engine.md#snapshotrenderingreset)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:717

___

### startTimeQuery

▸ **startTimeQuery**(): [`Nullable`](../modules.md#nullable)`_TimeToken`

Starts a time query (used to measure time spent by the GPU on a specific frame)
Please note that only one query can be issued at a time

#### Returns

[`Nullable`](../modules.md#nullable)`_TimeToken`

a time token used to track the time span

#### Inherited from

[Engine](Engine.md).[startTimeQuery](Engine.md#starttimequery)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.query.ts:87

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

#### Inherited from

[Engine](Engine.md).[stopRenderLoop](Engine.md#stoprenderloop)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1518

___

### switchFullscreen

▸ **switchFullscreen**(`requestPointerLock`): `void`

Toggle full screen mode

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `requestPointerLock` | `boolean` | defines if a pointer lock should be requested from the user |

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[switchFullscreen](Engine.md#switchfullscreen)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1356

___

### unBindFramebuffer

▸ **unBindFramebuffer**(`rtWrapper`, `disableGenerateMipMaps?`, `onBeforeUnbind?`): `void`

Unbind the current render target texture from the webGL context

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `rtWrapper` | [`RenderTargetWrapper`](RenderTargetWrapper.md) | `undefined` | defines the render target wrapper to unbind |
| `disableGenerateMipMaps` | `boolean` | `false` | defines a boolean indicating that mipmaps must not be generated |
| `onBeforeUnbind?` | () => `void` | `undefined` | defines a function which will be called before the effective unbind |

#### Returns

`void`

#### Overrides

[Engine](Engine.md).[unBindFramebuffer](Engine.md#unbindframebuffer)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:869

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

#### Inherited from

[Engine](Engine.md).[unBindMultiColorAttachmentFramebuffer](Engine.md#unbindmulticolorattachmentframebuffer)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.multiRender.ts:21

___

### unRegisterView

▸ **unRegisterView**(`canvas`): [`Engine`](Engine.md)

Remove a registered child canvas

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `canvas` | `HTMLCanvasElement` | defines the canvas to remove |

#### Returns

[`Engine`](Engine.md)

the current engine

#### Inherited from

[Engine](Engine.md).[unRegisterView](Engine.md#unregisterview)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.views.ts:62

___

### unbindAllAttributes

▸ **unbindAllAttributes**(): `void`

Unbind all vertex attributes from the webGL context

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[unbindAllAttributes](Engine.md#unbindallattributes)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:5229

___

### unbindAllTextures

▸ **unbindAllTextures**(): `void`

Unbind all textures from the webGL context

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[unbindAllTextures](Engine.md#unbindalltextures)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:5010

___

### unbindInstanceAttributes

▸ **unbindInstanceAttributes**(): `void`

Unbind all instance attributes

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[unbindInstanceAttributes](Engine.md#unbindinstanceattributes)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:2436

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

#### Inherited from

[Engine](Engine.md).[updateAndBindInstancesBuffer](Engine.md#updateandbindinstancesbuffer)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:2484

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

#### Inherited from

[Engine](Engine.md).[updateArrayBuffer](Engine.md#updatearraybuffer)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:2191

___

### updateDynamicIndexBuffer

▸ **updateDynamicIndexBuffer**(`indexBuffer`, `indices`, `offset?`): `void`

Update a dynamic index buffer

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `indexBuffer` | `WebGLBuffer` | `undefined` | defines the target index buffer |
| `indices` | [`IndicesArray`](../modules.md#indicesarray) | `undefined` | defines the data to update |
| `offset` | `number` | `0` | defines the offset in the target index buffer where update should start |

#### Returns

`void`

#### Overrides

[Engine](Engine.md).[updateDynamicIndexBuffer](Engine.md#updatedynamicindexbuffer)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:935

___

### updateDynamicTexture

▸ **updateDynamicTexture**(`texture`, `canvas`, `invertY`, `premulAlpha?`, `format?`): `void`

Update the content of a dynamic texture

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `texture` | [`Nullable`](../modules.md#nullable)[`InternalTexture`](InternalTexture.md) | `undefined` | defines the texture to update |
| `canvas` | `HTMLCanvasElement` | `undefined` | defines the canvas containing the source |
| `invertY` | `boolean` | `undefined` | defines if data must be stored with Y axis inverted |
| `premulAlpha` | `boolean` | `false` | defines if alpha is stored as premultiplied |
| `format?` | `number` | `undefined` | defines the format of the data |

#### Returns

`void`

#### Overrides

[Engine](Engine.md).[updateDynamicTexture](Engine.md#updatedynamictexture)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:898

___

### updateDynamicVertexBuffer

▸ **updateDynamicVertexBuffer**(`vertexBuffer`, `vertices`, `byteOffset?`, `byteLength?`): `void`

Updates a dynamic vertex buffer.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vertexBuffer` | `WebGLBuffer` | the vertex buffer to update |
| `vertices` | [`FloatArray`](../modules.md#floatarray) | the data used to update the vertex buffer |
| `byteOffset?` | `number` | the byte offset of the data (optional) |
| `byteLength?` | `number` | the byte length of the data (optional) |

#### Returns

`void`

#### Overrides

[Engine](Engine.md).[updateDynamicVertexBuffer](Engine.md#updatedynamicvertexbuffer)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:944

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

#### Inherited from

[Engine](Engine.md).[updateMultipleRenderTargetTextureSampleCount](Engine.md#updatemultiplerendertargettexturesamplecount)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.multiRender.ts:41

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

#### Inherited from

[Engine](Engine.md).[updateRawCubeTexture](Engine.md#updaterawcubetexture)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.rawTexture.ts:101

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

#### Inherited from

[Engine](Engine.md).[updateRawCubeTexture](Engine.md#updaterawcubetexture)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.rawTexture.ts:112

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

#### Inherited from

[Engine](Engine.md).[updateRawCubeTexture](Engine.md#updaterawcubetexture)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.rawTexture.ts:124

___

### updateRawTexture

▸ **updateRawTexture**(`texture`, `data`, `format`, `invertY`, `compression?`, `type?`, `useSRGBBuffer?`): `void`

Update a raw texture

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `texture` | [`Nullable`](../modules.md#nullable)[`InternalTexture`](InternalTexture.md) | `undefined` | defines the texture to update |
| `data` | [`Nullable`](../modules.md#nullable)`ArrayBufferView` | `undefined` | defines the data to store in the texture |
| `format` | `number` | `undefined` | defines the format of the data |
| `invertY` | `boolean` | `undefined` | defines if data must be stored with Y axis inverted |
| `compression` | [`Nullable`](../modules.md#nullable)`string` | `null` | defines the compression used (null by default) |
| `type` | `number` | `Constants.TEXTURETYPE_UNSIGNED_INT` | defines the type fo the data (Engine.TEXTURETYPE_UNSIGNED_INT by default) |
| `useSRGBBuffer` | `boolean` | `false` | defines if the texture must be loaded in a sRGB GPU buffer (if supported by the GPU). |

#### Returns

`void`

#### Overrides

[Engine](Engine.md).[updateRawTexture](Engine.md#updaterawtexture)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:825

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

#### Inherited from

[Engine](Engine.md).[updateRawTexture2DArray](Engine.md#updaterawtexture2darray)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.rawTexture.ts:269

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

#### Inherited from

[Engine](Engine.md).[updateRawTexture2DArray](Engine.md#updaterawtexture2darray)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.rawTexture.ts:280

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

#### Inherited from

[Engine](Engine.md).[updateRawTexture3D](Engine.md#updaterawtexture3d)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.rawTexture.ts:220

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

#### Inherited from

[Engine](Engine.md).[updateRawTexture3D](Engine.md#updaterawtexture3d)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.rawTexture.ts:231

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

#### Inherited from

[Engine](Engine.md).[updateRenderTargetTextureSampleCount](Engine.md#updaterendertargettexturesamplecount)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.renderTarget.ts:45

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

#### Inherited from

[Engine](Engine.md).[updateStorageBuffer](Engine.md#updatestoragebuffer)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.storageBuffer.ts:24

___

### updateTextureComparisonFunction

▸ **updateTextureComparisonFunction**(`texture`, `comparisonFunction`): `void`

Updates a depth texture Comparison Mode and Function.
If the comparison Function is equal to 0, the mode will be set to none.
Otherwise, this only works in webgl 2 and requires a shadow sampler in the shader.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `texture` | [`InternalTexture`](InternalTexture.md) | The texture to set the comparison function for |
| `comparisonFunction` | `number` | The comparison function to set, 0 if no comparison required |

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[updateTextureComparisonFunction](Engine.md#updatetexturecomparisonfunction)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1762

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

#### Inherited from

[Engine](Engine.md).[updateTextureData](Engine.md#updatetexturedata)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:4650

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

#### Inherited from

[Engine](Engine.md).[updateTextureDimensions](Engine.md#updatetexturedimensions)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:4431

___

### updateTextureSamplingMode

▸ **updateTextureSamplingMode**(`samplingMode`, `texture`): `void`

Update the sampling mode of a given texture

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `samplingMode` | `number` | defines the required sampling mode |
| `texture` | [`InternalTexture`](InternalTexture.md) | defines the texture to update |

#### Returns

`void`

#### Overrides

[Engine](Engine.md).[updateTextureSamplingMode](Engine.md#updatetexturesamplingmode)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:763

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

#### Inherited from

[Engine](Engine.md).[updateTextureWrappingMode](Engine.md#updatetexturewrappingmode)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:4440

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

#### Inherited from

[Engine](Engine.md).[updateUniformBuffer](Engine.md#updateuniformbuffer)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.uniformBuffer.ts:34

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

#### Inherited from

[Engine](Engine.md).[updateVideoTexture](Engine.md#updatevideotexture)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.videoTexture.ts:13

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

#### Overrides

[Engine](Engine.md).[wipeCaches](Engine.md#wipecaches)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:579

___

### wrapWebGLTexture

▸ **wrapWebGLTexture**(`texture`): [`InternalTexture`](InternalTexture.md)

Wraps an external web gl texture in a Babylon texture.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `texture` | `WebGLTexture` | defines the external texture |

#### Returns

[`InternalTexture`](InternalTexture.md)

the babylon internal texture

#### Inherited from

[Engine](Engine.md).[wrapWebGLTexture](Engine.md#wrapwebgltexture)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1719

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

#### Inherited from

[Engine](Engine.md).[CeilingPOT](Engine.md#ceilingpot)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:5855

___

### DefaultLoadingScreenFactory

▸ `Static` **DefaultLoadingScreenFactory**(`canvas`): [`ILoadingScreen`](../interfaces/ILoadingScreen.md)

Method called to create the default loading screen.
This can be overridden in your own app.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `canvas` | `HTMLCanvasElement` | The rendering canvas element |

#### Returns

[`ILoadingScreen`](../interfaces/ILoadingScreen.md)

The loading screen

#### Inherited from

[Engine](Engine.md).[DefaultLoadingScreenFactory](Engine.md#defaultloadingscreenfactory)

#### Defined in

packages/dev/core/src/Engines/engine.ts:377

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

#### Inherited from

[Engine](Engine.md).[FloorPOT](Engine.md#floorpot)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:5871

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

#### Inherited from

[Engine](Engine.md).[GetExponentOfTwo](Engine.md#getexponentoftwo)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:5898

___

### MarkAllMaterialsAsDirty

▸ `Static` **MarkAllMaterialsAsDirty**(`flag`, `predicate?`): `void`

Will flag all materials in all scenes in all engines as dirty to trigger new shader compilation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `flag` | `number` | defines which part of the materials must be marked as dirty |
| `predicate?` | (`mat`: [`Material`](Material.md)) => `boolean` | defines a predicate used to filter which materials should be affected |

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[MarkAllMaterialsAsDirty](Engine.md#markallmaterialsasdirty)

#### Defined in

packages/dev/core/src/Engines/engine.ts:360

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

#### Inherited from

[Engine](Engine.md).[NearestPOT](Engine.md#nearestpot)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:5885

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

#### Inherited from

[Engine](Engine.md).[QueueNewFrame](Engine.md#queuenewframe)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:5923

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

#### Inherited from

[Engine](Engine.md).[_ConcatenateShader](Engine.md#_concatenateshader)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:2837

___

### \_ExitFullscreen

▸ `Static` **_ExitFullscreen**(): `void`

Asks the browser to exit fullscreen mode

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[_ExitFullscreen](Engine.md#_exitfullscreen)

#### Defined in

packages/dev/core/src/Engines/engine.ts:2094

___

### \_ExitPointerlock

▸ `Static` **_ExitPointerlock**(): `void`

Asks the browser to exit pointerlock mode

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[_ExitPointerlock](Engine.md#_exitpointerlock)

#### Defined in

packages/dev/core/src/Engines/engine.ts:2070

___

### \_RequestFullscreen

▸ `Static` **_RequestFullscreen**(`element`): `void`

Ask the browser to promote the current element to fullscreen rendering mode

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `element` | `HTMLElement` | defines the DOM element to promote |

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[_RequestFullscreen](Engine.md#_requestfullscreen)

#### Defined in

packages/dev/core/src/Engines/engine.ts:2083

___

### \_RequestPointerlock

▸ `Static` **_RequestPointerlock**(`element`): `void`

Ask the browser to promote the current element to pointerlock mode

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `element` | `HTMLElement` | defines the DOM element to promote |

#### Returns

`void`

#### Inherited from

[Engine](Engine.md).[_RequestPointerlock](Engine.md#_requestpointerlock)

#### Defined in

packages/dev/core/src/Engines/engine.ts:2058

___

### isSupported

▸ `Static` **isSupported**(): `boolean`

Gets a boolean indicating if the engine can be instantiated (ie. if a webGL context can be found)

**`Ignorenaming`**

#### Returns

`boolean`

true if the engine can be created

#### Inherited from

[Engine](Engine.md).[isSupported](Engine.md#issupported-1)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:5811
