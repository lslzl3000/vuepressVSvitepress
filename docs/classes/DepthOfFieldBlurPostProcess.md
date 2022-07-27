[@dev/core](../README.md) / [Exports](../modules.md) / DepthOfFieldBlurPostProcess

# Class: DepthOfFieldBlurPostProcess

The DepthOfFieldBlurPostProcess applied a blur in a give direction.
This blur differs from the standard BlurPostProcess as it attempts to avoid blurring pixels
based on samples that have a large difference in distance than the center pixel.
See section 2.6.2 http://fileadmin.cs.lth.se/cs/education/edan35/lectures/12dof.pdf

## Hierarchy

- [`BlurPostProcess`](BlurPostProcess.md)

  ↳ **`DepthOfFieldBlurPostProcess`**

## Table of contents

### Constructors

- [constructor](DepthOfFieldBlurPostProcess.md#constructor)

### Properties

- [\_idealKernel](DepthOfFieldBlurPostProcess.md#_idealkernel)
- [\_indexParameters](DepthOfFieldBlurPostProcess.md#_indexparameters)
- [\_kernel](DepthOfFieldBlurPostProcess.md#_kernel)
- [\_packedFloat](DepthOfFieldBlurPostProcess.md#_packedfloat)
- [\_postProcessDefines](DepthOfFieldBlurPostProcess.md#_postprocessdefines)
- [\_scene](DepthOfFieldBlurPostProcess.md#_scene)
- [adaptScaleToCurrentViewport](DepthOfFieldBlurPostProcess.md#adaptscaletocurrentviewport)
- [alphaConstants](DepthOfFieldBlurPostProcess.md#alphaconstants)
- [alphaMode](DepthOfFieldBlurPostProcess.md#alphamode)
- [alwaysForcePOT](DepthOfFieldBlurPostProcess.md#alwaysforcepot)
- [animations](DepthOfFieldBlurPostProcess.md#animations)
- [autoClear](DepthOfFieldBlurPostProcess.md#autoclear)
- [clearColor](DepthOfFieldBlurPostProcess.md#clearcolor)
- [direction](DepthOfFieldBlurPostProcess.md#direction)
- [enablePixelPerfectMode](DepthOfFieldBlurPostProcess.md#enablepixelperfectmode)
- [externalTextureSamplerBinding](DepthOfFieldBlurPostProcess.md#externaltexturesamplerbinding)
- [forceFullscreenViewport](DepthOfFieldBlurPostProcess.md#forcefullscreenviewport)
- [height](DepthOfFieldBlurPostProcess.md#height)
- [inspectableCustomProperties](DepthOfFieldBlurPostProcess.md#inspectablecustomproperties)
- [name](DepthOfFieldBlurPostProcess.md#name)
- [nodeMaterialSource](DepthOfFieldBlurPostProcess.md#nodematerialsource)
- [onActivateObservable](DepthOfFieldBlurPostProcess.md#onactivateobservable)
- [onAfterRenderObservable](DepthOfFieldBlurPostProcess.md#onafterrenderobservable)
- [onApplyObservable](DepthOfFieldBlurPostProcess.md#onapplyobservable)
- [onBeforeRenderObservable](DepthOfFieldBlurPostProcess.md#onbeforerenderobservable)
- [onSizeChangedObservable](DepthOfFieldBlurPostProcess.md#onsizechangedobservable)
- [renderTargetSamplingMode](DepthOfFieldBlurPostProcess.md#rendertargetsamplingmode)
- [scaleMode](DepthOfFieldBlurPostProcess.md#scalemode)
- [uniqueId](DepthOfFieldBlurPostProcess.md#uniqueid)
- [width](DepthOfFieldBlurPostProcess.md#width)

### Accessors

- [aspectRatio](DepthOfFieldBlurPostProcess.md#aspectratio)
- [inputTexture](DepthOfFieldBlurPostProcess.md#inputtexture)
- [isSupported](DepthOfFieldBlurPostProcess.md#issupported)
- [kernel](DepthOfFieldBlurPostProcess.md#kernel)
- [onActivate](DepthOfFieldBlurPostProcess.md#onactivate)
- [onAfterRender](DepthOfFieldBlurPostProcess.md#onafterrender)
- [onApply](DepthOfFieldBlurPostProcess.md#onapply)
- [onBeforeRender](DepthOfFieldBlurPostProcess.md#onbeforerender)
- [onSizeChanged](DepthOfFieldBlurPostProcess.md#onsizechanged)
- [packedFloat](DepthOfFieldBlurPostProcess.md#packedfloat)
- [samples](DepthOfFieldBlurPostProcess.md#samples)
- [texelSize](DepthOfFieldBlurPostProcess.md#texelsize)

### Methods

- [\_gaussianWeight](DepthOfFieldBlurPostProcess.md#_gaussianweight)
- [\_glslFloat](DepthOfFieldBlurPostProcess.md#_glslfloat)
- [\_nearestBestKernel](DepthOfFieldBlurPostProcess.md#_nearestbestkernel)
- [\_updateParameters](DepthOfFieldBlurPostProcess.md#_updateparameters)
- [activate](DepthOfFieldBlurPostProcess.md#activate)
- [apply](DepthOfFieldBlurPostProcess.md#apply)
- [clone](DepthOfFieldBlurPostProcess.md#clone)
- [dispose](DepthOfFieldBlurPostProcess.md#dispose)
- [getCamera](DepthOfFieldBlurPostProcess.md#getcamera)
- [getClassName](DepthOfFieldBlurPostProcess.md#getclassname)
- [getEffect](DepthOfFieldBlurPostProcess.md#geteffect)
- [getEffectName](DepthOfFieldBlurPostProcess.md#geteffectname)
- [getEngine](DepthOfFieldBlurPostProcess.md#getengine)
- [isReady](DepthOfFieldBlurPostProcess.md#isready)
- [isReusable](DepthOfFieldBlurPostProcess.md#isreusable)
- [markTextureDirty](DepthOfFieldBlurPostProcess.md#marktexturedirty)
- [restoreDefaultInputTexture](DepthOfFieldBlurPostProcess.md#restoredefaultinputtexture)
- [serialize](DepthOfFieldBlurPostProcess.md#serialize)
- [setPrePassRenderer](DepthOfFieldBlurPostProcess.md#setprepassrenderer)
- [shareOutputWith](DepthOfFieldBlurPostProcess.md#shareoutputwith)
- [updateEffect](DepthOfFieldBlurPostProcess.md#updateeffect)
- [useOwnOutput](DepthOfFieldBlurPostProcess.md#useownoutput)
- [Parse](DepthOfFieldBlurPostProcess.md#parse)

## Constructors

### constructor

• **new DepthOfFieldBlurPostProcess**(`name`, `scene`, `direction`, `kernel`, `options`, `camera`, `circleOfConfusion`, `imageToBlur?`, `samplingMode?`, `engine?`, `reusable?`, `textureType?`, `blockCompilation?`)

Creates a new instance DepthOfFieldBlurPostProcess

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | The name of the effect. |
| `scene` | [`Scene`](Scene.md) | `undefined` | The scene the effect belongs to. |
| `direction` | [`Vector2`](Vector2.md) | `undefined` | The direction the blur should be applied. |
| `kernel` | `number` | `undefined` | The size of the kernel used to blur. |
| `options` | `number` \| [`PostProcessOptions`](../modules.md#postprocessoptions) | `undefined` | The required width/height ratio to downsize to before computing the render pass. |
| `camera` | [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md) | `undefined` | The camera to apply the render pass to. |
| `circleOfConfusion` | [`PostProcess`](PostProcess.md) | `undefined` | The circle of confusion + depth map to be used to avoid blurring across edges |
| `imageToBlur` | [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md) | `null` | The image to apply the blur to (default: Current rendered frame) |
| `samplingMode` | `number` | `Texture.BILINEAR_SAMPLINGMODE` | The sampling mode to be used when computing the pass. (default: 0) |
| `engine?` | [`Engine`](Engine.md) | `undefined` | The engine which the post process will be applied. (default: current engine) |
| `reusable?` | `boolean` | `undefined` | If the post process can be reused on the same frame. (default: false) |
| `textureType` | `number` | `Constants.TEXTURETYPE_UNSIGNED_INT` | Type of textures used when performing the post process. (default: 0) |
| `blockCompilation` | `boolean` | `false` | If compilation of the shader should not be done in the constructor. The updateEffect method can be used to compile the shader at a later time. (default: false) |

#### Overrides

[BlurPostProcess](BlurPostProcess.md).[constructor](BlurPostProcess.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/depthOfFieldBlurPostProcess.ts:51

## Properties

### \_idealKernel

• `Protected` **\_idealKernel**: `number`

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[_idealKernel](BlurPostProcess.md#_idealkernel)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/blurPostProcess.ts:26

___

### \_indexParameters

• `Protected` **\_indexParameters**: `any`

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[_indexParameters](BlurPostProcess.md#_indexparameters)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:211

___

### \_kernel

• `Protected` **\_kernel**: `number`

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[_kernel](BlurPostProcess.md#_kernel)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/blurPostProcess.ts:25

___

### \_packedFloat

• `Protected` **\_packedFloat**: `boolean` = `false`

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[_packedFloat](BlurPostProcess.md#_packedfloat)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/blurPostProcess.ts:28

___

### \_postProcessDefines

• `Protected` **\_postProcessDefines**: [`Nullable`](../modules.md#nullable)`string`

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[_postProcessDefines](BlurPostProcess.md#_postprocessdefines)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:209

___

### \_scene

• `Protected` **\_scene**: [`Scene`](Scene.md)

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[_scene](BlurPostProcess.md#_scene)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:173

___

### adaptScaleToCurrentViewport

• **adaptScaleToCurrentViewport**: `boolean` = `false`

Modify the scale of the post process to be the same as the viewport (default: false)

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[adaptScaleToCurrentViewport](BlurPostProcess.md#adaptscaletocurrentviewport)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:170

___

### alphaConstants

• **alphaConstants**: [`Color4`](Color4.md)

Sets the setAlphaBlendConstants of the babylon engine

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[alphaConstants](BlurPostProcess.md#alphaconstants)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:103

___

### alphaMode

• **alphaMode**: `number` = `Constants.ALPHA_DISABLE`

Type of alpha mode to use when performing the post process (default: Engine.ALPHA_DISABLE)

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[alphaMode](BlurPostProcess.md#alphamode)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:98

___

### alwaysForcePOT

• **alwaysForcePOT**: `boolean` = `false`

Force textures to be a power of two (default: false)

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[alwaysForcePOT](BlurPostProcess.md#alwaysforcepot)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:144

___

### animations

• **animations**: [`Animation`](Animation.md)[]

Animations to be used for the post processing

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[animations](BlurPostProcess.md#animations)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:107

___

### autoClear

• **autoClear**: `boolean` = `true`

If the buffer needs to be cleared before applying the post process. (default: true)
Should be set to false if shader will overwrite all previous pixels.

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[autoClear](BlurPostProcess.md#autoclear)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:93

___

### clearColor

• **clearColor**: [`Color4`](Color4.md)

Clear color to use when screen clearing

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[clearColor](BlurPostProcess.md#clearcolor)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:87

___

### direction

• **direction**: [`Vector2`](Vector2.md)

The direction the blur should be applied

#### Overrides

[BlurPostProcess](BlurPostProcess.md).[direction](BlurPostProcess.md#direction)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/depthOfFieldBlurPostProcess.ts:25

___

### enablePixelPerfectMode

• **enablePixelPerfectMode**: `boolean` = `false`

Enable Pixel Perfect mode where texture is not scaled to be power of 2.
Can only be used on a single postprocess or on the last one of a chain. (default: false)

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[enablePixelPerfectMode](BlurPostProcess.md#enablepixelperfectmode)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:114

___

### externalTextureSamplerBinding

• **externalTextureSamplerBinding**: `boolean` = `false`

if externalTextureSamplerBinding is true, the "apply" method won't bind the textureSampler texture, it is expected to be done by the "outside" (by the onApplyObservable observer most probably).
counter-productive in some cases because if the texture bound by "apply" is different from the currently texture bound, (the one set by the onApplyObservable observer, for eg) some
internal structures (materialContext) will be dirtified, which may impact performances

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[externalTextureSamplerBinding](BlurPostProcess.md#externaltexturesamplerbinding)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:187

___

### forceFullscreenViewport

• **forceFullscreenViewport**: `boolean` = `true`

Force the postprocess to be applied without taking in account viewport

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[forceFullscreenViewport](BlurPostProcess.md#forcefullscreenviewport)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:120

___

### height

• **height**: `number` = `-1`

Height of the texture to apply the post process on

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[height](BlurPostProcess.md#height)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:65

___

### inspectableCustomProperties

• **inspectableCustomProperties**: [`IInspectable`](../interfaces/IInspectable.md)[]

List of inspectable custom properties (used by the Inspector)

**`See`**

https://doc.babylonjs.com/how_to/debug_layer#extensibility

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[inspectableCustomProperties](BlurPostProcess.md#inspectablecustomproperties)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:126

___

### name

• **name**: `string`

Name of the PostProcess.

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[name](BlurPostProcess.md#name)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:53

___

### nodeMaterialSource

• **nodeMaterialSource**: [`Nullable`](../modules.md#nullable)[`NodeMaterial`](NodeMaterial.md) = `null`

Gets the node material used to create this postprocess (null if the postprocess was manually created)

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[nodeMaterialSource](BlurPostProcess.md#nodematerialsource)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:70

___

### onActivateObservable

• **onActivateObservable**: [`Observable`](Observable.md)[`Camera`](Camera.md)

An event triggered when the postprocess is activated.

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[onActivateObservable](BlurPostProcess.md#onactivateobservable)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:236

___

### onAfterRenderObservable

• **onAfterRenderObservable**: [`Observable`](Observable.md)[`Effect`](Effect.md)

An event triggered after rendering the postprocess

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[onAfterRenderObservable](BlurPostProcess.md#onafterrenderobservable)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:302

___

### onApplyObservable

• **onApplyObservable**: [`Observable`](Observable.md)[`Effect`](Effect.md)

An event triggered when the postprocess applies its effect.

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[onApplyObservable](BlurPostProcess.md#onapplyobservable)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:270

___

### onBeforeRenderObservable

• **onBeforeRenderObservable**: [`Observable`](Observable.md)[`Effect`](Effect.md)

An event triggered before rendering the postprocess

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[onBeforeRenderObservable](BlurPostProcess.md#onbeforerenderobservable)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:286

___

### onSizeChangedObservable

• **onSizeChangedObservable**: [`Observable`](Observable.md)[`PostProcess`](PostProcess.md)

An event triggered when the postprocess changes its size.

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[onSizeChangedObservable](BlurPostProcess.md#onsizechangedobservable)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:254

___

### renderTargetSamplingMode

• **renderTargetSamplingMode**: `number`

Sampling mode used by the shader
See https://doc.babylonjs.com/classes/3.1/texture

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[renderTargetSamplingMode](BlurPostProcess.md#rendertargetsamplingmode)

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

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[scaleMode](BlurPostProcess.md#scalemode)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:139

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the post process

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[uniqueId](BlurPostProcess.md#uniqueid)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:49

___

### width

• **width**: `number` = `-1`

Width of the texture to apply the post process on

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[width](BlurPostProcess.md#width)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:59

## Accessors

### aspectRatio

• `get` **aspectRatio**(): `number`

The aspect ratio of the output texture.

#### Returns

`number`

#### Inherited from

BlurPostProcess.aspectRatio

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:731

___

### inputTexture

• `get` **inputTexture**(): [`RenderTargetWrapper`](RenderTargetWrapper.md)

The input texture for this post process and the output texture of the previous post process. When added to a pipeline the previous post process will
render it's output into this texture and this texture will be used as textureSampler in the fragment shader of this post process.

#### Returns

[`RenderTargetWrapper`](RenderTargetWrapper.md)

#### Inherited from

BlurPostProcess.inputTexture

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:319

• `set` **inputTexture**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`RenderTargetWrapper`](RenderTargetWrapper.md) |

#### Returns

`void`

#### Inherited from

BlurPostProcess.inputTexture

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:323

___

### isSupported

• `get` **isSupported**(): `boolean`

If the post process is supported.

#### Returns

`boolean`

#### Inherited from

BlurPostProcess.isSupported

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:724

___

### kernel

• `get` **kernel**(): `number`

Gets the length in pixels of the blur sample region

#### Returns

`number`

#### Inherited from

BlurPostProcess.kernel

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/blurPostProcess.ts:54

• `set` **kernel**(`v`): `void`

Sets the length in pixels of the blur sample region

#### Parameters

| Name | Type |
| :------ | :------ |
| `v` | `number` |

#### Returns

`void`

#### Inherited from

BlurPostProcess.kernel

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/blurPostProcess.ts:38

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

#### Inherited from

BlurPostProcess.onActivate

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

#### Inherited from

BlurPostProcess.onAfterRender

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

#### Inherited from

BlurPostProcess.onApply

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

#### Inherited from

BlurPostProcess.onBeforeRender

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

#### Inherited from

BlurPostProcess.onSizeChanged

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:260

___

### packedFloat

• `get` **packedFloat**(): `boolean`

Gets whether or not the blur is unpacking/repacking floats

#### Returns

`boolean`

#### Inherited from

BlurPostProcess.packedFloat

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/blurPostProcess.ts:74

• `set` **packedFloat**(`v`): `void`

Sets whether or not the blur needs to unpack/repack floats

#### Parameters

| Name | Type |
| :------ | :------ |
| `v` | `boolean` |

#### Returns

`void`

#### Inherited from

BlurPostProcess.packedFloat

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/blurPostProcess.ts:61

___

### samples

• `get` **samples**(): `number`

Number of sample textures (default: 1)

#### Returns

`number`

#### Inherited from

BlurPostProcess.samples

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:152

• `set` **samples**(`n`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `n` | `number` |

#### Returns

`void`

#### Inherited from

BlurPostProcess.samples

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:156

___

### texelSize

• `get` **texelSize**(): [`Vector2`](Vector2.md)

Gets the texel size of the postprocess.
See https://en.wikipedia.org/wiki/Texel_(graphics)

#### Returns

[`Vector2`](Vector2.md)

#### Inherited from

BlurPostProcess.texelSize

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:350

## Methods

### \_gaussianWeight

▸ `Protected` **_gaussianWeight**(`x`): `number`

Calculates the value of a Gaussian distribution with sigma 3 at a given point.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | The point on the Gaussian distribution to sample. |

#### Returns

`number`

the value of the Gaussian function at x.

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[_gaussianWeight](BlurPostProcess.md#_gaussianweight)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/blurPostProcess.ts:292

___

### \_glslFloat

▸ `Protected` **_glslFloat**(`x`, `decimalFigures?`): `string`

Generates a string that can be used as a floating point number in GLSL.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `x` | `number` | `undefined` | Value to print. |
| `decimalFigures` | `number` | `8` | Number of decimal places to print the number to (excluding trailing 0s). |

#### Returns

`string`

GLSL float string.

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[_glslFloat](BlurPostProcess.md#_glslfloat)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/blurPostProcess.ts:313

___

### \_nearestBestKernel

▸ `Protected` **_nearestBestKernel**(`idealKernel`): `number`

Best kernels are odd numbers that when divided by 2, their integer part is even, so 5, 9 or 13.
Other odd kernels optimize correctly but require proportionally more samples, even kernels are
possible but will produce minor visual artifacts. Since each new kernel requires a new shader we
want to minimize kernel changes, having gaps between physical kernels is helpful in that regard.
The gaps between physical kernels are compensated for in the weighting of the samples

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `idealKernel` | `number` | Ideal blur kernel. |

#### Returns

`number`

Nearest best kernel.

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[_nearestBestKernel](BlurPostProcess.md#_nearestbestkernel)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/blurPostProcess.ts:277

___

### \_updateParameters

▸ `Protected` **_updateParameters**(`onCompiled?`, `onError?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `onCompiled?` | (`effect`: [`Effect`](Effect.md)) => `void` |
| `onError?` | (`effect`: [`Effect`](Effect.md), `errors`: `string`) => `void` |

#### Returns

`void`

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[_updateParameters](BlurPostProcess.md#_updateparameters)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/blurPostProcess.ts:162

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

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[activate](BlurPostProcess.md#activate)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:614

___

### apply

▸ **apply**(): [`Nullable`](../modules.md#nullable)[`Effect`](Effect.md)

Binds all textures and uniforms to the shader, this will be run on every pass.

#### Returns

[`Nullable`](../modules.md#nullable)[`Effect`](Effect.md)

the effect corresponding to this post process. Null if not compiled or not ready.

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[apply](BlurPostProcess.md#apply)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:754

___

### clone

▸ **clone**(): [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)

Clones this post process

#### Returns

[`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)

a new post process similar to this one

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[clone](BlurPostProcess.md#clone)

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

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[dispose](BlurPostProcess.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:830

___

### getCamera

▸ **getCamera**(): [`Camera`](Camera.md)

Gets the camera which post process is applied to.

#### Returns

[`Camera`](Camera.md)

The camera the post process is applied to.

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[getCamera](BlurPostProcess.md#getcamera)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:342

___

### getClassName

▸ **getClassName**(): `string`

Gets a string identifying the name of the class

#### Returns

`string`

"DepthOfFieldBlurPostProcess" string

#### Overrides

[BlurPostProcess](BlurPostProcess.md).[getClassName](BlurPostProcess.md#getclassname)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/depthOfFieldBlurPostProcess.ts:31

___

### getEffect

▸ **getEffect**(): [`Effect`](Effect.md)

The effect that is created when initializing the post process.

#### Returns

[`Effect`](Effect.md)

The created effect corresponding the the postprocess.

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[getEffect](BlurPostProcess.md#geteffect)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:453

___

### getEffectName

▸ **getEffectName**(): `string`

Returns the fragment url or shader name used in the post process.

#### Returns

`string`

the fragment url or name in the shader store.

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[getEffectName](BlurPostProcess.md#geteffectname)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:227

___

### getEngine

▸ **getEngine**(): [`Engine`](Engine.md)

Gets the engine which this post process belongs to.

#### Returns

[`Engine`](Engine.md)

The engine the post process was enabled with.

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[getEngine](BlurPostProcess.md#getengine)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:445

___

### isReady

▸ **isReady**(): `boolean`

Get a value indicating if the post-process is ready to be used

#### Returns

`boolean`

true if the post-process is ready (shader is compiled)

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[isReady](BlurPostProcess.md#isready)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:746

___

### isReusable

▸ **isReusable**(): `boolean`

The post process is reusable if it can be used multiple times within one frame.

#### Returns

`boolean`

If the post process is reusable

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[isReusable](BlurPostProcess.md#isreusable)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:521

___

### markTextureDirty

▸ **markTextureDirty**(): `void`

invalidate frameBuffer to hint the postprocess to create a depth buffer

#### Returns

`void`

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[markTextureDirty](BlurPostProcess.md#marktexturedirty)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:526

___

### restoreDefaultInputTexture

▸ **restoreDefaultInputTexture**(): `void`

Since inputTexture should always be defined, if we previously manually set `inputTexture`,
the only way to unset it is to use this function to restore its internal state

#### Returns

`void`

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[restoreDefaultInputTexture](BlurPostProcess.md#restoredefaultinputtexture)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:331

___

### serialize

▸ **serialize**(): `any`

Serializes the post process to a JSON object

#### Returns

`any`

the JSON object

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[serialize](BlurPostProcess.md#serialize)

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

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[setPrePassRenderer](BlurPostProcess.md#setprepassrenderer)

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

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[shareOutputWith](BlurPostProcess.md#shareoutputwith)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:462

___

### updateEffect

▸ **updateEffect**(`defines?`, `uniforms?`, `samplers?`, `indexParameters?`, `onCompiled?`, `onError?`): `void`

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

#### Returns

`void`

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[updateEffect](BlurPostProcess.md#updateeffect)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/blurPostProcess.ts:151

___

### useOwnOutput

▸ **useOwnOutput**(): `void`

Reverses the effect of calling shareOutputWith and returns the post process back to its original state.
This should be called if the post process that shares output with this post process is disabled/disposed.

#### Returns

`void`

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[useOwnOutput](BlurPostProcess.md#useownoutput)

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

#### Inherited from

[BlurPostProcess](BlurPostProcess.md).[Parse](BlurPostProcess.md#parse)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:932
