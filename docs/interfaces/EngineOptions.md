[@dev/core](../README.md) / [Exports](../modules.md) / EngineOptions

# Interface: EngineOptions

Interface defining initialization parameters for Engine class

## Hierarchy

- `WebGLContextAttributes`

  ↳ **`EngineOptions`**

## Table of contents

### Properties

- [adaptToDeviceRatio](EngineOptions.md#adapttodeviceratio)
- [alpha](EngineOptions.md#alpha)
- [antialias](EngineOptions.md#antialias)
- [audioEngine](EngineOptions.md#audioengine)
- [audioEngineOptions](EngineOptions.md#audioengineoptions)
- [autoEnableWebVR](EngineOptions.md#autoenablewebvr)
- [depth](EngineOptions.md#depth)
- [desynchronized](EngineOptions.md#desynchronized)
- [deterministicLockstep](EngineOptions.md#deterministiclockstep)
- [disableWebGL2Support](EngineOptions.md#disablewebgl2support)
- [doNotHandleContextLost](EngineOptions.md#donothandlecontextlost)
- [doNotHandleTouchAction](EngineOptions.md#donothandletouchaction)
- [failIfMajorPerformanceCaveat](EngineOptions.md#failifmajorperformancecaveat)
- [forceSRGBBufferSupportState](EngineOptions.md#forcesrgbbuffersupportstate)
- [limitDeviceRatio](EngineOptions.md#limitdeviceratio)
- [lockstepMaxSteps](EngineOptions.md#lockstepmaxsteps)
- [powerPreference](EngineOptions.md#powerpreference)
- [premultipliedAlpha](EngineOptions.md#premultipliedalpha)
- [preserveDrawingBuffer](EngineOptions.md#preservedrawingbuffer)
- [stencil](EngineOptions.md#stencil)
- [timeStep](EngineOptions.md#timestep)
- [useExactSrgbConversions](EngineOptions.md#useexactsrgbconversions)
- [useHighPrecisionFloats](EngineOptions.md#usehighprecisionfloats)
- [useHighPrecisionMatrix](EngineOptions.md#usehighprecisionmatrix)
- [xrCompatible](EngineOptions.md#xrcompatible)

## Properties

### adaptToDeviceRatio

• `Optional` **adaptToDeviceRatio**: `boolean`

Defines whether to adapt to the device's viewport characteristics (default: false)

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:160

___

### alpha

• `Optional` **alpha**: `boolean`

#### Inherited from

WebGLContextAttributes.alpha

#### Defined in

node_modules/typescript/lib/lib.dom.d.ts:1789

___

### antialias

• `Optional` **antialias**: `boolean`

#### Inherited from

WebGLContextAttributes.antialias

#### Defined in

node_modules/typescript/lib/lib.dom.d.ts:1790

___

### audioEngine

• `Optional` **audioEngine**: `boolean`

Defines if webaudio should be initialized as well

**`See`**

https://doc.babylonjs.com/how_to/playing_sounds_and_music

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:113

___

### audioEngineOptions

• `Optional` **audioEngineOptions**: `IAudioEngineOptions`

Specifies options for the audio engine

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:117

___

### autoEnableWebVR

• `Optional` **autoEnableWebVR**: `boolean`

Defines if webvr should be enabled automatically

**`See`**

https://doc.babylonjs.com/how_to/webvr_camera

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:103

___

### depth

• `Optional` **depth**: `boolean`

#### Inherited from

WebGLContextAttributes.depth

#### Defined in

node_modules/typescript/lib/lib.dom.d.ts:1791

___

### desynchronized

• `Optional` **desynchronized**: `boolean`

#### Inherited from

WebGLContextAttributes.desynchronized

#### Defined in

node_modules/typescript/lib/lib.dom.d.ts:1792

___

### deterministicLockstep

• `Optional` **deterministicLockstep**: `boolean`

Defines if animations should run using a deterministic lock step

**`See`**

https://doc.babylonjs.com/babylon101/animations#deterministic-lockstep

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:123

___

### disableWebGL2Support

• `Optional` **disableWebGL2Support**: `boolean`

Defines if webgl2 should be turned off even if supported

**`See`**

https://doc.babylonjs.com/features/webgl2

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:108

___

### doNotHandleContextLost

• `Optional` **doNotHandleContextLost**: `boolean`

Defines that engine should ignore context lost events
If this event happens when this parameter is true, you will have to reload the page to restore rendering

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:132

___

### doNotHandleTouchAction

• `Optional` **doNotHandleTouchAction**: `boolean`

Defines that engine should ignore modifying touch action attribute and style
If not handle, you might need to set it up on your side for expected touch devices behavior.

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:137

___

### failIfMajorPerformanceCaveat

• `Optional` **failIfMajorPerformanceCaveat**: `boolean`

Will prevent the system from falling back to software implementation if a hardware device cannot be created

#### Overrides

WebGLContextAttributes.failIfMajorPerformanceCaveat

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:155

___

### forceSRGBBufferSupportState

• `Optional` **forceSRGBBufferSupportState**: `boolean`

If sRGB Buffer support is not set during construction, use this value to force a specific state
This is added due to an issue when processing textures in chrome/edge/firefox
This will not influence NativeEngine and WebGPUEngine which set the behavior to true during construction.

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:167

___

### limitDeviceRatio

• `Optional` **limitDeviceRatio**: `number`

Defines if the engine should no exceed a specified device ratio

**`See`**

https://developer.mozilla.org/en-US/docs/Web/API/Window/devicePixelRatio

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:98

___

### lockstepMaxSteps

• `Optional` **lockstepMaxSteps**: `number`

Defines the maximum steps to use with deterministic lock step mode

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:125

___

### powerPreference

• `Optional` **powerPreference**: `WebGLPowerPreference`

#### Inherited from

WebGLContextAttributes.powerPreference

#### Defined in

node_modules/typescript/lib/lib.dom.d.ts:1794

___

### premultipliedAlpha

• `Optional` **premultipliedAlpha**: `boolean`

#### Inherited from

WebGLContextAttributes.premultipliedAlpha

#### Defined in

node_modules/typescript/lib/lib.dom.d.ts:1795

___

### preserveDrawingBuffer

• `Optional` **preserveDrawingBuffer**: `boolean`

#### Inherited from

WebGLContextAttributes.preserveDrawingBuffer

#### Defined in

node_modules/typescript/lib/lib.dom.d.ts:1796

___

### stencil

• `Optional` **stencil**: `boolean`

#### Inherited from

WebGLContextAttributes.stencil

#### Defined in

node_modules/typescript/lib/lib.dom.d.ts:1797

___

### timeStep

• `Optional` **timeStep**: `number`

Defines the seconds between each deterministic lock step

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:127

___

### useExactSrgbConversions

• `Optional` **useExactSrgbConversions**: `boolean`

True if the more expensive but exact conversions should be used for transforming colors to and from linear space within shaders.
Otherwise, the default is to use a cheaper approximation.

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:172

___

### useHighPrecisionFloats

• `Optional` **useHighPrecisionFloats**: `boolean`

Defines that engine should compile shaders with high precision floats (if supported). True by default

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:141

___

### useHighPrecisionMatrix

• `Optional` **useHighPrecisionMatrix**: `boolean`

Make the matrix computations to be performed in 64 bits instead of 32 bits. False by default

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:150

___

### xrCompatible

• `Optional` **xrCompatible**: `boolean`

Make the canvas XR Compatible for XR sessions

#### Defined in

https://github.com/babylon.js/core/src/Engines/thinEngine.ts:145
