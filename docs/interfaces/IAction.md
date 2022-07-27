[@dev/core](../README.md) / [Exports](../modules.md) / IAction

# Interface: IAction

Interface used to define Action

## Implemented by

- [`Action`](../classes/Action.md)

## Table of contents

### Properties

- [trigger](IAction.md#trigger)
- [triggerOptions](IAction.md#triggeroptions)

### Methods

- [getTriggerParameter](IAction.md#gettriggerparameter)
- [serialize](IAction.md#serialize)
- [then](IAction.md#then)

## Properties

### trigger

• **trigger**: `number`

Trigger for the action

#### Defined in

https://github.com/babylon.js/core/src/Actions/action.ts:24

___

### triggerOptions

• **triggerOptions**: `any`

Options of the trigger

#### Defined in

https://github.com/babylon.js/core/src/Actions/action.ts:27

## Methods

### getTriggerParameter

▸ **getTriggerParameter**(): `any`

Gets the trigger parameters

#### Returns

`any`

the trigger parameters

#### Defined in

https://github.com/babylon.js/core/src/Actions/action.ts:33

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

#### Defined in

https://github.com/babylon.js/core/src/Actions/action.ts:46

___

### then

▸ **then**(`action`): [`IAction`](IAction.md)

Adds action to chain of actions, may be a DoNothingAction

**`See`**

https://www.babylonjs-playground.com/#1T30HR#0

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `action` | [`IAction`](IAction.md) | defines the next action to execute |

#### Returns

[`IAction`](IAction.md)

The action passed in

#### Defined in

https://github.com/babylon.js/core/src/Actions/action.ts:66
