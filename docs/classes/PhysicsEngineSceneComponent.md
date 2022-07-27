[@dev/core](../README.md) / [Exports](../modules.md) / PhysicsEngineSceneComponent

# Class: PhysicsEngineSceneComponent

Defines the physics engine scene component responsible to manage a physics engine

## Implements

- [`ISceneComponent`](../interfaces/ISceneComponent.md)

## Table of contents

### Constructors

- [constructor](PhysicsEngineSceneComponent.md#constructor)

### Properties

- [name](PhysicsEngineSceneComponent.md#name)
- [scene](PhysicsEngineSceneComponent.md#scene)

### Methods

- [dispose](PhysicsEngineSceneComponent.md#dispose)
- [rebuild](PhysicsEngineSceneComponent.md#rebuild)
- [register](PhysicsEngineSceneComponent.md#register)

## Constructors

### constructor

• **new PhysicsEngineSceneComponent**(`scene`)

Creates a new instance of the component for the given scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | Defines the scene to register the component in |

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsEngineComponent.ts:293

## Properties

### name

• `Readonly` **name**: ``"PhysicsEngine"``

The component name helpful to identify the component in the list of scene components.

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[name](../interfaces/ISceneComponent.md#name)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsEngineComponent.ts:282

___

### scene

• **scene**: [`Scene`](Scene.md)

The scene the component belongs to.

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[scene](../interfaces/ISceneComponent.md#scene)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsEngineComponent.ts:287

## Methods

### dispose

▸ **dispose**(): `void`

Disposes the component and the associated resources

#### Returns

`void`

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[dispose](../interfaces/ISceneComponent.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsEngineComponent.ts:324

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

https://github.com/babylon.js/core/src/Physics/physicsEngineComponent.ts:317

___

### register

▸ **register**(): `void`

Registers the component in a given scene

#### Returns

`void`

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[register](../interfaces/ISceneComponent.md#register)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsEngineComponent.ts:311
