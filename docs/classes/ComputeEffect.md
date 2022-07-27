[@dev/core](../README.md) / [Exports](../modules.md) / ComputeEffect

# Class: ComputeEffect

Effect wrapping a compute shader and let execute (dispatch) the shader

## Table of contents

### Constructors

- [constructor](ComputeEffect.md#constructor)

### Properties

- [\_compilationError](ComputeEffect.md#_compilationerror)
- [\_computeSourceCodeOverride](ComputeEffect.md#_computesourcecodeoverride)
- [\_engine](ComputeEffect.md#_engine)
- [\_entryPoint](ComputeEffect.md#_entrypoint)
- [\_includeShaderStore](ComputeEffect.md#_includeshaderstore)
- [\_isReady](ComputeEffect.md#_isready)
- [\_rawComputeSourceCode](ComputeEffect.md#_rawcomputesourcecode)
- [\_shaderLanguage](ComputeEffect.md#_shaderlanguage)
- [\_shaderRepository](ComputeEffect.md#_shaderrepository)
- [\_shaderStore](ComputeEffect.md#_shaderstore)
- [defines](ComputeEffect.md#defines)
- [name](ComputeEffect.md#name)
- [onBindObservable](ComputeEffect.md#onbindobservable)
- [onCompileObservable](ComputeEffect.md#oncompileobservable)
- [onCompiled](ComputeEffect.md#oncompiled)
- [onError](ComputeEffect.md#onerror)
- [onErrorObservable](ComputeEffect.md#onerrorobservable)
- [uniqueId](ComputeEffect.md#uniqueid)
- [LogShaderCodeOnCompilationError](ComputeEffect.md#logshadercodeoncompilationerror)
- [\_UniqueIdSeed](ComputeEffect.md#_uniqueidseed)

### Accessors

- [computeSourceCode](ComputeEffect.md#computesourcecode)
- [key](ComputeEffect.md#key)
- [rawComputeSourceCode](ComputeEffect.md#rawcomputesourcecode)

### Methods

- [\_checkIsReady](ComputeEffect.md#_checkisready)
- [\_getShaderCodeAndErrorLine](ComputeEffect.md#_getshadercodeanderrorline)
- [\_isReadyInternal](ComputeEffect.md#_isreadyinternal)
- [\_loadShader](ComputeEffect.md#_loadshader)
- [\_processCompilationErrors](ComputeEffect.md#_processcompilationerrors)
- [\_useFinalCode](ComputeEffect.md#_usefinalcode)
- [dispose](ComputeEffect.md#dispose)
- [executeWhenCompiled](ComputeEffect.md#executewhencompiled)
- [getCompilationError](ComputeEffect.md#getcompilationerror)
- [getEngine](ComputeEffect.md#getengine)
- [getPipelineContext](ComputeEffect.md#getpipelinecontext)
- [isReady](ComputeEffect.md#isready)
- [RegisterShader](ComputeEffect.md#registershader)

## Constructors

### constructor

• **new ComputeEffect**(`baseName`, `options`, `engine`, `key?`)

Creates a compute effect that can be used to execute a compute shader

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `baseName` | `any` | `undefined` | Name of the effect |
| `options` | [`IComputeEffectCreationOptions`](../interfaces/IComputeEffectCreationOptions.md) | `undefined` | Set of all options to create the effect |
| `engine` | [`Engine`](Engine.md) | `undefined` | The engine the effect is created for |
| `key` | `string` | `""` | Effect Key identifying uniquely compiled shader variants |

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeEffect.ts:113

## Properties

### \_compilationError

• `Private` **\_compilationError**: `string` = `""`

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeEffect.ts:91

___

### \_computeSourceCodeOverride

• `Private` **\_computeSourceCodeOverride**: `string` = `""`

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeEffect.ts:94

___

### \_engine

• `Private` **\_engine**: [`Engine`](Engine.md)

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeEffect.ts:89

___

### \_entryPoint

• `Private` **\_entryPoint**: `string`

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeEffect.ts:100

___

### \_includeShaderStore

• `Private` **\_includeShaderStore**: `Object`

#### Index signature

▪ [key: `string`]: `string`

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeEffect.ts:104

___

### \_isReady

• `Private` **\_isReady**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeEffect.ts:90

___

### \_rawComputeSourceCode

• `Private` **\_rawComputeSourceCode**: `string` = `""`

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeEffect.ts:99

___

### \_shaderLanguage

• `Private` **\_shaderLanguage**: [`ShaderLanguage`](../enums/ShaderLanguage.md) = `ShaderLanguage.WGSL`

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeEffect.ts:101

___

### \_shaderRepository

• `Private` **\_shaderRepository**: `string`

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeEffect.ts:103

___

### \_shaderStore

• `Private` **\_shaderStore**: `Object`

#### Index signature

▪ [key: `string`]: `string`

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeEffect.ts:102

___

### defines

• **defines**: `string` = `""`

String container all the define statements that should be set on the shader.

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeEffect.ts:56

___

### name

• **name**: `any` = `null`

Name of the effect.

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeEffect.ts:52

___

### onBindObservable

• **onBindObservable**: [`Observable`](Observable.md)[`ComputeEffect`](ComputeEffect.md)

Observable that will be called when effect is bound.

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeEffect.ts:81

___

### onCompileObservable

• **onCompileObservable**: [`Observable`](Observable.md)[`ComputeEffect`](ComputeEffect.md)

Observable that will be called when the shader is compiled.
It is recommended to use executeWhenCompile() or to make sure that scene.isReady() is called to get this observable raised.

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeEffect.ts:73

___

### onCompiled

• **onCompiled**: [`Nullable`](../modules.md#nullable)(`effect`: [`ComputeEffect`](ComputeEffect.md)) => `void` = `null`

Callback that will be called when the shader is compiled.

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeEffect.ts:60

___

### onError

• **onError**: [`Nullable`](../modules.md#nullable)(`effect`: [`ComputeEffect`](ComputeEffect.md), `errors`: `string`) => `void` = `null`

Callback that will be called if an error occurs during shader compilation.

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeEffect.ts:64

___

### onErrorObservable

• **onErrorObservable**: [`Observable`](Observable.md)[`ComputeEffect`](ComputeEffect.md)

Observable that will be called if an error occurs during shader compilation.

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeEffect.ts:77

___

### uniqueId

• **uniqueId**: `number` = `0`

Unique ID of the effect.

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeEffect.ts:68

___

### LogShaderCodeOnCompilationError

▪ `Static` **LogShaderCodeOnCompilationError**: `boolean` = `true`

Enable logging of the shader code when a compilation error occurs

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeEffect.ts:48

___

### \_UniqueIdSeed

▪ `Static` `Private` **\_UniqueIdSeed**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeEffect.ts:43

## Accessors

### computeSourceCode

• `get` **computeSourceCode**(): `string`

Gets the compute shader source code of this effect

#### Returns

`string`

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeEffect.ts:327

___

### key

• `get` **key**(): `string`

Unique key for this effect

#### Returns

`string`

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeEffect.ts:193

___

### rawComputeSourceCode

• `get` **rawComputeSourceCode**(): `string`

Gets the compute shader source code before it has been processed by the preprocessor

#### Returns

`string`

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeEffect.ts:334

## Methods

### \_checkIsReady

▸ `Private` **_checkIsReady**(`previousPipelineContext`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `previousPipelineContext` | [`Nullable`](../modules.md#nullable)`IComputePipelineContext` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeEffect.ts:264

___

### \_getShaderCodeAndErrorLine

▸ `Private` **_getShaderCodeAndErrorLine**(`code`, `error`): [[`Nullable`](../modules.md#nullable)`string`, [`Nullable`](../modules.md#nullable)`string`]

#### Parameters

| Name | Type |
| :------ | :------ |
| `code` | [`Nullable`](../modules.md#nullable)`string` |
| `error` | [`Nullable`](../modules.md#nullable)`string` |

#### Returns

[[`Nullable`](../modules.md#nullable)`string`, [`Nullable`](../modules.md#nullable)`string`]

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeEffect.ts:385

___

### \_isReadyInternal

▸ `Private` **_isReadyInternal**(): `boolean`

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeEffect.ts:209

___

### \_loadShader

▸ `Private` **_loadShader**(`shader`, `key`, `optionalKey`, `callback`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `shader` | `any` |
| `key` | `string` |
| `optionalKey` | `string` |
| `callback` | (`data`: `any`) => `void` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeEffect.ts:279

___

### \_processCompilationErrors

▸ `Private` **_processCompilationErrors**(`e`, `previousPipelineContext?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `e` | `any` | `undefined` |
| `previousPipelineContext` | [`Nullable`](../modules.md#nullable)`IComputePipelineContext` | `null` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeEffect.ts:404

___

### \_useFinalCode

▸ `Private` **_useFinalCode**(`migratedCommputeCode`, `baseName`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `migratedCommputeCode` | `string` |
| `baseName` | `any` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeEffect.ts:179

___

### dispose

▸ **dispose**(): `void`

Release all associated resources.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeEffect.ts:438

___

### executeWhenCompiled

▸ **executeWhenCompiled**(`func`): `void`

Adds a callback to the onCompiled observable and call the callback immediately if already ready.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `func` | (`effect`: [`ComputeEffect`](ComputeEffect.md)) => `void` | The callback to be used. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeEffect.ts:247

___

### getCompilationError

▸ **getCompilationError**(): `string`

The error from the last compilation.

#### Returns

`string`

the error string.

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeEffect.ts:239

___

### getEngine

▸ **getEngine**(): [`Engine`](Engine.md)

The engine the effect was initialized with.

#### Returns

[`Engine`](Engine.md)

the engine.

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeEffect.ts:223

___

### getPipelineContext

▸ **getPipelineContext**(): [`Nullable`](../modules.md#nullable)`IComputePipelineContext`

The pipeline context for this effect

#### Returns

[`Nullable`](../modules.md#nullable)`IComputePipelineContext`

the associated pipeline context

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeEffect.ts:231

___

### isReady

▸ **isReady**(): `boolean`

If the effect has been compiled and prepared.

#### Returns

`boolean`

if the effect is compiled and prepared.

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeEffect.ts:201

___

### RegisterShader

▸ `Static` **RegisterShader**(`name`, `computeShader`): `void`

This function will add a new compute shader to the shader store

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | the name of the shader |
| `computeShader` | `string` | compute shader content |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeEffect.ts:450
