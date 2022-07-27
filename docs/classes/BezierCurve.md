[@dev/core](../README.md) / [Exports](../modules.md) / BezierCurve

# Class: BezierCurve

Class used to represent a Bezier curve

## Table of contents

### Constructors

- [constructor](BezierCurve.md#constructor)

### Methods

- [Interpolate](BezierCurve.md#interpolate)

## Constructors

### constructor

• **new BezierCurve**()

## Methods

### Interpolate

▸ `Static` **Interpolate**(`t`, `x1`, `y1`, `x2`, `y2`): `number`

Returns the cubic Bezier interpolated value (float) at "t" (float) from the given x1, y1, x2, y2 floats

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `t` | `number` | defines the time |
| `x1` | `number` | defines the left coordinate on X axis |
| `y1` | `number` | defines the left coordinate on Y axis |
| `x2` | `number` | defines the right coordinate on X axis |
| `y2` | `number` | defines the right coordinate on Y axis |

#### Returns

`number`

the interpolated value

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:29
