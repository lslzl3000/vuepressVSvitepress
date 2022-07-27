[@dev/core](../README.md) / [Exports](../modules.md) / AnimationEvent

# Class: AnimationEvent

Composed of a frame, and an action function

## Table of contents

### Constructors

- [constructor](AnimationEvent.md#constructor)

### Properties

- [action](AnimationEvent.md#action)
- [frame](AnimationEvent.md#frame)
- [isDone](AnimationEvent.md#isdone)
- [onlyOnce](AnimationEvent.md#onlyonce)

## Constructors

### constructor

• **new AnimationEvent**(`frame`, `action`, `onlyOnce?`)

Initializes the animation event

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `frame` | `number` | The frame for which the event is triggered |
| `action` | (`currentFrame`: `number`) => `void` | The event to perform when triggered |
| `onlyOnce?` | `boolean` | Specifies if the event should be triggered only once |

#### Defined in

packages/dev/core/src/Animations/animationEvent.ts:16

## Properties

### action

• **action**: (`currentFrame`: `number`) => `void`

#### Type declaration

▸ (`currentFrame`): `void`

The event to perform when triggered *

##### Parameters

| Name | Type |
| :------ | :------ |
| `currentFrame` | `number` |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Animations/animationEvent.ts:20

___

### frame

• **frame**: `number`

#### Defined in

packages/dev/core/src/Animations/animationEvent.ts:18

___

### isDone

• **isDone**: `boolean` = `false`

Specifies if the animation event is done

#### Defined in

packages/dev/core/src/Animations/animationEvent.ts:8

___

### onlyOnce

• `Optional` **onlyOnce**: `boolean`

#### Defined in

packages/dev/core/src/Animations/animationEvent.ts:22
