[@dev/core](../README.md) / [Exports](../modules.md) / KeyboardInfo

# Class: KeyboardInfo

This class is used to store keyboard related info for the onKeyboardObservable event.

## Hierarchy

- **`KeyboardInfo`**

  ↳ [`KeyboardInfoPre`](KeyboardInfoPre.md)

## Table of contents

### Constructors

- [constructor](KeyboardInfo.md#constructor)

### Properties

- [event](KeyboardInfo.md#event)
- [type](KeyboardInfo.md#type)

## Constructors

### constructor

• **new KeyboardInfo**(`type`, `event`)

Instantiates a new keyboard info.
This class is used to store keyboard related info for the onKeyboardObservable event.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | `number` | Defines the type of event (KeyboardEventTypes) |
| `event` | [`IKeyboardEvent`](../interfaces/IKeyboardEvent.md) | Defines the related dom event |

#### Defined in

https://github.com/babylon.js/core/src/Events/keyboardEvents.ts:27

## Properties

### event

• **event**: [`IKeyboardEvent`](../interfaces/IKeyboardEvent.md)

#### Defined in

https://github.com/babylon.js/core/src/Events/keyboardEvents.ts:35

___

### type

• **type**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Events/keyboardEvents.ts:31
