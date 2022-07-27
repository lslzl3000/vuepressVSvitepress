[@dev/core](../README.md) / [Exports](../modules.md) / SwitchBooleanAction

# Class: SwitchBooleanAction

This defines an action responsible to toggle a boolean once triggered.

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions

## Hierarchy

- [`Action`](Action.md)

  ↳ **`SwitchBooleanAction`**

## Table of contents

### Constructors

- [constructor](SwitchBooleanAction.md#constructor)

### Properties

- [\_effectiveTarget](SwitchBooleanAction.md#_effectivetarget)
- [\_property](SwitchBooleanAction.md#_property)
- [\_target](SwitchBooleanAction.md#_target)
- [onBeforeExecuteObservable](SwitchBooleanAction.md#onbeforeexecuteobservable)
- [propertyPath](SwitchBooleanAction.md#propertypath)
- [trigger](SwitchBooleanAction.md#trigger)
- [triggerOptions](SwitchBooleanAction.md#triggeroptions)

### Methods

- [execute](SwitchBooleanAction.md#execute)
- [getTriggerParameter](SwitchBooleanAction.md#gettriggerparameter)
- [serialize](SwitchBooleanAction.md#serialize)
- [setTriggerParameter](SwitchBooleanAction.md#settriggerparameter)
- [skipToNextActiveAction](SwitchBooleanAction.md#skiptonextactiveaction)
- [then](SwitchBooleanAction.md#then)

## Constructors

### constructor

• **new SwitchBooleanAction**(`triggerOptions`, `target`, `propertyPath`, `condition?`)

Instantiate the action

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `triggerOptions` | `any` | defines the trigger options |
| `target` | `any` | defines the object containing the boolean |
| `propertyPath` | `string` | defines the path to the boolean property in the target object |
| `condition?` | [`Condition`](Condition.md) | defines the trigger related conditions |

#### Overrides

[Action](Action.md).[constructor](Action.md#constructor)

#### Defined in

packages/dev/core/src/Actions/directActions.ts:31

## Properties

### \_effectiveTarget

• `Private` **\_effectiveTarget**: `any`

#### Defined in

packages/dev/core/src/Actions/directActions.ts:21

___

### \_property

• `Private` **\_property**: `string`

#### Defined in

packages/dev/core/src/Actions/directActions.ts:22

___

### \_target

• `Private` **\_target**: `any`

#### Defined in

packages/dev/core/src/Actions/directActions.ts:20

___

### onBeforeExecuteObservable

• **onBeforeExecuteObservable**: [`Observable`](Observable.md)[`Action`](Action.md)

An event triggered prior to action being executed.

#### Inherited from

[Action](Action.md).[onBeforeExecuteObservable](Action.md#onbeforeexecuteobservable)

#### Defined in

packages/dev/core/src/Actions/action.ts:93

___

### propertyPath

• **propertyPath**: `string`

The path to the boolean property in the target object

#### Defined in

packages/dev/core/src/Actions/directActions.ts:18

___

### trigger

• **trigger**: `number`

Trigger for the action

#### Inherited from

[Action](Action.md).[trigger](Action.md#trigger)

#### Defined in

packages/dev/core/src/Actions/action.ts:77

___

### triggerOptions

• **triggerOptions**: `any`

Options of the trigger

#### Inherited from

[Action](Action.md).[triggerOptions](Action.md#triggeroptions)

#### Defined in

packages/dev/core/src/Actions/action.ts:102

## Methods

### execute

▸ **execute**(): `void`

Execute the action toggle the boolean value.

#### Returns

`void`

#### Overrides

[Action](Action.md).[execute](Action.md#execute)

#### Defined in

packages/dev/core/src/Actions/directActions.ts:46

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

packages/dev/core/src/Actions/action.ts:128

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

packages/dev/core/src/Actions/directActions.ts:55

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

packages/dev/core/src/Actions/action.ts:136

___

### skipToNextActiveAction

▸ **skipToNextActiveAction**(): `void`

Skips to next active action

#### Returns

`void`

#### Inherited from

[Action](Action.md).[skipToNextActiveAction](Action.md#skiptonextactiveaction)

#### Defined in

packages/dev/core/src/Actions/action.ts:188

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

packages/dev/core/src/Actions/action.ts:206
