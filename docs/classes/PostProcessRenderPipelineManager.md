[@dev/core](../README.md) / [Exports](../modules.md) / PostProcessRenderPipelineManager

# Class: PostProcessRenderPipelineManager

PostProcessRenderPipelineManager class

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_postprocessrenderpipeline

## Table of contents

### Constructors

- [constructor](PostProcessRenderPipelineManager.md#constructor)

### Properties

- [\_renderPipelines](PostProcessRenderPipelineManager.md#_renderpipelines)

### Accessors

- [supportedPipelines](PostProcessRenderPipelineManager.md#supportedpipelines)

### Methods

- [addPipeline](PostProcessRenderPipelineManager.md#addpipeline)
- [attachCamerasToRenderPipeline](PostProcessRenderPipelineManager.md#attachcamerastorenderpipeline)
- [detachCamerasFromRenderPipeline](PostProcessRenderPipelineManager.md#detachcamerasfromrenderpipeline)
- [disableEffectInPipeline](PostProcessRenderPipelineManager.md#disableeffectinpipeline)
- [dispose](PostProcessRenderPipelineManager.md#dispose)
- [enableEffectInPipeline](PostProcessRenderPipelineManager.md#enableeffectinpipeline)
- [update](PostProcessRenderPipelineManager.md#update)

## Constructors

### constructor

• **new PostProcessRenderPipelineManager**()

Initializes a PostProcessRenderPipelineManager

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_postprocessrenderpipeline

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderPipelineManager.ts:14

## Properties

### \_renderPipelines

• `Private` **\_renderPipelines**: `Object`

#### Index signature

▪ [Key: `string`]: [`PostProcessRenderPipeline`](PostProcessRenderPipeline.md)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderPipelineManager.ts:8

## Accessors

### supportedPipelines

• `get` **supportedPipelines**(): [`PostProcessRenderPipeline`](PostProcessRenderPipeline.md)[]

Gets the list of supported render pipelines

#### Returns

[`PostProcessRenderPipeline`](PostProcessRenderPipeline.md)[]

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderPipelineManager.ts:21

## Methods

### addPipeline

▸ **addPipeline**(`renderPipeline`): `void`

Adds a pipeline to the manager

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `renderPipeline` | [`PostProcessRenderPipeline`](PostProcessRenderPipeline.md) | The pipeline to add |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderPipelineManager.ts:40

___

### attachCamerasToRenderPipeline

▸ **attachCamerasToRenderPipeline**(`renderPipelineName`, `cameras`, `unique?`): `void`

Attaches a camera to the pipeline

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `renderPipelineName` | `string` | `undefined` | The name of the pipeline to attach to |
| `cameras` | `any` | `undefined` | the camera to attach |
| `unique` | `boolean` | `false` | if the camera can be attached multiple times to the pipeline |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderPipelineManager.ts:50

___

### detachCamerasFromRenderPipeline

▸ **detachCamerasFromRenderPipeline**(`renderPipelineName`, `cameras`): `void`

Detaches a camera from the pipeline

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `renderPipelineName` | `string` | The name of the pipeline to detach from |
| `cameras` | `any` | the camera to detach |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderPipelineManager.ts:65

___

### disableEffectInPipeline

▸ **disableEffectInPipeline**(`renderPipelineName`, `renderEffectName`, `cameras`): `void`

Disables an effect by name on a pipeline

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `renderPipelineName` | `string` | the name of the pipeline to disable the effect in |
| `renderEffectName` | `string` | the name of the effect to disable |
| `cameras` | `any` | the cameras that the effect should be disabled on |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderPipelineManager.ts:97

___

### dispose

▸ **dispose**(): `void`

Disposes of the manager and pipelines

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderPipelineManager.ts:137

___

### enableEffectInPipeline

▸ **enableEffectInPipeline**(`renderPipelineName`, `renderEffectName`, `cameras`): `void`

Enables an effect by name on a pipeline

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `renderPipelineName` | `string` | the name of the pipeline to enable the effect in |
| `renderEffectName` | `string` | the name of the effect to enable |
| `cameras` | `any` | the cameras that the effect should be enabled on |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderPipelineManager.ts:81

___

### update

▸ **update**(): `void`

Updates the state of all contained render pipelines and disposes of any non supported pipelines

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderPipelineManager.ts:110
