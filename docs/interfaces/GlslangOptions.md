[@dev/core](../README.md) / [Exports](../modules.md) / GlslangOptions

# Interface: GlslangOptions

Options to load the associated Glslang library

## Table of contents

### Properties

- [glslang](GlslangOptions.md#glslang)
- [jsPath](GlslangOptions.md#jspath)
- [wasmPath](GlslangOptions.md#wasmpath)

## Properties

### glslang

• `Optional` **glslang**: `any`

Defines an existing instance of Glslang (useful in modules who do not access the global instance).

#### Defined in

https://github.com/babylon.js/core/src/Engines/webgpuEngine.ts:73

___

### jsPath

• `Optional` **jsPath**: `string`

Defines the URL of the glslang JS File.

#### Defined in

https://github.com/babylon.js/core/src/Engines/webgpuEngine.ts:77

___

### wasmPath

• `Optional` **wasmPath**: `string`

Defines the URL of the glslang WASM File.

#### Defined in

https://github.com/babylon.js/core/src/Engines/webgpuEngine.ts:81
