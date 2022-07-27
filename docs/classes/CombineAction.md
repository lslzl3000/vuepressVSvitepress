[@dev/core](../README.md) / [Exports](../modules.md) / CombineAction

# Class: CombineAction

This defines an action responsible to trigger several actions once triggered.

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions

## Hierarchy

- [`Action`](Action.md)

  ↳ **`CombineAction`**

## Table of contents

### Constructors

- [constructor](CombineAction.md#constructor)

### Properties

- [children](CombineAction.md#children)
- [enableChildrenConditions](CombineAction.md#enablechildrenconditions)
- [onBeforeExecuteObservable](CombineAction.md#onbeforeexecuteobservable)
- [trigger](CombineAction.md#trigger)
- [triggerOptions](CombineAction.md#triggeroptions)

### Methods

- [execute](CombineAction.md#execute)
- [getTriggerParameter](CombineAction.md#gettriggerparameter)
- [serialize](CombineAction.md#serialize)
- [setTriggerParameter](CombineAction.md#settriggerparameter)
- [skipToNextActiveAction](CombineAction.md#skiptonextactiveaction)
- [then](CombineAction.md#then)

## Constructors

### constructor

• **new CombineAction**(`triggerOptions`, `children`, `condition?`, `enableChildrenConditions?`)

Instantiate the action

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `triggerOptions` | `any` | `undefined` | defines the trigger options |
| `children` | [`Action`](Action.md)[] | `undefined` | defines the list of aggregated animations to run |
| `condition?` | [`Condition`](Condition.md) | `undefined` | defines the trigger related conditions |
| `enableChildrenConditions` | `boolean` | `true` | defines if the children actions conditions should be check before execution |

#### Overrides

[Action](Action.md).[constructor](Action.md#constructor)

#### Defined in

packages/dev/core/src/Actions/directActions.ts:436

## Properties

### children

• **children**: [`Action`](Action.md)[]

The list of aggregated animations to run.

#### Defined in

packages/dev/core/src/Actions/directActions.ts:422

___

### enableChildrenConditions

• **enableChildrenConditions**: `boolean`

defines if the children actions conditions should be check before execution

#### Defined in

packages/dev/core/src/Actions/directActions.ts:427

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

Execute the action and executes all the aggregated actions.

#### Parameters

| Name | Type |
| :------ | :------ |
| `evt` | [`ActionEvent`](ActionEvent.md) |

#### Returns

`void`

#### Overrides

[Action](Action.md).[execute](Action.md#execute)

#### Defined in

packages/dev/core/src/Actions/directActions.ts:454

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

packages/dev/core/src/Actions/directActions.ts:467

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
