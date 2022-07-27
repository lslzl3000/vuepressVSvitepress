[@dev/core](../README.md) / [Exports](../modules.md) / PointParticleEmitter

# Class: PointParticleEmitter

Particle emitter emitting particles from a point.
It emits the particles randomly between 2 given directions.

## Implements

- [`IParticleEmitterType`](../interfaces/IParticleEmitterType.md)

## Table of contents

### Constructors

- [constructor](PointParticleEmitter.md#constructor)

### Properties

- [direction1](PointParticleEmitter.md#direction1)
- [direction2](PointParticleEmitter.md#direction2)

### Methods

- [applyToShader](PointParticleEmitter.md#applytoshader)
- [buildUniformLayout](PointParticleEmitter.md#builduniformlayout)
- [clone](PointParticleEmitter.md#clone)
- [getClassName](PointParticleEmitter.md#getclassname)
- [getEffectDefines](PointParticleEmitter.md#geteffectdefines)
- [parse](PointParticleEmitter.md#parse)
- [serialize](PointParticleEmitter.md#serialize)
- [startDirectionFunction](PointParticleEmitter.md#startdirectionfunction)
- [startPositionFunction](PointParticleEmitter.md#startpositionfunction)

## Constructors

### constructor

• **new PointParticleEmitter**()

Creates a new instance PointParticleEmitter

#### Defined in

packages/dev/core/src/Particles/EmitterTypes/pointParticleEmitter.ts:26

## Properties

### direction1

• **direction1**: [`Vector3`](Vector3.md)

Random direction of each particle after it has been emitted, between direction1 and direction2 vectors.

#### Defined in

packages/dev/core/src/Particles/EmitterTypes/pointParticleEmitter.ts:17

___

### direction2

• **direction2**: [`Vector3`](Vector3.md)

Random direction of each particle after it has been emitted, between direction1 and direction2 vectors.

#### Defined in

packages/dev/core/src/Particles/EmitterTypes/pointParticleEmitter.ts:21

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

packages/dev/core/src/Particles/EmitterTypes/pointParticleEmitter.ts:79

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

packages/dev/core/src/Particles/EmitterTypes/pointParticleEmitter.ts:88

___

### clone

▸ **clone**(): [`PointParticleEmitter`](PointParticleEmitter.md)

Clones the current emitter and returns a copy of it

#### Returns

[`PointParticleEmitter`](PointParticleEmitter.md)

the new emitter

#### Implementation of

[IParticleEmitterType](../interfaces/IParticleEmitterType.md).[clone](../interfaces/IParticleEmitterType.md#clone)

#### Defined in

packages/dev/core/src/Particles/EmitterTypes/pointParticleEmitter.ts:67

___

### getClassName

▸ **getClassName**(): `string`

Returns the string "PointParticleEmitter"

#### Returns

`string`

a string containing the class name

#### Implementation of

[IParticleEmitterType](../interfaces/IParticleEmitterType.md).[getClassName](../interfaces/IParticleEmitterType.md#getclassname)

#### Defined in

packages/dev/core/src/Particles/EmitterTypes/pointParticleEmitter.ts:105

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

packages/dev/core/src/Particles/EmitterTypes/pointParticleEmitter.ts:97

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

packages/dev/core/src/Particles/EmitterTypes/pointParticleEmitter.ts:127

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

packages/dev/core/src/Particles/EmitterTypes/pointParticleEmitter.ts:113

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

packages/dev/core/src/Particles/EmitterTypes/pointParticleEmitter.ts:35

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

packages/dev/core/src/Particles/EmitterTypes/pointParticleEmitter.ts:55
