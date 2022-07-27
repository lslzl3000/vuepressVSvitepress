[@dev/core](../README.md) / [Exports](../modules.md) / ValueCondition

# Class: ValueCondition

Defines specific conditional operators as extensions of Condition

## Hierarchy

- [`Condition`](Condition.md)

  ↳ **`ValueCondition`**

## Table of contents

### Constructors

- [constructor](ValueCondition.md#constructor)

### Properties

- [operator](ValueCondition.md#operator)
- [propertyPath](ValueCondition.md#propertypath)
- [value](ValueCondition.md#value)

### Accessors

- [IsDifferent](ValueCondition.md#isdifferent)
- [IsEqual](ValueCondition.md#isequal)
- [IsGreater](ValueCondition.md#isgreater)
- [IsLesser](ValueCondition.md#islesser)

### Methods

- [isValid](ValueCondition.md#isvalid)
- [serialize](ValueCondition.md#serialize)
- [GetOperatorName](ValueCondition.md#getoperatorname)

## Constructors

### constructor

• **new ValueCondition**(`actionManager`, `target`, `propertyPath`, `value`, `operator?`)

Creates a new ValueCondition

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `actionManager` | [`ActionManager`](ActionManager.md) | `undefined` | manager for the action the condition applies to |
| `target` | `any` | `undefined` | for the action |
| `propertyPath` | `string` | `undefined` | path to specify the property of the target the conditional operator uses |
| `value` | `any` | `undefined` | the value compared by the conditional operator against the current value of the property |
| `operator` | `number` | `ValueCondition.IsEqual` | the conditional operator, default ValueCondition.IsEqual |

#### Overrides

[Condition](Condition.md).[constructor](Condition.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Actions/condition.ts:172

## Properties

### operator

• **operator**: `number` = `ValueCondition.IsEqual`

#### Defined in

https://github.com/babylon.js/core/src/Actions/condition.ts:180

___

### propertyPath

• **propertyPath**: `string`

#### Defined in

https://github.com/babylon.js/core/src/Actions/condition.ts:176

___

### value

• **value**: `any`

#### Defined in

https://github.com/babylon.js/core/src/Actions/condition.ts:178

## Accessors

### IsDifferent

• `Static` `get` **IsDifferent**(): `number`

Returns the number for IsDifferent

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Actions/condition.ts:122

___

### IsEqual

• `Static` `get` **IsEqual**(): `number`

returns the number for IsEqual

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Actions/condition.ts:115

___

### IsGreater

• `Static` `get` **IsGreater**(): `number`

Returns the number for IsGreater

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Actions/condition.ts:129

___

### IsLesser

• `Static` `get` **IsLesser**(): `number`

Returns the number for IsLesser

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Actions/condition.ts:136

## Methods

### isValid

▸ **isValid**(): `boolean`

Compares the given value with the property value for the specified conditional operator

#### Returns

`boolean`

the result of the comparison

#### Overrides

[Condition](Condition.md).[isValid](Condition.md#isvalid)

#### Defined in

https://github.com/babylon.js/core/src/Actions/condition.ts:193

___

### serialize

▸ **serialize**(): `any`

Serialize the ValueCondition into a JSON compatible object

#### Returns

`any`

serialization object

#### Overrides

[Condition](Condition.md).[serialize](Condition.md#serialize)

#### Defined in

https://github.com/babylon.js/core/src/Actions/condition.ts:219

___

### GetOperatorName

▸ `Static` **GetOperatorName**(`operator`): `string`

Gets the name of the conditional operator for the ValueCondition

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `operator` | `number` | the conditional operator |

#### Returns

`string`

the name

#### Defined in

https://github.com/babylon.js/core/src/Actions/condition.ts:236
