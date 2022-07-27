[@dev/core](../README.md) / [Exports](../modules.md) / HighlightsPostProcess

# Class: HighlightsPostProcess

Extracts highlights from the image

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_postprocesses

## Hierarchy

- [`PostProcess`](PostProcess.md)

  ↳ **`HighlightsPostProcess`**

## Table of contents

### Constructors

- [constructor](HighlightsPostProcess.md#constructor)

### Properties

- [\_indexParameters](HighlightsPostProcess.md#_indexparameters)
- [\_postProcessDefines](HighlightsPostProcess.md#_postprocessdefines)
- [\_scene](HighlightsPostProcess.md#_scene)
- [adaptScaleToCurrentViewport](HighlightsPostProcess.md#adaptscaletocurrentviewport)
- [alphaConstants](HighlightsPostProcess.md#alphaconstants)
- [alphaMode](HighlightsPostProcess.md#alphamode)
- [alwaysForcePOT](HighlightsPostProcess.md#alwaysforcepot)
- [animations](HighlightsPostProcess.md#animations)
- [autoClear](HighlightsPostProcess.md#autoclear)
- [clearColor](HighlightsPostProcess.md#clearcolor)
- [enablePixelPerfectMode](HighlightsPostProcess.md#enablepixelperfectmode)
- [externalTextureSamplerBinding](HighlightsPostProcess.md#externaltexturesamplerbinding)
- [forceFullscreenViewport](HighlightsPostProcess.md#forcefullscreenviewport)
- [height](HighlightsPostProcess.md#height)
- [inspectableCustomProperties](HighlightsPostProcess.md#inspectablecustomproperties)
- [name](HighlightsPostProcess.md#name)
- [nodeMaterialSource](HighlightsPostProcess.md#nodematerialsource)
- [onActivateObservable](HighlightsPostProcess.md#onactivateobservable)
- [onAfterRenderObservable](HighlightsPostProcess.md#onafterrenderobservable)
- [onApplyObservable](HighlightsPostProcess.md#onapplyobservable)
- [onBeforeRenderObservable](HighlightsPostProcess.md#onbeforerenderobservable)
- [onSizeChangedObservable](HighlightsPostProcess.md#onsizechangedobservable)
- [renderTargetSamplingMode](HighlightsPostProcess.md#rendertargetsamplingmode)
- [scaleMode](HighlightsPostProcess.md#scalemode)
- [uniqueId](HighlightsPostProcess.md#uniqueid)
- [width](HighlightsPostProcess.md#width)

### Accessors

- [aspectRatio](HighlightsPostProcess.md#aspectratio)
- [inputTexture](HighlightsPostProcess.md#inputtexture)
- [isSupported](HighlightsPostProcess.md#issupported)
- [onActivate](HighlightsPostProcess.md#onactivate)
- [onAfterRender](HighlightsPostProcess.md#onafterrender)
- [onApply](HighlightsPostProcess.md#onapply)
- [onBeforeRender](HighlightsPostProcess.md#onbeforerender)
- [onSizeChanged](HighlightsPostProcess.md#onsizechanged)
- [samples](HighlightsPostProcess.md#samples)
- [texelSize](HighlightsPostProcess.md#texelsize)

### Methods

- [activate](HighlightsPostProcess.md#activate)
- [apply](HighlightsPostProcess.md#apply)
- [clone](HighlightsPostProcess.md#clone)
- [dispose](HighlightsPostProcess.md#dispose)
- [getCamera](HighlightsPostProcess.md#getcamera)
- [getClassName](HighlightsPostProcess.md#getclassname)
- [getEffect](HighlightsPostProcess.md#geteffect)
- [getEffectName](HighlightsPostProcess.md#geteffectname)
- [getEngine](HighlightsPostProcess.md#getengine)
- [isReady](HighlightsPostProcess.md#isready)
- [isReusable](HighlightsPostProcess.md#isreusable)
- [markTextureDirty](HighlightsPostProcess.md#marktexturedirty)
- [restoreDefaultInputTexture](HighlightsPostProcess.md#restoredefaultinputtexture)
- [serialize](HighlightsPostProcess.md#serialize)
- [setPrePassRenderer](HighlightsPostProcess.md#setprepassrenderer)
- [shareOutputWith](HighlightsPostProcess.md#shareoutputwith)
- [updateEffect](HighlightsPostProcess.md#updateeffect)
- [useOwnOutput](HighlightsPostProcess.md#useownoutput)
- [Parse](HighlightsPostProcess.md#parse)

## Constructors

### constructor

• **new HighlightsPostProcess**(`name`, `options`, `camera`, `samplingMode?`, `engine?`, `reusable?`, `textureType?`)

Extracts highlights from the image

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_postprocesses

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | The name of the effect. |
| `options` | `number` \| [`PostProcessOptions`](../modules.md#postprocessoptions) | `undefined` | The required width/height ratio to downsize to before computing the render pass. |
| `camera` | [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md) | `undefined` | The camera to apply the render pass to. |
| `samplingMode?` | `number` | `undefined` | The sampling mode to be used when computing the pass. (default: 0) |
| `engine?` | [`Engine`](Engine.md) | `undefined` | The engine which the post process will be applied. (default: current engine) |
| `reusable?` | `boolean` | `undefined` | If the post process can be reused on the same frame. (default: false) |
| `textureType` | `number` | `Constants.TEXTURETYPE_UNSIGNED_INT` | Type of texture for the post process (default: Engine.TEXTURETYPE_UNSIGNED_INT) |

#### Overrides

[PostProcess](PostProcess.md).[constructor](PostProcess.md#constructor)

#### Defined in

packages/dev/core/src/PostProcesses/highlightsPostProcess.ts:34

## Properties

### \_indexParameters

• `Protected` **\_indexParameters**: `any`

#### Inherited from

[PostProcess](PostProcess.md).[_indexParameters](PostProcess.md#_indexparameters)

#### Defined in

packages/dev/core/src/PostProcesses/postProcess.ts:211

___

### \_postProcessDefines

• `Protected` **\_postProcessDefines**: [`Nullable`](../modules.md#nullable)`string`

#### Inherited from

[PostProcess](PostProcess.md).[_postProcessDefines](PostProcess.md#_postprocessdefines)

#### Defined in

packages/dev/core/src/PostProcesses/postProcess.ts:209

___

### \_scene

• `Protected` **\_scene**: [`Scene`](Scene.md)

#### Inherited from

[PostProcess](PostProcess.md).[_scene](PostProcess.md#_scene)

#### Defined in

packages/dev/core/src/PostProcesses/postProcess.ts:173

___

### adaptScaleToCurrentViewport

• **adaptScaleToCurrentViewport**: `boolean` = `false`

Modify the scale of the post process to be the same as the viewport (default: false)

#### Inherited from

[PostProcess](PostProcess.md).[adaptScaleToCurrentViewport](PostProcess.md#adaptscaletocurrentviewport)

#### Defined in

packages/dev/core/src/PostProcesses/postProcess.ts:170

___

### alphaConstants

• **alphaConstants**: [`Color4`](Color4.md)

Sets the setAlphaBlendConstants of the babylon engine

#### Inherited from

[PostProcess](PostProcess.md).[alphaConstants](PostProcess.md#alphaconstants)

#### Defined in

packages/dev/core/src/PostProcesses/postProcess.ts:103

___

### alphaMode

• **alphaMode**: `number` = `Constants.ALPHA_DISABLE`

Type of alpha mode to use when performing the post process (default: Engine.ALPHA_DISABLE)

#### Inherited from

[PostProcess](PostProcess.md).[alphaMode](PostProcess.md#alphamode)

#### Defined in

packages/dev/core/src/PostProcesses/postProcess.ts:98

___

### alwaysForcePOT

• **alwaysForcePOT**: `boolean` = `false`

Force textures to be a power of two (default: false)

#### Inherited from

[PostProcess](PostProcess.md).[alwaysForcePOT](PostProcess.md#alwaysforcepot)

#### Defined in

packages/dev/core/src/PostProcesses/postProcess.ts:144

___

### animations

• **animations**: [`Animation`](Animation.md)[]

Animations to be used for the post processing

#### Inherited from

[PostProcess](PostProcess.md).[animations](PostProcess.md#animations)

#### Defined in

packages/dev/core/src/PostProcesses/postProcess.ts:107

___

### autoClear

• **autoClear**: `boolean` = `true`

If the buffer needs to be cleared before applying the post process. (default: true)
Should be set to false if shader will overwrite all previous pixels.

#### Inherited from

[PostProcess](PostProcess.md).[autoClear](PostProcess.md#autoclear)

#### Defined in

packages/dev/core/src/PostProcesses/postProcess.ts:93

___

### clearColor

• **clearColor**: [`Color4`](Color4.md)

Clear color to use when screen clearing

#### Inherited from

[PostProcess](PostProcess.md).[clearColor](PostProcess.md#clearcolor)

#### Defined in

packages/dev/core/src/PostProcesses/postProcess.ts:87

___

### enablePixelPerfectMode

• **enablePixelPerfectMode**: `boolean` = `false`

Enable Pixel Perfect mode where texture is not scaled to be power of 2.
Can only be used on a single postprocess or on the last one of a chain. (default: false)

#### Inherited from

[PostProcess](PostProcess.md).[enablePixelPerfectMode](PostProcess.md#enablepixelperfectmode)

#### Defined in

packages/dev/core/src/PostProcesses/postProcess.ts:114

___

### externalTextureSamplerBinding

• **externalTextureSamplerBinding**: `boolean` = `false`

if externalTextureSamplerBinding is true, the "apply" method won't bind the textureSampler texture, it is expected to be done by the "outside" (by the onApplyObservable observer most probably).
counter-productive in some cases because if the texture bound by "apply" is different from the currently texture bound, (the one set by the onApplyObservable observer, for eg) some
internal structures (materialContext) will be dirtified, which may impact performances

#### Inherited from

[PostProcess](PostProcess.md).[externalTextureSamplerBinding](PostProcess.md#externaltexturesamplerbinding)

#### Defined in

packages/dev/core/src/PostProcesses/postProcess.ts:187

___

### forceFullscreenViewport

• **forceFullscreenViewport**: `boolean` = `true`

Force the postprocess to be applied without taking in account viewport

#### Inherited from

[PostProcess](PostProcess.md).[forceFullscreenViewport](PostProcess.md#forcefullscreenviewport)

#### Defined in

packages/dev/core/src/PostProcesses/postProcess.ts:120

___

### height

• **height**: `number` = `-1`

Height of the texture to apply the post process on

#### Inherited from

[PostProcess](PostProcess.md).[height](PostProcess.md#height)

#### Defined in

packages/dev/core/src/PostProcesses/postProcess.ts:65

___

### inspectableCustomProperties

• **inspectableCustomProperties**: [`IInspectable`](../interfaces/IInspectable.md)[]

List of inspectable custom properties (used by the Inspector)

**`See`**

https://doc.babylonjs.com/how_to/debug_layer#extensibility

#### Inherited from

[PostProcess](PostProcess.md).[inspectableCustomProperties](PostProcess.md#inspectablecustomproperties)

#### Defined in

packages/dev/core/src/PostProcesses/postProcess.ts:126

___

### name

• **name**: `string`

Name of the PostProcess.

#### Inherited from

[PostProcess](PostProcess.md).[name](PostProcess.md#name)

#### Defined in

packages/dev/core/src/PostProcesses/postProcess.ts:53

___

### nodeMaterialSource

• **nodeMaterialSource**: [`Nullable`](../modules.md#nullable)[`NodeMaterial`](NodeMaterial.md) = `null`

Gets the node material used to create this postprocess (null if the postprocess was manually created)

#### Inherited from

[PostProcess](PostProcess.md).[nodeMaterialSource](PostProcess.md#nodematerialsource)

#### Defined in

packages/dev/core/src/PostProcesses/postProcess.ts:70

___

### onActivateObservable

• **onActivateObservable**: [`Observable`](Observable.md)[`Camera`](Camera.md)

An event triggered when the postprocess is activated.

#### Inherited from

[PostProcess](PostProcess.md).[onActivateObservable](PostProcess.md#onactivateobservable)

#### Defined in

packages/dev/core/src/PostProcesses/postProcess.ts:236

___

### onAfterRenderObservable

• **onAfterRenderObservable**: [`Observable`](Observable.md)[`Effect`](Effect.md)

An event triggered after rendering the postprocess

#### Inherited from

[PostProcess](PostProcess.md).[onAfterRenderObservable](PostProcess.md#onafterrenderobservable)

#### Defined in

packages/dev/core/src/PostProcesses/postProcess.ts:302

___

### onApplyObservable

• **onApplyObservable**: [`Observable`](Observable.md)[`Effect`](Effect.md)

An event triggered when the postprocess applies its effect.

#### Inherited from

[PostProcess](PostProcess.md).[onApplyObservable](PostProcess.md#onapplyobservable)

#### Defined in

packages/dev/core/src/PostProcesses/postProcess.ts:270

___

### onBeforeRenderObservable

• **onBeforeRenderObservable**: [`Observable`](Observable.md)[`Effect`](Effect.md)

An event triggered before rendering the postprocess

#### Inherited from

[PostProcess](PostProcess.md).[onBeforeRenderObservable](PostProcess.md#onbeforerenderobservable)

#### Defined in

packages/dev/core/src/PostProcesses/postProcess.ts:286

___

### onSizeChangedObservable

• **onSizeChangedObservable**: [`Observable`](Observable.md)[`PostProcess`](PostProcess.md)

An event triggered when the postprocess changes its size.

#### Inherited from

[PostProcess](PostProcess.md).[onSizeChangedObservable](PostProcess.md#onsizechangedobservable)

#### Defined in

packages/dev/core/src/PostProcesses/postProcess.ts:254

___

### renderTargetSamplingMode

• **renderTargetSamplingMode**: `number`

Sampling mode used by the shader
See https://doc.babylonjs.com/classes/3.1/texture

#### Inherited from

[PostProcess](PostProcess.md).[renderTargetSamplingMode](PostProcess.md#rendertargetsamplingmode)

#### Defined in

packages/dev/core/src/PostProcesses/postProcess.ts:82

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

packages/dev/core/src/PostProcesses/postProcess.ts:139

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the post process

#### Inherited from

[PostProcess](PostProcess.md).[uniqueId](PostProcess.md#uniqueid)

#### Defined in

packages/dev/core/src/PostProcesses/postProcess.ts:49

___

### width

• **width**: `number` = `-1`

Width of the texture to apply the post process on

#### Inherited from

[PostProcess](PostProcess.md).[width](PostProcess.md#width)

#### Defined in

packages/dev/core/src/PostProcesses/postProcess.ts:59

## Accessors

### aspectRatio

• `get` **aspectRatio**(): `number`

The aspect ratio of the output texture.

#### Returns

`number`

#### Inherited from

PostProcess.aspectRatio

#### Defined in

packages/dev/core/src/PostProcesses/postProcess.ts:731

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

packages/dev/core/src/PostProcesses/postProcess.ts:319

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

packages/dev/core/src/PostProcesses/postProcess.ts:323

___

### isSupported

• `get` **isSupported**(): `boolean`

If the post process is supported.

#### Returns

`boolean`

#### Inherited from

PostProcess.isSupported

#### Defined in

packages/dev/core/src/PostProcesses/postProcess.ts:724

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

packages/dev/core/src/PostProcesses/postProcess.ts:242

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

packages/dev/core/src/PostProcesses/postProcess.ts:308

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

packages/dev/core/src/PostProcesses/postProcess.ts:276

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

packages/dev/core/src/PostProcesses/postProcess.ts:292

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

packages/dev/core/src/PostProcesses/postProcess.ts:260

___

### samples

• `get` **samples**(): `number`

Number of sample textures (default: 1)

#### Returns

`number`

#### Inherited from

PostProcess.samples

#### Defined in

packages/dev/core/src/PostProcesses/postProcess.ts:152

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

packages/dev/core/src/PostProcesses/postProcess.ts:156

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

packages/dev/core/src/PostProcesses/postProcess.ts:350

## Methods

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

packages/dev/core/src/PostProcesses/postProcess.ts:614

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

packages/dev/core/src/PostProcesses/postProcess.ts:754

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

packages/dev/core/src/PostProcesses/postProcess.ts:903

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

packages/dev/core/src/PostProcesses/postProcess.ts:830

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

packages/dev/core/src/PostProcesses/postProcess.ts:342

___

### getClassName

▸ **getClassName**(): `string`

Gets a string identifying the name of the class

#### Returns

`string`

"HighlightsPostProcess" string

#### Overrides

[PostProcess](PostProcess.md).[getClassName](PostProcess.md#getclassname)

#### Defined in

packages/dev/core/src/PostProcesses/highlightsPostProcess.ts:19

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

packages/dev/core/src/PostProcesses/postProcess.ts:453

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

packages/dev/core/src/PostProcesses/postProcess.ts:227

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

packages/dev/core/src/PostProcesses/postProcess.ts:445

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

packages/dev/core/src/PostProcesses/postProcess.ts:746

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

packages/dev/core/src/PostProcesses/postProcess.ts:521

___

### markTextureDirty

▸ **markTextureDirty**(): `void`

invalidate frameBuffer to hint the postprocess to create a depth buffer

#### Returns

`void`

#### Inherited from

[PostProcess](PostProcess.md).[markTextureDirty](PostProcess.md#marktexturedirty)

#### Defined in

packages/dev/core/src/PostProcesses/postProcess.ts:526

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

packages/dev/core/src/PostProcesses/postProcess.ts:331

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

packages/dev/core/src/PostProcesses/postProcess.ts:880

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

packages/dev/core/src/PostProcesses/postProcess.ts:816

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

packages/dev/core/src/PostProcesses/postProcess.ts:462

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

packages/dev/core/src/PostProcesses/postProcess.ts:493

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

packages/dev/core/src/PostProcesses/postProcess.ts:474

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

packages/dev/core/src/PostProcesses/postProcess.ts:932
