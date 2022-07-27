[@dev/core](../README.md) / [Exports](../modules.md) / ExternalTexture

# Class: ExternalTexture

Class used to store an external texture (like GPUExternalTexture in WebGPU)

## Table of contents

### Constructors

- [constructor](ExternalTexture.md#constructor)

### Properties

- [\_video](ExternalTexture.md#_video)
- [type](ExternalTexture.md#type)
- [uniqueId](ExternalTexture.md#uniqueid)
- [useMipMaps](ExternalTexture.md#usemipmaps)

### Accessors

- [underlyingResource](ExternalTexture.md#underlyingresource)

### Methods

- [dispose](ExternalTexture.md#dispose)
- [getClassName](ExternalTexture.md#getclassname)
- [isReady](ExternalTexture.md#isready)
- [IsExternalTexture](ExternalTexture.md#isexternaltexture)

## Constructors

### constructor

• **new ExternalTexture**(`video`)

Constructs the texture

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `video` | `HTMLVideoElement` | The video the texture should be wrapped around |

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/externalTexture.ts:53

## Properties

### \_video

• `Private` **\_video**: `HTMLVideoElement`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/externalTexture.ts:17

___

### type

• `Readonly` **type**: ``16``

The type of the underlying texture is implementation dependent, so return "UNDEFINED" for the type

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/externalTexture.ts:42

___

### uniqueId

• `Readonly` **uniqueId**: `number`

Gets the unique id of this texture

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/externalTexture.ts:47

___

### useMipMaps

• **useMipMaps**: `boolean` = `false`

Gets a boolean indicating if the texture uses mipmaps

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/externalTexture.ts:37

## Accessors

### underlyingResource

• `get` **underlyingResource**(): `any`

Gets the underlying texture object

#### Returns

`any`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/externalTexture.ts:30

## Methods

### dispose

▸ **dispose**(): `void`

Dispose the texture and release its associated resources.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/externalTexture.ts:69

___

### getClassName

▸ **getClassName**(): `string`

Get the class name of the texture.

#### Returns

`string`

"ExternalTexture"

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/externalTexture.ts:23

___

### isReady

▸ **isReady**(): `boolean`

Get if the texture is ready to be used (downloaded, converted, mip mapped...).

#### Returns

`boolean`

true if fully ready

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/externalTexture.ts:62

___

### IsExternalTexture

▸ `Static` **IsExternalTexture**(`texture`): texture is ExternalTexture

Checks if a texture is an external or internal texture

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `texture` | [`InternalTexture`](InternalTexture.md) \| [`ExternalTexture`](ExternalTexture.md) | the external or internal texture |

#### Returns

texture is ExternalTexture

true if the texture is an external texture, else false

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/externalTexture.ts:13
