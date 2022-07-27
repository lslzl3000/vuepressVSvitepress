[@dev/core](../README.md) / [Exports](../modules.md) / LensRenderingPipeline

# Class: LensRenderingPipeline

BABYLON.JS Chromatic Aberration GLSL Shader
Author: Olivier Guyot
Separates very slightly R, G and B colors on the edges of the screen
Inspired by Francois Tarlier & Martins Upitis

## Hierarchy

- [`PostProcessRenderPipeline`](PostProcessRenderPipeline.md)

  ↳ **`LensRenderingPipeline`**

## Table of contents

### Constructors

- [constructor](LensRenderingPipeline.md#constructor)

### Properties

- [\_blurNoise](LensRenderingPipeline.md#_blurnoise)
- [\_chromaticAberration](LensRenderingPipeline.md#_chromaticaberration)
- [\_chromaticAberrationPostProcess](LensRenderingPipeline.md#_chromaticaberrationpostprocess)
- [\_depthOfFieldPostProcess](LensRenderingPipeline.md#_depthoffieldpostprocess)
- [\_depthTexture](LensRenderingPipeline.md#_depthtexture)
- [\_distortion](LensRenderingPipeline.md#_distortion)
- [\_dofAperture](LensRenderingPipeline.md#_dofaperture)
- [\_dofDarken](LensRenderingPipeline.md#_dofdarken)
- [\_dofDistance](LensRenderingPipeline.md#_dofdistance)
- [\_dofPentagon](LensRenderingPipeline.md#_dofpentagon)
- [\_edgeBlur](LensRenderingPipeline.md#_edgeblur)
- [\_grainAmount](LensRenderingPipeline.md#_grainamount)
- [\_grainTexture](LensRenderingPipeline.md#_graintexture)
- [\_highlightsGain](LensRenderingPipeline.md#_highlightsgain)
- [\_highlightsPostProcess](LensRenderingPipeline.md#_highlightspostprocess)
- [\_highlightsThreshold](LensRenderingPipeline.md#_highlightsthreshold)
- [\_pentagonBokehIsEnabled](LensRenderingPipeline.md#_pentagonbokehisenabled)
- [\_scene](LensRenderingPipeline.md#_scene)
- [inspectableCustomProperties](LensRenderingPipeline.md#inspectablecustomproperties)

### Accessors

- [blurNoise](LensRenderingPipeline.md#blurnoise)
- [cameras](LensRenderingPipeline.md#cameras)
- [chromaticAberration](LensRenderingPipeline.md#chromaticaberration)
- [darkenOutOfFocus](LensRenderingPipeline.md#darkenoutoffocus)
- [dofAperture](LensRenderingPipeline.md#dofaperture)
- [dofDistortion](LensRenderingPipeline.md#dofdistortion)
- [edgeBlur](LensRenderingPipeline.md#edgeblur)
- [edgeDistortion](LensRenderingPipeline.md#edgedistortion)
- [grainAmount](LensRenderingPipeline.md#grainamount)
- [highlightsGain](LensRenderingPipeline.md#highlightsgain)
- [highlightsThreshold](LensRenderingPipeline.md#highlightsthreshold)
- [isSupported](LensRenderingPipeline.md#issupported)
- [name](LensRenderingPipeline.md#name)
- [pentagonBokeh](LensRenderingPipeline.md#pentagonbokeh)
- [scene](LensRenderingPipeline.md#scene)

### Methods

- [\_createChromaticAberrationPostProcess](LensRenderingPipeline.md#_createchromaticaberrationpostprocess)
- [\_createDepthOfFieldPostProcess](LensRenderingPipeline.md#_createdepthoffieldpostprocess)
- [\_createGrainTexture](LensRenderingPipeline.md#_creategraintexture)
- [\_createHighlightsPostProcess](LensRenderingPipeline.md#_createhighlightspostprocess)
- [\_enableMSAAOnFirstPostProcess](LensRenderingPipeline.md#_enablemsaaonfirstpostprocess)
- [addEffect](LensRenderingPipeline.md#addeffect)
- [disableChromaticAberration](LensRenderingPipeline.md#disablechromaticaberration)
- [disableDepthOfField](LensRenderingPipeline.md#disabledepthoffield)
- [disableEdgeBlur](LensRenderingPipeline.md#disableedgeblur)
- [disableEdgeDistortion](LensRenderingPipeline.md#disableedgedistortion)
- [disableGrain](LensRenderingPipeline.md#disablegrain)
- [disableHighlights](LensRenderingPipeline.md#disablehighlights)
- [disableNoiseBlur](LensRenderingPipeline.md#disablenoiseblur)
- [disablePentagonBokeh](LensRenderingPipeline.md#disablepentagonbokeh)
- [dispose](LensRenderingPipeline.md#dispose)
- [enableNoiseBlur](LensRenderingPipeline.md#enablenoiseblur)
- [enablePentagonBokeh](LensRenderingPipeline.md#enablepentagonbokeh)
- [getClassName](LensRenderingPipeline.md#getclassname)
- [setAperture](LensRenderingPipeline.md#setaperture)
- [setChromaticAberration](LensRenderingPipeline.md#setchromaticaberration)
- [setDarkenOutOfFocus](LensRenderingPipeline.md#setdarkenoutoffocus)
- [setEdgeBlur](LensRenderingPipeline.md#setedgeblur)
- [setEdgeDistortion](LensRenderingPipeline.md#setedgedistortion)
- [setFocusDistance](LensRenderingPipeline.md#setfocusdistance)
- [setGrainAmount](LensRenderingPipeline.md#setgrainamount)
- [setHighlightsGain](LensRenderingPipeline.md#sethighlightsgain)
- [setHighlightsThreshold](LensRenderingPipeline.md#sethighlightsthreshold)
- [setPrePassRenderer](LensRenderingPipeline.md#setprepassrenderer)

## Constructors

### constructor

• **new LensRenderingPipeline**(`name`, `parameters`, `scene`, `ratio?`, `cameras?`)

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | The rendering pipeline name |
| `parameters` | `any` | `undefined` | An object containing all parameters (see above) |
| `scene` | [`Scene`](Scene.md) | `undefined` | The scene linked to this pipeline |
| `ratio` | `number` | `1.0` | The size of the postprocesses (0.5 means that your postprocess will have a width = canvas.width 0.5 and a height = canvas.height 0.5) |
| `cameras?` | [`Camera`](Camera.md)[] | `undefined` | The array of cameras that the rendering pipeline will be attached to |

#### Overrides

[PostProcessRenderPipeline](PostProcessRenderPipeline.md).[constructor](PostProcessRenderPipeline.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:99

## Properties

### \_blurNoise

• `Private` **\_blurNoise**: `boolean`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:71

___

### \_chromaticAberration

• `Private` **\_chromaticAberration**: `number`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:63

___

### \_chromaticAberrationPostProcess

• `Private` **\_chromaticAberrationPostProcess**: [`PostProcess`](PostProcess.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:57

___

### \_depthOfFieldPostProcess

• `Private` **\_depthOfFieldPostProcess**: [`PostProcess`](PostProcess.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:59

___

### \_depthTexture

• `Private` **\_depthTexture**: [`RenderTargetTexture`](RenderTargetTexture.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:54

___

### \_distortion

• `Private` **\_distortion**: `number`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:64

___

### \_dofAperture

• `Private` **\_dofAperture**: `number`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:68

___

### \_dofDarken

• `Private` **\_dofDarken**: `number`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:69

___

### \_dofDistance

• `Private` **\_dofDistance**: `number`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:67

___

### \_dofPentagon

• `Private` **\_dofPentagon**: `boolean`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:70

___

### \_edgeBlur

• `Private` **\_edgeBlur**: `number`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:61

___

### \_grainAmount

• `Private` **\_grainAmount**: `number`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:62

___

### \_grainTexture

• `Private` **\_grainTexture**: [`Texture`](Texture.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:55

___

### \_highlightsGain

• `Private` **\_highlightsGain**: `number`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:65

___

### \_highlightsPostProcess

• `Private` **\_highlightsPostProcess**: [`PostProcess`](PostProcess.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:58

___

### \_highlightsThreshold

• `Private` **\_highlightsThreshold**: `number`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:66

___

### \_pentagonBokehIsEnabled

• `Private` **\_pentagonBokehIsEnabled**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:396

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:53

___

### inspectableCustomProperties

• **inspectableCustomProperties**: [`IInspectable`](../interfaces/IInspectable.md)[]

List of inspectable custom properties (used by the Inspector)

**`See`**

https://doc.babylonjs.com/how_to/debug_layer#extensibility

#### Inherited from

[PostProcessRenderPipeline](PostProcessRenderPipeline.md).[inspectableCustomProperties](PostProcessRenderPipeline.md#inspectablecustomproperties)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderPipeline.ts:23

## Accessors

### blurNoise

• `get` **blurNoise**(): `boolean`

Gets or sets a boolean indicating if blur noise is enabled

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:270

• `set` **blurNoise**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:274

___

### cameras

• `get` **cameras**(): [`Camera`](Camera.md)[]

Gets the list of attached cameras

#### Returns

[`Camera`](Camera.md)[]

#### Inherited from

PostProcessRenderPipeline.cameras

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderPipeline.ts:42

___

### chromaticAberration

• `get` **chromaticAberration**(): `number`

Gets or sets the chromatic aberration amount

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:215

• `set` **chromaticAberration**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:219

___

### darkenOutOfFocus

• `get` **darkenOutOfFocus**(): `number`

Gets or sets the darken out of focus amount

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:259

• `set` **darkenOutOfFocus**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:263

___

### dofAperture

• `get` **dofAperture**(): `number`

Gets or sets the depth of field aperture

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:226

• `set` **dofAperture**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:230

___

### dofDistortion

• `get` **dofDistortion**(): `number`

Gets or sets the depth of field distortion

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:248

• `set` **dofDistortion**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:252

___

### edgeBlur

• `get` **edgeBlur**(): `number`

Gets or sets the edge blur

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:193

• `set` **edgeBlur**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:197

___

### edgeDistortion

• `get` **edgeDistortion**(): `number`

Gets or sets the edge distortion

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:237

• `set` **edgeDistortion**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:241

___

### grainAmount

• `get` **grainAmount**(): `number`

Gets or sets the grain amount

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:204

• `set` **grainAmount**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:208

___

### highlightsGain

• `get` **highlightsGain**(): `number`

Gets or sets the highlight grain amount

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:296

• `set` **highlightsGain**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:300

___

### highlightsThreshold

• `get` **highlightsThreshold**(): `number`

Gets or sets the highlight threshold

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:307

• `set` **highlightsThreshold**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:311

___

### isSupported

• `get` **isSupported**(): `boolean`

If all the render effects in the pipeline are supported

#### Returns

`boolean`

#### Inherited from

PostProcessRenderPipeline.isSupported

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderPipeline.ts:71

___

### name

• `get` **name**(): `string`

Gets pipeline name

#### Returns

`string`

#### Inherited from

PostProcessRenderPipeline.name

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderPipeline.ts:37

___

### pentagonBokeh

• `get` **pentagonBokeh**(): `boolean`

Gets or sets a boolean indicating if pentagon bokeh is enabled

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:281

• `set` **pentagonBokeh**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:285

___

### scene

• `get` **scene**(): [`Scene`](Scene.md)

Gets associated scene

#### Returns

[`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:186

## Methods

### \_createChromaticAberrationPostProcess

▸ `Private` **_createChromaticAberrationPostProcess**(`ratio`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `ratio` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:466

___

### \_createDepthOfFieldPostProcess

▸ `Private` **_createDepthOfFieldPostProcess**(`ratio`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `ratio` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:515

___

### \_createGrainTexture

▸ `Private` **_createGrainTexture**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:574

___

### \_createHighlightsPostProcess

▸ `Private` **_createHighlightsPostProcess**(`ratio`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `ratio` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:490

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

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderPipeline.ts:228

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

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderPipeline.ts:87

___

### disableChromaticAberration

▸ **disableChromaticAberration**(): `void`

Sets chromatic aberration amount to 0

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:352

___

### disableDepthOfField

▸ **disableDepthOfField**(): `void`

Disables depth of field

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:378

___

### disableEdgeBlur

▸ **disableEdgeBlur**(): `void`

Sets edge blur to 0

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:326

___

### disableEdgeDistortion

▸ **disableEdgeDistortion**(): `void`

Sets edge distortion to 0

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:365

___

### disableGrain

▸ **disableGrain**(): `void`

Set grain amount to 0

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:339

___

### disableHighlights

▸ **disableHighlights**(): `void`

Disables highlights

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:443

___

### disableNoiseBlur

▸ **disableNoiseBlur**(): `void`

Disables noise blur

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:420

___

### disablePentagonBokeh

▸ **disablePentagonBokeh**(): `void`

Disables the pentagon bokeh effect

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:407

___

### dispose

▸ **dispose**(`disableDepthRender?`): `void`

Removes the internal pipeline assets and detaches the pipeline from the scene cameras

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `disableDepthRender` | `boolean` | `false` | If the scene's depth rendering should be disabled (default: false) |

#### Returns

`void`

#### Overrides

[PostProcessRenderPipeline](PostProcessRenderPipeline.md).[dispose](PostProcessRenderPipeline.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:451

___

### enableNoiseBlur

▸ **enableNoiseBlur**(): `void`

Enables noise blur

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:414

___

### enablePentagonBokeh

▸ **enablePentagonBokeh**(): `void`

Creates a pentagon bokeh effect

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:400

___

### getClassName

▸ **getClassName**(): `string`

Get the class name

#### Returns

`string`

"LensRenderingPipeline"

#### Overrides

[PostProcessRenderPipeline](PostProcessRenderPipeline.md).[getClassName](PostProcessRenderPipeline.md#getclassname)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:177

___

### setAperture

▸ **setAperture**(`amount`): `void`

Sets the Aperture amount

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `amount` | `number` | amount of Aperture |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:385

___

### setChromaticAberration

▸ **setChromaticAberration**(`amount`): `void`

Sets the chromatic aberration amount

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `amount` | `number` | amount of chromatic aberration |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:346

___

### setDarkenOutOfFocus

▸ **setDarkenOutOfFocus**(`amount`): `void`

Sets the DarkenOutOfFocus amount

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `amount` | `number` | amount of DarkenOutOfFocus |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:392

___

### setEdgeBlur

▸ **setEdgeBlur**(`amount`): `void`

Sets the amount of blur at the edges

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `amount` | `number` | blur amount |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:320

___

### setEdgeDistortion

▸ **setEdgeDistortion**(`amount`): `void`

Sets the EdgeDistortion amount

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `amount` | `number` | amount of EdgeDistortion |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:359

___

### setFocusDistance

▸ **setFocusDistance**(`amount`): `void`

Sets the FocusDistance amount

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `amount` | `number` | amount of FocusDistance |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:372

___

### setGrainAmount

▸ **setGrainAmount**(`amount`): `void`

Sets the amount of grain

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `amount` | `number` | Amount of grain |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:333

___

### setHighlightsGain

▸ **setHighlightsGain**(`amount`): `void`

Sets the HighlightsGain amount

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `amount` | `number` | amount of HighlightsGain |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:427

___

### setHighlightsThreshold

▸ **setHighlightsThreshold**(`amount`): `void`

Sets the HighlightsThreshold amount

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `amount` | `number` | amount of HighlightsThreshold |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/lensRenderingPipeline.ts:434

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

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderPipeline.ts:250
