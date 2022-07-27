[@dev/core](../README.md) / [Exports](../modules.md) / Engine

# Class: Engine

The engine class is responsible for interfacing with all lower-level APIs such as WebGL and Audio

## Hierarchy

- [`ThinEngine`](ThinEngine.md)

  ↳ **`Engine`**

  ↳↳ [`NullEngine`](NullEngine.md)

  ↳↳ [`WebGPUEngine`](WebGPUEngine.md)

## Table of contents

### Constructors

- [constructor](Engine.md#constructor)

### Properties

- [\_activeRenderLoops](Engine.md#_activerenderloops)
- [\_audioContext](Engine.md#_audiocontext)
- [\_audioDestination](Engine.md#_audiodestination)
- [\_boundUniforms](Engine.md#_bounduniforms)
- [\_cachedStencilBuffer](Engine.md#_cachedstencilbuffer)
- [\_cachedStencilFunction](Engine.md#_cachedstencilfunction)
- [\_cachedStencilMask](Engine.md#_cachedstencilmask)
- [\_cachedStencilOperationDepthFail](Engine.md#_cachedstenciloperationdepthfail)
- [\_cachedStencilOperationFail](Engine.md#_cachedstenciloperationfail)
- [\_cachedStencilOperationPass](Engine.md#_cachedstenciloperationpass)
- [\_cachedStencilReference](Engine.md#_cachedstencilreference)
- [\_compatibilityMode](Engine.md#_compatibilitymode)
- [\_compiledEffects](Engine.md#_compiledeffects)
- [\_contextWasLost](Engine.md#_contextwaslost)
- [\_creationOptions](Engine.md#_creationoptions)
- [\_currentBoundBuffer](Engine.md#_currentboundbuffer)
- [\_currentEffect](Engine.md#_currenteffect)
- [\_deltaTime](Engine.md#_deltatime)
- [\_deterministicLockstep](Engine.md#_deterministiclockstep)
- [\_fps](Engine.md#_fps)
- [\_highPrecisionShadersAllowed](Engine.md#_highprecisionshadersallowed)
- [\_isStencilEnable](Engine.md#_isstencilenable)
- [\_loadingScreen](Engine.md#_loadingscreen)
- [\_lockstepMaxSteps](Engine.md#_lockstepmaxsteps)
- [\_onBlur](Engine.md#_onblur)
- [\_onCanvasBlur](Engine.md#_oncanvasblur)
- [\_onCanvasContextMenu](Engine.md#_oncanvascontextmenu)
- [\_onCanvasFocus](Engine.md#_oncanvasfocus)
- [\_onCanvasPointerOut](Engine.md#_oncanvaspointerout)
- [\_onFocus](Engine.md#_onfocus)
- [\_onFullscreenChange](Engine.md#_onfullscreenchange)
- [\_onPointerLockChange](Engine.md#_onpointerlockchange)
- [\_performanceMonitor](Engine.md#_performancemonitor)
- [\_pointerLockRequested](Engine.md#_pointerlockrequested)
- [\_renderPassNames](Engine.md#_renderpassnames)
- [\_renderingCanvas](Engine.md#_renderingcanvas)
- [\_renderingQueueLaunched](Engine.md#_renderingqueuelaunched)
- [\_rescalePostProcess](Engine.md#_rescalepostprocess)
- [\_shaderProcessor](Engine.md#_shaderprocessor)
- [\_snapshotRenderingMode](Engine.md#_snapshotrenderingmode)
- [\_timeStep](Engine.md#_timestep)
- [\_useExactSrgbConversions](Engine.md#_useexactsrgbconversions)
- [\_viewportCached](Engine.md#_viewportcached)
- [\_windowIsBackground](Engine.md#_windowisbackground)
- [activeView](Engine.md#activeview)
- [adaptToDeviceRatio](Engine.md#adapttodeviceratio)
- [canvasTabIndex](Engine.md#canvastabindex)
- [cullBackFaces](Engine.md#cullbackfaces)
- [currentRenderPassId](Engine.md#currentrenderpassid)
- [customAnimationFrameRequester](Engine.md#customanimationframerequester)
- [disableContextMenu](Engine.md#disablecontextmenu)
- [disableManifestCheck](Engine.md#disablemanifestcheck)
- [disablePerformanceMonitorInBackground](Engine.md#disableperformancemonitorinbackground)
- [disableUniformBuffers](Engine.md#disableuniformbuffers)
- [disableVertexArrayObjects](Engine.md#disablevertexarrayobjects)
- [enableOfflineSupport](Engine.md#enableofflinesupport)
- [enableUnpackFlipYCached](Engine.md#enableunpackflipycached)
- [forcePOTTextures](Engine.md#forcepottextures)
- [hasOriginBottomLeft](Engine.md#hasoriginbottomleft)
- [hostInformation](Engine.md#hostinformation)
- [inputElement](Engine.md#inputelement)
- [isFullscreen](Engine.md#isfullscreen)
- [isInVRExclusivePointerMode](Engine.md#isinvrexclusivepointermode)
- [isNDCHalfZRange](Engine.md#isndchalfzrange)
- [isPointerLock](Engine.md#ispointerlock)
- [onAfterShaderCompilationObservable](Engine.md#onaftershadercompilationobservable)
- [onBeforeShaderCompilationObservable](Engine.md#onbeforeshadercompilationobservable)
- [onBeforeTextureInitObservable](Engine.md#onbeforetextureinitobservable)
- [onBeginFrameObservable](Engine.md#onbeginframeobservable)
- [onCanvasBlurObservable](Engine.md#oncanvasblurobservable)
- [onCanvasFocusObservable](Engine.md#oncanvasfocusobservable)
- [onCanvasPointerOutObservable](Engine.md#oncanvaspointeroutobservable)
- [onContextLostObservable](Engine.md#oncontextlostobservable)
- [onContextRestoredObservable](Engine.md#oncontextrestoredobservable)
- [onDisposeObservable](Engine.md#ondisposeobservable)
- [onEndFrameObservable](Engine.md#onendframeobservable)
- [onNewSceneAddedObservable](Engine.md#onnewsceneaddedobservable)
- [onResizeObservable](Engine.md#onresizeobservable)
- [onVRDisplayChangedObservable](Engine.md#onvrdisplaychangedobservable)
- [onVRRequestPresentComplete](Engine.md#onvrrequestpresentcomplete)
- [onVRRequestPresentStart](Engine.md#onvrrequestpresentstart)
- [postProcesses](Engine.md#postprocesses)
- [premultipliedAlpha](Engine.md#premultipliedalpha)
- [preventCacheWipeBetweenFrames](Engine.md#preventcachewipebetweenframes)
- [renderEvenInBackground](Engine.md#rendereveninbackground)
- [scenes](Engine.md#scenes)
- [textureFormatInUse](Engine.md#textureformatinuse)
- [texturesSupported](Engine.md#texturessupported)
- [validateShaderPrograms](Engine.md#validateshaderprograms)
- [views](Engine.md#views)
- [vrPresentationAttributes](Engine.md#vrpresentationattributes)
- [ALPHA\_ADD](Engine.md#alpha_add)
- [ALPHA\_COMBINE](Engine.md#alpha_combine)
- [ALPHA\_DISABLE](Engine.md#alpha_disable)
- [ALPHA\_INTERPOLATE](Engine.md#alpha_interpolate)
- [ALPHA\_MAXIMIZED](Engine.md#alpha_maximized)
- [ALPHA\_MULTIPLY](Engine.md#alpha_multiply)
- [ALPHA\_ONEONE](Engine.md#alpha_oneone)
- [ALPHA\_PREMULTIPLIED](Engine.md#alpha_premultiplied)
- [ALPHA\_PREMULTIPLIED\_PORTERDUFF](Engine.md#alpha_premultiplied_porterduff)
- [ALPHA\_SCREENMODE](Engine.md#alpha_screenmode)
- [ALPHA\_SUBTRACT](Engine.md#alpha_subtract)
- [ALWAYS](Engine.md#always)
- [AudioEngineFactory](Engine.md#audioenginefactory)
- [CollisionsEpsilon](Engine.md#collisionsepsilon)
- [DECR](Engine.md#decr)
- [DECR\_WRAP](Engine.md#decr_wrap)
- [DELAYLOADSTATE\_LOADED](Engine.md#delayloadstate_loaded)
- [DELAYLOADSTATE\_LOADING](Engine.md#delayloadstate_loading)
- [DELAYLOADSTATE\_NONE](Engine.md#delayloadstate_none)
- [DELAYLOADSTATE\_NOTLOADED](Engine.md#delayloadstate_notloaded)
- [EQUAL](Engine.md#equal)
- [ExceptionList](Engine.md#exceptionlist)
- [GEQUAL](Engine.md#gequal)
- [GREATER](Engine.md#greater)
- [INCR](Engine.md#incr)
- [INCR\_WRAP](Engine.md#incr_wrap)
- [INVERT](Engine.md#invert)
- [KEEP](Engine.md#keep)
- [LEQUAL](Engine.md#lequal)
- [LESS](Engine.md#less)
- [NEVER](Engine.md#never)
- [NOTEQUAL](Engine.md#notequal)
- [OfflineProviderFactory](Engine.md#offlineproviderfactory)
- [REPLACE](Engine.md#replace)
- [SCALEMODE\_CEILING](Engine.md#scalemode_ceiling)
- [SCALEMODE\_FLOOR](Engine.md#scalemode_floor)
- [SCALEMODE\_NEAREST](Engine.md#scalemode_nearest)
- [TEXTUREFORMAT\_ALPHA](Engine.md#textureformat_alpha)
- [TEXTUREFORMAT\_LUMINANCE](Engine.md#textureformat_luminance)
- [TEXTUREFORMAT\_LUMINANCE\_ALPHA](Engine.md#textureformat_luminance_alpha)
- [TEXTUREFORMAT\_R](Engine.md#textureformat_r)
- [TEXTUREFORMAT\_RED](Engine.md#textureformat_red)
- [TEXTUREFORMAT\_RED\_INTEGER](Engine.md#textureformat_red_integer)
- [TEXTUREFORMAT\_RG](Engine.md#textureformat_rg)
- [TEXTUREFORMAT\_RGB](Engine.md#textureformat_rgb)
- [TEXTUREFORMAT\_RGBA](Engine.md#textureformat_rgba)
- [TEXTUREFORMAT\_RGBA\_INTEGER](Engine.md#textureformat_rgba_integer)
- [TEXTUREFORMAT\_RGB\_INTEGER](Engine.md#textureformat_rgb_integer)
- [TEXTUREFORMAT\_RG\_INTEGER](Engine.md#textureformat_rg_integer)
- [TEXTUREFORMAT\_R\_INTEGER](Engine.md#textureformat_r_integer)
- [TEXTURETYPE\_BYTE](Engine.md#texturetype_byte)
- [TEXTURETYPE\_FLOAT](Engine.md#texturetype_float)
- [TEXTURETYPE\_FLOAT\_32\_UNSIGNED\_INT\_24\_8\_REV](Engine.md#texturetype_float_32_unsigned_int_24_8_rev)
- [TEXTURETYPE\_HALF\_FLOAT](Engine.md#texturetype_half_float)
- [TEXTURETYPE\_INT](Engine.md#texturetype_int)
- [TEXTURETYPE\_SHORT](Engine.md#texturetype_short)
- [TEXTURETYPE\_UNSIGNED\_BYTE](Engine.md#texturetype_unsigned_byte)
- [TEXTURETYPE\_UNSIGNED\_INT](Engine.md#texturetype_unsigned_int)
- [TEXTURETYPE\_UNSIGNED\_INTEGER](Engine.md#texturetype_unsigned_integer)
- [TEXTURETYPE\_UNSIGNED\_INT\_10F\_11F\_11F\_REV](Engine.md#texturetype_unsigned_int_10f_11f_11f_rev)
- [TEXTURETYPE\_UNSIGNED\_INT\_24\_8](Engine.md#texturetype_unsigned_int_24_8)
- [TEXTURETYPE\_UNSIGNED\_INT\_2\_10\_10\_10\_REV](Engine.md#texturetype_unsigned_int_2_10_10_10_rev)
- [TEXTURETYPE\_UNSIGNED\_INT\_5\_9\_9\_9\_REV](Engine.md#texturetype_unsigned_int_5_9_9_9_rev)
- [TEXTURETYPE\_UNSIGNED\_SHORT](Engine.md#texturetype_unsigned_short)
- [TEXTURETYPE\_UNSIGNED\_SHORT\_4\_4\_4\_4](Engine.md#texturetype_unsigned_short_4_4_4_4)
- [TEXTURETYPE\_UNSIGNED\_SHORT\_5\_5\_5\_1](Engine.md#texturetype_unsigned_short_5_5_5_1)
- [TEXTURETYPE\_UNSIGNED\_SHORT\_5\_6\_5](Engine.md#texturetype_unsigned_short_5_6_5)
- [TEXTURE\_BILINEAR\_SAMPLINGMODE](Engine.md#texture_bilinear_samplingmode)
- [TEXTURE\_CLAMP\_ADDRESSMODE](Engine.md#texture_clamp_addressmode)
- [TEXTURE\_CUBIC\_MODE](Engine.md#texture_cubic_mode)
- [TEXTURE\_EQUIRECTANGULAR\_MODE](Engine.md#texture_equirectangular_mode)
- [TEXTURE\_EXPLICIT\_MODE](Engine.md#texture_explicit_mode)
- [TEXTURE\_FIXED\_EQUIRECTANGULAR\_MIRRORED\_MODE](Engine.md#texture_fixed_equirectangular_mirrored_mode)
- [TEXTURE\_FIXED\_EQUIRECTANGULAR\_MODE](Engine.md#texture_fixed_equirectangular_mode)
- [TEXTURE\_INVCUBIC\_MODE](Engine.md#texture_invcubic_mode)
- [TEXTURE\_LINEAR\_LINEAR](Engine.md#texture_linear_linear)
- [TEXTURE\_LINEAR\_LINEAR\_MIPLINEAR](Engine.md#texture_linear_linear_miplinear)
- [TEXTURE\_LINEAR\_LINEAR\_MIPNEAREST](Engine.md#texture_linear_linear_mipnearest)
- [TEXTURE\_LINEAR\_NEAREST](Engine.md#texture_linear_nearest)
- [TEXTURE\_LINEAR\_NEAREST\_MIPLINEAR](Engine.md#texture_linear_nearest_miplinear)
- [TEXTURE\_LINEAR\_NEAREST\_MIPNEAREST](Engine.md#texture_linear_nearest_mipnearest)
- [TEXTURE\_MIRROR\_ADDRESSMODE](Engine.md#texture_mirror_addressmode)
- [TEXTURE\_NEAREST\_LINEAR](Engine.md#texture_nearest_linear)
- [TEXTURE\_NEAREST\_LINEAR\_MIPLINEAR](Engine.md#texture_nearest_linear_miplinear)
- [TEXTURE\_NEAREST\_LINEAR\_MIPNEAREST](Engine.md#texture_nearest_linear_mipnearest)
- [TEXTURE\_NEAREST\_NEAREST](Engine.md#texture_nearest_nearest)
- [TEXTURE\_NEAREST\_NEAREST\_MIPLINEAR](Engine.md#texture_nearest_nearest_miplinear)
- [TEXTURE\_NEAREST\_NEAREST\_MIPNEAREST](Engine.md#texture_nearest_nearest_mipnearest)
- [TEXTURE\_NEAREST\_SAMPLINGMODE](Engine.md#texture_nearest_samplingmode)
- [TEXTURE\_PLANAR\_MODE](Engine.md#texture_planar_mode)
- [TEXTURE\_PROJECTION\_MODE](Engine.md#texture_projection_mode)
- [TEXTURE\_SKYBOX\_MODE](Engine.md#texture_skybox_mode)
- [TEXTURE\_SPHERICAL\_MODE](Engine.md#texture_spherical_mode)
- [TEXTURE\_TRILINEAR\_SAMPLINGMODE](Engine.md#texture_trilinear_samplingmode)
- [TEXTURE\_WRAP\_ADDRESSMODE](Engine.md#texture_wrap_addressmode)
- [\_RenderPassIdCounter](Engine.md#_renderpassidcounter)
- [\_RescalePostProcessFactory](Engine.md#_rescalepostprocessfactory)
- [audioEngine](Engine.md#audioengine)

### Accessors

- [\_supportsHardwareTextureRescaling](Engine.md#_supportshardwaretexturerescaling)
- [activeRenderLoops](Engine.md#activerenderloops)
- [alphaState](Engine.md#alphastate)
- [compatibilityMode](Engine.md#compatibilitymode)
- [currentViewport](Engine.md#currentviewport)
- [depthCullingState](Engine.md#depthcullingstate)
- [description](Engine.md#description)
- [doNotHandleContextLost](Engine.md#donothandlecontextlost)
- [emptyCubeTexture](Engine.md#emptycubetexture)
- [emptyTexture](Engine.md#emptytexture)
- [emptyTexture2DArray](Engine.md#emptytexture2darray)
- [emptyTexture3D](Engine.md#emptytexture3d)
- [frameId](Engine.md#frameid)
- [framebufferDimensionsObject](Engine.md#framebufferdimensionsobject)
- [isStencilEnable](Engine.md#isstencilenable)
- [isWebGPU](Engine.md#iswebgpu)
- [loadingScreen](Engine.md#loadingscreen)
- [loadingUIBackgroundColor](Engine.md#loadinguibackgroundcolor)
- [loadingUIText](Engine.md#loadinguitext)
- [name](Engine.md#name)
- [needPOTTextures](Engine.md#needpottextures)
- [performanceMonitor](Engine.md#performancemonitor)
- [shaderPlatformName](Engine.md#shaderplatformname)
- [snapshotRendering](Engine.md#snapshotrendering)
- [snapshotRenderingMode](Engine.md#snapshotrenderingmode)
- [stencilState](Engine.md#stencilstate)
- [stencilStateComposer](Engine.md#stencilstatecomposer)
- [supportsUniformBuffers](Engine.md#supportsuniformbuffers)
- [useExactSrgbConversions](Engine.md#useexactsrgbconversions)
- [useReverseDepthBuffer](Engine.md#usereversedepthbuffer)
- [version](Engine.md#version)
- [webGLVersion](Engine.md#webglversion)
- [HasMajorPerformanceCaveat](Engine.md#hasmajorperformancecaveat)
- [Instances](Engine.md#instances)
- [IsSupported](Engine.md#issupported)
- [IsSupportedAsync](Engine.md#issupportedasync)
- [LastCreatedEngine](Engine.md#lastcreatedengine)
- [LastCreatedScene](Engine.md#lastcreatedscene)
- [NpmPackage](Engine.md#npmpackage)
- [ShadersRepository](Engine.md#shadersrepository)
- [Version](Engine.md#version-1)

### Methods

- [\_clientWaitAsync](Engine.md#_clientwaitasync)
- [\_createDepthStencilCubeTexture](Engine.md#_createdepthstencilcubetexture)
- [\_createImageBitmapFromSource](Engine.md#_createimagebitmapfromsource)
- [\_createShaderProgram](Engine.md#_createshaderprogram)
- [\_createTextureBase](Engine.md#_createtexturebase)
- [\_deleteBuffer](Engine.md#_deletebuffer)
- [\_deletePipelineContext](Engine.md#_deletepipelinecontext)
- [\_deleteTexture](Engine.md#_deletetexture)
- [\_disableTouchAction](Engine.md#_disabletouchaction)
- [\_finalizePipelineContext](Engine.md#_finalizepipelinecontext)
- [\_initFeatures](Engine.md#_initfeatures)
- [\_initGLContext](Engine.md#_initglcontext)
- [\_measureFps](Engine.md#_measurefps)
- [\_normalizeIndexData](Engine.md#_normalizeindexdata)
- [\_prepareWebGLTextureContinuation](Engine.md#_preparewebgltexturecontinuation)
- [\_rebuildBuffers](Engine.md#_rebuildbuffers)
- [\_renderLoop](Engine.md#_renderloop)
- [\_resetIndexBufferBinding](Engine.md#_resetindexbufferbinding)
- [\_restoreEngineAfterContextLost](Engine.md#_restoreengineaftercontextlost)
- [\_setProgram](Engine.md#_setprogram)
- [\_setTexture](Engine.md#_settexture)
- [\_sharedInit](Engine.md#_sharedinit)
- [applyStates](Engine.md#applystates)
- [areAllComputeEffectsReady](Engine.md#areallcomputeeffectsready)
- [areAllEffectsReady](Engine.md#arealleffectsready)
- [attachContextLostEvent](Engine.md#attachcontextlostevent)
- [attachContextRestoredEvent](Engine.md#attachcontextrestoredevent)
- [beginFrame](Engine.md#beginframe)
- [beginOcclusionQuery](Engine.md#beginocclusionquery)
- [beginTransformFeedback](Engine.md#begintransformfeedback)
- [bindArrayBuffer](Engine.md#bindarraybuffer)
- [bindAttachments](Engine.md#bindattachments)
- [bindBuffers](Engine.md#bindbuffers)
- [bindBuffersDirectly](Engine.md#bindbuffersdirectly)
- [bindFramebuffer](Engine.md#bindframebuffer)
- [bindIndexBuffer](Engine.md#bindindexbuffer)
- [bindInstancesBuffer](Engine.md#bindinstancesbuffer)
- [bindMultiviewFramebuffer](Engine.md#bindmultiviewframebuffer)
- [bindSamplers](Engine.md#bindsamplers)
- [bindTransformFeedback](Engine.md#bindtransformfeedback)
- [bindTransformFeedbackBuffer](Engine.md#bindtransformfeedbackbuffer)
- [bindUniformBlock](Engine.md#binduniformblock)
- [bindUniformBuffer](Engine.md#binduniformbuffer)
- [bindUniformBufferBase](Engine.md#binduniformbufferbase)
- [bindVertexArrayObject](Engine.md#bindvertexarrayobject)
- [buildTextureLayout](Engine.md#buildtexturelayout)
- [cacheStencilState](Engine.md#cachestencilstate)
- [captureGPUFrameTime](Engine.md#capturegpuframetime)
- [clear](Engine.md#clear)
- [clearInternalTexturesCache](Engine.md#clearinternaltexturescache)
- [computeDispatch](Engine.md#computedispatch)
- [createCanvas](Engine.md#createcanvas)
- [createCanvasImage](Engine.md#createcanvasimage)
- [createComputeContext](Engine.md#createcomputecontext)
- [createComputeEffect](Engine.md#createcomputeeffect)
- [createComputePipelineContext](Engine.md#createcomputepipelinecontext)
- [createCubeTexture](Engine.md#createcubetexture)
- [createDepthStencilTexture](Engine.md#createdepthstenciltexture)
- [createDrawContext](Engine.md#createdrawcontext)
- [createDynamicTexture](Engine.md#createdynamictexture)
- [createDynamicUniformBuffer](Engine.md#createdynamicuniformbuffer)
- [createDynamicVertexBuffer](Engine.md#createdynamicvertexbuffer)
- [createEffect](Engine.md#createeffect)
- [createEffectForParticles](Engine.md#createeffectforparticles)
- [createExternalTexture](Engine.md#createexternaltexture)
- [createImageBitmap](Engine.md#createimagebitmap)
- [createIndexBuffer](Engine.md#createindexbuffer)
- [createInstancesBuffer](Engine.md#createinstancesbuffer)
- [createMaterialContext](Engine.md#creatematerialcontext)
- [createMultipleRenderTarget](Engine.md#createmultiplerendertarget)
- [createMultiviewRenderTargetTexture](Engine.md#createmultiviewrendertargettexture)
- [createPipelineContext](Engine.md#createpipelinecontext)
- [createPrefilteredCubeTexture](Engine.md#createprefilteredcubetexture)
- [createQuery](Engine.md#createquery)
- [createRawCubeTexture](Engine.md#createrawcubetexture)
- [createRawCubeTextureFromUrl](Engine.md#createrawcubetexturefromurl)
- [createRawShaderProgram](Engine.md#createrawshaderprogram)
- [createRawTexture](Engine.md#createrawtexture)
- [createRawTexture2DArray](Engine.md#createrawtexture2darray)
- [createRawTexture3D](Engine.md#createrawtexture3d)
- [createRenderPassId](Engine.md#createrenderpassid)
- [createRenderTargetCubeTexture](Engine.md#createrendertargetcubetexture)
- [createRenderTargetTexture](Engine.md#createrendertargettexture)
- [createShaderProgram](Engine.md#createshaderprogram)
- [createStorageBuffer](Engine.md#createstoragebuffer)
- [createTexture](Engine.md#createtexture)
- [createTransformFeedback](Engine.md#createtransformfeedback)
- [createUniformBuffer](Engine.md#createuniformbuffer)
- [createVertexBuffer](Engine.md#createvertexbuffer)
- [createVideoElement](Engine.md#createvideoelement)
- [deleteInstancesBuffer](Engine.md#deleteinstancesbuffer)
- [deleteQuery](Engine.md#deletequery)
- [deleteTransformFeedback](Engine.md#deletetransformfeedback)
- [disableAttributeByIndex](Engine.md#disableattributebyindex)
- [disableInstanceAttribute](Engine.md#disableinstanceattribute)
- [disableInstanceAttributeByName](Engine.md#disableinstanceattributebyname)
- [disableScissor](Engine.md#disablescissor)
- [disableVR](Engine.md#disablevr)
- [displayLoadingUI](Engine.md#displayloadingui)
- [dispose](Engine.md#dispose)
- [draw](Engine.md#draw)
- [drawArraysType](Engine.md#drawarraystype)
- [drawElementsType](Engine.md#drawelementstype)
- [drawPointClouds](Engine.md#drawpointclouds)
- [drawUnIndexed](Engine.md#drawunindexed)
- [enableEffect](Engine.md#enableeffect)
- [enableScissor](Engine.md#enablescissor)
- [enableVR](Engine.md#enablevr)
- [endFrame](Engine.md#endframe)
- [endOcclusionQuery](Engine.md#endocclusionquery)
- [endTimeQuery](Engine.md#endtimequery)
- [endTransformFeedback](Engine.md#endtransformfeedback)
- [enterFullscreen](Engine.md#enterfullscreen)
- [enterPointerlock](Engine.md#enterpointerlock)
- [exitFullscreen](Engine.md#exitfullscreen)
- [exitPointerlock](Engine.md#exitpointerlock)
- [flushFramebuffer](Engine.md#flushframebuffer)
- [generateMipMapsForCubemap](Engine.md#generatemipmapsforcubemap)
- [generateMipmaps](Engine.md#generatemipmaps)
- [getAlphaEquation](Engine.md#getalphaequation)
- [getAlphaMode](Engine.md#getalphamode)
- [getAspectRatio](Engine.md#getaspectratio)
- [getAttributes](Engine.md#getattributes)
- [getAudioContext](Engine.md#getaudiocontext)
- [getAudioDestination](Engine.md#getaudiodestination)
- [getCaps](Engine.md#getcaps)
- [getClassName](Engine.md#getclassname)
- [getColorWrite](Engine.md#getcolorwrite)
- [getCreationOptions](Engine.md#getcreationoptions)
- [getCurrentRenderPassName](Engine.md#getcurrentrenderpassname)
- [getDeltaTime](Engine.md#getdeltatime)
- [getDepthBuffer](Engine.md#getdepthbuffer)
- [getDepthFunction](Engine.md#getdepthfunction)
- [getDepthWrite](Engine.md#getdepthwrite)
- [getError](Engine.md#geterror)
- [getFontOffset](Engine.md#getfontoffset)
- [getFps](Engine.md#getfps)
- [getFragmentShaderSource](Engine.md#getfragmentshadersource)
- [getGPUFrameTimeCounter](Engine.md#getgpuframetimecounter)
- [getGlInfo](Engine.md#getglinfo)
- [getHardwareScalingLevel](Engine.md#gethardwarescalinglevel)
- [getHostDocument](Engine.md#gethostdocument)
- [getHostWindow](Engine.md#gethostwindow)
- [getInfo](Engine.md#getinfo)
- [getInputElement](Engine.md#getinputelement)
- [getInputElementClientRect](Engine.md#getinputelementclientrect)
- [getLoadedTexturesCache](Engine.md#getloadedtexturescache)
- [getLockstepMaxSteps](Engine.md#getlockstepmaxsteps)
- [getQueryResult](Engine.md#getqueryresult)
- [getRenderHeight](Engine.md#getrenderheight)
- [getRenderPassNames](Engine.md#getrenderpassnames)
- [getRenderWidth](Engine.md#getrenderwidth)
- [getRenderingCanvas](Engine.md#getrenderingcanvas)
- [getRenderingCanvasClientRect](Engine.md#getrenderingcanvasclientrect)
- [getScreenAspectRatio](Engine.md#getscreenaspectratio)
- [getStencilBuffer](Engine.md#getstencilbuffer)
- [getStencilFunction](Engine.md#getstencilfunction)
- [getStencilFunctionMask](Engine.md#getstencilfunctionmask)
- [getStencilFunctionReference](Engine.md#getstencilfunctionreference)
- [getStencilMask](Engine.md#getstencilmask)
- [getStencilOperationDepthFail](Engine.md#getstenciloperationdepthfail)
- [getStencilOperationFail](Engine.md#getstenciloperationfail)
- [getStencilOperationPass](Engine.md#getstenciloperationpass)
- [getTimeStep](Engine.md#gettimestep)
- [getUniforms](Engine.md#getuniforms)
- [getVRDevice](Engine.md#getvrdevice)
- [getVertexShaderSource](Engine.md#getvertexshadersource)
- [getZOffset](Engine.md#getzoffset)
- [getZOffsetUnits](Engine.md#getzoffsetunits)
- [hideLoadingUI](Engine.md#hideloadingui)
- [initWebVR](Engine.md#initwebvr)
- [initWebVRAsync](Engine.md#initwebvrasync)
- [inlineShaderCode](Engine.md#inlineshadercode)
- [isDeterministicLockStep](Engine.md#isdeterministiclockstep)
- [isQueryResultAvailable](Engine.md#isqueryresultavailable)
- [isVRDevicePresent](Engine.md#isvrdevicepresent)
- [isVRPresenting](Engine.md#isvrpresenting)
- [readFromStorageBuffer](Engine.md#readfromstoragebuffer)
- [readPixels](Engine.md#readpixels)
- [recordVertexArrayObject](Engine.md#recordvertexarrayobject)
- [registerView](Engine.md#registerview)
- [releaseComputeEffects](Engine.md#releasecomputeeffects)
- [releaseEffects](Engine.md#releaseeffects)
- [releaseRenderPassId](Engine.md#releaserenderpassid)
- [releaseVertexArrayObject](Engine.md#releasevertexarrayobject)
- [resetTextureCache](Engine.md#resettexturecache)
- [resize](Engine.md#resize)
- [resizeImageBitmap](Engine.md#resizeimagebitmap)
- [restoreDefaultFramebuffer](Engine.md#restoredefaultframebuffer)
- [restoreSingleAttachment](Engine.md#restoresingleattachment)
- [restoreSingleAttachmentForRenderTarget](Engine.md#restoresingleattachmentforrendertarget)
- [restoreStencilState](Engine.md#restorestencilstate)
- [runRenderLoop](Engine.md#runrenderloop)
- [scissorClear](Engine.md#scissorclear)
- [setAlphaConstants](Engine.md#setalphaconstants)
- [setAlphaEquation](Engine.md#setalphaequation)
- [setAlphaMode](Engine.md#setalphamode)
- [setArray](Engine.md#setarray)
- [setArray2](Engine.md#setarray2)
- [setArray3](Engine.md#setarray3)
- [setArray4](Engine.md#setarray4)
- [setColorWrite](Engine.md#setcolorwrite)
- [setCompressedTextureExclusions](Engine.md#setcompressedtextureexclusions)
- [setDepthBuffer](Engine.md#setdepthbuffer)
- [setDepthFunction](Engine.md#setdepthfunction)
- [setDepthFunctionToGreater](Engine.md#setdepthfunctiontogreater)
- [setDepthFunctionToGreaterOrEqual](Engine.md#setdepthfunctiontogreaterorequal)
- [setDepthFunctionToLess](Engine.md#setdepthfunctiontoless)
- [setDepthFunctionToLessOrEqual](Engine.md#setdepthfunctiontolessorequal)
- [setDepthStencilTexture](Engine.md#setdepthstenciltexture)
- [setDepthWrite](Engine.md#setdepthwrite)
- [setDirectViewport](Engine.md#setdirectviewport)
- [setDitheringState](Engine.md#setditheringstate)
- [setExternalTexture](Engine.md#setexternaltexture)
- [setFloat](Engine.md#setfloat)
- [setFloat2](Engine.md#setfloat2)
- [setFloat3](Engine.md#setfloat3)
- [setFloat4](Engine.md#setfloat4)
- [setHardwareScalingLevel](Engine.md#sethardwarescalinglevel)
- [setInt](Engine.md#setint)
- [setInt2](Engine.md#setint2)
- [setInt3](Engine.md#setint3)
- [setInt4](Engine.md#setint4)
- [setIntArray](Engine.md#setintarray)
- [setIntArray2](Engine.md#setintarray2)
- [setIntArray3](Engine.md#setintarray3)
- [setIntArray4](Engine.md#setintarray4)
- [setMatrices](Engine.md#setmatrices)
- [setMatrix2x2](Engine.md#setmatrix2x2)
- [setMatrix3x3](Engine.md#setmatrix3x3)
- [setRasterizerState](Engine.md#setrasterizerstate)
- [setSize](Engine.md#setsize)
- [setState](Engine.md#setstate)
- [setStencilBuffer](Engine.md#setstencilbuffer)
- [setStencilFunction](Engine.md#setstencilfunction)
- [setStencilFunctionMask](Engine.md#setstencilfunctionmask)
- [setStencilFunctionReference](Engine.md#setstencilfunctionreference)
- [setStencilMask](Engine.md#setstencilmask)
- [setStencilOperationDepthFail](Engine.md#setstenciloperationdepthfail)
- [setStencilOperationFail](Engine.md#setstenciloperationfail)
- [setStencilOperationPass](Engine.md#setstenciloperationpass)
- [setStorageBuffer](Engine.md#setstoragebuffer)
- [setTexture](Engine.md#settexture)
- [setTextureArray](Engine.md#settexturearray)
- [setTextureFormatToUse](Engine.md#settextureformattouse)
- [setTextureFromPostProcess](Engine.md#settexturefrompostprocess)
- [setTextureFromPostProcessOutput](Engine.md#settexturefrompostprocessoutput)
- [setTextureSampler](Engine.md#settexturesampler)
- [setTranformFeedbackVaryings](Engine.md#settranformfeedbackvaryings)
- [setViewport](Engine.md#setviewport)
- [setZOffset](Engine.md#setzoffset)
- [setZOffsetUnits](Engine.md#setzoffsetunits)
- [snapshotRenderingReset](Engine.md#snapshotrenderingreset)
- [startTimeQuery](Engine.md#starttimequery)
- [stopRenderLoop](Engine.md#stoprenderloop)
- [switchFullscreen](Engine.md#switchfullscreen)
- [unBindFramebuffer](Engine.md#unbindframebuffer)
- [unBindMultiColorAttachmentFramebuffer](Engine.md#unbindmulticolorattachmentframebuffer)
- [unRegisterView](Engine.md#unregisterview)
- [unbindAllAttributes](Engine.md#unbindallattributes)
- [unbindAllTextures](Engine.md#unbindalltextures)
- [unbindInstanceAttributes](Engine.md#unbindinstanceattributes)
- [updateAndBindInstancesBuffer](Engine.md#updateandbindinstancesbuffer)
- [updateArrayBuffer](Engine.md#updatearraybuffer)
- [updateDynamicIndexBuffer](Engine.md#updatedynamicindexbuffer)
- [updateDynamicTexture](Engine.md#updatedynamictexture)
- [updateDynamicVertexBuffer](Engine.md#updatedynamicvertexbuffer)
- [updateMultipleRenderTargetTextureSampleCount](Engine.md#updatemultiplerendertargettexturesamplecount)
- [updateRawCubeTexture](Engine.md#updaterawcubetexture)
- [updateRawTexture](Engine.md#updaterawtexture)
- [updateRawTexture2DArray](Engine.md#updaterawtexture2darray)
- [updateRawTexture3D](Engine.md#updaterawtexture3d)
- [updateRenderTargetTextureSampleCount](Engine.md#updaterendertargettexturesamplecount)
- [updateStorageBuffer](Engine.md#updatestoragebuffer)
- [updateTextureComparisonFunction](Engine.md#updatetexturecomparisonfunction)
- [updateTextureData](Engine.md#updatetexturedata)
- [updateTextureDimensions](Engine.md#updatetexturedimensions)
- [updateTextureSamplingMode](Engine.md#updatetexturesamplingmode)
- [updateTextureWrappingMode](Engine.md#updatetexturewrappingmode)
- [updateUniformBuffer](Engine.md#updateuniformbuffer)
- [updateVideoTexture](Engine.md#updatevideotexture)
- [wipeCaches](Engine.md#wipecaches)
- [wrapWebGLTexture](Engine.md#wrapwebgltexture)
- [CeilingPOT](Engine.md#ceilingpot)
- [DefaultLoadingScreenFactory](Engine.md#defaultloadingscreenfactory)
- [FloorPOT](Engine.md#floorpot)
- [GetExponentOfTwo](Engine.md#getexponentoftwo)
- [MarkAllMaterialsAsDirty](Engine.md#markallmaterialsasdirty)
- [NearestPOT](Engine.md#nearestpot)
- [QueueNewFrame](Engine.md#queuenewframe)
- [\_ConcatenateShader](Engine.md#_concatenateshader)
- [\_ExitFullscreen](Engine.md#_exitfullscreen)
- [\_ExitPointerlock](Engine.md#_exitpointerlock)
- [\_RequestFullscreen](Engine.md#_requestfullscreen)
- [\_RequestPointerlock](Engine.md#_requestpointerlock)
- [isSupported](Engine.md#issupported-1)

## Constructors

### constructor

• **new Engine**(`canvasOrContext`, `antialias?`, `options?`, `adaptToDeviceRatio?`)

Creates a new engine

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `canvasOrContext` | [`Nullable`](../modules.md#nullable)`HTMLCanvasElement` \| `WebGLRenderingContext` \| `OffscreenCanvas` \| `WebGL2RenderingContext` | `undefined` | defines the canvas or WebGL context to use for rendering. If you provide a WebGL context, Babylon.js will not hook events on the canvas (like pointers, keyboards, etc...) so no event observables will be available. This is mostly used when Babylon.js is used as a plugin on a system which already used the WebGL context |
| `antialias?` | `boolean` | `undefined` | defines enable antialiasing (default: false) |
| `options?` | [`EngineOptions`](../interfaces/EngineOptions.md) | `undefined` | defines further options to be sent to the getContext() function |
| `adaptToDeviceRatio` | `boolean` | `false` | defines whether to adapt to the device's viewport characteristics (default: false) |

#### Overrides

[ThinEngine](ThinEngine.md).[constructor](ThinEngine.md#constructor)

#### Defined in

packages/dev/core/src/Engines/engine.ts:578

## Properties

### \_activeRenderLoops

• `Protected` **\_activeRenderLoops**: () => `void`[]

#### Inherited from

[ThinEngine](ThinEngine.md).[_activeRenderLoops](ThinEngine.md#_activerenderloops)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:424

___

### \_audioContext

• `Protected` **\_audioContext**: [`Nullable`](../modules.md#nullable)`AudioContext`

#### Inherited from

[ThinEngine](ThinEngine.md).[_audioContext](ThinEngine.md#_audiocontext)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:377

___

### \_audioDestination

• `Protected` **\_audioDestination**: [`Nullable`](../modules.md#nullable)`AudioDestinationNode` \| `MediaStreamAudioDestinationNode`

#### Inherited from

[ThinEngine](ThinEngine.md).[_audioDestination](ThinEngine.md#_audiodestination)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:378

___

### \_boundUniforms

• `Protected` **\_boundUniforms**: `Object` = `{}`

#### Index signature

▪ [key: `number`]: `WebGLUniformLocation`

#### Inherited from

[ThinEngine](ThinEngine.md).[_boundUniforms](ThinEngine.md#_bounduniforms)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:4916

___

### \_cachedStencilBuffer

• `Private` **\_cachedStencilBuffer**: `boolean`

#### Defined in

packages/dev/core/src/Engines/engine.ts:1029

___

### \_cachedStencilFunction

• `Private` **\_cachedStencilFunction**: `number`

#### Defined in

packages/dev/core/src/Engines/engine.ts:1030

___

### \_cachedStencilMask

• `Private` **\_cachedStencilMask**: `number`

#### Defined in

packages/dev/core/src/Engines/engine.ts:1031

___

### \_cachedStencilOperationDepthFail

• `Private` **\_cachedStencilOperationDepthFail**: `number`

#### Defined in

packages/dev/core/src/Engines/engine.ts:1034

___

### \_cachedStencilOperationFail

• `Private` **\_cachedStencilOperationFail**: `number`

#### Defined in

packages/dev/core/src/Engines/engine.ts:1033

___

### \_cachedStencilOperationPass

• `Private` **\_cachedStencilOperationPass**: `number`

#### Defined in

packages/dev/core/src/Engines/engine.ts:1032

___

### \_cachedStencilReference

• `Private` **\_cachedStencilReference**: `number`

#### Defined in

packages/dev/core/src/Engines/engine.ts:1035

___

### \_compatibilityMode

• `Protected` **\_compatibilityMode**: `boolean` = `true`

#### Defined in

packages/dev/core/src/Engines/engine.ts:545

___

### \_compiledEffects

• `Protected` **\_compiledEffects**: `Object` = `{}`

#### Index signature

▪ [key: `string`]: [`Effect`](Effect.md)

#### Inherited from

[ThinEngine](ThinEngine.md).[_compiledEffects](ThinEngine.md#_compiledeffects)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:502

___

### \_contextWasLost

• `Protected` **\_contextWasLost**: `boolean` = `false`

#### Inherited from

[ThinEngine](ThinEngine.md).[_contextWasLost](ThinEngine.md#_contextwaslost)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:445

___

### \_creationOptions

• `Protected` **\_creationOptions**: [`EngineOptions`](../interfaces/EngineOptions.md)

#### Inherited from

[ThinEngine](ThinEngine.md).[_creationOptions](ThinEngine.md#_creationoptions)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:376

___

### \_currentBoundBuffer

• `Protected` **\_currentBoundBuffer**: [`Nullable`](../modules.md#nullable)`WebGLBuffer`[]

#### Inherited from

[ThinEngine](ThinEngine.md).[_currentBoundBuffer](ThinEngine.md#_currentboundbuffer)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:517

___

### \_currentEffect

• `Protected` **\_currentEffect**: [`Nullable`](../modules.md#nullable)[`Effect`](Effect.md)

#### Inherited from

[ThinEngine](ThinEngine.md).[_currentEffect](ThinEngine.md#_currenteffect)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:495

___

### \_deltaTime

• `Private` **\_deltaTime**: `number` = `0`

#### Defined in

packages/dev/core/src/Engines/engine.ts:512

___

### \_deterministicLockstep

• `Protected` **\_deterministicLockstep**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Engines/engine.ts:502

___

### \_fps

• `Private` **\_fps**: `number` = `60`

#### Defined in

packages/dev/core/src/Engines/engine.ts:511

___

### \_highPrecisionShadersAllowed

• `Protected` **\_highPrecisionShadersAllowed**: `boolean` = `true`

#### Inherited from

[ThinEngine](ThinEngine.md).[_highPrecisionShadersAllowed](ThinEngine.md#_highprecisionshadersallowed)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:388

___

### \_isStencilEnable

• `Protected` **\_isStencilEnable**: `boolean`

#### Inherited from

[ThinEngine](ThinEngine.md).[_isStencilEnable](ThinEngine.md#_isstencilenable)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:414

___

### \_loadingScreen

• `Private` **\_loadingScreen**: [`ILoadingScreen`](../interfaces/ILoadingScreen.md)

#### Defined in

packages/dev/core/src/Engines/engine.ts:497

___

### \_lockstepMaxSteps

• `Protected` **\_lockstepMaxSteps**: `number` = `4`

#### Defined in

packages/dev/core/src/Engines/engine.ts:503

___

### \_onBlur

• `Private` **\_onBlur**: () => `void`

#### Type declaration

▸ (): `void`

##### Returns

`void`

#### Defined in

packages/dev/core/src/Engines/engine.ts:536

___

### \_onCanvasBlur

• `Private` **\_onCanvasBlur**: () => `void`

#### Type declaration

▸ (): `void`

##### Returns

`void`

#### Defined in

packages/dev/core/src/Engines/engine.ts:538

___

### \_onCanvasContextMenu

• `Private` **\_onCanvasContextMenu**: (`evt`: `Event`) => `void`

#### Type declaration

▸ (`evt`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `evt` | `Event` |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Engines/engine.ts:540

___

### \_onCanvasFocus

• `Private` **\_onCanvasFocus**: () => `void`

#### Type declaration

▸ (): `void`

##### Returns

`void`

#### Defined in

packages/dev/core/src/Engines/engine.ts:539

___

### \_onCanvasPointerOut

• `Private` **\_onCanvasPointerOut**: (`event`: `PointerEvent`) => `void`

#### Type declaration

▸ (`event`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `event` | `PointerEvent` |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Engines/engine.ts:537

___

### \_onFocus

• `Private` **\_onFocus**: () => `void`

#### Type declaration

▸ (): `void`

##### Returns

`void`

#### Defined in

packages/dev/core/src/Engines/engine.ts:535

___

### \_onFullscreenChange

• `Private` **\_onFullscreenChange**: () => `void`

#### Type declaration

▸ (): `void`

##### Returns

`void`

#### Defined in

packages/dev/core/src/Engines/engine.ts:542

___

### \_onPointerLockChange

• `Private` **\_onPointerLockChange**: () => `void`

#### Type declaration

▸ (): `void`

##### Returns

`void`

#### Defined in

packages/dev/core/src/Engines/engine.ts:543

___

### \_performanceMonitor

• `Private` **\_performanceMonitor**: [`PerformanceMonitor`](PerformanceMonitor.md)

#### Defined in

packages/dev/core/src/Engines/engine.ts:525

___

### \_pointerLockRequested

• `Private` **\_pointerLockRequested**: `boolean`

#### Defined in

packages/dev/core/src/Engines/engine.ts:498

___

### \_renderPassNames

• `Private` **\_renderPassNames**: `string`[]

#### Defined in

packages/dev/core/src/Engines/engine.ts:1582

___

### \_renderingCanvas

• `Protected` **\_renderingCanvas**: [`Nullable`](../modules.md#nullable)`HTMLCanvasElement`

#### Inherited from

[ThinEngine](ThinEngine.md).[_renderingCanvas](ThinEngine.md#_renderingcanvas)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:374

___

### \_renderingQueueLaunched

• `Protected` **\_renderingQueueLaunched**: `boolean` = `false`

#### Inherited from

[ThinEngine](ThinEngine.md).[_renderingQueueLaunched](ThinEngine.md#_renderingqueuelaunched)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:423

___

### \_rescalePostProcess

• `Private` **\_rescalePostProcess**: [`PostProcess`](PostProcess.md)

#### Defined in

packages/dev/core/src/Engines/engine.ts:499

___

### \_shaderProcessor

• `Protected` **\_shaderProcessor**: [`Nullable`](../modules.md#nullable)`IShaderProcessor`

#### Inherited from

[ThinEngine](ThinEngine.md).[_shaderProcessor](ThinEngine.md#_shaderprocessor)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:265

___

### \_snapshotRenderingMode

• `Protected` **\_snapshotRenderingMode**: `number` = `Constants.SNAPSHOTRENDERING_STANDARD`

#### Inherited from

[ThinEngine](ThinEngine.md).[_snapshotRenderingMode](ThinEngine.md#_snapshotrenderingmode)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:694

___

### \_timeStep

• `Protected` **\_timeStep**: `number`

#### Defined in

packages/dev/core/src/Engines/engine.ts:504

___

### \_useExactSrgbConversions

• `Protected` **\_useExactSrgbConversions**: `boolean` = `false`

#### Inherited from

[ThinEngine](ThinEngine.md).[_useExactSrgbConversions](ThinEngine.md#_useexactsrgbconversions)

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

[ThinEngine](ThinEngine.md).[_viewportCached](ThinEngine.md#_viewportcached)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1692

___

### \_windowIsBackground

• `Protected` **\_windowIsBackground**: `boolean` = `false`

#### Inherited from

[ThinEngine](ThinEngine.md).[_windowIsBackground](ThinEngine.md#_windowisbackground)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:375

___

### activeView

• **activeView**: [`Nullable`](../modules.md#nullable)[`EngineView`](EngineView.md)

Gets the current engine view

**`See`**

https://doc.babylonjs.com/how_to/multi_canvases

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.views.ts:43

___

### adaptToDeviceRatio

• **adaptToDeviceRatio**: `boolean` = `false`

If set to true zooming in and out in the browser will rescale the hardware-scaling correctly.

#### Inherited from

[ThinEngine](ThinEngine.md).[adaptToDeviceRatio](ThinEngine.md#adapttodeviceratio)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:555

___

### canvasTabIndex

• **canvasTabIndex**: `number` = `1`

Gets or sets the tab index to set to the rendering canvas. 1 is the minimum value to set to be able to capture keyboard events

#### Defined in

packages/dev/core/src/Engines/engine.ts:518

___

### cullBackFaces

• **cullBackFaces**: [`Nullable`](../modules.md#nullable)`boolean` = `null`

Gets or sets a boolean indicating if back faces must be culled. If false, front faces are culled instead (true by default)
If non null, this takes precedence over the value from the material

#### Inherited from

[ThinEngine](ThinEngine.md).[cullBackFaces](ThinEngine.md#cullbackfaces)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:289

___

### currentRenderPassId

• **currentRenderPassId**: `number` = `Constants.RENDERPASS_MAIN`

Gets or sets the current render pass id

#### Defined in

packages/dev/core/src/Engines/engine.ts:1580

___

### customAnimationFrameRequester

• **customAnimationFrameRequester**: [`Nullable`](../modules.md#nullable)[`ICustomAnimationFrameRequester`](../interfaces/ICustomAnimationFrameRequester.md) = `null`

If set, will be used to request the next animation frame for the render loop

#### Defined in

packages/dev/core/src/Engines/engine.ts:456

___

### disableContextMenu

• **disableContextMenu**: `boolean` = `true`

Gets or sets a boolean to enable/disable the context menu (right-click) from appearing on the main canvas

#### Defined in

packages/dev/core/src/Engines/engine.ts:401

___

### disableManifestCheck

• **disableManifestCheck**: `boolean` = `false`

Gets or sets a boolean to enable/disable checking manifest if IndexedDB support is enabled (js will always consider the database is up to date)

#### Defined in

packages/dev/core/src/Engines/engine.ts:396

___

### disablePerformanceMonitorInBackground

• **disablePerformanceMonitorInBackground**: `boolean` = `false`

Turn this value on if you want to pause FPS computation when in background

#### Defined in

packages/dev/core/src/Engines/engine.ts:523

___

### disableUniformBuffers

• **disableUniformBuffers**: `boolean` = `false`

Gets or sets a boolean indicating that uniform buffers must be disabled even if they are supported

#### Inherited from

[ThinEngine](ThinEngine.md).[disableUniformBuffers](ThinEngine.md#disableuniformbuffers)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:340

___

### disableVertexArrayObjects

• **disableVertexArrayObjects**: `boolean` = `false`

Gets or sets a boolean indicating that vertex array object must be disabled even if they are supported

#### Inherited from

[ThinEngine](ThinEngine.md).[disableVertexArrayObjects](ThinEngine.md#disablevertexarrayobjects)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:465

___

### enableOfflineSupport

• **enableOfflineSupport**: `boolean` = `false`

Gets or sets a boolean to enable/disable IndexedDB support and avoid XHR on .manifest

#### Defined in

packages/dev/core/src/Engines/engine.ts:391

___

### enableUnpackFlipYCached

• **enableUnpackFlipYCached**: `boolean` = `true`

In case you are sharing the context with other applications, it might
be interested to not cache the unpack flip y state to ensure a consistent
value would be set.

#### Inherited from

[ThinEngine](ThinEngine.md).[enableUnpackFlipYCached](ThinEngine.md#enableunpackflipycached)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:4369

___

### forcePOTTextures

• **forcePOTTextures**: `boolean` = `false`

Gets or sets a boolean that indicates if textures must be forced to power of 2 size even if not required

#### Inherited from

[ThinEngine](ThinEngine.md).[forcePOTTextures](ThinEngine.md#forcepottextures)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:278

___

### hasOriginBottomLeft

• `Readonly` **hasOriginBottomLeft**: ``true``

Indicates that the origin of the texture/framebuffer space is the bottom left corner. If false, the origin is top left

#### Inherited from

[ThinEngine](ThinEngine.md).[hasOriginBottomLeft](ThinEngine.md#hasoriginbottomleft)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:335

___

### hostInformation

• **hostInformation**: [`HostInformation`](../interfaces/HostInformation.md)

Gets information about the current host

#### Inherited from

[ThinEngine](ThinEngine.md).[hostInformation](ThinEngine.md#hostinformation)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:565

___

### inputElement

• **inputElement**: [`Nullable`](../modules.md#nullable)`HTMLElement`

Gets or sets the  HTML element to use for attaching events

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.views.ts:31

___

### isFullscreen

• **isFullscreen**: `boolean` = `false`

Gets a boolean indicating if the engine is currently rendering in fullscreen mode

#### Inherited from

[ThinEngine](ThinEngine.md).[isFullscreen](ThinEngine.md#isfullscreen)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:283

___

### isInVRExclusivePointerMode

• **isInVRExclusivePointerMode**: `boolean`

Gets a boolean indicating that the engine is currently in VR exclusive mode for the pointers

**`See`**

https://docs.microsoft.com/en-us/microsoft-edge/webvr/essentials#mouse-input

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.webVR.ts:68

___

### isNDCHalfZRange

• `Readonly` **isNDCHalfZRange**: ``false``

Indicates if the z range in NDC space is 0..1 (value: true) or -1..1 (value: false)

#### Inherited from

[ThinEngine](ThinEngine.md).[isNDCHalfZRange](ThinEngine.md#isndchalfzrange)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:330

___

### isPointerLock

• **isPointerLock**: `boolean` = `false`

Gets a boolean indicating if the pointer is currently locked

#### Defined in

packages/dev/core/src/Engines/engine.ts:424

___

### onAfterShaderCompilationObservable

• **onAfterShaderCompilationObservable**: [`Observable`](Observable.md)[`Engine`](Engine.md)

Observable raised when the engine has just compiled a shader

#### Defined in

packages/dev/core/src/Engines/engine.ts:471

___

### onBeforeShaderCompilationObservable

• **onBeforeShaderCompilationObservable**: [`Observable`](Observable.md)[`Engine`](Engine.md)

Observable raised when the engine is about to compile a shader

#### Defined in

packages/dev/core/src/Engines/engine.ts:466

___

### onBeforeTextureInitObservable

• **onBeforeTextureInitObservable**: [`Observable`](Observable.md)[`Texture`](Texture.md)

Observable event triggered before each texture is initialized

#### Inherited from

[ThinEngine](ThinEngine.md).[onBeforeTextureInitObservable](ThinEngine.md#onbeforetextureinitobservable)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:662

___

### onBeginFrameObservable

• **onBeginFrameObservable**: [`Observable`](Observable.md)[`Engine`](Engine.md)

Observable raised when the engine begins a new frame

#### Defined in

packages/dev/core/src/Engines/engine.ts:451

___

### onCanvasBlurObservable

• **onCanvasBlurObservable**: [`Observable`](Observable.md)[`Engine`](Engine.md)

Observable event triggered each time the canvas loses focus

#### Defined in

packages/dev/core/src/Engines/engine.ts:436

___

### onCanvasFocusObservable

• **onCanvasFocusObservable**: [`Observable`](Observable.md)[`Engine`](Engine.md)

Observable event triggered each time the canvas gains focus

#### Defined in

packages/dev/core/src/Engines/engine.ts:441

___

### onCanvasPointerOutObservable

• **onCanvasPointerOutObservable**: [`Observable`](Observable.md)`PointerEvent`

Observable event triggered each time the canvas receives pointerout event

#### Defined in

packages/dev/core/src/Engines/engine.ts:446

___

### onContextLostObservable

• **onContextLostObservable**: [`Observable`](Observable.md)[`ThinEngine`](ThinEngine.md)

Observable signaled when a context lost event is raised

#### Inherited from

[ThinEngine](ThinEngine.md).[onContextLostObservable](ThinEngine.md#oncontextlostobservable)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:438

___

### onContextRestoredObservable

• **onContextRestoredObservable**: [`Observable`](Observable.md)[`ThinEngine`](ThinEngine.md)

Observable signaled when a context restored event is raised

#### Inherited from

[ThinEngine](ThinEngine.md).[onContextRestoredObservable](ThinEngine.md#oncontextrestoredobservable)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:442

___

### onDisposeObservable

• `Readonly` **onDisposeObservable**: [`Observable`](Observable.md)[`ThinEngine`](ThinEngine.md)

An event triggered when the engine is disposed.

#### Inherited from

[ThinEngine](ThinEngine.md).[onDisposeObservable](ThinEngine.md#ondisposeobservable)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:345

___

### onEndFrameObservable

• **onEndFrameObservable**: [`Observable`](Observable.md)[`Engine`](Engine.md)

Observable raised when the engine ends the current frame

#### Defined in

packages/dev/core/src/Engines/engine.ts:461

___

### onNewSceneAddedObservable

• **onNewSceneAddedObservable**: [`Observable`](Observable.md)[`Scene`](Scene.md)

Event raised when a new scene is created

#### Defined in

packages/dev/core/src/Engines/engine.ts:414

___

### onResizeObservable

• **onResizeObservable**: [`Observable`](Observable.md)[`Engine`](Engine.md)

Observable event triggered each time the rendering canvas is resized

#### Defined in

packages/dev/core/src/Engines/engine.ts:431

___

### onVRDisplayChangedObservable

• **onVRDisplayChangedObservable**: [`Observable`](Observable.md)[`IDisplayChangedEventArgs`](../interfaces/IDisplayChangedEventArgs.md)

Observable signaled when VR display mode changes

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.webVR.ts:54

___

### onVRRequestPresentComplete

• **onVRRequestPresentComplete**: [`Observable`](Observable.md)`boolean`

Observable signaled when VR request present is complete

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.webVR.ts:58

___

### onVRRequestPresentStart

• **onVRRequestPresentStart**: [`Observable`](Observable.md)[`Engine`](Engine.md)

Observable signaled when VR request present starts

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.webVR.ts:62

___

### postProcesses

• **postProcesses**: [`PostProcess`](PostProcess.md)[]

Gets the list of created postprocesses

#### Defined in

packages/dev/core/src/Engines/engine.ts:419

___

### premultipliedAlpha

• **premultipliedAlpha**: `boolean` = `true`

Defines whether the engine has been created with the premultipliedAlpha option on or not.

#### Inherited from

[ThinEngine](ThinEngine.md).[premultipliedAlpha](ThinEngine.md#premultipliedalpha)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:657

___

### preventCacheWipeBetweenFrames

• **preventCacheWipeBetweenFrames**: `boolean` = `false`

Gets or sets a boolean indicating that cache can be kept between frames

#### Inherited from

[ThinEngine](ThinEngine.md).[preventCacheWipeBetweenFrames](ThinEngine.md#preventcachewipebetweenframes)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:299

___

### renderEvenInBackground

• **renderEvenInBackground**: `boolean` = `true`

Gets or sets a boolean indicating if the engine must keep rendering even if the window is not in foreground

#### Inherited from

[ThinEngine](ThinEngine.md).[renderEvenInBackground](ThinEngine.md#rendereveninbackground)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:294

___

### scenes

• **scenes**: [`Scene`](Scene.md)[]

Gets the list of created scenes

#### Defined in

packages/dev/core/src/Engines/engine.ts:406

___

### textureFormatInUse

• `Readonly` **textureFormatInUse**: [`Nullable`](../modules.md#nullable)`string`

Gets the texture format in use

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.textureSelector.ts:20

___

### texturesSupported

• `Readonly` **texturesSupported**: `string`[]

Gets the list of texture formats supported

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.textureSelector.ts:15

___

### validateShaderPrograms

• **validateShaderPrograms**: `boolean` = `false`

Gets or sets a boolean indicating if the engine should validate programs after compilation

#### Inherited from

[ThinEngine](ThinEngine.md).[validateShaderPrograms](ThinEngine.md#validateshaderprograms)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:302

___

### views

• **views**: [`EngineView`](EngineView.md)[]

Gets or sets the list of views

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.views.ts:46

___

### vrPresentationAttributes

• `Optional` **vrPresentationAttributes**: [`IVRPresentationAttributes`](../interfaces/IVRPresentationAttributes.md)

Gets or sets the presentation attributes used to configure VR rendering

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.webVR.ts:95

___

### ALPHA\_ADD

▪ `Static` `Readonly` **ALPHA\_ADD**: ``1``

Defines that alpha blending to SRC ALPHA * SRC + DEST

#### Defined in

packages/dev/core/src/Engines/engine.ts:63

___

### ALPHA\_COMBINE

▪ `Static` `Readonly` **ALPHA\_COMBINE**: ``2``

Defines that alpha blending to SRC ALPHA * SRC + (1 - SRC ALPHA) * DEST

#### Defined in

packages/dev/core/src/Engines/engine.ts:65

___

### ALPHA\_DISABLE

▪ `Static` `Readonly` **ALPHA\_DISABLE**: ``0``

Defines that alpha blending is disabled

#### Defined in

packages/dev/core/src/Engines/engine.ts:61

___

### ALPHA\_INTERPOLATE

▪ `Static` `Readonly` **ALPHA\_INTERPOLATE**: ``9``

Defines that alpha blending to CST * SRC + (1 - CST) * DEST

#### Defined in

packages/dev/core/src/Engines/engine.ts:82

___

### ALPHA\_MAXIMIZED

▪ `Static` `Readonly` **ALPHA\_MAXIMIZED**: ``5``

Defines that alpha blending to SRC ALPHA * SRC + (1 - SRC) * DEST

#### Defined in

packages/dev/core/src/Engines/engine.ts:71

___

### ALPHA\_MULTIPLY

▪ `Static` `Readonly` **ALPHA\_MULTIPLY**: ``4``

Defines that alpha blending to SRC * DEST

#### Defined in

packages/dev/core/src/Engines/engine.ts:69

___

### ALPHA\_ONEONE

▪ `Static` `Readonly` **ALPHA\_ONEONE**: ``6``

Defines that alpha blending to SRC + DEST

#### Defined in

packages/dev/core/src/Engines/engine.ts:73

___

### ALPHA\_PREMULTIPLIED

▪ `Static` `Readonly` **ALPHA\_PREMULTIPLIED**: ``7``

Defines that alpha blending to SRC + (1 - SRC ALPHA) * DEST

#### Defined in

packages/dev/core/src/Engines/engine.ts:75

___

### ALPHA\_PREMULTIPLIED\_PORTERDUFF

▪ `Static` `Readonly` **ALPHA\_PREMULTIPLIED\_PORTERDUFF**: ``8``

Defines that alpha blending to SRC + (1 - SRC ALPHA) * DEST
Alpha will be set to (1 - SRC ALPHA) * DEST ALPHA

#### Defined in

packages/dev/core/src/Engines/engine.ts:80

___

### ALPHA\_SCREENMODE

▪ `Static` `Readonly` **ALPHA\_SCREENMODE**: ``10``

Defines that alpha blending to SRC + (1 - SRC) * DEST
Alpha will be set to SRC ALPHA + (1 - SRC ALPHA) * DEST ALPHA

#### Defined in

packages/dev/core/src/Engines/engine.ts:87

___

### ALPHA\_SUBTRACT

▪ `Static` `Readonly` **ALPHA\_SUBTRACT**: ``3``

Defines that alpha blending to DEST - SRC * DEST

#### Defined in

packages/dev/core/src/Engines/engine.ts:67

___

### ALWAYS

▪ `Static` `Readonly` **ALWAYS**: ``519``

Passed to depthFunction or stencilFunction to specify depth or stencil tests will always pass. i.e. Pixels will be drawn in the order they are drawn

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

#### Defined in

packages/dev/core/src/Engines/engine.ts:485

___

### CollisionsEpsilon

▪ `Static` **CollisionsEpsilon**: `number` = `0.001`

Gets or sets the epsilon value used by collision engine

#### Inherited from

[ThinEngine](ThinEngine.md).[CollisionsEpsilon](ThinEngine.md#collisionsepsilon)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:253

___

### DECR

▪ `Static` `Readonly` **DECR**: ``7683``

Passed to stencilOperation to specify that stencil value must be decremented

#### Defined in

packages/dev/core/src/Engines/engine.ts:124

___

### DECR\_WRAP

▪ `Static` `Readonly` **DECR\_WRAP**: ``34056``

Passed to stencilOperation to specify that stencil value must be decremented with wrapping

#### Defined in

packages/dev/core/src/Engines/engine.ts:130

___

### DELAYLOADSTATE\_LOADED

▪ `Static` `Readonly` **DELAYLOADSTATE\_LOADED**: ``1``

Defines that the resource was successfully delay loaded

#### Defined in

packages/dev/core/src/Engines/engine.ts:92

___

### DELAYLOADSTATE\_LOADING

▪ `Static` `Readonly` **DELAYLOADSTATE\_LOADING**: ``2``

Defines that the resource is currently delay loading

#### Defined in

packages/dev/core/src/Engines/engine.ts:94

___

### DELAYLOADSTATE\_NONE

▪ `Static` `Readonly` **DELAYLOADSTATE\_NONE**: ``0``

Defines that the resource is not delayed

#### Defined in

packages/dev/core/src/Engines/engine.ts:90

___

### DELAYLOADSTATE\_NOTLOADED

▪ `Static` `Readonly` **DELAYLOADSTATE\_NOTLOADED**: ``4``

Defines that the resource is delayed and has not started loading

#### Defined in

packages/dev/core/src/Engines/engine.ts:96

___

### EQUAL

▪ `Static` `Readonly` **EQUAL**: ``514``

Passed to depthFunction or stencilFunction to specify depth or stencil tests will pass if the new depth value is equals to the stored value

#### Defined in

packages/dev/core/src/Engines/engine.ts:106

___

### ExceptionList

▪ `Static` **ExceptionList**: ({ `capture`: `string` = "63\\.0\\.3239\\.(\\d+)"; `captureConstraint`: `number` = 108; `key`: `string` = "Chrome/63.0"; `targets`: `string`[]  } \| { `capture`: ``null`` = null; `captureConstraint`: ``null`` = null; `key`: `string` = "Firefox/58"; `targets`: `string`[]  })[]

Use this array to turn off some WebGL2 features on known buggy browsers version

#### Inherited from

[ThinEngine](ThinEngine.md).[ExceptionList](ThinEngine.md#exceptionlist)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:180

___

### GEQUAL

▪ `Static` `Readonly` **GEQUAL**: ``518``

Passed to depthFunction or stencilFunction to specify depth or stencil tests will pass if the new depth value is greater than or equal to the stored value

#### Defined in

packages/dev/core/src/Engines/engine.ts:112

___

### GREATER

▪ `Static` `Readonly` **GREATER**: ``516``

Passed to depthFunction or stencilFunction to specify depth or stencil tests will pass if the new depth value is greater than the stored value

#### Defined in

packages/dev/core/src/Engines/engine.ts:110

___

### INCR

▪ `Static` `Readonly` **INCR**: ``7682``

Passed to stencilOperation to specify that stencil value must be incremented

#### Defined in

packages/dev/core/src/Engines/engine.ts:122

___

### INCR\_WRAP

▪ `Static` `Readonly` **INCR\_WRAP**: ``34055``

Passed to stencilOperation to specify that stencil value must be incremented with wrapping

#### Defined in

packages/dev/core/src/Engines/engine.ts:128

___

### INVERT

▪ `Static` `Readonly` **INVERT**: ``5386``

Passed to stencilOperation to specify that stencil value must be inverted

#### Defined in

packages/dev/core/src/Engines/engine.ts:126

___

### KEEP

▪ `Static` `Readonly` **KEEP**: ``7680``

Passed to stencilOperation to specify that stencil value must be kept

#### Defined in

packages/dev/core/src/Engines/engine.ts:118

___

### LEQUAL

▪ `Static` `Readonly` **LEQUAL**: ``515``

Passed to depthFunction or stencilFunction to specify depth or stencil tests will pass if the new depth value is less than or equal to the stored value

#### Defined in

packages/dev/core/src/Engines/engine.ts:108

___

### LESS

▪ `Static` `Readonly` **LESS**: ``513``

Passed to depthFunction or stencilFunction to specify depth or stencil tests will pass if the new depth value is less than the stored value

#### Defined in

packages/dev/core/src/Engines/engine.ts:104

___

### NEVER

▪ `Static` `Readonly` **NEVER**: ``512``

Passed to depthFunction or stencilFunction to specify depth or stencil tests will never pass. i.e. Nothing will be drawn

#### Defined in

packages/dev/core/src/Engines/engine.ts:100

___

### NOTEQUAL

▪ `Static` `Readonly` **NOTEQUAL**: ``517``

Passed to depthFunction or stencilFunction to specify depth or stencil tests will pass if the new depth value is not equal to the stored value

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

#### Defined in

packages/dev/core/src/Engines/engine.ts:495

___

### REPLACE

▪ `Static` `Readonly` **REPLACE**: ``7681``

Passed to stencilOperation to specify that stencil value must be replaced

#### Defined in

packages/dev/core/src/Engines/engine.ts:120

___

### SCALEMODE\_CEILING

▪ `Static` `Readonly` **SCALEMODE\_CEILING**: ``3``

Defines that texture rescaling will use a ceil to find the closer power of 2 size

#### Defined in

packages/dev/core/src/Engines/engine.ts:259

___

### SCALEMODE\_FLOOR

▪ `Static` `Readonly` **SCALEMODE\_FLOOR**: ``1``

Defines that texture rescaling will use a floor to find the closer power of 2 size

#### Defined in

packages/dev/core/src/Engines/engine.ts:255

___

### SCALEMODE\_NEAREST

▪ `Static` `Readonly` **SCALEMODE\_NEAREST**: ``2``

Defines that texture rescaling will look for the nearest power of 2 size

#### Defined in

packages/dev/core/src/Engines/engine.ts:257

___

### TEXTUREFORMAT\_ALPHA

▪ `Static` `Readonly` **TEXTUREFORMAT\_ALPHA**: ``0``

ALPHA

#### Defined in

packages/dev/core/src/Engines/engine.ts:140

___

### TEXTUREFORMAT\_LUMINANCE

▪ `Static` `Readonly` **TEXTUREFORMAT\_LUMINANCE**: ``1``

LUMINANCE

#### Defined in

packages/dev/core/src/Engines/engine.ts:142

___

### TEXTUREFORMAT\_LUMINANCE\_ALPHA

▪ `Static` `Readonly` **TEXTUREFORMAT\_LUMINANCE\_ALPHA**: ``2``

LUMINANCE_ALPHA

#### Defined in

packages/dev/core/src/Engines/engine.ts:144

___

### TEXTUREFORMAT\_R

▪ `Static` `Readonly` **TEXTUREFORMAT\_R**: ``6``

RED (2nd reference)

#### Defined in

packages/dev/core/src/Engines/engine.ts:152

___

### TEXTUREFORMAT\_RED

▪ `Static` `Readonly` **TEXTUREFORMAT\_RED**: ``6``

RED

#### Defined in

packages/dev/core/src/Engines/engine.ts:150

___

### TEXTUREFORMAT\_RED\_INTEGER

▪ `Static` `Readonly` **TEXTUREFORMAT\_RED\_INTEGER**: ``8``

RED_INTEGER

#### Defined in

packages/dev/core/src/Engines/engine.ts:156

___

### TEXTUREFORMAT\_RG

▪ `Static` `Readonly` **TEXTUREFORMAT\_RG**: ``7``

RG

#### Defined in

packages/dev/core/src/Engines/engine.ts:154

___

### TEXTUREFORMAT\_RGB

▪ `Static` `Readonly` **TEXTUREFORMAT\_RGB**: ``4``

RGB

#### Defined in

packages/dev/core/src/Engines/engine.ts:146

___

### TEXTUREFORMAT\_RGBA

▪ `Static` `Readonly` **TEXTUREFORMAT\_RGBA**: ``5``

RGBA

#### Defined in

packages/dev/core/src/Engines/engine.ts:148

___

### TEXTUREFORMAT\_RGBA\_INTEGER

▪ `Static` `Readonly` **TEXTUREFORMAT\_RGBA\_INTEGER**: ``11``

RGBA_INTEGER

#### Defined in

packages/dev/core/src/Engines/engine.ts:164

___

### TEXTUREFORMAT\_RGB\_INTEGER

▪ `Static` `Readonly` **TEXTUREFORMAT\_RGB\_INTEGER**: ``10``

RGB_INTEGER

#### Defined in

packages/dev/core/src/Engines/engine.ts:162

___

### TEXTUREFORMAT\_RG\_INTEGER

▪ `Static` `Readonly` **TEXTUREFORMAT\_RG\_INTEGER**: ``9``

RG_INTEGER

#### Defined in

packages/dev/core/src/Engines/engine.ts:160

___

### TEXTUREFORMAT\_R\_INTEGER

▪ `Static` `Readonly` **TEXTUREFORMAT\_R\_INTEGER**: ``8``

RED_INTEGER (2nd reference)

#### Defined in

packages/dev/core/src/Engines/engine.ts:158

___

### TEXTURETYPE\_BYTE

▪ `Static` `Readonly` **TEXTURETYPE\_BYTE**: ``3``

BYTE

#### Defined in

packages/dev/core/src/Engines/engine.ts:175

___

### TEXTURETYPE\_FLOAT

▪ `Static` `Readonly` **TEXTURETYPE\_FLOAT**: ``1``

FLOAT

#### Defined in

packages/dev/core/src/Engines/engine.ts:171

___

### TEXTURETYPE\_FLOAT\_32\_UNSIGNED\_INT\_24\_8\_REV

▪ `Static` `Readonly` **TEXTURETYPE\_FLOAT\_32\_UNSIGNED\_INT\_24\_8\_REV**: ``15``

FLOAT_32_UNSIGNED_INT_24_8_REV

#### Defined in

packages/dev/core/src/Engines/engine.ts:199

___

### TEXTURETYPE\_HALF\_FLOAT

▪ `Static` `Readonly` **TEXTURETYPE\_HALF\_FLOAT**: ``2``

HALF_FLOAT

#### Defined in

packages/dev/core/src/Engines/engine.ts:173

___

### TEXTURETYPE\_INT

▪ `Static` `Readonly` **TEXTURETYPE\_INT**: ``6``

INT

#### Defined in

packages/dev/core/src/Engines/engine.ts:181

___

### TEXTURETYPE\_SHORT

▪ `Static` `Readonly` **TEXTURETYPE\_SHORT**: ``4``

SHORT

#### Defined in

packages/dev/core/src/Engines/engine.ts:177

___

### TEXTURETYPE\_UNSIGNED\_BYTE

▪ `Static` `Readonly` **TEXTURETYPE\_UNSIGNED\_BYTE**: ``0``

UNSIGNED_BYTE

#### Defined in

packages/dev/core/src/Engines/engine.ts:167

___

### TEXTURETYPE\_UNSIGNED\_INT

▪ `Static` `Readonly` **TEXTURETYPE\_UNSIGNED\_INT**: ``0``

UNSIGNED_BYTE (2nd reference)

#### Defined in

packages/dev/core/src/Engines/engine.ts:169

___

### TEXTURETYPE\_UNSIGNED\_INTEGER

▪ `Static` `Readonly` **TEXTURETYPE\_UNSIGNED\_INTEGER**: ``7``

UNSIGNED_INT

#### Defined in

packages/dev/core/src/Engines/engine.ts:183

___

### TEXTURETYPE\_UNSIGNED\_INT\_10F\_11F\_11F\_REV

▪ `Static` `Readonly` **TEXTURETYPE\_UNSIGNED\_INT\_10F\_11F\_11F\_REV**: ``13``

UNSIGNED_INT_10F_11F_11F_REV

#### Defined in

packages/dev/core/src/Engines/engine.ts:195

___

### TEXTURETYPE\_UNSIGNED\_INT\_24\_8

▪ `Static` `Readonly` **TEXTURETYPE\_UNSIGNED\_INT\_24\_8**: ``12``

UNSIGNED_INT_24_8

#### Defined in

packages/dev/core/src/Engines/engine.ts:193

___

### TEXTURETYPE\_UNSIGNED\_INT\_2\_10\_10\_10\_REV

▪ `Static` `Readonly` **TEXTURETYPE\_UNSIGNED\_INT\_2\_10\_10\_10\_REV**: ``11``

UNSIGNED_INT_2_10_10_10_REV

#### Defined in

packages/dev/core/src/Engines/engine.ts:191

___

### TEXTURETYPE\_UNSIGNED\_INT\_5\_9\_9\_9\_REV

▪ `Static` `Readonly` **TEXTURETYPE\_UNSIGNED\_INT\_5\_9\_9\_9\_REV**: ``14``

UNSIGNED_INT_5_9_9_9_REV

#### Defined in

packages/dev/core/src/Engines/engine.ts:197

___

### TEXTURETYPE\_UNSIGNED\_SHORT

▪ `Static` `Readonly` **TEXTURETYPE\_UNSIGNED\_SHORT**: ``5``

UNSIGNED_SHORT

#### Defined in

packages/dev/core/src/Engines/engine.ts:179

___

### TEXTURETYPE\_UNSIGNED\_SHORT\_4\_4\_4\_4

▪ `Static` `Readonly` **TEXTURETYPE\_UNSIGNED\_SHORT\_4\_4\_4\_4**: ``8``

UNSIGNED_SHORT_4_4_4_4

#### Defined in

packages/dev/core/src/Engines/engine.ts:185

___

### TEXTURETYPE\_UNSIGNED\_SHORT\_5\_5\_5\_1

▪ `Static` `Readonly` **TEXTURETYPE\_UNSIGNED\_SHORT\_5\_5\_5\_1**: ``9``

UNSIGNED_SHORT_5_5_5_1

#### Defined in

packages/dev/core/src/Engines/engine.ts:187

___

### TEXTURETYPE\_UNSIGNED\_SHORT\_5\_6\_5

▪ `Static` `Readonly` **TEXTURETYPE\_UNSIGNED\_SHORT\_5\_6\_5**: ``10``

UNSIGNED_SHORT_5_6_5

#### Defined in

packages/dev/core/src/Engines/engine.ts:189

___

### TEXTURE\_BILINEAR\_SAMPLINGMODE

▪ `Static` `Readonly` **TEXTURE\_BILINEAR\_SAMPLINGMODE**: ``2``

Bilinear is mag = linear and min = linear and mip = nearest

#### Defined in

packages/dev/core/src/Engines/engine.ts:204

___

### TEXTURE\_CLAMP\_ADDRESSMODE

▪ `Static` `Readonly` **TEXTURE\_CLAMP\_ADDRESSMODE**: ``0``

Texture is not repeating outside of 0..1 UVs

#### Defined in

packages/dev/core/src/Engines/engine.ts:133

___

### TEXTURE\_CUBIC\_MODE

▪ `Static` `Readonly` **TEXTURE\_CUBIC\_MODE**: ``3``

Cubic coordinates mode

#### Defined in

packages/dev/core/src/Engines/engine.ts:239

___

### TEXTURE\_EQUIRECTANGULAR\_MODE

▪ `Static` `Readonly` **TEXTURE\_EQUIRECTANGULAR\_MODE**: ``7``

Equirectangular coordinates mode

#### Defined in

packages/dev/core/src/Engines/engine.ts:247

___

### TEXTURE\_EXPLICIT\_MODE

▪ `Static` `Readonly` **TEXTURE\_EXPLICIT\_MODE**: ``0``

Explicit coordinates mode

#### Defined in

packages/dev/core/src/Engines/engine.ts:233

___

### TEXTURE\_FIXED\_EQUIRECTANGULAR\_MIRRORED\_MODE

▪ `Static` `Readonly` **TEXTURE\_FIXED\_EQUIRECTANGULAR\_MIRRORED\_MODE**: ``9``

Equirectangular Fixed Mirrored coordinates mode

#### Defined in

packages/dev/core/src/Engines/engine.ts:251

___

### TEXTURE\_FIXED\_EQUIRECTANGULAR\_MODE

▪ `Static` `Readonly` **TEXTURE\_FIXED\_EQUIRECTANGULAR\_MODE**: ``8``

Equirectangular Fixed coordinates mode

#### Defined in

packages/dev/core/src/Engines/engine.ts:249

___

### TEXTURE\_INVCUBIC\_MODE

▪ `Static` `Readonly` **TEXTURE\_INVCUBIC\_MODE**: ``6``

Inverse Cubic coordinates mode

#### Defined in

packages/dev/core/src/Engines/engine.ts:245

___

### TEXTURE\_LINEAR\_LINEAR

▪ `Static` `Readonly` **TEXTURE\_LINEAR\_LINEAR**: ``2``

mag = linear and min = linear and mip = none

#### Defined in

packages/dev/core/src/Engines/engine.ts:228

___

### TEXTURE\_LINEAR\_LINEAR\_MIPLINEAR

▪ `Static` `Readonly` **TEXTURE\_LINEAR\_LINEAR\_MIPLINEAR**: ``3``

Trilinear is mag = linear and min = linear and mip = linear

#### Defined in

packages/dev/core/src/Engines/engine.ts:212

___

### TEXTURE\_LINEAR\_LINEAR\_MIPNEAREST

▪ `Static` `Readonly` **TEXTURE\_LINEAR\_LINEAR\_MIPNEAREST**: ``11``

Bilinear is mag = linear and min = linear and mip = nearest

#### Defined in

packages/dev/core/src/Engines/engine.ts:210

___

### TEXTURE\_LINEAR\_NEAREST

▪ `Static` `Readonly` **TEXTURE\_LINEAR\_NEAREST**: ``12``

mag = linear and min = nearest and mip = none

#### Defined in

packages/dev/core/src/Engines/engine.ts:230

___

### TEXTURE\_LINEAR\_NEAREST\_MIPLINEAR

▪ `Static` `Readonly` **TEXTURE\_LINEAR\_NEAREST\_MIPLINEAR**: ``10``

mag = linear and min = nearest and mip = linear

#### Defined in

packages/dev/core/src/Engines/engine.ts:226

___

### TEXTURE\_LINEAR\_NEAREST\_MIPNEAREST

▪ `Static` `Readonly` **TEXTURE\_LINEAR\_NEAREST\_MIPNEAREST**: ``9``

mag = linear and min = nearest and mip = nearest

#### Defined in

packages/dev/core/src/Engines/engine.ts:224

___

### TEXTURE\_MIRROR\_ADDRESSMODE

▪ `Static` `Readonly` **TEXTURE\_MIRROR\_ADDRESSMODE**: ``2``

Texture is repeating and mirrored

#### Defined in

packages/dev/core/src/Engines/engine.ts:137

___

### TEXTURE\_NEAREST\_LINEAR

▪ `Static` `Readonly` **TEXTURE\_NEAREST\_LINEAR**: ``7``

mag = nearest and min = linear and mip = none

#### Defined in

packages/dev/core/src/Engines/engine.ts:220

___

### TEXTURE\_NEAREST\_LINEAR\_MIPLINEAR

▪ `Static` `Readonly` **TEXTURE\_NEAREST\_LINEAR\_MIPLINEAR**: ``6``

mag = nearest and min = linear and mip = linear

#### Defined in

packages/dev/core/src/Engines/engine.ts:218

___

### TEXTURE\_NEAREST\_LINEAR\_MIPNEAREST

▪ `Static` `Readonly` **TEXTURE\_NEAREST\_LINEAR\_MIPNEAREST**: ``5``

mag = nearest and min = linear and mip = nearest

#### Defined in

packages/dev/core/src/Engines/engine.ts:216

___

### TEXTURE\_NEAREST\_NEAREST

▪ `Static` `Readonly` **TEXTURE\_NEAREST\_NEAREST**: ``1``

mag = nearest and min = nearest and mip = none

#### Defined in

packages/dev/core/src/Engines/engine.ts:222

___

### TEXTURE\_NEAREST\_NEAREST\_MIPLINEAR

▪ `Static` `Readonly` **TEXTURE\_NEAREST\_NEAREST\_MIPLINEAR**: ``8``

nearest is mag = nearest and min = nearest and mip = linear

#### Defined in

packages/dev/core/src/Engines/engine.ts:208

___

### TEXTURE\_NEAREST\_NEAREST\_MIPNEAREST

▪ `Static` `Readonly` **TEXTURE\_NEAREST\_NEAREST\_MIPNEAREST**: ``4``

mag = nearest and min = nearest and mip = nearest

#### Defined in

packages/dev/core/src/Engines/engine.ts:214

___

### TEXTURE\_NEAREST\_SAMPLINGMODE

▪ `Static` `Readonly` **TEXTURE\_NEAREST\_SAMPLINGMODE**: ``1``

nearest is mag = nearest and min = nearest and mip = none

#### Defined in

packages/dev/core/src/Engines/engine.ts:202

___

### TEXTURE\_PLANAR\_MODE

▪ `Static` `Readonly` **TEXTURE\_PLANAR\_MODE**: ``2``

Planar coordinates mode

#### Defined in

packages/dev/core/src/Engines/engine.ts:237

___

### TEXTURE\_PROJECTION\_MODE

▪ `Static` `Readonly` **TEXTURE\_PROJECTION\_MODE**: ``4``

Projection coordinates mode

#### Defined in

packages/dev/core/src/Engines/engine.ts:241

___

### TEXTURE\_SKYBOX\_MODE

▪ `Static` `Readonly` **TEXTURE\_SKYBOX\_MODE**: ``5``

Skybox coordinates mode

#### Defined in

packages/dev/core/src/Engines/engine.ts:243

___

### TEXTURE\_SPHERICAL\_MODE

▪ `Static` `Readonly` **TEXTURE\_SPHERICAL\_MODE**: ``1``

Spherical coordinates mode

#### Defined in

packages/dev/core/src/Engines/engine.ts:235

___

### TEXTURE\_TRILINEAR\_SAMPLINGMODE

▪ `Static` `Readonly` **TEXTURE\_TRILINEAR\_SAMPLINGMODE**: ``3``

Trilinear is mag = linear and min = linear and mip = linear

#### Defined in

packages/dev/core/src/Engines/engine.ts:206

___

### TEXTURE\_WRAP\_ADDRESSMODE

▪ `Static` `Readonly` **TEXTURE\_WRAP\_ADDRESSMODE**: ``1``

Texture is repeating outside of 0..1 UVs

#### Defined in

packages/dev/core/src/Engines/engine.ts:135

___

### \_RenderPassIdCounter

▪ `Static` `Protected` **\_RenderPassIdCounter**: `number` = `0`

#### Defined in

packages/dev/core/src/Engines/engine.ts:1576

___

### \_RescalePostProcessFactory

▪ `Static` **\_RescalePostProcessFactory**: [`Nullable`](../modules.md#nullable)(`engine`: [`Engine`](Engine.md)) => [`PostProcess`](PostProcess.md) = `null`

Method called to create the default rescale post process on each engine.

#### Defined in

packages/dev/core/src/Engines/engine.ts:384

___

### audioEngine

▪ `Static` **audioEngine**: [`Nullable`](../modules.md#nullable)[`IAudioEngine`](../interfaces/IAudioEngine.md)

Gets the audio engine

**`See`**

https://doc.babylonjs.com/how_to/playing_sounds_and_music

**`Ignorenaming`**

#### Defined in

packages/dev/core/src/Engines/engine.ts:479

## Accessors

### \_supportsHardwareTextureRescaling

• `Protected` `get` **_supportsHardwareTextureRescaling**(): `boolean`

#### Returns

`boolean`

#### Overrides

ThinEngine.\_supportsHardwareTextureRescaling

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

ThinEngine.activeRenderLoops

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:430

___

### alphaState

• `get` **alphaState**(): `AlphaState`

Gets the alpha state manager

#### Returns

`AlphaState`

#### Inherited from

ThinEngine.alphaState

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

#### Defined in

packages/dev/core/src/Engines/engine.ts:552

• `set` **compatibilityMode**(`mode`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `mode` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Engines/engine.ts:556

___

### currentViewport

• `get` **currentViewport**(): [`Nullable`](../modules.md#nullable)`IViewportLike`

Gets the current viewport

#### Returns

[`Nullable`](../modules.md#nullable)`IViewportLike`

#### Inherited from

ThinEngine.currentViewport

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:587

___

### depthCullingState

• `get` **depthCullingState**(): `DepthCullingState`

Gets the depth culling state manager

#### Returns

`DepthCullingState`

#### Inherited from

ThinEngine.depthCullingState

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:3546

___

### description

• `get` **description**(): `string`

Returns a string describing the current engine

#### Returns

`string`

#### Inherited from

ThinEngine.description

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

ThinEngine.doNotHandleContextLost

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

ThinEngine.doNotHandleContextLost

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:458

___

### emptyCubeTexture

• `get` **emptyCubeTexture**(): [`InternalTexture`](InternalTexture.md)

Gets the default empty cube texture

#### Returns

[`InternalTexture`](InternalTexture.md)

#### Inherited from

ThinEngine.emptyCubeTexture

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:636

___

### emptyTexture

• `get` **emptyTexture**(): [`InternalTexture`](InternalTexture.md)

Gets the default empty texture

#### Returns

[`InternalTexture`](InternalTexture.md)

#### Inherited from

ThinEngine.emptyTexture

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:594

___

### emptyTexture2DArray

• `get` **emptyTexture2DArray**(): [`InternalTexture`](InternalTexture.md)

Gets the default empty 2D array texture

#### Returns

[`InternalTexture`](InternalTexture.md)

#### Inherited from

ThinEngine.emptyTexture2DArray

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:616

___

### emptyTexture3D

• `get` **emptyTexture3D**(): [`InternalTexture`](InternalTexture.md)

Gets the default empty 3D texture

#### Returns

[`InternalTexture`](InternalTexture.md)

#### Inherited from

ThinEngine.emptyTexture3D

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:605

___

### frameId

• `get` **frameId**(): `number`

Gets the current frame id

#### Returns

`number`

#### Inherited from

ThinEngine.frameId

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

ThinEngine.framebufferDimensionsObject

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:580

___

### isStencilEnable

• `get` **isStencilEnable**(): `boolean`

Returns true if the stencil buffer has been enabled through the creation option of the context.

#### Returns

`boolean`

#### Inherited from

ThinEngine.isStencilEnable

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1425

___

### isWebGPU

• `get` **isWebGPU**(): `boolean`

Gets a boolean indicating if the engine runs in WebGPU or not.

#### Returns

`boolean`

#### Inherited from

ThinEngine.isWebGPU

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

#### Defined in

packages/dev/core/src/Engines/engine.ts:2038

___

### loadingUIText

• `set` **loadingUIText**(`text`): `void`

Sets the current loading screen text

**`See`**

https://doc.babylonjs.com/how_to/creating_a_custom_loading_screen

#### Parameters

| Name | Type |
| :------ | :------ |
| `text` | `string` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Engines/engine.ts:2030

___

### name

• `get` **name**(): `string`

Gets or sets the name of the engine

#### Returns

`string`

#### Inherited from

ThinEngine.name

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

ThinEngine.name

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

ThinEngine.needPOTTextures

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

#### Defined in

packages/dev/core/src/Engines/engine.ts:530

___

### shaderPlatformName

• `get` **shaderPlatformName**(): `string`

Gets the shader platform name used by the effects.

#### Returns

`string`

#### Inherited from

ThinEngine.shaderPlatformName

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

ThinEngine.snapshotRendering

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

ThinEngine.snapshotRendering

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:690

___

### snapshotRenderingMode

• `get` **snapshotRenderingMode**(): `number`

Gets or sets the snapshot rendering mode

#### Returns

`number`

#### Inherited from

ThinEngine.snapshotRenderingMode

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

ThinEngine.snapshotRenderingMode

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:702

___

### stencilState

• `get` **stencilState**(): `StencilState`

Gets the stencil state manager

#### Returns

`StencilState`

#### Inherited from

ThinEngine.stencilState

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:3560

___

### stencilStateComposer

• `get` **stencilStateComposer**(): `StencilStateComposer`

Gets the stencil state composer

#### Returns

`StencilStateComposer`

#### Inherited from

ThinEngine.stencilStateComposer

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

ThinEngine.supportsUniformBuffers

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:364

___

### useExactSrgbConversions

• `get` **useExactSrgbConversions**(): `boolean`

Gets a boolean indicating if the exact sRGB conversions or faster approximations are used for converting to and from linear space.

#### Returns

`boolean`

#### Inherited from

ThinEngine.useExactSrgbConversions

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

ThinEngine.useReverseDepthBuffer

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

ThinEngine.useReverseDepthBuffer

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:313

___

### version

• `get` **version**(): `number`

Returns the version of the engine

#### Returns

`number`

#### Inherited from

ThinEngine.version

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

ThinEngine.webGLVersion

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1410

___

### HasMajorPerformanceCaveat

• `Static` `get` **HasMajorPerformanceCaveat**(): `boolean`

Gets a boolean indicating if the engine can be instantiated on a performant device (ie. if a webGL context can be found and it does not use a slow implementation)

#### Returns

`boolean`

#### Inherited from

ThinEngine.HasMajorPerformanceCaveat

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:5833

___

### Instances

• `Static` `get` **Instances**(): [`Engine`](Engine.md)[]

Gets the list of created engines

#### Returns

[`Engine`](Engine.md)[]

#### Defined in

packages/dev/core/src/Engines/engine.ts:277

___

### IsSupported

• `Static` `get` **IsSupported**(): `boolean`

Gets a boolean indicating if the engine can be instantiated (ie. if a webGL context can be found)

#### Returns

`boolean`

#### Inherited from

ThinEngine.IsSupported

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:5801

___

### IsSupportedAsync

• `Static` `get` **IsSupportedAsync**(): `Promise``boolean`

Gets a Promise indicating if the engine can be instantiated (ie. if a webGL context can be found)

#### Returns

`Promise``boolean`

#### Inherited from

ThinEngine.IsSupportedAsync

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:5794

___

### LastCreatedEngine

• `Static` `get` **LastCreatedEngine**(): [`Nullable`](../modules.md#nullable)[`Engine`](Engine.md)

Gets the latest created engine

#### Returns

[`Nullable`](../modules.md#nullable)[`Engine`](Engine.md)

#### Defined in

packages/dev/core/src/Engines/engine.ts:284

___

### LastCreatedScene

• `Static` `get` **LastCreatedScene**(): [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md)

Gets the latest created scene

#### Returns

[`Nullable`](../modules.md#nullable)[`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/Engines/engine.ts:291

___

### NpmPackage

• `Static` `get` **NpmPackage**(): `string`

Returns the current npm package of the sdk

#### Returns

`string`

#### Overrides

ThinEngine.NpmPackage

#### Defined in

packages/dev/core/src/Engines/engine.ts:265

___

### ShadersRepository

• `Static` `get` **ShadersRepository**(): `string`

Gets or sets the relative url used to load shaders if using the engine in non-minified mode

#### Returns

`string`

#### Inherited from

ThinEngine.ShadersRepository

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

ThinEngine.ShadersRepository

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:261

___

### Version

• `Static` `get` **Version**(): `string`

Returns the current version of the framework

#### Returns

`string`

#### Overrides

ThinEngine.Version

#### Defined in

packages/dev/core/src/Engines/engine.ts:272

## Methods

### \_clientWaitAsync

▸ `Private` **_clientWaitAsync**(`sync`, `flags?`, `intervalms?`): `Promise``void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `sync` | `WebGLSync` | `undefined` |
| `flags` | `number` | `0` |
| `intervalms` | `number` | `10` |

#### Returns

`Promise``void`

#### Defined in

packages/dev/core/src/Engines/engine.ts:1830

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

#### Inherited from

[ThinEngine](ThinEngine.md).[_createDepthStencilCubeTexture](ThinEngine.md#_createdepthstencilcubetexture)

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

#### Overrides

[ThinEngine](ThinEngine.md).[_createShaderProgram](ThinEngine.md#_createshaderprogram)

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

[ThinEngine](ThinEngine.md).[_createTextureBase](ThinEngine.md#_createtexturebase)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:3851

___

### \_deleteBuffer

▸ `Protected` **_deleteBuffer**(`buffer`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `buffer` | [`DataBuffer`](DataBuffer.md) |

#### Returns

`void`

#### Inherited from

[ThinEngine](ThinEngine.md).[_deleteBuffer](ThinEngine.md#_deletebuffer)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:2474

___

### \_deletePipelineContext

▸ **_deletePipelineContext**(`pipelineContext`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `pipelineContext` | [`IPipelineContext`](../interfaces/IPipelineContext.md) |

#### Returns

`void`

#### Overrides

ThinEngine.\_deletePipelineContext

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

[ThinEngine](ThinEngine.md).[_deleteTexture](ThinEngine.md#_deletetexture)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:4903

___

### \_disableTouchAction

▸ `Private` **_disableTouchAction**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Engines/engine.ts:1966

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

[ThinEngine](ThinEngine.md).[_finalizePipelineContext](ThinEngine.md#_finalizepipelinecontext)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:2999

___

### \_initFeatures

▸ `Protected` **_initFeatures**(): `void`

#### Returns

`void`

#### Inherited from

[ThinEngine](ThinEngine.md).[_initFeatures](ThinEngine.md#_initfeatures)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1378

___

### \_initGLContext

▸ `Protected` **_initGLContext**(): `void`

#### Returns

`void`

#### Inherited from

[ThinEngine](ThinEngine.md).[_initGLContext](ThinEngine.md#_initglcontext)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1130

___

### \_measureFps

▸ `Private` **_measureFps**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Engines/engine.ts:1708

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

[ThinEngine](ThinEngine.md).[_normalizeIndexData](ThinEngine.md#_normalizeindexdata)

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

[ThinEngine](ThinEngine.md).[_prepareWebGLTextureContinuation](ThinEngine.md#_preparewebgltexturecontinuation)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:4702

___

### \_rebuildBuffers

▸ `Protected` **_rebuildBuffers**(): `void`

#### Returns

`void`

#### Overrides

[ThinEngine](ThinEngine.md).[_rebuildBuffers](ThinEngine.md#_rebuildbuffers)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1281

___

### \_renderLoop

▸ **_renderLoop**(): `void`

#### Returns

`void`

#### Overrides

ThinEngine.\_renderLoop

#### Defined in

packages/dev/core/src/Engines/engine.ts:1307

___

### \_resetIndexBufferBinding

▸ `Protected` **_resetIndexBufferBinding**(): `void`

#### Returns

`void`

#### Inherited from

[ThinEngine](ThinEngine.md).[_resetIndexBufferBinding](ThinEngine.md#_resetindexbufferbinding)

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

[ThinEngine](ThinEngine.md).[_restoreEngineAfterContextLost](ThinEngine.md#_restoreengineaftercontextlost)

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

[ThinEngine](ThinEngine.md).[_setProgram](ThinEngine.md#_setprogram)

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

[ThinEngine](ThinEngine.md).[_setTexture](ThinEngine.md#_settexture)

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

#### Overrides

[ThinEngine](ThinEngine.md).[_sharedInit](ThinEngine.md#_sharedinit)

#### Defined in

packages/dev/core/src/Engines/engine.ts:669

___

### applyStates

▸ **applyStates**(): `void`

Apply all cached states (depth, culling, stencil and alpha)

#### Returns

`void`

#### Inherited from

[ThinEngine](ThinEngine.md).[applyStates](ThinEngine.md#applystates)

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

[ThinEngine](ThinEngine.md).[areAllComputeEffectsReady](ThinEngine.md#areallcomputeeffectsready)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.computeShader.ts:79

___

### areAllEffectsReady

▸ **areAllEffectsReady**(): `boolean`

Gets a boolean indicating if all created effects are ready

#### Returns

`boolean`

true if all effects are ready

#### Inherited from

[ThinEngine](ThinEngine.md).[areAllEffectsReady](ThinEngine.md#arealleffectsready)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1107

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

[ThinEngine](ThinEngine.md).[attachContextLostEvent](ThinEngine.md#attachcontextlostevent)

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

[ThinEngine](ThinEngine.md).[attachContextRestoredEvent](ThinEngine.md#attachcontextrestoredevent)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:5337

___

### beginFrame

▸ **beginFrame**(): `void`

Begin a new frame

#### Returns

`void`

#### Overrides

[ThinEngine](ThinEngine.md).[beginFrame](ThinEngine.md#beginframe)

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

[ThinEngine](ThinEngine.md).[bindArrayBuffer](ThinEngine.md#bindarraybuffer)

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

[ThinEngine](ThinEngine.md).[bindAttachments](ThinEngine.md#bindattachments)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.multiRender.ts:47

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

#### Inherited from

[ThinEngine](ThinEngine.md).[bindBuffers](ThinEngine.md#bindbuffers)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:2417

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

[ThinEngine](ThinEngine.md).[bindBuffersDirectly](ThinEngine.md#bindbuffersdirectly)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:2372

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

#### Inherited from

[ThinEngine](ThinEngine.md).[bindFramebuffer](ThinEngine.md#bindframebuffer)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1807

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

[ThinEngine](ThinEngine.md).[bindIndexBuffer](ThinEngine.md#bindindexbuffer)

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

[ThinEngine](ThinEngine.md).[bindInstancesBuffer](ThinEngine.md#bindinstancesbuffer)

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

#### Inherited from

[ThinEngine](ThinEngine.md).[bindSamplers](ThinEngine.md#bindsamplers)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:4922

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

[ThinEngine](ThinEngine.md).[bindUniformBlock](ThinEngine.md#binduniformblock)

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

[ThinEngine](ThinEngine.md).[bindUniformBlock](ThinEngine.md#binduniformblock)

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

[ThinEngine](ThinEngine.md).[bindUniformBuffer](ThinEngine.md#binduniformbuffer)

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

[ThinEngine](ThinEngine.md).[bindUniformBufferBase](ThinEngine.md#binduniformbufferbase)

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

[ThinEngine](ThinEngine.md).[bindVertexArrayObject](ThinEngine.md#bindvertexarrayobject)

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

[ThinEngine](ThinEngine.md).[buildTextureLayout](ThinEngine.md#buildtexturelayout)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.multiRender.ts:54

___

### cacheStencilState

▸ **cacheStencilState**(): `void`

Caches the the state of the stencil buffer

#### Returns

`void`

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

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.query.ts:106

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

#### Inherited from

[ThinEngine](ThinEngine.md).[clear](ThinEngine.md#clear)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1662

___

### clearInternalTexturesCache

▸ **clearInternalTexturesCache**(): `void`

Clears the list of texture accessible through engine.
This can help preventing texture load conflict due to name collision.

#### Returns

`void`

#### Inherited from

[ThinEngine](ThinEngine.md).[clearInternalTexturesCache](ThinEngine.md#clearinternaltexturescache)

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

[ThinEngine](ThinEngine.md).[computeDispatch](ThinEngine.md#computedispatch)

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

[ThinEngine](ThinEngine.md).[createCanvas](ThinEngine.md#createcanvas)

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

[ThinEngine](ThinEngine.md).[createCanvasImage](ThinEngine.md#createcanvasimage)

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

[ThinEngine](ThinEngine.md).[createComputeContext](ThinEngine.md#createcomputecontext)

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

[ThinEngine](ThinEngine.md).[createComputeEffect](ThinEngine.md#createcomputeeffect)

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

[ThinEngine](ThinEngine.md).[createComputePipelineContext](ThinEngine.md#createcomputepipelinecontext)

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

[ThinEngine](ThinEngine.md).[createCubeTexture](ThinEngine.md#createcubetexture)

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

[ThinEngine](ThinEngine.md).[createCubeTexture](ThinEngine.md#createcubetexture)

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

[ThinEngine](ThinEngine.md).[createCubeTexture](ThinEngine.md#createcubetexture)

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

[ThinEngine](ThinEngine.md).[createDepthStencilTexture](ThinEngine.md#createdepthstenciltexture)

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

[ThinEngine](ThinEngine.md).[createDrawContext](ThinEngine.md#createdrawcontext)

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

[ThinEngine](ThinEngine.md).[createDynamicTexture](ThinEngine.md#createdynamictexture)

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

[ThinEngine](ThinEngine.md).[createDynamicUniformBuffer](ThinEngine.md#createdynamicuniformbuffer)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.uniformBuffer.ts:24

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

#### Inherited from

[ThinEngine](ThinEngine.md).[createDynamicVertexBuffer](ThinEngine.md#createdynamicvertexbuffer)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:2088

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

[ThinEngine](ThinEngine.md).[createEffect](ThinEngine.md#createeffect)

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

[ThinEngine](ThinEngine.md).[createExternalTexture](ThinEngine.md#createexternaltexture)

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

#### Defined in

packages/dev/core/src/Engines/engine.ts:328

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

#### Inherited from

[ThinEngine](ThinEngine.md).[createIndexBuffer](ThinEngine.md#createindexbuffer)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:2103

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

[ThinEngine](ThinEngine.md).[createMaterialContext](ThinEngine.md#creatematerialcontext)

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

[ThinEngine](ThinEngine.md).[createMultipleRenderTarget](ThinEngine.md#createmultiplerendertarget)

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

[ThinEngine](ThinEngine.md).[createPipelineContext](ThinEngine.md#createpipelinecontext)

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

[ThinEngine](ThinEngine.md).[createPrefilteredCubeTexture](ThinEngine.md#createprefilteredcubetexture)

#### Defined in

packages/dev/core/src/Misc/dds.ts:733

___

### createQuery

▸ **createQuery**(): `OcclusionQuery`

Create a new webGL query (you must be sure that queries are supported by checking getCaps() function)

#### Returns

`OcclusionQuery`

the new query

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

[ThinEngine](ThinEngine.md).[createRawCubeTexture](ThinEngine.md#createrawcubetexture)

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

[ThinEngine](ThinEngine.md).[createRawCubeTexture](ThinEngine.md#createrawcubetexture)

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

[ThinEngine](ThinEngine.md).[createRawCubeTextureFromUrl](ThinEngine.md#createrawcubetexturefromurl)

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

[ThinEngine](ThinEngine.md).[createRawCubeTextureFromUrl](ThinEngine.md#createrawcubetexturefromurl)

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

[ThinEngine](ThinEngine.md).[createRawShaderProgram](ThinEngine.md#createrawshaderprogram)

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

#### Inherited from

[ThinEngine](ThinEngine.md).[createRawTexture](ThinEngine.md#createrawtexture)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:4263

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

#### Inherited from

[ThinEngine](ThinEngine.md).[createRawTexture](ThinEngine.md#createrawtexture)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.rawTexture.ts:27

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

[ThinEngine](ThinEngine.md).[createRawTexture2DArray](ThinEngine.md#createrawtexture2darray)

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

[ThinEngine](ThinEngine.md).[createRawTexture2DArray](ThinEngine.md#createrawtexture2darray)

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

[ThinEngine](ThinEngine.md).[createRawTexture3D](ThinEngine.md#createrawtexture3d)

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

[ThinEngine](ThinEngine.md).[createRawTexture3D](ThinEngine.md#createrawtexture3d)

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

[ThinEngine](ThinEngine.md).[createRenderTargetCubeTexture](ThinEngine.md#createrendertargetcubetexture)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.renderTargetCube.ts:17

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

#### Inherited from

[ThinEngine](ThinEngine.md).[createRenderTargetTexture](ThinEngine.md#createrendertargettexture)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.renderTarget.ts:26

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

#### Overrides

[ThinEngine](ThinEngine.md).[createShaderProgram](ThinEngine.md#createshaderprogram)

#### Defined in

packages/dev/core/src/Engines/engine.ts:1481

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

[ThinEngine](ThinEngine.md).[createStorageBuffer](ThinEngine.md#createstoragebuffer)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.storageBuffer.ts:15

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

#### Inherited from

[ThinEngine](ThinEngine.md).[createTexture](ThinEngine.md#createtexture)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:4124

___

### createTransformFeedback

▸ **createTransformFeedback**(): `WebGLTransformFeedback`

Creates a webGL transform feedback object
Please makes sure to check webGLVersion property to check if you are running webGL 2+

#### Returns

`WebGLTransformFeedback`

the webGL transform feedback object

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

[ThinEngine](ThinEngine.md).[createUniformBuffer](ThinEngine.md#createuniformbuffer)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.uniformBuffer.ts:16

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

#### Inherited from

[ThinEngine](ThinEngine.md).[createVertexBuffer](ThinEngine.md#createvertexbuffer)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:2057

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

[ThinEngine](ThinEngine.md).[disableAttributeByIndex](ThinEngine.md#disableattributebyindex)

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

[ThinEngine](ThinEngine.md).[disableInstanceAttribute](ThinEngine.md#disableinstanceattribute)

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

[ThinEngine](ThinEngine.md).[disableInstanceAttributeByName](ThinEngine.md#disableinstanceattributebyname)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:2552

___

### disableScissor

▸ **disableScissor**(): `void`

Disable previously set scissor test rectangle

#### Returns

`void`

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

#### Defined in

packages/dev/core/src/Engines/engine.ts:1983

___

### dispose

▸ **dispose**(): `void`

Dispose and release all associated resources

#### Returns

`void`

#### Overrides

[ThinEngine](ThinEngine.md).[dispose](ThinEngine.md#dispose)

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

#### Inherited from

[ThinEngine](ThinEngine.md).[draw](ThinEngine.md#draw)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:2599

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

#### Inherited from

[ThinEngine](ThinEngine.md).[drawArraysType](ThinEngine.md#drawarraystype)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:2656

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

#### Inherited from

[ThinEngine](ThinEngine.md).[drawElementsType](ThinEngine.md#drawelementstype)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:2631

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

[ThinEngine](ThinEngine.md).[drawPointClouds](ThinEngine.md#drawpointclouds)

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

[ThinEngine](ThinEngine.md).[drawUnIndexed](ThinEngine.md#drawunindexed)

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

#### Inherited from

[ThinEngine](ThinEngine.md).[enableEffect](ThinEngine.md#enableeffect)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:3174

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

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.webVR.ts:103

___

### endFrame

▸ **endFrame**(): `void`

End the current frame

#### Returns

`void`

#### Overrides

[ThinEngine](ThinEngine.md).[endFrame](ThinEngine.md#endframe)

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

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.query.ts:94

___

### endTransformFeedback

▸ **endTransformFeedback**(): `void`

Ends a transform feedback operation

#### Returns

`void`

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

#### Defined in

packages/dev/core/src/Engines/engine.ts:1368

___

### enterPointerlock

▸ **enterPointerlock**(): `void`

Enters Pointerlock mode

#### Returns

`void`

#### Defined in

packages/dev/core/src/Engines/engine.ts:1389

___

### exitFullscreen

▸ **exitFullscreen**(): `void`

Exits full screen mode

#### Returns

`void`

#### Defined in

packages/dev/core/src/Engines/engine.ts:1380

___

### exitPointerlock

▸ **exitPointerlock**(): `void`

Exits Pointerlock mode

#### Returns

`void`

#### Defined in

packages/dev/core/src/Engines/engine.ts:1398

___

### flushFramebuffer

▸ **flushFramebuffer**(): `void`

Force a webGL flush (ie. a flush of all waiting webGL commands)

#### Returns

`void`

#### Inherited from

[ThinEngine](ThinEngine.md).[flushFramebuffer](ThinEngine.md#flushframebuffer)

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

[ThinEngine](ThinEngine.md).[generateMipmaps](ThinEngine.md#generatemipmaps)

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

[ThinEngine](ThinEngine.md).[getAlphaEquation](ThinEngine.md#getalphaequation)

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

[ThinEngine](ThinEngine.md).[getAlphaMode](ThinEngine.md#getalphamode)

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

#### Defined in

packages/dev/core/src/Engines/engine.ts:738

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

#### Inherited from

[ThinEngine](ThinEngine.md).[getAttributes](ThinEngine.md#getattributes)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:3155

___

### getAudioContext

▸ **getAudioContext**(): [`Nullable`](../modules.md#nullable)`AudioContext`

Gets the audio context specified in engine initialization options

#### Returns

[`Nullable`](../modules.md#nullable)`AudioContext`

an Audio Context

#### Inherited from

[ThinEngine](ThinEngine.md).[getAudioContext](ThinEngine.md#getaudiocontext)

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

[ThinEngine](ThinEngine.md).[getAudioDestination](ThinEngine.md#getaudiodestination)

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

[ThinEngine](ThinEngine.md).[getCaps](ThinEngine.md#getcaps)

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

[ThinEngine](ThinEngine.md).[getClassName](ThinEngine.md#getclassname)

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

[ThinEngine](ThinEngine.md).[getColorWrite](ThinEngine.md#getcolorwrite)

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

[ThinEngine](ThinEngine.md).[getCreationOptions](ThinEngine.md#getcreationoptions)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:384

___

### getCurrentRenderPassName

▸ **getCurrentRenderPassName**(): `string`

Gets the name of the current render pass

#### Returns

`string`

name of the current render pass

#### Defined in

packages/dev/core/src/Engines/engine.ts:1595

___

### getDeltaTime

▸ **getDeltaTime**(): `number`

Gets the time spent between current and previous frame

#### Returns

`number`

a number representing the delta time in ms

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

[ThinEngine](ThinEngine.md).[getDepthBuffer](ThinEngine.md#getdepthbuffer)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1910

___

### getDepthFunction

▸ **getDepthFunction**(): [`Nullable`](../modules.md#nullable)`number`

Gets the current depth function

#### Returns

[`Nullable`](../modules.md#nullable)`number`

a number defining the depth function

#### Defined in

packages/dev/core/src/Engines/engine.ts:989

___

### getDepthWrite

▸ **getDepthWrite**(): `boolean`

Gets a boolean indicating if depth writing is enabled

#### Returns

`boolean`

the current depth writing state

#### Defined in

packages/dev/core/src/Engines/engine.ts:821

___

### getError

▸ **getError**(): `number`

Get the current error code of the webGL context

**`See`**

https://developer.mozilla.org/en-US/docs/Web/API/WebGLRenderingContext/getError

#### Returns

`number`

the error code

#### Inherited from

[ThinEngine](ThinEngine.md).[getError](ThinEngine.md#geterror)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:5348

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

#### Defined in

packages/dev/core/src/Engines/engine.ts:2113

___

### getFps

▸ **getFps**(): `number`

Gets the current framerate

#### Returns

`number`

a number representing the framerate

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

#### Defined in

packages/dev/core/src/Engines/engine.ts:1219

___

### getGPUFrameTimeCounter

▸ **getGPUFrameTimeCounter**(): [`PerfCounter`](PerfCounter.md)

Get the performance counter associated with the frame time computation

#### Returns

[`PerfCounter`](PerfCounter.md)

the perf counter

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

[ThinEngine](ThinEngine.md).[getGlInfo](ThinEngine.md#getglinfo)

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

#### Inherited from

[ThinEngine](ThinEngine.md).[getHardwareScalingLevel](ThinEngine.md#gethardwarescalinglevel)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1494

___

### getHostDocument

▸ **getHostDocument**(): [`Nullable`](../modules.md#nullable)`Document`

Gets host document

#### Returns

[`Nullable`](../modules.md#nullable)`Document`

the host document object

#### Inherited from

[ThinEngine](ThinEngine.md).[getHostDocument](ThinEngine.md#gethostdocument)

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

[ThinEngine](ThinEngine.md).[getHostWindow](ThinEngine.md#gethostwindow)

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

[ThinEngine](ThinEngine.md).[getInfo](ThinEngine.md#getinfo)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1461

___

### getInputElement

▸ **getInputElement**(): [`Nullable`](../modules.md#nullable)`HTMLElement`

Gets the HTML element used to attach event listeners

#### Returns

[`Nullable`](../modules.md#nullable)`HTMLElement`

a HTML element

#### Defined in

packages/dev/core/src/Engines/engine.ts:567

___

### getInputElementClientRect

▸ **getInputElementClientRect**(): [`Nullable`](../modules.md#nullable)`ClientRect`

Gets the client rect of the HTML element used for events

#### Returns

[`Nullable`](../modules.md#nullable)`ClientRect`

a client rectangle

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

[ThinEngine](ThinEngine.md).[getLoadedTexturesCache](ThinEngine.md#getloadedtexturescache)

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

#### Defined in

packages/dev/core/src/Engines/engine.ts:787

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

#### Inherited from

[ThinEngine](ThinEngine.md).[getRenderHeight](ThinEngine.md#getrenderheight)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1619

___

### getRenderPassNames

▸ **getRenderPassNames**(): `string`[]

Gets the names of the render passes that are currently created

#### Returns

`string`[]

list of the render pass names

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

#### Inherited from

[ThinEngine](ThinEngine.md).[getRenderWidth](ThinEngine.md#getrenderwidth)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1606

___

### getRenderingCanvas

▸ **getRenderingCanvas**(): [`Nullable`](../modules.md#nullable)`HTMLCanvasElement`

Gets the HTML canvas attached with the current webGL context

#### Returns

[`Nullable`](../modules.md#nullable)`HTMLCanvasElement`

a HTML canvas

#### Inherited from

[ThinEngine](ThinEngine.md).[getRenderingCanvas](ThinEngine.md#getrenderingcanvas)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1565

___

### getRenderingCanvasClientRect

▸ **getRenderingCanvasClientRect**(): [`Nullable`](../modules.md#nullable)`ClientRect`

Gets the client rect of the HTML canvas attached with the current webGL context

#### Returns

[`Nullable`](../modules.md#nullable)`ClientRect`

a client rectangle

#### Defined in

packages/dev/core/src/Engines/engine.ts:755

___

### getScreenAspectRatio

▸ **getScreenAspectRatio**(): `number`

Gets current screen aspect ratio

#### Returns

`number`

a number defining the aspect ratio

#### Defined in

packages/dev/core/src/Engines/engine.ts:747

___

### getStencilBuffer

▸ **getStencilBuffer**(): `boolean`

Gets a boolean indicating if stencil buffer is enabled

#### Returns

`boolean`

the current stencil buffer state

#### Defined in

packages/dev/core/src/Engines/engine.ts:837

___

### getStencilFunction

▸ **getStencilFunction**(): `number`

Gets the current stencil function

#### Returns

`number`

a number defining the stencil function to use

#### Defined in

packages/dev/core/src/Engines/engine.ts:869

___

### getStencilFunctionMask

▸ **getStencilFunctionMask**(): `number`

Gets the current stencil mask

#### Returns

`number`

a number defining the stencil mask to use

#### Defined in

packages/dev/core/src/Engines/engine.ts:885

___

### getStencilFunctionReference

▸ **getStencilFunctionReference**(): `number`

Gets the current stencil reference value

#### Returns

`number`

a number defining the stencil reference value to use

#### Defined in

packages/dev/core/src/Engines/engine.ts:877

___

### getStencilMask

▸ **getStencilMask**(): `number`

Gets the current stencil mask

#### Returns

`number`

a number defining the new stencil mask to use

#### Defined in

packages/dev/core/src/Engines/engine.ts:853

___

### getStencilOperationDepthFail

▸ **getStencilOperationDepthFail**(): `number`

Gets the current stencil operation when depth fails

#### Returns

`number`

a number defining stencil operation to use when depth fails

#### Defined in

packages/dev/core/src/Engines/engine.ts:925

___

### getStencilOperationFail

▸ **getStencilOperationFail**(): `number`

Gets the current stencil operation when stencil fails

#### Returns

`number`

a number defining stencil operation to use when stencil fails

#### Defined in

packages/dev/core/src/Engines/engine.ts:917

___

### getStencilOperationPass

▸ **getStencilOperationPass**(): `number`

Gets the current stencil operation when stencil passes

#### Returns

`number`

a number defining stencil operation to use when stencil passes

#### Defined in

packages/dev/core/src/Engines/engine.ts:933

___

### getTimeStep

▸ **getTimeStep**(): `number`

Returns the time in ms between steps when using deterministic lock step.

#### Returns

`number`

time step in (ms)

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

#### Inherited from

[ThinEngine](ThinEngine.md).[getUniforms](ThinEngine.md#getuniforms)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:3138

___

### getVRDevice

▸ **getVRDevice**(): `any`

Gets the current webVR device

#### Returns

`any`

the current webVR device (or null)

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

[ThinEngine](ThinEngine.md).[getZOffset](ThinEngine.md#getzoffset)

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

[ThinEngine](ThinEngine.md).[getZOffsetUnits](ThinEngine.md#getzoffsetunits)

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

#### Defined in

packages/dev/core/src/Engines/engine.ts:1997

___

### initWebVR

▸ **initWebVR**(): [`Observable`](Observable.md)[`IDisplayChangedEventArgs`](../interfaces/IDisplayChangedEventArgs.md)

Initializes a webVR display and starts listening to display change events
The onVRDisplayChangedObservable will be notified upon these changes

#### Returns

[`Observable`](Observable.md)[`IDisplayChangedEventArgs`](../interfaces/IDisplayChangedEventArgs.md)

The onVRDisplayChangedObservable

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

[ThinEngine](ThinEngine.md).[inlineShaderCode](ThinEngine.md#inlineshadercode)

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

#### Defined in

packages/dev/core/src/Engines/engine.ts:778

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

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.query.ts:56

___

### isVRDevicePresent

▸ **isVRDevicePresent**(): `boolean`

Gets a boolean indicating if a webVR device was detected

#### Returns

`boolean`

true if a webVR device was detected

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.webVR.ts:74

___

### isVRPresenting

▸ **isVRPresenting**(): `boolean`

Gets a boolean indicating that the system is in VR mode and is presenting

#### Returns

`boolean`

true if VR mode is engaged

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

[ThinEngine](ThinEngine.md).[readFromStorageBuffer](ThinEngine.md#readfromstoragebuffer)

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

[ThinEngine](ThinEngine.md).[readPixels](ThinEngine.md#readpixels)

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

[ThinEngine](ThinEngine.md).[recordVertexArrayObject](ThinEngine.md#recordvertexarrayobject)

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

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.views.ts:55

___

### releaseComputeEffects

▸ **releaseComputeEffects**(): `void`

Forces the engine to release all cached compute effects. This means that next effect compilation will have to be done completely even if a similar effect was already compiled

#### Returns

`void`

#### Inherited from

[ThinEngine](ThinEngine.md).[releaseComputeEffects](ThinEngine.md#releasecomputeeffects)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.computeShader.ts:84

___

### releaseEffects

▸ **releaseEffects**(): `void`

Force the engine to release all cached effects. This means that next effect compilation will have to be done completely even if a similar effect was already compiled

#### Returns

`void`

#### Inherited from

[ThinEngine](ThinEngine.md).[releaseEffects](ThinEngine.md#releaseeffects)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:5251

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

[ThinEngine](ThinEngine.md).[releaseVertexArrayObject](ThinEngine.md#releasevertexarrayobject)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:2455

___

### resetTextureCache

▸ **resetTextureCache**(): `void`

Reset the texture cache to empty state

#### Returns

`void`

#### Inherited from

[ThinEngine](ThinEngine.md).[resetTextureCache](ThinEngine.md#resettexturecache)

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

#### Overrides

[ThinEngine](ThinEngine.md).[resize](ThinEngine.md#resize)

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

#### Defined in

packages/dev/core/src/Engines/engine.ts:339

___

### restoreDefaultFramebuffer

▸ **restoreDefaultFramebuffer**(): `void`

Unbind the current render target and bind the default framebuffer

#### Returns

`void`

#### Inherited from

[ThinEngine](ThinEngine.md).[restoreDefaultFramebuffer](ThinEngine.md#restoredefaultframebuffer)

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

[ThinEngine](ThinEngine.md).[restoreSingleAttachment](ThinEngine.md#restoresingleattachment)

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

[ThinEngine](ThinEngine.md).[restoreSingleAttachmentForRenderTarget](ThinEngine.md#restoresingleattachmentforrendertarget)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.multiRender.ts:66

___

### restoreStencilState

▸ **restoreStencilState**(): `void`

Restores the state of the stencil buffer

#### Returns

`void`

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

[ThinEngine](ThinEngine.md).[runRenderLoop](ThinEngine.md#runrenderloop)

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

[ThinEngine](ThinEngine.md).[setAlphaConstants](ThinEngine.md#setalphaconstants)

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

[ThinEngine](ThinEngine.md).[setAlphaEquation](ThinEngine.md#setalphaequation)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.alpha.ts:34

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

#### Inherited from

[ThinEngine](ThinEngine.md).[setAlphaMode](ThinEngine.md#setalphamode)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.alpha.ts:21

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

#### Inherited from

[ThinEngine](ThinEngine.md).[setArray](ThinEngine.md#setarray)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:3335

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

#### Inherited from

[ThinEngine](ThinEngine.md).[setArray2](ThinEngine.md#setarray2)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:3353

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

#### Inherited from

[ThinEngine](ThinEngine.md).[setArray3](ThinEngine.md#setarray3)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:3368

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

#### Inherited from

[ThinEngine](ThinEngine.md).[setArray4](ThinEngine.md#setarray4)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:3383

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

[ThinEngine](ThinEngine.md).[setColorWrite](ThinEngine.md#setcolorwrite)

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

[ThinEngine](ThinEngine.md).[setDepthBuffer](ThinEngine.md#setdepthbuffer)

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

#### Defined in

packages/dev/core/src/Engines/engine.ts:997

___

### setDepthFunctionToGreater

▸ **setDepthFunctionToGreater**(): `void`

Sets the current depth function to GREATER

#### Returns

`void`

#### Defined in

packages/dev/core/src/Engines/engine.ts:1004

___

### setDepthFunctionToGreaterOrEqual

▸ **setDepthFunctionToGreaterOrEqual**(): `void`

Sets the current depth function to GEQUAL

#### Returns

`void`

#### Defined in

packages/dev/core/src/Engines/engine.ts:1011

___

### setDepthFunctionToLess

▸ **setDepthFunctionToLess**(): `void`

Sets the current depth function to LESS

#### Returns

`void`

#### Defined in

packages/dev/core/src/Engines/engine.ts:1018

___

### setDepthFunctionToLessOrEqual

▸ **setDepthFunctionToLessOrEqual**(): `void`

Sets the current depth function to LEQUAL

#### Returns

`void`

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

[ThinEngine](ThinEngine.md).[setExternalTexture](ThinEngine.md#setexternaltexture)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.externalTexture.ts:19

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

#### Inherited from

[ThinEngine](ThinEngine.md).[setFloat](ThinEngine.md#setfloat)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:3443

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

#### Inherited from

[ThinEngine](ThinEngine.md).[setFloat2](ThinEngine.md#setfloat2)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:3460

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

#### Inherited from

[ThinEngine](ThinEngine.md).[setFloat3](ThinEngine.md#setfloat3)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:3478

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

#### Inherited from

[ThinEngine](ThinEngine.md).[setFloat4](ThinEngine.md#setfloat4)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:3497

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

[ThinEngine](ThinEngine.md).[setHardwareScalingLevel](ThinEngine.md#sethardwarescalinglevel)

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

[ThinEngine](ThinEngine.md).[setInt](ThinEngine.md#setint)

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

[ThinEngine](ThinEngine.md).[setInt2](ThinEngine.md#setint2)

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

[ThinEngine](ThinEngine.md).[setInt3](ThinEngine.md#setint3)

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

[ThinEngine](ThinEngine.md).[setInt4](ThinEngine.md#setint4)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:3258

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

#### Inherited from

[ThinEngine](ThinEngine.md).[setIntArray](ThinEngine.md#setintarray)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:3274

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

#### Inherited from

[ThinEngine](ThinEngine.md).[setIntArray2](ThinEngine.md#setintarray2)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:3290

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

#### Inherited from

[ThinEngine](ThinEngine.md).[setIntArray3](ThinEngine.md#setintarray3)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:3305

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

#### Inherited from

[ThinEngine](ThinEngine.md).[setIntArray4](ThinEngine.md#setintarray4)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:3320

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

#### Inherited from

[ThinEngine](ThinEngine.md).[setMatrices](ThinEngine.md#setmatrices)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:3398

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

#### Inherited from

[ThinEngine](ThinEngine.md).[setMatrix2x2](ThinEngine.md#setmatrix2x2)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:3428

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

#### Inherited from

[ThinEngine](ThinEngine.md).[setMatrix3x3](ThinEngine.md#setmatrix3x3)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:3413

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

#### Overrides

[ThinEngine](ThinEngine.md).[setSize](ThinEngine.md#setsize)

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

#### Inherited from

[ThinEngine](ThinEngine.md).[setState](ThinEngine.md#setstate)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1881

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

[ThinEngine](ThinEngine.md).[setStorageBuffer](ThinEngine.md#setstoragebuffer)

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

[ThinEngine](ThinEngine.md).[setTexture](ThinEngine.md#settexture)

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

[ThinEngine](ThinEngine.md).[setTextureArray](ThinEngine.md#settexturearray)

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

[ThinEngine](ThinEngine.md).[setTextureSampler](ThinEngine.md#settexturesampler)

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

#### Inherited from

[ThinEngine](ThinEngine.md).[setViewport](ThinEngine.md#setviewport)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1718

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

[ThinEngine](ThinEngine.md).[setZOffset](ThinEngine.md#setzoffset)

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

[ThinEngine](ThinEngine.md).[setZOffsetUnits](ThinEngine.md#setzoffsetunits)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1943

___

### snapshotRenderingReset

▸ **snapshotRenderingReset**(): `void`

Creates a new snapshot at the next frame using the current snapshotRenderingMode

#### Returns

`void`

#### Inherited from

[ThinEngine](ThinEngine.md).[snapshotRenderingReset](ThinEngine.md#snapshotrenderingreset)

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

[ThinEngine](ThinEngine.md).[stopRenderLoop](ThinEngine.md#stoprenderloop)

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

#### Defined in

packages/dev/core/src/Engines/engine.ts:1356

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

#### Inherited from

[ThinEngine](ThinEngine.md).[unBindFramebuffer](ThinEngine.md#unbindframebuffer)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:1988

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

[ThinEngine](ThinEngine.md).[unBindMultiColorAttachmentFramebuffer](ThinEngine.md#unbindmulticolorattachmentframebuffer)

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

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.views.ts:62

___

### unbindAllAttributes

▸ **unbindAllAttributes**(): `void`

Unbind all vertex attributes from the webGL context

#### Returns

`void`

#### Inherited from

[ThinEngine](ThinEngine.md).[unbindAllAttributes](ThinEngine.md#unbindallattributes)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:5229

___

### unbindAllTextures

▸ **unbindAllTextures**(): `void`

Unbind all textures from the webGL context

#### Returns

`void`

#### Inherited from

[ThinEngine](ThinEngine.md).[unbindAllTextures](ThinEngine.md#unbindalltextures)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:5010

___

### unbindInstanceAttributes

▸ **unbindInstanceAttributes**(): `void`

Unbind all instance attributes

#### Returns

`void`

#### Inherited from

[ThinEngine](ThinEngine.md).[unbindInstanceAttributes](ThinEngine.md#unbindinstanceattributes)

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

[ThinEngine](ThinEngine.md).[updateAndBindInstancesBuffer](ThinEngine.md#updateandbindinstancesbuffer)

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

[ThinEngine](ThinEngine.md).[updateArrayBuffer](ThinEngine.md#updatearraybuffer)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:2191

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

#### Inherited from

[ThinEngine](ThinEngine.md).[updateDynamicIndexBuffer](ThinEngine.md#updatedynamicindexbuffer)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.dynamicBuffer.ts:13

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

#### Inherited from

[ThinEngine](ThinEngine.md).[updateDynamicTexture](ThinEngine.md#updatedynamictexture)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.dynamicTexture.ts:28

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

#### Inherited from

[ThinEngine](ThinEngine.md).[updateDynamicVertexBuffer](ThinEngine.md#updatedynamicvertexbuffer)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.dynamicBuffer.ts:22

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

[ThinEngine](ThinEngine.md).[updateMultipleRenderTargetTextureSampleCount](ThinEngine.md#updatemultiplerendertargettexturesamplecount)

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

[ThinEngine](ThinEngine.md).[updateRawCubeTexture](ThinEngine.md#updaterawcubetexture)

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

[ThinEngine](ThinEngine.md).[updateRawCubeTexture](ThinEngine.md#updaterawcubetexture)

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

[ThinEngine](ThinEngine.md).[updateRawCubeTexture](ThinEngine.md#updaterawcubetexture)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.rawTexture.ts:124

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

#### Inherited from

[ThinEngine](ThinEngine.md).[updateRawTexture](ThinEngine.md#updaterawtexture)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.rawTexture.ts:48

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

#### Inherited from

[ThinEngine](ThinEngine.md).[updateRawTexture](ThinEngine.md#updaterawtexture)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.rawTexture.ts:60

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

[ThinEngine](ThinEngine.md).[updateRawTexture2DArray](ThinEngine.md#updaterawtexture2darray)

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

[ThinEngine](ThinEngine.md).[updateRawTexture2DArray](ThinEngine.md#updaterawtexture2darray)

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

[ThinEngine](ThinEngine.md).[updateRawTexture3D](ThinEngine.md#updaterawtexture3d)

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

[ThinEngine](ThinEngine.md).[updateRawTexture3D](ThinEngine.md#updaterawtexture3d)

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

[ThinEngine](ThinEngine.md).[updateRenderTargetTextureSampleCount](ThinEngine.md#updaterendertargettexturesamplecount)

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

[ThinEngine](ThinEngine.md).[updateStorageBuffer](ThinEngine.md#updatestoragebuffer)

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

[ThinEngine](ThinEngine.md).[updateTextureData](ThinEngine.md#updatetexturedata)

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

[ThinEngine](ThinEngine.md).[updateTextureDimensions](ThinEngine.md#updatetexturedimensions)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:4431

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

#### Inherited from

[ThinEngine](ThinEngine.md).[updateTextureSamplingMode](ThinEngine.md#updatetexturesamplingmode)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:4407

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

[ThinEngine](ThinEngine.md).[updateTextureWrappingMode](ThinEngine.md#updatetexturewrappingmode)

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

[ThinEngine](ThinEngine.md).[updateUniformBuffer](ThinEngine.md#updateuniformbuffer)

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

[ThinEngine](ThinEngine.md).[updateVideoTexture](ThinEngine.md#updatevideotexture)

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

#### Inherited from

[ThinEngine](ThinEngine.md).[wipeCaches](ThinEngine.md#wipecaches)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:3586

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

[ThinEngine](ThinEngine.md).[CeilingPOT](ThinEngine.md#ceilingpot)

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

[ThinEngine](ThinEngine.md).[FloorPOT](ThinEngine.md#floorpot)

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

[ThinEngine](ThinEngine.md).[GetExponentOfTwo](ThinEngine.md#getexponentoftwo)

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

[ThinEngine](ThinEngine.md).[NearestPOT](ThinEngine.md#nearestpot)

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

[ThinEngine](ThinEngine.md).[QueueNewFrame](ThinEngine.md#queuenewframe)

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

[ThinEngine](ThinEngine.md).[_ConcatenateShader](ThinEngine.md#_concatenateshader)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:2837

___

### \_ExitFullscreen

▸ `Static` **_ExitFullscreen**(): `void`

Asks the browser to exit fullscreen mode

#### Returns

`void`

#### Defined in

packages/dev/core/src/Engines/engine.ts:2094

___

### \_ExitPointerlock

▸ `Static` **_ExitPointerlock**(): `void`

Asks the browser to exit pointerlock mode

#### Returns

`void`

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

[ThinEngine](ThinEngine.md).[isSupported](ThinEngine.md#issupported-1)

#### Defined in

packages/dev/core/src/Engines/thinEngine.ts:5811
