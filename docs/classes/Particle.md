[@dev/core](../README.md) / [Exports](../modules.md) / Particle

# Class: Particle

A particle represents one of the element emitted by a particle system.
This is mainly define by its coordinates, direction, velocity and age.

## Table of contents

### Constructors

- [constructor](Particle.md#constructor)

### Properties

- [age](Particle.md#age)
- [angle](Particle.md#angle)
- [angularSpeed](Particle.md#angularspeed)
- [cellIndex](Particle.md#cellindex)
- [color](Particle.md#color)
- [colorStep](Particle.md#colorstep)
- [direction](Particle.md#direction)
- [id](Particle.md#id)
- [lifeTime](Particle.md#lifetime)
- [particleSystem](Particle.md#particlesystem)
- [position](Particle.md#position)
- [remapData](Particle.md#remapdata)
- [scale](Particle.md#scale)
- [size](Particle.md#size)
- [\_Count](Particle.md#_count)

### Methods

- [\_updateCellInfoFromSystem](Particle.md#_updatecellinfofromsystem)
- [copyTo](Particle.md#copyto)
- [updateCellIndex](Particle.md#updatecellindex)

## Constructors

### constructor

• **new Particle**(`particleSystem`)

Creates a new instance Particle

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `particleSystem` | [`ParticleSystem`](ParticleSystem.md) | the particle system the particle belongs to |

#### Defined in

packages/dev/core/src/Particles/particle.ts:151

## Properties

### age

• **age**: `number` = `0`

The current age of the particle.

#### Defined in

packages/dev/core/src/Particles/particle.ts:49

___

### angle

• **angle**: `number` = `0`

The current angle of the particle.

#### Defined in

packages/dev/core/src/Particles/particle.ts:64

___

### angularSpeed

• **angularSpeed**: `number` = `0`

Defines how fast is the angle changing.

#### Defined in

packages/dev/core/src/Particles/particle.ts:69

___

### cellIndex

• **cellIndex**: `number` = `0`

Defines the cell index used by the particle to be rendered from a sprite.

#### Defined in

packages/dev/core/src/Particles/particle.ts:74

___

### color

• **color**: [`Color4`](Color4.md)

The color of the particle.

#### Defined in

packages/dev/core/src/Particles/particle.ts:34

___

### colorStep

• **colorStep**: [`Color4`](Color4.md)

The color change of the particle per step.

#### Defined in

packages/dev/core/src/Particles/particle.ts:39

___

### direction

• **direction**: [`Vector3`](Vector3.md)

The world direction of the particle in the scene.

#### Defined in

packages/dev/core/src/Particles/particle.ts:29

___

### id

• **id**: `number`

Unique ID of the particle

#### Defined in

packages/dev/core/src/Particles/particle.ts:20

___

### lifeTime

• **lifeTime**: `number` = `1.0`

Defines how long will the life of the particle be.

#### Defined in

packages/dev/core/src/Particles/particle.ts:44

___

### particleSystem

• **particleSystem**: [`ParticleSystem`](ParticleSystem.md)

#### Defined in

packages/dev/core/src/Particles/particle.ts:155

___

### position

• **position**: [`Vector3`](Vector3.md)

The world position of the particle in the scene.

#### Defined in

packages/dev/core/src/Particles/particle.ts:24

___

### remapData

• **remapData**: [`Vector4`](Vector4.md)

The information required to support color remapping

#### Defined in

packages/dev/core/src/Particles/particle.ts:79

___

### scale

• **scale**: [`Vector2`](Vector2.md)

The current scale of the particle.

#### Defined in

packages/dev/core/src/Particles/particle.ts:59

___

### size

• **size**: `number` = `0`

The current size of the particle.

#### Defined in

packages/dev/core/src/Particles/particle.ts:54

___

### \_Count

▪ `Static` `Private` **\_Count**: `number` = `0`

#### Defined in

packages/dev/core/src/Particles/particle.ts:16

## Methods

### \_updateCellInfoFromSystem

▸ `Private` **_updateCellInfoFromSystem**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Particles/particle.ts:165

___

### copyTo

▸ **copyTo**(`other`): `void`

Copy the properties of particle to another one.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`Particle`](Particle.md) | the particle to copy the information to. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Particles/particle.ts:249

___

### updateCellIndex

▸ **updateCellIndex**(): `void`

Defines how the sprite cell index is updated for the particle

#### Returns

`void`

#### Defined in

packages/dev/core/src/Particles/particle.ts:172
