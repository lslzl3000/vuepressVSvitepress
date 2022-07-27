[@dev/core](../README.md) / [Exports](../modules.md) / DistanceJoint

# Class: DistanceJoint

A class representing a physics distance joint

**`See`**

https://doc.babylonjs.com/how_to/using_the_physics_engine

## Hierarchy

- [`PhysicsJoint`](PhysicsJoint.md)

  ↳ **`DistanceJoint`**

## Table of contents

### Constructors

- [constructor](DistanceJoint.md#constructor)

### Properties

- [\_physicsPlugin](DistanceJoint.md#_physicsplugin)
- [jointData](DistanceJoint.md#jointdata)
- [type](DistanceJoint.md#type)
- [BallAndSocketJoint](DistanceJoint.md#ballandsocketjoint)
- [DistanceJoint](DistanceJoint.md#distancejoint)
- [Hinge2Joint](DistanceJoint.md#hinge2joint)
- [HingeJoint](DistanceJoint.md#hingejoint)
- [LockJoint](DistanceJoint.md#lockjoint)
- [PointToPointJoint](DistanceJoint.md#pointtopointjoint)
- [PrismaticJoint](DistanceJoint.md#prismaticjoint)
- [SliderJoint](DistanceJoint.md#sliderjoint)
- [SpringJoint](DistanceJoint.md#springjoint)
- [UniversalJoint](DistanceJoint.md#universaljoint)
- [WheelJoint](DistanceJoint.md#wheeljoint)

### Accessors

- [physicsJoint](DistanceJoint.md#physicsjoint)
- [physicsPlugin](DistanceJoint.md#physicsplugin)

### Methods

- [executeNativeFunction](DistanceJoint.md#executenativefunction)
- [updateDistance](DistanceJoint.md#updatedistance)

## Constructors

### constructor

• **new DistanceJoint**(`jointData`)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `jointData` | [`DistanceJointData`](../interfaces/DistanceJointData.md) | The data for the Distance-Joint |

#### Overrides

[PhysicsJoint](PhysicsJoint.md).[constructor](PhysicsJoint.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:159

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

### updateDistance

▸ **updateDistance**(`maxDistance`, `minDistance?`): `void`

Update the predefined distance.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `maxDistance` | `number` | The maximum preferred distance |
| `minDistance?` | `number` | The minimum preferred distance |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:168
