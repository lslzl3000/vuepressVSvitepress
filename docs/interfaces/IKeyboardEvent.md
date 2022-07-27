[@dev/core](../README.md) / [Exports](../modules.md) / IKeyboardEvent

# Interface: IKeyboardEvent

Native friendly interface for KeyboardEvent Object

## Hierarchy

- [`IUIEvent`](IUIEvent.md)

  ↳ **`IKeyboardEvent`**

## Table of contents

### Properties

- [altKey](IKeyboardEvent.md#altkey)
- [charCode](IKeyboardEvent.md#charcode)
- [code](IKeyboardEvent.md#code)
- [ctrlKey](IKeyboardEvent.md#ctrlkey)
- [currentTarget](IKeyboardEvent.md#currenttarget)
- [inputIndex](IKeyboardEvent.md#inputindex)
- [key](IKeyboardEvent.md#key)
- [keyCode](IKeyboardEvent.md#keycode)
- [metaKey](IKeyboardEvent.md#metakey)
- [preventDefault](IKeyboardEvent.md#preventdefault)
- [shiftKey](IKeyboardEvent.md#shiftkey)
- [srcElement](IKeyboardEvent.md#srcelement)
- [target](IKeyboardEvent.md#target)
- [type](IKeyboardEvent.md#type)

## Properties

### altKey

• **altKey**: `boolean`

Status of Alt key being pressed

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:59

___

### charCode

• `Optional` **charCode**: `number`

Unicode value of character pressed

**`Deprecated`**

Required for event, use keyCode instead.

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:65

___

### code

• **code**: `string`

Code for key based on layout

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:70

___

### ctrlKey

• **ctrlKey**: `boolean`

Status of Ctrl key being pressed

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:75

___

### currentTarget

• `Optional` **currentTarget**: `any`

Current target for an event

#### Inherited from

[IUIEvent](IUIEvent.md).[currentTarget](IUIEvent.md#currenttarget)

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:28

___

### inputIndex

• **inputIndex**: `number`

Input array index

#### Inherited from

[IUIEvent](IUIEvent.md).[inputIndex](IUIEvent.md#inputindex)

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:23

___

### key

• **key**: `string`

String representation of key

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:80

___

### keyCode

• **keyCode**: `number`

ASCII value of key

**`Deprecated`**

Used with DeviceSourceManager

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:85

___

### metaKey

• **metaKey**: `boolean`

Status of Meta key (eg. Windows key) being pressed

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:90

___

### preventDefault

• **preventDefault**: () => `void`

#### Type declaration

▸ (): `void`

Tells user agent what to do when not explicitly handled

##### Returns

`void`

#### Inherited from

[IUIEvent](IUIEvent.md).[preventDefault](IUIEvent.md#preventdefault)

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:49

___

### shiftKey

• **shiftKey**: `boolean`

Status of Shift key being pressed

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:95

___

### srcElement

• `Optional` **srcElement**: `any`

Alias for target

**`Deprecated`**

Use target instead

#### Inherited from

[IUIEvent](IUIEvent.md).[srcElement](IUIEvent.md#srcelement)

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:34

___

### target

• **target**: `any`

Reference to object where object was dispatched

#### Inherited from

[IUIEvent](IUIEvent.md).[target](IUIEvent.md#target)

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:44

___

### type

• **type**: `string`

Type of event

#### Inherited from

[IUIEvent](IUIEvent.md).[type](IUIEvent.md#type)

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:39
