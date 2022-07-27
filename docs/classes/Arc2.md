[@dev/core](../README.md) / [Exports](../modules.md) / Arc2

# Class: Arc2

This represents an arc in a 2d space.

## Table of contents

### Constructors

- [constructor](Arc2.md#constructor)

### Properties

- [angle](Arc2.md#angle)
- [centerPoint](Arc2.md#centerpoint)
- [endPoint](Arc2.md#endpoint)
- [midPoint](Arc2.md#midpoint)
- [orientation](Arc2.md#orientation)
- [radius](Arc2.md#radius)
- [startAngle](Arc2.md#startangle)
- [startPoint](Arc2.md#startpoint)

## Constructors

### constructor

• **new Arc2**(`startPoint`, `midPoint`, `endPoint`)

Creates an Arc object from the three given points : start, middle and end.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `startPoint` | [`Vector2`](Vector2.md) | Defines the start point of the arc |
| `midPoint` | [`Vector2`](Vector2.md) | Defines the middle point of the arc |
| `endPoint` | [`Vector2`](Vector2.md) | Defines the end point of the arc |

#### Defined in

packages/dev/core/src/Maths/math.path.ts:145

## Properties

### angle

• **angle**: [`Angle`](Angle.md)

Defines the angle of the arc (from mid point to end point).

#### Defined in

packages/dev/core/src/Maths/math.path.ts:129

___

### centerPoint

• **centerPoint**: [`Vector2`](Vector2.md)

Defines the center point of the arc.

#### Defined in

packages/dev/core/src/Maths/math.path.ts:121

___

### endPoint

• **endPoint**: [`Vector2`](Vector2.md)

#### Defined in

packages/dev/core/src/Maths/math.path.ts:151

___

### midPoint

• **midPoint**: [`Vector2`](Vector2.md)

#### Defined in

packages/dev/core/src/Maths/math.path.ts:149

___

### orientation

• **orientation**: [`Orientation`](../enums/Orientation.md)

Defines the orientation of the arc (clock wise/counter clock wise).

#### Defined in

packages/dev/core/src/Maths/math.path.ts:137

___

### radius

• **radius**: `number`

Defines the radius of the arc.

#### Defined in

packages/dev/core/src/Maths/math.path.ts:125

___

### startAngle

• **startAngle**: [`Angle`](Angle.md)

Defines the start angle of the arc (from start point to middle point).

#### Defined in

packages/dev/core/src/Maths/math.path.ts:133

___

### startPoint

• **startPoint**: [`Vector2`](Vector2.md)

#### Defined in

packages/dev/core/src/Maths/math.path.ts:147
