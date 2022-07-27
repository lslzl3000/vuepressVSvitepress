[@dev/core](../README.md) / [Exports](../modules.md) / PointerInfoPre

# Class: PointerInfoPre

This class is used to store pointer related info for the onPrePointerObservable event.
Set the skipOnPointerObservable property to true if you want the engine to stop any process after this event is triggered, even not calling onPointerObservable

## Hierarchy

- [`PointerInfoBase`](PointerInfoBase.md)

  ↳ **`PointerInfoPre`**

## Table of contents

### Constructors

- [constructor](PointerInfoPre.md#constructor)

### Properties

- [event](PointerInfoPre.md#event)
- [localPosition](PointerInfoPre.md#localposition)
- [nearInteractionPickingInfo](PointerInfoPre.md#nearinteractionpickinginfo)
- [ray](PointerInfoPre.md#ray)
- [skipOnPointerObservable](PointerInfoPre.md#skiponpointerobservable)
- [type](PointerInfoPre.md#type)

## Constructors

### constructor

• **new PointerInfoPre**(`type`, `event`, `localX`, `localY`)

Instantiates a PointerInfoPre to store pointer related info to the onPrePointerObservable event.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | `number` | Defines the type of event (PointerEventTypes) |
| `event` | [`IMouseEvent`](../interfaces/IMouseEvent.md) | Defines the related dom event |
| `localX` | `number` | Defines the local x coordinates of the pointer when the event occured |
| `localY` | `number` | Defines the local y coordinates of the pointer when the event occured |

#### Overrides

[PointerInfoBase](PointerInfoBase.md).[constructor](PointerInfoBase.md#constructor)

#### Defined in

packages/dev/core/src/Events/pointerEvents.ts:95

## Properties

### event

• **event**: [`IMouseEvent`](../interfaces/IMouseEvent.md)

#### Inherited from

[PointerInfoBase](PointerInfoBase.md).[event](PointerInfoBase.md#event)

#### Defined in

packages/dev/core/src/Events/pointerEvents.ts:59

___

### localPosition

• **localPosition**: [`Vector2`](Vector2.md)

Defines the local position of the pointer on the canvas.

#### Defined in

packages/dev/core/src/Events/pointerEvents.ts:81

___

### nearInteractionPickingInfo

• **nearInteractionPickingInfo**: [`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md)

Defines picking info coming from a near interaction (proximity instead of ray-based picking)

#### Defined in

packages/dev/core/src/Events/pointerEvents.ts:76

___

### ray

• **ray**: [`Nullable`](../modules.md#nullable)[`Ray`](Ray.md) = `null`

Ray from a pointer if available (eg. 6dof controller)

#### Defined in

packages/dev/core/src/Events/pointerEvents.ts:71

___

### skipOnPointerObservable

• **skipOnPointerObservable**: `boolean`

Defines whether the engine should skip the next OnPointerObservable associated to this pre.

#### Defined in

packages/dev/core/src/Events/pointerEvents.ts:86

___

### type

• **type**: `number`

#### Inherited from

[PointerInfoBase](PointerInfoBase.md).[type](PointerInfoBase.md#type)

#### Defined in

packages/dev/core/src/Events/pointerEvents.ts:55
