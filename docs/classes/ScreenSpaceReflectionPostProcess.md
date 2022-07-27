[@dev/core](../README.md) / [Exports](../modules.md) / ScreenSpaceReflectionPostProcess

# Class: ScreenSpaceReflectionPostProcess

The ScreenSpaceReflectionPostProcess performs realtime reflections using only and only the available informations on the screen (positions and normals).
Basically, the screen space reflection post-process will compute reflections according the material's reflectivity.

## Hierarchy

- [`PostProcess`](PostProcess.md)

  ↳ **`ScreenSpaceReflectionPostProcess`**

## Table of contents

### Constructors

- [constructor](ScreenSpaceReflectionPostProcess.md#constructor)

### Properties

- [\_enableSmoothReflections](ScreenSpaceReflectionPostProcess.md#_enablesmoothreflections)
- [\_forceGeometryBuffer](ScreenSpaceReflectionPostProcess.md#_forcegeometrybuffer)
- [\_indexParameters](ScreenSpaceReflectionPostProcess.md#_indexparameters)
- [\_isSceneRightHanded](ScreenSpaceReflectionPostProcess.md#_isscenerighthanded)
- [\_postProcessDefines](ScreenSpaceReflectionPostProcess.md#_postprocessdefines)
- [\_reflectionSamples](ScreenSpaceReflectionPostProcess.md#_reflectionsamples)
- [\_scene](ScreenSpaceReflectionPostProcess.md#_scene)
- [\_smoothSteps](ScreenSpaceReflectionPostProcess.md#_smoothsteps)
- [adaptScaleToCurrentViewport](ScreenSpaceReflectionPostProcess.md#adaptscaletocurrentviewport)
- [alphaConstants](ScreenSpaceReflectionPostProcess.md#alphaconstants)
- [alphaMode](ScreenSpaceReflectionPostProcess.md#alphamode)
- [alwaysForcePOT](ScreenSpaceReflectionPostProcess.md#alwaysforcepot)
- [animations](ScreenSpaceReflectionPostProcess.md#animations)
- [autoClear](ScreenSpaceReflectionPostProcess.md#autoclear)
- [clearColor](ScreenSpaceReflectionPostProcess.md#clearcolor)
- [enablePixelPerfectMode](ScreenSpaceReflectionPostProcess.md#enablepixelperfectmode)
- [externalTextureSamplerBinding](ScreenSpaceReflectionPostProcess.md#externaltexturesamplerbinding)
- [forceFullscreenViewport](ScreenSpaceReflectionPostProcess.md#forcefullscreenviewport)
- [height](ScreenSpaceReflectionPostProcess.md#height)
- [inspectableCustomProperties](ScreenSpaceReflectionPostProcess.md#inspectablecustomproperties)
- [name](ScreenSpaceReflectionPostProcess.md#name)
- [nodeMaterialSource](ScreenSpaceReflectionPostProcess.md#nodematerialsource)
- [onActivateObservable](ScreenSpaceReflectionPostProcess.md#onactivateobservable)
- [onAfterRenderObservable](ScreenSpaceReflectionPostProcess.md#onafterrenderobservable)
- [onApplyObservable](ScreenSpaceReflectionPostProcess.md#onapplyobservable)
- [onBeforeRenderObservable](ScreenSpaceReflectionPostProcess.md#onbeforerenderobservable)
- [onSizeChangedObservable](ScreenSpaceReflectionPostProcess.md#onsizechangedobservable)
- [reflectionSpecularFalloffExponent](ScreenSpaceReflectionPostProcess.md#reflectionspecularfalloffexponent)
- [renderTargetSamplingMode](ScreenSpaceReflectionPostProcess.md#rendertargetsamplingmode)
- [roughnessFactor](ScreenSpaceReflectionPostProcess.md#roughnessfactor)
- [scaleMode](ScreenSpaceReflectionPostProcess.md#scalemode)
- [step](ScreenSpaceReflectionPostProcess.md#step)
- [strength](ScreenSpaceReflectionPostProcess.md#strength)
- [threshold](ScreenSpaceReflectionPostProcess.md#threshold)
- [uniqueId](ScreenSpaceReflectionPostProcess.md#uniqueid)
- [width](ScreenSpaceReflectionPostProcess.md#width)

### Accessors

- [\_geometryBufferRenderer](ScreenSpaceReflectionPostProcess.md#_geometrybufferrenderer)
- [\_prePassRenderer](ScreenSpaceReflectionPostProcess.md#_prepassrenderer)
- [aspectRatio](ScreenSpaceReflectionPostProcess.md#aspectratio)
- [enableSmoothReflections](ScreenSpaceReflectionPostProcess.md#enablesmoothreflections)
- [inputTexture](ScreenSpaceReflectionPostProcess.md#inputtexture)
- [isSupported](ScreenSpaceReflectionPostProcess.md#issupported)
- [onActivate](ScreenSpaceReflectionPostProcess.md#onactivate)
- [onAfterRender](ScreenSpaceReflectionPostProcess.md#onafterrender)
- [onApply](ScreenSpaceReflectionPostProcess.md#onapply)
- [onBeforeRender](ScreenSpaceReflectionPostProcess.md#onbeforerender)
- [onSizeChanged](ScreenSpaceReflectionPostProcess.md#onsizechanged)
- [reflectionSamples](ScreenSpaceReflectionPostProcess.md#reflectionsamples)
- [samples](ScreenSpaceReflectionPostProcess.md#samples)
- [smoothSteps](ScreenSpaceReflectionPostProcess.md#smoothsteps)
- [texelSize](ScreenSpaceReflectionPostProcess.md#texelsize)

### Methods

- [\_updateEffectDefines](ScreenSpaceReflectionPostProcess.md#_updateeffectdefines)
- [activate](ScreenSpaceReflectionPostProcess.md#activate)
- [apply](ScreenSpaceReflectionPostProcess.md#apply)
- [clone](ScreenSpaceReflectionPostProcess.md#clone)
- [dispose](ScreenSpaceReflectionPostProcess.md#dispose)
- [getCamera](ScreenSpaceReflectionPostProcess.md#getcamera)
- [getClassName](ScreenSpaceReflectionPostProcess.md#getclassname)
- [getEffect](ScreenSpaceReflectionPostProcess.md#geteffect)
- [getEffectName](ScreenSpaceReflectionPostProcess.md#geteffectname)
- [getEngine](ScreenSpaceReflectionPostProcess.md#getengine)
- [isReady](ScreenSpaceReflectionPostProcess.md#isready)
- [isReusable](ScreenSpaceReflectionPostProcess.md#isreusable)
- [markTextureDirty](ScreenSpaceReflectionPostProcess.md#marktexturedirty)
- [restoreDefaultInputTexture](ScreenSpaceReflectionPostProcess.md#restoredefaultinputtexture)
- [serialize](ScreenSpaceReflectionPostProcess.md#serialize)
- [setPrePassRenderer](ScreenSpaceReflectionPostProcess.md#setprepassrenderer)
- [shareOutputWith](ScreenSpaceReflectionPostProcess.md#shareoutputwith)
- [updateEffect](ScreenSpaceReflectionPostProcess.md#updateeffect)
- [useOwnOutput](ScreenSpaceReflectionPostProcess.md#useownoutput)
- [Parse](ScreenSpaceReflectionPostProcess.md#parse)

## Constructors

### constructor

• **new ScreenSpaceReflectionPostProcess**(`name`, `scene`, `options`, `camera`, `samplingMode?`, `engine?`, `reusable?`, `textureType?`, `blockCompilation?`, `forceGeometryBuffer?`)

Creates a new instance of ScreenSpaceReflectionPostProcess.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | The name of the effect. |
| `scene` | [`Scene`](Scene.md) | `undefined` | The scene containing the objects to calculate reflections. |
| `options` | `number` \| [`PostProcessOptions`](../modules.md#postprocessoptions) | `undefined` | The required width/height ratio to downsize to before computing the render pass. |
| `camera` | [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md) | `undefined` | The camera to apply the render pass to. |
| `samplingMode?` | `number` | `undefined` | The sampling mode to be used when computing the pass. (default: 0) |
| `engine?` | [`Engine`](Engine.md) | `undefined` | The engine which the post process will be applied. (default: current engine) |
| `reusable?` | `boolean` | `undefined` | If the post process can be reused on the same frame. (default: false) |
| `textureType` | `number` | `Constants.TEXTURETYPE_UNSIGNED_INT` | Type of textures used when performing the post process. (default: 0) |
| `blockCompilation` | `boolean` | `false` | If compilation of the shader should not be done in the constructor. The updateEffect method can be used to compile the shader at a later time. (default: true) |
| `forceGeometryBuffer` | `boolean` | `false` | If this post process should use geometry buffer instead of prepass (default: false) |

#### Overrides

[PostProcess](PostProcess.md).[constructor](PostProcess.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/screenSpaceReflectionPostProcess.ts:92

## Properties

### \_enableSmoothReflections

• `Private` **\_enableSmoothReflections**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/screenSpaceReflectionPostProcess.ts:66

___

### \_forceGeometryBuffer

• `Private` **\_forceGeometryBuffer**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/screenSpaceReflectionPostProcess.ts:49

___

### \_indexParameters

• `Protected` **\_indexParameters**: `any`

#### Inherited from

[PostProcess](PostProcess.md).[_indexParameters](PostProcess.md#_indexparameters)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:211

___

### \_isSceneRightHanded

• `Private` **\_isSceneRightHanded**: `boolean`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/screenSpaceReflectionPostProcess.ts:69

___

### \_postProcessDefines

• `Protected` **\_postProcessDefines**: [`Nullable`](../modules.md#nullable)`string`

#### Inherited from

[PostProcess](PostProcess.md).[_postProcessDefines](PostProcess.md#_postprocessdefines)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:209

___

### \_reflectionSamples

• `Private` **\_reflectionSamples**: `number` = `64`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/screenSpaceReflectionPostProcess.ts:67

___

### \_scene

• `Protected` **\_scene**: [`Scene`](Scene.md)

#### Inherited from

[PostProcess](PostProcess.md).[_scene](PostProcess.md#_scene)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:173

___

### \_smoothSteps

• `Private` **\_smoothSteps**: `number` = `5`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/screenSpaceReflectionPostProcess.ts:68

___

### adaptScaleToCurrentViewport

• **adaptScaleToCurrentViewport**: `boolean` = `false`

Modify the scale of the post process to be the same as the viewport (default: false)

#### Inherited from

[PostProcess](PostProcess.md).[adaptScaleToCurrentViewport](PostProcess.md#adaptscaletocurrentviewport)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:170

___

### alphaConstants

• **alphaConstants**: [`Color4`](Color4.md)

Sets the setAlphaBlendConstants of the babylon engine

#### Inherited from

[PostProcess](PostProcess.md).[alphaConstants](PostProcess.md#alphaconstants)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:103

___

### alphaMode

• **alphaMode**: `number` = `Constants.ALPHA_DISABLE`

Type of alpha mode to use when performing the post process (default: Engine.ALPHA_DISABLE)

#### Inherited from

[PostProcess](PostProcess.md).[alphaMode](PostProcess.md#alphamode)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:98

___

### alwaysForcePOT

• **alwaysForcePOT**: `boolean` = `false`

Force textures to be a power of two (default: false)

#### Inherited from

[PostProcess](PostProcess.md).[alwaysForcePOT](PostProcess.md#alwaysforcepot)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:144

___

### animations

• **animations**: [`Animation`](Animation.md)[]

Animations to be used for the post processing

#### Inherited from

[PostProcess](PostProcess.md).[animations](PostProcess.md#animations)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:107

___

### autoClear

• **autoClear**: `boolean` = `true`

If the buffer needs to be cleared before applying the post process. (default: true)
Should be set to false if shader will overwrite all previous pixels.

#### Inherited from

[PostProcess](PostProcess.md).[autoClear](PostProcess.md#autoclear)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:93

___

### clearColor

• **clearColor**: [`Color4`](Color4.md)

Clear color to use when screen clearing

#### Inherited from

[PostProcess](PostProcess.md).[clearColor](PostProcess.md#clearcolor)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:87

___

### enablePixelPerfectMode

• **enablePixelPerfectMode**: `boolean` = `false`

Enable Pixel Perfect mode where texture is not scaled to be power of 2.
Can only be used on a single postprocess or on the last one of a chain. (default: false)

#### Inherited from

[PostProcess](PostProcess.md).[enablePixelPerfectMode](PostProcess.md#enablepixelperfectmode)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:114

___

### externalTextureSamplerBinding

• **externalTextureSamplerBinding**: `boolean` = `false`

if externalTextureSamplerBinding is true, the "apply" method won't bind the textureSampler texture, it is expected to be done by the "outside" (by the onApplyObservable observer most probably).
counter-productive in some cases because if the texture bound by "apply" is different from the currently texture bound, (the one set by the onApplyObservable observer, for eg) some
internal structures (materialContext) will be dirtified, which may impact performances

#### Inherited from

[PostProcess](PostProcess.md).[externalTextureSamplerBinding](PostProcess.md#externaltexturesamplerbinding)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:187

___

### forceFullscreenViewport

• **forceFullscreenViewport**: `boolean` = `true`

Force the postprocess to be applied without taking in account viewport

#### Inherited from

[PostProcess](PostProcess.md).[forceFullscreenViewport](PostProcess.md#forcefullscreenviewport)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:120

___

### height

• **height**: `number` = `-1`

Height of the texture to apply the post process on

#### Inherited from

[PostProcess](PostProcess.md).[height](PostProcess.md#height)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:65

___

### inspectableCustomProperties

• **inspectableCustomProperties**: [`IInspectable`](../interfaces/IInspectable.md)[]

List of inspectable custom properties (used by the Inspector)

**`See`**

https://doc.babylonjs.com/how_to/debug_layer#extensibility

#### Inherited from

[PostProcess](PostProcess.md).[inspectableCustomProperties](PostProcess.md#inspectablecustomproperties)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:126

___

### name

• **name**: `string`

Name of the PostProcess.

#### Inherited from

[PostProcess](PostProcess.md).[name](PostProcess.md#name)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:53

___

### nodeMaterialSource

• **nodeMaterialSource**: [`Nullable`](../modules.md#nullable)[`NodeMaterial`](NodeMaterial.md) = `null`

Gets the node material used to create this postprocess (null if the postprocess was manually created)

#### Inherited from

[PostProcess](PostProcess.md).[nodeMaterialSource](PostProcess.md#nodematerialsource)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:70

___

### onActivateObservable

• **onActivateObservable**: [`Observable`](Observable.md)[`Camera`](Camera.md)

An event triggered when the postprocess is activated.

#### Inherited from

[PostProcess](PostProcess.md).[onActivateObservable](PostProcess.md#onactivateobservable)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:236

___

### onAfterRenderObservable

• **onAfterRenderObservable**: [`Observable`](Observable.md)[`Effect`](Effect.md)

An event triggered after rendering the postprocess

#### Inherited from

[PostProcess](PostProcess.md).[onAfterRenderObservable](PostProcess.md#onafterrenderobservable)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:302

___

### onApplyObservable

• **onApplyObservable**: [`Observable`](Observable.md)[`Effect`](Effect.md)

An event triggered when the postprocess applies its effect.

#### Inherited from

[PostProcess](PostProcess.md).[onApplyObservable](PostProcess.md#onapplyobservable)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:270

___

### onBeforeRenderObservable

• **onBeforeRenderObservable**: [`Observable`](Observable.md)[`Effect`](Effect.md)

An event triggered before rendering the postprocess

#### Inherited from

[PostProcess](PostProcess.md).[onBeforeRenderObservable](PostProcess.md#onbeforerenderobservable)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:286

___

### onSizeChangedObservable

• **onSizeChangedObservable**: [`Observable`](Observable.md)[`PostProcess`](PostProcess.md)

An event triggered when the postprocess changes its size.

#### Inherited from

[PostProcess](PostProcess.md).[onSizeChangedObservable](PostProcess.md#onsizechangedobservable)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:254

___

### reflectionSpecularFalloffExponent

• **reflectionSpecularFalloffExponent**: `number` = `3`

Gets or sets the falloff exponent used while computing fresnel. More the exponent is high, more the reflections will be discrete.

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/screenSpaceReflectionPostProcess.ts:37

___

### renderTargetSamplingMode

• **renderTargetSamplingMode**: `number`

Sampling mode used by the shader
See https://doc.babylonjs.com/classes/3.1/texture

#### Inherited from

[PostProcess](PostProcess.md).[renderTargetSamplingMode](PostProcess.md#rendertargetsamplingmode)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:82

___

### roughnessFactor

• **roughnessFactor**: `number` = `0.2`

Gets or sets the factor applied when computing roughness. Default value is 0.2.

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/screenSpaceReflectionPostProcess.ts:47

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

[PostProcess](PostProcess.md).[scaleMode](PostProcess.md#scalemode)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:139

___

### step

• **step**: `number` = `1.0`

Gets or sets the step size used to iterate until the effect finds the color of the reflection's pixel. Typically in interval [0.1, 1.0]

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/screenSpaceReflectionPostProcess.ts:42

___

### strength

• **strength**: `number` = `1`

Gets or sets the current reflection strength. 1.0 is an ideal value but can be increased/decreased for particular results.

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/screenSpaceReflectionPostProcess.ts:32

___

### threshold

• **threshold**: `number` = `1.2`

Gets or sets a reflection threshold mainly used to adjust the reflection's height.

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/screenSpaceReflectionPostProcess.ts:27

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the post process

#### Inherited from

[PostProcess](PostProcess.md).[uniqueId](PostProcess.md#uniqueid)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:49

___

### width

• **width**: `number` = `-1`

Width of the texture to apply the post process on

#### Inherited from

[PostProcess](PostProcess.md).[width](PostProcess.md#width)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:59

## Accessors

### \_geometryBufferRenderer

• `Private` `get` **_geometryBufferRenderer**(): [`Nullable`](../modules.md#nullable)[`GeometryBufferRenderer`](GeometryBufferRenderer.md)

#### Returns

[`Nullable`](../modules.md#nullable)[`GeometryBufferRenderer`](GeometryBufferRenderer.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/screenSpaceReflectionPostProcess.ts:50

___

### \_prePassRenderer

• `Private` `get` **_prePassRenderer**(): [`Nullable`](../modules.md#nullable)[`PrePassRenderer`](PrePassRenderer.md)

#### Returns

[`Nullable`](../modules.md#nullable)[`PrePassRenderer`](PrePassRenderer.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/screenSpaceReflectionPostProcess.ts:58

___

### aspectRatio

• `get` **aspectRatio**(): `number`

The aspect ratio of the output texture.

#### Returns

`number`

#### Inherited from

PostProcess.aspectRatio

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:731

___

### enableSmoothReflections

• `get` **enableSmoothReflections**(): `boolean`

Gets whether or not smoothing reflections is enabled.
Enabling smoothing will require more GPU power and can generate a drop in FPS.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/screenSpaceReflectionPostProcess.ts:193

• `set` **enableSmoothReflections**(`enabled`): `void`

Sets whether or not smoothing reflections is enabled.
Enabling smoothing will require more GPU power and can generate a drop in FPS.

#### Parameters

| Name | Type |
| :------ | :------ |
| `enabled` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/screenSpaceReflectionPostProcess.ts:202

___

### inputTexture

• `get` **inputTexture**(): [`RenderTargetWrapper`](RenderTargetWrapper.md)

The input texture for this post process and the output texture of the previous post process. When added to a pipeline the previous post process will
render it's output into this texture and this texture will be used as textureSampler in the fragment shader of this post process.

#### Returns

[`RenderTargetWrapper`](RenderTargetWrapper.md)

#### Inherited from

PostProcess.inputTexture

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

PostProcess.inputTexture

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:323

___

### isSupported

• `get` **isSupported**(): `boolean`

If the post process is supported.

#### Returns

`boolean`

#### Inherited from

PostProcess.isSupported

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

#### Inherited from

PostProcess.onActivate

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

PostProcess.onAfterRender

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

PostProcess.onApply

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

PostProcess.onBeforeRender

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

PostProcess.onSizeChanged

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:260

___

### reflectionSamples

• `get` **reflectionSamples**(): `number`

Gets the number of samples taken while computing reflections. More samples count is high,
more the post-process wil require GPU power and can generate a drop in FPS. Basically in interval [25, 100].

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/screenSpaceReflectionPostProcess.ts:215

• `set` **reflectionSamples**(`samples`): `void`

Sets the number of samples taken while computing reflections. More samples count is high,
more the post-process wil require GPU power and can generate a drop in FPS. Basically in interval [25, 100].

#### Parameters

| Name | Type |
| :------ | :------ |
| `samples` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/screenSpaceReflectionPostProcess.ts:224

___

### samples

• `get` **samples**(): `number`

Number of sample textures (default: 1)

#### Returns

`number`

#### Inherited from

PostProcess.samples

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

PostProcess.samples

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:156

___

### smoothSteps

• `get` **smoothSteps**(): `number`

Gets the number of samples taken while smoothing reflections. More samples count is high,
more the post-process will require GPU power and can generate a drop in FPS.
Default value (5.0) work pretty well in all cases but can be adjusted.

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/screenSpaceReflectionPostProcess.ts:238

• `set` **smoothSteps**(`steps`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `steps` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/screenSpaceReflectionPostProcess.ts:248

___

### texelSize

• `get` **texelSize**(): [`Vector2`](Vector2.md)

Gets the texel size of the postprocess.
See https://en.wikipedia.org/wiki/Texel_(graphics)

#### Returns

[`Vector2`](Vector2.md)

#### Inherited from

PostProcess.texelSize

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:350

## Methods

### \_updateEffectDefines

▸ `Private` **_updateEffectDefines**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/screenSpaceReflectionPostProcess.ts:257

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

[PostProcess](PostProcess.md).[activate](PostProcess.md#activate)

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

[PostProcess](PostProcess.md).[apply](PostProcess.md#apply)

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

[PostProcess](PostProcess.md).[clone](PostProcess.md#clone)

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

[PostProcess](PostProcess.md).[dispose](PostProcess.md#dispose)

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

[PostProcess](PostProcess.md).[getCamera](PostProcess.md#getcamera)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:342

___

### getClassName

▸ **getClassName**(): `string`

Gets a string identifying the name of the class

#### Returns

`string`

"ScreenSpaceReflectionPostProcess" string

#### Overrides

[PostProcess](PostProcess.md).[getClassName](PostProcess.md#getclassname)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/screenSpaceReflectionPostProcess.ts:75

___

### getEffect

▸ **getEffect**(): [`Effect`](Effect.md)

The effect that is created when initializing the post process.

#### Returns

[`Effect`](Effect.md)

The created effect corresponding the the postprocess.

#### Inherited from

[PostProcess](PostProcess.md).[getEffect](PostProcess.md#geteffect)

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

[PostProcess](PostProcess.md).[getEffectName](PostProcess.md#geteffectname)

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

[PostProcess](PostProcess.md).[getEngine](PostProcess.md#getengine)

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

[PostProcess](PostProcess.md).[isReady](PostProcess.md#isready)

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

[PostProcess](PostProcess.md).[isReusable](PostProcess.md#isreusable)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:521

___

### markTextureDirty

▸ **markTextureDirty**(): `void`

invalidate frameBuffer to hint the postprocess to create a depth buffer

#### Returns

`void`

#### Inherited from

[PostProcess](PostProcess.md).[markTextureDirty](PostProcess.md#marktexturedirty)

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

[PostProcess](PostProcess.md).[restoreDefaultInputTexture](PostProcess.md#restoredefaultinputtexture)

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

[PostProcess](PostProcess.md).[serialize](PostProcess.md#serialize)

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

[PostProcess](PostProcess.md).[setPrePassRenderer](PostProcess.md#setprepassrenderer)

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

[PostProcess](PostProcess.md).[shareOutputWith](PostProcess.md#shareoutputwith)

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

#### Inherited from

[PostProcess](PostProcess.md).[updateEffect](PostProcess.md#updateeffect)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:493

___

### useOwnOutput

▸ **useOwnOutput**(): `void`

Reverses the effect of calling shareOutputWith and returns the post process back to its original state.
This should be called if the post process that shares output with this post process is disabled/disposed.

#### Returns

`void`

#### Inherited from

[PostProcess](PostProcess.md).[useOwnOutput](PostProcess.md#useownoutput)

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

[PostProcess](PostProcess.md).[Parse](PostProcess.md#parse)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/postProcess.ts:932
