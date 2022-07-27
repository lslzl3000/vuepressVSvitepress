[@dev/core](../README.md) / [Exports](../modules.md) / GenericPad

# Class: GenericPad

Represents a generic gamepad

## Hierarchy

- [`Gamepad`](Gamepad.md)

  ↳ **`GenericPad`**

## Table of contents

### Constructors

- [constructor](GenericPad.md#constructor)

### Properties

- [\_buttons](GenericPad.md#_buttons)
- [\_invertLeftStickY](GenericPad.md#_invertleftsticky)
- [\_onbuttondown](GenericPad.md#_onbuttondown)
- [\_onbuttonup](GenericPad.md#_onbuttonup)
- [browserGamepad](GenericPad.md#browsergamepad)
- [id](GenericPad.md#id)
- [index](GenericPad.md#index)
- [onButtonDownObservable](GenericPad.md#onbuttondownobservable)
- [onButtonUpObservable](GenericPad.md#onbuttonupobservable)
- [type](GenericPad.md#type)
- [DUALSHOCK](GenericPad.md#dualshock)
- [GAMEPAD](GenericPad.md#gamepad)
- [GENERIC](GenericPad.md#generic)
- [POSE\_ENABLED](GenericPad.md#pose_enabled)
- [XBOX](GenericPad.md#xbox)

### Accessors

- [isConnected](GenericPad.md#isconnected)
- [leftStick](GenericPad.md#leftstick)
- [rightStick](GenericPad.md#rightstick)

### Methods

- [\_setButtonValue](GenericPad.md#_setbuttonvalue)
- [dispose](GenericPad.md#dispose)
- [onbuttondown](GenericPad.md#onbuttondown)
- [onbuttonup](GenericPad.md#onbuttonup)
- [onleftstickchanged](GenericPad.md#onleftstickchanged)
- [onrightstickchanged](GenericPad.md#onrightstickchanged)
- [update](GenericPad.md#update)

## Constructors

### constructor

• **new GenericPad**(`id`, `index`, `browserGamepad`)

Initializes the generic gamepad

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | The id of the generic gamepad |
| `index` | `number` | The index of the generic gamepad |
| `browserGamepad` | `any` | The browser gamepad |

#### Overrides

[Gamepad](Gamepad.md).[constructor](Gamepad.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:257

## Properties

### \_buttons

• `Private` **\_buttons**: `number`[]

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:223

___

### \_invertLeftStickY

• `Protected` **\_invertLeftStickY**: `boolean` = `false`

Specifies whether the left control stick should be Y-inverted

#### Inherited from

[Gamepad](Gamepad.md).[_invertLeftStickY](Gamepad.md#_invertleftsticky)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:100

___

### \_onbuttondown

• `Private` **\_onbuttondown**: (`buttonPressed`: `number`) => `void`

#### Type declaration

▸ (`buttonPressed`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `buttonPressed` | `number` |

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:224

___

### \_onbuttonup

• `Private` **\_onbuttonup**: (`buttonReleased`: `number`) => `void`

#### Type declaration

▸ (`buttonReleased`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `buttonReleased` | `number` |

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:225

___

### browserGamepad

• **browserGamepad**: `any`

#### Inherited from

[Gamepad](Gamepad.md).[browserGamepad](Gamepad.md#browsergamepad)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:131

___

### id

• **id**: `string`

#### Inherited from

[Gamepad](Gamepad.md).[id](Gamepad.md#id)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:123

___

### index

• **index**: `number`

#### Inherited from

[Gamepad](Gamepad.md).[index](Gamepad.md#index)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:127

___

### onButtonDownObservable

• **onButtonDownObservable**: [`Observable`](Observable.md)`number`

Observable triggered when a button has been pressed

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:230

___

### onButtonUpObservable

• **onButtonUpObservable**: [`Observable`](Observable.md)`number`

Observable triggered when a button has been released

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:234

___

### type

• **type**: `number`

Specifies what type of gamepad this represents

#### Inherited from

[Gamepad](Gamepad.md).[type](Gamepad.md#type)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:53

___

### DUALSHOCK

▪ `Static` **DUALSHOCK**: `number` = `4`

Represents an Dual Shock controller

#### Inherited from

[Gamepad](Gamepad.md).[DUALSHOCK](Gamepad.md#dualshock)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:95

___

### GAMEPAD

▪ `Static` **GAMEPAD**: `number` = `0`

Represents a gamepad controller

#### Inherited from

[Gamepad](Gamepad.md).[GAMEPAD](Gamepad.md#gamepad)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:79

___

### GENERIC

▪ `Static` **GENERIC**: `number` = `1`

Represents a generic controller

#### Inherited from

[Gamepad](Gamepad.md).[GENERIC](Gamepad.md#generic)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:83

___

### POSE\_ENABLED

▪ `Static` **POSE\_ENABLED**: `number` = `3`

Represents a pose-enabled controller

#### Inherited from

[Gamepad](Gamepad.md).[POSE_ENABLED](Gamepad.md#pose_enabled)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:91

___

### XBOX

▪ `Static` **XBOX**: `number` = `2`

Represents an XBox controller

#### Inherited from

[Gamepad](Gamepad.md).[XBOX](Gamepad.md#xbox)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:87

## Accessors

### isConnected

• `get` **isConnected**(): `boolean`

Specifies if the gamepad has been connected

#### Returns

`boolean`

#### Inherited from

Gamepad.isConnected

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:105

___

### leftStick

• `get` **leftStick**(): [`StickValues`](StickValues.md)

Gets the left joystick

#### Returns

[`StickValues`](StickValues.md)

#### Inherited from

Gamepad.leftStick

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:169

• `set` **leftStick**(`newValues`): `void`

Sets the left joystick values

#### Parameters

| Name | Type |
| :------ | :------ |
| `newValues` | [`StickValues`](StickValues.md) |

#### Returns

`void`

#### Inherited from

Gamepad.leftStick

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:175

___

### rightStick

• `get` **rightStick**(): [`StickValues`](StickValues.md)

Gets the right joystick

#### Returns

[`StickValues`](StickValues.md)

#### Inherited from

Gamepad.rightStick

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:184

• `set` **rightStick**(`newValues`): `void`

Sets the right joystick value

#### Parameters

| Name | Type |
| :------ | :------ |
| `newValues` | [`StickValues`](StickValues.md) |

#### Returns

`void`

#### Inherited from

Gamepad.rightStick

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:190

## Methods

### \_setButtonValue

▸ `Private` **_setButtonValue**(`newValue`, `currentValue`, `buttonIndex`): `number`

#### Parameters

| Name | Type |
| :------ | :------ |
| `newValue` | `number` |
| `currentValue` | `number` |
| `buttonIndex` | `number` |

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:263

___

### dispose

▸ **dispose**(): `void`

Disposes the generic gamepad

#### Returns

`void`

#### Overrides

[Gamepad](Gamepad.md).[dispose](Gamepad.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:296

___

### onbuttondown

▸ **onbuttondown**(`callback`): `void`

Callback triggered when a button has been pressed

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callback` | (`buttonPressed`: `number`) => `void` | Called when a button has been pressed |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:240

___

### onbuttonup

▸ **onbuttonup**(`callback`): `void`

Callback triggered when a button has been released

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callback` | (`buttonReleased`: `number`) => `void` | Called when a button has been released |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:247

___

### onleftstickchanged

▸ **onleftstickchanged**(`callback`): `void`

Callback triggered when the left joystick has changed

#### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | (`values`: [`StickValues`](StickValues.md)) => `void` |

#### Returns

`void`

#### Inherited from

[Gamepad](Gamepad.md).[onleftstickchanged](Gamepad.md#onleftstickchanged)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:154

___

### onrightstickchanged

▸ **onrightstickchanged**(`callback`): `void`

Callback triggered when the right joystick has changed

#### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | (`values`: [`StickValues`](StickValues.md)) => `void` |

#### Returns

`void`

#### Inherited from

[Gamepad](Gamepad.md).[onrightstickchanged](Gamepad.md#onrightstickchanged)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:162

___

### update

▸ **update**(): `void`

Updates the generic gamepad

#### Returns

`void`

#### Overrides

[Gamepad](Gamepad.md).[update](Gamepad.md#update)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:286
