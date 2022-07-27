[@dev/core](../README.md) / [Exports](../modules.md) / StorageBuffer

# Class: StorageBuffer

This class is a small wrapper around a native buffer that can be read and/or written

## Table of contents

### Constructors

- [constructor](StorageBuffer.md#constructor)

### Properties

- [\_buffer](StorageBuffer.md#_buffer)
- [\_bufferSize](StorageBuffer.md#_buffersize)
- [\_creationFlags](StorageBuffer.md#_creationflags)
- [\_engine](StorageBuffer.md#_engine)

### Methods

- [\_create](StorageBuffer.md#_create)
- [dispose](StorageBuffer.md#dispose)
- [getBuffer](StorageBuffer.md#getbuffer)
- [read](StorageBuffer.md#read)
- [update](StorageBuffer.md#update)

## Constructors

### constructor

• **new StorageBuffer**(`engine`, `size`, `creationFlags?`)

Creates a new storage buffer instance

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `engine` | [`ThinEngine`](ThinEngine.md) | `undefined` | The engine the buffer will be created inside |
| `size` | `number` | `undefined` | The size of the buffer in bytes |
| `creationFlags` | `number` | `Constants.BUFFER_CREATIONFLAG_READWRITE` | flags to use when creating the buffer (see Constants.BUFFER_CREATIONFLAG_XXX). The BUFFER_CREATIONFLAG_STORAGE flag will be automatically added. |

#### Defined in

packages/dev/core/src/Buffers/storageBuffer.ts:21

## Properties

### \_buffer

• `Private` **\_buffer**: [`DataBuffer`](DataBuffer.md)

#### Defined in

packages/dev/core/src/Buffers/storageBuffer.ts:11

___

### \_bufferSize

• `Private` **\_bufferSize**: `number`

#### Defined in

packages/dev/core/src/Buffers/storageBuffer.ts:12

___

### \_creationFlags

• `Private` **\_creationFlags**: `number`

#### Defined in

packages/dev/core/src/Buffers/storageBuffer.ts:13

___

### \_engine

• `Private` **\_engine**: [`ThinEngine`](ThinEngine.md)

#### Defined in

packages/dev/core/src/Buffers/storageBuffer.ts:10

## Methods

### \_create

▸ `Private` **_create**(`size`, `creationFlags`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `size` | `number` |
| `creationFlags` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Buffers/storageBuffer.ts:27

___

### dispose

▸ **dispose**(): `void`

Disposes the storage buffer

#### Returns

`void`

#### Defined in

packages/dev/core/src/Buffers/storageBuffer.ts:74

___

### getBuffer

▸ **getBuffer**(): [`DataBuffer`](DataBuffer.md)

Gets underlying native buffer

#### Returns

[`DataBuffer`](DataBuffer.md)

underlying native buffer

#### Defined in

packages/dev/core/src/Buffers/storageBuffer.ts:42

___

### read

▸ **read**(`offset?`, `size?`, `buffer?`): `Promise``ArrayBufferView`

Reads data from the storage buffer

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `offset?` | `number` | The offset in the storage buffer to start reading from (default: 0) |
| `size?` | `number` | The number of bytes to read from the storage buffer (default: capacity of the buffer) |
| `buffer?` | `ArrayBufferView` | The buffer to write the data we have read from the storage buffer to (optional) |

#### Returns

`Promise``ArrayBufferView`

If not undefined, returns the (promise) buffer (as provided by the 4th parameter) filled with the data, else it returns a (promise) Uint8Array with the data read from the storage buffer

#### Defined in

packages/dev/core/src/Buffers/storageBuffer.ts:67

___

### update

▸ **update**(`data`, `byteOffset?`, `byteLength?`): `void`

Updates the storage buffer

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | [`DataArray`](../modules.md#dataarray) | the data used to update the storage buffer |
| `byteOffset?` | `number` | the byte offset of the data (optional) |
| `byteLength?` | `number` | the byte length of the data (optional) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Buffers/storageBuffer.ts:52
