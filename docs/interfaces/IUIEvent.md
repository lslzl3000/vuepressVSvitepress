[@dev/core](../README.md) / [Exports](../modules.md) / IUIEvent

# Interface: IUIEvent

Native friendly interface for Event Object

## Hierarchy

- **`IUIEvent`**

  ↳ [`IKeyboardEvent`](IKeyboardEvent.md)

  ↳ [`IMouseEvent`](IMouseEvent.md)

## Table of contents

### Properties

- [currentTarget](IUIEvent.md#currenttarget)
- [inputIndex](IUIEvent.md#inputindex)
- [preventDefault](IUIEvent.md#preventdefault)
- [srcElement](IUIEvent.md#srcelement)
- [target](IUIEvent.md#target)
- [type](IUIEvent.md#type)

## Properties

### currentTarget

• `Optional` **currentTarget**: `any`

Current target for an event

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:28

___

### inputIndex

• **inputIndex**: `number`

Input array index

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:23

___

### preventDefault

• **preventDefault**: () => `void`

#### Type declaration

▸ (): `void`

Tells user agent what to do when not explicitly handled

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:49

___

### srcElement

• `Optional` **srcElement**: `any`

Alias for target

**`Deprecated`**

Use target instead

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:34

___

### target

• **target**: `any`

Reference to object where object was dispatched

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:44

___

### type

• **type**: `string`

Type of event

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:39
