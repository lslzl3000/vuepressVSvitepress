[@dev/core](../README.md) / [Exports](../modules.md) / DepthOfFieldEffect

# Class: DepthOfFieldEffect

The depth of field effect applies a blur to objects that are closer or further from where the camera is focusing.

## Hierarchy

- [`PostProcessRenderEffect`](PostProcessRenderEffect.md)

  ↳ **`DepthOfFieldEffect`**

## Table of contents

### Constructors

- [constructor](DepthOfFieldEffect.md#constructor)

### Properties

- [\_circleOfConfusion](DepthOfFieldEffect.md#_circleofconfusion)
- [\_depthOfFieldBlurY](DepthOfFieldEffect.md#_depthoffieldblury)
- [\_dofMerge](DepthOfFieldEffect.md#_dofmerge)

### Accessors

- [depthTexture](DepthOfFieldEffect.md#depthtexture)
- [fStop](DepthOfFieldEffect.md#fstop)
- [focalLength](DepthOfFieldEffect.md#focallength)
- [focusDistance](DepthOfFieldEffect.md#focusdistance)
- [isSupported](DepthOfFieldEffect.md#issupported)
- [lensSize](DepthOfFieldEffect.md#lenssize)

### Methods

- [disposeEffects](DepthOfFieldEffect.md#disposeeffects)
- [getClassName](DepthOfFieldEffect.md#getclassname)
- [getPostProcesses](DepthOfFieldEffect.md#getpostprocesses)

## Constructors

### constructor

• **new DepthOfFieldEffect**(`scene`, `depthTexture`, `blurLevel?`, `pipelineTextureType?`, `blockCompilation?`)

Creates a new instance DepthOfFieldEffect

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | `undefined` | The scene the effect belongs to. |
| `depthTexture` | [`Nullable`](../modules.md#nullable)[`RenderTargetTexture`](RenderTargetTexture.md) | `undefined` | The depth texture of the scene to compute the circle of confusion.This must be set in order for this to function but may be set after initialization if needed. |
| `blurLevel` | [`DepthOfFieldEffectBlurLevel`](../enums/DepthOfFieldEffectBlurLevel.md) | `DepthOfFieldEffectBlurLevel.Low` |  |
| `pipelineTextureType` | `number` | `0` | The type of texture to be used when performing the post processing. |
| `blockCompilation` | `boolean` | `false` | If compilation of the shader should not be done in the constructor. The updateEffect method can be used to compile the shader at a later time. (default: false) |

#### Overrides

[PostProcessRenderEffect](PostProcessRenderEffect.md).[constructor](PostProcessRenderEffect.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/depthOfFieldEffect.ts:92

## Properties

### \_circleOfConfusion

• `Private` **\_circleOfConfusion**: [`CircleOfConfusionPostProcess`](CircleOfConfusionPostProcess.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/depthOfFieldEffect.ts:34

___

### \_depthOfFieldBlurY

• `Private` **\_depthOfFieldBlurY**: [`DepthOfFieldBlurPostProcess`](DepthOfFieldBlurPostProcess.md)[]

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/depthOfFieldEffect.ts:39

___

### \_dofMerge

• `Private` **\_dofMerge**: [`Nullable`](../modules.md#nullable)[`DepthOfFieldMergePostProcess`](DepthOfFieldMergePostProcess.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/depthOfFieldEffect.ts:40

## Accessors

### depthTexture

• `set` **depthTexture**(`value`): `void`

Depth texture to be used to compute the circle of confusion. This must be set here or in the constructor in order for the post process to function.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`RenderTargetTexture`](RenderTargetTexture.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/depthOfFieldEffect.ts:220

___

### fStop

• `get` **fStop**(): `number`

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/depthOfFieldEffect.ts:62

• `set` **fStop**(`value`): `void`

F-Stop of the effect's camera. The diameter of the resulting aperture can be computed by lensSize/fStop. (default: 1.4)

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/depthOfFieldEffect.ts:59

___

### focalLength

• `get` **focalLength**(): `number`

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/depthOfFieldEffect.ts:53

• `set` **focalLength**(`value`): `void`

The focal the length of the camera used in the effect in scene units/1000 (eg. millimeter)

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/depthOfFieldEffect.ts:50

___

### focusDistance

• `get` **focusDistance**(): `number`

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/depthOfFieldEffect.ts:71

• `set` **focusDistance**(`value`): `void`

Distance away from the camera to focus on in scene units/1000 (eg. millimeter). (default: 2000)

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/depthOfFieldEffect.ts:68

___

### isSupported

• `get` **isSupported**(): `boolean`

Checks if all the post processes in the effect are supported.

#### Returns

`boolean`

#### Inherited from

PostProcessRenderEffect.isSupported

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderEffect.ts:49

___

### lensSize

• `get` **lensSize**(): `number`

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/depthOfFieldEffect.ts:80

• `set` **lensSize**(`value`): `void`

Max lens size in scene units/1000 (eg. millimeter). Standard cameras are 50mm. (default: 50) The diameter of the resulting aperture can be computed by lensSize/fStop.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/depthOfFieldEffect.ts:77

## Methods

### disposeEffects

▸ **disposeEffects**(`camera`): `void`

Disposes each of the internal effects for a given camera.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `camera` | [`Camera`](Camera.md) | The camera to dispose the effect on. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/depthOfFieldEffect.ts:228

___

### getClassName

▸ **getClassName**(): `string`

Get the current class name of the current effect

#### Returns

`string`

"DepthOfFieldEffect"

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/depthOfFieldEffect.ts:213

___

### getPostProcesses

▸ **getPostProcesses**(`camera?`): [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)[]

Gets a list of the post processes contained in the effect.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `camera?` | [`Camera`](Camera.md) | The camera to get the post processes on. |

#### Returns

[`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)[]

The list of the post processes in the effect.

#### Inherited from

[PostProcessRenderEffect](PostProcessRenderEffect.md).[getPostProcesses](PostProcessRenderEffect.md#getpostprocesses)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderEffect.ts:249
