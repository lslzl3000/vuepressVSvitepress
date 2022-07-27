[@dev/core](../README.md) / [Exports](../modules.md) / PhysicsJointData

# Interface: PhysicsJointData

Interface for Physics-Joint data

**`See`**

https://doc.babylonjs.com/how_to/using_the_physics_engine

## Hierarchy

- **`PhysicsJointData`**

  ↳ [`DistanceJointData`](DistanceJointData.md)

  ↳ [`SpringJointData`](SpringJointData.md)

## Table of contents

### Properties

- [collision](PhysicsJointData.md#collision)
- [connectedAxis](PhysicsJointData.md#connectedaxis)
- [connectedPivot](PhysicsJointData.md#connectedpivot)
- [mainAxis](PhysicsJointData.md#mainaxis)
- [mainPivot](PhysicsJointData.md#mainpivot)
- [nativeParams](PhysicsJointData.md#nativeparams)

## Properties

### collision

• `Optional` **collision**: `boolean`

The collision of the joint

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:28

___

### connectedAxis

• `Optional` **connectedAxis**: [`Vector3`](../classes/Vector3.md)

The connected axis of the joint

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:24

___

### connectedPivot

• `Optional` **connectedPivot**: [`Vector3`](../classes/Vector3.md)

The connected pivot of the joint

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:16

___

### mainAxis

• `Optional` **mainAxis**: [`Vector3`](../classes/Vector3.md)

The main axis of the joint

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:20

___

### mainPivot

• `Optional` **mainPivot**: [`Vector3`](../classes/Vector3.md)

The main pivot of the joint

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:12

___

### nativeParams

• `Optional` **nativeParams**: `any`

Native Oimo/Cannon/Energy data

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:32
