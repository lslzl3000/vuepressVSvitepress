[@dev/core](../README.md) / [Exports](../modules.md) / IMouseEvent

# Interface: IMouseEvent

Native friendly interface for MouseEvent Object

## Hierarchy

- [`IUIEvent`](IUIEvent.md)

  ↳ **`IMouseEvent`**

  ↳↳ [`IPointerEvent`](IPointerEvent.md)

  ↳↳ [`IWheelEvent`](IWheelEvent.md)

## Table of contents

### Properties

- [altKey](IMouseEvent.md#altkey)
- [button](IMouseEvent.md#button)
- [buttons](IMouseEvent.md#buttons)
- [clientX](IMouseEvent.md#clientx)
- [clientY](IMouseEvent.md#clienty)
- [ctrlKey](IMouseEvent.md#ctrlkey)
- [currentTarget](IMouseEvent.md#currenttarget)
- [detail](IMouseEvent.md#detail)
- [inputIndex](IMouseEvent.md#inputindex)
- [metaKey](IMouseEvent.md#metakey)
- [movementX](IMouseEvent.md#movementx)
- [movementY](IMouseEvent.md#movementy)
- [mozMovementX](IMouseEvent.md#mozmovementx)
- [mozMovementY](IMouseEvent.md#mozmovementy)
- [msMovementX](IMouseEvent.md#msmovementx)
- [msMovementY](IMouseEvent.md#msmovementy)
- [offsetX](IMouseEvent.md#offsetx)
- [offsetY](IMouseEvent.md#offsety)
- [pageX](IMouseEvent.md#pagex)
- [pageY](IMouseEvent.md#pagey)
- [preventDefault](IMouseEvent.md#preventdefault)
- [shiftKey](IMouseEvent.md#shiftkey)
- [srcElement](IMouseEvent.md#srcelement)
- [target](IMouseEvent.md#target)
- [type](IMouseEvent.md#type)
- [webkitMovementX](IMouseEvent.md#webkitmovementx)
- [webkitMovementY](IMouseEvent.md#webkitmovementy)
- [x](IMouseEvent.md#x)
- [y](IMouseEvent.md#y)

## Properties

### altKey

• **altKey**: `boolean`

Status of Alt key being pressed

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:110

___

### button

• **button**: `number`

Value of single mouse button pressed

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:115

___

### buttons

• **buttons**: `number`

Value of all mouse buttons pressed

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:120

___

### clientX

• **clientX**: `number`

Current X coordinate

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:125

___

### clientY

• **clientY**: `number`

Current Y coordinate

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:130

___

### ctrlKey

• **ctrlKey**: `boolean`

Status of Ctrl key being pressed

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:135

___

### currentTarget

• `Optional` **currentTarget**: `any`

Current target for an event

#### Inherited from

[IUIEvent](IUIEvent.md).[currentTarget](IUIEvent.md#currenttarget)

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:28

___

### detail

• `Optional` **detail**: `number`

Provides current click count

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:140

___

### inputIndex

• **inputIndex**: [`LeftClick`](../enums/PointerInput.md#leftclick) \| [`MiddleClick`](../enums/PointerInput.md#middleclick) \| [`RightClick`](../enums/PointerInput.md#rightclick) \| [`BrowserBack`](../enums/PointerInput.md#browserback) \| [`BrowserForward`](../enums/PointerInput.md#browserforward) \| [`MouseWheelX`](../enums/PointerInput.md#mousewheelx) \| [`MouseWheelY`](../enums/PointerInput.md#mousewheely) \| [`MouseWheelZ`](../enums/PointerInput.md#mousewheelz) \| [`Move`](../enums/PointerInput.md#move)

Subset of possible PointerInput values for events, excluding ones that CANNOT be in events organically

#### Overrides

[IUIEvent](IUIEvent.md).[inputIndex](IUIEvent.md#inputindex)

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:105

___

### metaKey

• **metaKey**: `boolean`

Status of Meta key (eg. Windows key) being pressed

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:145

___

### movementX

• **movementX**: `number`

Delta of movement on X axis

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:150

___

### movementY

• **movementY**: `number`

Delta of movement on Y axis

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:155

___

### mozMovementX

• `Optional` **mozMovementX**: `number`

Delta of movement on X axis

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:160

___

### mozMovementY

• `Optional` **mozMovementY**: `number`

Delta of movement on Y axis

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:165

___

### msMovementX

• `Optional` **msMovementX**: `any`

Delta of movement on X axis

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:170

___

### msMovementY

• `Optional` **msMovementY**: `any`

Delta of movement on Y axis

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:175

___

### offsetX

• **offsetX**: `number`

Current coordinate of X within container

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:180

___

### offsetY

• **offsetY**: `number`

Current coordinate of Y within container

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:185

___

### pageX

• **pageX**: `number`

Horizontal coordinate of event

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:190

___

### pageY

• **pageY**: `number`

Vertical coordinate of event

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:195

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

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:200

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

___

### webkitMovementX

• `Optional` **webkitMovementX**: `any`

Delta of movement on X axis

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:205

___

### webkitMovementY

• `Optional` **webkitMovementY**: `any`

Delta of movement on Y axis

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:210

___

### x

• **x**: `number`

Alias of clientX

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:215

___

### y

• **y**: `number`

Alias of clientY

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:220
