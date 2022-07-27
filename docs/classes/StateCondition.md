[@dev/core](../README.md) / [Exports](../modules.md) / StateCondition

# Class: StateCondition

Defines a state condition as an extension of Condition

## Hierarchy

- [`Condition`](Condition.md)

  ↳ **`StateCondition`**

## Table of contents

### Constructors

- [constructor](StateCondition.md#constructor)

### Properties

- [value](StateCondition.md#value)

### Methods

- [isValid](StateCondition.md#isvalid)
- [serialize](StateCondition.md#serialize)

## Constructors

### constructor

• **new StateCondition**(`actionManager`, `target`, `value`)

Creates a new StateCondition

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `actionManager` | [`ActionManager`](ActionManager.md) | manager for the action the condition applies to |
| `target` | `any` | of the condition |
| `value` | `string` | to compare with target state |

#### Overrides

[Condition](Condition.md).[constructor](Condition.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Actions/condition.ts:305

## Properties

### value

• **value**: `string`

#### Defined in

https://github.com/babylon.js/core/src/Actions/condition.ts:309

## Methods

### isValid

▸ **isValid**(): `boolean`

Gets a boolean indicating if the current condition is met

#### Returns

`boolean`

the validity of the state

#### Overrides

[Condition](Condition.md).[isValid](Condition.md#isvalid)

#### Defined in

https://github.com/babylon.js/core/src/Actions/condition.ts:320

___

### serialize

▸ **serialize**(): `any`

Serialize the StateCondition into a JSON compatible object

#### Returns

`any`

serialization object

#### Overrides

[Condition](Condition.md).[serialize](Condition.md#serialize)

#### Defined in

https://github.com/babylon.js/core/src/Actions/condition.ts:328
