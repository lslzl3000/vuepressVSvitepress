[@dev/core](../README.md) / [Exports](../modules.md) / EnvironmentTextureSpecularInfoV1

# Interface: EnvironmentTextureSpecularInfoV1

Defines the specular data enclosed in the file.
This corresponds to the version 1 of the data.

## Table of contents

### Properties

- [lodGenerationScale](EnvironmentTextureSpecularInfoV1.md#lodgenerationscale)
- [mipmaps](EnvironmentTextureSpecularInfoV1.md#mipmaps)
- [specularDataPosition](EnvironmentTextureSpecularInfoV1.md#speculardataposition)

## Properties

### lodGenerationScale

• **lodGenerationScale**: `number`

Defines the scale applied to environment texture. This manages the range of LOD level used for IBL according to the roughness.

#### Defined in

https://github.com/babylon.js/core/src/Misc/environmentTextureTools.ts:118

___

### mipmaps

• **mipmaps**: `BufferImageData`[]

This contains all the images data needed to reconstruct the cubemap.

#### Defined in

https://github.com/babylon.js/core/src/Misc/environmentTextureTools.ts:114

___

### specularDataPosition

• `Optional` **specularDataPosition**: `number`

Defines where the specular Payload is located. It is a runtime value only not stored in the file.

#### Defined in

https://github.com/babylon.js/core/src/Misc/environmentTextureTools.ts:110
