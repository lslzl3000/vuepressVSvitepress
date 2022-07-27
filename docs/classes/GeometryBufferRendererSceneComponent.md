[@dev/core](../README.md) / [Exports](../modules.md) / GeometryBufferRendererSceneComponent

# Class: GeometryBufferRendererSceneComponent

Defines the Geometry Buffer scene component responsible to manage a G-Buffer useful
in several rendering techniques.

## Implements

- [`ISceneComponent`](../interfaces/ISceneComponent.md)

## Table of contents

### Constructors

- [constructor](GeometryBufferRendererSceneComponent.md#constructor)

### Properties

- [name](GeometryBufferRendererSceneComponent.md#name)
- [scene](GeometryBufferRendererSceneComponent.md#scene)

### Methods

- [\_gatherRenderTargets](GeometryBufferRendererSceneComponent.md#_gatherrendertargets)
- [dispose](GeometryBufferRendererSceneComponent.md#dispose)
- [rebuild](GeometryBufferRendererSceneComponent.md#rebuild)
- [register](GeometryBufferRendererSceneComponent.md#register)

## Constructors

### constructor

• **new GeometryBufferRendererSceneComponent**(`scene`)

Creates a new instance of the component for the given scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | Defines the scene to register the component in |

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRendererSceneComponent.ts:87

## Properties

### name

• `Readonly` **name**: ``"GeometryBufferRenderer"``

The component name helpful to identify the component in the list of scene components.

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[name](../interfaces/ISceneComponent.md#name)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRendererSceneComponent.ts:76

___

### scene

• **scene**: [`Scene`](Scene.md)

The scene the component belongs to.

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[scene](../interfaces/ISceneComponent.md#scene)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRendererSceneComponent.ts:81

## Methods

### \_gatherRenderTargets

▸ `Private` **_gatherRenderTargets**(`renderTargets`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `renderTargets` | [`SmartArrayNoDuplicate`](SmartArrayNoDuplicate.md)[`RenderTargetTexture`](RenderTargetTexture.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRendererSceneComponent.ts:113

___

### dispose

▸ **dispose**(): `void`

Disposes the component and the associated resources

#### Returns

`void`

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[dispose](../interfaces/ISceneComponent.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRendererSceneComponent.ts:109

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

https://github.com/babylon.js/core/src/Rendering/geometryBufferRendererSceneComponent.ts:102

___

### register

▸ **register**(): `void`

Registers the component in a given scene

#### Returns

`void`

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[register](../interfaces/ISceneComponent.md#register)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRendererSceneComponent.ts:94
