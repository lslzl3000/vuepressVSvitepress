[@dev/core](../README.md) / [Exports](../modules.md) / MotorEnabledJoint

# Class: MotorEnabledJoint

Represents a Motor-Enabled Joint

**`See`**

https://doc.babylonjs.com/how_to/using_the_physics_engine

## Hierarchy

- [`PhysicsJoint`](PhysicsJoint.md)

  ↳ **`MotorEnabledJoint`**

  ↳↳ [`HingeJoint`](HingeJoint.md)

  ↳↳ [`Hinge2Joint`](Hinge2Joint.md)

## Implements

- [`IMotorEnabledJoint`](../interfaces/IMotorEnabledJoint.md)

## Table of contents

### Constructors

- [constructor](MotorEnabledJoint.md#constructor)

### Properties

- [\_physicsPlugin](MotorEnabledJoint.md#_physicsplugin)
- [jointData](MotorEnabledJoint.md#jointdata)
- [type](MotorEnabledJoint.md#type)
- [BallAndSocketJoint](MotorEnabledJoint.md#ballandsocketjoint)
- [DistanceJoint](MotorEnabledJoint.md#distancejoint)
- [Hinge2Joint](MotorEnabledJoint.md#hinge2joint)
- [HingeJoint](MotorEnabledJoint.md#hingejoint)
- [LockJoint](MotorEnabledJoint.md#lockjoint)
- [PointToPointJoint](MotorEnabledJoint.md#pointtopointjoint)
- [PrismaticJoint](MotorEnabledJoint.md#prismaticjoint)
- [SliderJoint](MotorEnabledJoint.md#sliderjoint)
- [SpringJoint](MotorEnabledJoint.md#springjoint)
- [UniversalJoint](MotorEnabledJoint.md#universaljoint)
- [WheelJoint](MotorEnabledJoint.md#wheeljoint)

### Accessors

- [physicsJoint](MotorEnabledJoint.md#physicsjoint)
- [physicsPlugin](MotorEnabledJoint.md#physicsplugin)

### Methods

- [executeNativeFunction](MotorEnabledJoint.md#executenativefunction)
- [setLimit](MotorEnabledJoint.md#setlimit)
- [setMotor](MotorEnabledJoint.md#setmotor)

## Constructors

### constructor

• **new MotorEnabledJoint**(`type`, `jointData`)

Initializes the Motor-Enabled Joint

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | `number` | The type of the joint |
| `jointData` | [`PhysicsJointData`](../interfaces/PhysicsJointData.md) | The physical joint data for the joint |

#### Overrides

[PhysicsJoint](PhysicsJoint.md).[constructor](PhysicsJoint.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:183

## Properties

### \_physicsPlugin

• `Protected` **\_physicsPlugin**: `IPhysicsEnginePlugin`

#### Inherited from

[PhysicsJoint](PhysicsJoint.md).[_physicsPlugin](PhysicsJoint.md#_physicsplugin)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:42

___

### jointData

• **jointData**: [`PhysicsJointData`](../interfaces/PhysicsJointData.md)

#### Inherited from

[PhysicsJoint](PhysicsJoint.md).[jointData](PhysicsJoint.md#jointdata)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:57

___

### type

• **type**: `number`

#### Inherited from

[PhysicsJoint](PhysicsJoint.md).[type](PhysicsJoint.md#type)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:53

___

### BallAndSocketJoint

▪ `Static` **BallAndSocketJoint**: `number` = `2`

Ball-and-Socket joint type

#### Inherited from

[PhysicsJoint](PhysicsJoint.md).[BallAndSocketJoint](PhysicsJoint.md#ballandsocketjoint)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:110

___

### DistanceJoint

▪ `Static` **DistanceJoint**: `number` = `0`

Distance-Joint type

#### Inherited from

[PhysicsJoint](PhysicsJoint.md).[DistanceJoint](PhysicsJoint.md#distancejoint)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:102

___

### Hinge2Joint

▪ `Static` **Hinge2Joint**: `number` = `PhysicsJoint.WheelJoint`

Hinge-Joint 2 type

#### Inherited from

[PhysicsJoint](PhysicsJoint.md).[Hinge2Joint](PhysicsJoint.md#hinge2joint)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:133

___

### HingeJoint

▪ `Static` **HingeJoint**: `number` = `1`

Hinge-Joint type

#### Inherited from

[PhysicsJoint](PhysicsJoint.md).[HingeJoint](PhysicsJoint.md#hingejoint)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:106

___

### LockJoint

▪ `Static` **LockJoint**: `number` = `10`

Lock-Joint type

#### Inherited from

[PhysicsJoint](PhysicsJoint.md).[LockJoint](PhysicsJoint.md#lockjoint)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:147

___

### PointToPointJoint

▪ `Static` **PointToPointJoint**: `number` = `8`

Point to Point Joint type.  Similar to a Ball-Joint.  Different in parameters

#### Inherited from

[PhysicsJoint](PhysicsJoint.md).[PointToPointJoint](PhysicsJoint.md#pointtopointjoint)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:138

___

### PrismaticJoint

▪ `Static` **PrismaticJoint**: `number` = `5`

Prismatic-Joint type

#### Inherited from

[PhysicsJoint](PhysicsJoint.md).[PrismaticJoint](PhysicsJoint.md#prismaticjoint)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:123

___

### SliderJoint

▪ `Static` **SliderJoint**: `number` = `4`

Slider-Joint type

#### Inherited from

[PhysicsJoint](PhysicsJoint.md).[SliderJoint](PhysicsJoint.md#sliderjoint)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:118

___

### SpringJoint

▪ `Static` **SpringJoint**: `number` = `9`

Spring-Joint type

#### Inherited from

[PhysicsJoint](PhysicsJoint.md).[SpringJoint](PhysicsJoint.md#springjoint)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:143

___

### UniversalJoint

▪ `Static` **UniversalJoint**: `number` = `6`

Universal-Joint type
ENERGY FTW! (compare with this -

**`See`**

http://ode-wiki.org/wiki/index.php?title=Manual:_Joint_Types_and_Functions)

#### Inherited from

[PhysicsJoint](PhysicsJoint.md).[UniversalJoint](PhysicsJoint.md#universaljoint)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:129

___

### WheelJoint

▪ `Static` **WheelJoint**: `number` = `3`

Wheel-Joint type

#### Inherited from

[PhysicsJoint](PhysicsJoint.md).[WheelJoint](PhysicsJoint.md#wheeljoint)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:114

## Accessors

### physicsJoint

• `get` **physicsJoint**(): `any`

Gets the physics joint

#### Returns

`any`

#### Implementation of

[IMotorEnabledJoint](../interfaces/IMotorEnabledJoint.md).[physicsJoint](../interfaces/IMotorEnabledJoint.md#physicsjoint)

#### Inherited from

PhysicsJoint.physicsJoint

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:65

• `set` **physicsJoint**(`newJoint`): `void`

Sets the physics joint

#### Parameters

| Name | Type |
| :------ | :------ |
| `newJoint` | `any` |

#### Returns

`void`

#### Implementation of

[IMotorEnabledJoint](../interfaces/IMotorEnabledJoint.md).[physicsJoint](../interfaces/IMotorEnabledJoint.md#physicsjoint)

#### Inherited from

PhysicsJoint.physicsJoint

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:72

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

#### Inherited from

PhysicsJoint.physicsPlugin

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:83

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

#### Inherited from

[PhysicsJoint](PhysicsJoint.md).[executeNativeFunction](PhysicsJoint.md#executenativefunction)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:92

___

### setLimit

▸ **setLimit**(`upperLimit`, `lowerLimit?`): `void`

Set the motor's limits.
Attention, this function is plugin specific. Engines won't react 100% the same.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `upperLimit` | `number` | The upper limit of the motor |
| `lowerLimit?` | `number` | The lower limit of the motor |

#### Returns

`void`

#### Implementation of

[IMotorEnabledJoint](../interfaces/IMotorEnabledJoint.md).[setLimit](../interfaces/IMotorEnabledJoint.md#setlimit)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:203

___

### setMotor

▸ **setMotor**(`force?`, `maxForce?`): `void`

Set the motor values.
Attention, this function is plugin specific. Engines won't react 100% the same.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `force?` | `number` | the force to apply |
| `maxForce?` | `number` | max force for this motor. |

#### Returns

`void`

#### Implementation of

[IMotorEnabledJoint](../interfaces/IMotorEnabledJoint.md).[setMotor](../interfaces/IMotorEnabledJoint.md#setmotor)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:193
