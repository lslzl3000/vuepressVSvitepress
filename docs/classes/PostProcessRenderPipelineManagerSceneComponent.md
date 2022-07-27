[@dev/core](../README.md) / [Exports](../modules.md) / PostProcessRenderPipelineManagerSceneComponent

# Class: PostProcessRenderPipelineManagerSceneComponent

Defines the Render Pipeline scene component responsible to rendering pipelines

## Implements

- [`ISceneComponent`](../interfaces/ISceneComponent.md)

## Table of contents

### Constructors

- [constructor](PostProcessRenderPipelineManagerSceneComponent.md#constructor)

### Properties

- [name](PostProcessRenderPipelineManagerSceneComponent.md#name)
- [scene](PostProcessRenderPipelineManagerSceneComponent.md#scene)

### Methods

- [\_gatherRenderTargets](PostProcessRenderPipelineManagerSceneComponent.md#_gatherrendertargets)
- [dispose](PostProcessRenderPipelineManagerSceneComponent.md#dispose)
- [rebuild](PostProcessRenderPipelineManagerSceneComponent.md#rebuild)
- [register](PostProcessRenderPipelineManagerSceneComponent.md#register)

## Constructors

### constructor

• **new PostProcessRenderPipelineManagerSceneComponent**(`scene`)

Creates a new instance of the component for the given scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | Defines the scene to register the component in |

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderPipelineManagerSceneComponent.ts:56

## Properties

### name

• `Readonly` **name**: ``"PostProcessRenderPipelineManager"``

The component name helpful to identify the component in the list of scene components.

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[name](../interfaces/ISceneComponent.md#name)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderPipelineManagerSceneComponent.ts:45

___

### scene

• **scene**: [`Scene`](Scene.md)

The scene the component belongs to.

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[scene](../interfaces/ISceneComponent.md#scene)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderPipelineManagerSceneComponent.ts:50

## Methods

### \_gatherRenderTargets

▸ `Private` **_gatherRenderTargets**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderPipelineManagerSceneComponent.ts:86

___

### dispose

▸ **dispose**(): `void`

Disposes the component and the associated resources

#### Returns

`void`

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[dispose](../interfaces/ISceneComponent.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderPipelineManagerSceneComponent.ts:80

___

### rebuild

▸ **rebuild**(): `void`

Rebuilds the elements related to this component in case of
context lost for instance.

#### Returns

`void`

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[rebuild](../interfaces/ISceneComponent.md#rebuild)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderPipelineManagerSceneComponent.ts:71

___

### register

▸ **register**(): `void`

Registers the component in a given scene

#### Returns

`void`

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[register](../interfaces/ISceneComponent.md#register)

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderPipelineManagerSceneComponent.ts:63
