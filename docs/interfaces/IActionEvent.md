[@dev/core](../README.md) / [Exports](../modules.md) / IActionEvent

# Interface: IActionEvent

Interface used to define ActionEvent

## Implemented by

- [`ActionEvent`](../classes/ActionEvent.md)

## Table of contents

### Properties

- [additionalData](IActionEvent.md#additionaldata)
- [meshUnderPointer](IActionEvent.md#meshunderpointer)
- [pointerX](IActionEvent.md#pointerx)
- [pointerY](IActionEvent.md#pointery)
- [source](IActionEvent.md#source)
- [sourceEvent](IActionEvent.md#sourceevent)

## Properties

### additionalData

• `Optional` **additionalData**: `any`

additional data for the event

#### Defined in

https://github.com/babylon.js/core/src/Actions/actionEvent.ts:22

___

### meshUnderPointer

• **meshUnderPointer**: [`Nullable`](../modules.md#nullable)[`AbstractMesh`](../classes/AbstractMesh.md)

The mesh that is currently pointed at (can be null)

#### Defined in

https://github.com/babylon.js/core/src/Actions/actionEvent.ts:18

___

### pointerX

• **pointerX**: `number`

The X mouse cursor position at the time of the event

#### Defined in

https://github.com/babylon.js/core/src/Actions/actionEvent.ts:14

___

### pointerY

• **pointerY**: `number`

The Y mouse cursor position at the time of the event

#### Defined in

https://github.com/babylon.js/core/src/Actions/actionEvent.ts:16

___

### source

• **source**: `any`

The mesh or sprite that triggered the action

#### Defined in

https://github.com/babylon.js/core/src/Actions/actionEvent.ts:12

___

### sourceEvent

• `Optional` **sourceEvent**: `any`

the original (browser) event that triggered the ActionEvent

#### Defined in

https://github.com/babylon.js/core/src/Actions/actionEvent.ts:20
