[@dev/core](../README.md) / [Exports](../modules.md) / PhysicsRadialExplosionEventOptions

# Class: PhysicsRadialExplosionEventOptions

Options fot the radial explosion event

**`See`**

https://doc.babylonjs.com/how_to/using_the_physics_engine#further-functionality-of-the-impostor-class

## Table of contents

### Constructors

- [constructor](PhysicsRadialExplosionEventOptions.md#constructor)

### Properties

- [affectedImpostorsCallback](PhysicsRadialExplosionEventOptions.md#affectedimpostorscallback)
- [falloff](PhysicsRadialExplosionEventOptions.md#falloff)
- [radius](PhysicsRadialExplosionEventOptions.md#radius)
- [sphere](PhysicsRadialExplosionEventOptions.md#sphere)
- [strength](PhysicsRadialExplosionEventOptions.md#strength)

## Constructors

### constructor

• **new PhysicsRadialExplosionEventOptions**()

## Properties

### affectedImpostorsCallback

• **affectedImpostorsCallback**: (`affectedImpostorsWithData`: [`PhysicsAffectedImpostorWithData`](../interfaces/PhysicsAffectedImpostorWithData.md)[]) => `void`

#### Type declaration

▸ (`affectedImpostorsWithData`): `void`

Sphere options for the radial explosion.

##### Parameters

| Name | Type |
| :------ | :------ |
| `affectedImpostorsWithData` | [`PhysicsAffectedImpostorWithData`](../interfaces/PhysicsAffectedImpostorWithData.md)[] |

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsHelper.ts:789

___

### falloff

• **falloff**: [`PhysicsRadialImpulseFalloff`](../enums/PhysicsRadialImpulseFalloff.md) = `PhysicsRadialImpulseFalloff.Constant`

The strength of the force in correspondence to the distance of the affected object

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsHelper.ts:779

___

### radius

• **radius**: `number` = `5`

The radius of the sphere for the radial explosion.

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsHelper.ts:769

___

### sphere

• **sphere**: `Object`

Sphere options for the radial explosion.

#### Type declaration

| Name | Type |
| :------ | :------ |
| `diameter` | `number` |
| `segments` | `number` |

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsHelper.ts:784

___

### strength

• **strength**: `number` = `10`

The strength of the explosion.

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsHelper.ts:774
