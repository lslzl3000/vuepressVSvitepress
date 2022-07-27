[@dev/core](../README.md) / [Exports](../modules.md) / Action

# Class: Action

The action to be carried out following a trigger

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions#available-actions

## Hierarchy

- **`Action`**

  ↳ [`SwitchBooleanAction`](SwitchBooleanAction.md)

  ↳ [`SetStateAction`](SetStateAction.md)

  ↳ [`SetValueAction`](SetValueAction.md)

  ↳ [`IncrementValueAction`](IncrementValueAction.md)

  ↳ [`PlayAnimationAction`](PlayAnimationAction.md)

  ↳ [`StopAnimationAction`](StopAnimationAction.md)

  ↳ [`DoNothingAction`](DoNothingAction.md)

  ↳ [`CombineAction`](CombineAction.md)

  ↳ [`ExecuteCodeAction`](ExecuteCodeAction.md)

  ↳ [`SetParentAction`](SetParentAction.md)

  ↳ [`PlaySoundAction`](PlaySoundAction.md)

  ↳ [`StopSoundAction`](StopSoundAction.md)

  ↳ [`InterpolateValueAction`](InterpolateValueAction.md)

## Implements

- [`IAction`](../interfaces/IAction.md)

## Table of contents

### Constructors

- [constructor](Action.md#constructor)

### Properties

- [\_child](Action.md#_child)
- [\_condition](Action.md#_condition)
- [\_nextActiveAction](Action.md#_nextactiveaction)
- [\_triggerParameter](Action.md#_triggerparameter)
- [onBeforeExecuteObservable](Action.md#onbeforeexecuteobservable)
- [trigger](Action.md#trigger)
- [triggerOptions](Action.md#triggeroptions)

### Methods

- [execute](Action.md#execute)
- [getTriggerParameter](Action.md#gettriggerparameter)
- [serialize](Action.md#serialize)
- [setTriggerParameter](Action.md#settriggerparameter)
- [skipToNextActiveAction](Action.md#skiptonextactiveaction)
- [then](Action.md#then)

## Constructors

### constructor

• **new Action**(`triggerOptions`, `condition?`)

Creates a new Action

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `triggerOptions` | `any` | the trigger, with or without parameters, for the action |
| `condition?` | [`Condition`](Condition.md) | an optional determinant of action |

#### Defined in

https://github.com/babylon.js/core/src/Actions/action.ts:100

## Properties

### \_child

• `Private` **\_child**: [`Action`](Action.md)

#### Defined in

https://github.com/babylon.js/core/src/Actions/action.ts:86

___

### \_condition

• `Private` `Optional` **\_condition**: [`Condition`](Condition.md)

#### Defined in

https://github.com/babylon.js/core/src/Actions/action.ts:87

___

### \_nextActiveAction

• `Private` **\_nextActiveAction**: [`Action`](Action.md)

#### Defined in

https://github.com/babylon.js/core/src/Actions/action.ts:85

___

### \_triggerParameter

• `Private` **\_triggerParameter**: `any`

#### Defined in

https://github.com/babylon.js/core/src/Actions/action.ts:88

___

### onBeforeExecuteObservable

• **onBeforeExecuteObservable**: [`Observable`](Observable.md)[`Action`](Action.md)

An event triggered prior to action being executed.

#### Defined in

https://github.com/babylon.js/core/src/Actions/action.ts:93

___

### trigger

• **trigger**: `number`

Trigger for the action

#### Implementation of

[IAction](../interfaces/IAction.md).[trigger](../interfaces/IAction.md#trigger)

#### Defined in

https://github.com/babylon.js/core/src/Actions/action.ts:77

___

### triggerOptions

• **triggerOptions**: `any`

Options of the trigger

#### Implementation of

[IAction](../interfaces/IAction.md).[triggerOptions](../interfaces/IAction.md#triggeroptions)

#### Defined in

https://github.com/babylon.js/core/src/Actions/action.ts:102

## Methods

### execute

▸ **execute**(`evt?`): `void`

Execute placeholder for child classes

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `evt?` | [`ActionEvent`](ActionEvent.md) | optional action event |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Actions/action.ts:183

___

### getTriggerParameter

▸ **getTriggerParameter**(): `any`

Gets the trigger parameter

#### Returns

`any`

the trigger parameter

#### Implementation of

[IAction](../interfaces/IAction.md).[getTriggerParameter](../interfaces/IAction.md#gettriggerparameter)

#### Defined in

https://github.com/babylon.js/core/src/Actions/action.ts:128

___

### serialize

▸ **serialize**(`parent`): `any`

Serialize placeholder for child classes

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `parent` | `any` | of child |

#### Returns

`any`

the serialized object

#### Implementation of

[IAction](../interfaces/IAction.md).[serialize](../interfaces/IAction.md#serialize)

#### Defined in

https://github.com/babylon.js/core/src/Actions/action.ts:240

___

### setTriggerParameter

▸ **setTriggerParameter**(`value`): `void`

Sets the trigger parameter

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `any` | defines the new trigger parameter |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Actions/action.ts:136

___

### skipToNextActiveAction

▸ **skipToNextActiveAction**(): `void`

Skips to next active action

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Actions/action.ts:188

___

### then

▸ **then**(`action`): [`Action`](Action.md)

Adds action to chain of actions, may be a DoNothingAction

**`See`**

https://www.babylonjs-playground.com/#1T30HR#0

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `action` | [`Action`](Action.md) | defines the next action to execute |

#### Returns

[`Action`](Action.md)

The action passed in

#### Implementation of

[IAction](../interfaces/IAction.md).[then](../interfaces/IAction.md#then)

#### Defined in

https://github.com/babylon.js/core/src/Actions/action.ts:206
