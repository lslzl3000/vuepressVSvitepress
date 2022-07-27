[@dev/core](../README.md) / [Exports](../modules.md) / DepthRendererSceneComponent

# Class: DepthRendererSceneComponent

Defines the Depth Renderer scene component responsible to manage a depth buffer useful
in several rendering techniques.

## Implements

- [`ISceneComponent`](../interfaces/ISceneComponent.md)

## Table of contents

### Constructors

- [constructor](DepthRendererSceneComponent.md#constructor)

### Properties

- [name](DepthRendererSceneComponent.md#name)
- [scene](DepthRendererSceneComponent.md#scene)

### Methods

- [\_gatherActiveCameraRenderTargets](DepthRendererSceneComponent.md#_gatheractivecamerarendertargets)
- [\_gatherRenderTargets](DepthRendererSceneComponent.md#_gatherrendertargets)
- [dispose](DepthRendererSceneComponent.md#dispose)
- [rebuild](DepthRendererSceneComponent.md#rebuild)
- [register](DepthRendererSceneComponent.md#register)

## Constructors

### constructor

• **new DepthRendererSceneComponent**(`scene`)

Creates a new instance of the component for the given scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | Defines the scene to register the component in |

#### Defined in

https://github.com/babylon.js/core/src/Rendering/depthRendererSceneComponent.ts:85

## Properties

### name

• `Readonly` **name**: ``"DepthRenderer"``

The component name helpful to identify the component in the list of scene components.

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[name](../interfaces/ISceneComponent.md#name)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/depthRendererSceneComponent.ts:74

___

### scene

• **scene**: [`Scene`](Scene.md)

The scene the component belongs to.

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[scene](../interfaces/ISceneComponent.md#scene)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/depthRendererSceneComponent.ts:79

## Methods

### \_gatherActiveCameraRenderTargets

▸ `Private` **_gatherActiveCameraRenderTargets**(`renderTargets`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `renderTargets` | [`SmartArrayNoDuplicate`](SmartArrayNoDuplicate.md)[`RenderTargetTexture`](RenderTargetTexture.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/depthRendererSceneComponent.ts:129

___

### \_gatherRenderTargets

▸ `Private` **_gatherRenderTargets**(`renderTargets`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `renderTargets` | [`SmartArrayNoDuplicate`](SmartArrayNoDuplicate.md)[`RenderTargetTexture`](RenderTargetTexture.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/depthRendererSceneComponent.ts:118

___

### dispose

▸ **dispose**(): `void`

Disposes the component and the associated resources

#### Returns

`void`

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[dispose](../interfaces/ISceneComponent.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/depthRendererSceneComponent.ts:112

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

https://github.com/babylon.js/core/src/Rendering/depthRendererSceneComponent.ts:105

___

### register

▸ **register**(): `void`

Registers the component in a given scene

#### Returns

`void`

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[register](../interfaces/ISceneComponent.md#register)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/depthRendererSceneComponent.ts:92
