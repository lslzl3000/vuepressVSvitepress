[@dev/core](../README.md) / [Exports](../modules.md) / ActionEvent

# Class: ActionEvent

ActionEvent is the event being sent when an action is triggered.

## Implements

- [`IActionEvent`](../interfaces/IActionEvent.md)

## Table of contents

### Constructors

- [constructor](ActionEvent.md#constructor)

### Properties

- [additionalData](ActionEvent.md#additionaldata)
- [meshUnderPointer](ActionEvent.md#meshunderpointer)
- [pointerX](ActionEvent.md#pointerx)
- [pointerY](ActionEvent.md#pointery)
- [source](ActionEvent.md#source)
- [sourceEvent](ActionEvent.md#sourceevent)

### Methods

- [CreateNew](ActionEvent.md#createnew)
- [CreateNewFromPrimitive](ActionEvent.md#createnewfromprimitive)
- [CreateNewFromScene](ActionEvent.md#createnewfromscene)
- [CreateNewFromSprite](ActionEvent.md#createnewfromsprite)

## Constructors

### constructor

• **new ActionEvent**(`source`, `pointerX`, `pointerY`, `meshUnderPointer`, `sourceEvent?`, `additionalData?`)

Creates a new ActionEvent

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | `any` | The mesh or sprite that triggered the action |
| `pointerX` | `number` | The X mouse cursor position at the time of the event |
| `pointerY` | `number` | The Y mouse cursor position at the time of the event |
| `meshUnderPointer` | [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md) | The mesh that is currently pointed at (can be null) |
| `sourceEvent?` | `any` | the original (browser) event that triggered the ActionEvent |
| `additionalData?` | `any` | additional data for the event |

#### Defined in

https://github.com/babylon.js/core/src/Actions/actionEvent.ts:38

## Properties

### additionalData

• `Optional` **additionalData**: `any`

additional data for the event

#### Implementation of

[IActionEvent](../interfaces/IActionEvent.md).[additionalData](../interfaces/IActionEvent.md#additionaldata)

#### Defined in

https://github.com/babylon.js/core/src/Actions/actionEvent.ts:50

___

### meshUnderPointer

• **meshUnderPointer**: [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

The mesh that is currently pointed at (can be null)

#### Implementation of

[IActionEvent](../interfaces/IActionEvent.md).[meshUnderPointer](../interfaces/IActionEvent.md#meshunderpointer)

#### Defined in

https://github.com/babylon.js/core/src/Actions/actionEvent.ts:46

___

### pointerX

• **pointerX**: `number`

The X mouse cursor position at the time of the event

#### Implementation of

[IActionEvent](../interfaces/IActionEvent.md).[pointerX](../interfaces/IActionEvent.md#pointerx)

#### Defined in

https://github.com/babylon.js/core/src/Actions/actionEvent.ts:42

___

### pointerY

• **pointerY**: `number`

The Y mouse cursor position at the time of the event

#### Implementation of

[IActionEvent](../interfaces/IActionEvent.md).[pointerY](../interfaces/IActionEvent.md#pointery)

#### Defined in

https://github.com/babylon.js/core/src/Actions/actionEvent.ts:44

___

### source

• **source**: `any`

The mesh or sprite that triggered the action

#### Implementation of

[IActionEvent](../interfaces/IActionEvent.md).[source](../interfaces/IActionEvent.md#source)

#### Defined in

https://github.com/babylon.js/core/src/Actions/actionEvent.ts:40

___

### sourceEvent

• `Optional` **sourceEvent**: `any`

the original (browser) event that triggered the ActionEvent

#### Implementation of

[IActionEvent](../interfaces/IActionEvent.md).[sourceEvent](../interfaces/IActionEvent.md#sourceevent)

#### Defined in

https://github.com/babylon.js/core/src/Actions/actionEvent.ts:48

## Methods

### CreateNew

▸ `Static` **CreateNew**(`source`, `evt?`, `additionalData?`): [`ActionEvent`](ActionEvent.md)

Helper function to auto-create an ActionEvent from a source mesh.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | [`AbstractMesh`](AbstractMesh.md) | The source mesh that triggered the event |
| `evt?` | `any` | The original (browser) event |
| `additionalData?` | `any` | additional data for the event |

#### Returns

[`ActionEvent`](ActionEvent.md)

the new ActionEvent

#### Defined in

https://github.com/babylon.js/core/src/Actions/actionEvent.ts:60

___

### CreateNewFromPrimitive

▸ `Static` **CreateNewFromPrimitive**(`prim`, `pointerPos`, `evt?`, `additionalData?`): [`ActionEvent`](ActionEvent.md)

Helper function to auto-create an ActionEvent from a primitive

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `prim` | `any` | defines the target primitive |
| `pointerPos` | [`Vector2`](Vector2.md) | defines the pointer position |
| `evt?` | `Event` | The original (browser) event |
| `additionalData?` | `any` | additional data for the event |

#### Returns

[`ActionEvent`](ActionEvent.md)

the new ActionEvent

#### Defined in

https://github.com/babylon.js/core/src/Actions/actionEvent.ts:95

___

### CreateNewFromScene

▸ `Static` **CreateNewFromScene**(`scene`, `evt`): [`ActionEvent`](ActionEvent.md)

Helper function to auto-create an ActionEvent from a scene. If triggered by a mesh use ActionEvent.CreateNew

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | the scene where the event occurred |
| `evt` | `any` | The original (browser) event |

#### Returns

[`ActionEvent`](ActionEvent.md)

the new ActionEvent

#### Defined in

https://github.com/babylon.js/core/src/Actions/actionEvent.ts:83

___

### CreateNewFromSprite

▸ `Static` **CreateNewFromSprite**(`source`, `scene`, `evt?`, `additionalData?`): [`ActionEvent`](ActionEvent.md)

Helper function to auto-create an ActionEvent from a source sprite

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `source` | [`Sprite`](Sprite.md) | The source sprite that triggered the event |
| `scene` | [`Scene`](Scene.md) | Scene associated with the sprite |
| `evt?` | `any` | The original (browser) event |
| `additionalData?` | `any` | additional data for the event |

#### Returns

[`ActionEvent`](ActionEvent.md)

the new ActionEvent

#### Defined in

https://github.com/babylon.js/core/src/Actions/actionEvent.ts:73
