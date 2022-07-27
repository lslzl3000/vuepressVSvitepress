[@dev/core](../README.md) / [Exports](../modules.md) / DataReader

# Class: DataReader

Utility class for reading from a data buffer

## Table of contents

### Constructors

- [constructor](DataReader.md#constructor)

### Properties

- [\_dataByteOffset](DataReader.md#_databyteoffset)
- [\_dataView](DataReader.md#_dataview)
- [buffer](DataReader.md#buffer)
- [byteOffset](DataReader.md#byteoffset)

### Methods

- [loadAsync](DataReader.md#loadasync)
- [readString](DataReader.md#readstring)
- [readUint32](DataReader.md#readuint32)
- [readUint8Array](DataReader.md#readuint8array)
- [skipBytes](DataReader.md#skipbytes)

## Constructors

### constructor

• **new DataReader**(`buffer`)

Constructor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `buffer` | [`IDataBuffer`](../interfaces/IDataBuffer.md) | The buffer to read |

#### Defined in

packages/dev/core/src/Misc/dataReader.ts:42

## Properties

### \_dataByteOffset

• `Private` **\_dataByteOffset**: `number`

#### Defined in

packages/dev/core/src/Misc/dataReader.ts:36

___

### \_dataView

• `Private` **\_dataView**: `DataView`

#### Defined in

packages/dev/core/src/Misc/dataReader.ts:35

___

### buffer

• `Readonly` **buffer**: [`IDataBuffer`](../interfaces/IDataBuffer.md)

The data buffer associated with this data reader.

#### Defined in

packages/dev/core/src/Misc/dataReader.ts:28

___

### byteOffset

• **byteOffset**: `number` = `0`

The current byte offset from the beginning of the data buffer.

#### Defined in

packages/dev/core/src/Misc/dataReader.ts:33

## Methods

### loadAsync

▸ **loadAsync**(`byteLength`): `Promise``void`

Loads the given byte length.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `byteLength` | `number` | The byte length to load |

#### Returns

`Promise``void`

A promise that resolves when the load is complete

#### Defined in

packages/dev/core/src/Misc/dataReader.ts:51

___

### readString

▸ **readString**(`byteLength`): `string`

Read a string from the currently loaded data range.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `byteLength` | `number` | The byte length to read |

#### Returns

`string`

The string read

#### Defined in

packages/dev/core/src/Misc/dataReader.ts:86

___

### readUint32

▸ **readUint32**(): `number`

Read a unsigned 32-bit integer from the currently loaded data range.

#### Returns

`number`

The 32-bit integer read

#### Defined in

packages/dev/core/src/Misc/dataReader.ts:62

___

### readUint8Array

▸ **readUint8Array**(`byteLength`): `Uint8Array`

Read a byte array from the currently loaded data range.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `byteLength` | `number` | The byte length to read |

#### Returns

`Uint8Array`

The byte array read

#### Defined in

packages/dev/core/src/Misc/dataReader.ts:74

___

### skipBytes

▸ **skipBytes**(`byteLength`): `void`

Skips the given byte length the currently loaded data range.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `byteLength` | `number` | The byte length to skip |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/dataReader.ts:94
