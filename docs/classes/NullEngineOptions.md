[@dev/core](../README.md) / [Exports](../modules.md) / NullEngineOptions

# Class: NullEngineOptions

Options to create the null engine

## Table of contents

### Constructors

- [constructor](NullEngineOptions.md#constructor)

### Properties

- [deterministicLockstep](NullEngineOptions.md#deterministiclockstep)
- [lockstepMaxSteps](NullEngineOptions.md#lockstepmaxsteps)
- [renderHeight](NullEngineOptions.md#renderheight)
- [renderWidth](NullEngineOptions.md#renderwidth)
- [textureSize](NullEngineOptions.md#texturesize)
- [useHighPrecisionMatrix](NullEngineOptions.md#usehighprecisionmatrix)

## Constructors

### constructor

• **new NullEngineOptions**()

## Properties

### deterministicLockstep

• **deterministicLockstep**: `boolean` = `false`

If delta time between frames should be constant

**`See`**

https://doc.babylonjs.com/babylon101/animations#deterministic-lockstep

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:43

___

### lockstepMaxSteps

• **lockstepMaxSteps**: `number` = `4`

Maximum about of steps between frames (Default: 4)

**`See`**

https://doc.babylonjs.com/babylon101/animations#deterministic-lockstep

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:49

___

### renderHeight

• **renderHeight**: `number` = `256`

Render height (Default: 256)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:32

___

### renderWidth

• **renderWidth**: `number` = `512`

Render width (Default: 512)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:28

___

### textureSize

• **textureSize**: `number` = `512`

Texture size (Default: 512)

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:37

___

### useHighPrecisionMatrix

• `Optional` **useHighPrecisionMatrix**: `boolean`

Make the matrix computations to be performed in 64 bits instead of 32 bits. False by default

#### Defined in

packages/dev/core/src/Engines/nullEngine.ts:54
