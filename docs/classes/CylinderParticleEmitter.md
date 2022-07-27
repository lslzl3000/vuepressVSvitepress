[@dev/core](../README.md) / [Exports](../modules.md) / CylinderParticleEmitter

# Class: CylinderParticleEmitter

Particle emitter emitting particles from the inside of a cylinder.
It emits the particles alongside the cylinder radius. The emission direction might be randomized.

## Hierarchy

- **`CylinderParticleEmitter`**

  ↳ [`CylinderDirectedParticleEmitter`](CylinderDirectedParticleEmitter.md)

## Implements

- [`IParticleEmitterType`](../interfaces/IParticleEmitterType.md)

## Table of contents

### Constructors

- [constructor](CylinderParticleEmitter.md#constructor)

### Properties

- [\_tempVector](CylinderParticleEmitter.md#_tempvector)
- [directionRandomizer](CylinderParticleEmitter.md#directionrandomizer)
- [height](CylinderParticleEmitter.md#height)
- [radius](CylinderParticleEmitter.md#radius)
- [radiusRange](CylinderParticleEmitter.md#radiusrange)

### Methods

- [applyToShader](CylinderParticleEmitter.md#applytoshader)
- [buildUniformLayout](CylinderParticleEmitter.md#builduniformlayout)
- [clone](CylinderParticleEmitter.md#clone)
- [getClassName](CylinderParticleEmitter.md#getclassname)
- [getEffectDefines](CylinderParticleEmitter.md#geteffectdefines)
- [parse](CylinderParticleEmitter.md#parse)
- [serialize](CylinderParticleEmitter.md#serialize)
- [startDirectionFunction](CylinderParticleEmitter.md#startdirectionfunction)
- [startPositionFunction](CylinderParticleEmitter.md#startpositionfunction)

## Constructors

### constructor

• **new CylinderParticleEmitter**(`radius?`, `height?`, `radiusRange?`, `directionRandomizer?`)

Creates a new instance CylinderParticleEmitter

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `radius` | `number` | `1` | the radius of the emission cylinder (1 by default) |
| `height` | `number` | `1` | the height of the emission cylinder (1 by default) |
| `radiusRange` | `number` | `1` | the range of the emission cylinder [0-1] 0 Surface only, 1 Entire Radius (1 by default) |
| `directionRandomizer` | `number` | `0` | defines how much to randomize the particle direction [0-1] |

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/cylinderParticleEmitter.ts:23

## Properties

### \_tempVector

• `Private` **\_tempVector**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/cylinderParticleEmitter.ts:14

___

### directionRandomizer

• **directionRandomizer**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/cylinderParticleEmitter.ts:39

___

### height

• **height**: `number` = `1`

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/cylinderParticleEmitter.ts:31

___

### radius

• **radius**: `number` = `1`

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/cylinderParticleEmitter.ts:27

___

### radiusRange

• **radiusRange**: `number` = `1`

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/cylinderParticleEmitter.ts:35

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

https://github.com/babylon.js/core/src/Particles/EmitterTypes/cylinderParticleEmitter.ts:116

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

https://github.com/babylon.js/core/src/Particles/EmitterTypes/cylinderParticleEmitter.ts:127

___

### clone

▸ **clone**(): [`CylinderParticleEmitter`](CylinderParticleEmitter.md)

Clones the current emitter and returns a copy of it

#### Returns

[`CylinderParticleEmitter`](CylinderParticleEmitter.md)

the new emitter

#### Implementation of

[IParticleEmitterType](../interfaces/IParticleEmitterType.md).[clone](../interfaces/IParticleEmitterType.md#clone)

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/cylinderParticleEmitter.ts:104

___

### getClassName

▸ **getClassName**(): `string`

Returns the string "CylinderParticleEmitter"

#### Returns

`string`

a string containing the class name

#### Implementation of

[IParticleEmitterType](../interfaces/IParticleEmitterType.md).[getClassName](../interfaces/IParticleEmitterType.md#getclassname)

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/cylinderParticleEmitter.ts:146

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

https://github.com/babylon.js/core/src/Particles/EmitterTypes/cylinderParticleEmitter.ts:138

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

https://github.com/babylon.js/core/src/Particles/EmitterTypes/cylinderParticleEmitter.ts:169

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

https://github.com/babylon.js/core/src/Particles/EmitterTypes/cylinderParticleEmitter.ts:154

___

### startDirectionFunction

▸ **startDirectionFunction**(`worldMatrix`, `directionToUpdate`, `particle`, `isLocal`, `inverseWorldMatrix`): `void`

Called by the particle System when the direction is computed for the created particle.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `worldMatrix` | [`Matrix`](Matrix.md) | is the world matrix of the particle system |
| `directionToUpdate` | [`Vector3`](Vector3.md) | is the direction vector to update with the result |
| `particle` | [`Particle`](Particle.md) | is the particle we are computed the direction for |
| `isLocal` | `boolean` | defines if the direction should be set in local space |
| `inverseWorldMatrix` | [`Matrix`](Matrix.md) | defines the inverted world matrix to use if isLocal is false |

#### Returns

`void`

#### Implementation of

[IParticleEmitterType](../interfaces/IParticleEmitterType.md).[startDirectionFunction](../interfaces/IParticleEmitterType.md#startdirectionfunction)

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/cylinderParticleEmitter.ts:50

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

https://github.com/babylon.js/core/src/Particles/EmitterTypes/cylinderParticleEmitter.ts:82
