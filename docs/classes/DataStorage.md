[@dev/core](../README.md) / [Exports](../modules.md) / DataStorage

# Class: DataStorage

Class for storing data to local storage if available or in-memory storage otherwise

## Table of contents

### Constructors

- [constructor](DataStorage.md#constructor)

### Properties

- [\_Storage](DataStorage.md#_storage)

### Methods

- [ReadBoolean](DataStorage.md#readboolean)
- [ReadNumber](DataStorage.md#readnumber)
- [ReadString](DataStorage.md#readstring)
- [WriteBoolean](DataStorage.md#writeboolean)
- [WriteNumber](DataStorage.md#writenumber)
- [WriteString](DataStorage.md#writestring)
- [\_GetStorage](DataStorage.md#_getstorage)

## Constructors

### constructor

• **new DataStorage**()

## Properties

### \_Storage

▪ `Static` `Private` **\_Storage**: `IStorage`

#### Defined in

packages/dev/core/src/Misc/dataStorage.ts:10

## Methods

### ReadBoolean

▸ `Static` **ReadBoolean**(`key`, `defaultValue`): `boolean`

Reads a boolean from the data storage

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | `string` | The key to read |
| `defaultValue` | `boolean` | The value if the key doesn't exist |

#### Returns

`boolean`

The boolean value

#### Defined in

packages/dev/core/src/Misc/dataStorage.ts:57

___

### ReadNumber

▸ `Static` **ReadNumber**(`key`, `defaultValue`): `number`

Reads a number from the data storage

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | `string` | The key to read |
| `defaultValue` | `number` | The value if the key doesn't exist |

#### Returns

`number`

The number value

#### Defined in

packages/dev/core/src/Misc/dataStorage.ts:77

___

### ReadString

▸ `Static` **ReadString**(`key`, `defaultValue`): `string`

Reads a string from the data storage

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | `string` | The key to read |
| `defaultValue` | `string` | The value if the key doesn't exist |

#### Returns

`string`

The string value

#### Defined in

packages/dev/core/src/Misc/dataStorage.ts:37

___

### WriteBoolean

▸ `Static` **WriteBoolean**(`key`, `value`): `void`

Writes a boolean to the data storage

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | `string` | The key to write |
| `value` | `boolean` | The value to write |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/dataStorage.ts:67

___

### WriteNumber

▸ `Static` **WriteNumber**(`key`, `value`): `void`

Writes a number to the data storage

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | `string` | The key to write |
| `value` | `number` | The value to write |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/dataStorage.ts:87

___

### WriteString

▸ `Static` **WriteString**(`key`, `value`): `void`

Writes a string to the data storage

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | `string` | The key to write |
| `value` | `string` | The value to write |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/dataStorage.ts:47

___

### \_GetStorage

▸ `Static` `Private` **_GetStorage**(): `IStorage`

#### Returns

`IStorage`

#### Defined in

packages/dev/core/src/Misc/dataStorage.ts:12
