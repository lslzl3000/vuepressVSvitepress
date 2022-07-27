[@dev/core](../README.md) / [Exports](../modules.md) / SSAO2RenderingPipeline

# Class: SSAO2RenderingPipeline

Render pipeline to produce ssao effect

## Hierarchy

- [`PostProcessRenderPipeline`](PostProcessRenderPipeline.md)

  ↳ **`SSAO2RenderingPipeline`**

## Table of contents

### Constructors

- [constructor](SSAO2RenderingPipeline.md#constructor)

### Properties

- [\_bits](SSAO2RenderingPipeline.md#_bits)
- [\_blurHPostProcess](SSAO2RenderingPipeline.md#_blurhpostprocess)
- [\_blurVPostProcess](SSAO2RenderingPipeline.md#_blurvpostprocess)
- [\_expensiveBlur](SSAO2RenderingPipeline.md#_expensiveblur)
- [\_forceGeometryBuffer](SSAO2RenderingPipeline.md#_forcegeometrybuffer)
- [\_originalColorPostProcess](SSAO2RenderingPipeline.md#_originalcolorpostprocess)
- [\_randomTexture](SSAO2RenderingPipeline.md#_randomtexture)
- [\_ratio](SSAO2RenderingPipeline.md#_ratio)
- [\_sampleSphere](SSAO2RenderingPipeline.md#_samplesphere)
- [\_samplerOffsets](SSAO2RenderingPipeline.md#_sampleroffsets)
- [\_samples](SSAO2RenderingPipeline.md#_samples)
- [\_scene](SSAO2RenderingPipeline.md#_scene)
- [\_ssaoCombinePostProcess](SSAO2RenderingPipeline.md#_ssaocombinepostprocess)
- [\_ssaoPostProcess](SSAO2RenderingPipeline.md#_ssaopostprocess)
- [\_textureSamples](SSAO2RenderingPipeline.md#_texturesamples)
- [base](SSAO2RenderingPipeline.md#base)
- [inspectableCustomProperties](SSAO2RenderingPipeline.md#inspectablecustomproperties)
- [maxZ](SSAO2RenderingPipeline.md#maxz)
- [minZAspect](SSAO2RenderingPipeline.md#minzaspect)
- [radius](SSAO2RenderingPipeline.md#radius)
- [totalStrength](SSAO2RenderingPipeline.md#totalstrength)
- [ORTHO\_DEPTH\_PROJECTION](SSAO2RenderingPipeline.md#ortho_depth_projection)
- [PERSPECTIVE\_DEPTH\_PROJECTION](SSAO2RenderingPipeline.md#perspective_depth_projection)

### Accessors

- [\_geometryBufferRenderer](SSAO2RenderingPipeline.md#_geometrybufferrenderer)
- [\_prePassRenderer](SSAO2RenderingPipeline.md#_prepassrenderer)
- [cameras](SSAO2RenderingPipeline.md#cameras)
- [expensiveBlur](SSAO2RenderingPipeline.md#expensiveblur)
- [isSupported](SSAO2RenderingPipeline.md#issupported)
- [name](SSAO2RenderingPipeline.md#name)
- [samples](SSAO2RenderingPipeline.md#samples)
- [scene](SSAO2RenderingPipeline.md#scene)
- [textureSamples](SSAO2RenderingPipeline.md#texturesamples)
- [IsSupported](SSAO2RenderingPipeline.md#issupported-1)

### Methods

- [\_createBlurPostProcess](SSAO2RenderingPipeline.md#_createblurpostprocess)
- [\_createRandomTexture](SSAO2RenderingPipeline.md#_createrandomtexture)
- [\_createSSAOCombinePostProcess](SSAO2RenderingPipeline.md#_createssaocombinepostprocess)
- [\_createSSAOPostProcess](SSAO2RenderingPipeline.md#_createssaopostprocess)
- [\_enableMSAAOnFirstPostProcess](SSAO2RenderingPipeline.md#_enablemsaaonfirstpostprocess)
- [\_generateHemisphere](SSAO2RenderingPipeline.md#_generatehemisphere)
- [\_getDefinesForSSAO](SSAO2RenderingPipeline.md#_getdefinesforssao)
- [\_hammersley](SSAO2RenderingPipeline.md#_hammersley)
- [\_hemisphereSample\_uniform](SSAO2RenderingPipeline.md#_hemispheresample_uniform)
- [\_radicalInverse\_VdC](SSAO2RenderingPipeline.md#_radicalinverse_vdc)
- [addEffect](SSAO2RenderingPipeline.md#addeffect)
- [dispose](SSAO2RenderingPipeline.md#dispose)
- [getClassName](SSAO2RenderingPipeline.md#getclassname)
- [serialize](SSAO2RenderingPipeline.md#serialize)
- [setPrePassRenderer](SSAO2RenderingPipeline.md#setprepassrenderer)
- [Parse](SSAO2RenderingPipeline.md#parse)

## Constructors

### constructor

• **new SSAO2RenderingPipeline**(`name`, `scene`, `ratio`, `cameras?`, `forceGeometryBuffer?`, `textureType?`)

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | The rendering pipeline name |
| `scene` | [`Scene`](Scene.md) | `undefined` | The scene linked to this pipeline |
| `ratio` | `any` | `undefined` | The size of the postprocesses. Can be a number shared between passes or an object for more precision: { ssaoRatio: 0.5, blurRatio: 1.0 } |
| `cameras?` | [`Camera`](Camera.md)[] | `undefined` | The array of cameras that the rendering pipeline will be attached to |
| `forceGeometryBuffer` | `boolean` | `false` | Set to true if you want to use the legacy geometry buffer renderer |
| `textureType` | `number` | `Constants.TEXTURETYPE_UNSIGNED_INT` | The texture type used by the different post processes created by SSAO (default: Constants.TEXTURETYPE_UNSIGNED_INT) |

#### Overrides

[PostProcessRenderPipeline](PostProcessRenderPipeline.md).[constructor](PostProcessRenderPipeline.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:207

## Properties

### \_bits

• `Private` **\_bits**: `Uint32Array`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:410

___

### \_blurHPostProcess

• `Private` **\_blurHPostProcess**: [`PostProcess`](PostProcess.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:187

___

### \_blurVPostProcess

• `Private` **\_blurVPostProcess**: [`PostProcess`](PostProcess.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:188

___

### \_expensiveBlur

• `Private` **\_expensiveBlur**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:142

___

### \_forceGeometryBuffer

• `Private` **\_forceGeometryBuffer**: `boolean` = `false`

Force rendering the geometry through geometry buffer

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:112

___

### \_originalColorPostProcess

• `Private` **\_originalColorPostProcess**: [`PassPostProcess`](PassPostProcess.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:185

___

### \_randomTexture

• `Private` **\_randomTexture**: [`DynamicTexture`](DynamicTexture.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:184

___

### \_ratio

• `Private` **\_ratio**: `any`

Ratio object used for SSAO ratio and blur ratio

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:129

___

### \_sampleSphere

• `Private` **\_sampleSphere**: `number`[]

Dynamically generated sphere sampler.

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:134

___

### \_samplerOffsets

• `Private` **\_samplerOffsets**: `number`[]

Blur filter offsets

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:139

___

### \_samples

• `Private` **\_samples**: `number` = `8`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:78

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:183

___

### \_ssaoCombinePostProcess

• `Private` **\_ssaoCombinePostProcess**: [`PostProcess`](PostProcess.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:189

___

### \_ssaoPostProcess

• `Private` **\_ssaoPostProcess**: [`PostProcess`](PostProcess.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:186

___

### \_textureSamples

• `Private` **\_textureSamples**: `number` = `1`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:92

___

### base

• **base**: `number` = `0`

The base color of the SSAO post-process
The final result is "base + ssao" between [0, 1]

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:170

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

### maxZ

• **maxZ**: `number` = `100.0`

Maximum depth value to still render AO. A smooth falloff makes the dimming more natural, so there will be no abrupt shading change.

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:69

___

### minZAspect

• **minZAspect**: `number` = `0.2`

In order to save performances, SSAO radius is clamped on close geometry. This ratio changes by how much

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:75

___

### radius

• **radius**: `number` = `2.0`

The radius around the analyzed pixel used by the SSAO post-process. Default value is 2.0

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:163

___

### totalStrength

• **totalStrength**: `number` = `1.0`

The output strength of the SSAO post-process. Default value is 1.0.

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:63

___

### ORTHO\_DEPTH\_PROJECTION

▪ `Static` `Private` `Readonly` **ORTHO\_DEPTH\_PROJECTION**: `number`[]

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:462

___

### PERSPECTIVE\_DEPTH\_PROJECTION

▪ `Static` `Private` `Readonly` **PERSPECTIVE\_DEPTH\_PROJECTION**: `number`[]

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:464

## Accessors

### \_geometryBufferRenderer

• `Private` `get` **_geometryBufferRenderer**(): [`Nullable`](../modules.md#nullable)[`GeometryBufferRenderer`](GeometryBufferRenderer.md)

#### Returns

[`Nullable`](../modules.md#nullable)[`GeometryBufferRenderer`](GeometryBufferRenderer.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:113

___

### \_prePassRenderer

• `Private` `get` **_prePassRenderer**(): [`Nullable`](../modules.md#nullable)[`PrePassRenderer`](PrePassRenderer.md)

#### Returns

[`Nullable`](../modules.md#nullable)[`PrePassRenderer`](PrePassRenderer.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:119

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

### expensiveBlur

• `get` **expensiveBlur**(): `boolean`

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:155

• `set` **expensiveBlur**(`b`): `void`

If bilateral blur should be used

#### Parameters

| Name | Type |
| :------ | :------ |
| `b` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:146

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

### samples

• `get` **samples**(): `number`

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:87

• `set` **samples**(`n`): `void`

Number of samples used for the SSAO calculations. Default value is 8

#### Parameters

| Name | Type |
| :------ | :------ |
| `n` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:82

___

### scene

• `get` **scene**(): [`Scene`](Scene.md)

Gets active scene

#### Returns

[`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:194

___

### textureSamples

• `get` **textureSamples**(): `number`

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:105

• `set` **textureSamples**(`n`): `void`

Number of samples to use for antialiasing

#### Parameters

| Name | Type |
| :------ | :------ |
| `n` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:96

___

### IsSupported

• `Static` `get` **IsSupported**(): `boolean`

Support test.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:175

## Methods

### \_createBlurPostProcess

▸ `Private` **_createBlurPostProcess**(`ssaoRatio`, `blurRatio`, `textureType`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `ssaoRatio` | `number` |
| `blurRatio` | `number` |
| `textureType` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:333

___

### \_createRandomTexture

▸ `Private` **_createRandomTexture**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:575

___

### \_createSSAOCombinePostProcess

▸ `Private` **_createSSAOCombinePostProcess**(`ratio`, `textureType`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `ratio` | `number` |
| `textureType` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:552

___

### \_createSSAOPostProcess

▸ `Private` **_createSSAOPostProcess**(`ratio`, `textureType`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `ratio` | `number` |
| `textureType` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:466

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

### \_generateHemisphere

▸ `Private` **_generateHemisphere**(): `number`[]

#### Returns

`number`[]

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:435

___

### \_getDefinesForSSAO

▸ `Private` **_getDefinesForSSAO**(): `string`

#### Returns

`string`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:456

___

### \_hammersley

▸ `Private` **_hammersley**(`i`, `n`): `number`[]

#### Parameters

| Name | Type |
| :------ | :------ |
| `i` | `number` |
| `n` | `number` |

#### Returns

`number`[]

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:423

___

### \_hemisphereSample\_uniform

▸ `Private` **_hemisphereSample_uniform**(`u`, `v`): [`Vector3`](Vector3.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `u` | `number` |
| `v` | `number` |

#### Returns

[`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:427

___

### \_radicalInverse\_VdC

▸ `Private` **_radicalInverse_VdC**(`i`): `number`

#### Parameters

| Name | Type |
| :------ | :------ |
| `i` | `number` |

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:413

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

▸ **dispose**(`disableGeometryBufferRenderer?`): `void`

Removes the internal pipeline assets and detaches the pipeline from the scene cameras

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `disableGeometryBufferRenderer` | `boolean` | `false` |

#### Returns

`void`

#### Overrides

[PostProcessRenderPipeline](PostProcessRenderPipeline.md).[dispose](PostProcessRenderPipeline.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:310

___

### getClassName

▸ **getClassName**(): `string`

Get the class name

#### Returns

`string`

"SSAO2RenderingPipeline"

#### Overrides

[PostProcessRenderPipeline](PostProcessRenderPipeline.md).[getClassName](PostProcessRenderPipeline.md#getclassname)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:302

___

### serialize

▸ **serialize**(): `any`

Serialize the rendering pipeline (Used when exporting)

#### Returns

`any`

the serialized object

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:614

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

___

### Parse

▸ `Static` **Parse**(`source`, `scene`, `rootUrl`): [`SSAO2RenderingPipeline`](SSAO2RenderingPipeline.md)

Parse the serialized pipeline

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | `any` | Source pipeline. |
| `scene` | [`Scene`](Scene.md) | The scene to load the pipeline to. |
| `rootUrl` | `string` | The URL of the serialized pipeline. |

#### Returns

[`SSAO2RenderingPipeline`](SSAO2RenderingPipeline.md)

An instantiated pipeline from the serialized object.

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/Pipelines/ssao2RenderingPipeline.ts:628
