[@dev/core](../README.md) / [Exports](../modules.md) / PositionNormalTextureVertex

# Class: PositionNormalTextureVertex

Contains position, normal and uv vectors for a vertex

## Table of contents

### Constructors

- [constructor](PositionNormalTextureVertex.md#constructor)

### Properties

- [normal](PositionNormalTextureVertex.md#normal)
- [position](PositionNormalTextureVertex.md#position)
- [uv](PositionNormalTextureVertex.md#uv)

### Methods

- [clone](PositionNormalTextureVertex.md#clone)

## Constructors

### constructor

• **new PositionNormalTextureVertex**(`position?`, `normal?`, `uv?`)

Creates a PositionNormalTextureVertex

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | [`Vector3`](Vector3.md) | the position of the vertex (defaut: 0,0,0) |
| `normal` | [`Vector3`](Vector3.md) | the normal of the vertex (defaut: 0,1,0) |
| `uv` | [`Vector2`](Vector2.md) | the uv of the vertex (default: 0,0) |

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vertexFormat.ts:38

## Properties

### normal

• **normal**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vertexFormat.ts:42

___

### position

• **position**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vertexFormat.ts:40

___

### uv

• **uv**: [`Vector2`](Vector2.md)

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vertexFormat.ts:44

## Methods

### clone

▸ **clone**(): [`PositionNormalTextureVertex`](PositionNormalTextureVertex.md)

Clones the PositionNormalTextureVertex

#### Returns

[`PositionNormalTextureVertex`](PositionNormalTextureVertex.md)

the cloned PositionNormalTextureVertex

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.vertexFormat.ts:50
