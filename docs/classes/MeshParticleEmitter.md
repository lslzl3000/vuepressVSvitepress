[@dev/core](../README.md) / [Exports](../modules.md) / MeshParticleEmitter

# Class: MeshParticleEmitter

Particle emitter emitting particles from the inside of a box.
It emits the particles randomly between 2 given directions.

## Implements

- [`IParticleEmitterType`](../interfaces/IParticleEmitterType.md)

## Table of contents

### Constructors

- [constructor](MeshParticleEmitter.md#constructor)

### Properties

- [\_indices](MeshParticleEmitter.md#_indices)
- [\_mesh](MeshParticleEmitter.md#_mesh)
- [\_normals](MeshParticleEmitter.md#_normals)
- [\_positions](MeshParticleEmitter.md#_positions)
- [\_storedNormal](MeshParticleEmitter.md#_storednormal)
- [direction1](MeshParticleEmitter.md#direction1)
- [direction2](MeshParticleEmitter.md#direction2)
- [useMeshNormalsForDirection](MeshParticleEmitter.md#usemeshnormalsfordirection)

### Accessors

- [mesh](MeshParticleEmitter.md#mesh)

### Methods

- [applyToShader](MeshParticleEmitter.md#applytoshader)
- [buildUniformLayout](MeshParticleEmitter.md#builduniformlayout)
- [clone](MeshParticleEmitter.md#clone)
- [getClassName](MeshParticleEmitter.md#getclassname)
- [getEffectDefines](MeshParticleEmitter.md#geteffectdefines)
- [parse](MeshParticleEmitter.md#parse)
- [serialize](MeshParticleEmitter.md#serialize)
- [startDirectionFunction](MeshParticleEmitter.md#startdirectionfunction)
- [startPositionFunction](MeshParticleEmitter.md#startpositionfunction)

## Constructors

### constructor

• **new MeshParticleEmitter**(`mesh?`)

Creates a new instance MeshParticleEmitter

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `mesh` | [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md) | `null` | defines the mesh to use as source |

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/meshParticleEmitter.ts:65

## Properties

### \_indices

• `Private` **\_indices**: [`Nullable`](../modules.md#nullable)[`IndicesArray`](../modules.md#indicesarray) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/meshParticleEmitter.ts:18

___

### \_mesh

• `Private` **\_mesh**: [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/meshParticleEmitter.ts:22

___

### \_normals

• `Private` **\_normals**: [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/meshParticleEmitter.ts:20

___

### \_positions

• `Private` **\_positions**: [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/meshParticleEmitter.ts:19

___

### \_storedNormal

• `Private` **\_storedNormal**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/meshParticleEmitter.ts:21

___

### direction1

• **direction1**: [`Vector3`](Vector3.md)

Random direction of each particle after it has been emitted, between direction1 and direction2 vectors.

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/meshParticleEmitter.ts:27

___

### direction2

• **direction2**: [`Vector3`](Vector3.md)

Random direction of each particle after it has been emitted, between direction1 and direction2 vectors.

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/meshParticleEmitter.ts:31

___

### useMeshNormalsForDirection

• **useMeshNormalsForDirection**: `boolean` = `true`

Gets or sets a boolean indicating that particle directions must be built from mesh face normals

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/meshParticleEmitter.ts:36

## Accessors

### mesh

• `get` **mesh**(): [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

Defines the mesh to use as source

#### Returns

[`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/meshParticleEmitter.ts:39

• `set` **mesh**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/meshParticleEmitter.ts:43

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

https://github.com/babylon.js/core/src/Particles/EmitterTypes/meshParticleEmitter.ts:160

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

https://github.com/babylon.js/core/src/Particles/EmitterTypes/meshParticleEmitter.ts:169

___

### clone

▸ **clone**(): [`MeshParticleEmitter`](MeshParticleEmitter.md)

Clones the current emitter and returns a copy of it

#### Returns

[`MeshParticleEmitter`](MeshParticleEmitter.md)

the new emitter

#### Implementation of

[IParticleEmitterType](../interfaces/IParticleEmitterType.md).[clone](../interfaces/IParticleEmitterType.md#clone)

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/meshParticleEmitter.ts:148

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

https://github.com/babylon.js/core/src/Particles/EmitterTypes/meshParticleEmitter.ts:186

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

https://github.com/babylon.js/core/src/Particles/EmitterTypes/meshParticleEmitter.ts:178

___

### parse

▸ **parse**(`serializationObject`, `scene`): `void`

Parse properties from a JSON object

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `serializationObject` | `any` | defines the JSON object |
| `scene` | [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) | defines the hosting scene |

#### Returns

`void`

#### Implementation of

[IParticleEmitterType](../interfaces/IParticleEmitterType.md).[parse](../interfaces/IParticleEmitterType.md#parse)

#### Defined in

https://github.com/babylon.js/core/src/Particles/EmitterTypes/meshParticleEmitter.ts:211

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

https://github.com/babylon.js/core/src/Particles/EmitterTypes/meshParticleEmitter.ts:194

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

https://github.com/babylon.js/core/src/Particles/EmitterTypes/meshParticleEmitter.ts:76

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

https://github.com/babylon.js/core/src/Particles/EmitterTypes/meshParticleEmitter.ts:101
