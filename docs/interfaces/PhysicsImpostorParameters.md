[@dev/core](../README.md) / [Exports](../modules.md) / PhysicsImpostorParameters

# Interface: PhysicsImpostorParameters

The interface for the physics imposter parameters

**`See`**

https://doc.babylonjs.com/how_to/using_the_physics_engine

## Table of contents

### Properties

- [damping](PhysicsImpostorParameters.md#damping)
- [disableBidirectionalTransformation](PhysicsImpostorParameters.md#disablebidirectionaltransformation)
- [fixedPoints](PhysicsImpostorParameters.md#fixedpoints)
- [friction](PhysicsImpostorParameters.md#friction)
- [ignoreParent](PhysicsImpostorParameters.md#ignoreparent)
- [margin](PhysicsImpostorParameters.md#margin)
- [mass](PhysicsImpostorParameters.md#mass)
- [nativeOptions](PhysicsImpostorParameters.md#nativeoptions)
- [path](PhysicsImpostorParameters.md#path)
- [positionIterations](PhysicsImpostorParameters.md#positioniterations)
- [pressure](PhysicsImpostorParameters.md#pressure)
- [restitution](PhysicsImpostorParameters.md#restitution)
- [shape](PhysicsImpostorParameters.md#shape)
- [stiffness](PhysicsImpostorParameters.md#stiffness)
- [velocityIterations](PhysicsImpostorParameters.md#velocityiterations)

## Properties

### damping

• `Optional` **damping**: `number`

The collision margin around a soft object

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsImpostor.ts:75

___

### disableBidirectionalTransformation

• `Optional` **disableBidirectionalTransformation**: `boolean`

Specifies if bi-directional transformations should be disabled

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsImpostor.ts:45

___

### fixedPoints

• `Optional` **fixedPoints**: `number`

The number used to fix points on a cloth (0, 1, 2, 4, 8) or rope (0, 1, 2) only
0 None, 1, back left or top, 2, back right or bottom, 4, front left, 8, front right
Add to fix multiple points

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsImpostor.ts:67

___

### friction

• `Optional` **friction**: `number`

The friction of the physics imposter

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsImpostor.ts:29

___

### ignoreParent

• `Optional` **ignoreParent**: `boolean`

Specifies if the parent should be ignored

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsImpostor.ts:41

___

### margin

• `Optional` **margin**: `number`

The collision margin around a soft object

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsImpostor.ts:71

___

### mass

• **mass**: `number`

The mass of the physics imposter

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsImpostor.ts:25

___

### nativeOptions

• `Optional` **nativeOptions**: `any`

The native options of the physics imposter

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsImpostor.ts:37

___

### path

• `Optional` **path**: `any`

The path for a rope based on an extrusion

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsImpostor.ts:79

___

### positionIterations

• `Optional` **positionIterations**: `number`

The number of iterations used in maintaining consistent vertex positions, soft object only

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsImpostor.ts:61

___

### pressure

• `Optional` **pressure**: `number`

The pressure inside the physics imposter, soft object only

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsImpostor.ts:49

___

### restitution

• `Optional` **restitution**: `number`

The coefficient of restitution of the physics imposter

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsImpostor.ts:33

___

### shape

• `Optional` **shape**: `any`

The shape of an extrusion used for a rope based on an extrusion

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsImpostor.ts:83

___

### stiffness

• `Optional` **stiffness**: `number`

The stiffness the physics imposter, soft object only

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsImpostor.ts:53

___

### velocityIterations

• `Optional` **velocityIterations**: `number`

The number of iterations used in maintaining consistent vertex velocities, soft object only

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsImpostor.ts:57
