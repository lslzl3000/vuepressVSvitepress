[@dev/core](../README.md) / [Exports](../modules.md) / SpringJointData

# Interface: SpringJointData

Joint data from a spring joint

**`See`**

https://doc.babylonjs.com/how_to/using_the_physics_engine

## Hierarchy

- [`PhysicsJointData`](PhysicsJointData.md)

  ↳ **`SpringJointData`**

## Table of contents

### Properties

- [collision](SpringJointData.md#collision)
- [connectedAxis](SpringJointData.md#connectedaxis)
- [connectedPivot](SpringJointData.md#connectedpivot)
- [damping](SpringJointData.md#damping)
- [forceApplicationCallback](SpringJointData.md#forceapplicationcallback)
- [length](SpringJointData.md#length)
- [mainAxis](SpringJointData.md#mainaxis)
- [mainPivot](SpringJointData.md#mainpivot)
- [nativeParams](SpringJointData.md#nativeparams)
- [stiffness](SpringJointData.md#stiffness)

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

### damping

• **damping**: `number`

Damping of the spring

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:332

___

### forceApplicationCallback

• **forceApplicationCallback**: () => `void`

#### Type declaration

▸ (): `void`

this callback will be called when applying the force to the impostors.

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:334

___

### length

• **length**: `number`

Length of the spring

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:324

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

### nativeParams

• `Optional` **nativeParams**: `any`

Native Oimo/Cannon/Energy data

#### Inherited from

[PhysicsJointData](PhysicsJointData.md).[nativeParams](PhysicsJointData.md#nativeparams)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:32

___

### stiffness

• **stiffness**: `number`

Stiffness of the spring

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsJoint.ts:328
