[@dev/core](../README.md) / [Exports](../modules.md) / Buffer

# Class: Buffer

Class used to store data that will be store in GPU memory

## Table of contents

### Constructors

- [constructor](Buffer.md#constructor)

### Properties

- [\_buffer](Buffer.md#_buffer)
- [\_divisor](Buffer.md#_divisor)
- [\_engine](Buffer.md#_engine)
- [\_instanced](Buffer.md#_instanced)
- [\_isAlreadyOwned](Buffer.md#_isalreadyowned)
- [\_updatable](Buffer.md#_updatable)
- [byteStride](Buffer.md#bytestride)

### Methods

- [create](Buffer.md#create)
- [createVertexBuffer](Buffer.md#createvertexbuffer)
- [dispose](Buffer.md#dispose)
- [getBuffer](Buffer.md#getbuffer)
- [getData](Buffer.md#getdata)
- [getStrideSize](Buffer.md#getstridesize)
- [isUpdatable](Buffer.md#isupdatable)
- [update](Buffer.md#update)
- [updateDirectly](Buffer.md#updatedirectly)

## Constructors

### constructor

• **new Buffer**(`engine`, `data`, `updatable`, `stride?`, `postponeInternalCreation?`, `instanced?`, `useBytes?`, `divisor?`)

Constructor

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `engine` | `any` | `undefined` | the engine |
| `data` | [`DataArray`](../modules.md#dataarray) \| [`DataBuffer`](DataBuffer.md) | `undefined` | the data to use for this buffer |
| `updatable` | `boolean` | `undefined` | whether the data is updatable |
| `stride` | `number` | `0` | the stride (optional) |
| `postponeInternalCreation` | `boolean` | `false` | whether to postpone creating the internal WebGL buffer (optional) |
| `instanced` | `boolean` | `false` | whether the buffer is instanced (optional) |
| `useBytes` | `boolean` | `false` | set to true if the stride in in bytes (optional) |
| `divisor?` | `number` | `undefined` | sets an optional divisor for instances (1 by default) |

#### Defined in

packages/dev/core/src/Buffers/buffer.ts:34

## Properties

### \_buffer

• `Private` **\_buffer**: [`Nullable`](../modules.md#nullable)[`DataBuffer`](DataBuffer.md)

#### Defined in

packages/dev/core/src/Buffers/buffer.ts:10

___

### \_divisor

• `Private` **\_divisor**: `number`

#### Defined in

packages/dev/core/src/Buffers/buffer.ts:15

___

### \_engine

• `Private` **\_engine**: [`ThinEngine`](ThinEngine.md)

#### Defined in

packages/dev/core/src/Buffers/buffer.ts:9

___

### \_instanced

• `Private` **\_instanced**: `boolean`

#### Defined in

packages/dev/core/src/Buffers/buffer.ts:14

___

### \_isAlreadyOwned

• `Private` **\_isAlreadyOwned**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Buffers/buffer.ts:16

___

### \_updatable

• `Private` **\_updatable**: `boolean`

#### Defined in

packages/dev/core/src/Buffers/buffer.ts:13

___

### byteStride

• `Readonly` **byteStride**: `number`

Gets the byte stride.

#### Defined in

packages/dev/core/src/Buffers/buffer.ts:21

## Methods

### create

▸ **create**(`data?`): `void`

Store data into the buffer. Creates the buffer if not used already.
If the buffer was already used, it will be updated only if it is updatable, otherwise it will do nothing.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `data` | [`Nullable`](../modules.md#nullable)[`DataArray`](../modules.md#dataarray) | `null` | defines the data to store |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Buffers/buffer.ts:147

___

### createVertexBuffer

▸ **createVertexBuffer**(`kind`, `offset`, `size`, `stride?`, `instanced?`, `useBytes?`, `divisor?`): [`VertexBuffer`](VertexBuffer.md)

Create a new VertexBuffer based on the current buffer

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `kind` | `string` | `undefined` | defines the vertex buffer kind (position, normal, etc.) |
| `offset` | `number` | `undefined` | defines offset in the buffer (0 by default) |
| `size` | `number` | `undefined` | defines the size in floats of attributes (position is 3 for instance) |
| `stride?` | `number` | `undefined` | defines the stride size in floats in the buffer (the offset to apply to reach next value when data is interleaved) |
| `instanced?` | `boolean` | `undefined` | defines if the vertex buffer contains indexed data |
| `useBytes` | `boolean` | `false` | defines if the offset and stride are in bytes     * |
| `divisor?` | `number` | `undefined` | sets an optional divisor for instances (1 by default) |

#### Returns

[`VertexBuffer`](VertexBuffer.md)

the new vertex buffer

#### Defined in

packages/dev/core/src/Buffers/buffer.ts:82

___

### dispose

▸ **dispose**(): `void`

Release all resources

#### Returns

`void`

#### Defined in

packages/dev/core/src/Buffers/buffer.ts:233

___

### getBuffer

▸ **getBuffer**(): [`Nullable`](../modules.md#nullable)[`DataBuffer`](DataBuffer.md)

Gets underlying native buffer

#### Returns

[`Nullable`](../modules.md#nullable)[`DataBuffer`](DataBuffer.md)

underlying native buffer

#### Defined in

packages/dev/core/src/Buffers/buffer.ts:126

___

### getData

▸ **getData**(): [`Nullable`](../modules.md#nullable)[`DataArray`](../modules.md#dataarray)

Gets current buffer's data

#### Returns

[`Nullable`](../modules.md#nullable)[`DataArray`](../modules.md#dataarray)

a DataArray or null

#### Defined in

packages/dev/core/src/Buffers/buffer.ts:118

___

### getStrideSize

▸ **getStrideSize**(): `number`

Gets the stride in float32 units (i.e. byte stride / 4).
May not be an integer if the byte stride is not divisible by 4.

**`Deprecated`**

Please use byteStride instead.

#### Returns

`number`

the stride in float32 units

#### Defined in

packages/dev/core/src/Buffers/buffer.ts:136

___

### isUpdatable

▸ **isUpdatable**(): `boolean`

Gets a boolean indicating if the Buffer is updatable?

#### Returns

`boolean`

true if the buffer is updatable

#### Defined in

packages/dev/core/src/Buffers/buffer.ts:110

___

### update

▸ **update**(`data`): `void`

Update current buffer data

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | [`DataArray`](../modules.md#dataarray) | defines the data to store |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Buffers/buffer.ts:183

___

### updateDirectly

▸ **updateDirectly**(`data`, `offset`, `vertexCount?`, `useBytes?`): `void`

Updates the data directly.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `data` | [`DataArray`](../modules.md#dataarray) | `undefined` | the new data |
| `offset` | `number` | `undefined` | the new offset |
| `vertexCount?` | `number` | `undefined` | the vertex count (optional) |
| `useBytes` | `boolean` | `false` | set to true if the offset is in bytes |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Buffers/buffer.ts:194
