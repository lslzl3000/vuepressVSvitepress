[@dev/core](../README.md) / [Exports](../modules.md) / IParticleEmitterType

# Interface: IParticleEmitterType

Particle emitter represents a volume emitting particles.
This is the responsibility of the implementation to define the volume shape like cone/sphere/box.

## Implemented by

- [`BoxParticleEmitter`](../classes/BoxParticleEmitter.md)
- [`ConeParticleEmitter`](../classes/ConeParticleEmitter.md)
- [`CustomParticleEmitter`](../classes/CustomParticleEmitter.md)
- [`CylinderParticleEmitter`](../classes/CylinderParticleEmitter.md)
- [`HemisphericParticleEmitter`](../classes/HemisphericParticleEmitter.md)
- [`MeshParticleEmitter`](../classes/MeshParticleEmitter.md)
- [`PointParticleEmitter`](../classes/PointParticleEmitter.md)
- [`SphereParticleEmitter`](../classes/SphereParticleEmitter.md)

## Table of contents

### Methods

- [applyToShader](IParticleEmitterType.md#applytoshader)
- [buildUniformLayout](IParticleEmitterType.md#builduniformlayout)
- [clone](IParticleEmitterType.md#clone)
- [getClassName](IParticleEmitterType.md#getclassname)
- [getEffectDefines](IParticleEmitterType.md#geteffectdefines)
- [parse](IParticleEmitterType.md#parse)
- [serialize](IParticleEmitterType.md#serialize)
- [startDirectionFunction](IParticleEmitterType.md#startdirectionfunction)
- [startPositionFunction](IParticleEmitterType.md#startpositionfunction)

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

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/IParticleEmitterType.ts:43

___

### buildUniformLayout

▸ **buildUniformLayout**(`ubo`): `void`

Creates the structure of the ubo for this particle emitter

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ubo` | [`UniformBuffer`](../classes/UniformBuffer.md) | ubo to create the structure for |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/IParticleEmitterType.ts:49

___

### clone

▸ **clone**(): [`IParticleEmitterType`](IParticleEmitterType.md)

Clones the current emitter and returns a copy of it

#### Returns

[`IParticleEmitterType`](IParticleEmitterType.md)

the new emitter

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/IParticleEmitterType.ts:37

___

### getClassName

▸ **getClassName**(): `string`

Returns a string representing the class name

#### Returns

`string`

a string containing the class name

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/IParticleEmitterType.ts:61

___

### getEffectDefines

▸ **getEffectDefines**(): `string`

Returns a string to use to update the GPU particles update shader

#### Returns

`string`

the effect defines string

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/IParticleEmitterType.ts:55

___

### parse

▸ **parse**(`serializationObject`, `scene`): `void`

Parse properties from a JSON object

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `serializationObject` | `any` | defines the JSON object |
| `scene` | [`Nullable`](../modules.md#nullable)[`Scene`](../classes/Scene.md) | defines the hosting scene |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/IParticleEmitterType.ts:74

___

### serialize

▸ **serialize**(): `any`

Serializes the particle system to a JSON object.

#### Returns

`any`

the JSON object

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/IParticleEmitterType.ts:67

___

### startDirectionFunction

▸ **startDirectionFunction**(`worldMatrix`, `directionToUpdate`, `particle`, `isLocal`, `inverseWorldMatrix`): `void`

Called by the particle System when the direction is computed for the created particle.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `worldMatrix` | [`Matrix`](../classes/Matrix.md) | is the world matrix of the particle system |
| `directionToUpdate` | [`Vector3`](../classes/Vector3.md) | is the direction vector to update with the result |
| `particle` | [`Particle`](../classes/Particle.md) | is the particle we are computed the direction for |
| `isLocal` | `boolean` | defines if the direction should be set in local space |
| `inverseWorldMatrix` | [`Matrix`](../classes/Matrix.md) | defines the inverted world matrix to use if isLocal is false |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/IParticleEmitterType.ts:22

___

### startPositionFunction

▸ **startPositionFunction**(`worldMatrix`, `positionToUpdate`, `particle`, `isLocal`): `void`

Called by the particle System when the position is computed for the created particle.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `worldMatrix` | [`Matrix`](../classes/Matrix.md) | is the world matrix of the particle system |
| `positionToUpdate` | [`Vector3`](../classes/Vector3.md) | is the position vector to update with the result |
| `particle` | [`Particle`](../classes/Particle.md) | is the particle we are computed the position for |
| `isLocal` | `boolean` | defines if the position should be set in local space |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/IParticleEmitterType.ts:31
