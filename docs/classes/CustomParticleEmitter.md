[@dev/core](../README.md) / [Exports](../modules.md) / CustomParticleEmitter

# Class: CustomParticleEmitter

Particle emitter emitting particles from a custom list of positions.

## Implements

- [`IParticleEmitterType`](../interfaces/IParticleEmitterType.md)

## Table of contents

### Constructors

- [constructor](CustomParticleEmitter.md#constructor)

### Properties

- [particleDestinationGenerator](CustomParticleEmitter.md#particledestinationgenerator)
- [particlePositionGenerator](CustomParticleEmitter.md#particlepositiongenerator)

### Methods

- [applyToShader](CustomParticleEmitter.md#applytoshader)
- [buildUniformLayout](CustomParticleEmitter.md#builduniformlayout)
- [clone](CustomParticleEmitter.md#clone)
- [getClassName](CustomParticleEmitter.md#getclassname)
- [getEffectDefines](CustomParticleEmitter.md#geteffectdefines)
- [parse](CustomParticleEmitter.md#parse)
- [serialize](CustomParticleEmitter.md#serialize)
- [startDirectionFunction](CustomParticleEmitter.md#startdirectionfunction)
- [startPositionFunction](CustomParticleEmitter.md#startpositionfunction)

## Constructors

### constructor

• **new CustomParticleEmitter**()

Creates a new instance CustomParticleEmitter

#### Defined in

packages/dev/core/src/Particles/EmitterTypes/customParticleEmitter.ts:28

## Properties

### particleDestinationGenerator

• **particleDestinationGenerator**: (`index`: `number`, `particle`: [`Nullable`](../modules.md#nullable)[`Particle`](Particle.md), `outDestination`: [`Vector3`](Vector3.md)) => `void`

#### Type declaration

▸ (`index`, `particle`, `outDestination`): `void`

Gets or sets the destination generator that will create the final destination of each particle.
 * Index will be provided when used with GPU particle. Particle will be provided when used with CPU particles

##### Parameters

| Name | Type |
| :------ | :------ |
| `index` | `number` |
| `particle` | [`Nullable`](../modules.md#nullable)[`Particle`](Particle.md) |
| `outDestination` | [`Vector3`](Vector3.md) |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Particles/EmitterTypes/customParticleEmitter.ts:23

___

### particlePositionGenerator

• **particlePositionGenerator**: (`index`: `number`, `particle`: [`Nullable`](../modules.md#nullable)[`Particle`](Particle.md), `outPosition`: [`Vector3`](Vector3.md)) => `void`

#### Type declaration

▸ (`index`, `particle`, `outPosition`): `void`

Gets or sets the position generator that will create the initial position of each particle.
Index will be provided when used with GPU particle. Particle will be provided when used with CPU particles

##### Parameters

| Name | Type |
| :------ | :------ |
| `index` | `number` |
| `particle` | [`Nullable`](../modules.md#nullable)[`Particle`](Particle.md) |
| `outPosition` | [`Vector3`](Vector3.md) |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Particles/EmitterTypes/customParticleEmitter.ts:17

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

packages/dev/core/src/Particles/EmitterTypes/customParticleEmitter.ts:101

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

packages/dev/core/src/Particles/EmitterTypes/customParticleEmitter.ts:108

___

### clone

▸ **clone**(): [`CustomParticleEmitter`](CustomParticleEmitter.md)

Clones the current emitter and returns a copy of it

#### Returns

[`CustomParticleEmitter`](CustomParticleEmitter.md)

the new emitter

#### Implementation of

[IParticleEmitterType](../interfaces/IParticleEmitterType.md).[clone](../interfaces/IParticleEmitterType.md#clone)

#### Defined in

packages/dev/core/src/Particles/EmitterTypes/customParticleEmitter.ts:88

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

packages/dev/core/src/Particles/EmitterTypes/customParticleEmitter.ts:122

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

packages/dev/core/src/Particles/EmitterTypes/customParticleEmitter.ts:114

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

packages/dev/core/src/Particles/EmitterTypes/customParticleEmitter.ts:143

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

packages/dev/core/src/Particles/EmitterTypes/customParticleEmitter.ts:130

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

packages/dev/core/src/Particles/EmitterTypes/customParticleEmitter.ts:37

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

packages/dev/core/src/Particles/EmitterTypes/customParticleEmitter.ts:67
