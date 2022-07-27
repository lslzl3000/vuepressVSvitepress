[@dev/core](../README.md) / [Exports](../modules.md) / Condition

# Class: Condition

A Condition applied to an Action

## Hierarchy

- **`Condition`**

  ↳ [`ValueCondition`](ValueCondition.md)

  ↳ [`PredicateCondition`](PredicateCondition.md)

  ↳ [`StateCondition`](StateCondition.md)

## Table of contents

### Constructors

- [constructor](Condition.md#constructor)

### Methods

- [isValid](Condition.md#isvalid)
- [serialize](Condition.md#serialize)

## Constructors

### constructor

• **new Condition**(`actionManager`)

Creates a new Condition

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `actionManager` | [`ActionManager`](ActionManager.md) | the manager of the action the condition is applied to |

#### Defined in

packages/dev/core/src/Actions/condition.ts:32

## Methods

### isValid

▸ **isValid**(): `boolean`

Check if the current condition is valid

#### Returns

`boolean`

a boolean

#### Defined in

packages/dev/core/src/Actions/condition.ts:40

___

### serialize

▸ **serialize**(): `any`

Serialize placeholder for child classes

#### Returns

`any`

the serialized object

#### Defined in

packages/dev/core/src/Actions/condition.ts:67
