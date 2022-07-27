[@dev/core](../README.md) / [Exports](../modules.md) / DistanceJointData

# Interface: DistanceJointData

Joint data for a Distance-Joint

**`See`**

https://doc.babylonjs.com/how_to/using_the_physics_engine

## Hierarchy

- [`PhysicsJointData`](PhysicsJointData.md)

  ↳ **`DistanceJointData`**

## Table of contents

### Properties

- [collision](DistanceJointData.md#collision)
- [connectedAxis](DistanceJointData.md#connectedaxis)
- [connectedPivot](DistanceJointData.md#connectedpivot)
- [mainAxis](DistanceJointData.md#mainaxis)
- [mainPivot](DistanceJointData.md#mainpivot)
- [maxDistance](DistanceJointData.md#maxdistance)
- [nativeParams](DistanceJointData.md#nativeparams)

## Properties

### collision

• `Optional` **collision**: `boolean`

The collision of the joint

#### Inherited from

[PhysicsJointData](PhysicsJointData.md).[collision](PhysicsJointData.md#collision)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:28

___

### connectedAxis

• `Optional` **connectedAxis**: [`Vector3`](../classes/Vector3.md)

The connected axis of the joint

#### Inherited from

[PhysicsJointData](PhysicsJointData.md).[connectedAxis](PhysicsJointData.md#connectedaxis)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:24

___

### connectedPivot

• `Optional` **connectedPivot**: [`Vector3`](../classes/Vector3.md)

The connected pivot of the joint

#### Inherited from

[PhysicsJointData](PhysicsJointData.md).[connectedPivot](PhysicsJointData.md#connectedpivot)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:16

___

### mainAxis

• `Optional` **mainAxis**: [`Vector3`](../classes/Vector3.md)

The main axis of the joint

#### Inherited from

[PhysicsJointData](PhysicsJointData.md).[mainAxis](PhysicsJointData.md#mainaxis)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:20

___

### mainPivot

• `Optional` **mainPivot**: [`Vector3`](../classes/Vector3.md)

The main pivot of the joint

#### Inherited from

[PhysicsJointData](PhysicsJointData.md).[mainPivot](PhysicsJointData.md#mainpivot)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:12

___

### maxDistance

• **maxDistance**: `number`

Max distance the 2 joint objects can be apart

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:311

___

### nativeParams

• `Optional` **nativeParams**: `any`

Native Oimo/Cannon/Energy data

#### Inherited from

[PhysicsJointData](PhysicsJointData.md).[nativeParams](PhysicsJointData.md#nativeparams)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:32
