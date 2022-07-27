[@dev/core](../README.md) / [Exports](../modules.md) / PhysicsJoint

# Class: PhysicsJoint

This is a holder class for the physics joint created by the physics plugin
It holds a set of functions to control the underlying joint

**`See`**

https://doc.babylonjs.com/how_to/using_the_physics_engine

## Hierarchy

- **`PhysicsJoint`**

  ↳ [`DistanceJoint`](DistanceJoint.md)

  ↳ [`MotorEnabledJoint`](MotorEnabledJoint.md)

## Table of contents

### Constructors

- [constructor](PhysicsJoint.md#constructor)

### Properties

- [\_physicsJoint](PhysicsJoint.md#_physicsjoint)
- [\_physicsPlugin](PhysicsJoint.md#_physicsplugin)
- [jointData](PhysicsJoint.md#jointdata)
- [type](PhysicsJoint.md#type)
- [BallAndSocketJoint](PhysicsJoint.md#ballandsocketjoint)
- [DistanceJoint](PhysicsJoint.md#distancejoint)
- [Hinge2Joint](PhysicsJoint.md#hinge2joint)
- [HingeJoint](PhysicsJoint.md#hingejoint)
- [LockJoint](PhysicsJoint.md#lockjoint)
- [PointToPointJoint](PhysicsJoint.md#pointtopointjoint)
- [PrismaticJoint](PhysicsJoint.md#prismaticjoint)
- [SliderJoint](PhysicsJoint.md#sliderjoint)
- [SpringJoint](PhysicsJoint.md#springjoint)
- [UniversalJoint](PhysicsJoint.md#universaljoint)
- [WheelJoint](PhysicsJoint.md#wheeljoint)

### Accessors

- [physicsJoint](PhysicsJoint.md#physicsjoint)
- [physicsPlugin](PhysicsJoint.md#physicsplugin)

### Methods

- [executeNativeFunction](PhysicsJoint.md#executenativefunction)

## Constructors

### constructor

• **new PhysicsJoint**(`type`, `jointData`)

Initializes the physics joint

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | `number` | The type of the physics joint |
| `jointData` | [`PhysicsJointData`](../interfaces/PhysicsJointData.md) | The data for the physics joint |

#### Defined in

packages/dev/core/src/Physics/physicsJoint.ts:49

## Properties

### \_physicsJoint

• `Private` **\_physicsJoint**: `any`

#### Defined in

packages/dev/core/src/Physics/physicsJoint.ts:41

___

### \_physicsPlugin

• `Protected` **\_physicsPlugin**: `IPhysicsEnginePlugin`

#### Defined in

packages/dev/core/src/Physics/physicsJoint.ts:42

___

### jointData

• **jointData**: [`PhysicsJointData`](../interfaces/PhysicsJointData.md)

#### Defined in

packages/dev/core/src/Physics/physicsJoint.ts:57

___

### type

• **type**: `number`

#### Defined in

packages/dev/core/src/Physics/physicsJoint.ts:53

___

### BallAndSocketJoint

▪ `Static` **BallAndSocketJoint**: `number` = `2`

Ball-and-Socket joint type

#### Defined in

packages/dev/core/src/Physics/physicsJoint.ts:110

___

### DistanceJoint

▪ `Static` **DistanceJoint**: `number` = `0`

Distance-Joint type

#### Defined in

packages/dev/core/src/Physics/physicsJoint.ts:102

___

### Hinge2Joint

▪ `Static` **Hinge2Joint**: `number` = `PhysicsJoint.WheelJoint`

Hinge-Joint 2 type

#### Defined in

packages/dev/core/src/Physics/physicsJoint.ts:133

___

### HingeJoint

▪ `Static` **HingeJoint**: `number` = `1`

Hinge-Joint type

#### Defined in

packages/dev/core/src/Physics/physicsJoint.ts:106

___

### LockJoint

▪ `Static` **LockJoint**: `number` = `10`

Lock-Joint type

#### Defined in

packages/dev/core/src/Physics/physicsJoint.ts:147

___

### PointToPointJoint

▪ `Static` **PointToPointJoint**: `number` = `8`

Point to Point Joint type.  Similar to a Ball-Joint.  Different in parameters

#### Defined in

packages/dev/core/src/Physics/physicsJoint.ts:138

___

### PrismaticJoint

▪ `Static` **PrismaticJoint**: `number` = `5`

Prismatic-Joint type

#### Defined in

packages/dev/core/src/Physics/physicsJoint.ts:123

___

### SliderJoint

▪ `Static` **SliderJoint**: `number` = `4`

Slider-Joint type

#### Defined in

packages/dev/core/src/Physics/physicsJoint.ts:118

___

### SpringJoint

▪ `Static` **SpringJoint**: `number` = `9`

Spring-Joint type

#### Defined in

packages/dev/core/src/Physics/physicsJoint.ts:143

___

### UniversalJoint

▪ `Static` **UniversalJoint**: `number` = `6`

Universal-Joint type
ENERGY FTW! (compare with this -

**`See`**

http://ode-wiki.org/wiki/index.php?title=Manual:_Joint_Types_and_Functions)

#### Defined in

packages/dev/core/src/Physics/physicsJoint.ts:129

___

### WheelJoint

▪ `Static` **WheelJoint**: `number` = `3`

Wheel-Joint type

#### Defined in

packages/dev/core/src/Physics/physicsJoint.ts:114

## Accessors

### physicsJoint

• `get` **physicsJoint**(): `any`

Gets the physics joint

#### Returns

`any`

#### Defined in

packages/dev/core/src/Physics/physicsJoint.ts:65

• `set` **physicsJoint**(`newJoint`): `void`

Sets the physics joint

#### Parameters

| Name | Type |
| :------ | :------ |
| `newJoint` | `any` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Physics/physicsJoint.ts:72

___

### physicsPlugin

• `set` **physicsPlugin**(`physicsPlugin`): `void`

Sets the physics plugin

#### Parameters

| Name | Type |
| :------ | :------ |
| `physicsPlugin` | `IPhysicsEnginePlugin` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Physics/physicsJoint.ts:83

## Methods

### executeNativeFunction

▸ **executeNativeFunction**(`func`): `void`

Execute a function that is physics-plugin specific.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `func` | (`world`: `any`, `physicsJoint`: `any`) => `void` | the function that will be executed.                         It accepts two parameters: the physics world and the physics joint |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Physics/physicsJoint.ts:92
