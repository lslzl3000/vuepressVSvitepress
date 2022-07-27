[@dev/core](../README.md) / [Exports](../modules.md) / IDataBuffer

# Interface: IDataBuffer

Interface for a data buffer

## Table of contents

### Properties

- [byteLength](IDataBuffer.md#bytelength)

### Methods

- [readAsync](IDataBuffer.md#readasync)

## Properties

### byteLength

• `Readonly` **byteLength**: `number`

The byte length of the buffer.

#### Defined in

https://github.com/babylon.js/core/src/Misc/dataReader.ts:18

## Methods

### readAsync

▸ **readAsync**(`byteOffset`, `byteLength`): `Promise``ArrayBufferView`

Reads bytes from the data buffer.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `byteOffset` | `number` | The byte offset to read |
| `byteLength` | `number` | The byte length to read |

#### Returns

`Promise``ArrayBufferView`

A promise that resolves when the bytes are read

#### Defined in

https://github.com/babylon.js/core/src/Misc/dataReader.ts:13
