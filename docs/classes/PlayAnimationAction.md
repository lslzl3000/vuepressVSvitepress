[@dev/core](../README.md) / [Exports](../modules.md) / PlayAnimationAction

# Class: PlayAnimationAction

This defines an action responsible to start an animation once triggered.

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions

## Hierarchy

- [`Action`](Action.md)

  ↳ **`PlayAnimationAction`**

## Table of contents

### Constructors

- [constructor](PlayAnimationAction.md#constructor)

### Properties

- [\_target](PlayAnimationAction.md#_target)
- [from](PlayAnimationAction.md#from)
- [loop](PlayAnimationAction.md#loop)
- [onBeforeExecuteObservable](PlayAnimationAction.md#onbeforeexecuteobservable)
- [to](PlayAnimationAction.md#to)
- [trigger](PlayAnimationAction.md#trigger)
- [triggerOptions](PlayAnimationAction.md#triggeroptions)

### Methods

- [execute](PlayAnimationAction.md#execute)
- [getTriggerParameter](PlayAnimationAction.md#gettriggerparameter)
- [serialize](PlayAnimationAction.md#serialize)
- [setTriggerParameter](PlayAnimationAction.md#settriggerparameter)
- [skipToNextActiveAction](PlayAnimationAction.md#skiptonextactiveaction)
- [then](PlayAnimationAction.md#then)

## Constructors

### constructor

• **new PlayAnimationAction**(`triggerOptions`, `target`, `from`, `to`, `loop?`, `condition?`)

Instantiate the action

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `triggerOptions` | `any` | defines the trigger options |
| `target` | `any` | defines the target animation or animation name |
| `from` | `number` | defines from where the animation should start (animation frame) |
| `to` | `number` | defines where the animation should stop (animation frame) |
| `loop?` | `boolean` | defines if the animation should loop or stop after the first play |
| `condition?` | [`Condition`](Condition.md) | defines the trigger related conditions |

#### Overrides

[Action](Action.md).[constructor](Action.md#constructor)

#### Defined in

packages/dev/core/src/Actions/directActions.ts:294

## Properties

### \_target

• `Private` **\_target**: `any`

#### Defined in

packages/dev/core/src/Actions/directActions.ts:283

___

### from

• **from**: `number`

Where the animation should start (animation frame)

#### Defined in

packages/dev/core/src/Actions/directActions.ts:271

___

### loop

• `Optional` **loop**: `boolean`

Define if the animation should loop or stop after the first play.

#### Defined in

packages/dev/core/src/Actions/directActions.ts:281

___

### onBeforeExecuteObservable

• **onBeforeExecuteObservable**: [`Observable`](Observable.md)[`Action`](Action.md)

An event triggered prior to action being executed.

#### Inherited from

[Action](Action.md).[onBeforeExecuteObservable](Action.md#onbeforeexecuteobservable)

#### Defined in

packages/dev/core/src/Actions/action.ts:93

___

### to

• **to**: `number`

Where the animation should stop (animation frame)

#### Defined in

packages/dev/core/src/Actions/directActions.ts:276

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

Execute the action and play the animation.

#### Returns

`void`

#### Overrides

[Action](Action.md).[execute](Action.md#execute)

#### Defined in

packages/dev/core/src/Actions/directActions.ts:308

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

packages/dev/core/src/Actions/directActions.ts:318

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
