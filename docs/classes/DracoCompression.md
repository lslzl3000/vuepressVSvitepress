[@dev/core](../README.md) / [Exports](../modules.md) / DracoCompression

# Class: DracoCompression

Draco compression (https://google.github.io/draco/)

This class wraps the Draco module.

**Encoder**

The encoder is not currently implemented.

**Decoder**

By default, the configuration points to a copy of the Draco decoder files for glTF from the babylon.js preview cdn https://preview.babylonjs.com/draco_wasm_wrapper_gltf.js.

To update the configuration, use the following code:
```javascript
    DracoCompression.Configuration = {
        decoder: {
            wasmUrl: "url to the WebAssembly library>",
            wasmBinaryUrl: "url to the WebAssembly binary>",
            fallbackUrl: "url to the fallback JavaScript library>",
        }
    };
```

Draco has two versions, one for WebAssembly and one for JavaScript. The decoder configuration can be set to only support WebAssembly or only support the JavaScript version.
Decoding will automatically fallback to the JavaScript version if WebAssembly version is not configured or if WebAssembly is not supported by the browser.
Use `DracoCompression.DecoderAvailable` to determine if the decoder configuration is available for the current context.

To decode Draco compressed data, get the default DracoCompression object and call decodeMeshAsync:
```javascript
    var vertexData = await DracoCompression.Default.decodeMeshAsync(data);
```

**`See`**

https://playground.babylonjs.com/#DMZIBD#0

## Implements

- [`IDisposable`](../interfaces/IDisposable.md)

## Table of contents

### Constructors

- [constructor](DracoCompression.md#constructor)

### Properties

- [\_decoderModulePromise](DracoCompression.md#_decodermodulepromise)
- [\_workerPoolPromise](DracoCompression.md#_workerpoolpromise)
- [Configuration](DracoCompression.md#configuration)
- [DefaultNumWorkers](DracoCompression.md#defaultnumworkers)
- [\_Default](DracoCompression.md#_default)

### Accessors

- [DecoderAvailable](DracoCompression.md#decoderavailable)
- [Default](DracoCompression.md#default)

### Methods

- [decodeMeshAsync](DracoCompression.md#decodemeshasync)
- [dispose](DracoCompression.md#dispose)
- [whenReadyAsync](DracoCompression.md#whenreadyasync)
- [GetDefaultNumWorkers](DracoCompression.md#getdefaultnumworkers)

## Constructors

### constructor

• **new DracoCompression**(`numWorkers?`)

Constructor

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `numWorkers` | `number` | `DracoCompression.DefaultNumWorkers` | The number of workers for async operations. Specify `0` to disable web workers and run synchronously in the current context. |

#### Defined in

packages/dev/core/src/Meshes/Compression/dracoCompression.ts:299

## Properties

### \_decoderModulePromise

• `Private` `Optional` **\_decoderModulePromise**: `Promise``any`

#### Defined in

packages/dev/core/src/Meshes/Compression/dracoCompression.ts:244

___

### \_workerPoolPromise

• `Private` `Optional` **\_workerPoolPromise**: `Promise`[`AutoReleaseWorkerPool`](AutoReleaseWorkerPool.md)

#### Defined in

packages/dev/core/src/Meshes/Compression/dracoCompression.ts:243

___

### Configuration

▪ `Static` **Configuration**: [`IDracoCompressionConfiguration`](../interfaces/IDracoCompressionConfiguration.md)

The configuration. Defaults to the following urls:
- wasmUrl: "https://preview.babylonjs.com/draco_wasm_wrapper_gltf.js"
- wasmBinaryUrl: "https://preview.babylonjs.com/draco_decoder_gltf.wasm"
- fallbackUrl: "https://preview.babylonjs.com/draco_decoder_gltf.js"

#### Defined in

packages/dev/core/src/Meshes/Compression/dracoCompression.ts:252

___

### DefaultNumWorkers

▪ `Static` **DefaultNumWorkers**: `number`

Default number of workers to create when creating the draco compression object.

#### Defined in

packages/dev/core/src/Meshes/Compression/dracoCompression.ts:271

___

### \_Default

▪ `Static` `Private` **\_Default**: [`Nullable`](../modules.md#nullable)[`DracoCompression`](DracoCompression.md) = `null`

#### Defined in

packages/dev/core/src/Meshes/Compression/dracoCompression.ts:282

## Accessors

### DecoderAvailable

• `Static` `get` **DecoderAvailable**(): `boolean`

Returns true if the decoder configuration is available.

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Meshes/Compression/dracoCompression.ts:263

___

### Default

• `Static` `get` **Default**(): [`DracoCompression`](DracoCompression.md)

Default instance for the draco compression object.

#### Returns

[`DracoCompression`](DracoCompression.md)

#### Defined in

packages/dev/core/src/Meshes/Compression/dracoCompression.ts:287

## Methods

### decodeMeshAsync

▸ **decodeMeshAsync**(`data`, `attributes?`, `dividers?`): `Promise`[`VertexData`](VertexData.md)

Decode Draco compressed mesh data to vertex data.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `ArrayBuffer` \| `ArrayBufferView` | The ArrayBuffer or ArrayBufferView for the Draco compression data |
| `attributes?` | `Object` | A map of attributes from vertex buffer kinds to Draco unique ids |
| `dividers?` | `Object` | a list of optional dividers for normalization |

#### Returns

`Promise`[`VertexData`](VertexData.md)

A promise that resolves with the decoded vertex data

#### Defined in

packages/dev/core/src/Meshes/Compression/dracoCompression.ts:398

___

### dispose

▸ **dispose**(): `void`

Stop all async operations and release resources.

#### Returns

`void`

#### Implementation of

[IDisposable](../interfaces/IDisposable.md).[dispose](../interfaces/IDisposable.md#dispose)

#### Defined in

packages/dev/core/src/Meshes/Compression/dracoCompression.ts:364

___

### whenReadyAsync

▸ **whenReadyAsync**(): `Promise``void`

Returns a promise that resolves when ready. Call this manually to ensure draco compression is ready before use.

#### Returns

`Promise``void`

a promise that resolves when ready

#### Defined in

packages/dev/core/src/Meshes/Compression/dracoCompression.ts:379

___

### GetDefaultNumWorkers

▸ `Static` `Private` **GetDefaultNumWorkers**(): `number`

#### Returns

`number`

#### Defined in

packages/dev/core/src/Meshes/Compression/dracoCompression.ts:273
