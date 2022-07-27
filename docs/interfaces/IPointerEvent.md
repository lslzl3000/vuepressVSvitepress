[@dev/core](../README.md) / [Exports](../modules.md) / IPointerEvent

# Interface: IPointerEvent

Native friendly interface for PointerEvent Object

## Hierarchy

- [`IMouseEvent`](IMouseEvent.md)

  ↳ **`IPointerEvent`**

## Table of contents

### Properties

- [altKey](IPointerEvent.md#altkey)
- [button](IPointerEvent.md#button)
- [buttons](IPointerEvent.md#buttons)
- [clientX](IPointerEvent.md#clientx)
- [clientY](IPointerEvent.md#clienty)
- [ctrlKey](IPointerEvent.md#ctrlkey)
- [currentTarget](IPointerEvent.md#currenttarget)
- [detail](IPointerEvent.md#detail)
- [inputIndex](IPointerEvent.md#inputindex)
- [metaKey](IPointerEvent.md#metakey)
- [movementX](IPointerEvent.md#movementx)
- [movementY](IPointerEvent.md#movementy)
- [mozMovementX](IPointerEvent.md#mozmovementx)
- [mozMovementY](IPointerEvent.md#mozmovementy)
- [msMovementX](IPointerEvent.md#msmovementx)
- [msMovementY](IPointerEvent.md#msmovementy)
- [offsetX](IPointerEvent.md#offsetx)
- [offsetY](IPointerEvent.md#offsety)
- [pageX](IPointerEvent.md#pagex)
- [pageY](IPointerEvent.md#pagey)
- [pointerId](IPointerEvent.md#pointerid)
- [pointerType](IPointerEvent.md#pointertype)
- [preventDefault](IPointerEvent.md#preventdefault)
- [shiftKey](IPointerEvent.md#shiftkey)
- [srcElement](IPointerEvent.md#srcelement)
- [target](IPointerEvent.md#target)
- [type](IPointerEvent.md#type)
- [webkitMovementX](IPointerEvent.md#webkitmovementx)
- [webkitMovementY](IPointerEvent.md#webkitmovementy)
- [x](IPointerEvent.md#x)
- [y](IPointerEvent.md#y)

## Properties

### altKey

• **altKey**: `boolean`

Status of Alt key being pressed

#### Inherited from

[IMouseEvent](IMouseEvent.md).[altKey](IMouseEvent.md#altkey)

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:110

___

### button

• **button**: `number`

Value of single mouse button pressed

#### Inherited from

[IMouseEvent](IMouseEvent.md).[button](IMouseEvent.md#button)

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:115

___

### buttons

• **buttons**: `number`

Value of all mouse buttons pressed

#### Inherited from

[IMouseEvent](IMouseEvent.md).[buttons](IMouseEvent.md#buttons)

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:120

___

### clientX

• **clientX**: `number`

Current X coordinate

#### Inherited from

[IMouseEvent](IMouseEvent.md).[clientX](IMouseEvent.md#clientx)

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:125

___

### clientY

• **clientY**: `number`

Current Y coordinate

#### Inherited from

[IMouseEvent](IMouseEvent.md).[clientY](IMouseEvent.md#clienty)

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:130

___

### ctrlKey

• **ctrlKey**: `boolean`

Status of Ctrl key being pressed

#### Inherited from

[IMouseEvent](IMouseEvent.md).[ctrlKey](IMouseEvent.md#ctrlkey)

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:135

___

### currentTarget

• `Optional` **currentTarget**: `any`

Current target for an event

#### Inherited from

[IMouseEvent](IMouseEvent.md).[currentTarget](IMouseEvent.md#currenttarget)

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:28

___

### detail

• `Optional` **detail**: `number`

Provides current click count

#### Inherited from

[IMouseEvent](IMouseEvent.md).[detail](IMouseEvent.md#detail)

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:140

___

### inputIndex

• **inputIndex**: [`LeftClick`](../enums/PointerInput.md#leftclick) \| [`MiddleClick`](../enums/PointerInput.md#middleclick) \| [`RightClick`](../enums/PointerInput.md#rightclick) \| [`BrowserBack`](../enums/PointerInput.md#browserback) \| [`BrowserForward`](../enums/PointerInput.md#browserforward) \| [`Move`](../enums/PointerInput.md#move)

Subset of possible PointerInput values for events, excluding ones that CANNOT be in events organically and mouse wheel values

#### Overrides

[IMouseEvent](IMouseEvent.md).[inputIndex](IMouseEvent.md#inputindex)

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:230

___

### metaKey

• **metaKey**: `boolean`

Status of Meta key (eg. Windows key) being pressed

#### Inherited from

[IMouseEvent](IMouseEvent.md).[metaKey](IMouseEvent.md#metakey)

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:145

___

### movementX

• **movementX**: `number`

Delta of movement on X axis

#### Inherited from

[IMouseEvent](IMouseEvent.md).[movementX](IMouseEvent.md#movementx)

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:150

___

### movementY

• **movementY**: `number`

Delta of movement on Y axis

#### Inherited from

[IMouseEvent](IMouseEvent.md).[movementY](IMouseEvent.md#movementy)

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:155

___

### mozMovementX

• `Optional` **mozMovementX**: `number`

Delta of movement on X axis

#### Inherited from

[IMouseEvent](IMouseEvent.md).[mozMovementX](IMouseEvent.md#mozmovementx)

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:160

___

### mozMovementY

• `Optional` **mozMovementY**: `number`

Delta of movement on Y axis

#### Inherited from

[IMouseEvent](IMouseEvent.md).[mozMovementY](IMouseEvent.md#mozmovementy)

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:165

___

### msMovementX

• `Optional` **msMovementX**: `any`

Delta of movement on X axis

#### Inherited from

[IMouseEvent](IMouseEvent.md).[msMovementX](IMouseEvent.md#msmovementx)

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:170

___

### msMovementY

• `Optional` **msMovementY**: `any`

Delta of movement on Y axis

#### Inherited from

[IMouseEvent](IMouseEvent.md).[msMovementY](IMouseEvent.md#msmovementy)

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:175

___

### offsetX

• **offsetX**: `number`

Current coordinate of X within container

#### Inherited from

[IMouseEvent](IMouseEvent.md).[offsetX](IMouseEvent.md#offsetx)

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:180

___

### offsetY

• **offsetY**: `number`

Current coordinate of Y within container

#### Inherited from

[IMouseEvent](IMouseEvent.md).[offsetY](IMouseEvent.md#offsety)

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:185

___

### pageX

• **pageX**: `number`

Horizontal coordinate of event

#### Inherited from

[IMouseEvent](IMouseEvent.md).[pageX](IMouseEvent.md#pagex)

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:190

___

### pageY

• **pageY**: `number`

Vertical coordinate of event

#### Inherited from

[IMouseEvent](IMouseEvent.md).[pageY](IMouseEvent.md#pagey)

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:195

___

### pointerId

• **pointerId**: `number`

Pointer Event ID

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:235

___

### pointerType

• **pointerType**: `string`

Type of pointer

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:240

___

### preventDefault

• **preventDefault**: () => `void`

#### Type declaration

▸ (): `void`

Tells user agent what to do when not explicitly handled

##### Returns

`void`

#### Inherited from

[IMouseEvent](IMouseEvent.md).[preventDefault](IMouseEvent.md#preventdefault)

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:49

___

### shiftKey

• **shiftKey**: `boolean`

Status of Shift key being pressed

#### Inherited from

[IMouseEvent](IMouseEvent.md).[shiftKey](IMouseEvent.md#shiftkey)

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:200

___

### srcElement

• `Optional` **srcElement**: `any`

Alias for target

**`Deprecated`**

Use target instead

#### Inherited from

[IMouseEvent](IMouseEvent.md).[srcElement](IMouseEvent.md#srcelement)

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:34

___

### target

• **target**: `any`

Reference to object where object was dispatched

#### Inherited from

[IMouseEvent](IMouseEvent.md).[target](IMouseEvent.md#target)

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:44

___

### type

• **type**: `string`

Type of event

#### Inherited from

[IMouseEvent](IMouseEvent.md).[type](IMouseEvent.md#type)

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:39

___

### webkitMovementX

• `Optional` **webkitMovementX**: `any`

Delta of movement on X axis

#### Inherited from

[IMouseEvent](IMouseEvent.md).[webkitMovementX](IMouseEvent.md#webkitmovementx)

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:205

___

### webkitMovementY

• `Optional` **webkitMovementY**: `any`

Delta of movement on Y axis

#### Inherited from

[IMouseEvent](IMouseEvent.md).[webkitMovementY](IMouseEvent.md#webkitmovementy)

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:210

___

### x

• **x**: `number`

Alias of clientX

#### Inherited from

[IMouseEvent](IMouseEvent.md).[x](IMouseEvent.md#x)

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:215

___

### y

• **y**: `number`

Alias of clientY

#### Inherited from

[IMouseEvent](IMouseEvent.md).[y](IMouseEvent.md#y)

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:220
