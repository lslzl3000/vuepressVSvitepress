[@dev/core](../README.md) / [Exports](../modules.md) / MeshoptCompression

# Class: MeshoptCompression

Meshopt compression (https://github.com/zeux/meshoptimizer)

This class wraps the meshopt library from https://github.com/zeux/meshoptimizer/tree/master/js.

**Encoder**

The encoder is not currently implemented.

**Decoder**

By default, the configuration points to a copy of the meshopt files on the Babylon.js preview CDN (e.g. https://preview.babylonjs.com/meshopt_decoder.js).

To update the configuration, use the following code:
```javascript
    MeshoptCompression.Configuration = {
        decoder: {
            url: "url to the meshopt decoder library>"
        }
    };
```

## Implements

- [`IDisposable`](../interfaces/IDisposable.md)

## Table of contents

### Constructors

- [constructor](MeshoptCompression.md#constructor)

### Properties

- [\_decoderModulePromise](MeshoptCompression.md#_decodermodulepromise)
- [Configuration](MeshoptCompression.md#configuration)
- [\_Default](MeshoptCompression.md#_default)

### Accessors

- [Default](MeshoptCompression.md#default)

### Methods

- [decodeGltfBufferAsync](MeshoptCompression.md#decodegltfbufferasync)
- [dispose](MeshoptCompression.md#dispose)

## Constructors

### constructor

• **new MeshoptCompression**()

Constructor

#### Defined in

packages/dev/core/src/Meshes/Compression/meshoptCompression.ts:78

## Properties

### \_decoderModulePromise

• `Private` `Optional` **\_decoderModulePromise**: `Promise``any`

#### Defined in

packages/dev/core/src/Meshes/Compression/meshoptCompression.ts:46

___

### Configuration

▪ `Static` **Configuration**: [`IMeshoptCompressionConfiguration`](../interfaces/IMeshoptCompressionConfiguration.md)

The configuration. Defaults to the following:
```javascript
decoder: {
  url: "https://preview.babylonjs.com/meshopt_decoder.js"
}
```

#### Defined in

packages/dev/core/src/Meshes/Compression/meshoptCompression.ts:56

___

### \_Default

▪ `Static` `Private` **\_Default**: [`Nullable`](../modules.md#nullable)[`MeshoptCompression`](MeshoptCompression.md) = `null`

#### Defined in

packages/dev/core/src/Meshes/Compression/meshoptCompression.ts:62

## Accessors

### Default

• `Static` `get` **Default**(): [`MeshoptCompression`](MeshoptCompression.md)

Default instance for the meshoptimizer object.

#### Returns

[`MeshoptCompression`](MeshoptCompression.md)

#### Defined in

packages/dev/core/src/Meshes/Compression/meshoptCompression.ts:67

## Methods

### decodeGltfBufferAsync

▸ **decodeGltfBufferAsync**(`source`, `count`, `stride`, `mode`, `filter?`): `Promise``Uint8Array`

Decode meshopt data.

**`See`**

https://github.com/zeux/meshoptimizer/tree/master/js#decoder

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | `Uint8Array` | The input data. |
| `count` | `number` | The number of elements. |
| `stride` | `number` | The stride in bytes. |
| `mode` | ``"ATTRIBUTES"`` \| ``"TRIANGLES"`` \| ``"INDICES"`` | The compression mode. |
| `filter?` | `string` | The compression filter. |

#### Returns

`Promise``Uint8Array`

a Promise that resolves to the decoded data

#### Defined in

packages/dev/core/src/Meshes/Compression/meshoptCompression.ts:104

___

### dispose

▸ **dispose**(): `void`

Stop all async operations and release resources.

#### Returns

`void`

#### Implementation of

[IDisposable](../interfaces/IDisposable.md).[dispose](../interfaces/IDisposable.md#dispose)

#### Defined in

packages/dev/core/src/Meshes/Compression/meshoptCompression.ts:90
