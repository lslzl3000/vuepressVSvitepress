[@dev/core](../README.md) / [Exports](../modules.md) / DepthPeelingSceneComponent

# Class: DepthPeelingSceneComponent

Scene component to render order independent transparency with depth peeling

## Implements

- [`ISceneComponent`](../interfaces/ISceneComponent.md)

## Table of contents

### Constructors

- [constructor](DepthPeelingSceneComponent.md#constructor)

### Properties

- [name](DepthPeelingSceneComponent.md#name)
- [scene](DepthPeelingSceneComponent.md#scene)

### Methods

- [dispose](DepthPeelingSceneComponent.md#dispose)
- [rebuild](DepthPeelingSceneComponent.md#rebuild)
- [register](DepthPeelingSceneComponent.md#register)

## Constructors

### constructor

• **new DepthPeelingSceneComponent**(`scene`)

Creates a new instance of the component for the given scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | Defines the scene to register the component in |

#### Defined in

packages/dev/core/src/Rendering/depthPeelingSceneComponent.ts:79

## Properties

### name

• `Readonly` **name**: ``"DepthPeelingRenderer"``

The component name helpful to identify the component in the list of scene components.

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[name](../interfaces/ISceneComponent.md#name)

#### Defined in

packages/dev/core/src/Rendering/depthPeelingSceneComponent.ts:68

___

### scene

• **scene**: [`Scene`](Scene.md)

The scene the component belongs to.

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[scene](../interfaces/ISceneComponent.md#scene)

#### Defined in

packages/dev/core/src/Rendering/depthPeelingSceneComponent.ts:73

## Methods

### dispose

▸ **dispose**(): `void`

Disposes the component and the associated resources.

#### Returns

`void`

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[dispose](../interfaces/ISceneComponent.md#dispose)

#### Defined in

packages/dev/core/src/Rendering/depthPeelingSceneComponent.ts:99

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

packages/dev/core/src/Rendering/depthPeelingSceneComponent.ts:94

___

### register

▸ **register**(): `void`

Registers the component in a given scene

#### Returns

`void`

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[register](../interfaces/ISceneComponent.md#register)

#### Defined in

packages/dev/core/src/Rendering/depthPeelingSceneComponent.ts:88
