[@dev/core](../README.md) / [Exports](../modules.md) / MirrorTexture

# Class: MirrorTexture

Mirror texture can be used to simulate the view from a mirror in a scene.
It will dynamically be rendered every frame to adapt to the camera point of view.
You can then easily use it as a reflectionTexture on a flat surface.
In case the surface is not a plane, please consider relying on reflection probes.

**`See`**

https://doc.babylonjs.com/how_to/reflect#mirrors

## Hierarchy

- [`RenderTargetTexture`](RenderTargetTexture.md)

  ↳ **`MirrorTexture`**

## Table of contents

### Constructors

- [constructor](MirrorTexture.md#constructor)

### Properties

- [\_adaptiveBlurKernel](MirrorTexture.md#_adaptiveblurkernel)
- [\_blurKernelX](MirrorTexture.md#_blurkernelx)
- [\_blurKernelY](MirrorTexture.md#_blurkernely)
- [\_blurRatio](MirrorTexture.md#_blurratio)
- [\_blurX](MirrorTexture.md#_blurx)
- [\_blurY](MirrorTexture.md#_blury)
- [\_coordinatesIndex](MirrorTexture.md#_coordinatesindex)
- [\_coordinatesMode](MirrorTexture.md#_coordinatesmode)
- [\_currentRefreshId](MirrorTexture.md#_currentrefreshid)
- [\_currentSceneUBO](MirrorTexture.md#_currentsceneubo)
- [\_doNotChangeAspectRatio](MirrorTexture.md#_donotchangeaspectratio)
- [\_engine](MirrorTexture.md#_engine)
- [\_errorObject](MirrorTexture.md#_errorobject)
- [\_format](MirrorTexture.md#_format)
- [\_imageProcessingConfigChangeObserver](MirrorTexture.md#_imageprocessingconfigchangeobserver)
- [\_initialSizeParameter](MirrorTexture.md#_initialsizeparameter)
- [\_isBlocking](MirrorTexture.md#_isblocking)
- [\_loadingError](MirrorTexture.md#_loadingerror)
- [\_mirrorMatrix](MirrorTexture.md#_mirrormatrix)
- [\_refreshRate](MirrorTexture.md#_refreshrate)
- [\_renderTarget](MirrorTexture.md#_rendertarget)
- [\_renderTargetOptions](MirrorTexture.md#_rendertargetoptions)
- [\_renderingManager](MirrorTexture.md#_renderingmanager)
- [\_samples](MirrorTexture.md#_samples)
- [\_scene](MirrorTexture.md#_scene)
- [\_sceneUBO](MirrorTexture.md#_sceneubo)
- [\_size](MirrorTexture.md#_size)
- [\_sizeRatio](MirrorTexture.md#_sizeratio)
- [\_textureMatrix](MirrorTexture.md#_texturematrix)
- [\_transformMatrix](MirrorTexture.md#_transformmatrix)
- [\_wrapU](MirrorTexture.md#_wrapu)
- [\_wrapV](MirrorTexture.md#_wrapv)
- [activeCamera](MirrorTexture.md#activecamera)
- [animations](MirrorTexture.md#animations)
- [anisotropicFilteringLevel](MirrorTexture.md#anisotropicfilteringlevel)
- [boundingBoxPosition](MirrorTexture.md#boundingboxposition)
- [clearColor](MirrorTexture.md#clearcolor)
- [customIsReadyFunction](MirrorTexture.md#customisreadyfunction)
- [customRenderFunction](MirrorTexture.md#customrenderfunction)
- [delayLoadState](MirrorTexture.md#delayloadstate)
- [getCustomRenderList](MirrorTexture.md#getcustomrenderlist)
- [homogeneousRotationInUVTransform](MirrorTexture.md#homogeneousrotationinuvtransform)
- [ignoreCameraViewport](MirrorTexture.md#ignorecameraviewport)
- [inspectableCustomProperties](MirrorTexture.md#inspectablecustomproperties)
- [invertZ](MirrorTexture.md#invertz)
- [isRenderTarget](MirrorTexture.md#isrendertarget)
- [level](MirrorTexture.md#level)
- [metadata](MirrorTexture.md#metadata)
- [mirrorPlane](MirrorTexture.md#mirrorplane)
- [name](MirrorTexture.md#name)
- [onAfterRenderObservable](MirrorTexture.md#onafterrenderobservable)
- [onAfterUnbindObservable](MirrorTexture.md#onafterunbindobservable)
- [onBeforeBindObservable](MirrorTexture.md#onbeforebindobservable)
- [onBeforeRenderObservable](MirrorTexture.md#onbeforerenderobservable)
- [onClearObservable](MirrorTexture.md#onclearobservable)
- [onDisposeObservable](MirrorTexture.md#ondisposeobservable)
- [onLoadObservable](MirrorTexture.md#onloadobservable)
- [onResizeObservable](MirrorTexture.md#onresizeobservable)
- [renderListPredicate](MirrorTexture.md#renderlistpredicate)
- [renderParticles](MirrorTexture.md#renderparticles)
- [renderPassId](MirrorTexture.md#renderpassid)
- [renderSprites](MirrorTexture.md#rendersprites)
- [reservedDataStore](MirrorTexture.md#reserveddatastore)
- [skipInitialClear](MirrorTexture.md#skipinitialclear)
- [sphericalPolynomial](MirrorTexture.md#sphericalpolynomial)
- [uAng](MirrorTexture.md#uang)
- [uOffset](MirrorTexture.md#uoffset)
- [uRotationCenter](MirrorTexture.md#urotationcenter)
- [uScale](MirrorTexture.md#uscale)
- [uniqueId](MirrorTexture.md#uniqueid)
- [url](MirrorTexture.md#url)
- [useCameraPostProcesses](MirrorTexture.md#usecamerapostprocesses)
- [vAng](MirrorTexture.md#vang)
- [vOffset](MirrorTexture.md#voffset)
- [vRotationCenter](MirrorTexture.md#vrotationcenter)
- [vScale](MirrorTexture.md#vscale)
- [wAng](MirrorTexture.md#wang)
- [wRotationCenter](MirrorTexture.md#wrotationcenter)
- [wrapR](MirrorTexture.md#wrapr)
- [BILINEAR\_SAMPLINGMODE](MirrorTexture.md#bilinear_samplingmode)
- [CLAMP\_ADDRESSMODE](MirrorTexture.md#clamp_addressmode)
- [CUBIC\_MODE](MirrorTexture.md#cubic_mode)
- [DEFAULT\_ANISOTROPIC\_FILTERING\_LEVEL](MirrorTexture.md#default_anisotropic_filtering_level)
- [EQUIRECTANGULAR\_MODE](MirrorTexture.md#equirectangular_mode)
- [EXPLICIT\_MODE](MirrorTexture.md#explicit_mode)
- [FIXED\_EQUIRECTANGULAR\_MIRRORED\_MODE](MirrorTexture.md#fixed_equirectangular_mirrored_mode)
- [FIXED\_EQUIRECTANGULAR\_MODE](MirrorTexture.md#fixed_equirectangular_mode)
- [ForceSerializeBuffers](MirrorTexture.md#forceserializebuffers)
- [INVCUBIC\_MODE](MirrorTexture.md#invcubic_mode)
- [LINEAR\_LINEAR](MirrorTexture.md#linear_linear)
- [LINEAR\_LINEAR\_MIPLINEAR](MirrorTexture.md#linear_linear_miplinear)
- [LINEAR\_LINEAR\_MIPNEAREST](MirrorTexture.md#linear_linear_mipnearest)
- [LINEAR\_NEAREST](MirrorTexture.md#linear_nearest)
- [LINEAR\_NEAREST\_MIPLINEAR](MirrorTexture.md#linear_nearest_miplinear)
- [LINEAR\_NEAREST\_MIPNEAREST](MirrorTexture.md#linear_nearest_mipnearest)
- [MIRROR\_ADDRESSMODE](MirrorTexture.md#mirror_addressmode)
- [NEAREST\_LINEAR](MirrorTexture.md#nearest_linear)
- [NEAREST\_LINEAR\_MIPLINEAR](MirrorTexture.md#nearest_linear_miplinear)
- [NEAREST\_LINEAR\_MIPNEAREST](MirrorTexture.md#nearest_linear_mipnearest)
- [NEAREST\_NEAREST](MirrorTexture.md#nearest_nearest)
- [NEAREST\_NEAREST\_MIPLINEAR](MirrorTexture.md#nearest_nearest_miplinear)
- [NEAREST\_NEAREST\_MIPNEAREST](MirrorTexture.md#nearest_nearest_mipnearest)
- [NEAREST\_SAMPLINGMODE](MirrorTexture.md#nearest_samplingmode)
- [OnTextureLoadErrorObservable](MirrorTexture.md#ontextureloaderrorobservable)
- [PLANAR\_MODE](MirrorTexture.md#planar_mode)
- [PROJECTION\_MODE](MirrorTexture.md#projection_mode)
- [REFRESHRATE\_RENDER\_ONCE](MirrorTexture.md#refreshrate_render_once)
- [REFRESHRATE\_RENDER\_ONEVERYFRAME](MirrorTexture.md#refreshrate_render_oneveryframe)
- [REFRESHRATE\_RENDER\_ONEVERYTWOFRAMES](MirrorTexture.md#refreshrate_render_oneverytwoframes)
- [SKYBOX\_MODE](MirrorTexture.md#skybox_mode)
- [SPHERICAL\_MODE](MirrorTexture.md#spherical_mode)
- [SerializeBuffers](MirrorTexture.md#serializebuffers)
- [TRILINEAR\_SAMPLINGMODE](MirrorTexture.md#trilinear_samplingmode)
- [UseSerializedUrlIfAny](MirrorTexture.md#useserializedurlifany)
- [WRAP\_ADDRESSMODE](MirrorTexture.md#wrap_addressmode)

### Accessors

- [\_prePassEnabled](MirrorTexture.md#_prepassenabled)
- [adaptiveBlurKernel](MirrorTexture.md#adaptiveblurkernel)
- [blurKernel](MirrorTexture.md#blurkernel)
- [blurKernelX](MirrorTexture.md#blurkernelx)
- [blurKernelY](MirrorTexture.md#blurkernely)
- [blurRatio](MirrorTexture.md#blurratio)
- [boundingBoxSize](MirrorTexture.md#boundingboxsize)
- [canRescale](MirrorTexture.md#canrescale)
- [coordinatesIndex](MirrorTexture.md#coordinatesindex)
- [coordinatesMode](MirrorTexture.md#coordinatesmode)
- [currentRefreshId](MirrorTexture.md#currentrefreshid)
- [depthStencilTexture](MirrorTexture.md#depthstenciltexture)
- [errorObject](MirrorTexture.md#errorobject)
- [gammaSpace](MirrorTexture.md#gammaspace)
- [getAlphaFromRGB](MirrorTexture.md#getalphafromrgb)
- [hasAlpha](MirrorTexture.md#hasalpha)
- [invertY](MirrorTexture.md#inverty)
- [irradianceTexture](MirrorTexture.md#irradiancetexture)
- [is2DArray](MirrorTexture.md#is2darray)
- [is3D](MirrorTexture.md#is3d)
- [isBlocking](MirrorTexture.md#isblocking)
- [isCube](MirrorTexture.md#iscube)
- [isRGBD](MirrorTexture.md#isrgbd)
- [linearSpecularLOD](MirrorTexture.md#linearspecularlod)
- [loadingError](MirrorTexture.md#loadingerror)
- [lodGenerationOffset](MirrorTexture.md#lodgenerationoffset)
- [lodGenerationScale](MirrorTexture.md#lodgenerationscale)
- [mimeType](MirrorTexture.md#mimetype)
- [noMipmap](MirrorTexture.md#nomipmap)
- [onAfterRender](MirrorTexture.md#onafterrender)
- [onAfterUnbind](MirrorTexture.md#onafterunbind)
- [onBeforeRender](MirrorTexture.md#onbeforerender)
- [onClear](MirrorTexture.md#onclear)
- [onDispose](MirrorTexture.md#ondispose)
- [postProcesses](MirrorTexture.md#postprocesses)
- [refreshRate](MirrorTexture.md#refreshrate)
- [renderList](MirrorTexture.md#renderlist)
- [renderPassIds](MirrorTexture.md#renderpassids)
- [renderTarget](MirrorTexture.md#rendertarget)
- [renderTargetOptions](MirrorTexture.md#rendertargetoptions)
- [samples](MirrorTexture.md#samples)
- [samplingMode](MirrorTexture.md#samplingmode)
- [textureFormat](MirrorTexture.md#textureformat)
- [textureType](MirrorTexture.md#texturetype)
- [uid](MirrorTexture.md#uid)
- [wrapU](MirrorTexture.md#wrapu)
- [wrapV](MirrorTexture.md#wrapv)

### Methods

- [\_autoComputeBlurKernel](MirrorTexture.md#_autocomputeblurkernel)
- [\_markAllSubMeshesAsTexturesDirty](MirrorTexture.md#_markallsubmeshesastexturesdirty)
- [\_onRatioRescale](MirrorTexture.md#_onratiorescale)
- [\_preparePostProcesses](MirrorTexture.md#_preparepostprocesses)
- [\_unbindFrameBuffer](MirrorTexture.md#_unbindframebuffer)
- [\_updateGammaSpace](MirrorTexture.md#_updategammaspace)
- [addPostProcess](MirrorTexture.md#addpostprocess)
- [checkTransformsAreIdentical](MirrorTexture.md#checktransformsareidentical)
- [clearPostProcesses](MirrorTexture.md#clearpostprocesses)
- [clone](MirrorTexture.md#clone)
- [createDepthStencilTexture](MirrorTexture.md#createdepthstenciltexture)
- [disableRescaling](MirrorTexture.md#disablerescaling)
- [dispose](MirrorTexture.md#dispose)
- [disposeFramebufferObjects](MirrorTexture.md#disposeframebufferobjects)
- [forceSphericalPolynomialsRecompute](MirrorTexture.md#forcesphericalpolynomialsrecompute)
- [freeRenderingGroups](MirrorTexture.md#freerenderinggroups)
- [getBaseSize](MirrorTexture.md#getbasesize)
- [getClassName](MirrorTexture.md#getclassname)
- [getInternalTexture](MirrorTexture.md#getinternaltexture)
- [getReflectionTextureMatrix](MirrorTexture.md#getreflectiontexturematrix)
- [getRenderHeight](MirrorTexture.md#getrenderheight)
- [getRenderLayers](MirrorTexture.md#getrenderlayers)
- [getRenderSize](MirrorTexture.md#getrendersize)
- [getRenderWidth](MirrorTexture.md#getrenderwidth)
- [getScene](MirrorTexture.md#getscene)
- [getSize](MirrorTexture.md#getsize)
- [getTextureMatrix](MirrorTexture.md#gettexturematrix)
- [getViewCount](MirrorTexture.md#getviewcount)
- [isReady](MirrorTexture.md#isready)
- [isReadyForRendering](MirrorTexture.md#isreadyforrendering)
- [isReadyOrNotBlocking](MirrorTexture.md#isreadyornotblocking)
- [readPixels](MirrorTexture.md#readpixels)
- [releaseInternalTexture](MirrorTexture.md#releaseinternaltexture)
- [removePostProcess](MirrorTexture.md#removepostprocess)
- [render](MirrorTexture.md#render)
- [resetRefreshCounter](MirrorTexture.md#resetrefreshcounter)
- [resize](MirrorTexture.md#resize)
- [scale](MirrorTexture.md#scale)
- [serialize](MirrorTexture.md#serialize)
- [setMaterialForRendering](MirrorTexture.md#setmaterialforrendering)
- [setRenderingAutoClearDepthStencil](MirrorTexture.md#setrenderingautocleardepthstencil)
- [setRenderingOrder](MirrorTexture.md#setrenderingorder)
- [toString](MirrorTexture.md#tostring)
- [updateSamplingMode](MirrorTexture.md#updatesamplingmode)
- [updateURL](MirrorTexture.md#updateurl)
- [CreateFromBase64String](MirrorTexture.md#createfrombase64string)
- [LoadFromDataString](MirrorTexture.md#loadfromdatastring)
- [Parse](MirrorTexture.md#parse)
- [WhenAllReady](MirrorTexture.md#whenallready)

## Constructors

### constructor

• **new MirrorTexture**(`name`, `size`, `scene?`, `generateMipMaps?`, `type?`, `samplingMode?`, `generateDepthBuffer?`)

Instantiates a Mirror Texture.
Mirror texture can be used to simulate the view from a mirror in a scene.
It will dynamically be rendered every frame to adapt to the camera point of view.
You can then easily use it as a reflectionTexture on a flat surface.
In case the surface is not a plane, please consider relying on reflection probes.

**`See`**

https://doc.babylonjs.com/how_to/reflect#mirrors

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `name` | `string` | `undefined` |
| `size` | `number` \| { `height`: `number` ; `width`: `number`  } \| { `ratio`: `number`  } | `undefined` |
| `scene?` | [`Scene`](Scene.md) | `undefined` |
| `generateMipMaps?` | `boolean` | `undefined` |
| `type` | `number` | `Constants.TEXTURETYPE_UNSIGNED_INT` |
| `samplingMode` | `number` | `Texture.BILINEAR_SAMPLINGMODE` |
| `generateDepthBuffer` | `boolean` | `true` |

#### Overrides

[RenderTargetTexture](RenderTargetTexture.md).[constructor](RenderTargetTexture.md#constructor)

#### Defined in

packages/dev/core/src/Materials/Textures/mirrorTexture.ts:157

## Properties

### \_adaptiveBlurKernel

• `Private` **\_adaptiveBlurKernel**: `number` = `0`

#### Defined in

packages/dev/core/src/Materials/Textures/mirrorTexture.ts:135

___

### \_blurKernelX

• `Private` **\_blurKernelX**: `number` = `0`

#### Defined in

packages/dev/core/src/Materials/Textures/mirrorTexture.ts:136

___

### \_blurKernelY

• `Private` **\_blurKernelY**: `number` = `0`

#### Defined in

packages/dev/core/src/Materials/Textures/mirrorTexture.ts:137

___

### \_blurRatio

• `Private` **\_blurRatio**: `number` = `1.0`

#### Defined in

packages/dev/core/src/Materials/Textures/mirrorTexture.ts:138

___

### \_blurX

• `Private` **\_blurX**: [`Nullable`](../modules.md#nullable)[`BlurPostProcess`](BlurPostProcess.md)

#### Defined in

packages/dev/core/src/Materials/Textures/mirrorTexture.ts:133

___

### \_blurY

• `Private` **\_blurY**: [`Nullable`](../modules.md#nullable)[`BlurPostProcess`](BlurPostProcess.md)

#### Defined in

packages/dev/core/src/Materials/Textures/mirrorTexture.ts:134

___

### \_coordinatesIndex

• `Protected` **\_coordinatesIndex**: `number` = `0`

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[_coordinatesIndex](RenderTargetTexture.md#_coordinatesindex)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:104

___

### \_coordinatesMode

• `Protected` **\_coordinatesMode**: `number` = `Constants.TEXTURE_EXPLICIT_MODE`

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[_coordinatesMode](RenderTargetTexture.md#_coordinatesmode)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:126

___

### \_currentRefreshId

• `Protected` **\_currentRefreshId**: `number` = `-1`

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[_currentRefreshId](RenderTargetTexture.md#_currentrefreshid)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:259

___

### \_currentSceneUBO

• `Private` **\_currentSceneUBO**: [`UniformBuffer`](UniformBuffer.md)

#### Defined in

packages/dev/core/src/Materials/Textures/mirrorTexture.ts:140

___

### \_doNotChangeAspectRatio

• `Protected` **\_doNotChangeAspectRatio**: `boolean`

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[_doNotChangeAspectRatio](RenderTargetTexture.md#_donotchangeaspectratio)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:258

___

### \_engine

• `Protected` **\_engine**: [`Nullable`](../modules.md#nullable)[`ThinEngine`](ThinEngine.md) = `null`

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[_engine](RenderTargetTexture.md#_engine)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:144

___

### \_errorObject

• `Protected` `Optional` **\_errorObject**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `exception?` | `any` |
| `message?` | `string` |

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[_errorObject](RenderTargetTexture.md#_errorobject)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:483

___

### \_format

• `Protected` **\_format**: [`Nullable`](../modules.md#nullable)`number` = `null`

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[_format](RenderTargetTexture.md#_format)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:312

___

### \_imageProcessingConfigChangeObserver

• `Private` **\_imageProcessingConfigChangeObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`ImageProcessingConfiguration`](ImageProcessingConfiguration.md)

#### Defined in

packages/dev/core/src/Materials/Textures/mirrorTexture.ts:128

___

### \_initialSizeParameter

• `Protected` **\_initialSizeParameter**: `number` \| { `height`: `number` ; `width`: `number`  } \| { `ratio`: `number`  }

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[_initialSizeParameter](RenderTargetTexture.md#_initialsizeparameter)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:245

___

### \_isBlocking

• `Protected` **\_isBlocking**: `boolean` = `true`

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[_isBlocking](RenderTargetTexture.md#_isblocking)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:331

___

### \_loadingError

• `Protected` **\_loadingError**: `boolean` = `false`

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[_loadingError](RenderTargetTexture.md#_loadingerror)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:482

___

### \_mirrorMatrix

• `Private` **\_mirrorMatrix**: [`Matrix`](Matrix.md)

#### Defined in

packages/dev/core/src/Materials/Textures/mirrorTexture.ts:131

___

### \_refreshRate

• `Protected` **\_refreshRate**: `number` = `1`

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[_refreshRate](RenderTargetTexture.md#_refreshrate)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:260

___

### \_renderTarget

• `Protected` **\_renderTarget**: [`Nullable`](../modules.md#nullable)[`RenderTargetWrapper`](RenderTargetWrapper.md) = `null`

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[_renderTarget](RenderTargetTexture.md#_rendertarget)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:265

___

### \_renderTargetOptions

• `Protected` **\_renderTargetOptions**: `RenderTargetCreationOptions`

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[_renderTargetOptions](RenderTargetTexture.md#_rendertargetoptions)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:263

___

### \_renderingManager

• `Protected` **\_renderingManager**: [`RenderingManager`](RenderingManager.md)

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[_renderingManager](RenderTargetTexture.md#_renderingmanager)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:255

___

### \_samples

• `Protected` **\_samples**: `number` = `1`

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[_samples](RenderTargetTexture.md#_samples)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:262

___

### \_scene

• `Protected` **\_scene**: [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) = `null`

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[_scene](RenderTargetTexture.md#_scene)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:466

___

### \_sceneUBO

• `Private` **\_sceneUBO**: [`UniformBuffer`](UniformBuffer.md)

#### Defined in

packages/dev/core/src/Materials/Textures/mirrorTexture.ts:139

___

### \_size

• `Protected` **\_size**: `TextureSize`

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[_size](RenderTargetTexture.md#_size)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:244

___

### \_sizeRatio

• `Protected` **\_sizeRatio**: [`Nullable`](../modules.md#nullable)`number`

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[_sizeRatio](RenderTargetTexture.md#_sizeratio)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:246

___

### \_textureMatrix

• `Protected` **\_textureMatrix**: [`Matrix`](Matrix.md)

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[_textureMatrix](RenderTargetTexture.md#_texturematrix)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:261

___

### \_transformMatrix

• `Private` **\_transformMatrix**: [`Matrix`](Matrix.md)

#### Defined in

packages/dev/core/src/Materials/Textures/mirrorTexture.ts:130

___

### \_wrapU

• `Protected` **\_wrapU**: `number` = `Constants.TEXTURE_WRAP_ADDRESSMODE`

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[_wrapU](RenderTargetTexture.md#_wrapu)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:15

___

### \_wrapV

• `Protected` **\_wrapV**: `number` = `Constants.TEXTURE_WRAP_ADDRESSMODE`

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[_wrapV](RenderTargetTexture.md#_wrapv)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:31

___

### activeCamera

• **activeCamera**: [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md)

Define the camera used to render the texture.

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[activeCamera](RenderTargetTexture.md#activecamera)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:123

___

### animations

• **animations**: [`Animation`](Animation.md)[]

Define the list of animation attached to the texture.

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[animations](RenderTargetTexture.md#animations)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:447

___

### anisotropicFilteringLevel

• **anisotropicFilteringLevel**: `number` = `BaseTexture.DEFAULT_ANISOTROPIC_FILTERING_LEVEL`

With compliant hardware and browser (supporting anisotropic filtering)
this defines the level of anisotropic filtering in the texture.
The higher the better but the slower. This defaults to 4 as it seems to be the best tradeoff.

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[anisotropicFilteringLevel](RenderTargetTexture.md#anisotropicfilteringlevel)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:205

___

### boundingBoxPosition

• **boundingBoxPosition**: [`Vector3`](Vector3.md)

Gets or sets the center of the bounding box associated with the texture (when in cube mode)
It must define where the camera used to render the texture is set

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[boundingBoxPosition](RenderTargetTexture.md#boundingboxposition)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:330

___

### clearColor

• **clearColor**: [`Color4`](Color4.md)

Define the clear color of the Render Target if it should be different from the scene.

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[clearColor](RenderTargetTexture.md#clearcolor)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:243

___

### customIsReadyFunction

• **customIsReadyFunction**: (`mesh`: [`AbstractMesh`](AbstractMesh.md), `refreshRate`: `number`) => `boolean`

#### Type declaration

▸ (`mesh`, `refreshRate`): `boolean`

Override the mesh isReady function with your own one.

##### Parameters

| Name | Type |
| :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) |
| `refreshRate` | `number` |

##### Returns

`boolean`

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[customIsReadyFunction](RenderTargetTexture.md#customisreadyfunction)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:127

___

### customRenderFunction

• **customRenderFunction**: (`opaqueSubMeshes`: [`SmartArray`](SmartArray.md)[`SubMesh`](SubMesh.md), `alphaTestSubMeshes`: [`SmartArray`](SmartArray.md)[`SubMesh`](SubMesh.md), `transparentSubMeshes`: [`SmartArray`](SmartArray.md)[`SubMesh`](SubMesh.md), `depthOnlySubMeshes`: [`SmartArray`](SmartArray.md)[`SubMesh`](SubMesh.md), `beforeTransparents?`: () => `void`) => `void`

#### Type declaration

▸ (`opaqueSubMeshes`, `alphaTestSubMeshes`, `transparentSubMeshes`, `depthOnlySubMeshes`, `beforeTransparents?`): `void`

Override the render function of the texture with your own one.

##### Parameters

| Name | Type |
| :------ | :------ |
| `opaqueSubMeshes` | [`SmartArray`](SmartArray.md)[`SubMesh`](SubMesh.md) |
| `alphaTestSubMeshes` | [`SmartArray`](SmartArray.md)[`SubMesh`](SubMesh.md) |
| `transparentSubMeshes` | [`SmartArray`](SmartArray.md)[`SubMesh`](SubMesh.md) |
| `depthOnlySubMeshes` | [`SmartArray`](SmartArray.md)[`SubMesh`](SubMesh.md) |
| `beforeTransparents?` | () => `void` |

##### Returns

`void`

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[customRenderFunction](RenderTargetTexture.md#customrenderfunction)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:131

___

### delayLoadState

• **delayLoadState**: `number` = `Constants.DELAYLOADSTATE_NONE`

Define the current state of the loading sequence when in delayed load mode.

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[delayLoadState](RenderTargetTexture.md#delayloadstate)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:66

___

### getCustomRenderList

• **getCustomRenderList**: (`layerOrFace`: `number`, `renderList`: [`Nullable`](../modules.md#nullable)readonly [`AbstractMesh`](AbstractMesh.md)[], `renderListLength`: `number`) => [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)[]

#### Type declaration

▸ (`layerOrFace`, `renderList`, `renderListLength`): [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)[]

Use this function to overload the renderList array at rendering time.
Return null to render with the current renderList, else return the list of meshes to use for rendering.
For 2DArray RTT, layerOrFace is the index of the layer that is going to be rendered, else it is the faceIndex of
the cube (if the RTT is a cube, else layerOrFace=0).
The renderList passed to the function is the current render list (the one that will be used if the function returns null).
The length of this list is passed through renderListLength: don't use renderList.length directly because the array can
hold dummy elements!

##### Parameters

| Name | Type |
| :------ | :------ |
| `layerOrFace` | `number` |
| `renderList` | [`Nullable`](../modules.md#nullable)readonly [`AbstractMesh`](AbstractMesh.md)[] |
| `renderListLength` | `number` |

##### Returns

[`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)[]

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[getCustomRenderList](RenderTargetTexture.md#getcustomrenderlist)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:78

___

### homogeneousRotationInUVTransform

• **homogeneousRotationInUVTransform**: `boolean` = `false`

Sets this property to true to avoid deformations when rotating the texture with non-uniform scaling

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[homogeneousRotationInUVTransform](RenderTargetTexture.md#homogeneousrotationinuvtransform)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:270

___

### ignoreCameraViewport

• **ignoreCameraViewport**: `boolean` = `false`

Define if the camera viewport should be respected while rendering the texture or if the render should be done to the entire texture.

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[ignoreCameraViewport](RenderTargetTexture.md#ignorecameraviewport)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:145

___

### inspectableCustomProperties

• **inspectableCustomProperties**: [`Nullable`](../modules.md#nullable)[`IInspectable`](../interfaces/IInspectable.md)[] = `null`

List of inspectable custom properties (used by the Inspector)

**`See`**

https://doc.babylonjs.com/how_to/debug_layer#extensibility

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[inspectableCustomProperties](RenderTargetTexture.md#inspectablecustomproperties)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:283

___

### invertZ

• **invertZ**: `boolean` = `false`

Is Z inverted in the texture (useful in a cube texture).

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[invertZ](RenderTargetTexture.md#invertz)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:320

___

### isRenderTarget

• **isRenderTarget**: `boolean` = `false`

Define if the texture is a render target.

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[isRenderTarget](RenderTargetTexture.md#isrendertarget)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:411

___

### level

• **level**: `number` = `1`

Intensity or strength of the texture.
It is commonly used by materials to fine tune the intensity of the texture

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[level](RenderTargetTexture.md#level)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:101

___

### metadata

• **metadata**: `any` = `null`

Gets or sets an object used to store user defined information.

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[metadata](RenderTargetTexture.md#metadata)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:48

___

### mirrorPlane

• **mirrorPlane**: [`Plane`](Plane.md)

Define the reflection plane we want to use. The mirrorPlane is usually set to the constructed reflector.
It is possible to directly set the mirrorPlane by directly using a Plane(a, b, c, d) where a, b and c give the plane normal vector (a, b, c) and d is a scalar displacement from the mirrorPlane to the origin. However in all but the very simplest of situations it is more straight forward to set it to the reflector as stated in the doc.

**`See`**

https://doc.babylonjs.com/how_to/reflect#mirrors

#### Defined in

packages/dev/core/src/Materials/Textures/mirrorTexture.ts:26

___

### name

• **name**: `string`

Define the name of the texture.

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[name](RenderTargetTexture.md#name)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:42

___

### onAfterRenderObservable

• **onAfterRenderObservable**: [`Observable`](Observable.md)`number`

An event triggered after rendering the texture

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[onAfterRenderObservable](RenderTargetTexture.md#onafterrenderobservable)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:204

___

### onAfterUnbindObservable

• **onAfterUnbindObservable**: [`Observable`](Observable.md)[`RenderTargetTexture`](RenderTargetTexture.md)

An event triggered when the texture is unbind.

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[onAfterUnbindObservable](RenderTargetTexture.md#onafterunbindobservable)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:170

___

### onBeforeBindObservable

• **onBeforeBindObservable**: [`Observable`](Observable.md)[`RenderTargetTexture`](RenderTargetTexture.md)

An event triggered when the texture is unbind.

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[onBeforeBindObservable](RenderTargetTexture.md#onbeforebindobservable)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:165

___

### onBeforeRenderObservable

• **onBeforeRenderObservable**: [`Observable`](Observable.md)`number`

An event triggered before rendering the texture

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[onBeforeRenderObservable](RenderTargetTexture.md#onbeforerenderobservable)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:187

___

### onClearObservable

• **onClearObservable**: [`Observable`](Observable.md)[`Engine`](Engine.md)

An event triggered after the texture clear

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[onClearObservable](RenderTargetTexture.md#onclearobservable)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:221

___

### onDisposeObservable

• **onDisposeObservable**: [`Observable`](Observable.md)[`BaseTexture`](BaseTexture.md)

An event triggered when the texture is disposed.

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[onDisposeObservable](RenderTargetTexture.md#ondisposeobservable)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:452

___

### onLoadObservable

• **onLoadObservable**: [`Observable`](Observable.md)[`Texture`](Texture.md)

Observable triggered once the texture has been loaded.

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[onLoadObservable](RenderTargetTexture.md#onloadobservable)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:329

___

### onResizeObservable

• **onResizeObservable**: [`Observable`](Observable.md)[`RenderTargetTexture`](RenderTargetTexture.md)

An event triggered when the texture is resized.

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[onResizeObservable](RenderTargetTexture.md#onresizeobservable)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:238

___

### renderListPredicate

• **renderListPredicate**: (`AbstractMesh`: [`AbstractMesh`](AbstractMesh.md)) => `boolean`

#### Type declaration

▸ (`AbstractMesh`): `boolean`

Use this predicate to dynamically define the list of mesh you want to render.
If set, the renderList property will be overwritten.

##### Parameters

| Name | Type |
| :------ | :------ |
| `AbstractMesh` | [`AbstractMesh`](AbstractMesh.md) |

##### Returns

`boolean`

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[renderListPredicate](RenderTargetTexture.md#renderlistpredicate)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:51

___

### renderParticles

• **renderParticles**: `boolean` = `true`

Define if particles should be rendered in your texture.

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[renderParticles](RenderTargetTexture.md#renderparticles)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:114

___

### renderPassId

• **renderPassId**: `number`

Current render pass id of the render target texture. Note it can change over the rendering as there's a separate id for each face of a cube / each layer of an array layer!

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[renderPassId](RenderTargetTexture.md#renderpassid)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:269

___

### renderSprites

• **renderSprites**: `boolean` = `false`

Define if sprites should be rendered in your texture.

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[renderSprites](RenderTargetTexture.md#rendersprites)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:118

___

### reservedDataStore

• **reservedDataStore**: `any` = `null`

For internal use only. Please do not use.

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[reservedDataStore](RenderTargetTexture.md#reserveddatastore)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:53

___

### skipInitialClear

• **skipInitialClear**: `boolean` = `false`

Skip the initial clear of the rtt at the beginning of the frame render loop

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[skipInitialClear](RenderTargetTexture.md#skipinitialclear)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:254

___

### sphericalPolynomial

• **sphericalPolynomial**: [`Nullable`](../modules.md#nullable)[`SphericalPolynomial`](SphericalPolynomial.md)

Get the polynomial representation of the texture data.
This is mainly use as a fast way to recover IBL Diffuse irradiance data.

**`See`**

https://learnopengl.com/PBR/IBL/Diffuse-irradiance

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[sphericalPolynomial](RenderTargetTexture.md#sphericalpolynomial)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.polynomial.ts:13

___

### uAng

• **uAng**: `number` = `0`

Define an offset on the texture to rotate around the u coordinates of the UVs
The angle is defined in radians.

**`See`**

https://doc.babylonjs.com/how_to/more_materials

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[uAng](RenderTargetTexture.md#uang)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:230

___

### uOffset

• **uOffset**: `number` = `0`

Define an offset on the texture to offset the u coordinates of the UVs

**`See`**

https://doc.babylonjs.com/how_to/more_materials#offsetting

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[uOffset](RenderTargetTexture.md#uoffset)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:201

___

### uRotationCenter

• **uRotationCenter**: `number` = `0.5`

Defines the center of rotation (U)

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[uRotationCenter](RenderTargetTexture.md#urotationcenter)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:252

___

### uScale

• **uScale**: `number` = `1.0`

Define an offset on the texture to scale the u coordinates of the UVs

**`See`**

https://doc.babylonjs.com/how_to/more_materials#tiling

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[uScale](RenderTargetTexture.md#uscale)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:215

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the texture

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[uniqueId](RenderTargetTexture.md#uniqueid)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:36

___

### url

• **url**: [`Nullable`](../modules.md#nullable)`string` = `null`

Define the url of the texture.

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[url](RenderTargetTexture.md#url)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:194

___

### useCameraPostProcesses

• **useCameraPostProcesses**: `boolean`

Define if camera post processes should be use while rendering the texture.

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[useCameraPostProcesses](RenderTargetTexture.md#usecamerapostprocesses)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:141

___

### vAng

• **vAng**: `number` = `0`

Define an offset on the texture to rotate around the v coordinates of the UVs
The angle is defined in radians.

**`See`**

https://doc.babylonjs.com/how_to/more_materials

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[vAng](RenderTargetTexture.md#vang)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:238

___

### vOffset

• **vOffset**: `number` = `0`

Define an offset on the texture to offset the v coordinates of the UVs

**`See`**

https://doc.babylonjs.com/how_to/more_materials#offsetting

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[vOffset](RenderTargetTexture.md#voffset)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:208

___

### vRotationCenter

• **vRotationCenter**: `number` = `0.5`

Defines the center of rotation (V)

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[vRotationCenter](RenderTargetTexture.md#vrotationcenter)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:258

___

### vScale

• **vScale**: `number` = `1.0`

Define an offset on the texture to scale the v coordinates of the UVs

**`See`**

https://doc.babylonjs.com/how_to/more_materials#tiling

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[vScale](RenderTargetTexture.md#vscale)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:222

___

### wAng

• **wAng**: `number` = `0`

Define an offset on the texture to rotate around the w coordinates of the UVs (in case of 3d texture)
The angle is defined in radians.

**`See`**

https://doc.babylonjs.com/how_to/more_materials

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[wAng](RenderTargetTexture.md#wang)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:246

___

### wRotationCenter

• **wRotationCenter**: `number` = `0.5`

Defines the center of rotation (W)

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[wRotationCenter](RenderTargetTexture.md#wrotationcenter)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:264

___

### wrapR

• **wrapR**: `number` = `Constants.TEXTURE_WRAP_ADDRESSMODE`

| Value | Type               | Description |
| ----- | ------------------ | ----------- |
| 0     | CLAMP_ADDRESSMODE  |             |
| 1     | WRAP_ADDRESSMODE   |             |
| 2     | MIRROR_ADDRESSMODE |             |

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[wrapR](RenderTargetTexture.md#wrapr)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:197

___

### BILINEAR\_SAMPLINGMODE

▪ `Static` `Readonly` **BILINEAR\_SAMPLINGMODE**: ``2``

Bilinear is mag = linear and min = linear and mip = nearest

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[BILINEAR_SAMPLINGMODE](RenderTargetTexture.md#bilinear_samplingmode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:129

___

### CLAMP\_ADDRESSMODE

▪ `Static` `Readonly` **CLAMP\_ADDRESSMODE**: ``0``

Texture is not repeating outside of 0..1 UVs

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[CLAMP_ADDRESSMODE](RenderTargetTexture.md#clamp_addressmode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:179

___

### CUBIC\_MODE

▪ `Static` `Readonly` **CUBIC\_MODE**: ``3``

Cubic coordinates mode

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[CUBIC_MODE](RenderTargetTexture.md#cubic_mode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:164

___

### DEFAULT\_ANISOTROPIC\_FILTERING\_LEVEL

▪ `Static` **DEFAULT\_ANISOTROPIC\_FILTERING\_LEVEL**: `number` = `4`

Default anisotropic filtering level for the application.
It is set to 4 as a good tradeoff between perf and quality.

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[DEFAULT_ANISOTROPIC_FILTERING_LEVEL](RenderTargetTexture.md#default_anisotropic_filtering_level)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:30

___

### EQUIRECTANGULAR\_MODE

▪ `Static` `Readonly` **EQUIRECTANGULAR\_MODE**: ``7``

Equirectangular coordinates mode

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[EQUIRECTANGULAR_MODE](RenderTargetTexture.md#equirectangular_mode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:172

___

### EXPLICIT\_MODE

▪ `Static` `Readonly` **EXPLICIT\_MODE**: ``0``

Explicit coordinates mode

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[EXPLICIT_MODE](RenderTargetTexture.md#explicit_mode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:158

___

### FIXED\_EQUIRECTANGULAR\_MIRRORED\_MODE

▪ `Static` `Readonly` **FIXED\_EQUIRECTANGULAR\_MIRRORED\_MODE**: ``9``

Equirectangular Fixed Mirrored coordinates mode

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[FIXED_EQUIRECTANGULAR_MIRRORED_MODE](RenderTargetTexture.md#fixed_equirectangular_mirrored_mode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:176

___

### FIXED\_EQUIRECTANGULAR\_MODE

▪ `Static` `Readonly` **FIXED\_EQUIRECTANGULAR\_MODE**: ``8``

Equirectangular Fixed coordinates mode

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[FIXED_EQUIRECTANGULAR_MODE](RenderTargetTexture.md#fixed_equirectangular_mode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:174

___

### ForceSerializeBuffers

▪ `Static` **ForceSerializeBuffers**: `boolean` = `false`

Gets or sets a general boolean used to indicate that texture buffers must be saved as part of the serialization process.
If no buffer exists, one will be created as base64 string from the internal webgl data.

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[ForceSerializeBuffers](RenderTargetTexture.md#forceserializebuffers)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:82

___

### INVCUBIC\_MODE

▪ `Static` `Readonly` **INVCUBIC\_MODE**: ``6``

Inverse Cubic coordinates mode

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[INVCUBIC_MODE](RenderTargetTexture.md#invcubic_mode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:170

___

### LINEAR\_LINEAR

▪ `Static` `Readonly` **LINEAR\_LINEAR**: ``2``

mag = linear and min = linear and mip = none

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[LINEAR_LINEAR](RenderTargetTexture.md#linear_linear)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:153

___

### LINEAR\_LINEAR\_MIPLINEAR

▪ `Static` `Readonly` **LINEAR\_LINEAR\_MIPLINEAR**: ``3``

Trilinear is mag = linear and min = linear and mip = linear

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[LINEAR_LINEAR_MIPLINEAR](RenderTargetTexture.md#linear_linear_miplinear)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:136

___

### LINEAR\_LINEAR\_MIPNEAREST

▪ `Static` `Readonly` **LINEAR\_LINEAR\_MIPNEAREST**: ``11``

Bilinear is mag = linear and min = linear and mip = nearest

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[LINEAR_LINEAR_MIPNEAREST](RenderTargetTexture.md#linear_linear_mipnearest)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:131

___

### LINEAR\_NEAREST

▪ `Static` `Readonly` **LINEAR\_NEAREST**: ``12``

mag = linear and min = nearest and mip = none

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[LINEAR_NEAREST](RenderTargetTexture.md#linear_nearest)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:155

___

### LINEAR\_NEAREST\_MIPLINEAR

▪ `Static` `Readonly` **LINEAR\_NEAREST\_MIPLINEAR**: ``10``

mag = linear and min = nearest and mip = linear

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[LINEAR_NEAREST_MIPLINEAR](RenderTargetTexture.md#linear_nearest_miplinear)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:151

___

### LINEAR\_NEAREST\_MIPNEAREST

▪ `Static` `Readonly` **LINEAR\_NEAREST\_MIPNEAREST**: ``9``

mag = linear and min = nearest and mip = nearest

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[LINEAR_NEAREST_MIPNEAREST](RenderTargetTexture.md#linear_nearest_mipnearest)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:149

___

### MIRROR\_ADDRESSMODE

▪ `Static` `Readonly` **MIRROR\_ADDRESSMODE**: ``2``

Texture is repeating and mirrored

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[MIRROR_ADDRESSMODE](RenderTargetTexture.md#mirror_addressmode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:183

___

### NEAREST\_LINEAR

▪ `Static` `Readonly` **NEAREST\_LINEAR**: ``7``

mag = nearest and min = linear and mip = none

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[NEAREST_LINEAR](RenderTargetTexture.md#nearest_linear)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:145

___

### NEAREST\_LINEAR\_MIPLINEAR

▪ `Static` `Readonly` **NEAREST\_LINEAR\_MIPLINEAR**: ``6``

mag = nearest and min = linear and mip = linear

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[NEAREST_LINEAR_MIPLINEAR](RenderTargetTexture.md#nearest_linear_miplinear)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:143

___

### NEAREST\_LINEAR\_MIPNEAREST

▪ `Static` `Readonly` **NEAREST\_LINEAR\_MIPNEAREST**: ``5``

mag = nearest and min = linear and mip = nearest

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[NEAREST_LINEAR_MIPNEAREST](RenderTargetTexture.md#nearest_linear_mipnearest)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:141

___

### NEAREST\_NEAREST

▪ `Static` `Readonly` **NEAREST\_NEAREST**: ``1``

mag = nearest and min = nearest and mip = none

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[NEAREST_NEAREST](RenderTargetTexture.md#nearest_nearest)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:147

___

### NEAREST\_NEAREST\_MIPLINEAR

▪ `Static` `Readonly` **NEAREST\_NEAREST\_MIPLINEAR**: ``8``

nearest is mag = nearest and min = nearest and mip = linear

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[NEAREST_NEAREST_MIPLINEAR](RenderTargetTexture.md#nearest_nearest_miplinear)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:126

___

### NEAREST\_NEAREST\_MIPNEAREST

▪ `Static` `Readonly` **NEAREST\_NEAREST\_MIPNEAREST**: ``4``

mag = nearest and min = nearest and mip = nearest

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[NEAREST_NEAREST_MIPNEAREST](RenderTargetTexture.md#nearest_nearest_mipnearest)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:139

___

### NEAREST\_SAMPLINGMODE

▪ `Static` `Readonly` **NEAREST\_SAMPLINGMODE**: ``1``

nearest is mag = nearest and min = nearest and mip = linear

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[NEAREST_SAMPLINGMODE](RenderTargetTexture.md#nearest_samplingmode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:124

___

### OnTextureLoadErrorObservable

▪ `Static` **OnTextureLoadErrorObservable**: [`Observable`](Observable.md)[`BaseTexture`](BaseTexture.md)

This observable will notify when any texture had a loading error

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[OnTextureLoadErrorObservable](RenderTargetTexture.md#ontextureloaderrorobservable)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:87

___

### PLANAR\_MODE

▪ `Static` `Readonly` **PLANAR\_MODE**: ``2``

Planar coordinates mode

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[PLANAR_MODE](RenderTargetTexture.md#planar_mode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:162

___

### PROJECTION\_MODE

▪ `Static` `Readonly` **PROJECTION\_MODE**: ``4``

Projection coordinates mode

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[PROJECTION_MODE](RenderTargetTexture.md#projection_mode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:166

___

### REFRESHRATE\_RENDER\_ONCE

▪ `Static` `Readonly` **REFRESHRATE\_RENDER\_ONCE**: `number` = `0`

The texture will only be rendered once which can be useful to improve performance if everything in your render is static for instance.

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[REFRESHRATE_RENDER_ONCE](RenderTargetTexture.md#refreshrate_render_once)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:36

___

### REFRESHRATE\_RENDER\_ONEVERYFRAME

▪ `Static` `Readonly` **REFRESHRATE\_RENDER\_ONEVERYFRAME**: `number` = `1`

The texture will only be rendered rendered every frame and is recommended for dynamic contents.

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[REFRESHRATE_RENDER_ONEVERYFRAME](RenderTargetTexture.md#refreshrate_render_oneveryframe)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:40

___

### REFRESHRATE\_RENDER\_ONEVERYTWOFRAMES

▪ `Static` `Readonly` **REFRESHRATE\_RENDER\_ONEVERYTWOFRAMES**: `number` = `2`

The texture will be rendered every 2 frames which could be enough if your dynamic objects are not
the central point of your effect and can save a lot of performances.

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[REFRESHRATE_RENDER_ONEVERYTWOFRAMES](RenderTargetTexture.md#refreshrate_render_oneverytwoframes)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:45

___

### SKYBOX\_MODE

▪ `Static` `Readonly` **SKYBOX\_MODE**: ``5``

Inverse Cubic coordinates mode

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[SKYBOX_MODE](RenderTargetTexture.md#skybox_mode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:168

___

### SPHERICAL\_MODE

▪ `Static` `Readonly` **SPHERICAL\_MODE**: ``1``

Spherical coordinates mode

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[SPHERICAL_MODE](RenderTargetTexture.md#spherical_mode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:160

___

### SerializeBuffers

▪ `Static` **SerializeBuffers**: `boolean` = `true`

Gets or sets a general boolean used to indicate that textures containing direct data (buffers) must be saved as part of the serialization process

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[SerializeBuffers](RenderTargetTexture.md#serializebuffers)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:76

___

### TRILINEAR\_SAMPLINGMODE

▪ `Static` `Readonly` **TRILINEAR\_SAMPLINGMODE**: ``3``

Trilinear is mag = linear and min = linear and mip = linear

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[TRILINEAR_SAMPLINGMODE](RenderTargetTexture.md#trilinear_samplingmode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:134

___

### UseSerializedUrlIfAny

▪ `Static` **UseSerializedUrlIfAny**: `boolean` = `false`

Gets or sets a boolean which defines if the texture url must be build from the serialized URL instead of just using the name and loading them side by side with the scene file

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[UseSerializedUrlIfAny](RenderTargetTexture.md#useserializedurlifany)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:188

___

### WRAP\_ADDRESSMODE

▪ `Static` `Readonly` **WRAP\_ADDRESSMODE**: ``1``

Texture is repeating outside of 0..1 UVs

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[WRAP_ADDRESSMODE](RenderTargetTexture.md#wrap_addressmode)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:181

## Accessors

### \_prePassEnabled

• `Private` `get` **_prePassEnabled**(): `boolean`

#### Returns

`boolean`

#### Inherited from

RenderTargetTexture.\_prePassEnabled

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:158

___

### adaptiveBlurKernel

• `set` **adaptiveBlurKernel**(`value`): `void`

Define the adaptive blur kernel used to blur the reflection if needed.
This will autocompute the closest best match for the `blurKernel`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/Textures/mirrorTexture.ts:48

___

### blurKernel

• `set` **blurKernel**(`value`): `void`

Define the blur kernel used to blur the reflection if needed.
Please consider using `adaptiveBlurKernel` as it could find the closest best value for you.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/Textures/mirrorTexture.ts:57

___

### blurKernelX

• `get` **blurKernelX**(): `number`

#### Returns

`number`

#### Defined in

packages/dev/core/src/Materials/Textures/mirrorTexture.ts:75

• `set` **blurKernelX**(`value`): `void`

Define the blur kernel on the X Axis used to blur the reflection if needed.
Please consider using `adaptiveBlurKernel` as it could find the closest best value for you.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/Textures/mirrorTexture.ts:66

___

### blurKernelY

• `get` **blurKernelY**(): `number`

#### Returns

`number`

#### Defined in

packages/dev/core/src/Materials/Textures/mirrorTexture.ts:92

• `set` **blurKernelY**(`value`): `void`

Define the blur kernel on the Y Axis used to blur the reflection if needed.
Please consider using `adaptiveBlurKernel` as it could find the closest best value for you.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/Textures/mirrorTexture.ts:83

___

### blurRatio

• `get` **blurRatio**(): `number`

#### Returns

`number`

#### Defined in

packages/dev/core/src/Materials/Textures/mirrorTexture.ts:40

• `set` **blurRatio**(`value`): `void`

Define the blur ratio used to blur the reflection if needed.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/Textures/mirrorTexture.ts:31

___

### boundingBoxSize

• `get` **boundingBoxSize**(): [`Vector3`](Vector3.md)

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

RenderTargetTexture.boundingBoxSize

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:350

• `set` **boundingBoxSize**(`value`): `void`

Gets or sets the size of the bounding box associated with the texture (when in cube mode)
When defined, the cubemap will switch to local mode

**`See`**

https://community.arm.com/graphics/b/blog/posts/reflections-based-on-local-cubemaps-in-unity

**`Example`**

```ts
https://www.babylonjs-playground.com/#RNASML
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Inherited from

RenderTargetTexture.boundingBoxSize

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:340

___

### canRescale

• `get` **canRescale**(): `boolean`

Get if the texture can be rescaled or not.

#### Returns

`boolean`

#### Inherited from

RenderTargetTexture.canRescale

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:689

___

### coordinatesIndex

• `get` **coordinatesIndex**(): `number`

#### Returns

`number`

#### Inherited from

RenderTargetTexture.coordinatesIndex

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:121

• `set` **coordinatesIndex**(`value`): `void`

Define the UV channel to use starting from 0 and defaulting to 0.
This is part of the texture as textures usually maps to one uv set.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

RenderTargetTexture.coordinatesIndex

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:110

___

### coordinatesMode

• `get` **coordinatesMode**(): `number`

How a texture is mapped.
Unused in thin texture mode.

#### Returns

`number`

#### Inherited from

RenderTargetTexture.coordinatesMode

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:155

• `set` **coordinatesMode**(`value`): `void`

How a texture is mapped.

| Value | Type                                | Description |
| ----- | ----------------------------------- | ----------- |
| 0     | EXPLICIT_MODE                       |             |
| 1     | SPHERICAL_MODE                      |             |
| 2     | PLANAR_MODE                         |             |
| 3     | CUBIC_MODE                          |             |
| 4     | PROJECTION_MODE                     |             |
| 5     | SKYBOX_MODE                         |             |
| 6     | INVCUBIC_MODE                       |             |
| 7     | EQUIRECTANGULAR_MODE                |             |
| 8     | FIXED_EQUIRECTANGULAR_MODE          |             |
| 9     | FIXED_EQUIRECTANGULAR_MIRRORED_MODE |             |

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

RenderTargetTexture.coordinatesMode

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:144

___

### currentRefreshId

• `get` **currentRefreshId**(): `number`

Gets the current value of the refreshId counter

#### Returns

`number`

#### Inherited from

RenderTargetTexture.currentRefreshId

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:282

___

### depthStencilTexture

• `get` **depthStencilTexture**(): [`Nullable`](../modules.md#nullable)[`InternalTexture`](InternalTexture.md)

In case the RTT has been created with a depth texture, get the associated
depth texture.
Otherwise, return null.

#### Returns

[`Nullable`](../modules.md#nullable)[`InternalTexture`](InternalTexture.md)

#### Inherited from

RenderTargetTexture.depthStencilTexture

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:359

___

### errorObject

• `get` **errorObject**(): `undefined` \| { `exception?`: `any` ; `message?`: `string`  }

If a loading error occurred this object will be populated with information about the error.

#### Returns

`undefined` \| { `exception?`: `any` ; `message?`: `string`  }

#### Inherited from

RenderTargetTexture.errorObject

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:498

___

### gammaSpace

• `get` **gammaSpace**(): `boolean`

Define if the texture contains data in gamma space (most of the png/jpg aside bump).
HDR texture are usually stored in linear space.
This only impacts the PBR and Background materials

#### Returns

`boolean`

#### Inherited from

RenderTargetTexture.gammaSpace

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:274

• `set` **gammaSpace**(`gamma`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `gamma` | `boolean` |

#### Returns

`void`

#### Inherited from

RenderTargetTexture.gammaSpace

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:287

___

### getAlphaFromRGB

• `get` **getAlphaFromRGB**(): `boolean`

#### Returns

`boolean`

#### Inherited from

RenderTargetTexture.getAlphaFromRGB

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:92

• `set` **getAlphaFromRGB**(`value`): `void`

Defines if the alpha value should be determined via the rgb values.
If true the luminance of the pixel might be used to find the corresponding alpha value.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

RenderTargetTexture.getAlphaFromRGB

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:81

___

### hasAlpha

• `get` **hasAlpha**(): `boolean`

#### Returns

`boolean`

#### Inherited from

RenderTargetTexture.hasAlpha

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:71

• `set` **hasAlpha**(`value`): `void`

Define if the texture is having a usable alpha value (can be use for transparency or glossiness for instance).

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

RenderTargetTexture.hasAlpha

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:60

___

### invertY

• `get` **invertY**(): `boolean`

Gets a boolean indicating if the texture needs to be inverted on the y axis during loading

#### Returns

`boolean`

#### Inherited from

RenderTargetTexture.invertY

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:347

___

### irradianceTexture

• `get` **irradianceTexture**(): [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

In case a better definition than spherical harmonics is required for the diffuse part of the environment.
You can set the irradiance texture to rely on a texture instead of the spherical approach.
This texture need to have the same characteristics than its parent (Cube vs 2d, coordinates mode, Gamma/Linear, RGBD).

#### Returns

[`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

#### Inherited from

RenderTargetTexture.irradianceTexture

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:393

• `set` **irradianceTexture**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) |

#### Returns

`void`

#### Inherited from

RenderTargetTexture.irradianceTexture

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:401

___

### is2DArray

• `get` **is2DArray**(): `boolean`

Define if the texture is a 2d array texture (webgl 2) or if false a 2d texture.

#### Returns

`boolean`

#### Inherited from

RenderTargetTexture.is2DArray

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:251

• `set` **is2DArray**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

RenderTargetTexture.is2DArray

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:260

___

### is3D

• `get` **is3D**(): `boolean`

Define if the texture is a 3d texture (webgl 2) or if false a 2d texture.

#### Returns

`boolean`

#### Inherited from

RenderTargetTexture.is3D

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:231

• `set` **is3D**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

RenderTargetTexture.is3D

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:240

___

### isBlocking

• `get` **isBlocking**(): `boolean`

Define if the texture is preventing a material to render or not.
If not and the texture is not ready, the engine will use a default black texture instead.

#### Returns

`boolean`

#### Inherited from

RenderTargetTexture.isBlocking

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:339

• `set` **isBlocking**(`value`): `void`

Is the texture preventing material to render while loading.
If false, a default texture will be used instead of the loading one during the preparation step.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

RenderTargetTexture.isBlocking

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:336

___

### isCube

• `get` **isCube**(): `boolean`

Define if the texture is a cube texture or if false a 2d texture.

#### Returns

`boolean`

#### Inherited from

RenderTargetTexture.isCube

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:211

• `set` **isCube**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

RenderTargetTexture.isCube

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:220

___

### isRGBD

• `get` **isRGBD**(): `boolean`

Gets or sets whether or not the texture contains RGBD data.

#### Returns

`boolean`

#### Inherited from

RenderTargetTexture.isRGBD

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:307

• `set` **isRGBD**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

RenderTargetTexture.isRGBD

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:310

___

### linearSpecularLOD

• `get` **linearSpecularLOD**(): `boolean`

With prefiltered texture, defined if the specular generation is based on a linear ramp.
By default we are using a log2 of the linear roughness helping to keep a better resolution for
average roughness values.

#### Returns

`boolean`

#### Inherited from

RenderTargetTexture.linearSpecularLOD

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:374

• `set` **linearSpecularLOD**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

RenderTargetTexture.linearSpecularLOD

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:382

___

### loadingError

• `get` **loadingError**(): `boolean`

Was there any loading error?

#### Returns

`boolean`

#### Inherited from

RenderTargetTexture.loadingError

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:491

___

### lodGenerationOffset

• `get` **lodGenerationOffset**(): `number`

With prefiltered texture, defined the offset used during the prefiltering steps.

#### Returns

`number`

#### Inherited from

RenderTargetTexture.lodGenerationOffset

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:338

• `set` **lodGenerationOffset**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

RenderTargetTexture.lodGenerationOffset

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:346

___

### lodGenerationScale

• `get` **lodGenerationScale**(): `number`

With prefiltered texture, defined the scale used during the prefiltering steps.

#### Returns

`number`

#### Inherited from

RenderTargetTexture.lodGenerationScale

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:355

• `set` **lodGenerationScale**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

RenderTargetTexture.lodGenerationScale

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:363

___

### mimeType

• `get` **mimeType**(): `undefined` \| `string`

Returns the texture mime type if it was defined by a loader (undefined else)

#### Returns

`undefined` \| `string`

#### Inherited from

RenderTargetTexture.mimeType

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:322

___

### noMipmap

• `get` **noMipmap**(): `boolean`

Are mip maps generated for this texture or not.

#### Returns

`boolean`

#### Inherited from

RenderTargetTexture.noMipmap

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:275

___

### onAfterRender

• `set` **onAfterRender**(`callback`): `void`

Set a after render callback in the texture.
This has been kept for backward compatibility and use of onAfterRenderObservable is recommended.

#### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | (`faceIndex`: `number`) => `void` |

#### Returns

`void`

#### Inherited from

RenderTargetTexture.onAfterRender

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:211

___

### onAfterUnbind

• `set` **onAfterUnbind**(`callback`): `void`

Set a after unbind callback in the texture.
This has been kept for backward compatibility and use of onAfterUnbindObservable is recommended.

#### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | () => `void` |

#### Returns

`void`

#### Inherited from

RenderTargetTexture.onAfterUnbind

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:177

___

### onBeforeRender

• `set` **onBeforeRender**(`callback`): `void`

Set a before render callback in the texture.
This has been kept for backward compatibility and use of onBeforeRenderObservable is recommended.

#### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | (`faceIndex`: `number`) => `void` |

#### Returns

`void`

#### Inherited from

RenderTargetTexture.onBeforeRender

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:194

___

### onClear

• `set` **onClear**(`callback`): `void`

Set a clear callback in the texture.
This has been kept for backward compatibility and use of onClearObservable is recommended.

#### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | (`Engine`: [`Engine`](Engine.md)) => `void` |

#### Returns

`void`

#### Inherited from

RenderTargetTexture.onClear

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:228

___

### onDispose

• `set` **onDispose**(`callback`): `void`

Callback triggered when the texture has been disposed.
Kept for back compatibility, you can use the onDisposeObservable instead.

#### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | () => `void` |

#### Returns

`void`

#### Inherited from

RenderTargetTexture.onDispose

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:459

___

### postProcesses

• `get` **postProcesses**(): [`PostProcess`](PostProcess.md)[]

Post-processes for this render target

#### Returns

[`PostProcess`](PostProcess.md)[]

#### Inherited from

RenderTargetTexture.postProcesses

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:152

___

### refreshRate

• `get` **refreshRate**(): `number`

Define the refresh rate of the texture or the rendering frequency.
Use 0 to render just once, 1 to render on every frame, 2 to render every two frames and so on...

#### Returns

`number`

#### Inherited from

RenderTargetTexture.refreshRate

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:550

• `set` **refreshRate**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

RenderTargetTexture.refreshRate

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:553

___

### renderList

• `get` **renderList**(): [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)[]

Use this list to define the list of mesh you want to render.

#### Returns

[`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)[]

#### Inherited from

RenderTargetTexture.renderList

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:57

• `set` **renderList**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)[] |

#### Returns

`void`

#### Inherited from

RenderTargetTexture.renderList

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:61

___

### renderPassIds

• `get` **renderPassIds**(): readonly `number`[]

Gets the render pass ids used by the render target texture. For a single render target the array length will be 1, for a cube texture it will be 6 and for
a 2D texture array it will return an array of ids the size of the 2D texture array

#### Returns

readonly `number`[]

#### Inherited from

RenderTargetTexture.renderPassIds

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:275

___

### renderTarget

• `get` **renderTarget**(): [`Nullable`](../modules.md#nullable)[`RenderTargetWrapper`](RenderTargetWrapper.md)

Gets the render target wrapper associated with this render target

#### Returns

[`Nullable`](../modules.md#nullable)[`RenderTargetWrapper`](RenderTargetWrapper.md)

#### Inherited from

RenderTargetTexture.renderTarget

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:316

___

### renderTargetOptions

• `get` **renderTargetOptions**(): `RenderTargetCreationOptions`

Gets render target creation options that were used.

#### Returns

`RenderTargetCreationOptions`

#### Inherited from

RenderTargetTexture.renderTargetOptions

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:309

___

### samples

• `get` **samples**(): `number`

Define the number of samples to use in case of MSAA.
It defaults to one meaning no MSAA has been enabled.

#### Returns

`number`

#### Inherited from

RenderTargetTexture.samples

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:528

• `set` **samples**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

RenderTargetTexture.samples

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:532

___

### samplingMode

• `get` **samplingMode**(): `number`

Get the current sampling mode associated with the texture.

#### Returns

`number`

#### Inherited from

RenderTargetTexture.samplingMode

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:243

___

### textureFormat

• `get` **textureFormat**(): `number`

Get the texture underlying format (RGB, RGBA...)

#### Returns

`number`

#### Inherited from

RenderTargetTexture.textureFormat

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:659

___

### textureType

• `get` **textureType**(): `number`

Get the texture underlying type (INT, FLOAT...)

#### Returns

`number`

#### Inherited from

RenderTargetTexture.textureType

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:648

___

### uid

• `get` **uid**(): `string`

Define the unique id of the texture in the scene.

#### Returns

`string`

#### Inherited from

RenderTargetTexture.uid

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:416

___

### wrapU

• `get` **wrapU**(): `number`

| Value | Type               | Description |
| ----- | ------------------ | ----------- |
| 0     | CLAMP_ADDRESSMODE  |             |
| 1     | WRAP_ADDRESSMODE   |             |
| 2     | MIRROR_ADDRESSMODE |             |

#### Returns

`number`

#### Inherited from

RenderTargetTexture.wrapU

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:166

• `set` **wrapU**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

RenderTargetTexture.wrapU

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:170

___

### wrapV

• `get` **wrapV**(): `number`

| Value | Type               | Description |
| ----- | ------------------ | ----------- |
| 0     | CLAMP_ADDRESSMODE  |             |
| 1     | WRAP_ADDRESSMODE   |             |
| 2     | MIRROR_ADDRESSMODE |             |

#### Returns

`number`

#### Inherited from

RenderTargetTexture.wrapV

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:181

• `set` **wrapV**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

RenderTargetTexture.wrapV

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:185

## Methods

### \_autoComputeBlurKernel

▸ `Private` **_autoComputeBlurKernel**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/Textures/mirrorTexture.ts:96

___

### \_markAllSubMeshesAsTexturesDirty

▸ `Protected` **_markAllSubMeshesAsTexturesDirty**(): `void`

Indicates that textures need to be re-calculated for all materials

#### Returns

`void`

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[_markAllSubMeshesAsTexturesDirty](RenderTargetTexture.md#_markallsubmeshesastexturesdirty)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:670

___

### \_onRatioRescale

▸ `Protected` **_onRatioRescale**(): `void`

#### Returns

`void`

#### Overrides

[RenderTargetTexture](RenderTargetTexture.md).[_onRatioRescale](RenderTargetTexture.md#_onratiorescale)

#### Defined in

packages/dev/core/src/Materials/Textures/mirrorTexture.ts:105

___

### \_preparePostProcesses

▸ `Private` **_preparePostProcesses**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/Textures/mirrorTexture.ts:228

___

### \_unbindFrameBuffer

▸ `Protected` **_unbindFrameBuffer**(`engine`, `faceIndex`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `engine` | [`Engine`](Engine.md) |
| `faceIndex` | `number` |

#### Returns

`void`

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[_unbindFrameBuffer](RenderTargetTexture.md#_unbindframebuffer)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:1034

___

### \_updateGammaSpace

▸ `Private` **_updateGammaSpace**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/Textures/mirrorTexture.ts:118

___

### addPostProcess

▸ **addPostProcess**(`postProcess`): `void`

Adds a post process to the render target rendering passes.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `postProcess` | [`PostProcess`](PostProcess.md) | define the post process to add |

#### Returns

`void`

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[addPostProcess](RenderTargetTexture.md#addpostprocess)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:562

___

### checkTransformsAreIdentical

▸ **checkTransformsAreIdentical**(`texture`): `boolean`

Checks if the texture has the same transform matrix than another texture

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `texture` | [`Nullable`](../modules.md#nullable)[`Texture`](Texture.md) | texture to check against |

#### Returns

`boolean`

true if the transforms are the same, else false

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[checkTransformsAreIdentical](RenderTargetTexture.md#checktransformsareidentical)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:633

___

### clearPostProcesses

▸ **clearPostProcesses**(`dispose?`): `void`

Clear all the post processes attached to the render target

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `dispose` | `boolean` | `false` | define if the cleared post processes should also be disposed (false by default) |

#### Returns

`void`

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[clearPostProcesses](RenderTargetTexture.md#clearpostprocesses)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:581

___

### clone

▸ **clone**(): [`MirrorTexture`](MirrorTexture.md)

Clone the mirror texture.

#### Returns

[`MirrorTexture`](MirrorTexture.md)

the cloned texture

#### Overrides

[RenderTargetTexture](RenderTargetTexture.md).[clone](RenderTargetTexture.md#clone)

#### Defined in

packages/dev/core/src/Materials/Textures/mirrorTexture.ts:290

___

### createDepthStencilTexture

▸ **createDepthStencilTexture**(`comparisonFunction?`, `bilinearFiltering?`, `generateStencil?`, `samples?`, `format?`): `void`

Creates a depth stencil texture.
This is only available in WebGL 2 or with the depth texture extension available.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `comparisonFunction` | `number` | `0` | Specifies the comparison function to set on the texture. If 0 or undefined, the texture is not in comparison mode (default: 0) |
| `bilinearFiltering` | `boolean` | `true` | Specifies whether or not bilinear filtering is enable on the texture (default: true) |
| `generateStencil` | `boolean` | `false` | Specifies whether or not a stencil should be allocated in the texture (default: false) |
| `samples` | `number` | `1` | sample count of the depth/stencil texture (default: 1) |
| `format` | `number` | `Constants.TEXTUREFORMAT_DEPTH32_FLOAT` | format of the depth texture (default: Constants.TEXTUREFORMAT_DEPTH32_FLOAT) |

#### Returns

`void`

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[createDepthStencilTexture](RenderTargetTexture.md#createdepthstenciltexture)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:478

___

### disableRescaling

▸ **disableRescaling**(): `void`

Don't allow this render target texture to rescale. Mainly used to prevent rescaling by the scene optimizer.

#### Returns

`void`

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[disableRescaling](RenderTargetTexture.md#disablerescaling)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:682

___

### dispose

▸ **dispose**(): `void`

Dispose the texture and release its associated resources.

#### Returns

`void`

#### Overrides

[RenderTargetTexture](RenderTargetTexture.md).[dispose](RenderTargetTexture.md#dispose)

#### Defined in

packages/dev/core/src/Materials/Textures/mirrorTexture.ts:340

___

### disposeFramebufferObjects

▸ **disposeFramebufferObjects**(): `void`

This will remove the attached framebuffer objects. The texture will not be able to be used as render target anymore

#### Returns

`void`

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[disposeFramebufferObjects](RenderTargetTexture.md#disposeframebufferobjects)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:1276

___

### forceSphericalPolynomialsRecompute

▸ **forceSphericalPolynomialsRecompute**(): `void`

Force recomputation of spherical polynomials.
Can be useful if you generate a cubemap multiple times (from a probe for eg) and you need the proper polynomials each time

#### Returns

`void`

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[forceSphericalPolynomialsRecompute](RenderTargetTexture.md#forcesphericalpolynomialsrecompute)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.polynomial.ts:19

___

### freeRenderingGroups

▸ **freeRenderingGroups**(): `void`

Clear the info related to rendering groups preventing retention point in material dispose.

#### Returns

`void`

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[freeRenderingGroups](RenderTargetTexture.md#freerenderinggroups)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:1360

___

### getBaseSize

▸ **getBaseSize**(): [`ISize`](../interfaces/ISize.md)

Get the base size of the texture.
It can be different from the size if the texture has been resized for POT for instance

#### Returns

[`ISize`](../interfaces/ISize.md)

the base size

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[getBaseSize](RenderTargetTexture.md#getbasesize)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:219

___

### getClassName

▸ **getClassName**(): `string`

Get the current class name of the texture useful for serialization or dynamic coding.

#### Returns

`string`

"Texture"

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[getClassName](RenderTargetTexture.md#getclassname)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:897

___

### getInternalTexture

▸ **getInternalTexture**(): [`Nullable`](../modules.md#nullable)[`InternalTexture`](InternalTexture.md)

Get the underlying lower level texture from Babylon.

#### Returns

[`Nullable`](../modules.md#nullable)[`InternalTexture`](InternalTexture.md)

the internal texture

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[getInternalTexture](RenderTargetTexture.md#getinternaltexture)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:188

___

### getReflectionTextureMatrix

▸ **getReflectionTextureMatrix**(): [`Matrix`](Matrix.md)

Get the texture reflection matrix used to rotate/transform the reflection.

#### Returns

[`Matrix`](Matrix.md)

the reflection matrix

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[getReflectionTextureMatrix](RenderTargetTexture.md#getreflectiontexturematrix)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:707

___

### getRenderHeight

▸ **getRenderHeight**(): `number`

Gets the actual render height of the texture.

#### Returns

`number`

the height of the render size

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[getRenderHeight](RenderTargetTexture.md#getrenderheight)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:658

___

### getRenderLayers

▸ **getRenderLayers**(): `number`

Gets the actual number of layers of the texture.

#### Returns

`number`

the number of layers

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[getRenderLayers](RenderTargetTexture.md#getrenderlayers)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:670

___

### getRenderSize

▸ **getRenderSize**(): `number`

Gets the actual render size of the texture.

#### Returns

`number`

the width of the render size

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[getRenderSize](RenderTargetTexture.md#getrendersize)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:638

___

### getRenderWidth

▸ **getRenderWidth**(): `number`

Gets the actual render width of the texture.

#### Returns

`number`

the width of the render size

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[getRenderWidth](RenderTargetTexture.md#getrenderwidth)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:646

___

### getScene

▸ **getScene**(): [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md)

Get the scene the texture belongs to.

#### Returns

[`Nullable`](../modules.md#nullable)[`Scene`](Scene.md)

the scene or null if undefined

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[getScene](RenderTargetTexture.md#getscene)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:540

___

### getSize

▸ **getSize**(): [`ISize`](../interfaces/ISize.md)

Get the size of the texture.

#### Returns

[`ISize`](../interfaces/ISize.md)

the texture size.

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[getSize](RenderTargetTexture.md#getsize)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:196

___

### getTextureMatrix

▸ **getTextureMatrix**(`uBase?`): [`Matrix`](Matrix.md)

Get the current texture matrix which includes the requested offsetting, tiling and rotation components.

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `uBase` | `number` | `1` |

#### Returns

[`Matrix`](Matrix.md)

the transform matrix of the texture.

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[getTextureMatrix](RenderTargetTexture.md#gettexturematrix)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:651

___

### getViewCount

▸ **getViewCount**(): `number`

Gets the number of views the corresponding to the texture (eg. a MultiviewRenderTarget will have > 1)

#### Returns

`number`

the view count

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[getViewCount](RenderTargetTexture.md#getviewcount)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:1370

___

### isReady

▸ **isReady**(): `boolean`

Get if the texture is ready to be used (downloaded, converted, mip mapped...).

#### Returns

`boolean`

true if fully ready

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[isReady](RenderTargetTexture.md#isready)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:166

___

### isReadyForRendering

▸ **isReadyForRendering**(): `boolean`

This function will check if the render target texture can be rendered (textures are loaded, shaders are compiled)

#### Returns

`boolean`

true if all required resources are ready

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[isReadyForRendering](RenderTargetTexture.md#isreadyforrendering)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:768

___

### isReadyOrNotBlocking

▸ **isReadyOrNotBlocking**(): `boolean`

Get if the texture is ready to be consumed (either it is ready or it is not blocking)

#### Returns

`boolean`

true if ready, not blocking or if there was an error loading the texture

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[isReadyOrNotBlocking](RenderTargetTexture.md#isreadyornotblocking)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:578

___

### readPixels

▸ **readPixels**(`faceIndex?`, `level?`, `buffer?`, `flushRenderer?`, `noDataConversion?`, `x?`, `y?`, `width?`, `height?`): [`Nullable`](../modules.md#nullable)`Promise``ArrayBufferView`

Reads the pixels stored in the webgl texture and returns them as an ArrayBuffer.
This will returns an RGBA array buffer containing either in values (0-255) or
float values (0-1) depending of the underlying buffer type.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `faceIndex` | `number` | `0` | defines the face of the texture to read (in case of cube texture) |
| `level` | `number` | `0` | defines the LOD level of the texture to read (in case of Mip Maps) |
| `buffer` | [`Nullable`](../modules.md#nullable)`ArrayBufferView` | `null` | defines a user defined buffer to fill with data (can be null) |
| `flushRenderer` | `boolean` | `true` | true to flush the renderer from the pending commands before reading the pixels |
| `noDataConversion` | `boolean` | `false` | false to convert the data to Uint8Array (if texture type is UNSIGNED_BYTE) or to Float32Array (if texture type is anything but UNSIGNED_BYTE). If true, the type of the generated buffer (if buffer==null) will depend on the type of the texture |
| `x` | `number` | `0` | defines the region x coordinates to start reading from (default to 0) |
| `y` | `number` | `0` | defines the region y coordinates to start reading from (default to 0) |
| `width` | `number` | `Number.MAX_VALUE` | defines the region width to read from (default to the texture size at level) |
| `height` | `number` | `Number.MAX_VALUE` | defines the region width to read from (default to the texture size at level) |

#### Returns

[`Nullable`](../modules.md#nullable)`Promise``ArrayBufferView`

The Array buffer promise containing the pixels data.

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[readPixels](RenderTargetTexture.md#readpixels)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:695

___

### releaseInternalTexture

▸ **releaseInternalTexture**(): `void`

Release and destroy the underlying lower level texture aka internalTexture.

#### Returns

`void`

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[releaseInternalTexture](RenderTargetTexture.md#releaseinternaltexture)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:1283

___

### removePostProcess

▸ **removePostProcess**(`postProcess`): `void`

Remove one of the post process from the list of attached post processes to the texture

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `postProcess` | [`PostProcess`](PostProcess.md) | define the post process to remove from the list |

#### Returns

`void`

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[removePostProcess](RenderTargetTexture.md#removepostprocess)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:599

___

### render

▸ **render**(`useCameraPostProcess?`, `dumpForDebug?`): `void`

Renders all the objects from the render list into the texture.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `useCameraPostProcess` | `boolean` | `false` | Define if camera post processes should be used during the rendering |
| `dumpForDebug` | `boolean` | `false` | Define if the rendering result should be dumped (copied) for debugging purpose |

#### Returns

`void`

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[render](RenderTargetTexture.md#render)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:760

___

### resetRefreshCounter

▸ **resetRefreshCounter**(): `void`

Resets the refresh counter of the texture and start bak from scratch.
Could be useful to regenerate the texture if it is setup to render only once.

#### Returns

`void`

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[resetRefreshCounter](RenderTargetTexture.md#resetrefreshcounter)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:542

___

### resize

▸ **resize**(`size`): `void`

Resize the texture to a new desired size.
Be careful as it will recreate all the data in the new texture.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `size` | `number` \| { `height`: `number` ; `width`: `number`  } \| { `ratio`: `number`  } | Define the new size. It can be:    - a number for squared texture,    - an object containing { width: number, height: number }    - or an object containing a ratio { ratio: number } |

#### Returns

`void`

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[resize](RenderTargetTexture.md#resize)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:723

___

### scale

▸ **scale**(`ratio`): `void`

Resize the texture using a ratio.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ratio` | `number` | the ratio to apply to the texture size in order to compute the new target size |

#### Returns

`void`

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[scale](RenderTargetTexture.md#scale)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:697

___

### serialize

▸ **serialize**(): `any`

Serialize the texture to a JSON representation you could use in Parse later on

#### Returns

`any`

the serialized JSON representation

#### Overrides

[RenderTargetTexture](RenderTargetTexture.md).[serialize](RenderTargetTexture.md#serialize)

#### Defined in

packages/dev/core/src/Materials/Textures/mirrorTexture.ts:325

___

### setMaterialForRendering

▸ **setMaterialForRendering**(`mesh`, `material?`): `void`

Sets a specific material to be used to render a mesh/a list of meshes in this render target texture

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) \| [`AbstractMesh`](AbstractMesh.md)[] | mesh or array of meshes |
| `material?` | [`Material`](Material.md) \| [`Material`](Material.md)[] | material or array of materials to use for this render pass. If undefined is passed, no specific material will be used but the regular material instead (mesh.material). It's possible to provide an array of materials to use a different material for each rendering in the case of a cube texture (6 rendering) and a 2D texture array (as many rendering as the length of the array) |

#### Returns

`void`

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[setMaterialForRendering](RenderTargetTexture.md#setmaterialforrendering)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:291

___

### setRenderingAutoClearDepthStencil

▸ **setRenderingAutoClearDepthStencil**(`renderingGroupId`, `autoClearDepthStencil`): `void`

Specifies whether or not the stencil and depth buffer are cleared between two rendering groups.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `renderingGroupId` | `number` | The rendering group id corresponding to its index |
| `autoClearDepthStencil` | `boolean` | Automatically clears depth and stencil between groups if true. |

#### Returns

`void`

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[setRenderingAutoClearDepthStencil](RenderTargetTexture.md#setrenderingautocleardepthstencil)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:1209

___

### setRenderingOrder

▸ **setRenderingOrder**(`renderingGroupId`, `opaqueSortCompareFn?`, `alphaTestSortCompareFn?`, `transparentSortCompareFn?`): `void`

Overrides the default sort function applied in the rendering group to prepare the meshes.
This allowed control for front to back rendering or reversely depending of the special needs.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `renderingGroupId` | `number` | `undefined` | The rendering group id corresponding to its index |
| `opaqueSortCompareFn` | [`Nullable`](../modules.md#nullable)(`a`: [`SubMesh`](SubMesh.md), `b`: [`SubMesh`](SubMesh.md)) => `number` | `null` | The opaque queue comparison function use to sort. |
| `alphaTestSortCompareFn` | [`Nullable`](../modules.md#nullable)(`a`: [`SubMesh`](SubMesh.md), `b`: [`SubMesh`](SubMesh.md)) => `number` | `null` | The alpha test queue comparison function use to sort. |
| `transparentSortCompareFn` | [`Nullable`](../modules.md#nullable)(`a`: [`SubMesh`](SubMesh.md), `b`: [`SubMesh`](SubMesh.md)) => `number` | `null` | The transparent queue comparison function use to sort. |

#### Returns

`void`

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[setRenderingOrder](RenderTargetTexture.md#setrenderingorder)

#### Defined in

packages/dev/core/src/Materials/Textures/renderTargetTexture.ts:1194

___

### toString

▸ **toString**(): `string`

Return a string representation of the texture.

#### Returns

`string`

the texture as a string

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[toString](RenderTargetTexture.md#tostring)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:432

___

### updateSamplingMode

▸ **updateSamplingMode**(`samplingMode`): `void`

Update the sampling mode of the texture.
Default is Trilinear mode.

| Value | Type               | Description |
| ----- | ------------------ | ----------- |
| 1     | NEAREST_SAMPLINGMODE or NEAREST_NEAREST_MIPLINEAR  | Nearest is: mag = nearest, min = nearest, mip = linear |
| 2     | BILINEAR_SAMPLINGMODE or LINEAR_LINEAR_MIPNEAREST | Bilinear is: mag = linear, min = linear, mip = nearest |
| 3     | TRILINEAR_SAMPLINGMODE or LINEAR_LINEAR_MIPLINEAR | Trilinear is: mag = linear, min = linear, mip = linear |
| 4     | NEAREST_NEAREST_MIPNEAREST |             |
| 5    | NEAREST_LINEAR_MIPNEAREST |             |
| 6    | NEAREST_LINEAR_MIPLINEAR |             |
| 7    | NEAREST_LINEAR |             |
| 8    | NEAREST_NEAREST |             |
| 9   | LINEAR_NEAREST_MIPNEAREST |             |
| 10   | LINEAR_NEAREST_MIPLINEAR |             |
| 11   | LINEAR_LINEAR |             |
| 12   | LINEAR_NEAREST |             |

   > _mag_: magnification filter (close to the viewer)
   > _min_: minification filter (far from the viewer)
   > _mip_: filter used between mip map levels

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `samplingMode` | `number` | Define the new sampling mode of the texture |

#### Returns

`void`

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[updateSamplingMode](RenderTargetTexture.md#updatesamplingmode)

#### Defined in

packages/dev/core/src/Materials/Textures/thinTexture.ts:275

___

### updateURL

▸ **updateURL**(`url`, `buffer?`, `onLoad?`, `forcedExtension?`): `void`

Update the url (and optional buffer) of this texture if url was null during construction.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `url` | `string` | `undefined` | the url of the texture |
| `buffer` | [`Nullable`](../modules.md#nullable)`string` \| `ArrayBuffer` \| `ArrayBufferView` \| `Blob` \| `HTMLImageElement` | `null` | the buffer of the texture (defaults to null) |
| `onLoad?` | () => `void` | `undefined` | callback called when the texture is loaded  (defaults to null) |
| `forcedExtension?` | `string` | `undefined` | defines the extension to use to pick the right loader |

#### Returns

`void`

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[updateURL](RenderTargetTexture.md#updateurl)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:539

___

### CreateFromBase64String

▸ `Static` **CreateFromBase64String**(`data`, `name`, `scene`, `noMipmapOrOptions?`, `invertY?`, `samplingMode?`, `onLoad?`, `onError?`, `format?`, `creationFlags?`): [`Texture`](Texture.md)

Creates a texture from its base 64 representation.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `data` | `string` | `undefined` | Define the base64 payload without the data: prefix |
| `name` | `string` | `undefined` | Define the name of the texture in the scene useful fo caching purpose for instance |
| `scene` | [`Scene`](Scene.md) | `undefined` | Define the scene the texture should belong to |
| `noMipmapOrOptions?` | `boolean` \| [`ITextureCreationOptions`](../interfaces/ITextureCreationOptions.md) | `undefined` | defines if the texture will require mip maps or not or set of all options to create the texture |
| `invertY?` | `boolean` | `undefined` | define if the texture needs to be inverted on the y axis during loading |
| `samplingMode` | `number` | `Texture.TRILINEAR_SAMPLINGMODE` | define the sampling mode we want for the texture while fetching from it (Texture.NEAREST_SAMPLINGMODE...) |
| `onLoad` | [`Nullable`](../modules.md#nullable)() => `void` | `null` | define a callback triggered when the texture has been loaded |
| `onError` | [`Nullable`](../modules.md#nullable)() => `void` | `null` | define a callback triggered when an error occurred during the loading session |
| `format` | `number` | `Constants.TEXTUREFORMAT_RGBA` | define the format of the texture we are trying to load (Engine.TEXTUREFORMAT_RGBA...) |
| `creationFlags?` | `number` | `undefined` | specific flags to use when creating the texture (Constants.TEXTURE_CREATIONFLAG_STORAGE for storage textures, for eg) |

#### Returns

[`Texture`](Texture.md)

the created texture

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[CreateFromBase64String](RenderTargetTexture.md#createfrombase64string)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:1057

___

### LoadFromDataString

▸ `Static` **LoadFromDataString**(`name`, `buffer`, `scene`, `deleteBuffer?`, `noMipmapOrOptions?`, `invertY?`, `samplingMode?`, `onLoad?`, `onError?`, `format?`, `creationFlags?`): [`Texture`](Texture.md)

Creates a texture from its data: representation. (data: will be added in case only the payload has been passed in)

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | Define the name of the texture in the scene useful fo caching purpose for instance |
| `buffer` | `any` | `undefined` | define the buffer to load the texture from in case the texture is loaded from a buffer representation |
| `scene` | [`Scene`](Scene.md) | `undefined` | Define the scene the texture should belong to |
| `deleteBuffer` | `boolean` | `false` | define if the buffer we are loading the texture from should be deleted after load |
| `noMipmapOrOptions?` | `boolean` \| [`ITextureCreationOptions`](../interfaces/ITextureCreationOptions.md) | `undefined` | defines if the texture will require mip maps or not or set of all options to create the texture |
| `invertY` | `boolean` | `true` | define if the texture needs to be inverted on the y axis during loading |
| `samplingMode` | `number` | `Texture.TRILINEAR_SAMPLINGMODE` | define the sampling mode we want for the texture while fetching from it (Texture.NEAREST_SAMPLINGMODE...) |
| `onLoad` | [`Nullable`](../modules.md#nullable)() => `void` | `null` | define a callback triggered when the texture has been loaded |
| `onError` | [`Nullable`](../modules.md#nullable)(`message?`: `string`, `exception?`: `any`) => `void` | `null` | define a callback triggered when an error occurred during the loading session |
| `format` | `number` | `Constants.TEXTUREFORMAT_RGBA` | define the format of the texture we are trying to load (Engine.TEXTUREFORMAT_RGBA...) |
| `creationFlags?` | `number` | `undefined` | specific flags to use when creating the texture (Constants.TEXTURE_CREATIONFLAG_STORAGE for storage textures, for eg) |

#### Returns

[`Texture`](Texture.md)

the created texture

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[LoadFromDataString](RenderTargetTexture.md#loadfromdatastring)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:1087

___

### Parse

▸ `Static` **Parse**(`parsedTexture`, `scene`, `rootUrl`): [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Parse the JSON representation of a texture in order to recreate the texture in the given scene.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `parsedTexture` | `any` | Define the JSON representation of the texture |
| `scene` | [`Scene`](Scene.md) | Define the scene the parsed texture should be instantiated in |
| `rootUrl` | `string` | Define the root url of the parsing sequence in the case of relative dependencies |

#### Returns

[`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

The parsed texture if successful

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[Parse](RenderTargetTexture.md#parse)

#### Defined in

packages/dev/core/src/Materials/Textures/texture.ts:920

___

### WhenAllReady

▸ `Static` **WhenAllReady**(`textures`, `callback`): `void`

Helper function to be called back once a list of texture contains only ready textures.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `textures` | [`BaseTexture`](BaseTexture.md)[] | Define the list of textures to wait for |
| `callback` | () => `void` | Define the callback triggered once the entire list will be ready |

#### Returns

`void`

#### Inherited from

[RenderTargetTexture](RenderTargetTexture.md).[WhenAllReady](RenderTargetTexture.md#whenallready)

#### Defined in

packages/dev/core/src/Materials/Textures/baseTexture.ts:864
