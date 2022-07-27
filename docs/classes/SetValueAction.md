[@dev/core](../README.md) / [Exports](../modules.md) / SetValueAction

# Class: SetValueAction

This defines an action responsible to set a property of the target
 to a desired value once triggered.

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions

## Hierarchy

- [`Action`](Action.md)

  ↳ **`SetValueAction`**

## Table of contents

### Constructors

- [constructor](SetValueAction.md#constructor)

### Properties

- [\_effectiveTarget](SetValueAction.md#_effectivetarget)
- [\_property](SetValueAction.md#_property)
- [\_target](SetValueAction.md#_target)
- [onBeforeExecuteObservable](SetValueAction.md#onbeforeexecuteobservable)
- [propertyPath](SetValueAction.md#propertypath)
- [trigger](SetValueAction.md#trigger)
- [triggerOptions](SetValueAction.md#triggeroptions)
- [value](SetValueAction.md#value)

### Methods

- [execute](SetValueAction.md#execute)
- [getTriggerParameter](SetValueAction.md#gettriggerparameter)
- [serialize](SetValueAction.md#serialize)
- [setTriggerParameter](SetValueAction.md#settriggerparameter)
- [skipToNextActiveAction](SetValueAction.md#skiptonextactiveaction)
- [then](SetValueAction.md#then)

## Constructors

### constructor

• **new SetValueAction**(`triggerOptions`, `target`, `propertyPath`, `value`, `condition?`)

Instantiate the action

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `triggerOptions` | `any` | defines the trigger options |
| `target` | `any` | defines the object containing the property |
| `propertyPath` | `string` | defines the path of the property to set in the target |
| `value` | `any` | defines the value to set in the property |
| `condition?` | [`Condition`](Condition.md) | defines the trigger related conditions |

#### Overrides

[Action](Action.md).[constructor](Action.md#constructor)

#### Defined in

packages/dev/core/src/Actions/directActions.ts:143

## Properties

### \_effectiveTarget

• `Private` **\_effectiveTarget**: `any`

#### Defined in

packages/dev/core/src/Actions/directActions.ts:132

___

### \_property

• `Private` **\_property**: `string`

#### Defined in

packages/dev/core/src/Actions/directActions.ts:133

___

### \_target

• `Private` **\_target**: `any`

#### Defined in

packages/dev/core/src/Actions/directActions.ts:131

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

The path of the property to set in the target.

#### Defined in

packages/dev/core/src/Actions/directActions.ts:124

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

___

### value

• **value**: `any`

The value to set in the property

#### Defined in

packages/dev/core/src/Actions/directActions.ts:129

## Methods

### execute

▸ **execute**(): `void`

Execute the action and set the targeted property to the desired value.

#### Returns

`void`

#### Overrides

[Action](Action.md).[execute](Action.md#execute)

#### Defined in

packages/dev/core/src/Actions/directActions.ts:159

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

packages/dev/core/src/Actions/directActions.ts:172

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
