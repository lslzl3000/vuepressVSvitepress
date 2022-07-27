[@dev/core](../README.md) / [Exports](../modules.md) / WebGPUEngineOptions

# Interface: WebGPUEngineOptions

Options to create the WebGPU engine

## Hierarchy

- `GPURequestAdapterOptions`

  ↳ **`WebGPUEngineOptions`**

## Table of contents

### Properties

- [adaptToDeviceRatio](WebGPUEngineOptions.md#adapttodeviceratio)
- [antialiasing](WebGPUEngineOptions.md#antialiasing)
- [audioEngine](WebGPUEngineOptions.md#audioengine)
- [deterministicLockstep](WebGPUEngineOptions.md#deterministiclockstep)
- [deviceDescriptor](WebGPUEngineOptions.md#devicedescriptor)
- [doNotHandleContextLost](WebGPUEngineOptions.md#donothandlecontextlost)
- [doNotHandleTouchAction](WebGPUEngineOptions.md#donothandletouchaction)
- [enableGPUDebugMarkers](WebGPUEngineOptions.md#enablegpudebugmarkers)
- [forceFallbackAdapter](WebGPUEngineOptions.md#forcefallbackadapter)
- [glslangOptions](WebGPUEngineOptions.md#glslangoptions)
- [limitDeviceRatio](WebGPUEngineOptions.md#limitdeviceratio)
- [lockstepMaxSteps](WebGPUEngineOptions.md#lockstepmaxsteps)
- [powerPreference](WebGPUEngineOptions.md#powerpreference)
- [premultipliedAlpha](WebGPUEngineOptions.md#premultipliedalpha)
- [stencil](WebGPUEngineOptions.md#stencil)
- [swapChainFormat](WebGPUEngineOptions.md#swapchainformat)
- [timeStep](WebGPUEngineOptions.md#timestep)
- [twgslOptions](WebGPUEngineOptions.md#twgsloptions)
- [useHighPrecisionMatrix](WebGPUEngineOptions.md#usehighprecisionmatrix)

## Properties

### adaptToDeviceRatio

• `Optional` **adaptToDeviceRatio**: `boolean`

Defines whether to adapt to the device's viewport characteristics (default: false)

#### Defined in

https://github.com/babylon.js/core/src/Engines/webgpuEngine.ts:173

___

### antialiasing

• `Optional` **antialiasing**: `boolean`

Defines whether MSAA is enabled on the canvas.

#### Defined in

https://github.com/babylon.js/core/src/Engines/webgpuEngine.ts:142

___

### audioEngine

• `Optional` **audioEngine**: `boolean`

Defines if webaudio should be initialized as well

**`See`**

http://doc.babylonjs.com/how_to/playing_sounds_and_music

#### Defined in

https://github.com/babylon.js/core/src/Engines/webgpuEngine.ts:121

___

### deterministicLockstep

• `Optional` **deterministicLockstep**: `boolean`

If delta time between frames should be constant

**`See`**

https://doc.babylonjs.com/babylon101/animations#deterministic-lockstep

#### Defined in

https://github.com/babylon.js/core/src/Engines/webgpuEngine.ts:92

___

### deviceDescriptor

• `Optional` **deviceDescriptor**: `GPUDeviceDescriptor`

Defines the device descriptor used to create a device.

#### Defined in

https://github.com/babylon.js/core/src/Engines/webgpuEngine.ts:132

___

### doNotHandleContextLost

• `Optional` **doNotHandleContextLost**: `boolean`

Defines that engine should ignore context lost events
If this event happens when this parameter is true, you will have to reload the page to restore rendering

#### Defined in

https://github.com/babylon.js/core/src/Engines/webgpuEngine.ts:109

___

### doNotHandleTouchAction

• `Optional` **doNotHandleTouchAction**: `boolean`

Defines that engine should ignore modifying touch action attribute and style
If not handle, you might need to set it up on your side for expected touch devices behavior.

#### Defined in

https://github.com/babylon.js/core/src/Engines/webgpuEngine.ts:115

___

### enableGPUDebugMarkers

• `Optional` **enableGPUDebugMarkers**: `boolean`

Defines whether we should generate debug markers in the gpu command lists (can be seen with PIX for eg)

#### Defined in

https://github.com/babylon.js/core/src/Engines/webgpuEngine.ts:152

___

### forceFallbackAdapter

• `Optional` **forceFallbackAdapter**: `boolean`

#### Inherited from

GPURequestAdapterOptions.forceFallbackAdapter

#### Defined in

https://github.com/babylon.js/core/src/LibDeclarations/webgpu.d.ts:58

___

### glslangOptions

• `Optional` **glslangOptions**: [`GlslangOptions`](GlslangOptions.md)

Options to load the associated Glslang library

#### Defined in

https://github.com/babylon.js/core/src/Engines/webgpuEngine.ts:157

___

### limitDeviceRatio

• `Optional` **limitDeviceRatio**: `number`

Defines if the engine should no exceed a specified device ratio

**`See`**

https://developer.mozilla.org/en-US/docs/Web/API/Window/devicePixelRatio

#### Defined in

https://github.com/babylon.js/core/src/Engines/webgpuEngine.ts:168

___

### lockstepMaxSteps

• `Optional` **lockstepMaxSteps**: `number`

Maximum about of steps between frames (Default: 4)

**`See`**

https://doc.babylonjs.com/babylon101/animations#deterministic-lockstep

#### Defined in

https://github.com/babylon.js/core/src/Engines/webgpuEngine.ts:98

___

### powerPreference

• `Optional` **powerPreference**: `GPUPowerPreference`

Defines the category of adapter to use.
Is it the discrete or integrated device.

#### Overrides

GPURequestAdapterOptions.powerPreference

#### Defined in

https://github.com/babylon.js/core/src/Engines/webgpuEngine.ts:127

___

### premultipliedAlpha

• `Optional` **premultipliedAlpha**: `boolean`

Defines whether the canvas should be created in "premultiplied" mode (if false, the canvas is created in the "opaque" mode) (true by default)

#### Defined in

https://github.com/babylon.js/core/src/Engines/webgpuEngine.ts:178

___

### stencil

• `Optional` **stencil**: `boolean`

Defines whether the stencil buffer should be enabled.

#### Defined in

https://github.com/babylon.js/core/src/Engines/webgpuEngine.ts:147

___

### swapChainFormat

• `Optional` **swapChainFormat**: `GPUTextureFormat`

Defines the requested Swap Chain Format.

#### Defined in

https://github.com/babylon.js/core/src/Engines/webgpuEngine.ts:137

___

### timeStep

• `Optional` **timeStep**: `number`

Defines the seconds between each deterministic lock step

#### Defined in

https://github.com/babylon.js/core/src/Engines/webgpuEngine.ts:103

___

### twgslOptions

• `Optional` **twgslOptions**: [`TwgslOptions`](TwgslOptions.md)

Options to load the associated Twgsl library

#### Defined in

https://github.com/babylon.js/core/src/Engines/webgpuEngine.ts:162

___

### useHighPrecisionMatrix

• `Optional` **useHighPrecisionMatrix**: `boolean`

Make the matrix computations to be performed in 64 bits instead of 32 bits. False by default

#### Defined in

https://github.com/babylon.js/core/src/Engines/webgpuEngine.ts:183
