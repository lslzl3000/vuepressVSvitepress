[@dev/core](../README.md) / [Exports](../modules.md) / InterpolateValueAction

# Class: InterpolateValueAction

This defines an action responsible to change the value of a property
by interpolating between its current value and the newly set one once triggered.

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions

## Hierarchy

- [`Action`](Action.md)

  ↳ **`InterpolateValueAction`**

## Table of contents

### Constructors

- [constructor](InterpolateValueAction.md#constructor)

### Properties

- [\_effectiveTarget](InterpolateValueAction.md#_effectivetarget)
- [\_property](InterpolateValueAction.md#_property)
- [\_target](InterpolateValueAction.md#_target)
- [duration](InterpolateValueAction.md#duration)
- [onBeforeExecuteObservable](InterpolateValueAction.md#onbeforeexecuteobservable)
- [onInterpolationDone](InterpolateValueAction.md#oninterpolationdone)
- [onInterpolationDoneObservable](InterpolateValueAction.md#oninterpolationdoneobservable)
- [propertyPath](InterpolateValueAction.md#propertypath)
- [stopOtherAnimations](InterpolateValueAction.md#stopotheranimations)
- [trigger](InterpolateValueAction.md#trigger)
- [triggerOptions](InterpolateValueAction.md#triggeroptions)
- [value](InterpolateValueAction.md#value)

### Methods

- [execute](InterpolateValueAction.md#execute)
- [getTriggerParameter](InterpolateValueAction.md#gettriggerparameter)
- [serialize](InterpolateValueAction.md#serialize)
- [setTriggerParameter](InterpolateValueAction.md#settriggerparameter)
- [skipToNextActiveAction](InterpolateValueAction.md#skiptonextactiveaction)
- [then](InterpolateValueAction.md#then)

## Constructors

### constructor

• **new InterpolateValueAction**(`triggerOptions`, `target`, `propertyPath`, `value`, `duration?`, `condition?`, `stopOtherAnimations?`, `onInterpolationDone?`)

Instantiate the action

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `triggerOptions` | `any` | `undefined` | defines the trigger options |
| `target` | `any` | `undefined` | defines the object containing the value to interpolate |
| `propertyPath` | `string` | `undefined` | defines the path to the property in the target object |
| `value` | `any` | `undefined` | defines the target value at the end of the interpolation |
| `duration` | `number` | `1000` | defines the time it will take for the property to interpolate to the value. |
| `condition?` | [`Condition`](Condition.md) | `undefined` | defines the trigger related conditions |
| `stopOtherAnimations?` | `boolean` | `undefined` | defines if the other scene animations should be stopped when the action has been triggered |
| `onInterpolationDone?` | () => `void` | `undefined` | defines a callback raised once the interpolation animation has been done |

#### Overrides

[Action](Action.md).[constructor](Action.md#constructor)

#### Defined in

packages/dev/core/src/Actions/interpolateValueAction.ts:62

## Properties

### \_effectiveTarget

• `Private` **\_effectiveTarget**: `any`

#### Defined in

packages/dev/core/src/Actions/interpolateValueAction.ts:48

___

### \_property

• `Private` **\_property**: `string`

#### Defined in

packages/dev/core/src/Actions/interpolateValueAction.ts:49

___

### \_target

• `Private` **\_target**: `any`

#### Defined in

packages/dev/core/src/Actions/interpolateValueAction.ts:47

___

### duration

• **duration**: `number` = `1000`

Defines the time it will take for the property to interpolate to the value.

#### Defined in

packages/dev/core/src/Actions/interpolateValueAction.ts:30

___

### onBeforeExecuteObservable

• **onBeforeExecuteObservable**: [`Observable`](Observable.md)[`Action`](Action.md)

An event triggered prior to action being executed.

#### Inherited from

[Action](Action.md).[onBeforeExecuteObservable](Action.md#onbeforeexecuteobservable)

#### Defined in

packages/dev/core/src/Actions/action.ts:93

___

### onInterpolationDone

• `Optional` **onInterpolationDone**: () => `void`

#### Type declaration

▸ (): `void`

Defines a callback raised once the interpolation animation has been done.

##### Returns

`void`

#### Defined in

packages/dev/core/src/Actions/interpolateValueAction.ts:40

___

### onInterpolationDoneObservable

• **onInterpolationDoneObservable**: [`Observable`](Observable.md)[`InterpolateValueAction`](InterpolateValueAction.md)

Observable triggered once the interpolation animation has been done.

#### Defined in

packages/dev/core/src/Actions/interpolateValueAction.ts:45

___

### propertyPath

• **propertyPath**: `string`

Defines the path of the property where the value should be interpolated

#### Defined in

packages/dev/core/src/Actions/interpolateValueAction.ts:20

___

### stopOtherAnimations

• `Optional` **stopOtherAnimations**: `boolean`

Defines if the other scene animations should be stopped when the action has been triggered

#### Defined in

packages/dev/core/src/Actions/interpolateValueAction.ts:35

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

Defines the target value at the end of the interpolation.

#### Defined in

packages/dev/core/src/Actions/interpolateValueAction.ts:25

## Methods

### execute

▸ **execute**(): `void`

Execute the action starts the value interpolation.

#### Returns

`void`

#### Overrides

[Action](Action.md).[execute](Action.md#execute)

#### Defined in

packages/dev/core/src/Actions/interpolateValueAction.ts:91

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

packages/dev/core/src/Actions/interpolateValueAction.ts:144

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
