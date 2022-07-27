[@dev/core](../README.md) / [Exports](../modules.md) / PathCursor

# Class: PathCursor

A cursor which tracks a point on a path

## Table of contents

### Constructors

- [constructor](PathCursor.md#constructor)

### Properties

- [\_onchange](PathCursor.md#_onchange)
- [animations](PathCursor.md#animations)
- [value](PathCursor.md#value)

### Methods

- [\_ensureLimits](PathCursor.md#_ensurelimits)
- [\_raiseOnChange](PathCursor.md#_raiseonchange)
- [getPoint](PathCursor.md#getpoint)
- [move](PathCursor.md#move)
- [moveAhead](PathCursor.md#moveahead)
- [moveBack](PathCursor.md#moveback)
- [onchange](PathCursor.md#onchange)

## Constructors

### constructor

• **new PathCursor**(`_path`)

Initializes the path cursor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `_path` | [`Path2`](Path2.md) | The path to track |

#### Defined in

packages/dev/core/src/Animations/pathCursor.ts:27

## Properties

### \_onchange

• `Private` **\_onchange**: (`cursor`: [`PathCursor`](PathCursor.md)) => `void`[]

Stores path cursor callbacks for when an onchange event is triggered

#### Defined in

packages/dev/core/src/Animations/pathCursor.ts:11

___

### animations

• **animations**: `Animation`[]

The animation array of the path cursor

#### Defined in

packages/dev/core/src/Animations/pathCursor.ts:21

___

### value

• **value**: `number` = `0`

The value of the path cursor

#### Defined in

packages/dev/core/src/Animations/pathCursor.ts:16

## Methods

### \_ensureLimits

▸ `Private` **_ensureLimits**(): [`PathCursor`](PathCursor.md)

Ensures that the value is limited between zero and one

#### Returns

[`PathCursor`](PathCursor.md)

This path cursor

#### Defined in

packages/dev/core/src/Animations/pathCursor.ts:82

___

### \_raiseOnChange

▸ `Private` **_raiseOnChange**(): [`PathCursor`](PathCursor.md)

Runs onchange callbacks on change (used by the animation engine)

#### Returns

[`PathCursor`](PathCursor.md)

This path cursor

#### Defined in

packages/dev/core/src/Animations/pathCursor.ts:97

___

### getPoint

▸ **getPoint**(): [`Vector3`](Vector3.md)

Gets the cursor point on the path

#### Returns

[`Vector3`](Vector3.md)

A point on the path cursor at the cursor location

#### Defined in

packages/dev/core/src/Animations/pathCursor.ts:33

___

### move

▸ **move**(`step`): [`PathCursor`](PathCursor.md)

Moves the cursor by the step amount
If the step amount is greater than one, an exception is thrown

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `step` | `number` | The amount to move the cursor |

#### Returns

[`PathCursor`](PathCursor.md)

This path cursor

#### Defined in

packages/dev/core/src/Animations/pathCursor.ts:66

___

### moveAhead

▸ **moveAhead**(`step?`): [`PathCursor`](PathCursor.md)

Moves the cursor ahead by the step amount

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `step` | `number` | `0.002` | The amount to move the cursor forward |

#### Returns

[`PathCursor`](PathCursor.md)

This path cursor

#### Defined in

packages/dev/core/src/Animations/pathCursor.ts:43

___

### moveBack

▸ **moveBack**(`step?`): [`PathCursor`](PathCursor.md)

Moves the cursor behind by the step amount

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `step` | `number` | `0.002` | The amount to move the cursor back |

#### Returns

[`PathCursor`](PathCursor.md)

This path cursor

#### Defined in

packages/dev/core/src/Animations/pathCursor.ts:54

___

### onchange

▸ **onchange**(`f`): [`PathCursor`](PathCursor.md)

Executes a function on change

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `f` | (`cursor`: [`PathCursor`](PathCursor.md)) => `void` | A path cursor onchange callback |

#### Returns

[`PathCursor`](PathCursor.md)

This path cursor

#### Defined in

packages/dev/core/src/Animations/pathCursor.ts:108
