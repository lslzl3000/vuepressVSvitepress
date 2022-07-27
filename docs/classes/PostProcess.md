[@dev/core](../README.md) / [Exports](../modules.md) / PostProcess

# Class: PostProcess

PostProcess can be used to apply a shader to a texture after it has been rendered
See https://doc.babylonjs.com/how_to/how_to_use_postprocesses

## Hierarchy

- **`PostProcess`**

  ↳ [`AnaglyphPostProcess`](AnaglyphPostProcess.md)

  ↳ [`BlackAndWhitePostProcess`](BlackAndWhitePostProcess.md)

  ↳ [`BloomMergePostProcess`](BloomMergePostProcess.md)

  ↳ [`BlurPostProcess`](BlurPostProcess.md)

  ↳ [`ChromaticAberrationPostProcess`](ChromaticAberrationPostProcess.md)

  ↳ [`CircleOfConfusionPostProcess`](CircleOfConfusionPostProcess.md)

  ↳ [`ColorCorrectionPostProcess`](ColorCorrectionPostProcess.md)

  ↳ [`ConvolutionPostProcess`](ConvolutionPostProcess.md)

  ↳ [`DepthOfFieldMergePostProcess`](DepthOfFieldMergePostProcess.md)

  ↳ [`DisplayPassPostProcess`](DisplayPassPostProcess.md)

  ↳ [`ExtractHighlightsPostProcess`](ExtractHighlightsPostProcess.md)

  ↳ [`FilterPostProcess`](FilterPostProcess.md)

  ↳ [`FxaaPostProcess`](FxaaPostProcess.md)

  ↳ [`GrainPostProcess`](GrainPostProcess.md)

  ↳ [`HighlightsPostProcess`](HighlightsPostProcess.md)

  ↳ [`ImageProcessingPostProcess`](ImageProcessingPostProcess.md)

  ↳ [`MotionBlurPostProcess`](MotionBlurPostProcess.md)

  ↳ [`PassPostProcess`](PassPostProcess.md)

  ↳ [`PassCubePostProcess`](PassCubePostProcess.md)

  ↳ [`RefractionPostProcess`](RefractionPostProcess.md)

  ↳ [`SharpenPostProcess`](SharpenPostProcess.md)

  ↳ [`StereoscopicInterlacePostProcessI`](StereoscopicInterlacePostProcessI.md)

  ↳ [`StereoscopicInterlacePostProcess`](StereoscopicInterlacePostProcess.md)

  ↳ [`TonemapPostProcess`](TonemapPostProcess.md)

  ↳ [`VolumetricLightScatteringPostProcess`](VolumetricLightScatteringPostProcess.md)

  ↳ [`VRDistortionCorrectionPostProcess`](VRDistortionCorrectionPostProcess.md)

  ↳ [`VRMultiviewToSingleviewPostProcess`](VRMultiviewToSingleviewPostProcess.md)

  ↳ [`ScreenSpaceReflectionPostProcess`](ScreenSpaceReflectionPostProcess.md)

  ↳ [`ScreenSpaceCurvaturePostProcess`](ScreenSpaceCurvaturePostProcess.md)

## Table of contents

### Constructors

