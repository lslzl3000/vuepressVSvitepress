[@dev/core](../README.md) / [Exports](../modules.md) / DDSInfo

# Interface: DDSInfo

Direct draw surface info

**`See`**

https://docs.microsoft.com/en-us/windows/desktop/direct3ddds/dx-graphics-dds-pguide

## Table of contents

### Properties

- [dxgiFormat](DDSInfo.md#dxgiformat)
- [height](DDSInfo.md#height)
- [isCompressed](DDSInfo.md#iscompressed)
- [isCube](DDSInfo.md#iscube)
- [isFourCC](DDSInfo.md#isfourcc)
- [isLuminance](DDSInfo.md#isluminance)
- [isRGB](DDSInfo.md#isrgb)
- [mipmapCount](DDSInfo.md#mipmapcount)
- [sphericalPolynomial](DDSInfo.md#sphericalpolynomial)
- [textureType](DDSInfo.md#texturetype)
- [width](DDSInfo.md#width)

## Properties

### dxgiFormat

• **dxgiFormat**: `number`

The dxgiFormat of the texture

**`See`**

https://docs.microsoft.com/en-us/windows/desktop/api/dxgiformat/ne-dxgiformat-dxgi_format

#### Defined in

https://github.com/babylon.js/core/src/Misc/dds.ts:138

___

### height

• **height**: `number`

Width of the texture

#### Defined in

https://github.com/babylon.js/core/src/Misc/dds.ts:106

___

### isCompressed

• **isCompressed**: `boolean`

If the texture is a compressed format eg. FOURCC_DXT1

#### Defined in

https://github.com/babylon.js/core/src/Misc/dds.ts:133

___

### isCube

• **isCube**: `boolean`

If this is a cube texture

**`See`**

https://docs.microsoft.com/en-us/windows/desktop/direct3ddds/dds-file-layout-for-cubic-environment-maps

#### Defined in

https://github.com/babylon.js/core/src/Misc/dds.ts:129

___

### isFourCC

• **isFourCC**: `boolean`

If the textures format is a known fourCC format

**`See`**

https://www.fourcc.org/

#### Defined in

https://github.com/babylon.js/core/src/Misc/dds.ts:116

___

### isLuminance

• **isLuminance**: `boolean`

If the texture is a lumincance format

#### Defined in

https://github.com/babylon.js/core/src/Misc/dds.ts:124

___

### isRGB

• **isRGB**: `boolean`

If the texture is an RGB format eg. DXGI_FORMAT_B8G8R8X8_UNORM format

#### Defined in

https://github.com/babylon.js/core/src/Misc/dds.ts:120

___

### mipmapCount

• **mipmapCount**: `number`

Number of Mipmaps for the texture

**`See`**

https://en.wikipedia.org/wiki/Mipmap

#### Defined in

https://github.com/babylon.js/core/src/Misc/dds.ts:111

___

### sphericalPolynomial

• `Optional` **sphericalPolynomial**: [`SphericalPolynomial`](../classes/SphericalPolynomial.md)

Sphericle polynomial created for the dds texture

#### Defined in

https://github.com/babylon.js/core/src/Misc/dds.ts:146

___

### textureType

• **textureType**: `number`

Texture type eg. Engine.TEXTURETYPE_UNSIGNED_INT, Engine.TEXTURETYPE_FLOAT

#### Defined in

https://github.com/babylon.js/core/src/Misc/dds.ts:142

___

### width

• **width**: `number`

Width of the texture

#### Defined in

https://github.com/babylon.js/core/src/Misc/dds.ts:102
