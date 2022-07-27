[@dev/core](../README.md) / [Exports](../modules.md) / IEffectCreationOptions

# Interface: IEffectCreationOptions

Options to be used when creating an effect.

## Table of contents

### Properties

- [attributes](IEffectCreationOptions.md#attributes)
- [defines](IEffectCreationOptions.md#defines)
- [fallbacks](IEffectCreationOptions.md#fallbacks)
- [indexParameters](IEffectCreationOptions.md#indexparameters)
- [maxSimultaneousLights](IEffectCreationOptions.md#maxsimultaneouslights)
- [multiTarget](IEffectCreationOptions.md#multitarget)
- [onCompiled](IEffectCreationOptions.md#oncompiled)
- [onError](IEffectCreationOptions.md#onerror)
- [processCodeAfterIncludes](IEffectCreationOptions.md#processcodeafterincludes)
- [processFinalCode](IEffectCreationOptions.md#processfinalcode)
- [samplers](IEffectCreationOptions.md#samplers)
- [shaderLanguage](IEffectCreationOptions.md#shaderlanguage)
- [transformFeedbackVaryings](IEffectCreationOptions.md#transformfeedbackvaryings)
- [uniformBuffersNames](IEffectCreationOptions.md#uniformbuffersnames)
- [uniformsNames](IEffectCreationOptions.md#uniformsnames)

## Properties

### attributes

• **attributes**: `string`[]

Attributes that will be used in the shader.

#### Defined in

https://github.com/babylon.js/core/src/Materials/effect.ts:30

___

### defines

• **defines**: `any`

Define statements that will be set in the shader.

#### Defined in

https://github.com/babylon.js/core/src/Materials/effect.ts:46

___

### fallbacks

• **fallbacks**: [`Nullable`](../modules.md#nullable)[`IEffectFallbacks`](IEffectFallbacks.md)

Possible fallbacks for this effect to improve performance when needed.

#### Defined in

https://github.com/babylon.js/core/src/Materials/effect.ts:50

___

### indexParameters

• `Optional` **indexParameters**: `any`

Parameters to be used with Babylons include syntax to iterate over an array (eg. {lights: 10})

#### Defined in

https://github.com/babylon.js/core/src/Materials/effect.ts:62

___

### maxSimultaneousLights

• `Optional` **maxSimultaneousLights**: `number`

Max number of lights that can be used in the shader.

#### Defined in

https://github.com/babylon.js/core/src/Materials/effect.ts:66

___

### multiTarget

• `Optional` **multiTarget**: `boolean`

Is this effect rendering to several color attachments ?

#### Defined in

https://github.com/babylon.js/core/src/Materials/effect.ts:82

___

### onCompiled

• **onCompiled**: [`Nullable`](../modules.md#nullable)(`effect`: [`Effect`](../classes/Effect.md)) => `void`

Callback that will be called when the shader is compiled.

#### Defined in

https://github.com/babylon.js/core/src/Materials/effect.ts:54

___

### onError

• **onError**: [`Nullable`](../modules.md#nullable)(`effect`: [`Effect`](../classes/Effect.md), `errors`: `string`) => `void`

Callback that will be called if an error occurs during shader compilation.

#### Defined in

https://github.com/babylon.js/core/src/Materials/effect.ts:58

___

### processCodeAfterIncludes

• `Optional` **processCodeAfterIncludes**: [`Nullable`](../modules.md#nullable)`ShaderCustomProcessingFunction`

If provided, will be called two times with the vertex and fragment code so that this code can be updated after the #include have been processed

#### Defined in

https://github.com/babylon.js/core/src/Materials/effect.ts:78

___

### processFinalCode

• `Optional` **processFinalCode**: [`Nullable`](../modules.md#nullable)`ShaderCustomProcessingFunction`

If provided, will be called two times with the vertex and fragment code so that this code can be updated before it is compiled by the GPU

#### Defined in

https://github.com/babylon.js/core/src/Materials/effect.ts:74

___

### samplers

• **samplers**: `string`[]

Sampler texture variable names that will be set in the shader.

#### Defined in

https://github.com/babylon.js/core/src/Materials/effect.ts:42

___

### shaderLanguage

• `Optional` **shaderLanguage**: [`ShaderLanguage`](../enums/ShaderLanguage.md)

The language the shader is written in (default: GLSL)

#### Defined in

https://github.com/babylon.js/core/src/Materials/effect.ts:86

___

### transformFeedbackVaryings

• `Optional` **transformFeedbackVaryings**: [`Nullable`](../modules.md#nullable)`string`[]

See https://developer.mozilla.org/en-US/docs/Web/API/WebGL2RenderingContext/transformFeedbackVaryings

#### Defined in

https://github.com/babylon.js/core/src/Materials/effect.ts:70

___

### uniformBuffersNames

• **uniformBuffersNames**: `string`[]

Uniform buffer variable names that will be set in the shader.

#### Defined in

https://github.com/babylon.js/core/src/Materials/effect.ts:38

___

### uniformsNames

• **uniformsNames**: `string`[]

Uniform variable names that will be set in the shader.

#### Defined in

https://github.com/babylon.js/core/src/Materials/effect.ts:34
