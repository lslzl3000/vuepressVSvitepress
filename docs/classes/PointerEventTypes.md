[@dev/core](../README.md) / [Exports](../modules.md) / PointerEventTypes

# Class: PointerEventTypes

Gather the list of pointer event types as constants.

## Table of contents

### Constructors

- [constructor](PointerEventTypes.md#constructor)

### Properties

- [POINTERDOUBLETAP](PointerEventTypes.md#pointerdoubletap)
- [POINTERDOWN](PointerEventTypes.md#pointerdown)
- [POINTERMOVE](PointerEventTypes.md#pointermove)
- [POINTERPICK](PointerEventTypes.md#pointerpick)
- [POINTERTAP](PointerEventTypes.md#pointertap)
- [POINTERUP](PointerEventTypes.md#pointerup)
- [POINTERWHEEL](PointerEventTypes.md#pointerwheel)

## Constructors

### constructor

• **new PointerEventTypes**()

## Properties

### POINTERDOUBLETAP

▪ `Static` `Readonly` **POINTERDOUBLETAP**: ``64``

The pointerdoubletap event is fired when a the object has been touched and released twice without drag.

#### Defined in

packages/dev/core/src/Events/pointerEvents.ts:39

___

### POINTERDOWN

▪ `Static` `Readonly` **POINTERDOWN**: ``1``

The pointerdown event is fired when a pointer becomes active. For mouse, it is fired when the device transitions from no buttons depressed to at least one button depressed. For touch, it is fired when physical contact is made with the digitizer. For pen, it is fired when the stylus makes physical contact with the digitizer.

#### Defined in

packages/dev/core/src/Events/pointerEvents.ts:15

___

### POINTERMOVE

▪ `Static` `Readonly` **POINTERMOVE**: ``4``

The pointermove event is fired when a pointer changes coordinates.

#### Defined in

packages/dev/core/src/Events/pointerEvents.ts:23

___

### POINTERPICK

▪ `Static` `Readonly` **POINTERPICK**: ``16``

The pointerpick event is fired when a mesh or sprite has been picked by the pointer.

#### Defined in

packages/dev/core/src/Events/pointerEvents.ts:31

___

### POINTERTAP

▪ `Static` `Readonly` **POINTERTAP**: ``32``

The pointertap event is fired when a the object has been touched and released without drag.

#### Defined in

packages/dev/core/src/Events/pointerEvents.ts:35

___

### POINTERUP

▪ `Static` `Readonly` **POINTERUP**: ``2``

The pointerup event is fired when a pointer is no longer active.

#### Defined in

packages/dev/core/src/Events/pointerEvents.ts:19

___

### POINTERWHEEL

▪ `Static` `Readonly` **POINTERWHEEL**: ``8``

The pointerwheel event is fired when a mouse wheel has been rotated.

#### Defined in

packages/dev/core/src/Events/pointerEvents.ts:27
