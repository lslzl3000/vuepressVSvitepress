[@dev/core](../README.md) / [Exports](../modules.md) / BoxParticleEmitter

# Class: BoxParticleEmitter

Particle emitter emitting particles from the inside of a box.
It emits the particles randomly between 2 given directions.

## Implements

- [`IParticleEmitterType`](../interfaces/IParticleEmitterType.md)

## Table of contents

### Constructors

- [constructor](BoxParticleEmitter.md#constructor)

### Properties

- [direction1](BoxParticleEmitter.md#direction1)
- [direction2](BoxParticleEmitter.md#direction2)
- [maxEmitBox](BoxParticleEmitter.md#maxemitbox)
- [minEmitBox](BoxParticleEmitter.md#minemitbox)

### Methods

- [applyToShader](BoxParticleEmitter.md#applytoshader)
- [buildUniformLayout](BoxParticleEmitter.md#builduniformlayout)
- [clone](BoxParticleEmitter.md#clone)
- [getClassName](BoxParticleEmitter.md#getclassname)
- [getEffectDefines](BoxParticleEmitter.md#geteffectdefines)
- [parse](BoxParticleEmitter.md#parse)
- [serialize](BoxParticleEmitter.md#serialize)
- [startDirectionFunction](BoxParticleEmitter.md#startdirectionfunction)
- [startPositionFunction](BoxParticleEmitter.md#startpositionfunction)

## Constructors

### constructor

• **new BoxParticleEmitter**()

Creates a new instance BoxParticleEmitter

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/boxParticleEmitter.ts:35

## Properties

### direction1

• **direction1**: [`Vector3`](Vector3.md)

Random direction of each particle after it has been emitted, between direction1 and direction2 vectors.

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/boxParticleEmitter.ts:17

___

### direction2

• **direction2**: [`Vector3`](Vector3.md)

Random direction of each particle after it has been emitted, between direction1 and direction2 vectors.

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/boxParticleEmitter.ts:21

___

### maxEmitBox

• **maxEmitBox**: [`Vector3`](Vector3.md)

Maximum box point around our emitter. Our emitter is the center of particles source, but if you want your particles to emit from more than one point, then you can tell it to do so.

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/boxParticleEmitter.ts:30

___

### minEmitBox

• **minEmitBox**: [`Vector3`](Vector3.md)

Minimum box point around our emitter. Our emitter is the center of particles source, but if you want your particles to emit from more than one point, then you can tell it to do so.

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/boxParticleEmitter.ts:26

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

https://github.com/babylon.js/core/src/Particles/EmitterTypes/boxParticleEmitter.ts:97

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

https://github.com/babylon.js/core/src/Particles/EmitterTypes/boxParticleEmitter.ts:108

___

### clone

▸ **clone**(): [`BoxParticleEmitter`](BoxParticleEmitter.md)

Clones the current emitter and returns a copy of it

#### Returns

[`BoxParticleEmitter`](BoxParticleEmitter.md)

the new emitter

#### Implementation of

[IParticleEmitterType](../interfaces/IParticleEmitterType.md).[clone](../interfaces/IParticleEmitterType.md#clone)

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/boxParticleEmitter.ts:85

___

### getClassName

▸ **getClassName**(): `string`

Returns the string "BoxParticleEmitter"

#### Returns

`string`

a string containing the class name

#### Implementation of

[IParticleEmitterType](../interfaces/IParticleEmitterType.md).[getClassName](../interfaces/IParticleEmitterType.md#getclassname)

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/boxParticleEmitter.ts:127

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

https://github.com/babylon.js/core/src/Particles/EmitterTypes/boxParticleEmitter.ts:119

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

https://github.com/babylon.js/core/src/Particles/EmitterTypes/boxParticleEmitter.ts:151

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

https://github.com/babylon.js/core/src/Particles/EmitterTypes/boxParticleEmitter.ts:135

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

https://github.com/babylon.js/core/src/Particles/EmitterTypes/boxParticleEmitter.ts:44

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

https://github.com/babylon.js/core/src/Particles/EmitterTypes/boxParticleEmitter.ts:66
