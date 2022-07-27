[@dev/core](../README.md) / [Exports](../modules.md) / SerializationHelper

# Class: SerializationHelper

Class used to help serialization objects

## Table of contents

### Constructors

- [constructor](SerializationHelper.md#constructor)

### Properties

- [AllowLoadingUniqueId](SerializationHelper.md#allowloadinguniqueid)

### Methods

- [AppendSerializedAnimations](SerializationHelper.md#appendserializedanimations)
- [Clone](SerializationHelper.md#clone)
- [Instanciate](SerializationHelper.md#instanciate)
- [Parse](SerializationHelper.md#parse)
- [Serialize](SerializationHelper.md#serialize)

## Constructors

### constructor

• **new SerializationHelper**()

## Properties

### AllowLoadingUniqueId

▪ `Static` **AllowLoadingUniqueId**: `boolean` = `false`

Gets or sets a boolean to indicate if the UniqueId property should be serialized

#### Defined in

packages/dev/core/src/Misc/decorators.ts:228

## Methods

### AppendSerializedAnimations

▸ `Static` **AppendSerializedAnimations**(`source`, `destination`): `void`

Appends the serialized animations from the source animations

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | [`IAnimatable`](../interfaces/IAnimatable.md) | Source containing the animations |
| `destination` | `any` | Target to store the animations |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/decorators.ts:269

___

### Clone

▸ `Static` **Clone**`T`(`creationFunction`, `source`): `T`

Clones an object

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `creationFunction` | () => `T` | defines the function used to instanciate the new object |
| `source` | `T` | defines the source object |

#### Returns

`T`

the cloned object

#### Defined in

packages/dev/core/src/Misc/decorators.ts:442

___

### Instanciate

▸ `Static` **Instanciate**`T`(`creationFunction`, `source`): `T`

Instanciates a new object based on a source one (some data will be shared between both object)

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `creationFunction` | () => `T` | defines the function used to instanciate the new object |
| `source` | `T` | defines the source object |

#### Returns

`T`

the new object

#### Defined in

packages/dev/core/src/Misc/decorators.ts:452

___

### Parse

▸ `Static` **Parse**`T`(`creationFunction`, `source`, `scene`, `rootUrl?`): `T`

Creates a new entity from a serialization data object

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `creationFunction` | () => `T` | `undefined` | defines a function used to instanciated the new entity |
| `source` | `any` | `undefined` | defines the source serialization data |
| `scene` | [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) | `undefined` | defines the hosting scene |
| `rootUrl` | [`Nullable`](../modules.md#nullable)`string` | `null` | defines the root url for resources |

#### Returns

`T`

a new entity

#### Defined in

packages/dev/core/src/Misc/decorators.ts:361

___

### Serialize

▸ `Static` **Serialize**`T`(`entity`, `serializationObject?`): `any`

Static function used to serialized a specific entity

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `entity` | `T` | defines the entity to serialize |
| `serializationObject?` | `any` | defines the optional target object where serialization data will be stored |

#### Returns

`any`

a JSON compatible object representing the serialization of the entity

#### Defined in

packages/dev/core/src/Misc/decorators.ts:286
