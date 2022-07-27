[@dev/core](../README.md) / [Exports](../modules.md) / ConeParticleEmitter

# Class: ConeParticleEmitter

Particle emitter emitting particles from the inside of a cone.
It emits the particles alongside the cone volume from the base to the particle.
The emission direction might be randomized.

## Implements

- [`IParticleEmitterType`](../interfaces/IParticleEmitterType.md)

## Table of contents

### Constructors

- [constructor](ConeParticleEmitter.md#constructor)

### Properties

- [\_angle](ConeParticleEmitter.md#_angle)
- [\_height](ConeParticleEmitter.md#_height)
- [\_radius](ConeParticleEmitter.md#_radius)
- [directionRandomizer](ConeParticleEmitter.md#directionrandomizer)
- [emitFromSpawnPointOnly](ConeParticleEmitter.md#emitfromspawnpointonly)
- [heightRange](ConeParticleEmitter.md#heightrange)
- [radiusRange](ConeParticleEmitter.md#radiusrange)

### Accessors

- [angle](ConeParticleEmitter.md#angle)
- [radius](ConeParticleEmitter.md#radius)

### Methods

- [\_buildHeight](ConeParticleEmitter.md#_buildheight)
- [applyToShader](ConeParticleEmitter.md#applytoshader)
- [buildUniformLayout](ConeParticleEmitter.md#builduniformlayout)
- [clone](ConeParticleEmitter.md#clone)
- [getClassName](ConeParticleEmitter.md#getclassname)
- [getEffectDefines](ConeParticleEmitter.md#geteffectdefines)
- [parse](ConeParticleEmitter.md#parse)
- [serialize](ConeParticleEmitter.md#serialize)
- [startDirectionFunction](ConeParticleEmitter.md#startdirectionfunction)
- [startPositionFunction](ConeParticleEmitter.md#startpositionfunction)

## Constructors

### constructor

• **new ConeParticleEmitter**(`radius?`, `angle?`, `directionRandomizer?`)

Creates a new instance ConeParticleEmitter

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `radius` | `number` | `1` | the radius of the emission cone (1 by default) |
| `angle` | `number` | `Math.PI` | the cone base angle (PI by default) |
| `directionRandomizer` | `number` | `0` | defines how much to randomize the particle direction [0-1] (default is 0) |

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/coneParticleEmitter.ts:72

## Properties

### \_angle

• `Private` **\_angle**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/coneParticleEmitter.ts:16

___

### \_height

• `Private` **\_height**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/coneParticleEmitter.ts:17

___

### \_radius

• `Private` **\_radius**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/coneParticleEmitter.ts:15

___

### directionRandomizer

• **directionRandomizer**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/coneParticleEmitter.ts:76

___

### emitFromSpawnPointOnly

• **emitFromSpawnPointOnly**: `boolean` = `false`

Gets or sets a value indicating if all the particles should be emitted from the spawn point only (the base of the cone)

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/coneParticleEmitter.ts:32

___

### heightRange

• **heightRange**: `number` = `1`

Gets or sets a value indicating where on the height the start position should be picked (1 = everywhere, 0 = only surface)

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/coneParticleEmitter.ts:27

___

### radiusRange

• **radiusRange**: `number` = `1`

Gets or sets a value indicating where on the radius the start position should be picked (1 = everywhere, 0 = only surface)

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/coneParticleEmitter.ts:22

## Accessors

### angle

• `get` **angle**(): `number`

Gets or sets the angle of the emission cone

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/coneParticleEmitter.ts:49

• `set` **angle**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/coneParticleEmitter.ts:53

___

### radius

• `get` **radius**(): `number`

Gets or sets the radius of the emission cone

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/coneParticleEmitter.ts:37

• `set` **radius**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/coneParticleEmitter.ts:41

## Methods

### \_buildHeight

▸ `Private` **_buildHeight**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/coneParticleEmitter.ts:58

___

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

https://github.com/babylon.js/core/src/Particles/EmitterTypes/coneParticleEmitter.ts:156

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

https://github.com/babylon.js/core/src/Particles/EmitterTypes/coneParticleEmitter.ts:167

___

### clone

▸ **clone**(): [`ConeParticleEmitter`](ConeParticleEmitter.md)

Clones the current emitter and returns a copy of it

#### Returns

[`ConeParticleEmitter`](ConeParticleEmitter.md)

the new emitter

#### Implementation of

[IParticleEmitterType](../interfaces/IParticleEmitterType.md).[clone](../interfaces/IParticleEmitterType.md#clone)

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/coneParticleEmitter.ts:144

___

### getClassName

▸ **getClassName**(): `string`

Returns the string "ConeParticleEmitter"

#### Returns

`string`

a string containing the class name

#### Implementation of

[IParticleEmitterType](../interfaces/IParticleEmitterType.md).[getClassName](../interfaces/IParticleEmitterType.md#getclassname)

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/coneParticleEmitter.ts:192

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

https://github.com/babylon.js/core/src/Particles/EmitterTypes/coneParticleEmitter.ts:178

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

https://github.com/babylon.js/core/src/Particles/EmitterTypes/coneParticleEmitter.ts:218

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

https://github.com/babylon.js/core/src/Particles/EmitterTypes/coneParticleEmitter.ts:200

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

https://github.com/babylon.js/core/src/Particles/EmitterTypes/coneParticleEmitter.ts:89

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

https://github.com/babylon.js/core/src/Particles/EmitterTypes/coneParticleEmitter.ts:112
