[@dev/core](../README.md) / [Exports](../modules.md) / PhysicsVortexEventOptions

# Class: PhysicsVortexEventOptions

Options fot the vortex event

**`See`**

https://doc.babylonjs.com/how_to/using_the_physics_engine#further-functionality-of-the-impostor-class

## Table of contents

### Constructors

- [constructor](PhysicsVortexEventOptions.md#constructor)

### Properties

- [centrifugalForceMultiplier](PhysicsVortexEventOptions.md#centrifugalforcemultiplier)
- [centripetalForceMultiplier](PhysicsVortexEventOptions.md#centripetalforcemultiplier)
- [centripetalForceThreshold](PhysicsVortexEventOptions.md#centripetalforcethreshold)
- [height](PhysicsVortexEventOptions.md#height)
- [radius](PhysicsVortexEventOptions.md#radius)
- [strength](PhysicsVortexEventOptions.md#strength)
- [updraftForceMultiplier](PhysicsVortexEventOptions.md#updraftforcemultiplier)

## Constructors

### constructor

• **new PhysicsVortexEventOptions**()

## Properties

### centrifugalForceMultiplier

• **centrifugalForceMultiplier**: `number` = `0.5`

This multiplier determines with how much force the objects will be pushed sideways/around the vortex, when above the threshold.

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsHelper.ts:851

___

### centripetalForceMultiplier

• **centripetalForceMultiplier**: `number` = `5`

This multiplier determines with how much force the objects will be pushed sideways/around the vortex, when below the threshold.

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsHelper.ts:846

___

### centripetalForceThreshold

• **centripetalForceThreshold**: `number` = `0.7`

At which distance, relative to the radius the centripetal forces should kick in? Range: 0-1

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsHelper.ts:841

___

### height

• **height**: `number` = `10`

The height of the cylinder for the vortex.

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsHelper.ts:836

___

### radius

• **radius**: `number` = `5`

The radius of the cylinder for the vortex

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsHelper.ts:826

___

### strength

• **strength**: `number` = `10`

The strength of the vortex.

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsHelper.ts:831

___

### updraftForceMultiplier

• **updraftForceMultiplier**: `number` = `0.02`

This multiplier determines with how much force the objects will be pushed upwards, when in the vortex.

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsHelper.ts:856
