[@dev/core](../README.md) / [Exports](../modules.md) / EngineCapabilities

# Interface: EngineCapabilities

Interface used to describe the capabilities of the engine relatively to the current browser

## Table of contents

### Properties

- [astc](EngineCapabilities.md#astc)
- [blendMinMax](EngineCapabilities.md#blendminmax)
- [bptc](EngineCapabilities.md#bptc)
- [canUseGLInstanceID](EngineCapabilities.md#canuseglinstanceid)
- [canUseGLVertexID](EngineCapabilities.md#canuseglvertexid)
- [canUseTimestampForTimerQuery](EngineCapabilities.md#canusetimestampfortimerquery)
- [colorBufferFloat](EngineCapabilities.md#colorbufferfloat)
- [depthTextureExtension](EngineCapabilities.md#depthtextureextension)
- [drawBuffersExtension](EngineCapabilities.md#drawbuffersextension)
- [etc1](EngineCapabilities.md#etc1)
- [etc2](EngineCapabilities.md#etc2)
- [fragmentDepthSupported](EngineCapabilities.md#fragmentdepthsupported)
- [highPrecisionShaderSupported](EngineCapabilities.md#highprecisionshadersupported)
- [instancedArrays](EngineCapabilities.md#instancedarrays)
- [maxAnisotropy](EngineCapabilities.md#maxanisotropy)
- [maxCombinedTexturesImageUnits](EngineCapabilities.md#maxcombinedtexturesimageunits)
- [maxCubemapTextureSize](EngineCapabilities.md#maxcubemaptexturesize)
- [maxFragmentUniformVectors](EngineCapabilities.md#maxfragmentuniformvectors)
- [maxMSAASamples](EngineCapabilities.md#maxmsaasamples)
- [maxRenderTextureSize](EngineCapabilities.md#maxrendertexturesize)
- [maxSamples](EngineCapabilities.md#maxsamples)
- [maxTextureSize](EngineCapabilities.md#maxtexturesize)
- [maxTexturesImageUnits](EngineCapabilities.md#maxtexturesimageunits)
- [maxVaryingVectors](EngineCapabilities.md#maxvaryingvectors)
- [maxVertexAttribs](EngineCapabilities.md#maxvertexattribs)
- [maxVertexTextureImageUnits](EngineCapabilities.md#maxvertextextureimageunits)
- [maxVertexUniformVectors](EngineCapabilities.md#maxvertexuniformvectors)
- [multiview](EngineCapabilities.md#multiview)
- [oculusMultiview](EngineCapabilities.md#oculusmultiview)
- [parallelShaderCompile](EngineCapabilities.md#parallelshadercompile)
- [pvrtc](EngineCapabilities.md#pvrtc)
- [s3tc](EngineCapabilities.md#s3tc)
- [s3tc\_srgb](EngineCapabilities.md#s3tc_srgb)
- [standardDerivatives](EngineCapabilities.md#standardderivatives)
- [supportComputeShaders](EngineCapabilities.md#supportcomputeshaders)
- [supportOcclusionQuery](EngineCapabilities.md#supportocclusionquery)
- [supportSRGBBuffers](EngineCapabilities.md#supportsrgbbuffers)
- [supportTransformFeedbacks](EngineCapabilities.md#supporttransformfeedbacks)
- [texture2DArrayMaxLayerCount](EngineCapabilities.md#texture2darraymaxlayercount)
- [textureAnisotropicFilterExtension](EngineCapabilities.md#textureanisotropicfilterextension)
- [textureFloat](EngineCapabilities.md#texturefloat)
- [textureFloatLinearFiltering](EngineCapabilities.md#texturefloatlinearfiltering)
- [textureFloatRender](EngineCapabilities.md#texturefloatrender)
- [textureHalfFloat](EngineCapabilities.md#texturehalffloat)
- [textureHalfFloatLinearFiltering](EngineCapabilities.md#texturehalffloatlinearfiltering)
- [textureHalfFloatRender](EngineCapabilities.md#texturehalffloatrender)
- [textureLOD](EngineCapabilities.md#texturelod)
- [textureMaxLevel](EngineCapabilities.md#texturemaxlevel)
- [timerQuery](EngineCapabilities.md#timerquery)
- [uintIndices](EngineCapabilities.md#uintindices)
- [vertexArrayObject](EngineCapabilities.md#vertexarrayobject)

## Properties

### astc

• **astc**: `any`

Defines if astc texture compression is supported

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:41

___

### blendMinMax

• **blendMinMax**: `boolean`

Defines if the blend min max extension is supported

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:96

___

### bptc

• **bptc**: `any`

Defines if bptc texture compression is supported

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:43

___

### canUseGLInstanceID

• **canUseGLInstanceID**: `boolean`

In some iOS + WebGL1, gl_InstanceID (and gl_InstanceIDEXT) is undefined even if instancedArrays is true. So don't use gl_InstanceID in those cases

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:98

___

### canUseGLVertexID

• **canUseGLVertexID**: `boolean`

Defines if gl_vertexID is available

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:100

___

### canUseTimestampForTimerQuery

• **canUseTimestampForTimerQuery**: `boolean`

Defines if timestamp can be used with timer query

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:81

___

### colorBufferFloat

• **colorBufferFloat**: `boolean`

Defines if float color buffer are supported

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:77

___

### depthTextureExtension

• **depthTextureExtension**: `boolean`

Defines if depth textures are supported

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:75

___

### drawBuffersExtension

• **drawBuffersExtension**: `boolean`

Defines if draw buffers extension is supported

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:73

___

### etc1

• **etc1**: `any`

Defines if etc1 texture compression is supported

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:37

___

### etc2

• **etc2**: `any`

Defines if etc2 texture compression is supported

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:39

___

### fragmentDepthSupported

• **fragmentDepthSupported**: `boolean`

Defines if depth reading in the fragment shader is supported

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:59

___

### highPrecisionShaderSupported

• **highPrecisionShaderSupported**: `boolean`

Defines if high precision shaders are supported

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:57

___

### instancedArrays

• **instancedArrays**: `boolean`

Defines if instancing is supported

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:53

___

### maxAnisotropy

• **maxAnisotropy**: `number`

Gets the maximum level of anisotropy supported

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:51

___

### maxCombinedTexturesImageUnits

• **maxCombinedTexturesImageUnits**: `number`

Maximum textures units in the entire pipeline

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:10

___

### maxCubemapTextureSize

• **maxCubemapTextureSize**: `number`

Maximum cube texture size

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:16

___

### maxFragmentUniformVectors

• **maxFragmentUniformVectors**: `number`

Maximum number of uniforms per fragment shader

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:26

___

### maxMSAASamples

• **maxMSAASamples**: `number`

Max number of texture samples for MSAA

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:94

___

### maxRenderTextureSize

• **maxRenderTextureSize**: `number`

Maximum render texture size

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:18

___

### maxSamples

• `Optional` **maxSamples**: `number`

Maximum texture samples

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:14

___

### maxTextureSize

• **maxTextureSize**: `number`

Maximum texture size

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:12

___

### maxTexturesImageUnits

• **maxTexturesImageUnits**: `number`

Maximum textures units per fragment shader

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:6

___

### maxVaryingVectors

• **maxVaryingVectors**: `number`

Maximum number of varyings

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:22

___

### maxVertexAttribs

• **maxVertexAttribs**: `number`

Maximum number of vertex attributes

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:20

___

### maxVertexTextureImageUnits

• **maxVertexTextureImageUnits**: `number`

Maximum texture units per vertex shader

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:8

___

### maxVertexUniformVectors

• **maxVertexUniformVectors**: `number`

Maximum number of uniforms per vertex shader

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:24

___

### multiview

• `Optional` **multiview**: `any`

Defines if multiview is supported (https://www.khronos.org/registry/webgl/extensions/WEBGL_multiview/)

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:85

___

### oculusMultiview

• `Optional` **oculusMultiview**: `any`

Defines if oculus multiview is supported (https://developer.oculus.com/documentation/oculus-browser/latest/concepts/browser-multiview/)

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:87

___

### parallelShaderCompile

• `Optional` **parallelShaderCompile**: `Object`

Function used to let the system compiles shaders in background

#### Type declaration

| Name | Type |
| :------ | :------ |
| `COMPLETION_STATUS_KHR` | `number` |

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:89

___

### pvrtc

• **pvrtc**: `any`

Defines if pvrtc texture compression is supported

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:35

___

### s3tc

• `Optional` **s3tc**: `WEBGL_compressed_texture_s3tc`

Defines if s3tc texture compression is supported

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:30

___

### s3tc\_srgb

• `Optional` **s3tc\_srgb**: `WEBGL_compressed_texture_s3tc_srgb`

Defines if s3tc sRGB texture compression is supported

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:33

___

### standardDerivatives

• **standardDerivatives**: `boolean`

Defines if standard derivatives (dx/dy) are supported

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:28

___

### supportComputeShaders

• **supportComputeShaders**: `boolean`

Defines if compute shaders are supported by the engine

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:102

___

### supportOcclusionQuery

• **supportOcclusionQuery**: `boolean`

Defines if occlusion queries are supported by the engine

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:83

___

### supportSRGBBuffers

• **supportSRGBBuffers**: `boolean`

Defines if sRGB texture formats are supported

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:104

___

### supportTransformFeedbacks

• **supportTransformFeedbacks**: `boolean`

Defines if transform feedbacks are supported

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:106

___

### texture2DArrayMaxLayerCount

• **texture2DArrayMaxLayerCount**: `number`

Defines the maximum layer count for a 2D Texture array.

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:111

___

### textureAnisotropicFilterExtension

• `Optional` **textureAnisotropicFilterExtension**: `EXT_texture_filter_anisotropic`

Gets the webgl extension for anisotropic filtering (null if not supported)

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:49

___

### textureFloat

• **textureFloat**: `boolean`

Defines if float textures are supported

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:45

___

### textureFloatLinearFiltering

• **textureFloatLinearFiltering**: `boolean`

Defines if float texture linear filtering is supported

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:61

___

### textureFloatRender

• **textureFloatRender**: `boolean`

Defines if rendering to float textures is supported

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:63

___

### textureHalfFloat

• **textureHalfFloat**: `boolean`

Defines if half float textures are supported

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:65

___

### textureHalfFloatLinearFiltering

• **textureHalfFloatLinearFiltering**: `boolean`

Defines if half float texture linear filtering is supported

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:67

___

### textureHalfFloatRender

• **textureHalfFloatRender**: `boolean`

Defines if rendering to half float textures is supported

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:69

___

### textureLOD

• **textureLOD**: `boolean`

Defines if textureLOD shader command is supported

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:71

___

### textureMaxLevel

• **textureMaxLevel**: `boolean`

Defines if texture max level are supported

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:108

___

### timerQuery

• `Optional` **timerQuery**: `EXT_disjoint_timer_query`

Gets disjoint timer query extension (null if not supported)

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:79

___

### uintIndices

• **uintIndices**: `boolean`

Defines if 32 bits indices are supported

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:55

___

### vertexArrayObject

• **vertexArrayObject**: `boolean`

Defines if vertex array objects are supported

#### Defined in

https://github.com/babylon.js/core/src/Engines/engineCapabilities.ts:47
