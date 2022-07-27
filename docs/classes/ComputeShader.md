[@dev/core](../README.md) / [Exports](../modules.md) / ComputeShader

# Class: ComputeShader

The ComputeShader object lets you execute a compute shader on your GPU (if supported by the engine)

## Table of contents

### Constructors

- [constructor](ComputeShader.md#constructor)

### Properties

- [\_bindings](ComputeShader.md#_bindings)
- [\_cachedDefines](ComputeShader.md#_cacheddefines)
- [\_context](ComputeShader.md#_context)
- [\_contextIsDirty](ComputeShader.md#_contextisdirty)
- [\_effect](ComputeShader.md#_effect)
- [\_engine](ComputeShader.md#_engine)
- [\_options](ComputeShader.md#_options)
- [\_samplers](ComputeShader.md#_samplers)
- [\_shaderPath](ComputeShader.md#_shaderpath)
- [name](ComputeShader.md#name)
- [onCompiled](ComputeShader.md#oncompiled)
- [onError](ComputeShader.md#onerror)
- [uniqueId](ComputeShader.md#uniqueid)

### Accessors

- [options](ComputeShader.md#options)
- [shaderPath](ComputeShader.md#shaderpath)

### Methods

- [dispatch](ComputeShader.md#dispatch)
- [dispatchWhenReady](ComputeShader.md#dispatchwhenready)
- [getClassName](ComputeShader.md#getclassname)
- [isReady](ComputeShader.md#isready)
- [serialize](ComputeShader.md#serialize)
- [setStorageBuffer](ComputeShader.md#setstoragebuffer)
- [setStorageTexture](ComputeShader.md#setstoragetexture)
- [setTexture](ComputeShader.md#settexture)
- [setTextureSampler](ComputeShader.md#settexturesampler)
- [setUniformBuffer](ComputeShader.md#setuniformbuffer)
- [Parse](ComputeShader.md#parse)

## Constructors

### constructor

• **new ComputeShader**(`name`, `engine`, `shaderPath`, `options?`)

Instantiates a new compute shader.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Defines the name of the compute shader in the scene |
| `engine` | [`ThinEngine`](ThinEngine.md) | Defines the engine the compute shader belongs to |
| `shaderPath` | `any` | Defines  the route to the shader code in one of three ways:   * object: { compute: "custom" }, used with ShaderStore.ShadersStoreWGSL["customComputeShader"]   * object: { computeElement: "HTMLElementId" }, used with shader code in script tags   * object: { computeSource: "compute shader code string" using with string containing the shader code   * string: try first to find the code in ShaderStore.ShadersStoreWGSL[shaderPath + "ComputeShader"]. If not, assumes it is a file with name shaderPath.compute.fx in index.html folder. |
| `options` | `Partial`[`IComputeShaderOptions`](../interfaces/IComputeShaderOptions.md) | Define the options used to create the shader |

#### Defined in

packages/dev/core/src/Compute/computeShader.ts:105

## Properties

### \_bindings

• `Private` **\_bindings**: `ComputeBindingList` = `{}`

#### Defined in

packages/dev/core/src/Compute/computeShader.ts:54

___

### \_cachedDefines

• `Private` **\_cachedDefines**: `string`

#### Defined in

packages/dev/core/src/Compute/computeShader.ts:53

___

### \_context

• `Private` **\_context**: `IComputeContext`

#### Defined in

packages/dev/core/src/Compute/computeShader.ts:56

___

### \_contextIsDirty

• `Private` **\_contextIsDirty**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Compute/computeShader.ts:57

___

### \_effect

• `Private` **\_effect**: [`ComputeEffect`](ComputeEffect.md)

#### Defined in

packages/dev/core/src/Compute/computeShader.ts:52

___

### \_engine

• `Private` **\_engine**: [`ThinEngine`](ThinEngine.md)

#### Defined in

packages/dev/core/src/Compute/computeShader.ts:49

___

### \_options

• `Private` **\_options**: [`IComputeShaderOptions`](../interfaces/IComputeShaderOptions.md)

#### Defined in

packages/dev/core/src/Compute/computeShader.ts:51

___

### \_samplers

• `Private` **\_samplers**: `Object` = `{}`

#### Index signature

▪ [key: `string`]: [`TextureSampler`](TextureSampler.md)

#### Defined in

packages/dev/core/src/Compute/computeShader.ts:55

___

### \_shaderPath

• `Private` **\_shaderPath**: `any`

#### Defined in

packages/dev/core/src/Compute/computeShader.ts:50

___

### name

• **name**: `string`

The name of the shader

#### Defined in

packages/dev/core/src/Compute/computeShader.ts:68

___

### onCompiled

• **onCompiled**: [`Nullable`](../modules.md#nullable)(`effect`: [`ComputeEffect`](ComputeEffect.md)) => `void` = `null`

Callback triggered when the shader is compiled

#### Defined in

packages/dev/core/src/Compute/computeShader.ts:87

___

### onError

• **onError**: [`Nullable`](../modules.md#nullable)(`effect`: [`ComputeEffect`](ComputeEffect.md), `errors`: `string`) => `void` = `null`

Callback triggered when an error occurs

#### Defined in

packages/dev/core/src/Compute/computeShader.ts:92

___

### uniqueId

• `Readonly` **uniqueId**: `number`

Gets the unique id of the compute shader

#### Defined in

packages/dev/core/src/Compute/computeShader.ts:62

## Accessors

### options

• `get` **options**(): [`IComputeShaderOptions`](../interfaces/IComputeShaderOptions.md)

The options used to create the shader

#### Returns

[`IComputeShaderOptions`](../interfaces/IComputeShaderOptions.md)

#### Defined in

packages/dev/core/src/Compute/computeShader.ts:73

___

### shaderPath

• `get` **shaderPath**(): `any`

The shaderPath used to create the shader

#### Returns

`any`

#### Defined in

packages/dev/core/src/Compute/computeShader.ts:80

## Methods

### dispatch

▸ **dispatch**(`x`, `y?`, `z?`): `boolean`

Dispatches (executes) the compute shader

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | Number of workgroups to execute on the X dimension |
| `y?` | `number` | Number of workgroups to execute on the Y dimension (default: 1) |
| `z?` | `number` | Number of workgroups to execute on the Z dimension (default: 1) |

#### Returns

`boolean`

True if the dispatch could be done, else false (meaning either the compute effect or at least one of the bound resources was not ready)

#### Defined in

packages/dev/core/src/Compute/computeShader.ts:287

___

### dispatchWhenReady

▸ **dispatchWhenReady**(`x`, `y?`, `z?`, `delay?`): `Promise``void`

Waits for the compute shader to be ready and executes it

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `x` | `number` | `undefined` | Number of workgroups to execute on the X dimension |
| `y?` | `number` | `undefined` | Number of workgroups to execute on the Y dimension (default: 1) |
| `z?` | `number` | `undefined` | Number of workgroups to execute on the Z dimension (default: 1) |
| `delay` | `number` | `10` | Delay between the retries while the shader is not ready (in milliseconds - 10 by default) |

#### Returns

`Promise``void`

A promise that is resolved once the shader has been sent to the GPU. Note that it does not mean that the shader execution itself is finished!

#### Defined in

packages/dev/core/src/Compute/computeShader.ts:339

___

### getClassName

▸ **getClassName**(): `string`

Gets the current class name of the material e.g. "ComputeShader"
Mainly use in serialization.

#### Returns

`string`

the class name

#### Defined in

packages/dev/core/src/Compute/computeShader.ts:133

___

### isReady

▸ **isReady**(): `boolean`

Specifies that the compute shader is ready to be executed (the compute effect and all the resources are ready)

#### Returns

`boolean`

true if the compute shader is ready to be executed

#### Defined in

packages/dev/core/src/Compute/computeShader.ts:227

___

### serialize

▸ **serialize**(): `any`

Serializes this compute shader in a JSON representation

#### Returns

`any`

the serialized compute shader object

#### Defined in

packages/dev/core/src/Compute/computeShader.ts:357

___

### setStorageBuffer

▸ **setStorageBuffer**(`name`, `buffer`): `void`

Binds a storage buffer to the shader

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Binding name of the buffer |
| `buffer` | [`StorageBuffer`](StorageBuffer.md) | Buffer to bind |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Compute/computeShader.ts:194

___

### setStorageTexture

▸ **setStorageTexture**(`name`, `texture`): `void`

Binds a storage texture to the shader

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Binding name of the texture |
| `texture` | [`BaseTexture`](BaseTexture.md) | Texture to bind |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Compute/computeShader.ts:160

___

### setTexture

▸ **setTexture**(`name`, `texture`, `bindSampler?`): `void`

Binds a texture to the shader

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | Binding name of the texture |
| `texture` | [`BaseTexture`](BaseTexture.md) | `undefined` | Texture to bind |
| `bindSampler` | `boolean` | `true` | Bind the sampler corresponding to the texture (default: true). The sampler will be bound just before the binding index of the texture |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Compute/computeShader.ts:143

___

### setTextureSampler

▸ **setTextureSampler**(`name`, `sampler`): `void`

Binds a texture sampler to the shader

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Binding name of the sampler |
| `sampler` | [`TextureSampler`](TextureSampler.md) | Sampler to bind |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Compute/computeShader.ts:211

___

### setUniformBuffer

▸ **setUniformBuffer**(`name`, `buffer`): `void`

Binds a uniform buffer to the shader

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Binding name of the buffer |
| `buffer` | [`UniformBuffer`](UniformBuffer.md) | Buffer to bind |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Compute/computeShader.ts:177

___

### Parse

▸ `Static` **Parse**(`source`, `scene`, `rootUrl`): [`ComputeShader`](ComputeShader.md)

Creates a compute shader from parsed compute shader data

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | `any` | defines the JSON representation of the compute shader |
| `scene` | [`Scene`](Scene.md) | defines the hosting scene |
| `rootUrl` | `string` | defines the root URL to use to load textures and relative dependencies |

#### Returns

[`ComputeShader`](ComputeShader.md)

a new compute shader

#### Defined in

packages/dev/core/src/Compute/computeShader.ts:399
