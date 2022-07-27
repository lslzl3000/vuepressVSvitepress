[@dev/core](../README.md) / [Exports](../modules.md) / ShaderStore

# Class: ShaderStore

Defines the shader related stores and directory

## Table of contents

### Constructors

- [constructor](ShaderStore.md#constructor)

### Properties

- [IncludesShadersStore](ShaderStore.md#includesshadersstore)
- [IncludesShadersStoreWGSL](ShaderStore.md#includesshadersstorewgsl)
- [ShadersRepository](ShaderStore.md#shadersrepository)
- [ShadersRepositoryWGSL](ShaderStore.md#shadersrepositorywgsl)
- [ShadersStore](ShaderStore.md#shadersstore)
- [ShadersStoreWGSL](ShaderStore.md#shadersstorewgsl)

### Methods

- [GetIncludesShadersStore](ShaderStore.md#getincludesshadersstore)
- [GetShadersRepository](ShaderStore.md#getshadersrepository)
- [GetShadersStore](ShaderStore.md#getshadersstore)

## Constructors

### constructor

• **new ShaderStore**()

## Properties

### IncludesShadersStore

▪ `Static` **IncludesShadersStore**: `Object` = `{}`

Store of each included file for a shader (The can be looked up using effect.key)

#### Index signature

▪ [key: `string`]: `string`

#### Defined in

packages/dev/core/src/Engines/shaderStore.ts:18

___

### IncludesShadersStoreWGSL

▪ `Static` **IncludesShadersStoreWGSL**: `Object` = `{}`

Store of each included file for a shader (WGSL)

#### Index signature

▪ [key: `string`]: `string`

#### Defined in

packages/dev/core/src/Engines/shaderStore.ts:31

___

### ShadersRepository

▪ `Static` **ShadersRepository**: `string` = `"src/Shaders/"`

Gets or sets the relative url used to load shaders if using the engine in non-minified mode

#### Defined in

packages/dev/core/src/Engines/shaderStore.ts:10

___

### ShadersRepositoryWGSL

▪ `Static` **ShadersRepositoryWGSL**: `string` = `"src/ShadersWGSL/"`

Gets or sets the relative url used to load shaders (WGSL) if using the engine in non-minified mode

#### Defined in

packages/dev/core/src/Engines/shaderStore.ts:23

___

### ShadersStore

▪ `Static` **ShadersStore**: `Object` = `{}`

Store of each shader (The can be looked up using effect.key)

#### Index signature

▪ [key: `string`]: `string`

#### Defined in

packages/dev/core/src/Engines/shaderStore.ts:14

___

### ShadersStoreWGSL

▪ `Static` **ShadersStoreWGSL**: `Object` = `{}`

Store of each shader  (WGSL)

#### Index signature

▪ [key: `string`]: `string`

#### Defined in

packages/dev/core/src/Engines/shaderStore.ts:27

## Methods

### GetIncludesShadersStore

▸ `Static` **GetIncludesShadersStore**(`shaderLanguage?`): `Object`

Gets the include shaders store of a given shader language

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `shaderLanguage` | [`ShaderLanguage`](../enums/ShaderLanguage.md) | `ShaderLanguage.GLSL` | the shader language |

#### Returns

`Object`

the include shaders store

#### Defined in

packages/dev/core/src/Engines/shaderStore.ts:56

___

### GetShadersRepository

▸ `Static` **GetShadersRepository**(`shaderLanguage?`): `string`

Gets the shaders repository path for a given shader language

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `shaderLanguage` | [`ShaderLanguage`](../enums/ShaderLanguage.md) | `ShaderLanguage.GLSL` | the shader language |

#### Returns

`string`

the path to the shaders repository

#### Defined in

packages/dev/core/src/Engines/shaderStore.ts:38

___

### GetShadersStore

▸ `Static` **GetShadersStore**(`shaderLanguage?`): `Object`

Gets the shaders store of a given shader language

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `shaderLanguage` | [`ShaderLanguage`](../enums/ShaderLanguage.md) | `ShaderLanguage.GLSL` | the shader language |

#### Returns

`Object`

the shaders store

#### Defined in

packages/dev/core/src/Engines/shaderStore.ts:47