- [constructor](PostProcess.md#constructor)

### Properties

- [\_camera](PostProcess.md#_camera)
- [\_drawWrapper](PostProcess.md#_drawwrapper)
- [\_engine](PostProcess.md#_engine)
- [\_fragmentUrl](PostProcess.md#_fragmenturl)
- [\_indexParameters](PostProcess.md#_indexparameters)
- [\_onActivateObserver](PostProcess.md#_onactivateobserver)
- [\_onAfterRenderObserver](PostProcess.md#_onafterrenderobserver)
- [\_onApplyObserver](PostProcess.md#_onapplyobserver)
- [\_onBeforeRenderObserver](PostProcess.md#_onbeforerenderobserver)
- [\_onSizeChangedObserver](PostProcess.md#_onsizechangedobserver)
- [\_options](PostProcess.md#_options)
- [\_parameters](PostProcess.md#_parameters)
- [\_postProcessDefines](PostProcess.md#_postprocessdefines)
- [\_renderId](PostProcess.md#_renderid)
- [\_reusable](PostProcess.md#_reusable)
- [\_samplers](PostProcess.md#_samplers)
- [\_samples](PostProcess.md#_samples)
- [\_scaleRatio](PostProcess.md#_scaleratio)
- [\_scene](PostProcess.md#_scene)
- [\_shareOutputWithPostProcess](PostProcess.md#_shareoutputwithpostprocess)
- [\_texelSize](PostProcess.md#_texelsize)
- [\_textureFormat](PostProcess.md#_textureformat)
- [\_textureType](PostProcess.md#_texturetype)
- [\_vertexUrl](PostProcess.md#_vertexurl)
- [adaptScaleToCurrentViewport](PostProcess.md#adaptscaletocurrentviewport)
- [alphaConstants](PostProcess.md#alphaconstants)
- [alphaMode](PostProcess.md#alphamode)
- [alwaysForcePOT](PostProcess.md#alwaysforcepot)
- [animations](PostProcess.md#animations)
- [autoClear](PostProcess.md#autoclear)
- [clearColor](PostProcess.md#clearcolor)
- [enablePixelPerfectMode](PostProcess.md#enablepixelperfectmode)
- [externalTextureSamplerBinding](PostProcess.md#externaltexturesamplerbinding)
- [forceFullscreenViewport](PostProcess.md#forcefullscreenviewport)
- [height](PostProcess.md#height)
- [inspectableCustomProperties](PostProcess.md#inspectablecustomproperties)
- [name](PostProcess.md#name)
- [nodeMaterialSource](PostProcess.md#nodematerialsource)
- [onActivateObservable](PostProcess.md#onactivateobservable)
- [onAfterRenderObservable](PostProcess.md#onafterrenderobservable)
- [onApplyObservable](PostProcess.md#onapplyobservable)
- [onBeforeRenderObservable](PostProcess.md#onbeforerenderobservable)
- [onSizeChangedObservable](PostProcess.md#onsizechangedobservable)
- [renderTargetSamplingMode](PostProcess.md#rendertargetsamplingmode)
- [scaleMode](PostProcess.md#scalemode)
- [uniqueId](PostProcess.md#uniqueid)
- [width](PostProcess.md#width)

### Accessors

- [aspectRatio](PostProcess.md#aspectratio)
- [inputTexture](PostProcess.md#inputtexture)
- [isSupported](PostProcess.md#issupported)
- [onActivate](PostProcess.md#onactivate)
- [onAfterRender](PostProcess.md#onafterrender)
- [onApply](PostProcess.md#onapply)
- [onBeforeRender](PostProcess.md#onbeforerender)
- [onSizeChanged](PostProcess.md#onsizechanged)
- [samples](PostProcess.md#samples)
- [texelSize](PostProcess.md#texelsize)

### Methods

- [\_createRenderTargetTexture](PostProcess.md#_createrendertargettexture)
- [\_disposeTextureCache](PostProcess.md#_disposetexturecache)
- [\_disposeTextures](PostProcess.md#_disposetextures)
- [\_flushTextureCache](PostProcess.md#_flushtexturecache)
- [\_resize](PostProcess.md#_resize)
- [activate](PostProcess.md#activate)
- [apply](PostProcess.md#apply)
- [clone](PostProcess.md#clone)
- [dispose](PostProcess.md#dispose)
- [getCamera](PostProcess.md#getcamera)
- [getClassName](PostProcess.md#getclassname)
- [getEffect](PostProcess.md#geteffect)
- [getEffectName](PostProcess.md#geteffectname)
- [getEngine](PostProcess.md#getengine)
- [isReady](PostProcess.md#isready)
- [isReusable](PostProcess.md#isreusable)
- [markTextureDirty](PostProcess.md#marktexturedirty)
- [restoreDefaultInputTexture](PostProcess.md#restoredefaultinputtexture)
- [serialize](PostProcess.md#serialize)
- [setPrePassRenderer](PostProcess.md#setprepassrenderer)
- [shareOutputWith](PostProcess.md#shareoutputwith)
- [updateEffect](PostProcess.md#updateeffect)
- [useOwnOutput](PostProcess.md#useownoutput)
- [Parse](PostProcess.md#parse)

## Constructors

### constructor

• **new PostProcess**(`name`, `fragmentUrl`, `parameters`, `samplers`, `options`, `camera`, `samplingMode?`, `engine?`, `reusable?`, `defines?`, `textureType?`, `vertexUrl?`, `indexParameters?`, `blockCompilation?`, `textureFormat?`)

Creates a new instance PostProcess

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | The name of the PostProcess. |
| `fragmentUrl` | `string` | `undefined` | The url of the fragment shader to be used. |
| `parameters` | [`Nullable`](../modules.md#nullable)`string`[] | `undefined` | Array of the names of uniform non-sampler2D variables that will be passed to the shader. |
| `samplers` | [`Nullable`](../modules.md#nullable)`string`[] | `undefined` | Array of the names of uniform sampler2D variables that will be passed to the shader. |
| `options` | `number` \| [`PostProcessOptions`](../modules.md#postprocessoptions) | `undefined` | The required width/height ratio to downsize to before computing the render pass. (Use 1.0 for full size) |
| `camera` | [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md) | `undefined` | The camera to apply the render pass to. |
| `samplingMode` | `number` | `Constants.TEXTURE_NEAREST_SAMPLINGMODE` | The sampling mode to be used when computing the pass. (default: 0) |
| `engine?` | [`Engine`](Engine.md) | `undefined` | The engine which the post process will be applied. (default: current engine) |
| `reusable?` | `boolean` | `undefined` | If the post process can be reused on the same frame. (default: false) |
| `defines` | [`Nullable`](../modules.md#nullable)`string` | `null` | String of defines that will be set when running the fragment shader. (default: null) |
| `textureType` | `number` | `Constants.TEXTURETYPE_UNSIGNED_INT` | Type of textures used when performing the post process. (default: 0) |
| `vertexUrl` | `string` | `"postprocess"` | The url of the vertex shader to be used. (default: "postprocess") |
| `indexParameters?` | `any` | `undefined` | The index parameters to be used for babylons include syntax . (default: undefined) See usage in babylon.blurPostProcess.ts and kernelBlur.vertex.fx |
| `blockCompilation` | `boolean` | `false` | If the shader should not be compiled immediatly. (default: false) |
| `textureFormat` | `number` | `Constants.TEXTUREFORMAT_RGBA` | Format of textures used when performing the post process. (default: TEXTUREFORMAT_RGBA) |

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:380

## Properties

### \_camera

• `Private` **\_camera**: [`Camera`](Camera.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:172

___

### \_drawWrapper

• `Private` **\_drawWrapper**: `DrawWrapper`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:204

___

### \_engine

• `Private` **\_engine**: [`Engine`](Engine.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:174

___

### \_fragmentUrl

• `Private` **\_fragmentUrl**: `string`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:206

___

### \_indexParameters

• `Protected` **\_indexParameters**: `any`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:211

___

### \_onActivateObserver

• `Private` **\_onActivateObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Camera`](Camera.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:238

___

### \_onAfterRenderObserver

• `Private` **\_onAfterRenderObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Effect`](Effect.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:304

___

### \_onApplyObserver

• `Private` **\_onApplyObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Effect`](Effect.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:272

___

### \_onBeforeRenderObserver

• `Private` **\_onBeforeRenderObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Effect`](Effect.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:288

___

### \_onSizeChangedObserver

• `Private` **\_onSizeChangedObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`PostProcess`](PostProcess.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:256

___

### \_options

• `Private` **\_options**: `number` \| [`PostProcessOptions`](../modules.md#postprocessoptions)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:176

___

### \_parameters

• `Private` **\_parameters**: `string`[]

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:208

___

### \_postProcessDefines

• `Protected` **\_postProcessDefines**: [`Nullable`](../modules.md#nullable)`string`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:209

___

### \_renderId

• `Private` **\_renderId**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:178

___

### \_reusable

• `Private` **\_reusable**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:177

___

### \_samplers

• `Private` **\_samplers**: `string`[]

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:205

___

### \_samples

• `Private` **\_samples**: `number` = `1`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:147

___

### \_scaleRatio

• `Private` **\_scaleRatio**: [`Vector2`](Vector2.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:210

___

### \_scene

• `Protected` **\_scene**: [`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:173

___

### \_shareOutputWithPostProcess

• `Private` **\_shareOutputWithPostProcess**: [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:212

___

### \_texelSize

• `Private` **\_texelSize**: [`Vector2`](Vector2.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:213

___

### \_textureFormat

• `Private` **\_textureFormat**: `number`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:180

___

### \_textureType

• `Private` **\_textureType**: `number`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:179

___

### \_vertexUrl

• `Private` **\_vertexUrl**: `string`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:207

___

### adaptScaleToCurrentViewport

• **adaptScaleToCurrentViewport**: `boolean` = `false`

Modify the scale of the post process to be the same as the viewport (default: false)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:170

___

### alphaConstants

• **alphaConstants**: [`Color4`](Color4.md)

Sets the setAlphaBlendConstants of the babylon engine

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:103

___

### alphaMode

• **alphaMode**: `number` = `Constants.ALPHA_DISABLE`

Type of alpha mode to use when performing the post process (default: Engine.ALPHA_DISABLE)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:98

___

### alwaysForcePOT

• **alwaysForcePOT**: `boolean` = `false`

Force textures to be a power of two (default: false)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:144

___

### animations

• **animations**: [`Animation`](Animation.md)[]

Animations to be used for the post processing

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:107

___

### autoClear

• **autoClear**: `boolean` = `true`

If the buffer needs to be cleared before applying the post process. (default: true)
Should be set to false if shader will overwrite all previous pixels.

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:93

___

### clearColor

• **clearColor**: [`Color4`](Color4.md)

Clear color to use when screen clearing

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:87

___

### enablePixelPerfectMode

• **enablePixelPerfectMode**: `boolean` = `false`

Enable Pixel Perfect mode where texture is not scaled to be power of 2.
Can only be used on a single postprocess or on the last one of a chain. (default: false)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:114

___

### externalTextureSamplerBinding

• **externalTextureSamplerBinding**: `boolean` = `false`

if externalTextureSamplerBinding is true, the "apply" method won't bind the textureSampler texture, it is expected to be done by the "outside" (by the onApplyObservable observer most probably).
counter-productive in some cases because if the texture bound by "apply" is different from the currently texture bound, (the one set by the onApplyObservable observer, for eg) some
internal structures (materialContext) will be dirtified, which may impact performances

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:187

___

### forceFullscreenViewport

• **forceFullscreenViewport**: `boolean` = `true`

Force the postprocess to be applied without taking in account viewport

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:120

___

### height

• **height**: `number` = `-1`

Height of the texture to apply the post process on

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:65

___

### inspectableCustomProperties

• **inspectableCustomProperties**: [`IInspectable`](../interfaces/IInspectable.md)[]

List of inspectable custom properties (used by the Inspector)

**`See`**

https://doc.babylonjs.com/how_to/debug_layer#extensibility

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:126

___

### name

• **name**: `string`

Name of the PostProcess.

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:53

___

### nodeMaterialSource

• **nodeMaterialSource**: [`Nullable`](../modules.md#nullable)[`NodeMaterial`](NodeMaterial.md) = `null`

Gets the node material used to create this postprocess (null if the postprocess was manually created)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:70

___

### onActivateObservable

• **onActivateObservable**: [`Observable`](Observable.md)[`Camera`](Camera.md)

An event triggered when the postprocess is activated.

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:236

___

### onAfterRenderObservable

• **onAfterRenderObservable**: [`Observable`](Observable.md)[`Effect`](Effect.md)

An event triggered after rendering the postprocess

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:302

___

### onApplyObservable

• **onApplyObservable**: [`Observable`](Observable.md)[`Effect`](Effect.md)

An event triggered when the postprocess applies its effect.

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:270

___

### onBeforeRenderObservable

• **onBeforeRenderObservable**: [`Observable`](Observable.md)[`Effect`](Effect.md)

An event triggered before rendering the postprocess

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:286

___

### onSizeChangedObservable

• **onSizeChangedObservable**: [`Observable`](Observable.md)[`PostProcess`](PostProcess.md)

An event triggered when the postprocess changes its size.

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:254

___

### renderTargetSamplingMode

• **renderTargetSamplingMode**: `number`

Sampling mode used by the shader
See https://doc.babylonjs.com/classes/3.1/texture

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:82

___

### scaleMode

• **scaleMode**: `number` = `Constants.SCALEMODE_FLOOR`

Scale mode for the post process (default: Engine.SCALEMODE_FLOOR)

| Value | Type                                | Description |
| ----- | ----------------------------------- | ----------- |
| 1     | SCALEMODE_FLOOR                     | [engine.scalemode_floor](https://doc.babylonjs.com/api/classes/babylon.engine#scalemode_floor) |
| 2     | SCALEMODE_NEAREST                   | [engine.scalemode_nearest](https://doc.babylonjs.com/api/classes/babylon.engine#scalemode_nearest) |
| 3     | SCALEMODE_CEILING                   | [engine.scalemode_ceiling](https://doc.babylonjs.com/api/classes/babylon.engine#scalemode_ceiling) |

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:139

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the post process

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:49

___

### width

• **width**: `number` = `-1`

Width of the texture to apply the post process on

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:59

## Accessors

### aspectRatio

• `get` **aspectRatio**(): `number`

The aspect ratio of the output texture.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:731

___

### inputTexture

• `get` **inputTexture**(): [`RenderTargetWrapper`](RenderTargetWrapper.md)

The input texture for this post process and the output texture of the previous post process. When added to a pipeline the previous post process will
render it's output into this texture and this texture will be used as textureSampler in the fragment shader of this post process.

#### Returns

[`RenderTargetWrapper`](RenderTargetWrapper.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:319

• `set` **inputTexture**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`RenderTargetWrapper`](RenderTargetWrapper.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:323

___

### isSupported

• `get` **isSupported**(): `boolean`

If the post process is supported.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:724

___

### onActivate

• `set` **onActivate**(`callback`): `void`

A function that is added to the onActivateObservable

#### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | [`Nullable`](../modules.md#nullable)(`camera`: [`Camera`](Camera.md)) => `void` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:242

___

### onAfterRender

• `set` **onAfterRender**(`callback`): `void`

A function that is added to the onAfterRenderObservable

#### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | (`efect`: [`Effect`](Effect.md)) => `void` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:308

___

### onApply

• `set` **onApply**(`callback`): `void`

A function that is added to the onApplyObservable

#### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | (`effect`: [`Effect`](Effect.md)) => `void` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:276

___

### onBeforeRender

• `set` **onBeforeRender**(`callback`): `void`

A function that is added to the onBeforeRenderObservable

#### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | (`effect`: [`Effect`](Effect.md)) => `void` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:292

___

### onSizeChanged

• `set` **onSizeChanged**(`callback`): `void`

A function that is added to the onSizeChangedObservable

#### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | (`postProcess`: [`PostProcess`](PostProcess.md)) => `void` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:260

___

### samples

• `get` **samples**(): `number`

Number of sample textures (default: 1)

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:152

• `set` **samples**(`n`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `n` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:156

___

### texelSize

• `get` **texelSize**(): [`Vector2`](Vector2.md)

Gets the texel size of the postprocess.
See https://en.wikipedia.org/wiki/Texel_(graphics)

#### Returns

[`Vector2`](Vector2.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:350

## Methods

### \_createRenderTargetTexture

▸ `Private` **_createRenderTargetTexture**(`textureSize`, `textureOptions`, `channel?`): [`RenderTargetWrapper`](RenderTargetWrapper.md)

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `textureSize` | `Object` | `undefined` |
| `textureSize.height` | `number` | `undefined` |
| `textureSize.width` | `number` | `undefined` |
| `textureOptions` | `RenderTargetCreationOptions` | `undefined` |
| `channel` | `number` | `0` |

#### Returns

[`RenderTargetWrapper`](RenderTargetWrapper.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:530

___

### \_disposeTextureCache

▸ `Private` **_disposeTextureCache**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:803

___

### \_disposeTextures

▸ `Private` **_disposeTextures**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:793

___

### \_flushTextureCache

▸ `Private` **_flushTextureCache**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:548

___

### \_resize

▸ `Private` **_resize**(`width`, `height`, `camera`, `needMipMaps`, `forceDepthStencil?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `width` | `number` |
| `height` | `number` |
| `camera` | [`Camera`](Camera.md) |
| `needMipMaps` | `boolean` |
| `forceDepthStencil?` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:569

___

### activate

▸ **activate**(`camera`, `sourceTexture?`, `forceDepthStencil?`): [`RenderTargetWrapper`](RenderTargetWrapper.md)

Activates the post process by intializing the textures to be used when executed. Notifies onActivateObservable.
When this post process is used in a pipeline, this is call will bind the input texture of this post process to the output of the previous.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `camera` | [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md) | `undefined` | The camera that will be used in the post process. This camera will be used when calling onActivateObservable. |
| `sourceTexture` | [`Nullable`](../modules.md#nullable)[`InternalTexture`](InternalTexture.md) | `null` | The source texture to be inspected to get the width and height if not specified in the post process constructor. (default: null) |
| `forceDepthStencil?` | `boolean` | `undefined` | If true, a depth and stencil buffer will be generated. (default: false) |

#### Returns

[`RenderTargetWrapper`](RenderTargetWrapper.md)

The render target wrapper that was bound to be written to.

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:614

___

### apply

▸ **apply**(): [`Nullable`](../modules.md#nullable)[`Effect`](Effect.md)

Binds all textures and uniforms to the shader, this will be run on every pass.

#### Returns

[`Nullable`](../modules.md#nullable)[`Effect`](Effect.md)

the effect corresponding to this post process. Null if not compiled or not ready.

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:754

___

### clone

▸ **clone**(): [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)

Clones this post process

#### Returns

[`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)

a new post process similar to this one

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:903

___

### dispose

▸ **dispose**(`camera?`): `void`

Disposes the post process.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `camera?` | [`Camera`](Camera.md) | The camera to dispose the post process on. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:830

___

### getCamera

▸ **getCamera**(): [`Camera`](Camera.md)

Gets the camera which post process is applied to.

#### Returns

[`Camera`](Camera.md)

The camera the post process is applied to.

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:342

___

### getClassName

▸ **getClassName**(): `string`

Gets a string identifying the name of the class

#### Returns

`string`

"PostProcess" string

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:437

___

### getEffect

▸ **getEffect**(): [`Effect`](Effect.md)

The effect that is created when initializing the post process.

#### Returns

[`Effect`](Effect.md)

The created effect corresponding the the postprocess.

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:453

___

### getEffectName

▸ **getEffectName**(): `string`

Returns the fragment url or shader name used in the post process.

#### Returns

`string`

the fragment url or name in the shader store.

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:227

___

### getEngine

▸ **getEngine**(): [`Engine`](Engine.md)

Gets the engine which this post process belongs to.

#### Returns

[`Engine`](Engine.md)

The engine the post process was enabled with.

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:445

___

### isReady

▸ **isReady**(): `boolean`

Get a value indicating if the post-process is ready to be used

#### Returns

`boolean`

true if the post-process is ready (shader is compiled)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:746

___

### isReusable

▸ **isReusable**(): `boolean`

The post process is reusable if it can be used multiple times within one frame.

#### Returns

`boolean`

If the post process is reusable

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:521

___

### markTextureDirty

▸ **markTextureDirty**(): `void`

invalidate frameBuffer to hint the postprocess to create a depth buffer

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:526

___

### restoreDefaultInputTexture

▸ **restoreDefaultInputTexture**(): `void`

Since inputTexture should always be defined, if we previously manually set `inputTexture`,
the only way to unset it is to use this function to restore its internal state

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:331

___

### serialize

▸ **serialize**(): `any`

Serializes the post process to a JSON object

#### Returns

`any`

the JSON object

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:880

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

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:816

___

### shareOutputWith

▸ **shareOutputWith**(`postProcess`): [`PostProcess`](PostProcess.md)

To avoid multiple redundant textures for multiple post process, the output the output texture for this post process can be shared with another.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `postProcess` | [`PostProcess`](PostProcess.md) | The post process to share the output with. |

#### Returns

[`PostProcess`](PostProcess.md)

This post process.

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:462

___

### updateEffect

▸ **updateEffect**(`defines?`, `uniforms?`, `samplers?`, `indexParameters?`, `onCompiled?`, `onError?`, `vertexUrl?`, `fragmentUrl?`): `void`

Updates the effect with the current post process compile time values and recompiles the shader.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `defines` | [`Nullable`](../modules.md#nullable)`string` | `null` | Define statements that should be added at the beginning of the shader. (default: null) |
| `uniforms` | [`Nullable`](../modules.md#nullable)`string`[] | `null` | Set of uniform variables that will be passed to the shader. (default: null) |
| `samplers` | [`Nullable`](../modules.md#nullable)`string`[] | `null` | Set of Texture2D variables that will be passed to the shader. (default: null) |
| `indexParameters?` | `any` | `undefined` | The index parameters to be used for babylons include syntax . (default: undefined) See usage in babylon.blurPostProcess.ts and kernelBlur.vertex.fx |
| `onCompiled?` | (`effect`: [`Effect`](Effect.md)) => `void` | `undefined` | Called when the shader has been compiled. |
| `onError?` | (`effect`: [`Effect`](Effect.md), `errors`: `string`) => `void` | `undefined` | Called if there is an error when compiling a shader. |
| `vertexUrl?` | `string` | `undefined` | The url of the vertex shader to be used (default: the one given at construction time) |
| `fragmentUrl?` | `string` | `undefined` | The url of the fragment shader to be used (default: the one given at construction time) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:493

___

### useOwnOutput

▸ **useOwnOutput**(): `void`

Reverses the effect of calling shareOutputWith and returns the post process back to its original state.
This should be called if the post process that shares output with this post process is disabled/disposed.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:474

___

### Parse

▸ `Static` **Parse**(`parsedPostProcess`, `scene`, `rootUrl`): [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)

Creates a material from parsed material data

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `parsedPostProcess` | `any` | defines parsed post process data |
| `scene` | [`Scene`](Scene.md) | defines the hosting scene |
| `rootUrl` | `string` | defines the root URL to use to load textures |

#### Returns

[`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)

a new post process

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:932
