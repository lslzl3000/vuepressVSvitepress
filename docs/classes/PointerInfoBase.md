[@dev/core](../README.md) / [Exports](../modules.md) / PointerInfoBase

# Class: PointerInfoBase

Base class of pointer info types.

## Hierarchy

- **`PointerInfoBase`**

  ↳ [`PointerInfoPre`](PointerInfoPre.md)

  ↳ [`PointerInfo`](PointerInfo.md)

## Table of contents

### Constructors

- [constructor](PointerInfoBase.md#constructor)

### Properties

- [event](PointerInfoBase.md#event)
- [type](PointerInfoBase.md#type)

## Constructors

### constructor

• **new PointerInfoBase**(`type`, `event`)

Instantiates the base class of pointers info.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | `number` | Defines the type of event (PointerEventTypes) |
| `event` | [`IMouseEvent`](../interfaces/IMouseEvent.md) | Defines the related dom event |

#### Defined in

https://github.com/babylon.js/core/src/Events/pointerEvents.ts:51

## Properties

### event

• **event**: [`IMouseEvent`](../interfaces/IMouseEvent.md)

#### Defined in

https://github.com/babylon.js/core/src/Events/pointerEvents.ts:59

___

### type

• **type**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Events/pointerEvents.ts:55
