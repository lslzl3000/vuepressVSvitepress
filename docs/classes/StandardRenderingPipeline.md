[@dev/core](../README.md) / [Exports](../modules.md) / StandardRenderingPipeline

# Class: StandardRenderingPipeline

Standard rendering pipeline
Default pipeline should be used going forward but the standard pipeline will be kept for backwards compatibility.

**`See`**

https://doc.babylonjs.com/how_to/using_standard_rendering_pipeline

## Hierarchy

- [`PostProcessRenderPipeline`](PostProcessRenderPipeline.md)

  ↳ **`StandardRenderingPipeline`**

## Implements

- [`IDisposable`](../interfaces/IDisposable.md)
- [`IAnimatable`](../interfaces/IAnimatable.md)

## Table of contents

### Constructors

- [constructor](StandardRenderingPipeline.md#constructor)

### Properties

- [\_basePostProcess](StandardRenderingPipeline.md#_basepostprocess)
- [\_bloomEnabled](StandardRenderingPipeline.md#_bloomenabled)
- [\_camerasToBeAttached](StandardRenderingPipeline.md#_camerastobeattached)
- [\_currentDepthOfFieldSource](StandardRenderingPipeline.md#_currentdepthoffieldsource)
- [\_currentExposure](StandardRenderingPipeline.md#_currentexposure)
- [\_depthOfFieldEnabled](StandardRenderingPipeline.md#_depthoffieldenabled)
- [\_fixedExposure](StandardRenderingPipeline.md#_fixedexposure)
- [\_floatTextureType](StandardRenderingPipeline.md#_floattexturetype)
- [\_fxaaEnabled](StandardRenderingPipeline.md#_fxaaenabled)
- [\_hdrAutoExposure](StandardRenderingPipeline.md#_hdrautoexposure)
- [\_hdrCurrentLuminance](StandardRenderingPipeline.md#_hdrcurrentluminance)
- [\_hdrEnabled](StandardRenderingPipeline.md#_hdrenabled)
- [\_isObjectBasedMotionBlur](StandardRenderingPipeline.md#_isobjectbasedmotionblur)
- [\_lensFlareEnabled](StandardRenderingPipeline.md#_lensflareenabled)
- [\_motionBlurEnabled](StandardRenderingPipeline.md#_motionblurenabled)
- [\_motionBlurSamples](StandardRenderingPipeline.md#_motionblursamples)
- [\_motionStrength](StandardRenderingPipeline.md#_motionstrength)
- [\_ratio](StandardRenderingPipeline.md#_ratio)
- [\_samples](StandardRenderingPipeline.md#_samples)
- [\_scene](StandardRenderingPipeline.md#_scene)
- [\_screenSpaceReflectionsEnabled](StandardRenderingPipeline.md#_screenspacereflectionsenabled)
- [\_vlsEnabled](StandardRenderingPipeline.md#_vlsenabled)
- [\_volumetricLightStepsCount](StandardRenderingPipeline.md#_volumetriclightstepscount)
- [animations](StandardRenderingPipeline.md#animations)
- [blurHPostProcesses](StandardRenderingPipeline.md#blurhpostprocesses)
- [blurVPostProcesses](StandardRenderingPipeline.md#blurvpostprocesses)
- [blurWidth](StandardRenderingPipeline.md#blurwidth)
- [brightPassPostProcess](StandardRenderingPipeline.md#brightpasspostprocess)
- [brightThreshold](StandardRenderingPipeline.md#brightthreshold)
- [depthOfFieldBlurWidth](StandardRenderingPipeline.md#depthoffieldblurwidth)
- [depthOfFieldDistance](StandardRenderingPipeline.md#depthoffielddistance)
- [depthOfFieldPostProcess](StandardRenderingPipeline.md#depthoffieldpostprocess)
- [downSampleX4PostProcess](StandardRenderingPipeline.md#downsamplex4postprocess)
- [fxaaPostProcess](StandardRenderingPipeline.md#fxaapostprocess)
- [hdrDecreaseRate](StandardRenderingPipeline.md#hdrdecreaserate)
- [hdrFinalPostProcess](StandardRenderingPipeline.md#hdrfinalpostprocess)
- [hdrIncreaseRate](StandardRenderingPipeline.md#hdrincreaserate)
- [hdrMinimumLuminance](StandardRenderingPipeline.md#hdrminimumluminance)
- [hdrPostProcess](StandardRenderingPipeline.md#hdrpostprocess)
- [horizontalBlur](StandardRenderingPipeline.md#horizontalblur)
- [inspectableCustomProperties](StandardRenderingPipeline.md#inspectablecustomproperties)
- [lensColorTexture](StandardRenderingPipeline.md#lenscolortexture)
- [lensFlareBlurWidth](StandardRenderingPipeline.md#lensflareblurwidth)
- [lensFlareComposePostProcess](StandardRenderingPipeline.md#lensflarecomposepostprocess)
- [lensFlareDirtTexture](StandardRenderingPipeline.md#lensflaredirttexture)
- [lensFlareDistortionStrength](StandardRenderingPipeline.md#lensflaredistortionstrength)
- [lensFlareFinalPostProcess](StandardRenderingPipeline.md#lensflarefinalpostprocess)
- [lensFlareGhostDispersal](StandardRenderingPipeline.md#lensflareghostdispersal)
- [lensFlareHaloWidth](StandardRenderingPipeline.md#lensflarehalowidth)
- [lensFlarePostProcess](StandardRenderingPipeline.md#lensflarepostprocess)
- [lensFlareStrength](StandardRenderingPipeline.md#lensflarestrength)
- [lensStarTexture](StandardRenderingPipeline.md#lensstartexture)
- [lensTexture](StandardRenderingPipeline.md#lenstexture)
- [luminanceDownSamplePostProcesses](StandardRenderingPipeline.md#luminancedownsamplepostprocesses)
- [luminancePostProcess](StandardRenderingPipeline.md#luminancepostprocess)
- [motionBlurPostProcess](StandardRenderingPipeline.md#motionblurpostprocess)
- [originalPostProcess](StandardRenderingPipeline.md#originalpostprocess)
- [screenSpaceReflectionPostProcess](StandardRenderingPipeline.md#screenspacereflectionpostprocess)
- [sourceLight](StandardRenderingPipeline.md#sourcelight)
- [textureAdderFinalPostProcess](StandardRenderingPipeline.md#textureadderfinalpostprocess)
- [textureAdderPostProcess](StandardRenderingPipeline.md#textureadderpostprocess)
- [volumetricLightBlurScale](StandardRenderingPipeline.md#volumetriclightblurscale)
- [volumetricLightCoefficient](StandardRenderingPipeline.md#volumetriclightcoefficient)
- [volumetricLightFinalPostProcess](StandardRenderingPipeline.md#volumetriclightfinalpostprocess)
- [volumetricLightMergePostProces](StandardRenderingPipeline.md#volumetriclightmergepostproces)
- [volumetricLightPostProcess](StandardRenderingPipeline.md#volumetriclightpostprocess)
- [volumetricLightPower](StandardRenderingPipeline.md#volumetriclightpower)
- [volumetricLightSmoothXPostProcess](StandardRenderingPipeline.md#volumetriclightsmoothxpostprocess)
- [volumetricLightSmoothYPostProcess](StandardRenderingPipeline.md#volumetriclightsmoothypostprocess)
- [LuminanceSteps](StandardRenderingPipeline.md#luminancesteps)

### Accessors

- [BloomEnabled](StandardRenderingPipeline.md#bloomenabled)
- [DepthOfFieldEnabled](StandardRenderingPipeline.md#depthoffieldenabled)
- [HDREnabled](StandardRenderingPipeline.md#hdrenabled)
- [LensFlareEnabled](StandardRenderingPipeline.md#lensflareenabled)
- [MotionBlurEnabled](StandardRenderingPipeline.md#motionblurenabled)
- [VLSEnabled](StandardRenderingPipeline.md#vlsenabled)
- [cameras](StandardRenderingPipeline.md#cameras)
- [exposure](StandardRenderingPipeline.md#exposure)
- [fxaaEnabled](StandardRenderingPipeline.md#fxaaenabled)
- [hdrAutoExposure](StandardRenderingPipeline.md#hdrautoexposure)
- [isSupported](StandardRenderingPipeline.md#issupported)
- [motionBlurSamples](StandardRenderingPipeline.md#motionblursamples)
- [motionStrength](StandardRenderingPipeline.md#motionstrength)
- [name](StandardRenderingPipeline.md#name)
- [objectBasedMotionBlur](StandardRenderingPipeline.md#objectbasedmotionblur)
- [samples](StandardRenderingPipeline.md#samples)
- [screenSpaceReflectionsEnabled](StandardRenderingPipeline.md#screenspacereflectionsenabled)
- [volumetricLightStepsCount](StandardRenderingPipeline.md#volumetriclightstepscount)

### Methods

- [\_buildPipeline](StandardRenderingPipeline.md#_buildpipeline)
- [\_createBlurPostProcesses](StandardRenderingPipeline.md#_createblurpostprocesses)
- [\_createBrightPassPostProcess](StandardRenderingPipeline.md#_createbrightpasspostprocess)
- [\_createDepthOfFieldPostProcess](StandardRenderingPipeline.md#_createdepthoffieldpostprocess)
- [\_createDownSampleX4PostProcess](StandardRenderingPipeline.md#_createdownsamplex4postprocess)
- [\_createHdrPostProcess](StandardRenderingPipeline.md#_createhdrpostprocess)
- [\_createLensFlarePostProcess](StandardRenderingPipeline.md#_createlensflarepostprocess)
- [\_createLuminancePostProcesses](StandardRenderingPipeline.md#_createluminancepostprocesses)
- [\_createMotionBlurPostProcess](StandardRenderingPipeline.md#_createmotionblurpostprocess)
- [\_createTextureAdderPostProcess](StandardRenderingPipeline.md#_createtextureadderpostprocess)
- [\_createVolumetricLightPostProcess](StandardRenderingPipeline.md#_createvolumetriclightpostprocess)
- [\_disposePostProcesses](StandardRenderingPipeline.md#_disposepostprocesses)
- [\_enableMSAAOnFirstPostProcess](StandardRenderingPipeline.md#_enablemsaaonfirstpostprocess)
- [\_getDepthTexture](StandardRenderingPipeline.md#_getdepthtexture)
- [addEffect](StandardRenderingPipeline.md#addeffect)
- [dispose](StandardRenderingPipeline.md#dispose)
- [getClassName](StandardRenderingPipeline.md#getclassname)
- [serialize](StandardRenderingPipeline.md#serialize)
- [setPrePassRenderer](StandardRenderingPipeline.md#setprepassrenderer)
- [Parse](StandardRenderingPipeline.md#parse)

## Constructors

### constructor

• **new StandardRenderingPipeline**(`name`, `scene`, `ratio`, `originalPostProcess?`, `cameras?`)

Default pipeline should be used going forward but the standard pipeline will be kept for backwards compatibility.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | The rendering pipeline name |
| `scene` | [`Scene`](Scene.md) | `undefined` | The scene linked to this pipeline |
| `ratio` | `number` | `undefined` | The size of the postprocesses (0.5 means that your postprocess will have a width = canvas.width 0.5 and a height = canvas.height 0.5) |
| `originalPostProcess` | [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md) | `null` | the custom original color post-process. Must be "reusable". Can be null. |
| `cameras?` | [`Camera`](Camera.md)[] | `undefined` | The array of cameras that the rendering pipeline will be attached to |

#### Overrides

[PostProcessRenderPipeline](PostProcessRenderPipeline.md).[constructor](PostProcessRenderPipeline.md#constructor)

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:584

## Properties

### \_basePostProcess

• `Private` **\_basePostProcess**: [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:338

___

### \_bloomEnabled

• `Private` **\_bloomEnabled**: `boolean` = `false`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:355

___

### \_camerasToBeAttached

• `Private` **\_camerasToBeAttached**: [`Camera`](Camera.md)[] = `[]`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:349

___

### \_currentDepthOfFieldSource

• `Private` **\_currentDepthOfFieldSource**: [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md) = `null`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:337

___

### \_currentExposure

• `Private` **\_currentExposure**: `number` = `1.0`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:341

___

### \_depthOfFieldEnabled

• `Private` **\_depthOfFieldEnabled**: `boolean` = `false`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:356

___

### \_fixedExposure

• `Private` **\_fixedExposure**: `number` = `1.0`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:340

___

### \_floatTextureType

• `Private` **\_floatTextureType**: `number`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:347

___

### \_fxaaEnabled

• `Private` **\_fxaaEnabled**: `boolean` = `false`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:361

___

### \_hdrAutoExposure

• `Private` **\_hdrAutoExposure**: `boolean` = `false`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:342

___

### \_hdrCurrentLuminance

• `Private` **\_hdrCurrentLuminance**: `number` = `1.0`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:343

___

### \_hdrEnabled

• `Private` **\_hdrEnabled**: `boolean` = `false`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:359

___

### \_isObjectBasedMotionBlur

• `Private` **\_isObjectBasedMotionBlur**: `boolean` = `false`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:345

___

### \_lensFlareEnabled

• `Private` **\_lensFlareEnabled**: `boolean` = `false`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:358

___

### \_motionBlurEnabled

• `Private` **\_motionBlurEnabled**: `boolean` = `false`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:360

___

### \_motionBlurSamples

• `Private` **\_motionBlurSamples**: `number` = `64.0`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:364

___

### \_motionStrength

• `Private` **\_motionStrength**: `number` = `1.0`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:344

___

### \_ratio

• `Private` **\_ratio**: `number`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:352

___

### \_samples

• `Private` **\_samples**: `number` = `1`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:366

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

Private members

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:336

___

### \_screenSpaceReflectionsEnabled

• `Private` **\_screenSpaceReflectionsEnabled**: `boolean` = `false`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:362

___

### \_vlsEnabled

• `Private` **\_vlsEnabled**: `boolean` = `false`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:357

___

### \_volumetricLightStepsCount

• `Private` **\_volumetricLightStepsCount**: `number` = `50.0`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:365

___

### animations

• **animations**: [`Animation`](Animation.md)[] = `[]`

List of animations for the pipeline (IAnimatable implementation)

#### Implementation of

[IAnimatable](../interfaces/IAnimatable.md).[animations](../interfaces/IAnimatable.md#animations)

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:331

___

### blurHPostProcesses

• **blurHPostProcesses**: [`PostProcess`](PostProcess.md)[] = `[]`

Post-process array storing all the horizontal blur post-processes used by the pipeline

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:56

___

### blurVPostProcesses

• **blurVPostProcesses**: [`PostProcess`](PostProcess.md)[] = `[]`

Post-process array storing all the vertical blur post-processes used by the pipeline

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:60

___

### blurWidth

• **blurWidth**: `number` = `512.0`

Configures the blur intensity used for surexposed surfaces are highlighted surfaces (light halo)

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:150

___

### brightPassPostProcess

• **brightPassPostProcess**: [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md) = `null`

Post-process used to calculate the illuminated surfaces controlled by a threshold

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:52

___

### brightThreshold

• **brightThreshold**: `number` = `1.0`

Represents the brightness threshold in order to configure the illuminated surfaces

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:144

___

### depthOfFieldBlurWidth

• **depthOfFieldBlurWidth**: `number` = `64.0`

Represents the blur intensity for the blurred part of the depth of field effect

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:289

___

### depthOfFieldDistance

• **depthOfFieldDistance**: `number` = `10.0`

Represents the focal length for the depth of field effect

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:284

___

### depthOfFieldPostProcess

• **depthOfFieldPostProcess**: [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md) = `null`

Post-process used to create a depth of field effect

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:128

___

### downSampleX4PostProcess

• **downSampleX4PostProcess**: [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md) = `null`

Post-process used to down scale an image x4

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:48

___

### fxaaPostProcess

• **fxaaPostProcess**: [`Nullable`](../modules.md#nullable)[`FxaaPostProcess`](FxaaPostProcess.md) = `null`

The Fast Approximate Anti-Aliasing post process which attempts to remove aliasing from an image.

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:132

___

### hdrDecreaseRate

• **hdrDecreaseRate**: `number` = `0.5`

For eye adaptation, represents the decrease luminance speed

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:209

___

### hdrFinalPostProcess

• **hdrFinalPostProcess**: [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md) = `null`

Post-process used to merge the final HDR post-process and the real scene color

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:112

___

### hdrIncreaseRate

• **hdrIncreaseRate**: `number` = `0.5`

For eye adaptation, represents the increase luminance speed

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:214

___

### hdrMinimumLuminance

• **hdrMinimumLuminance**: `number` = `1.0`

For eye adaptation, represents the minimum luminance the eye can see

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:204

___

### hdrPostProcess

• **hdrPostProcess**: [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md) = `null`

Post-process used to create a HDR effect (light adaptation)

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:100

___

### horizontalBlur

• **horizontalBlur**: `boolean` = `false`

Sets if the blur for highlighted surfaces must be only horizontal

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:155

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

### lensColorTexture

• **lensColorTexture**: [`Nullable`](../modules.md#nullable)[`Texture`](Texture.md) = `null`

Lens color texture used by the lens flare effect. Mandatory if lens flare effect enabled

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:240

___

### lensFlareBlurWidth

• **lensFlareBlurWidth**: `number` = `512.0`

Configures the blur intensity used for for lens flare (halo)

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:266

___

### lensFlareComposePostProcess

• **lensFlareComposePostProcess**: [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md) = `null`

Post-process that merges the result of the lens flare post-process and the real scene color

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:120

___

### lensFlareDirtTexture

• **lensFlareDirtTexture**: [`Nullable`](../modules.md#nullable)[`Texture`](Texture.md) = `null`

As the "lensTexture" (can be the same texture or different), it is used to apply the lens
flare effect by taking account of the dirt texture

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:278

___

### lensFlareDistortionStrength

• **lensFlareDistortionStrength**: `number` = `16.0`

Based on the lens distortion effect, defines how much the lens flare result
is distorted

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:261

___

### lensFlareFinalPostProcess

• **lensFlareFinalPostProcess**: [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md) = `null`

Post-process used to store the final lens flare post-process (attach/detach for debug purpose)

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:108

___

### lensFlareGhostDispersal

• **lensFlareGhostDispersal**: `number` = `1.4`

Dispersion coefficient for lens flare ghosts

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:250

___

### lensFlareHaloWidth

• **lensFlareHaloWidth**: `number` = `0.7`

Main lens flare halo width

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:255

___

### lensFlarePostProcess

• **lensFlarePostProcess**: [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md) = `null`

Post-process used to create a lens flare effect

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:116

___

### lensFlareStrength

• **lensFlareStrength**: `number` = `20.0`

The overall strength for the lens flare effect

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:245

___

### lensStarTexture

• **lensStarTexture**: [`Nullable`](../modules.md#nullable)[`Texture`](Texture.md) = `null`

Lens star texture must be used to simulate rays on the flares and is available
in the documentation

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:272

___

### lensTexture

• **lensTexture**: [`Nullable`](../modules.md#nullable)[`Texture`](Texture.md) = `null`

Texture used typically to simulate "dirty" on camera lens

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:176

___

### luminanceDownSamplePostProcesses

• **luminanceDownSamplePostProcesses**: [`PostProcess`](PostProcess.md)[] = `[]`

Post-processes used to create down sample post-processes in order to get
the average luminance of the final image for HDR
Array of length "StandardRenderingPipeline.LuminanceSteps"

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:96

___

### luminancePostProcess

• **luminancePostProcess**: [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md) = `null`

Base post-process used to calculate the average luminance of the final image for HDR

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:90

___

### motionBlurPostProcess

• **motionBlurPostProcess**: [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md) = `null`

Post-process used to create a motion blur effect

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:124

___

### originalPostProcess

• **originalPostProcess**: [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)

Post-process which contains the original scene color before the pipeline applies all the effects

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:44

___

### screenSpaceReflectionPostProcess

• **screenSpaceReflectionPostProcess**: [`Nullable`](../modules.md#nullable)[`ScreenSpaceReflectionPostProcess`](ScreenSpaceReflectionPostProcess.md) = `null`

Post-process used to simulate realtime reflections using the screen space and geometry renderer.

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:136

___

### sourceLight

• **sourceLight**: [`Nullable`](../modules.md#nullable)[`DirectionalLight`](DirectionalLight.md) \| [`SpotLight`](SpotLight.md) = `null`

Light (spot or directional) used to generate the volumetric lights rays
The source light must have a shadow generate so the pipeline can get its
depth map

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:198

___

### textureAdderFinalPostProcess

• **textureAdderFinalPostProcess**: [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md) = `null`

Post-process used to store the final texture adder post-process (attach/detach for debug purpose)

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:104

___

### textureAdderPostProcess

• **textureAdderPostProcess**: [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md) = `null`

Post-process used to add colors of 2 textures (typically brightness + real scene color)

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:64

___

### volumetricLightBlurScale

• **volumetricLightBlurScale**: `number` = `64.0`

Used the set the blur intensity to smooth the volumetric lights

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:192

___

### volumetricLightCoefficient

• **volumetricLightCoefficient**: `number` = `0.2`

Represents the offset coefficient based on Rayleigh principle. Typically in interval [-0.2, 0.2]

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:182

___

### volumetricLightFinalPostProcess

• **volumetricLightFinalPostProcess**: [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md) = `null`

Post-process used to store the final volumetric light post-process (attach/detach for debug purpose)

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:85

___

### volumetricLightMergePostProces

• **volumetricLightMergePostProces**: [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md) = `null`

Post-process used to merge the volumetric light effect and the real scene color

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:81

___

### volumetricLightPostProcess

• **volumetricLightPostProcess**: [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md) = `null`

Post-process used to create volumetric lighting effect

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:69

___

### volumetricLightPower

• **volumetricLightPower**: `number` = `4.0`

The overall power of volumetric lights, typically in interval [0, 10] maximum

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:187

___

### volumetricLightSmoothXPostProcess

• **volumetricLightSmoothXPostProcess**: [`Nullable`](../modules.md#nullable)[`BlurPostProcess`](BlurPostProcess.md) = `null`

Post-process used to smooth the previous volumetric light post-process on the X axis

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:73

___

### volumetricLightSmoothYPostProcess

• **volumetricLightSmoothYPostProcess**: [`Nullable`](../modules.md#nullable)[`BlurPostProcess`](BlurPostProcess.md) = `null`

Post-process used to smooth the previous volumetric light post-process on the Y axis

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:77

___

### LuminanceSteps

▪ `Static` **LuminanceSteps**: `number` = `6`

Luminance steps

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:1684

## Accessors

### BloomEnabled

• `set` **BloomEnabled**(`enabled`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `enabled` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:377

___

### DepthOfFieldEnabled

• `set` **DepthOfFieldEnabled**(`enabled`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `enabled` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:395

___

### HDREnabled

• `set` **HDREnabled**(`enabled`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `enabled` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:431

___

### LensFlareEnabled

• `set` **LensFlareEnabled**(`enabled`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `enabled` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:413

___

### MotionBlurEnabled

• `set` **MotionBlurEnabled**(`enabled`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `enabled` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:477

___

### VLSEnabled

• `set` **VLSEnabled**(`enabled`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `enabled` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:451

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

### exposure

• `get` **exposure**(): `number`

Gets the overall exposure used by the pipeline

#### Returns

`number`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:160

• `set` **exposure**(`value`): `void`

Sets the overall exposure used by the pipeline

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:167

___

### fxaaEnabled

• `get` **fxaaEnabled**(): `boolean`

Specifies if anti-aliasing is enabled

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:489

• `set` **fxaaEnabled**(`enabled`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `enabled` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:494

___

### hdrAutoExposure

• `get` **hdrAutoExposure**(): `boolean`

Gets whether or not the exposure of the overall pipeline should be automatically adjusted by the HDR post-process

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:218

• `set` **hdrAutoExposure**(`value`): `void`

Sets whether or not the exposure of the overall pipeline should be automatically adjusted by the HDR post-process

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:225

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

### motionBlurSamples

• `get` **motionBlurSamples**(): `number`

Specifies the number of samples used for the motion blur effect
Typically in interval [16, 64]

#### Returns

`number`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:541

• `set` **motionBlurSamples**(`samples`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `samples` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:546

___

### motionStrength

• `get` **motionStrength**(): `number`

Gets how much the image is blurred by the movement while using the motion blur post-process

#### Returns

`number`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:294

• `set` **motionStrength**(`strength`): `void`

Sets how much the image is blurred by the movement while using the motion blur post-process

#### Parameters

| Name | Type |
| :------ | :------ |
| `strength` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:301

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

### objectBasedMotionBlur

• `get` **objectBasedMotionBlur**(): `boolean`

Gets whether or not the motion blur post-process is object based or screen based.

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:312

• `set` **objectBasedMotionBlur**(`value`): `void`

Sets whether or not the motion blur post-process should be object based or screen based

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:319

___

### samples

• `get` **samples**(): `number`

Specifies MSAA sample count, setting this to 4 will provide 4x anti aliasing. (default: 1)

#### Returns

`number`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:561

• `set` **samples**(`sampleCount`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `sampleCount` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:566

___

### screenSpaceReflectionsEnabled

• `get` **screenSpaceReflectionsEnabled**(): `boolean`

Specifies if screen space reflections are enabled.

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:506

• `set` **screenSpaceReflectionsEnabled**(`enabled`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `enabled` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:511

___

### volumetricLightStepsCount

• `get` **volumetricLightStepsCount**(): `number`

Specifies the number of steps used to calculate the volumetric lights
Typically in interval [50, 200]

#### Returns

`number`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:524

• `set` **volumetricLightStepsCount**(`count`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `count` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:529

## Methods

### \_buildPipeline

▸ `Private` **_buildPipeline**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:603

___

### \_createBlurPostProcesses

▸ `Private` **_createBlurPostProcesses**(`scene`, `ratio`, `indice`, `blurWidthKey?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | `undefined` |
| `ratio` | `number` | `undefined` |
| `indice` | `number` | `undefined` |
| `blurWidthKey` | `string` | `"blurWidth"` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:921

___

### \_createBrightPassPostProcess

▸ `Private` **_createBrightPassPostProcess**(`scene`, `ratio`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `scene` | [`Scene`](Scene.md) |
| `ratio` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:874

___

### \_createDepthOfFieldPostProcess

▸ `Private` **_createDepthOfFieldPostProcess**(`scene`, `ratio`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `scene` | [`Scene`](Scene.md) |
| `ratio` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:1421

___

### \_createDownSampleX4PostProcess

▸ `Private` **_createDownSampleX4PostProcess**(`scene`, `ratio`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `scene` | [`Scene`](Scene.md) |
| `ratio` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:828

___

### \_createHdrPostProcess

▸ `Private` **_createHdrPostProcess**(`scene`, `ratio`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `scene` | [`Scene`](Scene.md) |
| `ratio` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:1236

___

### \_createLensFlarePostProcess

▸ `Private` **_createLensFlarePostProcess**(`scene`, `ratio`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `scene` | [`Scene`](Scene.md) |
| `ratio` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:1303

___

### \_createLuminancePostProcesses

▸ `Private` **_createLuminancePostProcesses**(`scene`, `textureType`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `scene` | [`Scene`](Scene.md) |
| `textureType` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:1110

___

### \_createMotionBlurPostProcess

▸ `Private` **_createMotionBlurPostProcess**(`scene`, `ratio`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `scene` | [`Scene`](Scene.md) |
| `ratio` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:1456

___

### \_createTextureAdderPostProcess

▸ `Private` **_createTextureAdderPostProcess**(`scene`, `ratio`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `scene` | [`Scene`](Scene.md) |
| `ratio` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:983

___

### \_createVolumetricLightPostProcess

▸ `Private` **_createVolumetricLightPostProcess**(`scene`, `ratio`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `scene` | [`Scene`](Scene.md) |
| `ratio` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:1019

___

### \_disposePostProcesses

▸ `Private` **_disposePostProcesses**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:1525

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

### \_getDepthTexture

▸ `Private` **_getDepthTexture**(): [`Texture`](Texture.md)

#### Returns

[`Texture`](Texture.md)

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:1516

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

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:1632

___

### getClassName

▸ **getClassName**(): `string`

Gets the class name

#### Returns

`string`

"PostProcessRenderPipeline"

#### Inherited from

[PostProcessRenderPipeline](PostProcessRenderPipeline.md).[getClassName](PostProcessRenderPipeline.md#getclassname)

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/postProcessRenderPipeline.ts:64

___

### serialize

▸ **serialize**(): `any`

Serialize the rendering pipeline (Used when exporting)

#### Returns

`any`

the serialized object

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:1644

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

▸ `Static` **Parse**(`source`, `scene`, `rootUrl`): [`StandardRenderingPipeline`](StandardRenderingPipeline.md)

Parse the serialized pipeline

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | `any` | Source pipeline. |
| `scene` | [`Scene`](Scene.md) | The scene to load the pipeline to. |
| `rootUrl` | `string` | The URL of the serialized pipeline. |

#### Returns

[`StandardRenderingPipeline`](StandardRenderingPipeline.md)

An instantiated pipeline from the serialized object.

#### Defined in

packages/dev/core/src/PostProcesses/RenderPipeline/Pipelines/standardRenderingPipeline.ts:1667
