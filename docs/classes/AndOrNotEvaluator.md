[@dev/core](../README.md) / [Exports](../modules.md) / AndOrNotEvaluator

# Class: AndOrNotEvaluator

Class used to evaluate queries containing `and` and `or` operators

## Table of contents

### Constructors

- [constructor](AndOrNotEvaluator.md#constructor)

### Methods

- [Eval](AndOrNotEvaluator.md#eval)
- [\_HandleParenthesisContent](AndOrNotEvaluator.md#_handleparenthesiscontent)
- [\_SimplifyNegation](AndOrNotEvaluator.md#_simplifynegation)

## Constructors

### constructor

• **new AndOrNotEvaluator**()

## Methods

### Eval

▸ `Static` **Eval**(`query`, `evaluateCallback`): `boolean`

Evaluate a query

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `query` | `string` | defines the query to evaluate |
| `evaluateCallback` | (`val`: `any`) => `boolean` | defines the callback used to filter result |

#### Returns

`boolean`

true if the query matches

#### Defined in

https://github.com/babylon.js/core/src/Misc/andOrNotEvaluator.ts:11

___

### \_HandleParenthesisContent

▸ `Static` `Private` **_HandleParenthesisContent**(`parenthesisContent`, `evaluateCallback`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `parenthesisContent` | `string` |
| `evaluateCallback` | (`val`: `string`) => `boolean` |

#### Returns

`string`

#### Defined in

https://github.com/babylon.js/core/src/Misc/andOrNotEvaluator.ts:33

___

### \_SimplifyNegation

▸ `Static` `Private` **_SimplifyNegation**(`booleanString`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `booleanString` | `string` |

#### Returns

`string`

#### Defined in

https://github.com/babylon.js/core/src/Misc/andOrNotEvaluator.ts:92
