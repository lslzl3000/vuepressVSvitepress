[@dev/core](../README.md) / [Exports](../modules.md) / Scalar

# Class: Scalar

Scalar computation library

## Table of contents

### Constructors

- [constructor](Scalar.md#constructor)

### Properties

- [TwoPi](Scalar.md#twopi)

### Methods

- [Clamp](Scalar.md#clamp)
- [DeltaAngle](Scalar.md#deltaangle)
- [Denormalize](Scalar.md#denormalize)
- [HCF](Scalar.md#hcf)
- [Hermite](Scalar.md#hermite)
- [Hermite1stDerivative](Scalar.md#hermite1stderivative)
- [ILog2](Scalar.md#ilog2)
- [InverseLerp](Scalar.md#inverselerp)
- [Lerp](Scalar.md#lerp)
- [LerpAngle](Scalar.md#lerpangle)
- [Log2](Scalar.md#log2)
- [MoveTowards](Scalar.md#movetowards)
- [MoveTowardsAngle](Scalar.md#movetowardsangle)
- [Normalize](Scalar.md#normalize)
- [NormalizeRadians](Scalar.md#normalizeradians)
- [PercentToRange](Scalar.md#percenttorange)
- [PingPong](Scalar.md#pingpong)
- [RandomRange](Scalar.md#randomrange)
- [RangeToPercent](Scalar.md#rangetopercent)
- [Repeat](Scalar.md#repeat)
- [Sign](Scalar.md#sign)
- [SmoothStep](Scalar.md#smoothstep)
- [ToHex](Scalar.md#tohex)
- [WithinEpsilon](Scalar.md#withinepsilon)

## Constructors

### constructor

• **new Scalar**()

## Properties

### TwoPi

▪ `Static` **TwoPi**: `number`

Two pi constants convenient for computation.

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.scalar.ts:8

## Methods

### Clamp

▸ `Static` **Clamp**(`value`, `min?`, `max?`): `number`

Returns the value itself if it's between min and max.
Returns min if the value is lower than min.
Returns max if the value is greater than max.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `value` | `number` | `undefined` | the value to clmap |
| `min` | `number` | `0` | the min value to clamp to (default: 0) |
| `max` | `number` | `1` | the max value to clamp to (default: 1) |

#### Returns

`number`

the clamped value

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.scalar.ts:60

___

### DeltaAngle

▸ `Static` **DeltaAngle**(`current`, `target`): `number`

Calculates the shortest difference between two given angles given in degrees.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `current` | `number` | current angle in degrees |
| `target` | `number` | target angle in degrees |

#### Returns

`number`

the delta

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.scalar.ts:149

___

### Denormalize

▸ `Static` **Denormalize**(`normalized`, `min`, `max`): `number`

Denormalize the value from 0.0 and 1.0 using min and max values

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `normalized` | `number` | value to denormalize |
| `min` | `number` | max to denormalize between |
| `max` | `number` | min to denormalize between |

#### Returns

`number`

the denormalized value

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.scalar.ts:139

___

### HCF

▸ `Static` **HCF**(`a`, `b`): `number`

Returns the highest common factor of two integers.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `a` | `number` | first parameter |
| `b` | `number` | second parameter |

#### Returns

`number`

HCF of a and b

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.scalar.ts:370

___

### Hermite

▸ `Static` **Hermite**(`value1`, `tangent1`, `value2`, `tangent2`, `amount`): `number`

Returns a new scalar located for "amount" (float) on the Hermite spline defined by the scalars "value1", "value3", "tangent1", "tangent2".

**`See`**

http://mathworld.wolfram.com/HermitePolynomial.html

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value1` | `number` | defines the first control point |
| `tangent1` | `number` | defines the first tangent |
| `value2` | `number` | defines the second control point |
| `tangent2` | `number` | defines the second tangent |
| `amount` | `number` | defines the amount on the interpolation spline (between 0 and 1) |

#### Returns

`number`

hermite result

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.scalar.ts:280

___

### Hermite1stDerivative

▸ `Static` **Hermite1stDerivative**(`value1`, `tangent1`, `value2`, `tangent2`, `time`): `number`

Returns a new scalar which is the 1st derivative of the Hermite spline defined by the scalars "value1", "value2", "tangent1", "tangent2".

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value1` | `number` | defines the first control point |
| `tangent1` | `number` | defines the first tangent |
| `value2` | `number` | defines the second control point |
| `tangent2` | `number` | defines the second tangent |
| `time` | `number` | define where the derivative must be done |

#### Returns

`number`

1st derivative

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.scalar.ts:300

___

### ILog2

▸ `Static` **ILog2**(`value`): `number`

the floor part of a log2 value.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `number` | the value to compute log2 of |

#### Returns

`number`

the log2 of value.

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.scalar.ts:78

___

### InverseLerp

▸ `Static` **InverseLerp**(`a`, `b`, `value`): `number`

Calculates the linear parameter t that produces the interpolant value within the range [a, b].

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `a` | `number` | start value |
| `b` | `number` | target value |
| `value` | `number` | value between a and b |

#### Returns

`number`

the inverseLerp value

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.scalar.ts:260

___

### Lerp

▸ `Static` **Lerp**(`start`, `end`, `amount`): `number`

Creates a new scalar with values linearly interpolated of "amount" between the start scalar and the end scalar.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `start` | `number` | start value |
| `end` | `number` | target value |
| `amount` | `number` | amount to lerp between |

#### Returns

`number`

the lerped value

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.scalar.ts:233

___

### LerpAngle

▸ `Static` **LerpAngle**(`start`, `end`, `amount`): `number`

Same as Lerp but makes sure the values interpolate correctly when they wrap around 360 degrees.
The parameter t is clamped to the range [0, 1]. Variables a and b are assumed to be in degrees.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `start` | `number` | start value |
| `end` | `number` | target value |
| `amount` | `number` | amount to lerp between |

#### Returns

`number`

the lerped value

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.scalar.ts:245

___

### Log2

▸ `Static` **Log2**(`value`): `number`

the log2 of value.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `number` | the value to compute log2 of |

#### Returns

`number`

the log2 of value.

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.scalar.ts:69

___

### MoveTowards

▸ `Static` **MoveTowards**(`current`, `target`, `maxDelta`): `number`

Moves a value current towards target.

This is essentially the same as Mathf.Lerp but instead the function will ensure that the speed never exceeds maxDelta.
Negative values of maxDelta pushes the value away from target.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `current` | `number` | current value |
| `target` | `number` | target value |
| `maxDelta` | `number` | max distance to move |

#### Returns

`number`

resulting value

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.scalar.ts:194

___

### MoveTowardsAngle

▸ `Static` **MoveTowardsAngle**(`current`, `target`, `maxDelta`): `number`

Same as MoveTowards but makes sure the values interpolate correctly when they wrap around 360 degrees.

Variables current and target are assumed to be in degrees. For optimization reasons, negative values of maxDelta
 are not supported and may cause oscillation. To push current away from a target angle, add 180 to that angle instead.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `current` | `number` | current value |
| `target` | `number` | target value |
| `maxDelta` | `number` | max distance to move |

#### Returns

`number`

resulting angle

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.scalar.ts:214

___

### Normalize

▸ `Static` **Normalize**(`value`, `min`, `max`): `number`

Normalize the value between 0.0 and 1.0 using min and max values

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `number` | value to normalize |
| `min` | `number` | max to normalize between |
| `max` | `number` | min to normalize between |

#### Returns

`number`

the normalized value

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.scalar.ts:128

___

### NormalizeRadians

▸ `Static` **NormalizeRadians**(`angle`): `number`

Returns the angle converted to equivalent value between -Math.PI and Math.PI radians.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `angle` | `number` | The angle to normalize in radian. |

#### Returns

`number`

The converted angle.

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.scalar.ts:350

___

### PercentToRange

▸ `Static` **PercentToRange**(`percent`, `min`, `max`): `number`

This function returns number that corresponds to the percentage in a given range.

PercentToRange(0.34,0,100) will return 34.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `percent` | `number` | to convert to number |
| `min` | `number` | min range |
| `max` | `number` | max range |

#### Returns

`number`

the number

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.scalar.ts:341

___

### PingPong

▸ `Static` **PingPong**(`tx`, `length`): `number`

PingPongs the value t, so that it is never larger than length and never smaller than 0.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `tx` | `number` | value |
| `length` | `number` | length |

#### Returns

`number`

The returned value will move back and forth between 0 and length

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.scalar.ts:163

___

### RandomRange

▸ `Static` **RandomRange**(`min`, `max`): `number`

Returns a random float number between and min and max values

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `min` | `number` | min value of random |
| `max` | `number` | max value of random |

#### Returns

`number`

random value

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.scalar.ts:311

___

### RangeToPercent

▸ `Static` **RangeToPercent**(`number`, `min`, `max`): `number`

This function returns percentage of a number in a given range.

RangeToPercent(40,20,60) will return 0.5 (50%)
RangeToPercent(34,0,100) will return 0.34 (34%)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `number` | `number` | to convert to percentage |
| `min` | `number` | min range |
| `max` | `number` | max range |

#### Returns

`number`

the percentage

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.scalar.ts:328

___

### Repeat

▸ `Static` **Repeat**(`value`, `length`): `number`

Loops the value, so that it is never larger than length and never smaller than 0.

This is similar to the modulo operator but it works with floating point numbers.
For example, using 3.0 for t and 2.5 for length, the result would be 0.5.
With t = 5 and length = 2.5, the result would be 0.0.
Note, however, that the behaviour is not defined for negative numbers as it is for the modulo operator

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `number` | the value |
| `length` | `number` | the length |

#### Returns

`number`

the looped value

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.scalar.ts:117

___

### Sign

▸ `Static` **Sign**(`value`): `number`

Returns -1 if value is negative and +1 is value is positive.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `number` | the value |

#### Returns

`number`

the value itself if it's equal to zero.

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.scalar.ts:41

___

### SmoothStep

▸ `Static` **SmoothStep**(`from`, `to`, `tx`): `number`

Interpolates between min and max with smoothing at the limits.

This function interpolates between min and max in a similar way to Lerp. However, the interpolation will gradually speed up
from the start and slow down toward the end. This is useful for creating natural-looking animation, fading and other transitions.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `from` | `number` | from |
| `to` | `number` | to |
| `tx` | `number` | value |

#### Returns

`number`

the smooth stepped value

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.scalar.ts:178

___

### ToHex

▸ `Static` **ToHex**(`i`): `string`

Returns a string : the upper case translation of the number i to hexadecimal.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `i` | `number` | number |

#### Returns

`string`

the upper case translation of the number i to hexadecimal.

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.scalar.ts:26

___

### WithinEpsilon

▸ `Static` **WithinEpsilon**(`a`, `b`, `epsilon?`): `boolean`

Boolean : true if the absolute difference between a and b is lower than epsilon (default = 1.401298E-45)

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `a` | `number` | `undefined` | number |
| `b` | `number` | `undefined` | number |
| `epsilon` | `number` | `1.401298e-45` | (default = 1.401298E-45) |

#### Returns

`boolean`

true if the absolute difference between a and b is lower than epsilon (default = 1.401298E-45)

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.scalar.ts:17
