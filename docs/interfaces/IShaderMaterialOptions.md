[@dev/core](../README.md) / [Exports](../modules.md) / IShaderMaterialOptions

# Interface: IShaderMaterialOptions

Defines the options associated with the creation of a shader material.

## Table of contents

### Properties

- [attributes](IShaderMaterialOptions.md#attributes)
- [defines](IShaderMaterialOptions.md#defines)
- [externalTextures](IShaderMaterialOptions.md#externaltextures)
- [needAlphaBlending](IShaderMaterialOptions.md#needalphablending)
- [needAlphaTesting](IShaderMaterialOptions.md#needalphatesting)
- [samplerObjects](IShaderMaterialOptions.md#samplerobjects)
- [samplers](IShaderMaterialOptions.md#samplers)
- [shaderLanguage](IShaderMaterialOptions.md#shaderlanguage)
- [storageBuffers](IShaderMaterialOptions.md#storagebuffers)
- [uniformBuffers](IShaderMaterialOptions.md#uniformbuffers)
- [uniforms](IShaderMaterialOptions.md#uniforms)
- [useClipPlane](IShaderMaterialOptions.md#useclipplane)

## Properties

### attributes

• **attributes**: `string`[]

The list of attribute names used in the shader

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:46

___

### defines

• **defines**: `string`[]

The list of defines used in the shader

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:81

___

### externalTextures

• **externalTextures**: `string`[]

The list of external texture names used in the shader

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:66

___

### needAlphaBlending

• **needAlphaBlending**: `boolean`

Does the material work in alpha blend mode

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:36

___

### needAlphaTesting

• **needAlphaTesting**: `boolean`

Does the material work in alpha test mode

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:41

___

### samplerObjects

• **samplerObjects**: `string`[]

The list of sampler object names used in the shader

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:71

___

### samplers

• **samplers**: `string`[]

The list of sampler (texture) names used in the shader

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:61

___

### shaderLanguage

• `Optional` **shaderLanguage**: [`ShaderLanguage`](../enums/ShaderLanguage.md)

The language the shader is written in (default: GLSL)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:91

___

### storageBuffers

• **storageBuffers**: `string`[]

The list of storage buffer names used in the shader

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:76

___

### uniformBuffers

• **uniformBuffers**: `string`[]

The list of UBO names used in the shader

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:56

___

### uniforms

• **uniforms**: `string`[]

The list of uniform names used in the shader

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:51

___

### useClipPlane

• **useClipPlane**: [`Nullable`](../modules.md#nullable)`boolean`

Defines if clip planes have to be turned on: true to turn them on, false to turn them off and null to turn them on/off depending on the scene configuration (scene.clipPlaneX)

#### Defined in

https://github.com/babylon.js/core/src/Materials/shaderMaterial.ts:86
