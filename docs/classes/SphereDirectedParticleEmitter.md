[@dev/core](../README.md) / [Exports](../modules.md) / SphereDirectedParticleEmitter

# Class: SphereDirectedParticleEmitter

Particle emitter emitting particles from the inside of a sphere.
It emits the particles randomly between two vectors.

## Hierarchy

- [`SphereParticleEmitter`](SphereParticleEmitter.md)

  ↳ **`SphereDirectedParticleEmitter`**

## Table of contents

### Constructors

- [constructor](SphereDirectedParticleEmitter.md#constructor)

### Properties

- [direction1](SphereDirectedParticleEmitter.md#direction1)
- [direction2](SphereDirectedParticleEmitter.md#direction2)
- [directionRandomizer](SphereDirectedParticleEmitter.md#directionrandomizer)
- [radius](SphereDirectedParticleEmitter.md#radius)
- [radiusRange](SphereDirectedParticleEmitter.md#radiusrange)

### Methods

- [applyToShader](SphereDirectedParticleEmitter.md#applytoshader)
- [buildUniformLayout](SphereDirectedParticleEmitter.md#builduniformlayout)
- [clone](SphereDirectedParticleEmitter.md#clone)
- [getClassName](SphereDirectedParticleEmitter.md#getclassname)
- [getEffectDefines](SphereDirectedParticleEmitter.md#geteffectdefines)
- [parse](SphereDirectedParticleEmitter.md#parse)
- [serialize](SphereDirectedParticleEmitter.md#serialize)
- [startDirectionFunction](SphereDirectedParticleEmitter.md#startdirectionfunction)
- [startPositionFunction](SphereDirectedParticleEmitter.md#startpositionfunction)

## Constructors

### constructor

• **new SphereDirectedParticleEmitter**(`radius?`, `direction1?`, `direction2?`)

Creates a new instance SphereDirectedParticleEmitter

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `radius` | `number` | `1` | the radius of the emission sphere (1 by default) |
| `direction1` | [`Vector3`](Vector3.md) | `undefined` | the min limit of the emission direction (up vector by default) |
| `direction2` | [`Vector3`](Vector3.md) | `undefined` | the max limit of the emission direction (up vector by default) |

#### Overrides

[SphereParticleEmitter](SphereParticleEmitter.md).[constructor](SphereParticleEmitter.md#constructor)

#### Defined in

packages/dev/core/src/Particles/EmitterTypes/sphereParticleEmitter.ts:168

## Properties

### direction1

• **direction1**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Particles/EmitterTypes/sphereParticleEmitter.ts:173

___

### direction2

• **direction2**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Particles/EmitterTypes/sphereParticleEmitter.ts:177

___

### directionRandomizer

• **directionRandomizer**: `number` = `0`

#### Inherited from

[SphereParticleEmitter](SphereParticleEmitter.md).[directionRandomizer](SphereParticleEmitter.md#directionrandomizer)

#### Defined in

packages/dev/core/src/Particles/EmitterTypes/sphereParticleEmitter.ts:32

___

### radius

• **radius**: `number` = `1`

#### Inherited from

[SphereParticleEmitter](SphereParticleEmitter.md).[radius](SphereParticleEmitter.md#radius)

#### Defined in

packages/dev/core/src/Particles/EmitterTypes/sphereParticleEmitter.ts:24

___

### radiusRange

• **radiusRange**: `number` = `1`

#### Inherited from

[SphereParticleEmitter](SphereParticleEmitter.md).[radiusRange](SphereParticleEmitter.md#radiusrange)

#### Defined in

packages/dev/core/src/Particles/EmitterTypes/sphereParticleEmitter.ts:28

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

#### Overrides

[SphereParticleEmitter](SphereParticleEmitter.md).[applyToShader](SphereParticleEmitter.md#applytoshader)

#### Defined in

packages/dev/core/src/Particles/EmitterTypes/sphereParticleEmitter.ts:210

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

#### Overrides

[SphereParticleEmitter](SphereParticleEmitter.md).[buildUniformLayout](SphereParticleEmitter.md#builduniformlayout)

#### Defined in

packages/dev/core/src/Particles/EmitterTypes/sphereParticleEmitter.ts:221

___

### clone

▸ **clone**(): [`SphereDirectedParticleEmitter`](SphereDirectedParticleEmitter.md)

Clones the current emitter and returns a copy of it

#### Returns

[`SphereDirectedParticleEmitter`](SphereDirectedParticleEmitter.md)

the new emitter

#### Overrides

[SphereParticleEmitter](SphereParticleEmitter.md).[clone](SphereParticleEmitter.md#clone)

#### Defined in

packages/dev/core/src/Particles/EmitterTypes/sphereParticleEmitter.ts:198

___

### getClassName

▸ **getClassName**(): `string`

Returns the string "SphereDirectedParticleEmitter"

#### Returns

`string`

a string containing the class name

#### Overrides

[SphereParticleEmitter](SphereParticleEmitter.md).[getClassName](SphereParticleEmitter.md#getclassname)

#### Defined in

packages/dev/core/src/Particles/EmitterTypes/sphereParticleEmitter.ts:240

___

### getEffectDefines

▸ **getEffectDefines**(): `string`

Returns a string to use to update the GPU particles update shader

#### Returns

`string`

a string containing the defines string

#### Overrides

[SphereParticleEmitter](SphereParticleEmitter.md).[getEffectDefines](SphereParticleEmitter.md#geteffectdefines)

#### Defined in

packages/dev/core/src/Particles/EmitterTypes/sphereParticleEmitter.ts:232

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

#### Overrides

[SphereParticleEmitter](SphereParticleEmitter.md).[parse](SphereParticleEmitter.md#parse)

#### Defined in

packages/dev/core/src/Particles/EmitterTypes/sphereParticleEmitter.ts:261

___

### serialize

▸ **serialize**(): `any`

Serializes the particle system to a JSON object.

#### Returns

`any`

the JSON object

#### Overrides

[SphereParticleEmitter](SphereParticleEmitter.md).[serialize](SphereParticleEmitter.md#serialize)

#### Defined in

packages/dev/core/src/Particles/EmitterTypes/sphereParticleEmitter.ts:248

___

### startDirectionFunction

▸ **startDirectionFunction**(`worldMatrix`, `directionToUpdate`): `void`

Called by the particle System when the direction is computed for the created particle.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `worldMatrix` | [`Matrix`](Matrix.md) | is the world matrix of the particle system |
| `directionToUpdate` | [`Vector3`](Vector3.md) | is the direction vector to update with the result |

#### Returns

`void`

#### Overrides

[SphereParticleEmitter](SphereParticleEmitter.md).[startDirectionFunction](SphereParticleEmitter.md#startdirectionfunction)

#### Defined in

packages/dev/core/src/Particles/EmitterTypes/sphereParticleEmitter.ts:187

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

#### Inherited from

[SphereParticleEmitter](SphereParticleEmitter.md).[startPositionFunction](SphereParticleEmitter.md#startpositionfunction)

#### Defined in

packages/dev/core/src/Particles/EmitterTypes/sphereParticleEmitter.ts:67
