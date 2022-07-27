[@dev/core](../README.md) / [Exports](../modules.md) / IComputeEffectCreationOptions

# Interface: IComputeEffectCreationOptions

Options to be used when creating a compute effect.

## Table of contents

### Properties

- [defines](IComputeEffectCreationOptions.md#defines)
- [entryPoint](IComputeEffectCreationOptions.md#entrypoint)
- [onCompiled](IComputeEffectCreationOptions.md#oncompiled)
- [onError](IComputeEffectCreationOptions.md#onerror)
- [processFinalCode](IComputeEffectCreationOptions.md#processfinalcode)

## Properties

### defines

• **defines**: `any`

Define statements that will be set in the shader.

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeEffect.ts:20

___

### entryPoint

• `Optional` **entryPoint**: `string`

The name of the entry point in the shader source (default: "main")

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeEffect.ts:24

___

### onCompiled

• **onCompiled**: [`Nullable`](../modules.md#nullable)(`effect`: [`ComputeEffect`](../classes/ComputeEffect.md)) => `void`

Callback that will be called when the shader is compiled.

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeEffect.ts:28

___

### onError

• **onError**: [`Nullable`](../modules.md#nullable)(`effect`: [`ComputeEffect`](../classes/ComputeEffect.md), `errors`: `string`) => `void`

Callback that will be called if an error occurs during shader compilation.

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeEffect.ts:32

___

### processFinalCode

• `Optional` **processFinalCode**: [`Nullable`](../modules.md#nullable)(`code`: `string`) => `string`

If provided, will be called with the shader code so that this code can be updated before it is compiled by the GPU

#### Defined in

https://github.com/babylon.js/core/src/Compute/computeEffect.ts:36
