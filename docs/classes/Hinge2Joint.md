[@dev/core](../README.md) / [Exports](../modules.md) / Hinge2Joint

# Class: Hinge2Joint

This class represents a dual hinge physics joint (same as wheel joint)

**`See`**

https://doc.babylonjs.com/how_to/using_the_physics_engine

## Hierarchy

- [`MotorEnabledJoint`](MotorEnabledJoint.md)

  ↳ **`Hinge2Joint`**

## Table of contents

### Constructors

- [constructor](Hinge2Joint.md#constructor)

### Properties

- [\_physicsPlugin](Hinge2Joint.md#_physicsplugin)
- [jointData](Hinge2Joint.md#jointdata)
- [type](Hinge2Joint.md#type)
- [BallAndSocketJoint](Hinge2Joint.md#ballandsocketjoint)
- [DistanceJoint](Hinge2Joint.md#distancejoint)
- [Hinge2Joint](Hinge2Joint.md#hinge2joint)
- [HingeJoint](Hinge2Joint.md#hingejoint)
- [LockJoint](Hinge2Joint.md#lockjoint)
- [PointToPointJoint](Hinge2Joint.md#pointtopointjoint)
- [PrismaticJoint](Hinge2Joint.md#prismaticjoint)
- [SliderJoint](Hinge2Joint.md#sliderjoint)
- [SpringJoint](Hinge2Joint.md#springjoint)
- [UniversalJoint](Hinge2Joint.md#universaljoint)
- [WheelJoint](Hinge2Joint.md#wheeljoint)

### Accessors

- [physicsJoint](Hinge2Joint.md#physicsjoint)
- [physicsPlugin](Hinge2Joint.md#physicsplugin)

### Methods

- [executeNativeFunction](Hinge2Joint.md#executenativefunction)
- [setLimit](Hinge2Joint.md#setlimit)
- [setMotor](Hinge2Joint.md#setmotor)

## Constructors

### constructor

• **new Hinge2Joint**(`jointData`)

Initializes the Hinge2-Joint

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `jointData` | [`PhysicsJointData`](../interfaces/PhysicsJointData.md) | The joint data for the Hinge2-Joint |

#### Overrides

[MotorEnabledJoint](MotorEnabledJoint.md).[constructor](MotorEnabledJoint.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:251

## Properties

### \_physicsPlugin

• `Protected` **\_physicsPlugin**: `IPhysicsEnginePlugin`

#### Inherited from

[MotorEnabledJoint](MotorEnabledJoint.md).[_physicsPlugin](MotorEnabledJoint.md#_physicsplugin)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:42

___

### jointData

• **jointData**: [`PhysicsJointData`](../interfaces/PhysicsJointData.md)

#### Inherited from

[MotorEnabledJoint](MotorEnabledJoint.md).[jointData](MotorEnabledJoint.md#jointdata)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:57

___

### type

• **type**: `number`

#### Inherited from

[MotorEnabledJoint](MotorEnabledJoint.md).[type](MotorEnabledJoint.md#type)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:53

___

### BallAndSocketJoint

▪ `Static` **BallAndSocketJoint**: `number` = `2`

Ball-and-Socket joint type

#### Inherited from

[MotorEnabledJoint](MotorEnabledJoint.md).[BallAndSocketJoint](MotorEnabledJoint.md#ballandsocketjoint)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:110

___

### DistanceJoint

▪ `Static` **DistanceJoint**: `number` = `0`

Distance-Joint type

#### Inherited from

[MotorEnabledJoint](MotorEnabledJoint.md).[DistanceJoint](MotorEnabledJoint.md#distancejoint)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:102

___

### Hinge2Joint

▪ `Static` **Hinge2Joint**: `number` = `PhysicsJoint.WheelJoint`

Hinge-Joint 2 type

#### Inherited from

[MotorEnabledJoint](MotorEnabledJoint.md).[Hinge2Joint](MotorEnabledJoint.md#hinge2joint)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:133

___

### HingeJoint

▪ `Static` **HingeJoint**: `number` = `1`

Hinge-Joint type

#### Inherited from

[MotorEnabledJoint](MotorEnabledJoint.md).[HingeJoint](MotorEnabledJoint.md#hingejoint)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:106

___

### LockJoint

▪ `Static` **LockJoint**: `number` = `10`

Lock-Joint type

#### Inherited from

[MotorEnabledJoint](MotorEnabledJoint.md).[LockJoint](MotorEnabledJoint.md#lockjoint)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:147

___

### PointToPointJoint

▪ `Static` **PointToPointJoint**: `number` = `8`

Point to Point Joint type.  Similar to a Ball-Joint.  Different in parameters

#### Inherited from

[MotorEnabledJoint](MotorEnabledJoint.md).[PointToPointJoint](MotorEnabledJoint.md#pointtopointjoint)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:138

___

### PrismaticJoint

▪ `Static` **PrismaticJoint**: `number` = `5`

Prismatic-Joint type

#### Inherited from

[MotorEnabledJoint](MotorEnabledJoint.md).[PrismaticJoint](MotorEnabledJoint.md#prismaticjoint)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:123

___

### SliderJoint

▪ `Static` **SliderJoint**: `number` = `4`

Slider-Joint type

#### Inherited from

[MotorEnabledJoint](MotorEnabledJoint.md).[SliderJoint](MotorEnabledJoint.md#sliderjoint)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:118

___

### SpringJoint

▪ `Static` **SpringJoint**: `number` = `9`

Spring-Joint type

#### Inherited from

[MotorEnabledJoint](MotorEnabledJoint.md).[SpringJoint](MotorEnabledJoint.md#springjoint)

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

[MotorEnabledJoint](MotorEnabledJoint.md).[UniversalJoint](MotorEnabledJoint.md#universaljoint)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:129

___

### WheelJoint

▪ `Static` **WheelJoint**: `number` = `3`

Wheel-Joint type

#### Inherited from

[MotorEnabledJoint](MotorEnabledJoint.md).[WheelJoint](MotorEnabledJoint.md#wheeljoint)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:114

## Accessors

### physicsJoint

• `get` **physicsJoint**(): `any`

Gets the physics joint

#### Returns

`any`

#### Inherited from

MotorEnabledJoint.physicsJoint

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

#### Inherited from

MotorEnabledJoint.physicsJoint

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

MotorEnabledJoint.physicsPlugin

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

[MotorEnabledJoint](MotorEnabledJoint.md).[executeNativeFunction](MotorEnabledJoint.md#executenativefunction)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:92

___

### setLimit

▸ **setLimit**(`upperLimit`, `lowerLimit?`, `motorIndex?`): `void`

Set the motor limits.
Attention, this function is plugin specific. Engines won't react 100% the same.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `upperLimit` | `number` | `undefined` | the upper limit |
| `lowerLimit?` | `number` | `undefined` | lower limit |
| `motorIndex` | `number` | `0` | the motor's index, 0 or 1. |

#### Returns

`void`

#### Overrides

[MotorEnabledJoint](MotorEnabledJoint.md).[setLimit](MotorEnabledJoint.md#setlimit)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:273

___

### setMotor

▸ **setMotor**(`targetSpeed?`, `maxForce?`, `motorIndex?`): `void`

Set the motor values.
Attention, this function is plugin specific. Engines won't react 100% the same.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `targetSpeed?` | `number` | `undefined` | the speed the motor is to reach |
| `maxForce?` | `number` | `undefined` | max force for this motor. |
| `motorIndex` | `number` | `0` | motor's index, 0 or 1. |

#### Returns

`void`

#### Overrides

[MotorEnabledJoint](MotorEnabledJoint.md).[setMotor](MotorEnabledJoint.md#setmotor)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:262
