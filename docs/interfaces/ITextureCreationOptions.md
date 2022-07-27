[@dev/core](../README.md) / [Exports](../modules.md) / ITextureCreationOptions

# Interface: ITextureCreationOptions

Defines the available options when creating a texture

## Table of contents

### Properties

- [buffer](ITextureCreationOptions.md#buffer)
- [creationFlags](ITextureCreationOptions.md#creationflags)
- [deleteBuffer](ITextureCreationOptions.md#deletebuffer)
- [format](ITextureCreationOptions.md#format)
- [internalTexture](ITextureCreationOptions.md#internaltexture)
- [invertY](ITextureCreationOptions.md#inverty)
- [loaderOptions](ITextureCreationOptions.md#loaderoptions)
- [mimeType](ITextureCreationOptions.md#mimetype)
- [noMipmap](ITextureCreationOptions.md#nomipmap)
- [onError](ITextureCreationOptions.md#onerror)
- [onLoad](ITextureCreationOptions.md#onload)
- [samplingMode](ITextureCreationOptions.md#samplingmode)
- [useSRGBBuffer](ITextureCreationOptions.md#usesrgbbuffer)

## Properties

### buffer

• `Optional` **buffer**: [`Nullable`](../modules.md#nullable)`string` \| `ArrayBuffer` \| `ArrayBufferView` \| `Blob` \| `HTMLImageElement` \| `ImageBitmap`

Defines the buffer to load the texture from in case the texture is loaded from a buffer representation (default: null)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:44

___

### creationFlags

• `Optional` **creationFlags**: `number`

Specific flags to use when creating the texture (Constants.TEXTURE_CREATIONFLAG_STORAGE for storage textures, for eg) (default: undefined)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:59

___

### deleteBuffer

• `Optional` **deleteBuffer**: `boolean`

Defines if the buffer we are loading the texture from should be deleted after load (default: false)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:47

___

### format

• `Optional` **format**: `number`

Defines the format of the texture we are trying to load (Engine.TEXTUREFORMAT_RGBA...) (default: )

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:50

___

### internalTexture

• `Optional` **internalTexture**: [`InternalTexture`](../classes/InternalTexture.md)

Defines the underlying texture from an already existing one

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:65

___

### invertY

• `Optional` **invertY**: `boolean`

Defines if the texture needs to be inverted on the y axis during loading (default: true)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:32

___

### loaderOptions

• `Optional` **loaderOptions**: `any`

Options to be passed to the loader (default: undefined)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:56

___

### mimeType

• `Optional` **mimeType**: `string`

Defines an optional mime type information (default: undefined)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:53

___

### noMipmap

• `Optional` **noMipmap**: `boolean`

Defines if the texture will require mip maps or not (default: false)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:29

___

### onError

• `Optional` **onError**: [`Nullable`](../modules.md#nullable)(`message?`: `string`, `exception?`: `any`) => `void`

Defines a callback triggered when an error occurred during the loading session (default: null)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:41

___

### onLoad

• `Optional` **onLoad**: [`Nullable`](../modules.md#nullable)() => `void`

Defines a callback triggered when the texture has been loaded (default: null)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:38

___

### samplingMode

• `Optional` **samplingMode**: `number`

Defines the sampling mode we want for the texture while fetching from it (Texture.NEAREST_SAMPLINGMODE...) (default: Texture.TRILINEAR_SAMPLINGMODE)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:35

___

### useSRGBBuffer

• `Optional` **useSRGBBuffer**: `boolean`

Defines if the texture must be loaded in a sRGB GPU buffer (if supported by the GPU) (default: false)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/texture.ts:62
