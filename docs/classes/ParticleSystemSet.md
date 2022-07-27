[@dev/core](../README.md) / [Exports](../modules.md) / ParticleSystemSet

# Class: ParticleSystemSet

Represents a set of particle systems working together to create a specific effect

## Implements

- [`IDisposable`](../interfaces/IDisposable.md)

## Table of contents

### Constructors

- [constructor](ParticleSystemSet.md#constructor)

### Properties

- [\_emitterCreationOptions](ParticleSystemSet.md#_emittercreationoptions)
- [\_emitterNode](ParticleSystemSet.md#_emitternode)
- [\_emitterNodeIsOwned](ParticleSystemSet.md#_emitternodeisowned)
- [systems](ParticleSystemSet.md#systems)
- [BaseAssetsUrl](ParticleSystemSet.md#baseassetsurl)

### Accessors

- [emitterNode](ParticleSystemSet.md#emitternode)

### Methods

- [dispose](ParticleSystemSet.md#dispose)
- [serialize](ParticleSystemSet.md#serialize)
- [setEmitterAsSphere](ParticleSystemSet.md#setemitterassphere)
- [start](ParticleSystemSet.md#start)
- [Parse](ParticleSystemSet.md#parse)

## Constructors

### constructor

• **new ParticleSystemSet**()

## Properties

### \_emitterCreationOptions

• `Private` **\_emitterCreationOptions**: `ParticleSystemSetEmitterCreationOptions`

#### Defined in

https://github.com/babylon.js/core/src/Particles/particleSystemSet.ts:29

___

### \_emitterNode

• `Private` **\_emitterNode**: [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md) \| [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Particles/particleSystemSet.ts:30

___

### \_emitterNodeIsOwned

• `Private` **\_emitterNodeIsOwned**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Particles/particleSystemSet.ts:31

___

### systems

• **systems**: [`IParticleSystem`](../interfaces/IParticleSystem.md)[]

Gets the particle system list

#### Defined in

https://github.com/babylon.js/core/src/Particles/particleSystemSet.ts:36

___

### BaseAssetsUrl

▪ `Static` **BaseAssetsUrl**: `string` = `"https://assets.babylonjs.com/particles"`

Gets or sets base Assets URL

#### Defined in

https://github.com/babylon.js/core/src/Particles/particleSystemSet.ts:27

## Accessors

### emitterNode

• `get` **emitterNode**(): [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md) \| [`Vector3`](Vector3.md)

Gets or sets the emitter node used with this set

#### Returns

[`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md) \| [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Particles/particleSystemSet.ts:41

• `set` **emitterNode**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md) \| [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/particleSystemSet.ts:45

## Methods

### dispose

▸ **dispose**(): `void`

Release all associated resources

#### Returns

`void`

#### Implementation of

[IDisposable](../interfaces/IDisposable.md).[dispose](../interfaces/IDisposable.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Particles/particleSystemSet.ts:114

___

### serialize

▸ **serialize**(`serializeTexture?`): `any`

Serialize the set into a JSON compatible object

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `serializeTexture` | `boolean` | `false` | defines if the texture must be serialized as well |

#### Returns

`any`

a JSON compatible representation of the set

#### Defined in

https://github.com/babylon.js/core/src/Particles/particleSystemSet.ts:134

___

### setEmitterAsSphere

▸ **setEmitterAsSphere**(`options`, `renderingGroupId`, `scene`): `void`

Creates a new emitter mesh as a sphere

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | `Object` | defines the options used to create the sphere |
| `options.color` | [`Color3`](Color3.md) |  |
| `options.diameter` | `number` |  |
| `options.segments` | `number` |  |
| `renderingGroupId` | `number` | defines the renderingGroupId to use for the sphere |
| `scene` | [`Scene`](Scene.md) | defines the hosting scene |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/particleSystemSet.ts:69

___

### start

▸ **start**(`emitter?`): `void`

Starts all particle systems of the set

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `emitter?` | [`AbstractMesh`](AbstractMesh.md) | defines an optional mesh to use as emitter for the particle systems |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/particleSystemSet.ts:102

___

### Parse

▸ `Static` **Parse**(`data`, `scene`, `gpu?`, `capacity?`): [`ParticleSystemSet`](ParticleSystemSet.md)

Parse a new ParticleSystemSet from a serialized source

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `data` | `any` | `undefined` | defines a JSON compatible representation of the set |
| `scene` | [`Scene`](Scene.md) | `undefined` | defines the hosting scene |
| `gpu` | `boolean` | `false` | defines if we want GPU particles or CPU particles |
| `capacity?` | `number` | `undefined` | defines the system capacity (if null or undefined the sotred capacity will be used) |

#### Returns

[`ParticleSystemSet`](ParticleSystemSet.md)

a new ParticleSystemSet

#### Defined in

https://github.com/babylon.js/core/src/Particles/particleSystemSet.ts:157
