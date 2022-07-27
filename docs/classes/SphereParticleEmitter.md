[@dev/core](../README.md) / [Exports](../modules.md) / SphereParticleEmitter

# Class: SphereParticleEmitter

Particle emitter emitting particles from the inside of a sphere.
It emits the particles alongside the sphere radius. The emission direction might be randomized.

## Hierarchy

- **`SphereParticleEmitter`**

  ↳ [`SphereDirectedParticleEmitter`](SphereDirectedParticleEmitter.md)

## Implements

- [`IParticleEmitterType`](../interfaces/IParticleEmitterType.md)

## Table of contents

### Constructors

- [constructor](SphereParticleEmitter.md#constructor)

### Properties

- [directionRandomizer](SphereParticleEmitter.md#directionrandomizer)
- [radius](SphereParticleEmitter.md#radius)
- [radiusRange](SphereParticleEmitter.md#radiusrange)

### Methods

- [applyToShader](SphereParticleEmitter.md#applytoshader)
- [buildUniformLayout](SphereParticleEmitter.md#builduniformlayout)
- [clone](SphereParticleEmitter.md#clone)
- [getClassName](SphereParticleEmitter.md#getclassname)
- [getEffectDefines](SphereParticleEmitter.md#geteffectdefines)
- [parse](SphereParticleEmitter.md#parse)
- [serialize](SphereParticleEmitter.md#serialize)
- [startDirectionFunction](SphereParticleEmitter.md#startdirectionfunction)
- [startPositionFunction](SphereParticleEmitter.md#startpositionfunction)

## Constructors

### constructor

• **new SphereParticleEmitter**(`radius?`, `radiusRange?`, `directionRandomizer?`)

Creates a new instance SphereParticleEmitter

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `radius` | `number` | `1` | the radius of the emission sphere (1 by default) |
| `radiusRange` | `number` | `1` | the range of the emission sphere [0-1] 0 Surface only, 1 Entire Radius (1 by default) |
| `directionRandomizer` | `number` | `0` | defines how much to randomize the particle direction [0-1] |

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/sphereParticleEmitter.ts:20

## Properties

### directionRandomizer

• **directionRandomizer**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/sphereParticleEmitter.ts:32

___

### radius

• **radius**: `number` = `1`

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/sphereParticleEmitter.ts:24

___

### radiusRange

• **radiusRange**: `number` = `1`

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/sphereParticleEmitter.ts:28

## Methods

### applyToShader

▸ **applyToShader**(`uboOrEffect`): `void`

Called by the GPUParticleSystem to setup the update shader

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uboOrEffect` | `UniformBufferEffectCommonAccessor` | defines the update shader |

#### Returns

`void`

#### Implementation of

[IParticleEmitterType](../interfaces/IParticleEmitterType.md).[applyToShader](../interfaces/IParticleEmitterType.md#applytoshader)

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/sphereParticleEmitter.ts:100

___

### buildUniformLayout

▸ **buildUniformLayout**(`ubo`): `void`

Creates the structure of the ubo for this particle emitter

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ubo` | [`UniformBuffer`](UniformBuffer.md) | ubo to create the structure for |

#### Returns

`void`

#### Implementation of

[IParticleEmitterType](../interfaces/IParticleEmitterType.md).[buildUniformLayout](../interfaces/IParticleEmitterType.md#builduniformlayout)

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/sphereParticleEmitter.ts:110

___

### clone

▸ **clone**(): [`SphereParticleEmitter`](SphereParticleEmitter.md)

Clones the current emitter and returns a copy of it

#### Returns

[`SphereParticleEmitter`](SphereParticleEmitter.md)

the new emitter

#### Implementation of

[IParticleEmitterType](../interfaces/IParticleEmitterType.md).[clone](../interfaces/IParticleEmitterType.md#clone)

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/sphereParticleEmitter.ts:88

___

### getClassName

▸ **getClassName**(): `string`

Returns the string "SphereParticleEmitter"

#### Returns

`string`

a string containing the class name

#### Implementation of

[IParticleEmitterType](../interfaces/IParticleEmitterType.md).[getClassName](../interfaces/IParticleEmitterType.md#getclassname)

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/sphereParticleEmitter.ts:128

___

### getEffectDefines

▸ **getEffectDefines**(): `string`

Returns a string to use to update the GPU particles update shader

#### Returns

`string`

a string containing the defines string

#### Implementation of

[IParticleEmitterType](../interfaces/IParticleEmitterType.md).[getEffectDefines](../interfaces/IParticleEmitterType.md#geteffectdefines)

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/sphereParticleEmitter.ts:120

___

### parse

▸ **parse**(`serializationObject`): `void`

Parse properties from a JSON object

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `serializationObject` | `any` | defines the JSON object |

#### Returns

`void`

#### Implementation of

[IParticleEmitterType](../interfaces/IParticleEmitterType.md).[parse](../interfaces/IParticleEmitterType.md#parse)

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/sphereParticleEmitter.ts:150

___

### serialize

▸ **serialize**(): `any`

Serializes the particle system to a JSON object.

#### Returns

`any`

the JSON object

#### Implementation of

[IParticleEmitterType](../interfaces/IParticleEmitterType.md).[serialize](../interfaces/IParticleEmitterType.md#serialize)

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/sphereParticleEmitter.ts:136

___

### startDirectionFunction

▸ **startDirectionFunction**(`worldMatrix`, `directionToUpdate`, `particle`, `isLocal`): `void`

Called by the particle System when the direction is computed for the created particle.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `worldMatrix` | [`Matrix`](Matrix.md) | is the world matrix of the particle system |
| `directionToUpdate` | [`Vector3`](Vector3.md) | is the direction vector to update with the result |
| `particle` | [`Particle`](Particle.md) | is the particle we are computed the direction for |
| `isLocal` | `boolean` | defines if the direction should be set in local space |

#### Returns

`void`

#### Implementation of

[IParticleEmitterType](../interfaces/IParticleEmitterType.md).[startDirectionFunction](../interfaces/IParticleEmitterType.md#startdirectionfunction)

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/sphereParticleEmitter.ts:42

___

### startPositionFunction

▸ **startPositionFunction**(`worldMatrix`, `positionToUpdate`, `particle`, `isLocal`): `void`

Called by the particle System when the position is computed for the created particle.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `worldMatrix` | [`Matrix`](Matrix.md) | is the world matrix of the particle system |
| `positionToUpdate` | [`Vector3`](Vector3.md) | is the position vector to update with the result |
| `particle` | [`Particle`](Particle.md) | is the particle we are computed the position for |
| `isLocal` | `boolean` | defines if the position should be set in local space |

#### Returns

`void`

#### Implementation of

[IParticleEmitterType](../interfaces/IParticleEmitterType.md).[startPositionFunction](../interfaces/IParticleEmitterType.md#startpositionfunction)

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/sphereParticleEmitter.ts:67
