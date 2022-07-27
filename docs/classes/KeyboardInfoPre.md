[@dev/core](../README.md) / [Exports](../modules.md) / KeyboardInfoPre

# Class: KeyboardInfoPre

This class is used to store keyboard related info for the onPreKeyboardObservable event.
Set the skipOnKeyboardObservable property to true if you want the engine to stop any process after this event is triggered, even not calling onKeyboardObservable

## Hierarchy

- [`KeyboardInfo`](KeyboardInfo.md)

  ↳ **`KeyboardInfoPre`**

## Table of contents

### Constructors

- [constructor](KeyboardInfoPre.md#constructor)

### Properties

- [event](KeyboardInfoPre.md#event)
- [skipOnKeyboardObservable](KeyboardInfoPre.md#skiponkeyboardobservable)
- [type](KeyboardInfoPre.md#type)

### Accessors

- [skipOnPointerObservable](KeyboardInfoPre.md#skiponpointerobservable)

## Constructors

### constructor

• **new KeyboardInfoPre**(`type`, `event`)

Instantiates a new keyboard pre info.
This class is used to store keyboard related info for the onPreKeyboardObservable event.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | `number` | Defines the type of event (KeyboardEventTypes) |
| `event` | [`IKeyboardEvent`](../interfaces/IKeyboardEvent.md) | Defines the related dom event |

#### Overrides

[KeyboardInfo](KeyboardInfo.md).[constructor](KeyboardInfo.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Events/keyboardEvents.ts:66

## Properties

### event

• **event**: [`IKeyboardEvent`](../interfaces/IKeyboardEvent.md)

#### Inherited from

[KeyboardInfo](KeyboardInfo.md).[event](KeyboardInfo.md#event)

#### Defined in

https://github.com/babylon.js/core/src/Events/keyboardEvents.ts:74

___

### skipOnKeyboardObservable

• **skipOnKeyboardObservable**: `boolean`

Defines whether the engine should skip the next onKeyboardObservable associated to this pre.

#### Defined in

https://github.com/babylon.js/core/src/Events/keyboardEvents.ts:47

___

### type

• **type**: `number`

#### Inherited from

[KeyboardInfo](KeyboardInfo.md).[type](KeyboardInfo.md#type)

#### Defined in

https://github.com/babylon.js/core/src/Events/keyboardEvents.ts:70

## Accessors

### skipOnPointerObservable

• `get` **skipOnPointerObservable**(): `boolean`

Defines whether the engine should skip the next onKeyboardObservable associated to this pre.

**`Deprecated`**

use skipOnKeyboardObservable property instead

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Events/keyboardEvents.ts:53

• `set` **skipOnPointerObservable**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Events/keyboardEvents.ts:56
