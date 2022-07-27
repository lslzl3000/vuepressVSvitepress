[@dev/core](../README.md) / [Exports](../modules.md) / CylinderDirectedParticleEmitter

# Class: CylinderDirectedParticleEmitter

Particle emitter emitting particles from the inside of a cylinder.
It emits the particles randomly between two vectors.

## Hierarchy

- [`CylinderParticleEmitter`](CylinderParticleEmitter.md)

  ↳ **`CylinderDirectedParticleEmitter`**

## Table of contents

### Constructors

- [constructor](CylinderDirectedParticleEmitter.md#constructor)

### Properties

- [direction1](CylinderDirectedParticleEmitter.md#direction1)
- [direction2](CylinderDirectedParticleEmitter.md#direction2)
- [directionRandomizer](CylinderDirectedParticleEmitter.md#directionrandomizer)
- [height](CylinderDirectedParticleEmitter.md#height)
- [radius](CylinderDirectedParticleEmitter.md#radius)
- [radiusRange](CylinderDirectedParticleEmitter.md#radiusrange)

### Methods

- [applyToShader](CylinderDirectedParticleEmitter.md#applytoshader)
- [buildUniformLayout](CylinderDirectedParticleEmitter.md#builduniformlayout)
- [clone](CylinderDirectedParticleEmitter.md#clone)
- [getClassName](CylinderDirectedParticleEmitter.md#getclassname)
- [getEffectDefines](CylinderDirectedParticleEmitter.md#geteffectdefines)
- [parse](CylinderDirectedParticleEmitter.md#parse)
- [serialize](CylinderDirectedParticleEmitter.md#serialize)
- [startDirectionFunction](CylinderDirectedParticleEmitter.md#startdirectionfunction)
- [startPositionFunction](CylinderDirectedParticleEmitter.md#startpositionfunction)

## Constructors

### constructor

• **new CylinderDirectedParticleEmitter**(`radius?`, `height?`, `radiusRange?`, `direction1?`, `direction2?`)

Creates a new instance CylinderDirectedParticleEmitter

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `radius` | `number` | `1` | the radius of the emission cylinder (1 by default) |
| `height` | `number` | `1` | the height of the emission cylinder (1 by default) |
| `radiusRange` | `number` | `1` | the range of the emission cylinder [0-1] 0 Surface only, 1 Entire Radius (1 by default) |
| `direction1` | [`Vector3`](Vector3.md) | `undefined` | the min limit of the emission direction (up vector by default) |
| `direction2` | [`Vector3`](Vector3.md) | `undefined` | the max limit of the emission direction (up vector by default) |

#### Overrides

[CylinderParticleEmitter](CylinderParticleEmitter.md).[constructor](CylinderParticleEmitter.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/cylinderParticleEmitter.ts:190

## Properties

### direction1

• **direction1**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/cylinderParticleEmitter.ts:197

___

### direction2

• **direction2**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/cylinderParticleEmitter.ts:201

___

### directionRandomizer

• **directionRandomizer**: `number` = `0`

#### Inherited from

[CylinderParticleEmitter](CylinderParticleEmitter.md).[directionRandomizer](CylinderParticleEmitter.md#directionrandomizer)

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/cylinderParticleEmitter.ts:39

___

### height

• **height**: `number` = `1`

#### Inherited from

[CylinderParticleEmitter](CylinderParticleEmitter.md).[height](CylinderParticleEmitter.md#height)

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/cylinderParticleEmitter.ts:31

___

### radius

• **radius**: `number` = `1`

#### Inherited from

[CylinderParticleEmitter](CylinderParticleEmitter.md).[radius](CylinderParticleEmitter.md#radius)

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/cylinderParticleEmitter.ts:27

___

### radiusRange

• **radiusRange**: `number` = `1`

#### Inherited from

[CylinderParticleEmitter](CylinderParticleEmitter.md).[radiusRange](CylinderParticleEmitter.md#radiusrange)

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

#### Overrides

[CylinderParticleEmitter](CylinderParticleEmitter.md).[applyToShader](CylinderParticleEmitter.md#applytoshader)

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/cylinderParticleEmitter.ts:234

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

[CylinderParticleEmitter](CylinderParticleEmitter.md).[buildUniformLayout](CylinderParticleEmitter.md#builduniformlayout)

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/cylinderParticleEmitter.ts:246

___

### clone

▸ **clone**(): [`CylinderDirectedParticleEmitter`](CylinderDirectedParticleEmitter.md)

Clones the current emitter and returns a copy of it

#### Returns

[`CylinderDirectedParticleEmitter`](CylinderDirectedParticleEmitter.md)

the new emitter

#### Overrides

[CylinderParticleEmitter](CylinderParticleEmitter.md).[clone](CylinderParticleEmitter.md#clone)

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/cylinderParticleEmitter.ts:222

___

### getClassName

▸ **getClassName**(): `string`

Returns the string "CylinderDirectedParticleEmitter"

#### Returns

`string`

a string containing the class name

#### Overrides

[CylinderParticleEmitter](CylinderParticleEmitter.md).[getClassName](CylinderParticleEmitter.md#getclassname)

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/cylinderParticleEmitter.ts:266

___

### getEffectDefines

▸ **getEffectDefines**(): `string`

Returns a string to use to update the GPU particles update shader

#### Returns

`string`

a string containing the defines string

#### Overrides

[CylinderParticleEmitter](CylinderParticleEmitter.md).[getEffectDefines](CylinderParticleEmitter.md#geteffectdefines)

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/cylinderParticleEmitter.ts:258

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

[CylinderParticleEmitter](CylinderParticleEmitter.md).[parse](CylinderParticleEmitter.md#parse)

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/cylinderParticleEmitter.ts:287

___

### serialize

▸ **serialize**(): `any`

Serializes the particle system to a JSON object.

#### Returns

`any`

the JSON object

#### Overrides

[CylinderParticleEmitter](CylinderParticleEmitter.md).[serialize](CylinderParticleEmitter.md#serialize)

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/cylinderParticleEmitter.ts:274

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

[CylinderParticleEmitter](CylinderParticleEmitter.md).[startDirectionFunction](CylinderParticleEmitter.md#startdirectionfunction)

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/cylinderParticleEmitter.ts:211

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

[CylinderParticleEmitter](CylinderParticleEmitter.md).[startPositionFunction](CylinderParticleEmitter.md#startpositionfunction)

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/cylinderParticleEmitter.ts:82
