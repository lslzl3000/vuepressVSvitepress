[@dev/core](../README.md) / [Exports](../modules.md) / IncrementValueAction

# Class: IncrementValueAction

This defines an action responsible to increment the target value
 to a desired value once triggered.

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions

## Hierarchy

- [`Action`](Action.md)

  ↳ **`IncrementValueAction`**

## Table of contents

### Constructors

- [constructor](IncrementValueAction.md#constructor)

### Properties

- [\_effectiveTarget](IncrementValueAction.md#_effectivetarget)
- [\_property](IncrementValueAction.md#_property)
- [\_target](IncrementValueAction.md#_target)
- [onBeforeExecuteObservable](IncrementValueAction.md#onbeforeexecuteobservable)
- [propertyPath](IncrementValueAction.md#propertypath)
- [trigger](IncrementValueAction.md#trigger)
- [triggerOptions](IncrementValueAction.md#triggeroptions)
- [value](IncrementValueAction.md#value)

### Methods

- [execute](IncrementValueAction.md#execute)
- [getTriggerParameter](IncrementValueAction.md#gettriggerparameter)
- [serialize](IncrementValueAction.md#serialize)
- [setTriggerParameter](IncrementValueAction.md#settriggerparameter)
- [skipToNextActiveAction](IncrementValueAction.md#skiptonextactiveaction)
- [then](IncrementValueAction.md#then)

## Constructors

### constructor

• **new IncrementValueAction**(`triggerOptions`, `target`, `propertyPath`, `value`, `condition?`)

Instantiate the action

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `triggerOptions` | `any` | defines the trigger options |
| `target` | `any` | defines the object containing the property |
| `propertyPath` | `string` | defines the path of the property to increment in the target |
| `value` | `any` | defines the value value we should increment the property by |
| `condition?` | [`Condition`](Condition.md) | defines the trigger related conditions |

#### Overrides

[Action](Action.md).[constructor](Action.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Actions/directActions.ts:215

## Properties

### \_effectiveTarget

• `Private` **\_effectiveTarget**: `any`

#### Defined in

https://github.com/babylon.js/core/src/Actions/directActions.ts:204

___

### \_property

• `Private` **\_property**: `string`

#### Defined in

https://github.com/babylon.js/core/src/Actions/directActions.ts:205

___

### \_target

• `Private` **\_target**: `any`

#### Defined in

https://github.com/babylon.js/core/src/Actions/directActions.ts:203

___

### onBeforeExecuteObservable

• **onBeforeExecuteObservable**: [`Observable`](Observable.md)[`Action`](Action.md)

An event triggered prior to action being executed.

#### Inherited from

[Action](Action.md).[onBeforeExecuteObservable](Action.md#onbeforeexecuteobservable)

#### Defined in

https://github.com/babylon.js/core/src/Actions/action.ts:93

___

### propertyPath

• **propertyPath**: `string`

The path of the property to increment in the target.

#### Defined in

https://github.com/babylon.js/core/src/Actions/directActions.ts:196

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

• **value**: `any`

The value we should increment the property by.

#### Defined in

https://github.com/babylon.js/core/src/Actions/directActions.ts:201

## Methods

### execute

▸ **execute**(): `void`

Execute the action and increment the target of the value amount.

#### Returns

`void`

#### Overrides

[Action](Action.md).[execute](Action.md#execute)

#### Defined in

https://github.com/babylon.js/core/src/Actions/directActions.ts:235

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

https://github.com/babylon.js/core/src/Actions/directActions.ts:248

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
