[@dev/core](../README.md) / [Exports](../modules.md) / IInternalTextureLoader

# Interface: IInternalTextureLoader

This represents the required contract to create a new type of texture loader.

## Implemented by

- [`_BasisTextureLoader`](../classes/BasisTextureLoader.md)

## Table of contents

### Properties

- [supportCascades](IInternalTextureLoader.md#supportcascades)

### Methods

- [canLoad](IInternalTextureLoader.md#canload)
- [loadCubeData](IInternalTextureLoader.md#loadcubedata)
- [loadData](IInternalTextureLoader.md#loaddata)

## Properties

### supportCascades

• **supportCascades**: `boolean`

Defines whether the loader supports cascade loading the different faces.

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/internalTextureLoader.ts:11

## Methods

### canLoad

▸ **canLoad**(`extension`, `mimeType?`): `boolean`

This returns if the loader support the current file information.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `extension` | `string` | defines the file extension of the file being loaded |
| `mimeType?` | `string` | defines the optional mime type of the file being loaded |

#### Returns

`boolean`

true if the loader can load the specified file

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/internalTextureLoader.ts:19

___

### loadCubeData

▸ **loadCubeData**(`data`, `texture`, `createPolynomials`, `onLoad`, `onError`, `options?`): `void`

Uploads the cube texture data to the WebGL texture. It has already been bound.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `ArrayBufferView` \| `ArrayBufferView`[] | contains the texture data |
| `texture` | [`InternalTexture`](../classes/InternalTexture.md) | defines the BabylonJS internal texture |
| `createPolynomials` | `boolean` | will be true if polynomials have been requested |
| `onLoad` | [`Nullable`](../modules.md#nullable)(`data?`: `any`) => `void` | defines the callback to trigger once the texture is ready |
| `onError` | [`Nullable`](../modules.md#nullable)(`message?`: `string`, `exception?`: `any`) => `void` | defines the callback to trigger in case of error |
| `options?` | `any` | options to be passed to the loader |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/internalTextureLoader.ts:30

___

### loadData

▸ **loadData**(`data`, `texture`, `callback`, `options?`): `void`

Uploads the 2D texture data to the WebGL texture. It has already been bound once in the callback.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `ArrayBufferView` | contains the texture data |
| `texture` | [`InternalTexture`](../classes/InternalTexture.md) | defines the BabylonJS internal texture |
| `callback` | (`width`: `number`, `height`: `number`, `loadMipmap`: `boolean`, `isCompressed`: `boolean`, `done`: () => `void`, `loadFailed?`: `boolean`) => `void` | defines the method to call once ready to upload |
| `options?` | `any` | options to be passed to the loader |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/internalTextureLoader.ts:46
