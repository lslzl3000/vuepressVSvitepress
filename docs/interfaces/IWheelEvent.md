[@dev/core](../README.md) / [Exports](../modules.md) / IWheelEvent

# Interface: IWheelEvent

Native friendly interface for WheelEvent Object

## Hierarchy

- [`IMouseEvent`](IMouseEvent.md)

  ↳ **`IWheelEvent`**

## Table of contents

### Properties

- [altKey](IWheelEvent.md#altkey)
- [button](IWheelEvent.md#button)
- [buttons](IWheelEvent.md#buttons)
- [clientX](IWheelEvent.md#clientx)
- [clientY](IWheelEvent.md#clienty)
- [ctrlKey](IWheelEvent.md#ctrlkey)
- [currentTarget](IWheelEvent.md#currenttarget)
- [deltaMode](IWheelEvent.md#deltamode)
- [deltaX](IWheelEvent.md#deltax)
- [deltaY](IWheelEvent.md#deltay)
- [deltaZ](IWheelEvent.md#deltaz)
- [detail](IWheelEvent.md#detail)
- [inputIndex](IWheelEvent.md#inputindex)
- [metaKey](IWheelEvent.md#metakey)
- [movementX](IWheelEvent.md#movementx)
- [movementY](IWheelEvent.md#movementy)
- [mozMovementX](IWheelEvent.md#mozmovementx)
- [mozMovementY](IWheelEvent.md#mozmovementy)
- [msMovementX](IWheelEvent.md#msmovementx)
- [msMovementY](IWheelEvent.md#msmovementy)
- [offsetX](IWheelEvent.md#offsetx)
- [offsetY](IWheelEvent.md#offsety)
- [pageX](IWheelEvent.md#pagex)
- [pageY](IWheelEvent.md#pagey)
- [preventDefault](IWheelEvent.md#preventdefault)
- [shiftKey](IWheelEvent.md#shiftkey)
- [srcElement](IWheelEvent.md#srcelement)
- [target](IWheelEvent.md#target)
- [type](IWheelEvent.md#type)
- [webkitMovementX](IWheelEvent.md#webkitmovementx)
- [webkitMovementY](IWheelEvent.md#webkitmovementy)
- [wheelDelta](IWheelEvent.md#wheeldelta)
- [x](IWheelEvent.md#x)
- [y](IWheelEvent.md#y)

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

### deltaMode

• **deltaMode**: `number`

Units for delta value

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:255

___

### deltaX

• **deltaX**: `number`

Horizontal scroll delta

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:260

___

### deltaY

• **deltaY**: `number`

Vertical scroll delta

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:265

___

### deltaZ

• **deltaZ**: `number`

Z-Axis scroll delta

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:270

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

• **inputIndex**: [`MouseWheelX`](../enums/PointerInput.md#mousewheelx) \| [`MouseWheelY`](../enums/PointerInput.md#mousewheely) \| [`MouseWheelZ`](../enums/PointerInput.md#mousewheelz)

Subset of possible PointerInput values for events that can only be used with mouse wheel

#### Overrides

[IMouseEvent](IMouseEvent.md).[inputIndex](IMouseEvent.md#inputindex)

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:250

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

### wheelDelta

• `Optional` **wheelDelta**: `number`

WheelDelta (From MouseWheel Event)

#### Defined in

https://github.com/babylon.js/core/src/Events/deviceInputEvents.ts:275

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
