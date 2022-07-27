[@dev/core](../README.md) / [Exports](../modules.md) / StopSoundAction

# Class: StopSoundAction

This defines an action helpful to stop a defined sound on a triggered action.

## Hierarchy

- [`Action`](Action.md)

  ↳ **`StopSoundAction`**

## Table of contents

### Constructors

- [constructor](StopSoundAction.md#constructor)

### Properties

- [\_sound](StopSoundAction.md#_sound)
- [onBeforeExecuteObservable](StopSoundAction.md#onbeforeexecuteobservable)
- [trigger](StopSoundAction.md#trigger)
- [triggerOptions](StopSoundAction.md#triggeroptions)

### Methods

- [execute](StopSoundAction.md#execute)
- [getTriggerParameter](StopSoundAction.md#gettriggerparameter)
- [serialize](StopSoundAction.md#serialize)
- [setTriggerParameter](StopSoundAction.md#settriggerparameter)
- [skipToNextActiveAction](StopSoundAction.md#skiptonextactiveaction)
- [then](StopSoundAction.md#then)

## Constructors

### constructor

• **new StopSoundAction**(`triggerOptions`, `sound`, `condition?`)

Instantiate the action

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `triggerOptions` | `any` | defines the trigger options |
| `sound` | [`Sound`](Sound.md) | defines the sound to stop |
| `condition?` | [`Condition`](Condition.md) | defines the trigger related conditions |

#### Overrides

[Action](Action.md).[constructor](Action.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Actions/directAudioActions.ts:63

## Properties

### \_sound

• `Private` **\_sound**: [`Sound`](Sound.md)

#### Defined in

https://github.com/babylon.js/core/src/Actions/directAudioActions.ts:55

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

## Methods

### execute

▸ **execute**(): `void`

Execute the action and stop the sound.

#### Returns

`void`

#### Overrides

[Action](Action.md).[execute](Action.md#execute)

#### Defined in

https://github.com/babylon.js/core/src/Actions/directAudioActions.ts:74

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

https://github.com/babylon.js/core/src/Actions/directAudioActions.ts:85

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
