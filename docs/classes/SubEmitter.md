[@dev/core](../README.md) / [Exports](../modules.md) / SubEmitter

# Class: SubEmitter

Sub emitter class used to emit particles from an existing particle

## Table of contents

### Constructors

- [constructor](SubEmitter.md#constructor)

### Properties

- [inheritDirection](SubEmitter.md#inheritdirection)
- [inheritedVelocityAmount](SubEmitter.md#inheritedvelocityamount)
- [particleSystem](SubEmitter.md#particlesystem)
- [type](SubEmitter.md#type)

### Methods

- [clone](SubEmitter.md#clone)
- [dispose](SubEmitter.md#dispose)
- [serialize](SubEmitter.md#serialize)
- [Parse](SubEmitter.md#parse)

## Constructors

### constructor

• **new SubEmitter**(`particleSystem`)

Creates a sub emitter

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `particleSystem` | [`ParticleSystem`](ParticleSystem.md) | the particle system to be used by the sub emitter |

#### Defined in

https://github.com/babylon.js/core/src/Particles/subEmitter.ts:46

## Properties

### inheritDirection

• **inheritDirection**: `boolean` = `false`

If the particle should inherit the direction from the particle it's attached to. (+Y will face the direction the particle is moving) (Default: false)
Note: This only is supported when using an emitter of type Mesh

#### Defined in

https://github.com/babylon.js/core/src/Particles/subEmitter.ts:36

___

### inheritedVelocityAmount

• **inheritedVelocityAmount**: `number` = `0`

How much of the attached particles speed should be added to the sub emitted particle (default: 0)

#### Defined in

https://github.com/babylon.js/core/src/Particles/subEmitter.ts:40

___

### particleSystem

• **particleSystem**: [`ParticleSystem`](ParticleSystem.md)

#### Defined in

https://github.com/babylon.js/core/src/Particles/subEmitter.ts:50

___

### type

• **type**: [`SubEmitterType`](../enums/SubEmitterType.md) = `SubEmitterType.END`

Type of the submitter (Default: END)

#### Defined in

https://github.com/babylon.js/core/src/Particles/subEmitter.ts:31

## Methods

### clone

▸ **clone**(): [`SubEmitter`](SubEmitter.md)

Clones the sub emitter

#### Returns

[`SubEmitter`](SubEmitter.md)

the cloned sub emitter

#### Defined in

https://github.com/babylon.js/core/src/Particles/subEmitter.ts:63

___

### dispose

▸ **dispose**(): `void`

Release associated resources

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Particles/subEmitter.ts:135

___

### serialize

▸ **serialize**(`serializeTexture?`): `any`

Serialize current object to a JSON object

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `serializeTexture` | `boolean` | `false` | defines if the texture must be serialized as well |

#### Returns

`any`

the serialized object

#### Defined in

https://github.com/babylon.js/core/src/Particles/subEmitter.ts:93

___

### Parse

▸ `Static` **Parse**(`serializationObject`, `sceneOrEngine`, `rootUrl`): [`SubEmitter`](SubEmitter.md)

Creates a new SubEmitter from a serialized JSON version

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `serializationObject` | `any` | defines the JSON object to read from |
| `sceneOrEngine` | [`Scene`](Scene.md) \| [`ThinEngine`](ThinEngine.md) | defines the hosting scene or the hosting engine |
| `rootUrl` | `string` | defines the rootUrl for data loading |

#### Returns

[`SubEmitter`](SubEmitter.md)

a new SubEmitter

#### Defined in

https://github.com/babylon.js/core/src/Particles/subEmitter.ts:123
