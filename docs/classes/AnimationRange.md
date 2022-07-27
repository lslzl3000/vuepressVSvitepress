[@dev/core](../README.md) / [Exports](../modules.md) / AnimationRange

# Class: AnimationRange

Represents the range of an animation

## Table of contents

### Constructors

- [constructor](AnimationRange.md#constructor)

### Properties

- [from](AnimationRange.md#from)
- [name](AnimationRange.md#name)
- [to](AnimationRange.md#to)

### Methods

- [clone](AnimationRange.md#clone)

## Constructors

### constructor

• **new AnimationRange**(`name`, `from`, `to`)

Initializes the range of an animation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | The name of the animation range |
| `from` | `number` | The starting frame of the animation |
| `to` | `number` | The ending frame of the animation |

#### Defined in

packages/dev/core/src/Animations/animationRange.ts:11

## Properties

### from

• **from**: `number`

#### Defined in

packages/dev/core/src/Animations/animationRange.ts:15

___

### name

• **name**: `string`

#### Defined in

packages/dev/core/src/Animations/animationRange.ts:13

___

### to

• **to**: `number`

#### Defined in

packages/dev/core/src/Animations/animationRange.ts:17

## Methods

### clone

▸ **clone**(): [`AnimationRange`](AnimationRange.md)

Makes a copy of the animation range

#### Returns

[`AnimationRange`](AnimationRange.md)

A copy of the animation range

#### Defined in

packages/dev/core/src/Animations/animationRange.ts:24
