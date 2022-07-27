[@dev/core](../README.md) / [Exports](../modules.md) / SubSurfaceSceneComponent

# Class: SubSurfaceSceneComponent

Defines the Geometry Buffer scene component responsible to manage a G-Buffer useful
in several rendering techniques.

## Implements

- [`ISceneSerializableComponent`](../interfaces/ISceneSerializableComponent.md)

## Table of contents

### Constructors

- [constructor](SubSurfaceSceneComponent.md#constructor)

### Properties

- [name](SubSurfaceSceneComponent.md#name)
- [scene](SubSurfaceSceneComponent.md#scene)

### Methods

- [addFromContainer](SubSurfaceSceneComponent.md#addfromcontainer)
- [dispose](SubSurfaceSceneComponent.md#dispose)
- [rebuild](SubSurfaceSceneComponent.md#rebuild)
- [register](SubSurfaceSceneComponent.md#register)
- [removeFromContainer](SubSurfaceSceneComponent.md#removefromcontainer)
- [serialize](SubSurfaceSceneComponent.md#serialize)

## Constructors

### constructor

• **new SubSurfaceSceneComponent**(`scene`)

Creates a new instance of the component for the given scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | Defines the scene to register the component in |

#### Defined in

https://github.com/babylon.js/core/src/Rendering/subSurfaceSceneComponent.ts:104

## Properties

### name

• `Readonly` **name**: ``"PrePassRenderer"``

The component name helpful to identify the component in the list of scene components.

#### Implementation of

[ISceneSerializableComponent](../interfaces/ISceneSerializableComponent.md).[name](../interfaces/ISceneSerializableComponent.md#name)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/subSurfaceSceneComponent.ts:93

___

### scene

• **scene**: [`Scene`](Scene.md)

The scene the component belongs to.

#### Implementation of

[ISceneSerializableComponent](../interfaces/ISceneSerializableComponent.md).[scene](../interfaces/ISceneSerializableComponent.md#scene)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/subSurfaceSceneComponent.ts:98

## Methods

### addFromContainer

▸ **addFromContainer**(): `void`

Adds all the elements from the container to the scene

#### Returns

`void`

#### Implementation of

[ISceneSerializableComponent](../interfaces/ISceneSerializableComponent.md).[addFromContainer](../interfaces/ISceneSerializableComponent.md#addfromcontainer)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/subSurfaceSceneComponent.ts:137

___

### dispose

▸ **dispose**(): `void`

Disposes the component and the associated resources

#### Returns

`void`

#### Implementation of

[ISceneSerializableComponent](../interfaces/ISceneSerializableComponent.md).[dispose](../interfaces/ISceneSerializableComponent.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/subSurfaceSceneComponent.ts:166

___

### rebuild

▸ **rebuild**(): `void`

Rebuilds the elements related to this component in case of
context lost for instance.

#### Returns

`void`

#### Implementation of

[ISceneSerializableComponent](../interfaces/ISceneSerializableComponent.md).[rebuild](../interfaces/ISceneSerializableComponent.md#rebuild)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/subSurfaceSceneComponent.ts:159

___

### register

▸ **register**(): `void`

Registers the component in a given scene

#### Returns

`void`

#### Implementation of

[ISceneSerializableComponent](../interfaces/ISceneSerializableComponent.md).[register](../interfaces/ISceneSerializableComponent.md#register)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/subSurfaceSceneComponent.ts:111

___

### removeFromContainer

▸ **removeFromContainer**(): `void`

Removes all the elements in the container from the scene

#### Returns

`void`

#### Implementation of

[ISceneSerializableComponent](../interfaces/ISceneSerializableComponent.md).[removeFromContainer](../interfaces/ISceneSerializableComponent.md#removefromcontainer)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/subSurfaceSceneComponent.ts:144

___

### serialize

▸ **serialize**(`serializationObject`): `void`

Serializes the component data to the specified json object

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `serializationObject` | `any` | The object to serialize to |

#### Returns

`void`

#### Implementation of

[ISceneSerializableComponent](../interfaces/ISceneSerializableComponent.md).[serialize](../interfaces/ISceneSerializableComponent.md#serialize)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/subSurfaceSceneComponent.ts:117
