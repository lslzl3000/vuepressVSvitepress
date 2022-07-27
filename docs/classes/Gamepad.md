[@dev/core](../README.md) / [Exports](../modules.md) / Gamepad

# Class: Gamepad

Represents a gamepad

## Hierarchy

- **`Gamepad`**

  ↳ [`PoseEnabledController`](PoseEnabledController.md)

  ↳ [`GenericPad`](GenericPad.md)

  ↳ [`Xbox360Pad`](Xbox360Pad.md)

  ↳ [`DualShockPad`](DualShockPad.md)

## Table of contents

### Constructors

- [constructor](Gamepad.md#constructor)

### Properties

- [\_invertLeftStickY](Gamepad.md#_invertleftsticky)
- [\_leftStick](Gamepad.md#_leftstick)
- [\_leftStickAxisX](Gamepad.md#_leftstickaxisx)
- [\_leftStickAxisY](Gamepad.md#_leftstickaxisy)
- [\_onleftstickchanged](Gamepad.md#_onleftstickchanged)
- [\_onrightstickchanged](Gamepad.md#_onrightstickchanged)
- [\_rightStick](Gamepad.md#_rightstick)
- [\_rightStickAxisX](Gamepad.md#_rightstickaxisx)
- [\_rightStickAxisY](Gamepad.md#_rightstickaxisy)
- [browserGamepad](Gamepad.md#browsergamepad)
- [id](Gamepad.md#id)
- [index](Gamepad.md#index)
- [type](Gamepad.md#type)
- [DUALSHOCK](Gamepad.md#dualshock)
- [GAMEPAD](Gamepad.md#gamepad)
- [GENERIC](Gamepad.md#generic)
- [POSE\_ENABLED](Gamepad.md#pose_enabled)
- [XBOX](Gamepad.md#xbox)

### Accessors

- [isConnected](Gamepad.md#isconnected)
- [leftStick](Gamepad.md#leftstick)
- [rightStick](Gamepad.md#rightstick)

### Methods

- [dispose](Gamepad.md#dispose)
- [onleftstickchanged](Gamepad.md#onleftstickchanged)
- [onrightstickchanged](Gamepad.md#onrightstickchanged)
- [update](Gamepad.md#update)

## Constructors

### constructor

• **new Gamepad**(`id`, `index`, `browserGamepad`, `leftStickX?`, `leftStickY?`, `rightStickX?`, `rightStickY?`)

Initializes the gamepad

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `id` | `string` | `undefined` | The id of the gamepad |
| `index` | `number` | `undefined` | The index of the gamepad |
| `browserGamepad` | `any` | `undefined` | The browser gamepad |
| `leftStickX` | `number` | `0` | The x component of the left joystick |
| `leftStickY` | `number` | `1` | The y component of the left joystick |
| `rightStickX` | `number` | `2` | The x component of the right joystick |
| `rightStickY` | `number` | `3` | The y component of the right joystick |

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:119

## Properties

### \_invertLeftStickY

• `Protected` **\_invertLeftStickY**: `boolean` = `false`

Specifies whether the left control stick should be Y-inverted

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:100

___

### \_leftStick

• `Private` **\_leftStick**: [`StickValues`](StickValues.md)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:55

___

### \_leftStickAxisX

• `Private` **\_leftStickAxisX**: `number`

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:61

___

### \_leftStickAxisY

• `Private` **\_leftStickAxisY**: `number`

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:62

___

### \_onleftstickchanged

• `Private` **\_onleftstickchanged**: (`values`: [`StickValues`](StickValues.md)) => `void`

#### Type declaration

▸ (`values`): `void`

Triggered when the left control stick has been changed

##### Parameters

| Name | Type |
| :------ | :------ |
| `values` | [`StickValues`](StickValues.md) |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:69

___

### \_onrightstickchanged

• `Private` **\_onrightstickchanged**: (`values`: [`StickValues`](StickValues.md)) => `void`

#### Type declaration

▸ (`values`): `void`

Triggered when the right control stick has been changed

##### Parameters

| Name | Type |
| :------ | :------ |
| `values` | [`StickValues`](StickValues.md) |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:74

___

### \_rightStick

• `Private` **\_rightStick**: [`StickValues`](StickValues.md)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:56

___

### \_rightStickAxisX

• `Private` **\_rightStickAxisX**: `number`

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:63

___

### \_rightStickAxisY

• `Private` **\_rightStickAxisY**: `number`

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:64

___

### browserGamepad

• **browserGamepad**: `any`

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:131

___

### id

• **id**: `string`

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:123

___

### index

• **index**: `number`

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:127

___

### type

• **type**: `number`

Specifies what type of gamepad this represents

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:53

___

### DUALSHOCK

▪ `Static` **DUALSHOCK**: `number` = `4`

Represents an Dual Shock controller

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:95

___

### GAMEPAD

▪ `Static` **GAMEPAD**: `number` = `0`

Represents a gamepad controller

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:79

___

### GENERIC

▪ `Static` **GENERIC**: `number` = `1`

Represents a generic controller

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:83

___

### POSE\_ENABLED

▪ `Static` **POSE\_ENABLED**: `number` = `3`

Represents a pose-enabled controller

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:91

___

### XBOX

▪ `Static` **XBOX**: `number` = `2`

Represents an XBox controller

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:87

## Accessors

### isConnected

• `get` **isConnected**(): `boolean`

Specifies if the gamepad has been connected

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:105

___

### leftStick

• `get` **leftStick**(): [`StickValues`](StickValues.md)

Gets the left joystick

#### Returns

[`StickValues`](StickValues.md)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:169

• `set` **leftStick**(`newValues`): `void`

Sets the left joystick values

#### Parameters

| Name | Type |
| :------ | :------ |
| `newValues` | [`StickValues`](StickValues.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:175

___

### rightStick

• `get` **rightStick**(): [`StickValues`](StickValues.md)

Gets the right joystick

#### Returns

[`StickValues`](StickValues.md)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:184

• `set` **rightStick**(`newValues`): `void`

Sets the right joystick value

#### Parameters

| Name | Type |
| :------ | :------ |
| `newValues` | [`StickValues`](StickValues.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:190

## Methods

### dispose

▸ **dispose**(): `void`

Disposes the gamepad

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:216

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

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:154

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

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:162

___

### update

▸ **update**(): `void`

Updates the gamepad joystick positions

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:201
