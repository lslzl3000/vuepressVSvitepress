[@dev/core](../README.md) / [Exports](../modules.md) / DataBuffer

# Class: DataBuffer

Class used to store gfx data (like WebGLBuffer)

## Table of contents

### Constructors

- [constructor](DataBuffer.md#constructor)

### Properties

- [capacity](DataBuffer.md#capacity)
- [is32Bits](DataBuffer.md#is32bits)
- [references](DataBuffer.md#references)
- [uniqueId](DataBuffer.md#uniqueid)
- [\_Counter](DataBuffer.md#_counter)

### Accessors

- [underlyingResource](DataBuffer.md#underlyingresource)

## Constructors

### constructor

• **new DataBuffer**()

Constructs the buffer

#### Defined in

packages/dev/core/src/Buffers/dataBuffer.ts:33

## Properties

### capacity

• **capacity**: `number` = `0`

Gets or sets the size of the underlying buffer

#### Defined in

packages/dev/core/src/Buffers/dataBuffer.ts:12

___

### is32Bits

• **is32Bits**: `boolean` = `false`

Gets or sets a boolean indicating if the buffer contains 32bits indices

#### Defined in

packages/dev/core/src/Buffers/dataBuffer.ts:16

___

### references

• **references**: `number` = `0`

Gets or sets the number of objects referencing this buffer

#### Defined in

packages/dev/core/src/Buffers/dataBuffer.ts:10

___

### uniqueId

• `Readonly` **uniqueId**: `number`

Gets the unique id of this buffer

#### Defined in

packages/dev/core/src/Buffers/dataBuffer.ts:28

___

### \_Counter

▪ `Static` `Private` **\_Counter**: `number` = `0`

#### Defined in

packages/dev/core/src/Buffers/dataBuffer.ts:5

## Accessors

### underlyingResource

• `get` **underlyingResource**(): `any`

Gets the underlying buffer

#### Returns

`any`

#### Defined in

packages/dev/core/src/Buffers/dataBuffer.ts:21
