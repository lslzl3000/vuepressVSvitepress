[@dev/core](../README.md) / [Exports](../modules.md) / \_BasisTextureLoader

# Class: \_BasisTextureLoader

Loader for .basis file format

## Implements

- [`IInternalTextureLoader`](../interfaces/IInternalTextureLoader.md)

## Table of contents

### Constructors

- [constructor](BasisTextureLoader.md#constructor)

### Properties

- [supportCascades](BasisTextureLoader.md#supportcascades)

### Methods

- [canLoad](BasisTextureLoader.md#canload)
- [loadCubeData](BasisTextureLoader.md#loadcubedata)
- [loadData](BasisTextureLoader.md#loaddata)

## Constructors

### constructor

• **new _BasisTextureLoader**()

## Properties

### supportCascades

• `Readonly` **supportCascades**: ``false``

Defines whether the loader supports cascade loading the different faces.

#### Implementation of

[IInternalTextureLoader](../interfaces/IInternalTextureLoader.md).[supportCascades](../interfaces/IInternalTextureLoader.md#supportcascades)

#### Defined in

packages/dev/core/src/Materials/Textures/Loaders/basisTextureLoader.ts:16

## Methods

### canLoad

▸ **canLoad**(`extension`): `boolean`

This returns if the loader support the current file information.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `extension` | `string` | defines the file extension of the file being loaded |

#### Returns

`boolean`

true if the loader can load the specified file

#### Implementation of

[IInternalTextureLoader](../interfaces/IInternalTextureLoader.md).[canLoad](../interfaces/IInternalTextureLoader.md#canload)

#### Defined in

packages/dev/core/src/Materials/Textures/Loaders/basisTextureLoader.ts:23

___

### loadCubeData

▸ **loadCubeData**(`data`, `texture`, `createPolynomials`, `onLoad`, `onError`): `void`

Uploads the cube texture data to the WebGL texture. It has already been bound.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `ArrayBufferView` \| `ArrayBufferView`[] | contains the texture data |
| `texture` | [`InternalTexture`](InternalTexture.md) | defines the BabylonJS internal texture |
| `createPolynomials` | `boolean` | will be true if polynomials have been requested |
| `onLoad` | [`Nullable`](../modules.md#nullable)(`data?`: `any`) => `void` | defines the callback to trigger once the texture is ready |
| `onError` | [`Nullable`](../modules.md#nullable)(`message?`: `string`, `exception?`: `any`) => `void` | defines the callback to trigger in case of error |

#### Returns

`void`

#### Implementation of

[IInternalTextureLoader](../interfaces/IInternalTextureLoader.md).[loadCubeData](../interfaces/IInternalTextureLoader.md#loadcubedata)

#### Defined in

packages/dev/core/src/Materials/Textures/Loaders/basisTextureLoader.ts:35

___

### loadData

▸ **loadData**(`data`, `texture`, `callback`): `void`

Uploads the 2D texture data to the WebGL texture. It has already been bound once in the callback.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `ArrayBufferView` | contains the texture data |
| `texture` | [`InternalTexture`](InternalTexture.md) | defines the BabylonJS internal texture |
| `callback` | (`width`: `number`, `height`: `number`, `loadMipmap`: `boolean`, `isCompressed`: `boolean`, `done`: () => `void`, `failedLoading?`: `boolean`) => `void` | defines the method to call once ready to upload |

#### Returns

`void`

#### Implementation of

[IInternalTextureLoader](../interfaces/IInternalTextureLoader.md).[loadData](../interfaces/IInternalTextureLoader.md#loaddata)

#### Defined in

packages/dev/core/src/Materials/Textures/Loaders/basisTextureLoader.ts:84
