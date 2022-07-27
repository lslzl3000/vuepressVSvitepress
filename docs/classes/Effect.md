[@dev/core](../README.md) / [Exports](../modules.md) / Effect

# Class: Effect

Effect containing vertex and fragment shader that can be executed on an object.

## Implements

- [`IDisposable`](../interfaces/IDisposable.md)

## Table of contents

### Constructors

- [constructor](Effect.md#constructor)

### Properties

- [\_allFallbacksProcessed](Effect.md#_allfallbacksprocessed)
- [\_attributeLocationByName](Effect.md#_attributelocationbyname)
- [\_attributes](Effect.md#_attributes)
- [\_attributesNames](Effect.md#_attributesnames)
- [\_compilationError](Effect.md#_compilationerror)
- [\_fallbacks](Effect.md#_fallbacks)
- [\_fragmentSourceCodeOverride](Effect.md#_fragmentsourcecodeoverride)
- [\_indexParameters](Effect.md#_indexparameters)
- [\_isDisposed](Effect.md#_isdisposed)
- [\_isReady](Effect.md#_isready)
- [\_processingContext](Effect.md#_processingcontext)
- [\_samplers](Effect.md#_samplers)
- [\_shaderLanguage](Effect.md#_shaderlanguage)
- [\_transformFeedbackVaryings](Effect.md#_transformfeedbackvaryings)
- [\_uniformBuffersNamesList](Effect.md#_uniformbuffersnameslist)
- [\_uniforms](Effect.md#_uniforms)
- [\_uniformsNames](Effect.md#_uniformsnames)
- [\_vertexSourceCodeOverride](Effect.md#_vertexsourcecodeoverride)
- [defines](Effect.md#defines)
- [name](Effect.md#name)
- [onBind](Effect.md#onbind)
- [onCompileObservable](Effect.md#oncompileobservable)
- [onCompiled](Effect.md#oncompiled)
- [onError](Effect.md#onerror)
- [onErrorObservable](Effect.md#onerrorobservable)
- [uniqueId](Effect.md#uniqueid)
- [IncludesShadersStore](Effect.md#includesshadersstore)
- [LogShaderCodeOnCompilationError](Effect.md#logshadercodeoncompilationerror)
- [ShadersStore](Effect.md#shadersstore)
- [\_BaseCache](Effect.md#_basecache)
- [\_UniqueIdSeed](Effect.md#_uniqueidseed)

### Accessors

- [fragmentSourceCode](Effect.md#fragmentsourcecode)
- [isSupported](Effect.md#issupported)
- [key](Effect.md#key)
- [onBindObservable](Effect.md#onbindobservable)
- [rawFragmentSourceCode](Effect.md#rawfragmentsourcecode)
- [rawVertexSourceCode](Effect.md#rawvertexsourcecode)
- [vertexSourceCode](Effect.md#vertexsourcecode)
- [ShadersRepository](Effect.md#shadersrepository)

### Methods

- [\_checkIsReady](Effect.md#_checkisready)
- [\_getShaderCodeAndErrorLine](Effect.md#_getshadercodeanderrorline)
- [\_isReadyInternal](Effect.md#_isreadyinternal)
- [\_loadShader](Effect.md#_loadshader)
- [\_processCompilationErrors](Effect.md#_processcompilationerrors)
- [\_useFinalCode](Effect.md#_usefinalcode)
- [allFallbacksProcessed](Effect.md#allfallbacksprocessed)
- [bindUniformBlock](Effect.md#binduniformblock)
- [bindUniformBuffer](Effect.md#binduniformbuffer)
- [dispose](Effect.md#dispose)
- [executeWhenCompiled](Effect.md#executewhencompiled)
- [getAttributeLocation](Effect.md#getattributelocation)
- [getAttributeLocationByName](Effect.md#getattributelocationbyname)
- [getAttributesCount](Effect.md#getattributescount)
- [getAttributesNames](Effect.md#getattributesnames)
- [getCompilationError](Effect.md#getcompilationerror)
- [getEngine](Effect.md#getengine)
- [getIndexParameters](Effect.md#getindexparameters)
- [getPipelineContext](Effect.md#getpipelinecontext)
- [getSamplers](Effect.md#getsamplers)
- [getUniform](Effect.md#getuniform)
- [getUniformBuffersNames](Effect.md#getuniformbuffersnames)
- [getUniformIndex](Effect.md#getuniformindex)
- [getUniformNames](Effect.md#getuniformnames)
- [isReady](Effect.md#isready)
- [setArray](Effect.md#setarray)
- [setArray2](Effect.md#setarray2)
- [setArray3](Effect.md#setarray3)
- [setArray4](Effect.md#setarray4)
- [setBool](Effect.md#setbool)
- [setColor3](Effect.md#setcolor3)
- [setColor4](Effect.md#setcolor4)
- [setDepthStencilTexture](Effect.md#setdepthstenciltexture)
- [setDirectColor4](Effect.md#setdirectcolor4)
- [setExternalTexture](Effect.md#setexternaltexture)
- [setFloat](Effect.md#setfloat)
- [setFloat2](Effect.md#setfloat2)
- [setFloat3](Effect.md#setfloat3)
- [setFloat4](Effect.md#setfloat4)
- [setFloatArray](Effect.md#setfloatarray)
- [setFloatArray2](Effect.md#setfloatarray2)
- [setFloatArray3](Effect.md#setfloatarray3)
- [setFloatArray4](Effect.md#setfloatarray4)
- [setInt](Effect.md#setint)
- [setInt2](Effect.md#setint2)
- [setInt3](Effect.md#setint3)
- [setInt4](Effect.md#setint4)
- [setIntArray](Effect.md#setintarray)
- [setIntArray2](Effect.md#setintarray2)
- [setIntArray3](Effect.md#setintarray3)
- [setIntArray4](Effect.md#setintarray4)
- [setMatrices](Effect.md#setmatrices)
- [setMatrix](Effect.md#setmatrix)
- [setMatrix2x2](Effect.md#setmatrix2x2)
- [setMatrix3x3](Effect.md#setmatrix3x3)
- [setQuaternion](Effect.md#setquaternion)
- [setStorageBuffer](Effect.md#setstoragebuffer)
- [setTexture](Effect.md#settexture)
- [setTextureArray](Effect.md#settexturearray)
- [setTextureFromPostProcess](Effect.md#settexturefrompostprocess)
- [setTextureFromPostProcessOutput](Effect.md#settexturefrompostprocessoutput)
- [setTextureSampler](Effect.md#settexturesampler)
- [setVector2](Effect.md#setvector2)
- [setVector3](Effect.md#setvector3)
- [setVector4](Effect.md#setvector4)
- [RegisterShader](Effect.md#registershader)
- [ResetCache](Effect.md#resetcache)

## Constructors

### constructor

• **new Effect**(`baseName`, `attributesNamesOrOptions`, `uniformsNamesOrEngine`, `samplers?`, `engine?`, `defines?`, `fallbacks?`, `onCompiled?`, `onError?`, `indexParameters?`, `key?`, `shaderLanguage?`)

Instantiates an effect.
An effect can be used to create/manage/execute vertex and fragment shaders.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `baseName` | `any` | `undefined` | Name of the effect. |
| `attributesNamesOrOptions` | `string`[] \| [`IEffectCreationOptions`](../interfaces/IEffectCreationOptions.md) | `undefined` | List of attribute names that will be passed to the shader or set of all options to create the effect. |
| `uniformsNamesOrEngine` | `string`[] \| [`ThinEngine`](ThinEngine.md) | `undefined` | List of uniform variable names that will be passed to the shader or the engine that will be used to render effect. |
| `samplers` | [`Nullable`](../modules.md#nullable)`string`[] | `null` | List of sampler variables that will be passed to the shader. |
| `engine?` | [`ThinEngine`](ThinEngine.md) | `undefined` | Engine to be used to render the effect |
| `defines` | [`Nullable`](../modules.md#nullable)`string` | `null` | Define statements to be added to the shader. |
| `fallbacks` | [`Nullable`](../modules.md#nullable)[`IEffectFallbacks`](../interfaces/IEffectFallbacks.md) | `null` | Possible fallbacks for this effect to improve performance when needed. |
| `onCompiled` | [`Nullable`](../modules.md#nullable)(`effect`: [`Effect`](Effect.md)) => `void` | `null` | Callback that will be called when the shader is compiled. |
| `onError` | [`Nullable`](../modules.md#nullable)(`effect`: [`Effect`](Effect.md), `errors`: `string`) => `void` | `null` | Callback that will be called if an error occurs during shader compilation. |
| `indexParameters?` | `any` | `undefined` | Parameters to be used with Babylons include syntax to iterate over an array (eg. {lights: 10}) |
| `key` | `string` | `""` | Effect Key identifying uniquely compiled shader variants |
| `shaderLanguage` | [`ShaderLanguage`](../enums/ShaderLanguage.md) | `ShaderLanguage.GLSL` | the language the shader is written in (default: GLSL) |

#### Defined in

packages/dev/core/src/Materials/effect.ts:235

## Properties

### \_allFallbacksProcessed

• `Private` **\_allFallbacksProcessed**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Materials/effect.ts:185

___

### \_attributeLocationByName

• `Private` **\_attributeLocationByName**: `Object`

#### Index signature

▪ [name: `string`]: `number`

#### Defined in

packages/dev/core/src/Materials/effect.ts:188

___

### \_attributes

• `Private` **\_attributes**: `number`[]

#### Defined in

packages/dev/core/src/Materials/effect.ts:187

___

### \_attributesNames

• `Private` **\_attributesNames**: `string`[]

#### Defined in

packages/dev/core/src/Materials/effect.ts:186

___

### \_compilationError

• `Private` **\_compilationError**: `string` = `""`

#### Defined in

packages/dev/core/src/Materials/effect.ts:184

___

### \_fallbacks

• `Private` **\_fallbacks**: [`Nullable`](../modules.md#nullable)[`IEffectFallbacks`](../interfaces/IEffectFallbacks.md) = `null`

#### Defined in

packages/dev/core/src/Materials/effect.ts:196

___

### \_fragmentSourceCodeOverride

• `Private` **\_fragmentSourceCodeOverride**: `string` = `""`

#### Defined in

packages/dev/core/src/Materials/effect.ts:198

___

### \_indexParameters

• `Private` **\_indexParameters**: `any`

#### Defined in

packages/dev/core/src/Materials/effect.ts:195

___

### \_isDisposed

• `Private` **\_isDisposed**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Materials/effect.ts:155

___

### \_isReady

• `Private` **\_isReady**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Materials/effect.ts:183

___

### \_processingContext

• `Private` **\_processingContext**: [`Nullable`](../modules.md#nullable)`ShaderProcessingContext`

#### Defined in

packages/dev/core/src/Materials/effect.ts:217

___

### \_samplers

• `Private` **\_samplers**: `Object` = `{}`

#### Index signature

▪ [key: `string`]: `number`

#### Defined in

packages/dev/core/src/Materials/effect.ts:182

___

### \_shaderLanguage

• `Private` **\_shaderLanguage**: [`ShaderLanguage`](../enums/ShaderLanguage.md)

#### Defined in

packages/dev/core/src/Materials/effect.ts:200

___

### \_transformFeedbackVaryings

• `Private` **\_transformFeedbackVaryings**: [`Nullable`](../modules.md#nullable)`string`[] = `null`

#### Defined in

packages/dev/core/src/Materials/effect.ts:199

___

### \_uniformBuffersNamesList

• `Private` **\_uniformBuffersNamesList**: `string`[]

#### Defined in

packages/dev/core/src/Materials/effect.ts:180

___

### \_uniforms

• `Private` **\_uniforms**: `Object` = `{}`

#### Index signature

▪ [key: `string`]: [`Nullable`](../modules.md#nullable)`WebGLUniformLocation`

#### Defined in

packages/dev/core/src/Materials/effect.ts:189

___

### \_uniformsNames

• `Private` **\_uniformsNames**: `string`[]

#### Defined in

packages/dev/core/src/Materials/effect.ts:181

___

### \_vertexSourceCodeOverride

• `Private` **\_vertexSourceCodeOverride**: `string` = `""`

#### Defined in

packages/dev/core/src/Materials/effect.ts:197

___

### defines

• **defines**: `string` = `""`

String container all the define statements that should be set on the shader.

#### Defined in

packages/dev/core/src/Materials/effect.ts:113

___

### name

• **name**: `any` = `null`

Name of the effect.

#### Defined in

packages/dev/core/src/Materials/effect.ts:109

___

### onBind

• **onBind**: [`Nullable`](../modules.md#nullable)(`effect`: [`Effect`](Effect.md)) => `void` = `null`

Callback that will be called when effect is bound.

#### Defined in

packages/dev/core/src/Materials/effect.ts:125

___

### onCompileObservable

• **onCompileObservable**: [`Observable`](Observable.md)[`Effect`](Effect.md)

Observable that will be called when the shader is compiled.
It is recommended to use executeWhenCompile() or to make sure that scene.isReady() is called to get this observable raised.

#### Defined in

packages/dev/core/src/Materials/effect.ts:134

___

### onCompiled

• **onCompiled**: [`Nullable`](../modules.md#nullable)(`effect`: [`Effect`](Effect.md)) => `void` = `null`

Callback that will be called when the shader is compiled.

#### Defined in

packages/dev/core/src/Materials/effect.ts:117

___

### onError

• **onError**: [`Nullable`](../modules.md#nullable)(`effect`: [`Effect`](Effect.md), `errors`: `string`) => `void` = `null`

Callback that will be called if an error occurs during shader compilation.

#### Defined in

packages/dev/core/src/Materials/effect.ts:121

___

### onErrorObservable

• **onErrorObservable**: [`Observable`](Observable.md)[`Effect`](Effect.md)

Observable that will be called if an error occurs during shader compilation.

#### Defined in

packages/dev/core/src/Materials/effect.ts:138

___

### uniqueId

• **uniqueId**: `number` = `0`

Unique ID of the effect.

#### Defined in

packages/dev/core/src/Materials/effect.ts:129

___

### IncludesShadersStore

▪ `Static` **IncludesShadersStore**: `Object` = `EngineShaderStore.IncludesShadersStore`

Store of each included file for a shader (The can be looked up using effect.key)

#### Index signature

▪ [key: `string`]: `string`

#### Defined in

packages/dev/core/src/Materials/effect.ts:1402

___

### LogShaderCodeOnCompilationError

▪ `Static` **LogShaderCodeOnCompilationError**: `boolean` = `true`

Enable logging of the shader code when a compilation error occurs

#### Defined in

packages/dev/core/src/Materials/effect.ts:105

___

### ShadersStore

▪ `Static` **ShadersStore**: `Object` = `EngineShaderStore.ShadersStore`

Store of each shader (The can be looked up using effect.key)

#### Index signature

▪ [key: `string`]: `string`

#### Defined in

packages/dev/core/src/Materials/effect.ts:1398

___

### \_BaseCache

▪ `Static` `Private` **\_BaseCache**: `Object` = `{}`

#### Index signature

▪ [key: `number`]: [`DataBuffer`](DataBuffer.md)

#### Defined in

packages/dev/core/src/Materials/effect.ts:216

___

### \_UniqueIdSeed

▪ `Static` `Private` **\_UniqueIdSeed**: `number` = `0`

#### Defined in

packages/dev/core/src/Materials/effect.ts:177

## Accessors

### fragmentSourceCode

• `get` **fragmentSourceCode**(): `string`

Gets the fragment shader source code of this effect

#### Returns

`string`

#### Defined in

packages/dev/core/src/Materials/effect.ts:649

___

### isSupported

• `get` **isSupported**(): `boolean`

Checks if the effect is supported. (Must be called after compilation)

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Materials/effect.ts:900

___

### key

• `get` **key**(): `string`

Unique key for this effect

#### Returns

`string`

#### Defined in

packages/dev/core/src/Materials/effect.ts:407

___

### onBindObservable

• `get` **onBindObservable**(): [`Observable`](Observable.md)[`Effect`](Effect.md)

Observable that will be called when effect is bound.

#### Returns

[`Observable`](Observable.md)[`Effect`](Effect.md)

#### Defined in

packages/dev/core/src/Materials/effect.ts:160

___

### rawFragmentSourceCode

• `get` **rawFragmentSourceCode**(): `string`

Gets the fragment shader source code before it has been processed by the preprocessor

#### Returns

`string`

#### Defined in

packages/dev/core/src/Materials/effect.ts:665

___

### rawVertexSourceCode

• `get` **rawVertexSourceCode**(): `string`

Gets the vertex shader source code before it has been processed by the preprocessor

#### Returns

`string`

#### Defined in

packages/dev/core/src/Materials/effect.ts:658

___

### vertexSourceCode

• `get` **vertexSourceCode**(): `string`

Gets the vertex shader source code of this effect

#### Returns

`string`

#### Defined in

packages/dev/core/src/Materials/effect.ts:640

___

### ShadersRepository

• `Static` `get` **ShadersRepository**(): `string`

Gets or sets the relative url used to load shaders if using the engine in non-minified mode

#### Returns

`string`

#### Defined in

packages/dev/core/src/Materials/effect.ts:96

• `Static` `set` **ShadersRepository**(`repo`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `repo` | `string` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/effect.ts:99

## Methods

### \_checkIsReady

▸ `Private` **_checkIsReady**(`previousPipelineContext`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `previousPipelineContext` | [`Nullable`](../modules.md#nullable)[`IPipelineContext`](../interfaces/IPipelineContext.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/effect.ts:570

___

### \_getShaderCodeAndErrorLine

▸ `Private` **_getShaderCodeAndErrorLine**(`code`, `error`, `isFragment`): [[`Nullable`](../modules.md#nullable)`string`, [`Nullable`](../modules.md#nullable)`string`]

#### Parameters

| Name | Type |
| :------ | :------ |
| `code` | [`Nullable`](../modules.md#nullable)`string` |
| `error` | [`Nullable`](../modules.md#nullable)`string` |
| `isFragment` | `boolean` |

#### Returns

[[`Nullable`](../modules.md#nullable)`string`, [`Nullable`](../modules.md#nullable)`string`]

#### Defined in

packages/dev/core/src/Materials/effect.ts:797

___

### \_isReadyInternal

▸ `Private` **_isReadyInternal**(): `boolean`

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Materials/effect.ts:423

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

packages/dev/core/src/Materials/effect.ts:589

___

### \_processCompilationErrors

▸ `Private` **_processCompilationErrors**(`e`, `previousPipelineContext?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `e` | `any` | `undefined` |
| `previousPipelineContext` | [`Nullable`](../modules.md#nullable)[`IPipelineContext`](../interfaces/IPipelineContext.md) | `null` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/effect.ts:816

___

### \_useFinalCode

▸ `Private` **_useFinalCode**(`migratedVertexCode`, `migratedFragmentCode`, `baseName`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `migratedVertexCode` | `string` |
| `migratedFragmentCode` | `string` |
| `baseName` | `any` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/effect.ts:390

___

### allFallbacksProcessed

▸ **allFallbacksProcessed**(): `boolean`

Gets a boolean indicating that all fallbacks were used during compilation

#### Returns

`boolean`

true if all fallbacks were used

#### Defined in

packages/dev/core/src/Materials/effect.ts:545

___

### bindUniformBlock

▸ **bindUniformBlock**(`blockName`, `index`): `void`

Binds block to a uniform.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `blockName` | `string` | Name of the block to bind. |
| `index` | `number` | Index to bind. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/effect.ts:995

___

### bindUniformBuffer

▸ **bindUniformBuffer**(`buffer`, `name`): `void`

Binds a buffer to a uniform.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `buffer` | [`DataBuffer`](DataBuffer.md) | Buffer to bind. |
| `name` | `string` | Name of the uniform variable to bind to. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/effect.ts:981

___

### dispose

▸ **dispose**(): `void`

Release all associated resources.

#### Returns

`void`

#### Implementation of

[IDisposable](../interfaces/IDisposable.md).[dispose](../interfaces/IDisposable.md#dispose)

#### Defined in

packages/dev/core/src/Materials/effect.ts:1369

___

### executeWhenCompiled

▸ **executeWhenCompiled**(`func`): `void`

Adds a callback to the onCompiled observable and call the callback immediately if already ready.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `func` | (`effect`: [`Effect`](Effect.md)) => `void` | The callback to be used. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/effect.ts:553

___

### getAttributeLocation

▸ **getAttributeLocation**(`index`): `number`

Returns the attribute at the given index.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | The index of the attribute. |

#### Returns

`number`

The location of the attribute.

#### Defined in

packages/dev/core/src/Materials/effect.ts:462

___

### getAttributeLocationByName

▸ **getAttributeLocationByName**(`name`): `number`

Returns the attribute based on the name of the variable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | of the attribute to look up. |

#### Returns

`number`

the attribute location.

#### Defined in

packages/dev/core/src/Materials/effect.ts:471

___

### getAttributesCount

▸ **getAttributesCount**(): `number`

The number of attributes.

#### Returns

`number`

the number of attributes.

#### Defined in

packages/dev/core/src/Materials/effect.ts:479

___

### getAttributesNames

▸ **getAttributesNames**(): `string`[]

The set of names of attribute variables for the shader.

#### Returns

`string`[]

An array of attribute names.

#### Defined in

packages/dev/core/src/Materials/effect.ts:453

___

### getCompilationError

▸ **getCompilationError**(): `string`

The error from the last compilation.

#### Returns

`string`

the error string.

#### Defined in

packages/dev/core/src/Materials/effect.ts:537

___

### getEngine

▸ **getEngine**(): [`Engine`](Engine.md)

The engine the effect was initialized with.

#### Returns

[`Engine`](Engine.md)

the engine.

#### Defined in

packages/dev/core/src/Materials/effect.ts:437

___

### getIndexParameters

▸ **getIndexParameters**(): `any`

Returns the index parameters used to create the effect

#### Returns

`any`

The index parameters object

#### Defined in

packages/dev/core/src/Materials/effect.ts:529

___

### getPipelineContext

▸ **getPipelineContext**(): [`Nullable`](../modules.md#nullable)[`IPipelineContext`](../interfaces/IPipelineContext.md)

The pipeline context for this effect

#### Returns

[`Nullable`](../modules.md#nullable)[`IPipelineContext`](../interfaces/IPipelineContext.md)

the associated pipeline context

#### Defined in

packages/dev/core/src/Materials/effect.ts:445

___

### getSamplers

▸ **getSamplers**(): `string`[]

Returns an array of sampler variable names

#### Returns

`string`[]

The array of sampler variable names.

#### Defined in

packages/dev/core/src/Materials/effect.ts:505

___

### getUniform

▸ **getUniform**(`uniformName`): [`Nullable`](../modules.md#nullable)`WebGLUniformLocation`

Returns the attribute based on the name of the variable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | of the uniform to look up. |

#### Returns

[`Nullable`](../modules.md#nullable)`WebGLUniformLocation`

the location of the uniform.

#### Defined in

packages/dev/core/src/Materials/effect.ts:497

___

### getUniformBuffersNames

▸ **getUniformBuffersNames**(): `string`[]

Returns an array of uniform buffer variable names

#### Returns

`string`[]

The array of uniform buffer variable names.

#### Defined in

packages/dev/core/src/Materials/effect.ts:521

___

### getUniformIndex

▸ **getUniformIndex**(`uniformName`): `number`

Gets the index of a uniform variable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | of the uniform to look up. |

#### Returns

`number`

the index.

#### Defined in

packages/dev/core/src/Materials/effect.ts:488

___

### getUniformNames

▸ **getUniformNames**(): `string`[]

Returns an array of uniform variable names

#### Returns

`string`[]

The array of uniform variable names.

#### Defined in

packages/dev/core/src/Materials/effect.ts:513

___

### isReady

▸ **isReady**(): `boolean`

If the effect has been compiled and prepared.

#### Returns

`boolean`

if the effect is compiled and prepared.

#### Defined in

packages/dev/core/src/Materials/effect.ts:415

___

### setArray

▸ **setArray**(`uniformName`, `array`): [`Effect`](Effect.md)

Sets an array on a uniform variable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `array` | `number`[] | array to be set. |

#### Returns

[`Effect`](Effect.md)

this effect.

#### Defined in

packages/dev/core/src/Materials/effect.ts:1143

___

### setArray2

▸ **setArray2**(`uniformName`, `array`): [`Effect`](Effect.md)

Sets an array 2 on a uniform variable. (Array is specified as single array eg. [1,2,3,4] will result in [[1,2],[3,4]] in the shader)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `array` | `number`[] | array to be set. |

#### Returns

[`Effect`](Effect.md)

this effect.

#### Defined in

packages/dev/core/src/Materials/effect.ts:1154

___

### setArray3

▸ **setArray3**(`uniformName`, `array`): [`Effect`](Effect.md)

Sets an array 3 on a uniform variable. (Array is specified as single array eg. [1,2,3,4,5,6] will result in [[1,2,3],[4,5,6]] in the shader)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `array` | `number`[] | array to be set. |

#### Returns

[`Effect`](Effect.md)

this effect.

#### Defined in

packages/dev/core/src/Materials/effect.ts:1165

___

### setArray4

▸ **setArray4**(`uniformName`, `array`): [`Effect`](Effect.md)

Sets an array 4 on a uniform variable. (Array is specified as single array eg. [1,2,3,4,5,6,7,8] will result in [[1,2,3,4],[5,6,7,8]] in the shader)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `array` | `number`[] | array to be set. |

#### Returns

[`Effect`](Effect.md)

this effect.

#### Defined in

packages/dev/core/src/Materials/effect.ts:1176

___

### setBool

▸ **setBool**(`uniformName`, `bool`): [`Effect`](Effect.md)

Sets a boolean on a uniform variable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `bool` | `boolean` | value to be set. |

#### Returns

[`Effect`](Effect.md)

this effect.

#### Defined in

packages/dev/core/src/Materials/effect.ts:1244

___

### setColor3

▸ **setColor3**(`uniformName`, `color3`): [`Effect`](Effect.md)

Sets a Color3 on a uniform variable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `color3` | `IColor3Like` | Value to be set. |

#### Returns

[`Effect`](Effect.md)

this effect.

#### Defined in

packages/dev/core/src/Materials/effect.ts:1338

___

### setColor4

▸ **setColor4**(`uniformName`, `color3`, `alpha`): [`Effect`](Effect.md)

Sets a Color4 on a uniform variable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `color3` | `IColor3Like` | Value to be set. |
| `alpha` | `number` | Alpha value to be set. |

#### Returns

[`Effect`](Effect.md)

this effect.

#### Defined in

packages/dev/core/src/Materials/effect.ts:1350

___

### setDepthStencilTexture

▸ **setDepthStencilTexture**(`channel`, `texture`): `void`

Sets a depth stencil texture from a render target on the engine to be used in the shader.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `channel` | `string` | Name of the sampler variable. |
| `texture` | [`Nullable`](../modules.md#nullable)[`RenderTargetTexture`](RenderTargetTexture.md) | Texture to set. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/effect.ts:928

___

### setDirectColor4

▸ **setDirectColor4**(`uniformName`, `color4`): [`Effect`](Effect.md)

Sets a Color4 on a uniform variable

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | defines the name of the variable |
| `color4` | `IColor4Like` | defines the value to be set |

#### Returns

[`Effect`](Effect.md)

this effect.

#### Defined in

packages/dev/core/src/Materials/effect.ts:1361

___

### setExternalTexture

▸ **setExternalTexture**(`name`, `texture`): `void`

Sets an external texture on the engine to be used in the shader.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Name of the external texture variable. |
| `texture` | [`Nullable`](../modules.md#nullable)[`ExternalTexture`](ExternalTexture.md) | Texture to set. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Engines/WebGPU/Extensions/engine.externalTexture.ts:14

___

### setFloat

▸ **setFloat**(`uniformName`, `value`): [`Effect`](Effect.md)

Sets a float on a uniform variable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `value` | `number` | value to be set. |

#### Returns

[`Effect`](Effect.md)

this effect.

#### Defined in

packages/dev/core/src/Materials/effect.ts:1233

___

### setFloat2

▸ **setFloat2**(`uniformName`, `x`, `y`): [`Effect`](Effect.md)

Sets a float2 on a uniform variable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `x` | `number` | First float in float2. |
| `y` | `number` | Second float in float2. |

#### Returns

[`Effect`](Effect.md)

this effect.

#### Defined in

packages/dev/core/src/Materials/effect.ts:1267

___

### setFloat3

▸ **setFloat3**(`uniformName`, `x`, `y`, `z`): [`Effect`](Effect.md)

Sets a float3 on a uniform variable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `x` | `number` | First float in float3. |
| `y` | `number` | Second float in float3. |
| `z` | `number` | Third float in float3. |

#### Returns

[`Effect`](Effect.md)

this effect.

#### Defined in

packages/dev/core/src/Materials/effect.ts:1291

___

### setFloat4

▸ **setFloat4**(`uniformName`, `x`, `y`, `z`, `w`): [`Effect`](Effect.md)

Sets a float4 on a uniform variable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `x` | `number` | First float in float4. |
| `y` | `number` | Second float in float4. |
| `z` | `number` | Third float in float4. |
| `w` | `number` | Fourth float in float4. |

#### Returns

[`Effect`](Effect.md)

this effect.

#### Defined in

packages/dev/core/src/Materials/effect.ts:1327

___

### setFloatArray

▸ **setFloatArray**(`uniformName`, `array`): [`Effect`](Effect.md)

Sets an float array on a uniform variable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `array` | [`FloatArray`](../modules.md#floatarray) | array to be set. |

#### Returns

[`Effect`](Effect.md)

this effect.

#### Defined in

packages/dev/core/src/Materials/effect.ts:1099

___

### setFloatArray2

▸ **setFloatArray2**(`uniformName`, `array`): [`Effect`](Effect.md)

Sets an float array 2 on a uniform variable. (Array is specified as single array eg. [1,2,3,4] will result in [[1,2],[3,4]] in the shader)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `array` | [`FloatArray`](../modules.md#floatarray) | array to be set. |

#### Returns

[`Effect`](Effect.md)

this effect.

#### Defined in

packages/dev/core/src/Materials/effect.ts:1110

___

### setFloatArray3

▸ **setFloatArray3**(`uniformName`, `array`): [`Effect`](Effect.md)

Sets an float array 3 on a uniform variable. (Array is specified as single array eg. [1,2,3,4,5,6] will result in [[1,2,3],[4,5,6]] in the shader)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `array` | [`FloatArray`](../modules.md#floatarray) | array to be set. |

#### Returns

[`Effect`](Effect.md)

this effect.

#### Defined in

packages/dev/core/src/Materials/effect.ts:1121

___

### setFloatArray4

▸ **setFloatArray4**(`uniformName`, `array`): [`Effect`](Effect.md)

Sets an float array 4 on a uniform variable. (Array is specified as single array eg. [1,2,3,4,5,6,7,8] will result in [[1,2,3,4],[5,6,7,8]] in the shader)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `array` | [`FloatArray`](../modules.md#floatarray) | array to be set. |

#### Returns

[`Effect`](Effect.md)

this effect.

#### Defined in

packages/dev/core/src/Materials/effect.ts:1132

___

### setInt

▸ **setInt**(`uniformName`, `value`): [`Effect`](Effect.md)

Sets an integer value on a uniform variable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `value` | `number` | Value to be set. |

#### Returns

[`Effect`](Effect.md)

this effect.

#### Defined in

packages/dev/core/src/Materials/effect.ts:1005

___

### setInt2

▸ **setInt2**(`uniformName`, `x`, `y`): [`Effect`](Effect.md)

Sets an int2 value on a uniform variable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `x` | `number` | First int in int2. |
| `y` | `number` | Second int in int2. |

#### Returns

[`Effect`](Effect.md)

this effect.

#### Defined in

packages/dev/core/src/Materials/effect.ts:1017

___

### setInt3

▸ **setInt3**(`uniformName`, `x`, `y`, `z`): [`Effect`](Effect.md)

Sets an int3 value on a uniform variable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `x` | `number` | First int in int3. |
| `y` | `number` | Second int in int3. |
| `z` | `number` | Third int in int3. |

#### Returns

[`Effect`](Effect.md)

this effect.

#### Defined in

packages/dev/core/src/Materials/effect.ts:1030

___

### setInt4

▸ **setInt4**(`uniformName`, `x`, `y`, `z`, `w`): [`Effect`](Effect.md)

Sets an int4 value on a uniform variable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `x` | `number` | First int in int4. |
| `y` | `number` | Second int in int4. |
| `z` | `number` | Third int in int4. |
| `w` | `number` | Fourth int in int4. |

#### Returns

[`Effect`](Effect.md)

this effect.

#### Defined in

packages/dev/core/src/Materials/effect.ts:1044

___

### setIntArray

▸ **setIntArray**(`uniformName`, `array`): [`Effect`](Effect.md)

Sets an int array on a uniform variable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `array` | `Int32Array` | array to be set. |

#### Returns

[`Effect`](Effect.md)

this effect.

#### Defined in

packages/dev/core/src/Materials/effect.ts:1055

___

### setIntArray2

▸ **setIntArray2**(`uniformName`, `array`): [`Effect`](Effect.md)

Sets an int array 2 on a uniform variable. (Array is specified as single array eg. [1,2,3,4] will result in [[1,2],[3,4]] in the shader)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `array` | `Int32Array` | array to be set. |

#### Returns

[`Effect`](Effect.md)

this effect.

#### Defined in

packages/dev/core/src/Materials/effect.ts:1066

___

### setIntArray3

▸ **setIntArray3**(`uniformName`, `array`): [`Effect`](Effect.md)

Sets an int array 3 on a uniform variable. (Array is specified as single array eg. [1,2,3,4,5,6] will result in [[1,2,3],[4,5,6]] in the shader)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `array` | `Int32Array` | array to be set. |

#### Returns

[`Effect`](Effect.md)

this effect.

#### Defined in

packages/dev/core/src/Materials/effect.ts:1077

___

### setIntArray4

▸ **setIntArray4**(`uniformName`, `array`): [`Effect`](Effect.md)

Sets an int array 4 on a uniform variable. (Array is specified as single array eg. [1,2,3,4,5,6,7,8] will result in [[1,2,3,4],[5,6,7,8]] in the shader)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `array` | `Int32Array` | array to be set. |

#### Returns

[`Effect`](Effect.md)

this effect.

#### Defined in

packages/dev/core/src/Materials/effect.ts:1088

___

### setMatrices

▸ **setMatrices**(`uniformName`, `matrices`): [`Effect`](Effect.md)

Sets matrices on a uniform variable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `matrices` | `number`[] \| `Float32Array` | matrices to be set. |

#### Returns

[`Effect`](Effect.md)

this effect.

#### Defined in

packages/dev/core/src/Materials/effect.ts:1187

___

### setMatrix

▸ **setMatrix**(`uniformName`, `matrix`): [`Effect`](Effect.md)

Sets matrix on a uniform variable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `matrix` | `IMatrixLike` | matrix to be set. |

#### Returns

[`Effect`](Effect.md)

this effect.

#### Defined in

packages/dev/core/src/Materials/effect.ts:1198

___

### setMatrix2x2

▸ **setMatrix2x2**(`uniformName`, `matrix`): [`Effect`](Effect.md)

Sets a 2x2 matrix on a uniform variable. (Specified as [1,2,3,4] will result in [1,2][3,4] matrix)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `matrix` | `number`[] \| `Float32Array` | matrix to be set. |

#### Returns

[`Effect`](Effect.md)

this effect.

#### Defined in

packages/dev/core/src/Materials/effect.ts:1221

___

### setMatrix3x3

▸ **setMatrix3x3**(`uniformName`, `matrix`): [`Effect`](Effect.md)

Sets a 3x3 matrix on a uniform variable. (Specified as [1,2,3,4,5,6,7,8,9] will result in [1,2,3][4,5,6][7,8,9] matrix)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `matrix` | `number`[] \| `Float32Array` | matrix to be set. |

#### Returns

[`Effect`](Effect.md)

this effect.

#### Defined in

packages/dev/core/src/Materials/effect.ts:1209

___

### setQuaternion

▸ **setQuaternion**(`uniformName`, `quaternion`): [`Effect`](Effect.md)

Sets a Quaternion on a uniform variable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `quaternion` | `IQuaternionLike` | Value to be set. |

#### Returns

[`Effect`](Effect.md)

this effect.

#### Defined in

packages/dev/core/src/Materials/effect.ts:1313

___

### setStorageBuffer

▸ **setStorageBuffer**(`name`, `buffer`): `void`

Sets a storage buffer on the engine to be used in the shader.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Name of the storage buffer variable. |
| `buffer` | [`Nullable`](../modules.md#nullable)[`StorageBuffer`](StorageBuffer.md) | Storage buffer to set. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Engines/WebGPU/Extensions/engine.storageBuffer.ts:18

___

### setTexture

▸ **setTexture**(`channel`, `texture`): `void`

Sets a texture on the engine to be used in the shader.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `channel` | `string` | Name of the sampler variable. |
| `texture` | [`Nullable`](../modules.md#nullable)[`ThinTexture`](ThinTexture.md) | Texture to set. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/effect.ts:919

___

### setTextureArray

▸ **setTextureArray**(`channel`, `textures`): `void`

Sets an array of textures on the engine to be used in the shader.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `channel` | `string` | Name of the variable. |
| `textures` | [`ThinTexture`](ThinTexture.md)[] | Textures to set. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/effect.ts:937

___

### setTextureFromPostProcess

▸ **setTextureFromPostProcess**(`channel`, `postProcess`): `void`

Sets a texture to be the input of the specified post process. (To use the output, pass in the next post process in the pipeline)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `channel` | `string` | Name of the sampler variable. |
| `postProcess` | [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md) | Post process to get the input texture from. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/effect.ts:962

___

### setTextureFromPostProcessOutput

▸ **setTextureFromPostProcessOutput**(`channel`, `postProcess`): `void`

(Warning! setTextureFromPostProcessOutput may be desired instead)
Sets the input texture of the passed in post process to be input of this effect. (To use the output of the passed in post process use setTextureFromPostProcessOutput)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `channel` | `string` | Name of the sampler variable. |
| `postProcess` | [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md) | Post process to get the output texture from. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/effect.ts:972

___

### setTextureSampler

▸ **setTextureSampler**(`name`, `sampler`): `void`

Sets a sampler on the engine to be used in the shader.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Name of the sampler variable. |
| `sampler` | [`Nullable`](../modules.md#nullable)[`TextureSampler`](TextureSampler.md) | Sampler to set. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Engines/WebGPU/Extensions/engine.textureSampler.ts:14

___

### setVector2

▸ **setVector2**(`uniformName`, `vector2`): [`Effect`](Effect.md)

Sets a Vector2 on a uniform variable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `vector2` | `IVector2Like` | vector2 to be set. |

#### Returns

[`Effect`](Effect.md)

this effect.

#### Defined in

packages/dev/core/src/Materials/effect.ts:1255

___

### setVector3

▸ **setVector3**(`uniformName`, `vector3`): [`Effect`](Effect.md)

Sets a Vector3 on a uniform variable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `vector3` | `IVector3Like` | Value to be set. |

#### Returns

[`Effect`](Effect.md)

this effect.

#### Defined in

packages/dev/core/src/Materials/effect.ts:1278

___

### setVector4

▸ **setVector4**(`uniformName`, `vector4`): [`Effect`](Effect.md)

Sets a Vector4 on a uniform variable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniformName` | `string` | Name of the variable. |
| `vector4` | `IVector4Like` | Value to be set. |

#### Returns

[`Effect`](Effect.md)

this effect.

#### Defined in

packages/dev/core/src/Materials/effect.ts:1302

___

### RegisterShader

▸ `Static` **RegisterShader**(`name`, `pixelShader?`, `vertexShader?`, `shaderLanguage?`): `void`

This function will add a new shader to the shader store

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | the name of the shader |
| `pixelShader?` | `string` | `undefined` | optional pixel shader content |
| `vertexShader?` | `string` | `undefined` | optional vertex shader content |
| `shaderLanguage` | [`ShaderLanguage`](../enums/ShaderLanguage.md) | `ShaderLanguage.GLSL` | the language the shader is written in (default: GLSL) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/effect.ts:1385

___

### ResetCache

▸ `Static` **ResetCache**(): `void`

Resets the cache of effects.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/effect.ts:1407
