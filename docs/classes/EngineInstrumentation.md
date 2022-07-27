[@dev/core](../README.md) / [Exports](../modules.md) / EngineInstrumentation

# Class: EngineInstrumentation

This class can be used to get instrumentation data from a Babylon engine

**`See`**

https://doc.babylonjs.com/how_to/optimizing_your_scene#engineinstrumentation

## Implements

- [`IDisposable`](../interfaces/IDisposable.md)

## Table of contents

### Constructors

- [constructor](EngineInstrumentation.md#constructor)

### Properties

- [\_captureGPUFrameTime](EngineInstrumentation.md#_capturegpuframetime)
- [\_captureShaderCompilationTime](EngineInstrumentation.md#_captureshadercompilationtime)
- [\_onAfterShaderCompilationObserver](EngineInstrumentation.md#_onaftershadercompilationobserver)
- [\_onBeforeShaderCompilationObserver](EngineInstrumentation.md#_onbeforeshadercompilationobserver)
- [\_onBeginFrameObserver](EngineInstrumentation.md#_onbeginframeobserver)
- [\_onEndFrameObserver](EngineInstrumentation.md#_onendframeobserver)
- [\_shaderCompilationTime](EngineInstrumentation.md#_shadercompilationtime)
- [engine](EngineInstrumentation.md#engine)

### Accessors

- [captureGPUFrameTime](EngineInstrumentation.md#capturegpuframetime)
- [captureShaderCompilationTime](EngineInstrumentation.md#captureshadercompilationtime)
- [gpuFrameTimeCounter](EngineInstrumentation.md#gpuframetimecounter)
- [shaderCompilationTimeCounter](EngineInstrumentation.md#shadercompilationtimecounter)

### Methods

- [dispose](EngineInstrumentation.md#dispose)

## Constructors

### constructor

• **new EngineInstrumentation**(`engine`)

Instantiates a new engine instrumentation.
This class can be used to get instrumentation data from a Babylon engine

**`See`**

https://doc.babylonjs.com/how_to/optimizing_your_scene#engineinstrumentation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `engine` | [`Engine`](Engine.md) | Defines the engine to instrument |

#### Defined in

packages/dev/core/src/Instrumentation/engineInstrumentation.ts:96

## Properties

### \_captureGPUFrameTime

• `Private` **\_captureGPUFrameTime**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Instrumentation/engineInstrumentation.ts:11

___

### \_captureShaderCompilationTime

• `Private` **\_captureShaderCompilationTime**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Instrumentation/engineInstrumentation.ts:13

___

### \_onAfterShaderCompilationObserver

• `Private` **\_onAfterShaderCompilationObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Engine`](Engine.md) = `null`

#### Defined in

packages/dev/core/src/Instrumentation/engineInstrumentation.ts:20

___

### \_onBeforeShaderCompilationObserver

• `Private` **\_onBeforeShaderCompilationObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Engine`](Engine.md) = `null`

#### Defined in

packages/dev/core/src/Instrumentation/engineInstrumentation.ts:19

___

### \_onBeginFrameObserver

• `Private` **\_onBeginFrameObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Engine`](Engine.md) = `null`

#### Defined in

packages/dev/core/src/Instrumentation/engineInstrumentation.ts:17

___

### \_onEndFrameObserver

• `Private` **\_onEndFrameObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Engine`](Engine.md) = `null`

#### Defined in

packages/dev/core/src/Instrumentation/engineInstrumentation.ts:18

___

### \_shaderCompilationTime

• `Private` **\_shaderCompilationTime**: [`PerfCounter`](PerfCounter.md)

#### Defined in

packages/dev/core/src/Instrumentation/engineInstrumentation.ts:14

___

### engine

• **engine**: [`Engine`](Engine.md)

#### Defined in

packages/dev/core/src/Instrumentation/engineInstrumentation.ts:100

## Accessors

### captureGPUFrameTime

• `get` **captureGPUFrameTime**(): `boolean`

Gets the GPU frame time capture status

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Instrumentation/engineInstrumentation.ts:33

• `set` **captureGPUFrameTime**(`value`): `void`

Enable or disable the GPU frame time capture

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Instrumentation/engineInstrumentation.ts:40

___

### captureShaderCompilationTime

• `get` **captureShaderCompilationTime**(): `boolean`

Gets the shader compilation time capture status

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Instrumentation/engineInstrumentation.ts:59

• `set` **captureShaderCompilationTime**(`value`): `void`

Enable or disable the shader compilation time capture

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Instrumentation/engineInstrumentation.ts:66

___

### gpuFrameTimeCounter

• `get` **gpuFrameTimeCounter**(): [`PerfCounter`](PerfCounter.md)

Gets the perf counter used for GPU frame time

#### Returns

[`PerfCounter`](PerfCounter.md)

#### Defined in

packages/dev/core/src/Instrumentation/engineInstrumentation.ts:26

___

### shaderCompilationTimeCounter

• `get` **shaderCompilationTimeCounter**(): [`PerfCounter`](PerfCounter.md)

Gets the perf counter used for shader compilation time

#### Returns

[`PerfCounter`](PerfCounter.md)

#### Defined in

packages/dev/core/src/Instrumentation/engineInstrumentation.ts:52

## Methods

### dispose

▸ **dispose**(): `void`

Dispose and release associated resources.

#### Returns

`void`

#### Implementation of

[IDisposable](../interfaces/IDisposable.md).[dispose](../interfaces/IDisposable.md#dispose)

#### Defined in

packages/dev/core/src/Instrumentation/engineInstrumentation.ts:106
