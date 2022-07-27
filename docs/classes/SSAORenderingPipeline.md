[@dev/core](../README.md) / [Exports](../modules.md) / SSAORenderingPipeline

# Class: SSAORenderingPipeline

Render pipeline to produce ssao effect

## Hierarchy

- [`PostProcessRenderPipeline`](PostProcessRenderPipeline.md)

  ↳ **`SSAORenderingPipeline`**

## Table of contents

### Constructors

- [constructor](SSAORenderingPipeline.md#constructor)

### Properties

- [\_blurHPostProcess](SSAORenderingPipeline.md#_blurhpostprocess)
- [\_blurVPostProcess](SSAORenderingPipeline.md#_blurvpostprocess)
- [\_firstUpdate](SSAORenderingPipeline.md#_firstupdate)
- [\_originalColorPostProcess](SSAORenderingPipeline.md#_originalcolorpostprocess)
- [\_randomTexture](SSAORenderingPipeline.md#_randomtexture)
- [\_scene](SSAORenderingPipeline.md#_scene)
- [\_ssaoCombinePostProcess](SSAORenderingPipeline.md#_ssaocombinepostprocess)
- [\_ssaoPostProcess](SSAORenderingPipeline.md#_ssaopostprocess)
- [area](SSAORenderingPipeline.md#area)
- [base](SSAORenderingPipeline.md#base)
- [fallOff](SSAORenderingPipeline.md#falloff)
- [inspectableCustomProperties](SSAORenderingPipeline.md#inspectablecustomproperties)
- [radius](SSAORenderingPipeline.md#radius)
- [totalStrength](SSAORenderingPipeline.md#totalstrength)

### Accessors

- [cameras](SSAORenderingPipeline.md#cameras)
- [isSupported](SSAORenderingPipeline.md#issupported)
- [name](SSAORenderingPipeline.md#name)
- [scene](SSAORenderingPipeline.md#scene)

### Methods

- [\_createBlurPostProcess](SSAORenderingPipeline.md#_createblurpostprocess)
- [\_createRandomTexture](SSAORenderingPipeline.md#_createrandomtexture)
- [\_createSSAOCombinePostProcess](SSAORenderingPipeline.md#_createssaocombinepostprocess)
- [\_createSSAOPostProcess](SSAORenderingPipeline.md#_createssaopostprocess)
- [\_enableMSAAOnFirstPostProcess](SSAORenderingPipeline.md#_enablemsaaonfirstpostprocess)
- [addEffect](SSAORenderingPipeline.md#addeffect)
- [dispose](SSAORenderingPipeline.md#dispose)
- [getClassName](SSAORenderingPipeline.md#getclassname)
- [setPrePassRenderer](SSAORenderingPipeline.md#setprepassrenderer)

## Constructors

### constructor

• **new SSAORenderingPipeline**(`name`, `scene`, `ratio`, `cameras?`)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | The rendering pipeline name |
| `scene` | [`Scene`](Scene.md) | The scene linked to this pipeline |
| `ratio` | `any` | The size of the postprocesses. Can be a number shared between passes or an object for more precision: { ssaoRatio: 0.5, combineRatio: 1.0 } |
| `cameras?` | [`Camera`](Camera.md)[] | The array of cameras that the rendering pipeline will be attached to |

#### Overrides

[PostProcessRenderPipeline](PostProcessRenderPipeline.md).[constructor](PostProcessRenderPipeline.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssaoRenderingPipeline.ts:113

## Properties

### \_blurHPostProcess

• `Private` **\_blurHPostProcess**: [`BlurPostProcess`](BlurPostProcess.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssaoRenderingPipeline.ts:93

___

### \_blurVPostProcess

• `Private` **\_blurVPostProcess**: [`BlurPostProcess`](BlurPostProcess.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssaoRenderingPipeline.ts:94

___

### \_firstUpdate

• `Private` **\_firstUpdate**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssaoRenderingPipeline.ts:97

___

### \_originalColorPostProcess

• `Private` **\_originalColorPostProcess**: [`PassPostProcess`](PassPostProcess.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssaoRenderingPipeline.ts:91

___

### \_randomTexture

• `Private` **\_randomTexture**: [`DynamicTexture`](DynamicTexture.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssaoRenderingPipeline.ts:89

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssaoRenderingPipeline.ts:88

___

### \_ssaoCombinePostProcess

• `Private` **\_ssaoCombinePostProcess**: [`PostProcess`](PostProcess.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssaoRenderingPipeline.ts:95

___

### \_ssaoPostProcess

• `Private` **\_ssaoPostProcess**: [`PostProcess`](PostProcess.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssaoRenderingPipeline.ts:92

___

### area

• **area**: `number` = `0.0075`

Related to fallOff, used to interpolate SSAO samples (first interpolate function input) based on the occlusion difference of each pixel
Must not be equal to fallOff and superior to fallOff.
Default value is 0.0075

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssaoRenderingPipeline.ts:71

___

### base

• **base**: `number` = `0.5`

The base color of the SSAO post-process
The final result is "base + ssao" between [0, 1]

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssaoRenderingPipeline.ts:86

___

### fallOff

• **fallOff**: `number` = `0.000001`

Related to area, used to interpolate SSAO samples (second interpolate function input) based on the occlusion difference of each pixel
Must not be equal to area and inferior to area.
Default value is 0.000001

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssaoRenderingPipeline.ts:79

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

___

### radius

• **radius**: `number` = `0.0001`

The radius around the analyzed pixel used by the SSAO post-process. Default value is 0.0006

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssaoRenderingPipeline.ts:63

___

### totalStrength

• **totalStrength**: `number` = `1.0`

The output strength of the SSAO post-process. Default value is 1.0.

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssaoRenderingPipeline.ts:57

## Accessors

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

### scene

• `get` **scene**(): [`Scene`](Scene.md)

Gets active scene

#### Returns

[`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssaoRenderingPipeline.ts:102

## Methods

### \_createBlurPostProcess

▸ `Private` **_createBlurPostProcess**(`ratio`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `ratio` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssaoRenderingPipeline.ts:239

___

### \_createRandomTexture

▸ `Private` **_createRandomTexture**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssaoRenderingPipeline.ts:342

___

### \_createSSAOCombinePostProcess

▸ `Private` **_createSSAOCombinePostProcess**(`ratio`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `ratio` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssaoRenderingPipeline.ts:323

___

### \_createSSAOPostProcess

▸ `Private` **_createSSAOPostProcess**(`ratio`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `ratio` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssaoRenderingPipeline.ts:282

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

### dispose

▸ **dispose**(`disableDepthRender?`): `void`

Removes the internal pipeline assets and detaches the pipeline from the scene cameras

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `disableDepthRender` | `boolean` | `false` |

#### Returns

`void`

#### Overrides

[PostProcessRenderPipeline](PostProcessRenderPipeline.md).[dispose](PostProcessRenderPipeline.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssaoRenderingPipeline.ts:216

___

### getClassName

▸ **getClassName**(): `string`

Get the class name

#### Returns

`string`

"SSAORenderingPipeline"

#### Overrides

[PostProcessRenderPipeline](PostProcessRenderPipeline.md).[getClassName](PostProcessRenderPipeline.md#getclassname)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssaoRenderingPipeline.ts:208

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
