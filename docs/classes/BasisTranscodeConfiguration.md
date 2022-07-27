[@dev/core](../README.md) / [Exports](../modules.md) / BasisTranscodeConfiguration

# Class: BasisTranscodeConfiguration

Configuration options for the Basis transcoder

## Table of contents

### Constructors

- [constructor](BasisTranscodeConfiguration.md#constructor)

### Properties

- [loadMipmapLevels](BasisTranscodeConfiguration.md#loadmipmaplevels)
- [loadSingleImage](BasisTranscodeConfiguration.md#loadsingleimage)
- [supportedCompressionFormats](BasisTranscodeConfiguration.md#supportedcompressionformats)

## Constructors

### constructor

• **new BasisTranscodeConfiguration**()

## Properties

### loadMipmapLevels

• `Optional` **loadMipmapLevels**: `boolean`

If mipmap levels should be loaded for transcoded images (Default: true)

#### Defined in

https://github.com/babylon.js/core/src/Misc/basis.ts:74

___

### loadSingleImage

• `Optional` **loadSingleImage**: `number`

Index of a single image to load (Default: all images)

#### Defined in

https://github.com/babylon.js/core/src/Misc/basis.ts:78

___

### supportedCompressionFormats

• `Optional` **supportedCompressionFormats**: `Object`

Supported compression formats used to determine the supported output format of the transcoder

#### Type declaration

| Name | Type | Description |
| :------ | :------ | :------ |
| `astc?` | `boolean` | astc compression format |
| `bc7?` | `boolean` | bc7 compression format |
| `etc1?` | `boolean` | etc1 compression format |
| `etc2?` | `boolean` | etc2 compression format |
| `pvrtc?` | `boolean` | pvrtc compression format |
| `s3tc?` | `boolean` | s3tc compression format |

#### Defined in

https://github.com/babylon.js/core/src/Misc/basis.ts:45
