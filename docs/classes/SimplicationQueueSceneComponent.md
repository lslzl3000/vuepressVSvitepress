[@dev/core](../README.md) / [Exports](../modules.md) / SimplicationQueueSceneComponent

# Class: SimplicationQueueSceneComponent

Defines the simplification queue scene component responsible to help scheduling the various simplification task
created in a scene

## Implements

- [`ISceneComponent`](../interfaces/ISceneComponent.md)

## Table of contents

### Constructors

- [constructor](SimplicationQueueSceneComponent.md#constructor)

### Properties

- [name](SimplicationQueueSceneComponent.md#name)
- [scene](SimplicationQueueSceneComponent.md#scene)

### Methods

- [\_beforeCameraUpdate](SimplicationQueueSceneComponent.md#_beforecameraupdate)
- [dispose](SimplicationQueueSceneComponent.md#dispose)
- [rebuild](SimplicationQueueSceneComponent.md#rebuild)
- [register](SimplicationQueueSceneComponent.md#register)

## Constructors

### constructor

• **new SimplicationQueueSceneComponent**(`scene`)

Creates a new instance of the component for the given scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | Defines the scene to register the component in |

#### Defined in

https://github.com/babylon.js/core/src/Meshes/meshSimplificationSceneComponent.ts:94

## Properties

### name

• `Readonly` **name**: ``"SimplificationQueue"``

The component name helpfull to identify the component in the list of scene components.

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[name](../interfaces/ISceneComponent.md#name)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/meshSimplificationSceneComponent.ts:83

___

### scene

• **scene**: [`Scene`](Scene.md)

The scene the component belongs to.

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[scene](../interfaces/ISceneComponent.md#scene)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/meshSimplificationSceneComponent.ts:88

## Methods

### \_beforeCameraUpdate

▸ `Private` **_beforeCameraUpdate**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/meshSimplificationSceneComponent.ts:120

___

### dispose

▸ **dispose**(): `void`

Disposes the component and the associated resources

#### Returns

`void`

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[dispose](../interfaces/ISceneComponent.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/meshSimplificationSceneComponent.ts:116

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

https://github.com/babylon.js/core/src/Meshes/meshSimplificationSceneComponent.ts:109

___

### register

▸ **register**(): `void`

Registers the component in a given scene

#### Returns

`void`

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[register](../interfaces/ISceneComponent.md#register)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/meshSimplificationSceneComponent.ts:101
