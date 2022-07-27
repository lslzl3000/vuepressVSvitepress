[@dev/core](../README.md) / [Exports](../modules.md) / IComputeShaderOptions

# Interface: IComputeShaderOptions

Defines the options associated with the creation of a compute shader.

## Table of contents

### Properties

- [bindingsMapping](IComputeShaderOptions.md#bindingsmapping)
- [defines](IComputeShaderOptions.md#defines)
- [entryPoint](IComputeShaderOptions.md#entrypoint)
- [processFinalCode](IComputeShaderOptions.md#processfinalcode)

## Properties

### bindingsMapping

• **bindingsMapping**: [`ComputeBindingMapping`](../modules.md#computebindingmapping)

list of bindings mapping (key is property name, value is binding location)
Must be provided because browsers don't support reflection for wgsl shaders yet (so there's no way to query the binding/group from a variable name)
TODO: remove this when browsers support reflection for wgsl shaders

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeShader.ts:27

___

### defines

• `Optional` **defines**: `string`[]

The list of defines used in the shader

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeShader.ts:32

___

### entryPoint

• `Optional` **entryPoint**: `string`

The name of the entry point in the shader source (default: "main")

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeShader.ts:37

___

### processFinalCode

• `Optional` **processFinalCode**: [`Nullable`](../modules.md#nullable)(`code`: `string`) => `string`

If provided, will be called with the shader code so that this code can be updated before it is compiled by the GPU

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeShader.ts:42
