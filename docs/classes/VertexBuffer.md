[@dev/core](../README.md) / [Exports](../modules.md) / VertexBuffer

# Class: VertexBuffer

Specialized buffer used to store vertex data

## Table of contents

### Constructors

- [constructor](VertexBuffer.md#constructor)

### Properties

- [\_instanceDivisor](VertexBuffer.md#_instancedivisor)
- [\_instanced](VertexBuffer.md#_instanced)
- [\_kind](VertexBuffer.md#_kind)
- [\_ownsBuffer](VertexBuffer.md#_ownsbuffer)
- [\_size](VertexBuffer.md#_size)
- [byteOffset](VertexBuffer.md#byteoffset)
- [byteStride](VertexBuffer.md#bytestride)
- [hashCode](VertexBuffer.md#hashcode)
- [normalized](VertexBuffer.md#normalized)
- [type](VertexBuffer.md#type)
- [uniqueId](VertexBuffer.md#uniqueid)
- [BYTE](VertexBuffer.md#byte)
- [ColorInstanceKind](VertexBuffer.md#colorinstancekind)
- [ColorKind](VertexBuffer.md#colorkind)
- [FLOAT](VertexBuffer.md#float)
- [INT](VertexBuffer.md#int)
- [MatricesIndicesExtraKind](VertexBuffer.md#matricesindicesextrakind)
- [MatricesIndicesKind](VertexBuffer.md#matricesindiceskind)
- [MatricesWeightsExtraKind](VertexBuffer.md#matricesweightsextrakind)
- [MatricesWeightsKind](VertexBuffer.md#matricesweightskind)
- [NormalKind](VertexBuffer.md#normalkind)
- [PositionKind](VertexBuffer.md#positionkind)
- [SHORT](VertexBuffer.md#short)
- [TangentKind](VertexBuffer.md#tangentkind)
- [UNSIGNED\_BYTE](VertexBuffer.md#unsigned_byte)
- [UNSIGNED\_INT](VertexBuffer.md#unsigned_int)
- [UNSIGNED\_SHORT](VertexBuffer.md#unsigned_short)
- [UV2Kind](VertexBuffer.md#uv2kind)
- [UV3Kind](VertexBuffer.md#uv3kind)
- [UV4Kind](VertexBuffer.md#uv4kind)
- [UV5Kind](VertexBuffer.md#uv5kind)
- [UV6Kind](VertexBuffer.md#uv6kind)
- [UVKind](VertexBuffer.md#uvkind)
- [\_Counter](VertexBuffer.md#_counter)

### Accessors

- [instanceDivisor](VertexBuffer.md#instancedivisor)

### Methods

- [\_computeHashCode](VertexBuffer.md#_computehashcode)
- [create](VertexBuffer.md#create)
- [dispose](VertexBuffer.md#dispose)
- [forEach](VertexBuffer.md#foreach)
- [getBuffer](VertexBuffer.md#getbuffer)
- [getData](VertexBuffer.md#getdata)
- [getFloatData](VertexBuffer.md#getfloatdata)
- [getInstanceDivisor](VertexBuffer.md#getinstancedivisor)
- [getIsInstanced](VertexBuffer.md#getisinstanced)
- [getKind](VertexBuffer.md#getkind)
- [getOffset](VertexBuffer.md#getoffset)
- [getSize](VertexBuffer.md#getsize)
- [getStrideSize](VertexBuffer.md#getstridesize)
- [isUpdatable](VertexBuffer.md#isupdatable)
- [update](VertexBuffer.md#update)
- [updateDirectly](VertexBuffer.md#updatedirectly)
- [DeduceStride](VertexBuffer.md#deducestride)
- [ForEach](VertexBuffer.md#foreach-1)
- [GetTypeByteLength](VertexBuffer.md#gettypebytelength)
- [\_GetFloatValue](VertexBuffer.md#_getfloatvalue)

## Constructors

### constructor

• **new VertexBuffer**(`engine`, `data`, `kind`, `updatable`, `postponeInternalCreation?`, `stride?`, `instanced?`, `offset?`, `size?`, `type?`, `normalized?`, `useBytes?`, `divisor?`, `takeBufferOwnership?`)

Constructor

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `engine` | `any` | `undefined` | the engine |
| `data` | [`Buffer`](Buffer.md) \| [`DataArray`](../modules.md#dataarray) \| [`DataBuffer`](DataBuffer.md) | `undefined` | the data to use for this vertex buffer |
| `kind` | `string` | `undefined` | the vertex buffer kind |
| `updatable` | `boolean` | `undefined` | whether the data is updatable |
| `postponeInternalCreation?` | `boolean` | `undefined` | whether to postpone creating the internal WebGL buffer (optional) |
| `stride?` | `number` | `undefined` | the stride (optional) |
| `instanced?` | `boolean` | `undefined` | whether the buffer is instanced (optional) |
| `offset?` | `number` | `undefined` | the offset of the data (optional) |
| `size?` | `number` | `undefined` | the number of components (optional) |
| `type?` | `number` | `undefined` | the type of the component (optional) |
| `normalized` | `boolean` | `false` | whether the data contains normalized data (optional) |
| `useBytes` | `boolean` | `false` | set to true if stride and offset are in bytes (optional) |
| `divisor` | `number` | `1` | defines the instance divisor to use (1 by default) |
| `takeBufferOwnership` | `boolean` | `false` | defines if the buffer should be released when the vertex buffer is disposed |

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:360

## Properties

### \_instanceDivisor

• `Private` **\_instanceDivisor**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:258

___

### \_instanced

• `Private` **\_instanced**: `boolean`

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:257

___

### \_kind

• `Private` **\_kind**: `string`

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:254

___

### \_ownsBuffer

• `Private` **\_ownsBuffer**: `boolean`

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:256

___

### \_size

• `Private` **\_size**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:255

___

### byteOffset

• `Readonly` **byteOffset**: `number`

Gets the byte offset.

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:320

___

### byteStride

• `Readonly` **byteStride**: `number`

Gets the byte stride.

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:315

___

### hashCode

• `Readonly` **hashCode**: `number`

Gets a hash code representing the format (type, normalized, size, instanced, stride) of this buffer
All buffers with the same format will have the same hash code

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:341

___

### normalized

• `Readonly` **normalized**: `boolean`

Gets whether integer data values should be normalized into a certain range when being casted to a float.

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:325

___

### type

• `Readonly` **type**: `number`

Gets the data type of each component in the array.

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:330

___

### uniqueId

• `Readonly` **uniqueId**: `number`

Gets the unique id of this vertex buffer

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:335

___

### BYTE

▪ `Static` `Readonly` **BYTE**: ``5120``

The byte type.

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:263

___

### ColorInstanceKind

▪ `Static` `Readonly` **ColorInstanceKind**: ``"instanceColor"``

Instance Colors

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:673

___

### ColorKind

▪ `Static` `Readonly` **ColorKind**: ``"color"``

Colors

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:669

___

### FLOAT

▪ `Static` `Readonly` **FLOAT**: ``5126``

The float type.

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:293

___

### INT

▪ `Static` `Readonly` **INT**: ``5124``

The integer type.

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:283

___

### MatricesIndicesExtraKind

▪ `Static` `Readonly` **MatricesIndicesExtraKind**: ``"matricesIndicesExtra"``

Additional matrix indices (for bones)

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:685

___

### MatricesIndicesKind

▪ `Static` `Readonly` **MatricesIndicesKind**: ``"matricesIndices"``

Matrix indices (for bones)

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:677

___

### MatricesWeightsExtraKind

▪ `Static` `Readonly` **MatricesWeightsExtraKind**: ``"matricesWeightsExtra"``

Additional matrix weights (for bones)

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:689

___

### MatricesWeightsKind

▪ `Static` `Readonly` **MatricesWeightsKind**: ``"matricesWeights"``

Matrix weights (for bones)

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:681

___

### NormalKind

▪ `Static` `Readonly` **NormalKind**: ``"normal"``

Normals

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:637

___

### PositionKind

▪ `Static` `Readonly` **PositionKind**: ``"position"``

Positions

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:633

___

### SHORT

▪ `Static` `Readonly` **SHORT**: ``5122``

The short type.

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:273

___

### TangentKind

▪ `Static` `Readonly` **TangentKind**: ``"tangent"``

Tangents

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:641

___

### UNSIGNED\_BYTE

▪ `Static` `Readonly` **UNSIGNED\_BYTE**: ``5121``

The unsigned byte type.

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:268

___

### UNSIGNED\_INT

▪ `Static` `Readonly` **UNSIGNED\_INT**: ``5125``

The unsigned integer type.

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:288

___

### UNSIGNED\_SHORT

▪ `Static` `Readonly` **UNSIGNED\_SHORT**: ``5123``

The unsigned short type.

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:278

___

### UV2Kind

▪ `Static` `Readonly` **UV2Kind**: ``"uv2"``

Texture coordinates 2

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:649

___

### UV3Kind

▪ `Static` `Readonly` **UV3Kind**: ``"uv3"``

Texture coordinates 3

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:653

___

### UV4Kind

▪ `Static` `Readonly` **UV4Kind**: ``"uv4"``

Texture coordinates 4

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:657

___

### UV5Kind

▪ `Static` `Readonly` **UV5Kind**: ``"uv5"``

Texture coordinates 5

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:661

___

### UV6Kind

▪ `Static` `Readonly` **UV6Kind**: ``"uv6"``

Texture coordinates 6

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:665

___

### UVKind

▪ `Static` `Readonly` **UVKind**: ``"uv"``

Texture coordinates

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:645

___

### \_Counter

▪ `Static` `Private` **\_Counter**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:248

## Accessors

### instanceDivisor

• `get` **instanceDivisor**(): `number`

Gets or sets the instance divisor when in instanced mode

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:298

• `set` **instanceDivisor**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:302

## Methods

### \_computeHashCode

▸ `Private` **_computeHashCode**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:427

___

### create

▸ **create**(`data?`): `void`

Store data into the buffer. If the buffer was already used it will be either recreated or updated depending on isUpdatable property

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data?` | [`DataArray`](../modules.md#dataarray) | defines the data to store |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:587

___

### dispose

▸ **dispose**(): `void`

Disposes the VertexBuffer and the underlying WebGLBuffer.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:614

___

### forEach

▸ **forEach**(`count`, `callback`): `void`

Enumerates each value of this vertex buffer as numbers.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `count` | `number` | the number of values to enumerate |
| `callback` | (`value`: `number`, `index`: `number`) => `void` | the callback function called for each value |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:625

___

### getBuffer

▸ **getBuffer**(): [`Nullable`](../modules.md#nullable)[`DataBuffer`](DataBuffer.md)

Gets underlying native buffer

#### Returns

[`Nullable`](../modules.md#nullable)[`DataBuffer`](DataBuffer.md)

underlying native buffer

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:533

___

### getData

▸ **getData**(): [`Nullable`](../modules.md#nullable)[`DataArray`](../modules.md#dataarray)

Gets current buffer's data

#### Returns

[`Nullable`](../modules.md#nullable)[`DataArray`](../modules.md#dataarray)

a DataArray or null

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:469

___

### getFloatData

▸ **getFloatData**(`totalVertices`, `forceCopy?`): [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray)

Gets current buffer's data as a float array. Float data is constructed if the vertex buffer data cannot be returned directly.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `totalVertices` | `number` | number of vertices in the buffer to take into account |
| `forceCopy?` | `boolean` | defines a boolean indicating that the returned array must be cloned upon returning it |

#### Returns

[`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray)

a float array containing vertex data

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:479

___

### getInstanceDivisor

▸ **getInstanceDivisor**(): `number`

Returns the instancing divisor, zero for non-instanced (integer).

#### Returns

`number`

a number

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:577

___

### getIsInstanced

▸ **getIsInstanced**(): `boolean`

Gets a boolean indicating is the internal buffer of the VertexBuffer is instanced

#### Returns

`boolean`

true if this buffer is instanced

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:569

___

### getKind

▸ **getKind**(): `string`

Returns the kind of the VertexBuffer (string)

#### Returns

`string`

a string

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:451

___

### getOffset

▸ **getOffset**(): `number`

Returns the offset as a multiple of the type byte length.

**`Deprecated`**

Please use byteOffset instead.

#### Returns

`number`

the offset in bytes

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:552

___

### getSize

▸ **getSize**(`sizeInBytes?`): `number`

Returns the number of components or the byte size per vertex attribute

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `sizeInBytes` | `boolean` | `false` | If true, returns the size in bytes or else the size in number of components of the vertex attribute (default: false) |

#### Returns

`number`

the number of components

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:561

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

https://github.com/babylon.js/core/src/Buffers/buffer.ts:543

___

### isUpdatable

▸ **isUpdatable**(): `boolean`

Gets a boolean indicating if the VertexBuffer is updatable?

#### Returns

`boolean`

true if the buffer is updatable

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:461

___

### update

▸ **update**(`data`): `void`

Updates the underlying buffer according to the passed numeric array or Float32Array.
This function will create a new buffer if the current one is not updatable

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | [`DataArray`](../modules.md#dataarray) | defines the data to store |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:596

___

### updateDirectly

▸ **updateDirectly**(`data`, `offset`, `useBytes?`): `void`

Updates directly the underlying WebGLBuffer according to the passed numeric array or Float32Array.
Returns the directly updated WebGLBuffer.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `data` | [`DataArray`](../modules.md#dataarray) | `undefined` | the new data |
| `offset` | `number` | `undefined` | the new offset |
| `useBytes` | `boolean` | `false` | set to true if the offset is in bytes |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:607

___

### DeduceStride

▸ `Static` **DeduceStride**(`kind`): `number`

Deduces the stride given a kind.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `kind` | `string` | The kind string to deduce |

#### Returns

`number`

The deduced stride

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:696

___

### ForEach

▸ `Static` **ForEach**(`data`, `byteOffset`, `byteStride`, `componentCount`, `componentType`, `count`, `normalized`, `callback`): `void`

Enumerates each value of the given parameters as numbers.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | [`DataArray`](../modules.md#dataarray) | the data to enumerate |
| `byteOffset` | `number` | the byte offset of the data |
| `byteStride` | `number` | the byte stride of the data |
| `componentCount` | `number` | the number of components per element |
| `componentType` | `number` | the type of the component |
| `count` | `number` | the number of values to enumerate |
| `normalized` | `boolean` | whether the data is normalized |
| `callback` | (`value`: `number`, `index`: `number`) => `void` | the callback function called for each value |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:753

___

### GetTypeByteLength

▸ `Static` **GetTypeByteLength**(`type`): `number`

Gets the byte length of the given type.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | `number` | the type |

#### Returns

`number`

the number of bytes

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:725

___

### \_GetFloatValue

▸ `Static` `Private` **_GetFloatValue**(`dataView`, `type`, `byteOffset`, `normalized`): `number`

#### Parameters

| Name | Type |
| :------ | :------ |
| `dataView` | `DataView` |
| `type` | `number` |
| `byteOffset` | `number` |
| `normalized` | `boolean` |

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Buffers/buffer.ts:787
