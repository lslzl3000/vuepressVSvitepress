[@dev/core](../README.md) / [Exports](../modules.md) / ISceneComponent

# Interface: ISceneComponent

This represents a scene component.

This is used to decouple the dependency the scene is having on the different workloads like
layers, post processes...

## Hierarchy

- **`ISceneComponent`**

  ↳ [`ISceneSerializableComponent`](ISceneSerializableComponent.md)

## Implemented by

- [`BoundingBoxRenderer`](../classes/BoundingBoxRenderer.md)
- [`DepthPeelingSceneComponent`](../classes/DepthPeelingSceneComponent.md)
- [`DepthRendererSceneComponent`](../classes/DepthRendererSceneComponent.md)
- [`GamepadSystemSceneComponent`](../classes/GamepadSystemSceneComponent.md)
- [`GeometryBufferRendererSceneComponent`](../classes/GeometryBufferRendererSceneComponent.md)
- [`LayerSceneComponent`](../classes/LayerSceneComponent.md)
- [`OutlineRenderer`](../classes/OutlineRenderer.md)
- [`PhysicsEngineSceneComponent`](../classes/PhysicsEngineSceneComponent.md)
- [`PostProcessRenderPipelineManagerSceneComponent`](../classes/PostProcessRenderPipelineManagerSceneComponent.md)
- [`PrePassRendererSceneComponent`](../classes/PrePassRendererSceneComponent.md)
- [`ProceduralTextureSceneComponent`](../classes/ProceduralTextureSceneComponent.md)
- [`SimplicationQueueSceneComponent`](../classes/SimplicationQueueSceneComponent.md)
- [`SpriteSceneComponent`](../classes/SpriteSceneComponent.md)

## Table of contents

### Properties

- [name](ISceneComponent.md#name)
- [scene](ISceneComponent.md#scene)

### Methods

- [dispose](ISceneComponent.md#dispose)
- [rebuild](ISceneComponent.md#rebuild)
- [register](ISceneComponent.md#register)

## Properties

### name

• **name**: `string`

The name of the component. Each component must have a unique name.

#### Defined in

https://github.com/babylon.js/core/src/sceneComponent.ts:108

___

### scene

• **scene**: [`Scene`](../classes/Scene.md)

The scene the component belongs to.

#### Defined in

https://github.com/babylon.js/core/src/sceneComponent.ts:113

## Methods

### dispose

▸ **dispose**(): `void`

Disposes the component and the associated ressources.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/sceneComponent.ts:129

___

### rebuild

▸ **rebuild**(): `void`

Rebuilds the elements related to this component in case of
context lost for instance.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/sceneComponent.ts:124

___

### register

▸ **register**(): `void`

Register the component to one instance of a scene.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/sceneComponent.ts:118
