[@dev/core](../README.md) / [Exports](../modules.md) / DefaultRenderingPipeline

# Class: DefaultRenderingPipeline

The default rendering pipeline can be added to a scene to apply common post processing effects such as anti-aliasing or depth of field.
See https://doc.babylonjs.com/how_to/using_default_rendering_pipeline

## Hierarchy

- [`PostProcessRenderPipeline`](PostProcessRenderPipeline.md)

  ↳ **`DefaultRenderingPipeline`**

## Implements

- [`IDisposable`](../interfaces/IDisposable.md)
- [`IAnimatable`](../interfaces/IAnimatable.md)

## Table of contents

### Constructors

- [constructor](DefaultRenderingPipeline.md#constructor)

### Properties

- [ChromaticAberrationPostProcessId](DefaultRenderingPipeline.md#chromaticaberrationpostprocessid)
- [GrainPostProcessId](DefaultRenderingPipeline.md#grainpostprocessid)
- [SharpenPostProcessId](DefaultRenderingPipeline.md#sharpenpostprocessid)
- [\_bloomEnabled](DefaultRenderingPipeline.md#_bloomenabled)
- [\_bloomKernel](DefaultRenderingPipeline.md#_bloomkernel)
- [\_bloomScale](DefaultRenderingPipeline.md#_bloomscale)
- [\_bloomThreshold](DefaultRenderingPipeline.md#_bloomthreshold)
- [\_bloomWeight](DefaultRenderingPipeline.md#_bloomweight)
- [\_buildAllowed](DefaultRenderingPipeline.md#_buildallowed)
- [\_camerasToBeAttached](DefaultRenderingPipeline.md#_camerastobeattached)
- [\_chromaticAberrationEffect](DefaultRenderingPipeline.md#_chromaticaberrationeffect)
- [\_chromaticAberrationEnabled](DefaultRenderingPipeline.md#_chromaticaberrationenabled)
- [\_defaultPipelineTextureType](DefaultRenderingPipeline.md#_defaultpipelinetexturetype)
- [\_depthOfFieldBlurLevel](DefaultRenderingPipeline.md#_depthoffieldblurlevel)
- [\_depthOfFieldEnabled](DefaultRenderingPipeline.md#_depthoffieldenabled)
- [\_depthOfFieldSceneObserver](DefaultRenderingPipeline.md#_depthoffieldsceneobserver)
- [\_fxaaEnabled](DefaultRenderingPipeline.md#_fxaaenabled)
- [\_glowLayer](DefaultRenderingPipeline.md#_glowlayer)
- [\_grainEffect](DefaultRenderingPipeline.md#_graineffect)
- [\_grainEnabled](DefaultRenderingPipeline.md#_grainenabled)
- [\_hardwareScaleLevel](DefaultRenderingPipeline.md#_hardwarescalelevel)
- [\_hasCleared](DefaultRenderingPipeline.md#_hascleared)
- [\_hdr](DefaultRenderingPipeline.md#_hdr)
- [\_imageProcessingConfigurationObserver](DefaultRenderingPipeline.md#_imageprocessingconfigurationobserver)
- [\_imageProcessingEnabled](DefaultRenderingPipeline.md#_imageprocessingenabled)
- [\_prevPostProcess](DefaultRenderingPipeline.md#_prevpostprocess)
- [\_prevPrevPostProcess](DefaultRenderingPipeline.md#_prevprevpostprocess)
- [\_resizeObserver](DefaultRenderingPipeline.md#_resizeobserver)
- [\_samples](DefaultRenderingPipeline.md#_samples)
- [\_scene](DefaultRenderingPipeline.md#_scene)
- [\_sharpenEffect](DefaultRenderingPipeline.md#_sharpeneffect)
- [\_sharpenEnabled](DefaultRenderingPipeline.md#_sharpenenabled)
- [animations](DefaultRenderingPipeline.md#animations)
- [bloom](DefaultRenderingPipeline.md#bloom)
- [chromaticAberration](DefaultRenderingPipeline.md#chromaticaberration)
- [depthOfField](DefaultRenderingPipeline.md#depthoffield)
- [fxaa](DefaultRenderingPipeline.md#fxaa)
- [grain](DefaultRenderingPipeline.md#grain)
- [imageProcessing](DefaultRenderingPipeline.md#imageprocessing)
- [inspectableCustomProperties](DefaultRenderingPipeline.md#inspectablecustomproperties)
- [onBuildObservable](DefaultRenderingPipeline.md#onbuildobservable)
- [sharpen](DefaultRenderingPipeline.md#sharpen)

### Accessors

- [bloomEnabled](DefaultRenderingPipeline.md#bloomenabled)
- [bloomKernel](DefaultRenderingPipeline.md#bloomkernel)
- [bloomScale](DefaultRenderingPipeline.md#bloomscale)
- [bloomThreshold](DefaultRenderingPipeline.md#bloomthreshold)
- [bloomWeight](DefaultRenderingPipeline.md#bloomweight)
- [cameras](DefaultRenderingPipeline.md#cameras)
- [chromaticAberrationEnabled](DefaultRenderingPipeline.md#chromaticaberrationenabled)
- [depthOfFieldBlurLevel](DefaultRenderingPipeline.md#depthoffieldblurlevel)
- [depthOfFieldEnabled](DefaultRenderingPipeline.md#depthoffieldenabled)
- [fxaaEnabled](DefaultRenderingPipeline.md#fxaaenabled)
- [glowLayer](DefaultRenderingPipeline.md#glowlayer)
- [glowLayerEnabled](DefaultRenderingPipeline.md#glowlayerenabled)
- [grainEnabled](DefaultRenderingPipeline.md#grainenabled)
- [imageProcessingEnabled](DefaultRenderingPipeline.md#imageprocessingenabled)
- [isSupported](DefaultRenderingPipeline.md#issupported)
- [name](DefaultRenderingPipeline.md#name)
- [samples](DefaultRenderingPipeline.md#samples)
- [scene](DefaultRenderingPipeline.md#scene)
- [sharpenEnabled](DefaultRenderingPipeline.md#sharpenenabled)

### Methods

- [\_buildPipeline](DefaultRenderingPipeline.md#_buildpipeline)
- [\_disposePostProcesses](DefaultRenderingPipeline.md#_disposepostprocesses)
- [\_enableMSAAOnFirstPostProcess](DefaultRenderingPipeline.md#_enablemsaaonfirstpostprocess)
- [\_rebuildBloom](DefaultRenderingPipeline.md#_rebuildbloom)
- [\_setAutoClearAndTextureSharing](DefaultRenderingPipeline.md#_setautoclearandtexturesharing)
- [addCamera](DefaultRenderingPipeline.md#addcamera)
- [addEffect](DefaultRenderingPipeline.md#addeffect)
- [dispose](DefaultRenderingPipeline.md#dispose)
- [getClassName](DefaultRenderingPipeline.md#getclassname)
- [prepare](DefaultRenderingPipeline.md#prepare)
- [removeCamera](DefaultRenderingPipeline.md#removecamera)
- [serialize](DefaultRenderingPipeline.md#serialize)
- [setPrePassRenderer](DefaultRenderingPipeline.md#setprepassrenderer)
- [Parse](DefaultRenderingPipeline.md#parse)

## Constructors

### constructor

• **new DefaultRenderingPipeline**(`name?`, `hdr?`, `scene?`, `cameras?`, `automaticBuild?`)

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `""` | The rendering pipeline name (default: "") |
| `hdr` | `boolean` | `true` | If high dynamic range textures should be used (default: true) |
| `scene` | [`Scene`](Scene.md) | `undefined` | The scene linked to this pipeline (default: the last created scene) |
| `cameras?` | [`Camera`](Camera.md)[] | `undefined` | The array of cameras that the rendering pipeline will be attached to (default: scene.cameras) |
| `automaticBuild` | `boolean` | `true` | if false, you will have to manually call prepare() to update the pipeline (default: true) |

#### Overrides

[PostProcessRenderPipeline](PostProcessRenderPipeline.md).[constructor](PostProcessRenderPipeline.md#constructor)

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:418

## Properties

### ChromaticAberrationPostProcessId

• `Private` `Readonly` **ChromaticAberrationPostProcessId**: `string` = `"ChromaticAberrationPostProcessEffect"`

ID of the chromatic aberration post process,

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:57

___

### GrainPostProcessId

• `Private` `Readonly` **GrainPostProcessId**: `string` = `"GrainPostProcessEffect"`

ID of the grain post process

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:61

___

### SharpenPostProcessId

• `Private` `Readonly` **SharpenPostProcessId**: `string` = `"SharpenPostProcessEffect"`

ID of the sharpen post process,

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:43

___

### \_bloomEnabled

• `Private` **\_bloomEnabled**: `boolean` = `false`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:105

___

### \_bloomKernel

• `Private` **\_bloomKernel**: `number` = `64`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:148

___

### \_bloomScale

• `Private` **\_bloomScale**: `number` = `0.5`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:111

___

### \_bloomThreshold

• `Private` **\_bloomThreshold**: `number` = `0.9`

Specifies the luma threshold for the area that will be blurred by the bloom

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:170

___

### \_bloomWeight

• `Private` **\_bloomWeight**: `number` = `0.15`

Specifies the weight of the bloom in the final rendering

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:165

___

### \_buildAllowed

• `Private` **\_buildAllowed**: `boolean` = `true`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:115

___

### \_camerasToBeAttached

• `Private` **\_camerasToBeAttached**: [`Camera`](Camera.md)[] = `[]`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:39

___

### \_chromaticAberrationEffect

• `Private` **\_chromaticAberrationEffect**: [`PostProcessRenderEffect`](PostProcessRenderEffect.md)

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:86

___

### \_chromaticAberrationEnabled

• `Private` **\_chromaticAberrationEnabled**: `boolean` = `false`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:112

___

### \_defaultPipelineTextureType

• `Private` **\_defaultPipelineTextureType**: `number`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:110

___

### \_depthOfFieldBlurLevel

• `Private` **\_depthOfFieldBlurLevel**: [`DepthOfFieldEffectBlurLevel`](../enums/DepthOfFieldEffectBlurLevel.md) = `DepthOfFieldEffectBlurLevel.Low`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:107

___

### \_depthOfFieldEnabled

• `Private` **\_depthOfFieldEnabled**: `boolean` = `false`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:106

___

### \_depthOfFieldSceneObserver

• `Private` **\_depthOfFieldSceneObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Scene`](Scene.md) = `null`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:555

___

### \_fxaaEnabled

• `Private` **\_fxaaEnabled**: `boolean` = `false`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:108

___

### \_glowLayer

• `Private` **\_glowLayer**: [`Nullable`](../modules.md#nullable)[`GlowLayer`](GlowLayer.md) = `null`

Glow post process which adds a glow to emissive areas of the image

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:95

___

### \_grainEffect

• `Private` **\_grainEffect**: [`PostProcessRenderEffect`](PostProcessRenderEffect.md)

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:91

___

### \_grainEnabled

• `Private` **\_grainEnabled**: `boolean` = `false`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:113

___

### \_hardwareScaleLevel

• `Private` **\_hardwareScaleLevel**: `number` = `1.0`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:147

___

### \_hasCleared

• `Private` **\_hasCleared**: `boolean` = `false`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:528

___

### \_hdr

• `Private` **\_hdr**: `boolean`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:173

___

### \_imageProcessingConfigurationObserver

• `Private` **\_imageProcessingConfigurationObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`ImageProcessingConfiguration`](ImageProcessingConfiguration.md) = `null`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:102

___

### \_imageProcessingEnabled

• `Private` **\_imageProcessingEnabled**: `boolean` = `true`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:109

___

### \_prevPostProcess

• `Private` **\_prevPostProcess**: [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md) = `null`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:529

___

### \_prevPrevPostProcess

• `Private` **\_prevPrevPostProcess**: [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md) = `null`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:530

___

### \_resizeObserver

• `Private` **\_resizeObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Engine`](Engine.md) = `null`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:146

___

### \_samples

• `Private` **\_samples**: `number` = `1`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:319

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:38

___

### \_sharpenEffect

• `Private` **\_sharpenEffect**: [`PostProcessRenderEffect`](PostProcessRenderEffect.md)

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:68

___

### \_sharpenEnabled

• `Private` **\_sharpenEnabled**: `boolean` = `false`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:104

___

### animations

• **animations**: [`Animation`](Animation.md)[] = `[]`

Animations which can be used to tweak settings over a period of time

#### Implementation of

[IAnimatable](../interfaces/IAnimatable.md).[animations](../interfaces/IAnimatable.md#animations)

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:100

___

### bloom

• `Private` **bloom**: [`BloomEffect`](BloomEffect.md)

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:69

___

### chromaticAberration

• **chromaticAberration**: [`ChromaticAberrationPostProcess`](ChromaticAberrationPostProcess.md)

Chromatic aberration post process which will shift rgb colors in the image

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:85

___

### depthOfField

• **depthOfField**: [`DepthOfFieldEffect`](DepthOfFieldEffect.md)

Depth of field effect, applies a blur based on how far away objects are from the focus distance.

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:73

___

### fxaa

• **fxaa**: [`FxaaPostProcess`](FxaaPostProcess.md)

The Fast Approximate Anti-Aliasing post process which attempts to remove aliasing from an image.

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:77

___

### grain

• **grain**: [`GrainPostProcess`](GrainPostProcess.md)

Grain post process which add noise to the image

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:90

___

### imageProcessing

• **imageProcessing**: [`ImageProcessingPostProcess`](ImageProcessingPostProcess.md)

Image post processing pass used to perform operations such as tone mapping or color grading.

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:81

___

### inspectableCustomProperties

• **inspectableCustomProperties**: [`IInspectable`](../interfaces/IInspectable.md)[]

List of inspectable custom properties (used by the Inspector)

**`See`**

https://doc.babylonjs.com/how_to/debug_layer#extensibility

#### Inherited from

[PostProcessRenderPipeline](PostProcessRenderPipeline.md).[inspectableCustomProperties](PostProcessRenderPipeline.md#inspectablecustomproperties)

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/postProcessRenderPipeline.ts:23

___

### onBuildObservable

• **onBuildObservable**: [`Observable`](Observable.md)[`DefaultRenderingPipeline`](DefaultRenderingPipeline.md)

This is triggered each time the pipeline has been built.

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:120

___

### sharpen

• **sharpen**: [`SharpenPostProcess`](SharpenPostProcess.md)

Sharpen post process which will apply a sharpen convolution to enhance edges

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:67

## Accessors

### bloomEnabled

• `get` **bloomEnabled**(): `boolean`

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:240

• `set` **bloomEnabled**(`enabled`): `void`

Enable or disable the bloom from the pipeline

#### Parameters

| Name | Type |
| :------ | :------ |
| `enabled` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:231

___

### bloomKernel

• `get` **bloomKernel**(): `number`

Specifies the size of the bloom blur kernel, relative to the final output size

#### Returns

`number`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:152

• `set` **bloomKernel**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:156

___

### bloomScale

• `get` **bloomScale**(): `number`

#### Returns

`number`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:223

• `set` **bloomScale**(`value`): `void`

The scale of the bloom, lower value will provide better performance.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:211

___

### bloomThreshold

• `get` **bloomThreshold**(): `number`

#### Returns

`number`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:203

• `set` **bloomThreshold**(`value`): `void`

The luminance threshold to find bright areas of the image to bloom.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:195

___

### bloomWeight

• `get` **bloomWeight**(): `number`

#### Returns

`number`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:187

• `set` **bloomWeight**(`value`): `void`

The strength of the bloom.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:178

___

### cameras

• `get` **cameras**(): [`Camera`](Camera.md)[]

Gets the list of attached cameras

#### Returns

[`Camera`](Camera.md)[]

#### Inherited from

PostProcessRenderPipeline.cameras

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/postProcessRenderPipeline.ts:42

___

### chromaticAberrationEnabled

• `get` **chromaticAberrationEnabled**(): `boolean`

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:389

• `set` **chromaticAberrationEnabled**(`enabled`): `void`

Enable or disable the chromaticAberration process from the pipeline

#### Parameters

| Name | Type |
| :------ | :------ |
| `enabled` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:380

___

### depthOfFieldBlurLevel

• `get` **depthOfFieldBlurLevel**(): [`DepthOfFieldEffectBlurLevel`](../enums/DepthOfFieldEffectBlurLevel.md)

Blur level of the depth of field effect. (Higher blur will effect performance)

#### Returns

[`DepthOfFieldEffectBlurLevel`](../enums/DepthOfFieldEffectBlurLevel.md)

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:275

• `set` **depthOfFieldBlurLevel**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`DepthOfFieldEffectBlurLevel`](../enums/DepthOfFieldEffectBlurLevel.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:280

___

### depthOfFieldEnabled

• `get` **depthOfFieldEnabled**(): `boolean`

If the depth of field is enabled.

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:258

• `set` **depthOfFieldEnabled**(`enabled`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `enabled` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:263

___

### fxaaEnabled

• `get` **fxaaEnabled**(): `boolean`

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:314

• `set` **fxaaEnabled**(`enabled`): `void`

If the anti aliasing is enabled.

#### Parameters

| Name | Type |
| :------ | :------ |
| `enabled` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:305

___

### glowLayer

• `get` **glowLayer**(): [`Nullable`](../modules.md#nullable)[`GlowLayer`](GlowLayer.md)

Gets the glow layer (or null if not defined)

#### Returns

[`Nullable`](../modules.md#nullable)[`GlowLayer`](GlowLayer.md)

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:373

___

### glowLayerEnabled

• `get` **glowLayerEnabled**(): `boolean`

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:365

• `set` **glowLayerEnabled**(`enabled`): `void`

If glow layer is enabled. (Adds a glow effect to emmissive materials)

#### Parameters

| Name | Type |
| :------ | :------ |
| `enabled` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:356

___

### grainEnabled

• `get` **grainEnabled**(): `boolean`

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:405

• `set` **grainEnabled**(`enabled`): `void`

Enable or disable the grain process from the pipeline

#### Parameters

| Name | Type |
| :------ | :------ |
| `enabled` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:396

___

### imageProcessingEnabled

• `get` **imageProcessingEnabled**(): `boolean`

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:348

• `set` **imageProcessingEnabled**(`enabled`): `void`

If image processing is enabled.

#### Parameters

| Name | Type |
| :------ | :------ |
| `enabled` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:340

___

### isSupported

• `get` **isSupported**(): `boolean`

If all the render effects in the pipeline are supported

#### Returns

`boolean`

#### Inherited from

PostProcessRenderPipeline.isSupported

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/postProcessRenderPipeline.ts:71

___

### name

• `get` **name**(): `string`

Gets pipeline name

#### Returns

`string`

#### Inherited from

PostProcessRenderPipeline.name

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/postProcessRenderPipeline.ts:37

___

### samples

• `get` **samples**(): `number`

#### Returns

`number`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:332

• `set` **samples**(`sampleCount`): `void`

MSAA sample count, setting this to 4 will provide 4x anti aliasing. (default: 1)

#### Parameters

| Name | Type |
| :------ | :------ |
| `sampleCount` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:323

___

### scene

• `get` **scene**(): [`Scene`](Scene.md)

Gets active scene

#### Returns

[`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:125

___

### sharpenEnabled

• `get` **sharpenEnabled**(): `boolean`

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:141

• `set` **sharpenEnabled**(`enabled`): `void`

Enable or disable the sharpen process from the pipeline

#### Parameters

| Name | Type |
| :------ | :------ |
| `enabled` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:132

## Methods

### \_buildPipeline

▸ `Private` **_buildPipeline**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:557

___

### \_disposePostProcesses

▸ `Private` **_disposePostProcesses**(`disposeNonRecreated?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `disposeNonRecreated` | `boolean` | `false` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:703

___

### \_enableMSAAOnFirstPostProcess

▸ `Protected` **_enableMSAAOnFirstPostProcess**(`sampleCount`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `sampleCount` | `number` |

#### Returns

`boolean`

#### Inherited from

[PostProcessRenderPipeline](PostProcessRenderPipeline.md).[_enableMSAAOnFirstPostProcess](PostProcessRenderPipeline.md#_enablemsaaonfirstpostprocess)

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/postProcessRenderPipeline.ts:228

___

### \_rebuildBloom

▸ `Private` **_rebuildBloom**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:245

___

### \_setAutoClearAndTextureSharing

▸ `Private` **_setAutoClearAndTextureSharing**(`postProcess`, `skipTextureSharing?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `postProcess` | [`PostProcess`](PostProcess.md) | `undefined` |
| `skipTextureSharing` | `boolean` | `false` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:532

___

### addCamera

▸ **addCamera**(`camera`): `void`

Adds a camera to the pipeline

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `camera` | [`Camera`](Camera.md) | the camera to be added |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:763

___

### addEffect

▸ **addEffect**(`renderEffect`): `void`

Adds an effect to the pipeline

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `renderEffect` | [`PostProcessRenderEffect`](PostProcessRenderEffect.md) | the effect to add |

#### Returns

`void`

#### Inherited from

[PostProcessRenderPipeline](PostProcessRenderPipeline.md).[addEffect](PostProcessRenderPipeline.md#addeffect)

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/postProcessRenderPipeline.ts:87

___

### dispose

▸ **dispose**(): `void`

Dispose of the pipeline and stop all post processes

#### Returns

`void`

#### Implementation of

[IDisposable](../interfaces/IDisposable.md).[dispose](../interfaces/IDisposable.md#dispose)

#### Overrides

[PostProcessRenderPipeline](PostProcessRenderPipeline.md).[dispose](PostProcessRenderPipeline.md#dispose)

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:781

___

### getClassName

▸ **getClassName**(): `string`

Get the class name

#### Returns

`string`

"DefaultRenderingPipeline"

#### Overrides

[PostProcessRenderPipeline](PostProcessRenderPipeline.md).[getClassName](PostProcessRenderPipeline.md#getclassname)

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:514

___

### prepare

▸ **prepare**(): `void`

Force the compilation of the entire pipeline.

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:521

___

### removeCamera

▸ **removeCamera**(`camera`): `void`

Removes a camera from the pipeline

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `camera` | [`Camera`](Camera.md) | the camera to remove |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:772

___

### serialize

▸ **serialize**(): `any`

Serialize the rendering pipeline (Used when exporting)

#### Returns

`any`

the serialized object

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:798

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

[PostProcessRenderPipeline](PostProcessRenderPipeline.md).[setPrePassRenderer](PostProcessRenderPipeline.md#setprepassrenderer)

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/postProcessRenderPipeline.ts:250

___

### Parse

▸ `Static` **Parse**(`source`, `scene`, `rootUrl`): [`DefaultRenderingPipeline`](DefaultRenderingPipeline.md)

Parse the serialized pipeline

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | `any` | Source pipeline. |
| `scene` | [`Scene`](Scene.md) | The scene to load the pipeline to. |
| `rootUrl` | `string` | The URL of the serialized pipeline. |

#### Returns

[`DefaultRenderingPipeline`](DefaultRenderingPipeline.md)

An instantiated pipeline from the serialized object.

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/defaultRenderingPipeline.ts:812
