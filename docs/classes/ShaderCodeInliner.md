[@dev/core](../README.md) / [Exports](../modules.md) / ShaderCodeInliner

# Class: ShaderCodeInliner

Class used to inline functions in shader code

## Table of contents

### Constructors

- [constructor](ShaderCodeInliner.md#constructor)

### Properties

- [\_functionDescr](ShaderCodeInliner.md#_functiondescr)
- [\_numMaxIterations](ShaderCodeInliner.md#_nummaxiterations)
- [\_sourceCode](ShaderCodeInliner.md#_sourcecode)
- [debug](ShaderCodeInliner.md#debug)
- [inlineToken](ShaderCodeInliner.md#inlinetoken)
- [\_RegexpFindFunctionNameAndType](ShaderCodeInliner.md#_regexpfindfunctionnameandtype)

### Accessors

- [code](ShaderCodeInliner.md#code)

### Methods

- [\_collectFunctions](ShaderCodeInliner.md#_collectfunctions)
- [\_processInlining](ShaderCodeInliner.md#_processinlining)
- [\_replaceFunctionCallsByCode](ShaderCodeInliner.md#_replacefunctioncallsbycode)
- [\_replaceNames](ShaderCodeInliner.md#_replacenames)
- [processCode](ShaderCodeInliner.md#processcode)

## Constructors

### constructor

• **new ShaderCodeInliner**(`sourceCode`, `numMaxIterations?`)

Initializes the inliner

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `sourceCode` | `string` | `undefined` | shader code source to inline |
| `numMaxIterations` | `number` | `20` | maximum number of iterations (used to detect recursive calls) |

#### Defined in

packages/dev/core/src/Engines/Processors/shaderCodeInliner.ts:37

## Properties

### \_functionDescr

• `Private` **\_functionDescr**: `IInlineFunctionDescr`[]

#### Defined in

packages/dev/core/src/Engines/Processors/shaderCodeInliner.ts:18

___

### \_numMaxIterations

• `Private` **\_numMaxIterations**: `number`

#### Defined in

packages/dev/core/src/Engines/Processors/shaderCodeInliner.ts:19

___

### \_sourceCode

• `Private` **\_sourceCode**: `string`

#### Defined in

packages/dev/core/src/Engines/Processors/shaderCodeInliner.ts:17

___

### debug

• **debug**: `boolean` = `false`

Gets or sets the debug mode

#### Defined in

packages/dev/core/src/Engines/Processors/shaderCodeInliner.ts:25

___

### inlineToken

• **inlineToken**: `string`

Gets or sets the token used to mark the functions to inline

#### Defined in

packages/dev/core/src/Engines/Processors/shaderCodeInliner.ts:22

___

### \_RegexpFindFunctionNameAndType

▪ `Static` `Private` `Readonly` **\_RegexpFindFunctionNameAndType**: `RegExp`

#### Defined in

packages/dev/core/src/Engines/Processors/shaderCodeInliner.ts:15

## Accessors

### code

• `get` **code**(): `string`

Gets the code after the inlining process

#### Returns

`string`

#### Defined in

packages/dev/core/src/Engines/Processors/shaderCodeInliner.ts:28

## Methods

### \_collectFunctions

▸ `Private` **_collectFunctions**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Engines/Processors/shaderCodeInliner.ts:58

___

### \_processInlining

▸ `Private` **_processInlining**(`numMaxIterations?`): `boolean`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `numMaxIterations` | `number` | `20` |

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Engines/Processors/shaderCodeInliner.ts:165

___

### \_replaceFunctionCallsByCode

▸ `Private` **_replaceFunctionCallsByCode**(): `boolean`

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Engines/Processors/shaderCodeInliner.ts:179

___

### \_replaceNames

▸ `Private` **_replaceNames**(`code`, `sources`, `destinations`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `code` | `string` |
| `sources` | `string`[] |
| `destinations` | `string`[] |

#### Returns

`string`

#### Defined in

packages/dev/core/src/Engines/Processors/shaderCodeInliner.ts:325

___

### processCode

▸ **processCode**(): `void`

Start the processing of the shader code

#### Returns

`void`

#### Defined in

packages/dev/core/src/Engines/Processors/shaderCodeInliner.ts:47
