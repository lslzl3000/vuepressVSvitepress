[@dev/core](../README.md) / [Exports](../modules.md) / ISceneSerializableComponent

# Interface: ISceneSerializableComponent

This represents a SERIALIZABLE scene component.

This extends Scene Component to add Serialization methods on top.

## Hierarchy

- [`ISceneComponent`](ISceneComponent.md)

  ↳ **`ISceneSerializableComponent`**

## Implemented by

- [`AudioSceneComponent`](../classes/AudioSceneComponent.md)
- [`EffectLayerSceneComponent`](../classes/EffectLayerSceneComponent.md)
- [`LensFlareSystemSceneComponent`](../classes/LensFlareSystemSceneComponent.md)
- [`ShadowGeneratorSceneComponent`](../classes/ShadowGeneratorSceneComponent.md)
- [`SubSurfaceSceneComponent`](../classes/SubSurfaceSceneComponent.md)

## Table of contents

### Properties

- [name](ISceneSerializableComponent.md#name)
- [scene](ISceneSerializableComponent.md#scene)

### Methods

- [addFromContainer](ISceneSerializableComponent.md#addfromcontainer)
- [dispose](ISceneSerializableComponent.md#dispose)
- [rebuild](ISceneSerializableComponent.md#rebuild)
- [register](ISceneSerializableComponent.md#register)
- [removeFromContainer](ISceneSerializableComponent.md#removefromcontainer)
- [serialize](ISceneSerializableComponent.md#serialize)

## Properties

### name

• **name**: `string`

The name of the component. Each component must have a unique name.

#### Inherited from

[ISceneComponent](ISceneComponent.md).[name](ISceneComponent.md#name)

#### Defined in

https://github.com/babylon.js/core/src/sceneComponent.ts:108

___

### scene

• **scene**: [`Scene`](../classes/Scene.md)

The scene the component belongs to.

#### Inherited from

[ISceneComponent](ISceneComponent.md).[scene](ISceneComponent.md#scene)

#### Defined in

https://github.com/babylon.js/core/src/sceneComponent.ts:113

## Methods

### addFromContainer

▸ **addFromContainer**(`container`): `void`

Adds all the elements from the container to the scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `container` | [`AbstractScene`](../classes/AbstractScene.md) | the container holding the elements |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/sceneComponent.ts:142

___

### dispose

▸ **dispose**(): `void`

Disposes the component and the associated ressources.

#### Returns

`void`

#### Inherited from

[ISceneComponent](ISceneComponent.md).[dispose](ISceneComponent.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/sceneComponent.ts:129

___

### rebuild

▸ **rebuild**(): `void`

Rebuilds the elements related to this component in case of
context lost for instance.

#### Returns

`void`

#### Inherited from

[ISceneComponent](ISceneComponent.md).[rebuild](ISceneComponent.md#rebuild)

#### Defined in

https://github.com/babylon.js/core/src/sceneComponent.ts:124

___

### register

▸ **register**(): `void`

Register the component to one instance of a scene.

#### Returns

`void`

#### Inherited from

[ISceneComponent](ISceneComponent.md).[register](ISceneComponent.md#register)

#### Defined in

https://github.com/babylon.js/core/src/sceneComponent.ts:118

___

### removeFromContainer

▸ **removeFromContainer**(`container`, `dispose?`): `void`

Removes all the elements in the container from the scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `container` | [`AbstractScene`](../classes/AbstractScene.md) | contains the elements to remove |
| `dispose?` | `boolean` | if the removed element should be disposed (default: false) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/sceneComponent.ts:149

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

#### Defined in

https://github.com/babylon.js/core/src/sceneComponent.ts:155
