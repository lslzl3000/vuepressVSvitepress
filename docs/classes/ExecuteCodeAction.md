[@dev/core](../README.md) / [Exports](../modules.md) / ExecuteCodeAction

# Class: ExecuteCodeAction

This defines an action responsible to run code (external event) once triggered.

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions

## Hierarchy

- [`Action`](Action.md)

  ↳ **`ExecuteCodeAction`**

## Table of contents

### Constructors

- [constructor](ExecuteCodeAction.md#constructor)

### Properties

- [func](ExecuteCodeAction.md#func)
- [onBeforeExecuteObservable](ExecuteCodeAction.md#onbeforeexecuteobservable)
- [trigger](ExecuteCodeAction.md#trigger)
- [triggerOptions](ExecuteCodeAction.md#triggeroptions)

### Methods

- [execute](ExecuteCodeAction.md#execute)
- [getTriggerParameter](ExecuteCodeAction.md#gettriggerparameter)
- [serialize](ExecuteCodeAction.md#serialize)
- [setTriggerParameter](ExecuteCodeAction.md#settriggerparameter)
- [skipToNextActiveAction](ExecuteCodeAction.md#skiptonextactiveaction)
- [then](ExecuteCodeAction.md#then)

## Constructors

### constructor

• **new ExecuteCodeAction**(`triggerOptions`, `func`, `condition?`)

Instantiate the action

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `triggerOptions` | `any` | defines the trigger options |
| `func` | (`evt`: [`ActionEvent`](ActionEvent.md)) => `void` | defines the callback function to run |
| `condition?` | [`Condition`](Condition.md) | defines the trigger related conditions |

#### Overrides

[Action](Action.md).[constructor](Action.md#constructor)

#### Defined in

packages/dev/core/src/Actions/directActions.ts:501

## Properties

### func

• **func**: (`evt`: [`ActionEvent`](ActionEvent.md)) => `void`

#### Type declaration

▸ (`evt`): `void`

The callback function to run.

##### Parameters

| Name | Type |
| :------ | :------ |
| `evt` | [`ActionEvent`](ActionEvent.md) |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Actions/directActions.ts:493

___

### onBeforeExecuteObservable

• **onBeforeExecuteObservable**: [`Observable`](Observable.md)[`Action`](Action.md)

An event triggered prior to action being executed.

#### Inherited from

[Action](Action.md).[onBeforeExecuteObservable](Action.md#onbeforeexecuteobservable)

#### Defined in

packages/dev/core/src/Actions/action.ts:93

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

▸ **execute**(`evt`): `void`

Execute the action and run the attached code.

#### Parameters

| Name | Type |
| :------ | :------ |
| `evt` | [`ActionEvent`](ActionEvent.md) |

#### Returns

`void`

#### Overrides

[Action](Action.md).[execute](Action.md#execute)

#### Defined in

packages/dev/core/src/Actions/directActions.ts:510

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

Serialize placeholder for child classes

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `parent` | `any` | of child |

#### Returns

`any`

the serialized object

#### Inherited from

[Action](Action.md).[serialize](Action.md#serialize)

#### Defined in

packages/dev/core/src/Actions/action.ts:240

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
