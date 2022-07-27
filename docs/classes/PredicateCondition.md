[@dev/core](../README.md) / [Exports](../modules.md) / PredicateCondition

# Class: PredicateCondition

Defines a predicate condition as an extension of Condition

## Hierarchy

- [`Condition`](Condition.md)

  ↳ **`PredicateCondition`**

## Table of contents

### Constructors

- [constructor](PredicateCondition.md#constructor)

### Properties

- [predicate](PredicateCondition.md#predicate)

### Methods

- [isValid](PredicateCondition.md#isvalid)
- [serialize](PredicateCondition.md#serialize)

## Constructors

### constructor

• **new PredicateCondition**(`actionManager`, `predicate`)

Creates a new PredicateCondition

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `actionManager` | [`ActionManager`](ActionManager.md) | manager for the action the condition applies to |
| `predicate` | () => `boolean` | defines the predicate function used to validate the condition |

#### Overrides

[Condition](Condition.md).[constructor](Condition.md#constructor)

#### Defined in

packages/dev/core/src/Actions/condition.ts:267

## Properties

### predicate

• **predicate**: () => `boolean`

#### Type declaration

▸ (): `boolean`

defines the predicate function used to validate the condition

##### Returns

`boolean`

#### Defined in

packages/dev/core/src/Actions/condition.ts:270

## Methods

### isValid

▸ **isValid**(): `boolean`

#### Returns

`boolean`

the validity of the predicate condition

#### Overrides

[Condition](Condition.md).[isValid](Condition.md#isvalid)

#### Defined in

packages/dev/core/src/Actions/condition.ts:278

___

### serialize

▸ **serialize**(): `any`

Serialize placeholder for child classes

#### Returns

`any`

the serialized object

#### Inherited from

[Condition](Condition.md).[serialize](Condition.md#serialize)

#### Defined in

packages/dev/core/src/Actions/condition.ts:67
