[@dev/core](../README.md) / [Exports](../modules.md) / LensFlareSystemSceneComponent

# Class: LensFlareSystemSceneComponent

Defines the lens flare scene component responsible to manage any lens flares
in a given scene.

## Implements

- [`ISceneSerializableComponent`](../interfaces/ISceneSerializableComponent.md)

## Table of contents

### Constructors

- [constructor](LensFlareSystemSceneComponent.md#constructor)

### Properties

- [name](LensFlareSystemSceneComponent.md#name)
- [scene](LensFlareSystemSceneComponent.md#scene)

### Methods

- [\_draw](LensFlareSystemSceneComponent.md#_draw)
- [addFromContainer](LensFlareSystemSceneComponent.md#addfromcontainer)
- [dispose](LensFlareSystemSceneComponent.md#dispose)
- [rebuild](LensFlareSystemSceneComponent.md#rebuild)
- [register](LensFlareSystemSceneComponent.md#register)
- [removeFromContainer](LensFlareSystemSceneComponent.md#removefromcontainer)
- [serialize](LensFlareSystemSceneComponent.md#serialize)

## Constructors

### constructor

• **new LensFlareSystemSceneComponent**(`scene`)

Creates a new instance of the component for the given scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | Defines the scene to register the component in |

#### Defined in

packages/dev/core/src/LensFlares/lensFlareSystemSceneComponent.ts:126

## Properties

### name

• `Readonly` **name**: ``"LensFlareSystem"``

The component name helpful to identify the component in the list of scene components.

#### Implementation of

[ISceneSerializableComponent](../interfaces/ISceneSerializableComponent.md).[name](../interfaces/ISceneSerializableComponent.md#name)

#### Defined in

packages/dev/core/src/LensFlares/lensFlareSystemSceneComponent.ts:115

___

### scene

• **scene**: [`Scene`](Scene.md)

The scene the component belongs to.

#### Implementation of

[ISceneSerializableComponent](../interfaces/ISceneSerializableComponent.md).[scene](../interfaces/ISceneSerializableComponent.md#scene)

#### Defined in

packages/dev/core/src/LensFlares/lensFlareSystemSceneComponent.ts:120

## Methods

### \_draw

▸ `Private` **_draw**(`camera`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `camera` | [`Camera`](Camera.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/LensFlares/lensFlareSystemSceneComponent.ts:202

___

### addFromContainer

▸ **addFromContainer**(`container`): `void`

Adds all the elements from the container to the scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `container` | [`AbstractScene`](AbstractScene.md) | the container holding the elements |

#### Returns

`void`

#### Implementation of

[ISceneSerializableComponent](../interfaces/ISceneSerializableComponent.md).[addFromContainer](../interfaces/ISceneSerializableComponent.md#addfromcontainer)

#### Defined in

packages/dev/core/src/LensFlares/lensFlareSystemSceneComponent.ts:153

___

### dispose

▸ **dispose**(): `void`

Disposes the component and the associated resources.

#### Returns

`void`

#### Implementation of

[ISceneSerializableComponent](../interfaces/ISceneSerializableComponent.md).[dispose](../interfaces/ISceneSerializableComponent.md#dispose)

#### Defined in

packages/dev/core/src/LensFlares/lensFlareSystemSceneComponent.ts:195

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

packages/dev/core/src/LensFlares/lensFlareSystemSceneComponent.ts:143

___

### register

▸ **register**(): `void`

Registers the component in a given scene

#### Returns

`void`

#### Implementation of

[ISceneSerializableComponent](../interfaces/ISceneSerializableComponent.md).[register](../interfaces/ISceneSerializableComponent.md#register)

#### Defined in

packages/dev/core/src/LensFlares/lensFlareSystemSceneComponent.ts:135

___

### removeFromContainer

▸ **removeFromContainer**(`container`, `dispose?`): `void`

Removes all the elements in the container from the scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `container` | [`AbstractScene`](AbstractScene.md) | contains the elements to remove |
| `dispose?` | `boolean` | if the removed element should be disposed (default: false) |

#### Returns

`void`

#### Implementation of

[ISceneSerializableComponent](../interfaces/ISceneSerializableComponent.md).[removeFromContainer](../interfaces/ISceneSerializableComponent.md#removefromcontainer)

#### Defined in

packages/dev/core/src/LensFlares/lensFlareSystemSceneComponent.ts:167

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

packages/dev/core/src/LensFlares/lensFlareSystemSceneComponent.ts:183
