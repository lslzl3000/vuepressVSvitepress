[@dev/core](../README.md) / [Exports](../modules.md) / ICustomShaderNameResolveOptions

# Interface: ICustomShaderNameResolveOptions

Options passed when calling customShaderNameResolve

## Table of contents

### Properties

- [processFinalCode](ICustomShaderNameResolveOptions.md#processfinalcode)

## Properties

### processFinalCode

• `Optional` **processFinalCode**: [`Nullable`](../modules.md#nullable)`ShaderCustomProcessingFunction`

If provided, will be called two times with the vertex and fragment code so that this code can be updated before it is compiled by the GPU

#### Defined in

https://github.com/babylon.js/core/src/Materials/material.ts:77
