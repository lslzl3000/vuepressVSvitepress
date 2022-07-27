[@dev/core](../README.md) / [Exports](../modules.md) / PointerInfo

# Class: PointerInfo

This type contains all the data related to a pointer event in Babylon.js.
The event member is an instance of PointerEvent for all types except PointerWheel and is of type MouseWheelEvent when type equals PointerWheel. The different event types can be found in the PointerEventTypes class.

## Hierarchy

- [`PointerInfoBase`](PointerInfoBase.md)

  ↳ **`PointerInfo`**

## Table of contents

### Constructors

- [constructor](PointerInfo.md#constructor)

### Properties

- [event](PointerInfo.md#event)
- [pickInfo](PointerInfo.md#pickinfo)
- [type](PointerInfo.md#type)

## Constructors

### constructor

• **new PointerInfo**(`type`, `event`, `pickInfo`)

Instantiates a PointerInfo to store pointer related info to the onPointerObservable event.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | `number` | Defines the type of event (PointerEventTypes) |
| `event` | [`IMouseEvent`](../interfaces/IMouseEvent.md) | Defines the related dom event |
| `pickInfo` | [`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md) | Defines the picking info associated to the info (if any)\ |

#### Overrides

[PointerInfoBase](PointerInfoBase.md).[constructor](PointerInfoBase.md#constructor)

#### Defined in

packages/dev/core/src/Events/pointerEvents.ts:113

## Properties

### event

• **event**: [`IMouseEvent`](../interfaces/IMouseEvent.md)

#### Inherited from

[PointerInfoBase](PointerInfoBase.md).[event](PointerInfoBase.md#event)

#### Defined in

packages/dev/core/src/Events/pointerEvents.ts:59

___

### pickInfo

• **pickInfo**: [`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md)

#### Defined in

packages/dev/core/src/Events/pointerEvents.ts:119

___

### type

• **type**: `number`

#### Inherited from

[PointerInfoBase](PointerInfoBase.md).[type](PointerInfoBase.md#type)

#### Defined in

packages/dev/core/src/Events/pointerEvents.ts:55
