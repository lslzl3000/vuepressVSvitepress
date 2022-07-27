[@dev/core](../README.md) / [Exports](../modules.md) / ClipboardInfo

# Class: ClipboardInfo

This class is used to store clipboard related info for the onClipboardObservable event.

## Table of contents

### Constructors

- [constructor](ClipboardInfo.md#constructor)

### Properties

- [event](ClipboardInfo.md#event)
- [type](ClipboardInfo.md#type)

### Methods

- [GetTypeFromCharacter](ClipboardInfo.md#gettypefromcharacter)

## Constructors

### constructor

• **new ClipboardInfo**(`type`, `event`)

Creates an instance of ClipboardInfo.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | `number` | Defines the type of event (BABYLON.ClipboardEventTypes) |
| `event` | `ClipboardEvent` | Defines the related dom event |

#### Defined in

https://github.com/babylon.js/core/src/Events/clipboardEvents.ts:28

## Properties

### event

• **event**: `ClipboardEvent`

#### Defined in

https://github.com/babylon.js/core/src/Events/clipboardEvents.ts:36

___

### type

• **type**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Events/clipboardEvents.ts:32

## Methods

### GetTypeFromCharacter

▸ `Static` **GetTypeFromCharacter**(`keyCode`): `number`

Get the clipboard event's type from the keycode.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `keyCode` | `number` | Defines the keyCode for the current keyboard event. |

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Events/clipboardEvents.ts:44
