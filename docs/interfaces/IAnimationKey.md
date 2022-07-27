[@dev/core](../README.md) / [Exports](../modules.md) / IAnimationKey

# Interface: IAnimationKey

Defines an interface which represents an animation key frame

## Table of contents

### Properties

- [frame](IAnimationKey.md#frame)
- [inTangent](IAnimationKey.md#intangent)
- [interpolation](IAnimationKey.md#interpolation)
- [lockedTangent](IAnimationKey.md#lockedtangent)
- [outTangent](IAnimationKey.md#outtangent)
- [value](IAnimationKey.md#value)

## Properties

### frame

• **frame**: `number`

Frame of the key frame

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationKey.ts:8

___

### inTangent

• `Optional` **inTangent**: `any`

The input tangent for the cubic hermite spline

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationKey.ts:16

___

### interpolation

• `Optional` **interpolation**: [`AnimationKeyInterpolation`](../enums/AnimationKeyInterpolation.md)

The animation interpolation type

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationKey.ts:24

___

### lockedTangent

• `Optional` **lockedTangent**: `boolean`

Property defined by UI tools to link (or not ) the tangents

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationKey.ts:28

___

### outTangent

• `Optional` **outTangent**: `any`

The output tangent for the cubic hermite spline

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationKey.ts:20

___

### value

• **value**: `any`

Value at the specifies key frame

#### Defined in

https://github.com/babylon.js/core/src/Animations/animationKey.ts:12
