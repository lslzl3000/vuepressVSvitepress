[@dev/core](../README.md) / [Exports](../modules.md) / Path2

# Class: Path2

Represents a 2D path made up of multiple 2D points

## Table of contents

### Constructors

- [constructor](Path2.md#constructor)

### Properties

- [\_length](Path2.md#_length)
- [\_points](Path2.md#_points)
- [closed](Path2.md#closed)

### Methods

- [addArcTo](Path2.md#addarcto)
- [addLineTo](Path2.md#addlineto)
- [close](Path2.md#close)
- [getPointAtLengthPosition](Path2.md#getpointatlengthposition)
- [getPoints](Path2.md#getpoints)
- [length](Path2.md#length)
- [StartingAt](Path2.md#startingat)

## Constructors

### constructor

• **new Path2**(`x`, `y`)

Creates a Path2 object from the starting 2D coordinates x and y.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | the starting points x value |
| `y` | `number` | the starting points y value |

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:207

## Properties

### \_length

• `Private` **\_length**: `number` = `0.0`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:195

___

### \_points

• `Private` **\_points**: [`Vector2`](Vector2.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:194

___

### closed

• **closed**: `boolean` = `false`

If the path start and end point are the same

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:200

## Methods

### addArcTo

▸ **addArcTo**(`midX`, `midY`, `endX`, `endY`, `numberOfSegments?`): [`Path2`](Path2.md)

Adds _numberOfSegments_ segments according to the arc definition (middle point coordinates, end point coordinates, the arc start point being the current Path2 last point) to the current Path2.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `midX` | `number` | `undefined` | middle point x value |
| `midY` | `number` | `undefined` | middle point y value |
| `endX` | `number` | `undefined` | end point x value |
| `endY` | `number` | `undefined` | end point y value |
| `numberOfSegments` | `number` | `36` | (default: 36) |

#### Returns

[`Path2`](Path2.md)

the updated Path2.

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:237

___

### addLineTo

▸ **addLineTo**(`x`, `y`): [`Path2`](Path2.md)

Adds a new segment until the given coordinates (x, y) to the current Path2.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | the added points x value |
| `y` | `number` | the added points y value |

#### Returns

[`Path2`](Path2.md)

the updated Path2.

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:217

___

### close

▸ **close**(): [`Path2`](Path2.md)

Closes the Path2.

#### Returns

[`Path2`](Path2.md)

the Path2.

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:265

___

### getPointAtLengthPosition

▸ **getPointAtLengthPosition**(`normalizedLengthPosition`): [`Vector2`](Vector2.md)

Retreives the point at the distance aways from the starting point

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `normalizedLengthPosition` | `number` | the length along the path to retrieve the point from |

#### Returns

[`Vector2`](Vector2.md)

a new Vector2 located at a percentage of the Path2 total length on this path.

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:297

___

### getPoints

▸ **getPoints**(): [`Vector2`](Vector2.md)[]

Gets the points which construct the path

#### Returns

[`Vector2`](Vector2.md)[]

the Path2 internal array of points.

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:288

___

### length

▸ **length**(): `number`

Gets the sum of the distance between each sequential point in the path

#### Returns

`number`

the Path2 total length (float).

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:273

___

### StartingAt

▸ `Static` **StartingAt**(`x`, `y`): [`Path2`](Path2.md)

Creates a new path starting from an x and y position

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | starting x value |
| `y` | `number` | starting y value |

#### Returns

[`Path2`](Path2.md)

a new Path2 starting at the coordinates (x, y).

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.path.ts:331
