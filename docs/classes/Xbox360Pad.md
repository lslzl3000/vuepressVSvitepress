[@dev/core](../README.md) / [Exports](../modules.md) / Xbox360Pad

# Class: Xbox360Pad

Defines a XBox360 gamepad

## Hierarchy

- [`Gamepad`](Gamepad.md)

  ↳ **`Xbox360Pad`**

## Table of contents

### Constructors

- [constructor](Xbox360Pad.md#constructor)

### Properties

- [\_buttonA](Xbox360Pad.md#_buttona)
- [\_buttonB](Xbox360Pad.md#_buttonb)
- [\_buttonBack](Xbox360Pad.md#_buttonback)
- [\_buttonLB](Xbox360Pad.md#_buttonlb)
- [\_buttonLeftStick](Xbox360Pad.md#_buttonleftstick)
- [\_buttonRB](Xbox360Pad.md#_buttonrb)
- [\_buttonRightStick](Xbox360Pad.md#_buttonrightstick)
- [\_buttonStart](Xbox360Pad.md#_buttonstart)
- [\_buttonX](Xbox360Pad.md#_buttonx)
- [\_buttonY](Xbox360Pad.md#_buttony)
- [\_dPadDown](Xbox360Pad.md#_dpaddown)
- [\_dPadLeft](Xbox360Pad.md#_dpadleft)
- [\_dPadRight](Xbox360Pad.md#_dpadright)
- [\_dPadUp](Xbox360Pad.md#_dpadup)
- [\_invertLeftStickY](Xbox360Pad.md#_invertleftsticky)
- [\_isXboxOnePad](Xbox360Pad.md#_isxboxonepad)
- [\_leftTrigger](Xbox360Pad.md#_lefttrigger)
- [\_onbuttondown](Xbox360Pad.md#_onbuttondown)
- [\_onbuttonup](Xbox360Pad.md#_onbuttonup)
- [\_ondpaddown](Xbox360Pad.md#_ondpaddown)
- [\_ondpadup](Xbox360Pad.md#_ondpadup)
- [\_onlefttriggerchanged](Xbox360Pad.md#_onlefttriggerchanged)
- [\_onrighttriggerchanged](Xbox360Pad.md#_onrighttriggerchanged)
- [\_rightTrigger](Xbox360Pad.md#_righttrigger)
- [browserGamepad](Xbox360Pad.md#browsergamepad)
- [id](Xbox360Pad.md#id)
- [index](Xbox360Pad.md#index)
- [onButtonDownObservable](Xbox360Pad.md#onbuttondownobservable)
- [onButtonUpObservable](Xbox360Pad.md#onbuttonupobservable)
- [onPadDownObservable](Xbox360Pad.md#onpaddownobservable)
- [onPadUpObservable](Xbox360Pad.md#onpadupobservable)
- [type](Xbox360Pad.md#type)
- [DUALSHOCK](Xbox360Pad.md#dualshock)
- [GAMEPAD](Xbox360Pad.md#gamepad)
- [GENERIC](Xbox360Pad.md#generic)
- [POSE\_ENABLED](Xbox360Pad.md#pose_enabled)
- [XBOX](Xbox360Pad.md#xbox)

### Accessors

- [buttonA](Xbox360Pad.md#buttona)
- [buttonB](Xbox360Pad.md#buttonb)
- [buttonBack](Xbox360Pad.md#buttonback)
- [buttonLB](Xbox360Pad.md#buttonlb)
- [buttonLeftStick](Xbox360Pad.md#buttonleftstick)
- [buttonRB](Xbox360Pad.md#buttonrb)
- [buttonRightStick](Xbox360Pad.md#buttonrightstick)
- [buttonStart](Xbox360Pad.md#buttonstart)
- [buttonX](Xbox360Pad.md#buttonx)
- [buttonY](Xbox360Pad.md#buttony)
- [dPadDown](Xbox360Pad.md#dpaddown)
- [dPadLeft](Xbox360Pad.md#dpadleft)
- [dPadRight](Xbox360Pad.md#dpadright)
- [dPadUp](Xbox360Pad.md#dpadup)
- [isConnected](Xbox360Pad.md#isconnected)
- [leftStick](Xbox360Pad.md#leftstick)
- [leftTrigger](Xbox360Pad.md#lefttrigger)
- [rightStick](Xbox360Pad.md#rightstick)
- [rightTrigger](Xbox360Pad.md#righttrigger)

### Methods

- [\_setButtonValue](Xbox360Pad.md#_setbuttonvalue)
- [\_setDPadValue](Xbox360Pad.md#_setdpadvalue)
- [dispose](Xbox360Pad.md#dispose)
- [onbuttondown](Xbox360Pad.md#onbuttondown)
- [onbuttonup](Xbox360Pad.md#onbuttonup)
- [ondpaddown](Xbox360Pad.md#ondpaddown)
- [ondpadup](Xbox360Pad.md#ondpadup)
- [onleftstickchanged](Xbox360Pad.md#onleftstickchanged)
- [onlefttriggerchanged](Xbox360Pad.md#onlefttriggerchanged)
- [onrightstickchanged](Xbox360Pad.md#onrightstickchanged)
- [onrighttriggerchanged](Xbox360Pad.md#onrighttriggerchanged)
- [update](Xbox360Pad.md#update)

## Constructors

### constructor

• **new Xbox360Pad**(`id`, `index`, `gamepad`, `xboxOne?`)

Creates a new XBox360 gamepad object

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `id` | `string` | `undefined` | defines the id of this gamepad |
| `index` | `number` | `undefined` | defines its index |
| `gamepad` | `any` | `undefined` | defines the internal HTML gamepad object |
| `xboxOne` | `boolean` | `false` | defines if it is a XBox One gamepad |

#### Overrides

[Gamepad](Gamepad.md).[constructor](Gamepad.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:90

## Properties

### \_buttonA

• `Private` **\_buttonA**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:65

___

### \_buttonB

• `Private` **\_buttonB**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:66

___

### \_buttonBack

• `Private` **\_buttonBack**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:69

___

### \_buttonLB

• `Private` **\_buttonLB**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:71

___

### \_buttonLeftStick

• `Private` **\_buttonLeftStick**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:74

___

### \_buttonRB

• `Private` **\_buttonRB**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:72

___

### \_buttonRightStick

• `Private` **\_buttonRightStick**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:75

___

### \_buttonStart

• `Private` **\_buttonStart**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:70

___

### \_buttonX

• `Private` **\_buttonX**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:67

___

### \_buttonY

• `Private` **\_buttonY**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:68

___

### \_dPadDown

• `Private` **\_dPadDown**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:77

___

### \_dPadLeft

• `Private` **\_dPadLeft**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:78

___

### \_dPadRight

• `Private` **\_dPadRight**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:79

___

### \_dPadUp

• `Private` **\_dPadUp**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:76

___

### \_invertLeftStickY

• `Protected` **\_invertLeftStickY**: `boolean` = `false`

Specifies whether the left control stick should be Y-inverted

#### Inherited from

[Gamepad](Gamepad.md).[_invertLeftStickY](Gamepad.md#_invertleftsticky)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepad.ts:100

___

### \_isXboxOnePad

• `Private` **\_isXboxOnePad**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:81

___

### \_leftTrigger

• `Private` **\_leftTrigger**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:45

___

### \_onbuttondown

• `Private` **\_onbuttondown**: (`buttonPressed`: [`Xbox360Button`](../enums/Xbox360Button.md)) => `void`

#### Type declaration

▸ (`buttonPressed`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `buttonPressed` | [`Xbox360Button`](../enums/Xbox360Button.md) |

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:51

___

### \_onbuttonup

• `Private` **\_onbuttonup**: (`buttonReleased`: [`Xbox360Button`](../enums/Xbox360Button.md)) => `void`

#### Type declaration

▸ (`buttonReleased`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `buttonReleased` | [`Xbox360Button`](../enums/Xbox360Button.md) |

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:52

___

### \_ondpaddown

• `Private` **\_ondpaddown**: (`dPadPressed`: [`Xbox360Dpad`](../enums/Xbox360Dpad.md)) => `void`

#### Type declaration

▸ (`dPadPressed`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `dPadPressed` | [`Xbox360Dpad`](../enums/Xbox360Dpad.md) |

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:53

___

### \_ondpadup

• `Private` **\_ondpadup**: (`dPadReleased`: [`Xbox360Dpad`](../enums/Xbox360Dpad.md)) => `void`

#### Type declaration

▸ (`dPadReleased`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `dPadReleased` | [`Xbox360Dpad`](../enums/Xbox360Dpad.md) |

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:54

___

### \_onlefttriggerchanged

• `Private` **\_onlefttriggerchanged**: (`value`: `number`) => `void`

#### Type declaration

▸ (`value`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:48

___

### \_onrighttriggerchanged

• `Private` **\_onrighttriggerchanged**: (`value`: `number`) => `void`

#### Type declaration

▸ (`value`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:49

___

### \_rightTrigger

• `Private` **\_rightTrigger**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:46

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

• **onButtonDownObservable**: [`Observable`](Observable.md)[`Xbox360Button`](../enums/Xbox360Button.md)

Observable raised when a button is pressed

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:57

___

### onButtonUpObservable

• **onButtonUpObservable**: [`Observable`](Observable.md)[`Xbox360Button`](../enums/Xbox360Button.md)

Observable raised when a button is released

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:59

___

### onPadDownObservable

• **onPadDownObservable**: [`Observable`](Observable.md)[`Xbox360Dpad`](../enums/Xbox360Dpad.md)

Observable raised when a pad is pressed

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:61

___

### onPadUpObservable

• **onPadUpObservable**: [`Observable`](Observable.md)[`Xbox360Dpad`](../enums/Xbox360Dpad.md)

Observable raised when a pad is released

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:63

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

### buttonA

• `get` **buttonA**(): `number`

Gets the value of the `A` button

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:219

• `set` **buttonA**(`value`): `void`

Sets the value of the `A` button

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:225

___

### buttonB

• `get` **buttonB**(): `number`

Gets the value of the `B` button

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:232

• `set` **buttonB**(`value`): `void`

Sets the value of the `B` button

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:238

___

### buttonBack

• `get` **buttonBack**(): `number`

Gets the value of the `Back` button

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:284

• `set` **buttonBack**(`value`): `void`

Sets the value of the `Back` button

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:290

___

### buttonLB

• `get` **buttonLB**(): `number`

Gets the value of the `Left` button

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:297

• `set` **buttonLB**(`value`): `void`

Sets the value of the `Left` button

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:303

___

### buttonLeftStick

• `get` **buttonLeftStick**(): `number`

Gets the value of the Left joystick

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:323

• `set` **buttonLeftStick**(`value`): `void`

Sets the value of the Left joystick

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:329

___

### buttonRB

• `get` **buttonRB**(): `number`

Gets the value of the `Right` button

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:310

• `set` **buttonRB**(`value`): `void`

Sets the value of the `Right` button

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:316

___

### buttonRightStick

• `get` **buttonRightStick**(): `number`

Gets the value of the Right joystick

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:336

• `set` **buttonRightStick**(`value`): `void`

Sets the value of the Right joystick

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:342

___

### buttonStart

• `get` **buttonStart**(): `number`

Gets the value of the `Start` button

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:271

• `set` **buttonStart**(`value`): `void`

Sets the value of the `Start` button

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:277

___

### buttonX

• `get` **buttonX**(): `number`

Gets the value of the `X` button

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:245

• `set` **buttonX**(`value`): `void`

Sets the value of the `X` button

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:251

___

### buttonY

• `get` **buttonY**(): `number`

Gets the value of the `Y` button

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:258

• `set` **buttonY**(`value`): `void`

Sets the value of the `Y` button

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:264

___

### dPadDown

• `get` **dPadDown**(): `number`

Gets the value of D-pad down

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:362

• `set` **dPadDown**(`value`): `void`

Sets the value of D-pad down

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:368

___

### dPadLeft

• `get` **dPadLeft**(): `number`

Gets the value of D-pad left

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:375

• `set` **dPadLeft**(`value`): `void`

Sets the value of D-pad left

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:381

___

### dPadRight

• `get` **dPadRight**(): `number`

Gets the value of D-pad right

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:388

• `set` **dPadRight**(`value`): `void`

Sets the value of D-pad right

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:394

___

### dPadUp

• `get` **dPadUp**(): `number`

Gets the value of D-pad up

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:349

• `set` **dPadUp**(`value`): `void`

Sets the value of D-pad up

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:355

___

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

### leftTrigger

• `get` **leftTrigger**(): `number`

Gets the left trigger value

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:115

• `set` **leftTrigger**(`newValue`): `void`

Sets the left trigger value

#### Parameters

| Name | Type |
| :------ | :------ |
| `newValue` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:121

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

___

### rightTrigger

• `get` **rightTrigger**(): `number`

Gets the right trigger value

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:131

• `set` **rightTrigger**(`newValue`): `void`

Sets the right trigger value

#### Parameters

| Name | Type |
| :------ | :------ |
| `newValue` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:137

## Methods

### \_setButtonValue

▸ `Private` **_setButtonValue**(`newValue`, `currentValue`, `buttonType`): `number`

#### Parameters

| Name | Type |
| :------ | :------ |
| `newValue` | `number` |
| `currentValue` | `number` |
| `buttonType` | [`Xbox360Button`](../enums/Xbox360Button.md) |

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:176

___

### \_setDPadValue

▸ `Private` **_setDPadValue**(`newValue`, `currentValue`, `buttonType`): `number`

#### Parameters

| Name | Type |
| :------ | :------ |
| `newValue` | `number` |
| `currentValue` | `number` |
| `buttonType` | [`Xbox360Dpad`](../enums/Xbox360Dpad.md) |

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:196

___

### dispose

▸ **dispose**(): `void`

Disposes the gamepad

#### Returns

`void`

#### Overrides

[Gamepad](Gamepad.md).[dispose](Gamepad.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:443

___

### onbuttondown

▸ **onbuttondown**(`callback`): `void`

Defines the callback to call when a button is pressed

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callback` | (`buttonPressed`: [`Xbox360Button`](../enums/Xbox360Button.md)) => `void` | defines the callback to use |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:148

___

### onbuttonup

▸ **onbuttonup**(`callback`): `void`

Defines the callback to call when a button is released

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callback` | (`buttonReleased`: [`Xbox360Button`](../enums/Xbox360Button.md)) => `void` | defines the callback to use |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:156

___

### ondpaddown

▸ **ondpaddown**(`callback`): `void`

Defines the callback to call when a pad is pressed

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callback` | (`dPadPressed`: [`Xbox360Dpad`](../enums/Xbox360Dpad.md)) => `void` | defines the callback to use |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:164

___

### ondpadup

▸ **ondpadup**(`callback`): `void`

Defines the callback to call when a pad is released

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callback` | (`dPadReleased`: [`Xbox360Dpad`](../enums/Xbox360Dpad.md)) => `void` | defines the callback to use |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:172

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

### onlefttriggerchanged

▸ **onlefttriggerchanged**(`callback`): `void`

Defines the callback to call when left trigger is pressed

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callback` | (`value`: `number`) => `void` | defines the callback to use |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:100

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

### onrighttriggerchanged

▸ **onrighttriggerchanged**(`callback`): `void`

Defines the callback to call when right trigger is pressed

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callback` | (`value`: `number`) => `void` | defines the callback to use |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:108

___

### update

▸ **update**(): `void`

Force the gamepad to synchronize with device values

#### Returns

`void`

#### Overrides

[Gamepad](Gamepad.md).[update](Gamepad.md#update)

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/xboxGamepad.ts:401
