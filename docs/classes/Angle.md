[@dev/core](../README.md) / [Exports](../modules.md) / Angle

# Class: Angle

Defines angle representation

## Table of contents

### Constructors

- [constructor](Angle.md#constructor)

### Properties

- [\_radians](Angle.md#_radians)

### Methods

- [degrees](Angle.md#degrees)
- [radians](Angle.md#radians)
- [BetweenTwoPoints](Angle.md#betweentwopoints)
- [FromDegrees](Angle.md#fromdegrees)
- [FromRadians](Angle.md#fromradians)

## Constructors

### constructor

• **new Angle**(`radians`)

Creates an Angle object of "radians" radians (float).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `radians` | `number` | the angle in radians |

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:61

## Properties

### \_radians

• `Private` **\_radians**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:55

## Methods

### degrees

▸ **degrees**(): `number`

Get value in degrees

#### Returns

`number`

the Angle value in degrees (float)

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:72

___

### radians

▸ **radians**(): `number`

Get value in radians

#### Returns

`number`

the Angle value in radians (float)

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:80

___

### BetweenTwoPoints

▸ `Static` **BetweenTwoPoints**(`a`, `b`): [`Angle`](Angle.md)

Gets a new Angle object valued with the gradient angle, in radians, of the line joining two points

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `a` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines first point as the origin |
| `b` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector2`](Vector2.md) | defines point |

#### Returns

[`Angle`](Angle.md)

a new Angle

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:90

___

### FromDegrees

▸ `Static` **FromDegrees**(`degrees`): [`Angle`](Angle.md)

Gets a new Angle object from the given float in degrees

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `degrees` | `number` | defines the angle value in degrees |

#### Returns

[`Angle`](Angle.md)

a new Angle

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:109

___

### FromRadians

▸ `Static` **FromRadians**(`radians`): [`Angle`](Angle.md)

Gets a new Angle object from the given float in radians

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `radians` | `number` | defines the angle value in radians |

#### Returns

[`Angle`](Angle.md)

a new Angle

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:101
