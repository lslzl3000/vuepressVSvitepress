[@dev/core](../README.md) / [Exports](../modules.md) / PositionNormalVertex

# Class: PositionNormalVertex

Contains position and normal vectors for a vertex

## Table of contents

### Constructors

- [constructor](PositionNormalVertex.md#constructor)

### Properties

- [normal](PositionNormalVertex.md#normal)
- [position](PositionNormalVertex.md#position)

### Methods

- [clone](PositionNormalVertex.md#clone)

## Constructors

### constructor

• **new PositionNormalVertex**(`position?`, `normal?`)

Creates a PositionNormalVertex

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | [`Vector3`](Vector3.md) | the position of the vertex (defaut: 0,0,0) |
| `normal` | [`Vector3`](Vector3.md) | the normal of the vertex (defaut: 0,1,0) |

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vertexFormat.ts:12

## Properties

### normal

• **normal**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vertexFormat.ts:16

___

### position

• **position**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vertexFormat.ts:14

## Methods

### clone

▸ **clone**(): [`PositionNormalVertex`](PositionNormalVertex.md)

Clones the PositionNormalVertex

#### Returns

[`PositionNormalVertex`](PositionNormalVertex.md)

the cloned PositionNormalVertex

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vertexFormat.ts:23
