[@dev/core](../README.md) / [Exports](../modules.md) / IMultiRenderTargetOptions

# Interface: IMultiRenderTargetOptions

Creation options of the multi render target texture.

## Table of contents

### Properties

- [defaultType](IMultiRenderTargetOptions.md#defaulttype)
- [depthTextureFormat](IMultiRenderTargetOptions.md#depthtextureformat)
- [doNotChangeAspectRatio](IMultiRenderTargetOptions.md#donotchangeaspectratio)
- [drawOnlyOnFirstAttachmentByDefault](IMultiRenderTargetOptions.md#drawonlyonfirstattachmentbydefault)
- [generateDepthBuffer](IMultiRenderTargetOptions.md#generatedepthbuffer)
- [generateDepthTexture](IMultiRenderTargetOptions.md#generatedepthtexture)
- [generateMipMaps](IMultiRenderTargetOptions.md#generatemipmaps)
- [generateStencilBuffer](IMultiRenderTargetOptions.md#generatestencilbuffer)
- [samplingModes](IMultiRenderTargetOptions.md#samplingmodes)
- [textureCount](IMultiRenderTargetOptions.md#texturecount)
- [types](IMultiRenderTargetOptions.md#types)
- [useSRGBBuffers](IMultiRenderTargetOptions.md#usesrgbbuffers)

## Properties

### defaultType

• `Optional` **defaultType**: `number`

Define the default type of the buffers we are creating

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/multiRenderTarget.ts:57

___

### depthTextureFormat

• `Optional` **depthTextureFormat**: `number`

Define depth texture format to use

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/multiRenderTarget.ts:45

___

### doNotChangeAspectRatio

• `Optional` **doNotChangeAspectRatio**: `boolean`

Define if aspect ratio should be adapted to the texture or stay the scene one

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/multiRenderTarget.ts:53

___

### drawOnlyOnFirstAttachmentByDefault

• `Optional` **drawOnlyOnFirstAttachmentByDefault**: `boolean`

Define the default type of the buffers we are creating

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/multiRenderTarget.ts:61

___

### generateDepthBuffer

• `Optional` **generateDepthBuffer**: `boolean`

Define if a depth buffer is required

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/multiRenderTarget.ts:33

___

### generateDepthTexture

• `Optional` **generateDepthTexture**: `boolean`

Define if a depth texture is required instead of a depth buffer

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/multiRenderTarget.ts:41

___

### generateMipMaps

• `Optional` **generateMipMaps**: `boolean`

Define if the texture needs to create mip maps after render.

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/multiRenderTarget.ts:17

___

### generateStencilBuffer

• `Optional` **generateStencilBuffer**: `boolean`

Define if a stencil buffer is required

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/multiRenderTarget.ts:37

___

### samplingModes

• `Optional` **samplingModes**: `number`[]

Define the sampling modes of all the draw buffers we want to create

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/multiRenderTarget.ts:25

___

### textureCount

• `Optional` **textureCount**: `number`

Define the number of desired draw buffers

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/multiRenderTarget.ts:49

___

### types

• `Optional` **types**: `number`[]

Define the types of all the draw buffers we want to create

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/multiRenderTarget.ts:21

___

### useSRGBBuffers

• `Optional` **useSRGBBuffers**: `boolean`[]

Define if sRGB format should be used for each of the draw buffers we want to create

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/multiRenderTarget.ts:29
