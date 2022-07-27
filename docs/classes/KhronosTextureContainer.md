[@dev/core](../README.md) / [Exports](../modules.md) / KhronosTextureContainer

# Class: KhronosTextureContainer

for description see https://www.khronos.org/opengles/sdk/tools/KTX/
for file layout see https://www.khronos.org/opengles/sdk/tools/KTX/file_format_spec/

## Table of contents

### Constructors

- [constructor](KhronosTextureContainer.md#constructor)

### Properties

- [bytesOfKeyValueData](KhronosTextureContainer.md#bytesofkeyvaluedata)
- [data](KhronosTextureContainer.md#data)
- [glBaseInternalFormat](KhronosTextureContainer.md#glbaseinternalformat)
- [glFormat](KhronosTextureContainer.md#glformat)
- [glInternalFormat](KhronosTextureContainer.md#glinternalformat)
- [glType](KhronosTextureContainer.md#gltype)
- [glTypeSize](KhronosTextureContainer.md#gltypesize)
- [isInvalid](KhronosTextureContainer.md#isinvalid)
- [loadType](KhronosTextureContainer.md#loadtype)
- [numberOfArrayElements](KhronosTextureContainer.md#numberofarrayelements)
- [numberOfFaces](KhronosTextureContainer.md#numberoffaces)
- [numberOfMipmapLevels](KhronosTextureContainer.md#numberofmipmaplevels)
- [pixelDepth](KhronosTextureContainer.md#pixeldepth)
- [pixelHeight](KhronosTextureContainer.md#pixelheight)
- [pixelWidth](KhronosTextureContainer.md#pixelwidth)
- [COMPRESSED\_2D](KhronosTextureContainer.md#compressed_2d)
- [COMPRESSED\_3D](KhronosTextureContainer.md#compressed_3d)
- [HEADER\_LEN](KhronosTextureContainer.md#header_len)
- [TEX\_2D](KhronosTextureContainer.md#tex_2d)
- [TEX\_3D](KhronosTextureContainer.md#tex_3d)

### Methods

- [\_upload2DCompressedLevels](KhronosTextureContainer.md#_upload2dcompressedlevels)
- [IsValid](KhronosTextureContainer.md#isvalid)

## Constructors

### constructor

• **new KhronosTextureContainer**(`data`, `facesExpected`)

Creates a new KhronosTextureContainer

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `ArrayBufferView` | contents of the KTX container file |
| `facesExpected` | `number` | should be either 1 or 6, based whether a cube texture or or |

#### Defined in

https://github.com/babylon.js/core/src/Misc/khronosTextureContainer.ts:81

## Properties

### bytesOfKeyValueData

• **bytesOfKeyValueData**: `number`

Gets the bytes of key value data

#### Defined in

https://github.com/babylon.js/core/src/Misc/khronosTextureContainer.ts:66

___

### data

• **data**: `ArrayBufferView`

#### Defined in

https://github.com/babylon.js/core/src/Misc/khronosTextureContainer.ts:83

___

### glBaseInternalFormat

• **glBaseInternalFormat**: `number`

Gets the base internal format

#### Defined in

https://github.com/babylon.js/core/src/Misc/khronosTextureContainer.ts:38

___

### glFormat

• **glFormat**: `number`

Gets the openGL format

#### Defined in

https://github.com/babylon.js/core/src/Misc/khronosTextureContainer.ts:30

___

### glInternalFormat

• **glInternalFormat**: `number`

Gets the openGL internal format

#### Defined in

https://github.com/babylon.js/core/src/Misc/khronosTextureContainer.ts:34

___

### glType

• **glType**: `number`

Gets the openGL type

#### Defined in

https://github.com/babylon.js/core/src/Misc/khronosTextureContainer.ts:22

___

### glTypeSize

• **glTypeSize**: `number`

Gets the openGL type size

#### Defined in

https://github.com/babylon.js/core/src/Misc/khronosTextureContainer.ts:26

___

### isInvalid

• **isInvalid**: `boolean` = `false`

If the container has been made invalid (eg. constructor failed to correctly load array buffer)

#### Defined in

https://github.com/babylon.js/core/src/Misc/khronosTextureContainer.ts:74

___

### loadType

• **loadType**: `number`

Gets the load type

#### Defined in

https://github.com/babylon.js/core/src/Misc/khronosTextureContainer.ts:70

___

### numberOfArrayElements

• **numberOfArrayElements**: `number`

Gets the number of array elements

#### Defined in

https://github.com/babylon.js/core/src/Misc/khronosTextureContainer.ts:54

___

### numberOfFaces

• **numberOfFaces**: `number`

Gets the number of faces

#### Defined in

https://github.com/babylon.js/core/src/Misc/khronosTextureContainer.ts:58

___

### numberOfMipmapLevels

• **numberOfMipmapLevels**: `number`

Gets the number of mipmap levels

#### Defined in

https://github.com/babylon.js/core/src/Misc/khronosTextureContainer.ts:62

___

### pixelDepth

• **pixelDepth**: `number`

Gets image depth in pixels

#### Defined in

https://github.com/babylon.js/core/src/Misc/khronosTextureContainer.ts:50

___

### pixelHeight

• **pixelHeight**: `number`

Gets image height in pixel

#### Defined in

https://github.com/babylon.js/core/src/Misc/khronosTextureContainer.ts:46

___

### pixelWidth

• **pixelWidth**: `number`

Gets image width in pixel

#### Defined in

https://github.com/babylon.js/core/src/Misc/khronosTextureContainer.ts:42

___

### COMPRESSED\_2D

▪ `Static` `Private` **COMPRESSED\_2D**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Misc/khronosTextureContainer.ts:13

___

### COMPRESSED\_3D

▪ `Static` `Private` **COMPRESSED\_3D**: `number` = `1`

#### Defined in

https://github.com/babylon.js/core/src/Misc/khronosTextureContainer.ts:14

___

### HEADER\_LEN

▪ `Static` `Private` **HEADER\_LEN**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Misc/khronosTextureContainer.ts:10

___

### TEX\_2D

▪ `Static` `Private` **TEX\_2D**: `number` = `2`

#### Defined in

https://github.com/babylon.js/core/src/Misc/khronosTextureContainer.ts:15

___

### TEX\_3D

▪ `Static` `Private` **TEX\_3D**: `number` = `3`

#### Defined in

https://github.com/babylon.js/core/src/Misc/khronosTextureContainer.ts:16

## Methods

### \_upload2DCompressedLevels

▸ `Private` **_upload2DCompressedLevels**(`texture`, `loadMipmaps`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `texture` | [`InternalTexture`](InternalTexture.md) |
| `loadMipmaps` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/khronosTextureContainer.ts:159

___

### IsValid

▸ `Static` **IsValid**(`data`): `boolean`

Checks if the given data starts with a KTX file identifier.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `ArrayBufferView` | the data to check |

#### Returns

`boolean`

true if the data is a KTX file or false otherwise

#### Defined in

https://github.com/babylon.js/core/src/Misc/khronosTextureContainer.ts:188
