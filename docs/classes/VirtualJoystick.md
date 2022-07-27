[@dev/core](../README.md) / [Exports](../modules.md) / VirtualJoystick

# Class: VirtualJoystick

Class used to define virtual joystick (used in touch mode)

## Table of contents

### Constructors

- [constructor](VirtualJoystick.md#constructor)

### Properties

- [\_action](VirtualJoystick.md#_action)
- [\_alwaysVisible](VirtualJoystick.md#_alwaysvisible)
- [\_axisTargetedByLeftAndRight](VirtualJoystick.md#_axistargetedbyleftandright)
- [\_axisTargetedByUpAndDown](VirtualJoystick.md#_axistargetedbyupanddown)
- [\_clearContainerSize](VirtualJoystick.md#_clearcontainersize)
- [\_clearContainerSizeOffset](VirtualJoystick.md#_clearcontainersizeoffset)
- [\_clearPuckSize](VirtualJoystick.md#_clearpucksize)
- [\_clearPuckSizeOffset](VirtualJoystick.md#_clearpucksizeoffset)
- [\_containerImage](VirtualJoystick.md#_containerimage)
- [\_deltaJoystickVector](VirtualJoystick.md#_deltajoystickvector)
- [\_inversedSensibility](VirtualJoystick.md#_inversedsensibility)
- [\_joystickColor](VirtualJoystick.md#_joystickcolor)
- [\_joystickContainerSize](VirtualJoystick.md#_joystickcontainersize)
- [\_joystickPointerId](VirtualJoystick.md#_joystickpointerid)
- [\_joystickPointerPos](VirtualJoystick.md#_joystickpointerpos)
- [\_joystickPointerStartPos](VirtualJoystick.md#_joystickpointerstartpos)
- [\_joystickPosition](VirtualJoystick.md#_joystickposition)
- [\_joystickPreviousPointerPos](VirtualJoystick.md#_joystickpreviouspointerpos)
- [\_joystickPuckSize](VirtualJoystick.md#_joystickpucksize)
- [\_joystickSensibility](VirtualJoystick.md#_joysticksensibility)
- [\_leftJoystick](VirtualJoystick.md#_leftjoystick)
- [\_onPointerDownHandlerRef](VirtualJoystick.md#_onpointerdownhandlerref)
- [\_onPointerMoveHandlerRef](VirtualJoystick.md#_onpointermovehandlerref)
- [\_onPointerUpHandlerRef](VirtualJoystick.md#_onpointeruphandlerref)
- [\_onResize](VirtualJoystick.md#_onresize)
- [\_puckImage](VirtualJoystick.md#_puckimage)
- [\_touches](VirtualJoystick.md#_touches)
- [deltaPosition](VirtualJoystick.md#deltaposition)
- [limitToContainer](VirtualJoystick.md#limittocontainer)
- [pressed](VirtualJoystick.md#pressed)
- [reverseLeftRight](VirtualJoystick.md#reverseleftright)
- [reverseUpDown](VirtualJoystick.md#reverseupdown)
- [Canvas](VirtualJoystick.md#canvas)
- [\_AlwaysVisibleSticks](VirtualJoystick.md#_alwaysvisiblesticks)
- [\_GlobalJoystickIndex](VirtualJoystick.md#_globaljoystickindex)
- [\_HalfWidth](VirtualJoystick.md#_halfwidth)
- [\_VJCanvasContext](VirtualJoystick.md#_vjcanvascontext)
- [\_VJCanvasHeight](VirtualJoystick.md#_vjcanvasheight)
- [\_VJCanvasWidth](VirtualJoystick.md#_vjcanvaswidth)

### Accessors

- [alwaysVisible](VirtualJoystick.md#alwaysvisible)
- [containerSize](VirtualJoystick.md#containersize)
- [puckSize](VirtualJoystick.md#pucksize)

### Methods

- [\_clearPreviousDraw](VirtualJoystick.md#_clearpreviousdraw)
- [\_drawContainer](VirtualJoystick.md#_drawcontainer)
- [\_drawPuck](VirtualJoystick.md#_drawpuck)
- [\_drawVirtualJoystick](VirtualJoystick.md#_drawvirtualjoystick)
- [\_onPointerDown](VirtualJoystick.md#_onpointerdown)
- [\_onPointerMove](VirtualJoystick.md#_onpointermove)
- [\_onPointerUp](VirtualJoystick.md#_onpointerup)
- [clearPosition](VirtualJoystick.md#clearposition)
- [releaseCanvas](VirtualJoystick.md#releasecanvas)
- [setActionOnTouch](VirtualJoystick.md#setactionontouch)
- [setAxisForLeftRight](VirtualJoystick.md#setaxisforleftright)
- [setAxisForUpDown](VirtualJoystick.md#setaxisforupdown)
- [setContainerImage](VirtualJoystick.md#setcontainerimage)
- [setJoystickColor](VirtualJoystick.md#setjoystickcolor)
- [setJoystickSensibility](VirtualJoystick.md#setjoysticksensibility)
- [setPosition](VirtualJoystick.md#setposition)
- [setPuckImage](VirtualJoystick.md#setpuckimage)
- [\_GetDefaultOptions](VirtualJoystick.md#_getdefaultoptions)

## Constructors

### constructor

• **new VirtualJoystick**(`leftJoystick?`, `customizations?`)

Creates a new virtual joystick

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `leftJoystick?` | `boolean` | defines that the joystick is for left hand (false by default) |
| `customizations?` | `Partial``VirtualJoystickCustomizations` | Defines the options we want to customize the VirtualJoystick |

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:146

## Properties

### \_action

• `Private` **\_action**: () => `any`

#### Type declaration

▸ (): `any`

##### Returns

`any`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:110

___

### \_alwaysVisible

• `Private` **\_alwaysVisible**: `boolean`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:124

___

### \_axisTargetedByLeftAndRight

• `Private` **\_axisTargetedByLeftAndRight**: [`JoystickAxis`](../enums/JoystickAxis.md)

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:111

___

### \_axisTargetedByUpAndDown

• `Private` **\_axisTargetedByUpAndDown**: [`JoystickAxis`](../enums/JoystickAxis.md)

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:112

___

### \_clearContainerSize

• `Private` **\_clearContainerSize**: `number`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:132

___

### \_clearContainerSizeOffset

• `Private` **\_clearContainerSizeOffset**: `number`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:134

___

### \_clearPuckSize

• `Private` **\_clearPuckSize**: `number`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:131

___

### \_clearPuckSizeOffset

• `Private` **\_clearPuckSizeOffset**: `number`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:133

___

### \_containerImage

• `Private` **\_containerImage**: `HTMLImageElement`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:126

___

### \_deltaJoystickVector

• `Private` **\_deltaJoystickVector**: [`Vector2`](Vector2.md)

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:120

___

### \_inversedSensibility

• `Private` **\_inversedSensibility**: `number`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:114

___

### \_joystickColor

• `Private` **\_joystickColor**: `string`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:116

___

### \_joystickContainerSize

• `Private` **\_joystickContainerSize**: `number`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:130

___

### \_joystickPointerId

• `Private` **\_joystickPointerId**: `number`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:115

___

### \_joystickPointerPos

• `Private` **\_joystickPointerPos**: [`Vector2`](Vector2.md)

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:117

___

### \_joystickPointerStartPos

• `Private` **\_joystickPointerStartPos**: [`Vector2`](Vector2.md)

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:119

___

### \_joystickPosition

• `Private` **\_joystickPosition**: [`Nullable`](../modules.md#nullable)[`Vector2`](Vector2.md)

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:123

___

### \_joystickPreviousPointerPos

• `Private` **\_joystickPreviousPointerPos**: [`Vector2`](Vector2.md)

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:118

___

### \_joystickPuckSize

• `Private` **\_joystickPuckSize**: `number`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:129

___

### \_joystickSensibility

• `Private` **\_joystickSensibility**: `number`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:113

___

### \_leftJoystick

• `Private` **\_leftJoystick**: `boolean`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:121

___

### \_onPointerDownHandlerRef

• `Private` **\_onPointerDownHandlerRef**: (`e`: `PointerEvent`) => `any`

#### Type declaration

▸ (`e`): `any`

##### Parameters

| Name | Type |
| :------ | :------ |
| `e` | `PointerEvent` |

##### Returns

`any`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:136

___

### \_onPointerMoveHandlerRef

• `Private` **\_onPointerMoveHandlerRef**: (`e`: `PointerEvent`) => `any`

#### Type declaration

▸ (`e`): `any`

##### Parameters

| Name | Type |
| :------ | :------ |
| `e` | `PointerEvent` |

##### Returns

`any`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:137

___

### \_onPointerUpHandlerRef

• `Private` **\_onPointerUpHandlerRef**: (`e`: `PointerEvent`) => `any`

#### Type declaration

▸ (`e`): `any`

##### Parameters

| Name | Type |
| :------ | :------ |
| `e` | `PointerEvent` |

##### Returns

`any`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:138

___

### \_onResize

• `Private` **\_onResize**: (`e`: `any`) => `any`

#### Type declaration

▸ (`e`): `any`

##### Parameters

| Name | Type |
| :------ | :------ |
| `e` | `any` |

##### Returns

`any`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:139

___

### \_puckImage

• `Private` **\_puckImage**: `HTMLImageElement`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:125

___

### \_touches

• `Private` **\_touches**: [`StringDictionary`](StringDictionary.md)`PointerEvent` \| { `prevX`: `number` ; `prevY`: `number` ; `x`: `number` ; `y`: `number`  }

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:122

___

### deltaPosition

• **deltaPosition**: [`Vector3`](Vector3.md)

Gets the offset value for the position (ie. the change of the position value)

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:75

___

### limitToContainer

• **limitToContainer**: `boolean`

boolean indicating whether or not the joystick's puck's movement should be limited to the joystick's container area

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:88

___

### pressed

• **pressed**: `boolean`

Gets a boolean indicating if the virtual joystick was pressed

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:79

___

### reverseLeftRight

• **reverseLeftRight**: `boolean`

Gets or sets a boolean indicating that left and right values must be inverted

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:67

___

### reverseUpDown

• **reverseUpDown**: `boolean`

Gets or sets a boolean indicating that up and down values must be inverted

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:71

___

### Canvas

▪ `Static` **Canvas**: [`Nullable`](../modules.md#nullable)`HTMLCanvasElement`

Canvas the virtual joystick will render onto, default z-index of this is 5

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:83

___

### \_AlwaysVisibleSticks

▪ `Static` `Private` **\_AlwaysVisibleSticks**: `number` = `0`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:92

___

### \_GlobalJoystickIndex

▪ `Static` `Private` **\_GlobalJoystickIndex**: `number` = `0`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:91

___

### \_HalfWidth

▪ `Static` `Private` **\_HalfWidth**: `number`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:96

___

### \_VJCanvasContext

▪ `Static` `Private` **\_VJCanvasContext**: `CanvasRenderingContext2D`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:93

___

### \_VJCanvasHeight

▪ `Static` `Private` **\_VJCanvasHeight**: `number`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:95

___

### \_VJCanvasWidth

▪ `Static` `Private` **\_VJCanvasWidth**: `number`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:94

## Accessors

### alwaysVisible

• `get` **alwaysVisible**(): `boolean`

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:473

• `set` **alwaysVisible**(`value`): `void`

Defines whether or not the joystick container is always visible

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:458

___

### containerSize

• `get` **containerSize**(): `number`

#### Returns

`number`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:430

• `set` **containerSize**(`newSize`): `void`

Size of the joystick's container

#### Parameters

| Name | Type |
| :------ | :------ |
| `newSize` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:425

___

### puckSize

• `get` **puckSize**(): `number`

#### Returns

`number`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:442

• `set` **puckSize**(`newSize`): `void`

Size of the joystick's puck

#### Parameters

| Name | Type |
| :------ | :------ |
| `newSize` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:437

## Methods

### \_clearPreviousDraw

▸ `Private` **_clearPreviousDraw**(): `void`

Clears the canvas from the previous puck / container draw

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:536

___

### \_drawContainer

▸ `Private` **_drawContainer**(): `void`

Draws the Virtual Joystick's container

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:581

___

### \_drawPuck

▸ `Private` **_drawPuck**(): `void`

Draws the Virtual Joystick's puck

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:610

___

### \_drawVirtualJoystick

▸ `Private` **_drawVirtualJoystick**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:629

___

### \_onPointerDown

▸ `Private` **_onPointerDown**(`e`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `e` | `PointerEvent` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:285

___

### \_onPointerMove

▸ `Private` **_onPointerMove**(`e`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `e` | `PointerEvent` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:328

___

### \_onPointerUp

▸ `Private` **_onPointerUp**(`e`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `e` | `PointerEvent` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:396

___

### clearPosition

▸ **clearPosition**(): `void`

Clears the set position of the joystick

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:449

___

### releaseCanvas

▸ **releaseCanvas**(): `void`

Release internal HTML canvas

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:668

___

### setActionOnTouch

▸ **setActionOnTouch**(`action`): `void`

Defines a callback to call when the joystick is touched

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `action` | () => `any` | defines the callback |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:495

___

### setAxisForLeftRight

▸ **setAxisForLeftRight**(`axis`): `void`

Defines which axis you'd like to control for left & right

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `axis` | [`JoystickAxis`](../enums/JoystickAxis.md) | defines the axis to use |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:503

___

### setAxisForUpDown

▸ **setAxisForUpDown**(`axis`): `void`

Defines which axis you'd like to control for up & down

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `axis` | [`JoystickAxis`](../enums/JoystickAxis.md) | defines the axis to use |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:520

___

### setContainerImage

▸ **setContainerImage**(`urlPath`): `void`

Loads `urlPath` to be used for the container's image

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `urlPath` | `string` | defines the urlPath of an image to use |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:560

___

### setJoystickColor

▸ **setJoystickColor**(`newColor`): `void`

Change the color of the virtual joystick

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newColor` | `string` | a string that must be a CSS color value (like "red") or the hexa value (like "#FF0000") |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:418

___

### setJoystickSensibility

▸ **setJoystickSensibility**(`newJoystickSensibility`): `void`

Defines joystick sensibility (ie. the ratio between a physical move and virtual joystick position change)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newJoystickSensibility` | `number` | defines the new sensibility |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:280

___

### setPosition

▸ **setPosition**(`x`, `y`): `void`

Sets the constant position of the Joystick container

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | X axis coordinate |
| `y` | `number` | Y axis coordinate |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:482

___

### setPuckImage

▸ **setPuckImage**(`urlPath`): `void`

Loads `urlPath` to be used for the puck's image

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `urlPath` | `string` | defines the urlPath of an image to use |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:571

___

### \_GetDefaultOptions

▸ `Static` `Private` **_GetDefaultOptions**(): `VirtualJoystickCustomizations`

#### Returns

`VirtualJoystickCustomizations`

#### Defined in

packages/dev/core/src/Misc/virtualJoystick.ts:97
