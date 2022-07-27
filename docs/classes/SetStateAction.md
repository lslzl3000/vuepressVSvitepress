[@dev/core](../README.md) / [Exports](../modules.md) / SetStateAction

# Class: SetStateAction

This defines an action responsible to set a the state field of the target
 to a desired value once triggered.

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions

## Hierarchy

- [`Action`](Action.md)

  ↳ **`SetStateAction`**

## Table of contents

### Constructors

- [constructor](SetStateAction.md#constructor)

### Properties

- [\_target](SetStateAction.md#_target)
- [onBeforeExecuteObservable](SetStateAction.md#onbeforeexecuteobservable)
- [trigger](SetStateAction.md#trigger)
- [triggerOptions](SetStateAction.md#triggeroptions)
- [value](SetStateAction.md#value)

### Methods

- [execute](SetStateAction.md#execute)
- [getTriggerParameter](SetStateAction.md#gettriggerparameter)
- [serialize](SetStateAction.md#serialize)
- [setTriggerParameter](SetStateAction.md#settriggerparameter)
- [skipToNextActiveAction](SetStateAction.md#skiptonextactiveaction)
- [then](SetStateAction.md#then)

## Constructors

### constructor

• **new SetStateAction**(`triggerOptions`, `target`, `value`, `condition?`)

Instantiate the action

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `triggerOptions` | `any` | defines the trigger options |
| `target` | `any` | defines the object containing the state property |
| `value` | `string` | defines the value to store in the state field |
| `condition?` | [`Condition`](Condition.md) | defines the trigger related conditions |

#### Overrides

[Action](Action.md).[constructor](Action.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Actions/directActions.ts:86

## Properties

### \_target

• `Private` **\_target**: `any`

#### Defined in

https://github.com/babylon.js/core/src/Actions/directActions.ts:77

___

### onBeforeExecuteObservable

• **onBeforeExecuteObservable**: [`Observable`](Observable.md)[`Action`](Action.md)

An event triggered prior to action being executed.

#### Inherited from

[Action](Action.md).[onBeforeExecuteObservable](Action.md#onbeforeexecuteobservable)

#### Defined in

https://github.com/babylon.js/core/src/Actions/action.ts:93

___

### trigger

• **trigger**: `number`

Trigger for the action

#### Inherited from

[Action](Action.md).[trigger](Action.md#trigger)

#### Defined in

https://github.com/babylon.js/core/src/Actions/action.ts:77

___

### triggerOptions

• **triggerOptions**: `any`

Options of the trigger

#### Inherited from

[Action](Action.md).[triggerOptions](Action.md#triggeroptions)

#### Defined in

https://github.com/babylon.js/core/src/Actions/action.ts:102

___

### value

• **value**: `string`

The value to store in the state field.

#### Defined in

https://github.com/babylon.js/core/src/Actions/directActions.ts:75

## Methods

### execute

▸ **execute**(): `void`

Execute the action and store the value on the target state property.

#### Returns

`void`

#### Overrides

[Action](Action.md).[execute](Action.md#execute)

#### Defined in

https://github.com/babylon.js/core/src/Actions/directActions.ts:95

___

### getTriggerParameter

▸ **getTriggerParameter**(): `any`

Gets the trigger parameter

#### Returns

`any`

the trigger parameter

#### Inherited from

[Action](Action.md).[getTriggerParameter](Action.md#gettriggerparameter)

#### Defined in

https://github.com/babylon.js/core/src/Actions/action.ts:128

___

### serialize

▸ **serialize**(`parent`): `any`

Serializes the actions and its related information.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `parent` | `any` | defines the object to serialize in |

#### Returns

`any`

the serialized object

#### Overrides

[Action](Action.md).[serialize](Action.md#serialize)

#### Defined in

https://github.com/babylon.js/core/src/Actions/directActions.ts:104

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

#### Inherited from

[Action](Action.md).[setTriggerParameter](Action.md#settriggerparameter)

#### Defined in

https://github.com/babylon.js/core/src/Actions/action.ts:136

___

### skipToNextActiveAction

▸ **skipToNextActiveAction**(): `void`

Skips to next active action

#### Returns

`void`

#### Inherited from

[Action](Action.md).[skipToNextActiveAction](Action.md#skiptonextactiveaction)

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

#### Inherited from

[Action](Action.md).[then](Action.md#then)

#### Defined in

https://github.com/babylon.js/core/src/Actions/action.ts:206
