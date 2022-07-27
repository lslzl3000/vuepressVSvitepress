[@dev/core](../README.md) / [Exports](../modules.md) / TargetedAnimation

# Class: TargetedAnimation

This class defines the direct association between an animation and a target

## Table of contents

### Constructors

- [constructor](TargetedAnimation.md#constructor)

### Properties

- [animation](TargetedAnimation.md#animation)
- [target](TargetedAnimation.md#target)

### Methods

- [getClassName](TargetedAnimation.md#getclassname)
- [serialize](TargetedAnimation.md#serialize)

## Constructors

### constructor

• **new TargetedAnimation**()

## Properties

### animation

• **animation**: [`Animation`](Animation.md)

Animation to perform

#### Defined in

packages/dev/core/src/Animations/animationGroup.ts:20

___

### target

• **target**: `any`

Target to animate

#### Defined in

packages/dev/core/src/Animations/animationGroup.ts:24

## Methods

### getClassName

▸ **getClassName**(): `string`

Returns the string "TargetedAnimation"

#### Returns

`string`

"TargetedAnimation"

#### Defined in

packages/dev/core/src/Animations/animationGroup.ts:30

___

### serialize

▸ **serialize**(): `any`

Serialize the object

#### Returns

`any`

the JSON object representing the current entity

#### Defined in

packages/dev/core/src/Animations/animationGroup.ts:38
