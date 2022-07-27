[@dev/core](../README.md) / [Exports](../modules.md) / KhronosTextureContainer2

# Class: KhronosTextureContainer2

Class for loading KTX2 files

## Table of contents

### Constructors

- [constructor](KhronosTextureContainer2.md#constructor)

### Properties

- [\_engine](KhronosTextureContainer2.md#_engine)
- [DefaultNumWorkers](KhronosTextureContainer2.md#defaultnumworkers)
- [URLConfig](KhronosTextureContainer2.md#urlconfig)
- [\_DecoderModulePromise](KhronosTextureContainer2.md#_decodermodulepromise)
- [\_WorkerPoolPromise](KhronosTextureContainer2.md#_workerpoolpromise)

### Methods

- [\_createTexture](KhronosTextureContainer2.md#_createtexture)
- [GetDefaultNumWorkers](KhronosTextureContainer2.md#getdefaultnumworkers)
- [IsValid](KhronosTextureContainer2.md#isvalid)
- [\_Initialize](KhronosTextureContainer2.md#_initialize)

## Constructors

### constructor

• **new KhronosTextureContainer2**(`engine`, `numWorkers?`)

Constructor

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `engine` | [`ThinEngine`](ThinEngine.md) | `undefined` | The engine to use |
| `numWorkers` | `number` | `KhronosTextureContainer2.DefaultNumWorkers` | The number of workers for async operations. Specify `0` to disable web workers and run synchronously in the current context. |

#### Defined in

https://github.com/babylon.js/core/src/Misc/khronosTextureContainer2.ts:152

## Properties

### \_engine

• `Private` **\_engine**: [`ThinEngine`](ThinEngine.md)

#### Defined in

https://github.com/babylon.js/core/src/Misc/khronosTextureContainer2.ts:67

___

### DefaultNumWorkers

▪ `Static` **DefaultNumWorkers**: `number`

Default number of workers used to handle data decoding

#### Defined in

https://github.com/babylon.js/core/src/Misc/khronosTextureContainer2.ts:56

___

### URLConfig

▪ `Static` **URLConfig**: `Object`

URLs to use when loading the KTX2 decoder module as well as its dependencies
If a url is null, the default url is used (pointing to https://preview.babylonjs.com)
Note that jsDecoderModule can't be null and that the other dependencies will only be loaded if necessary
Urls you can change:
    URLConfig.jsDecoderModule
    URLConfig.wasmUASTCToASTC
    URLConfig.wasmUASTCToBC7
    URLConfig.wasmUASTCToRGBA_UNORM
    URLConfig.wasmUASTCToRGBA_SRGB
    URLConfig.jsMSCTranscoder
    URLConfig.wasmMSCTranscoder
    URLConfig.wasmZSTDDecoder
You can see their default values in this PG: https://playground.babylonjs.com/#EIJH8L#29

#### Type declaration

| Name | Type |
| :------ | :------ |
| `jsDecoderModule` | `string` |
| `jsMSCTranscoder` | [`Nullable`](../modules.md#nullable)`string` |
| `wasmMSCTranscoder` | [`Nullable`](../modules.md#nullable)`string` |
| `wasmUASTCToASTC` | [`Nullable`](../modules.md#nullable)`string` |
| `wasmUASTCToBC7` | [`Nullable`](../modules.md#nullable)`string` |
| `wasmUASTCToRGBA_SRGB` | [`Nullable`](../modules.md#nullable)`string` |
| `wasmUASTCToRGBA_UNORM` | [`Nullable`](../modules.md#nullable)`string` |
| `wasmZSTDDecoder` | [`Nullable`](../modules.md#nullable)`string` |

#### Defined in

https://github.com/babylon.js/core/src/Misc/khronosTextureContainer2.ts:33

___

### \_DecoderModulePromise

▪ `Static` `Private` `Optional` **\_DecoderModulePromise**: `Promise``any`

#### Defined in

https://github.com/babylon.js/core/src/Misc/khronosTextureContainer2.ts:16

___

### \_WorkerPoolPromise

▪ `Static` `Private` `Optional` **\_WorkerPoolPromise**: `Promise`[`AutoReleaseWorkerPool`](AutoReleaseWorkerPool.md)

#### Defined in

https://github.com/babylon.js/core/src/Misc/khronosTextureContainer2.ts:15

## Methods

### \_createTexture

▸ `Protected` **_createTexture**(`data`, `internalTexture`, `options?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `data` | `any` |
| `internalTexture` | [`InternalTexture`](InternalTexture.md) |
| `options?` | `any` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/khronosTextureContainer2.ts:234

___

### GetDefaultNumWorkers

▸ `Static` `Private` **GetDefaultNumWorkers**(): `number`

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Misc/khronosTextureContainer2.ts:58

___

### IsValid

▸ `Static` **IsValid**(`data`): `boolean`

Checks if the given data starts with a KTX2 file identifier.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `ArrayBufferView` | the data to check |

#### Returns

`boolean`

true if the data is a KTX2 file or false otherwise

#### Defined in

https://github.com/babylon.js/core/src/Misc/khronosTextureContainer2.ts:292

___

### \_Initialize

▸ `Static` `Private` **_Initialize**(`numWorkers`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `numWorkers` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/khronosTextureContainer2.ts:69
