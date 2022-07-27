[@dev/core](../README.md) / [Exports](../modules.md) / DualShockPad

# Class: DualShockPad

Defines a DualShock gamepad

## Hierarchy

- [`Gamepad`](Gamepad.md)

  ↳ **`DualShockPad`**

## Table of contents

### Constructors

- [constructor](DualShockPad.md#constructor)

### Properties

- [\_buttonCircle](DualShockPad.md#_buttoncircle)
- [\_buttonCross](DualShockPad.md#_buttoncross)
- [\_buttonL1](DualShockPad.md#_buttonl1)
- [\_buttonLeftStick](DualShockPad.md#_buttonleftstick)
- [\_buttonOptions](DualShockPad.md#_buttonoptions)
- [\_buttonR1](DualShockPad.md#_buttonr1)
- [\_buttonRightStick](DualShockPad.md#_buttonrightstick)
- [\_buttonShare](DualShockPad.md#_buttonshare)
- [\_buttonSquare](DualShockPad.md#_buttonsquare)
- [\_buttonTriangle](DualShockPad.md#_buttontriangle)
- [\_dPadDown](DualShockPad.md#_dpaddown)
- [\_dPadLeft](DualShockPad.md#_dpadleft)
- [\_dPadRight](DualShockPad.md#_dpadright)
- [\_dPadUp](DualShockPad.md#_dpadup)
- [\_invertLeftStickY](DualShockPad.md#_invertleftsticky)
- [\_leftTrigger](DualShockPad.md#_lefttrigger)
- [\_onbuttondown](DualShockPad.md#_onbuttondown)
- [\_onbuttonup](DualShockPad.md#_onbuttonup)
- [\_ondpaddown](DualShockPad.md#_ondpaddown)
- [\_ondpadup](DualShockPad.md#_ondpadup)
- [\_onlefttriggerchanged](DualShockPad.md#_onlefttriggerchanged)
- [\_onrighttriggerchanged](DualShockPad.md#_onrighttriggerchanged)
- [\_rightTrigger](DualShockPad.md#_righttrigger)
- [browserGamepad](DualShockPad.md#browsergamepad)
- [id](DualShockPad.md#id)
- [index](DualShockPad.md#index)
- [onButtonDownObservable](DualShockPad.md#onbuttondownobservable)
- [onButtonUpObservable](DualShockPad.md#onbuttonupobservable)
- [onPadDownObservable](DualShockPad.md#onpaddownobservable)
- [onPadUpObservable](DualShockPad.md#onpadupobservable)
- [type](DualShockPad.md#type)
- [DUALSHOCK](DualShockPad.md#dualshock)
- [GAMEPAD](DualShockPad.md#gamepad)
- [GENERIC](DualShockPad.md#generic)
- [POSE\_ENABLED](DualShockPad.md#pose_enabled)
- [XBOX](DualShockPad.md#xbox)

### Accessors

- [buttonCircle](DualShockPad.md#buttoncircle)
- [buttonCross](DualShockPad.md#buttoncross)
- [buttonL1](DualShockPad.md#buttonl1)
- [buttonLeftStick](DualShockPad.md#buttonleftstick)
- [buttonOptions](DualShockPad.md#buttonoptions)
- [buttonR1](DualShockPad.md#buttonr1)
- [buttonRightStick](DualShockPad.md#buttonrightstick)
- [buttonShare](DualShockPad.md#buttonshare)
- [buttonSquare](DualShockPad.md#buttonsquare)
- [buttonTriangle](DualShockPad.md#buttontriangle)
- [dPadDown](DualShockPad.md#dpaddown)
- [dPadLeft](DualShockPad.md#dpadleft)
- [dPadRight](DualShockPad.md#dpadright)
- [dPadUp](DualShockPad.md#dpadup)
- [isConnected](DualShockPad.md#isconnected)
- [leftStick](DualShockPad.md#leftstick)
- [leftTrigger](DualShockPad.md#lefttrigger)
- [rightStick](DualShockPad.md#rightstick)
- [rightTrigger](DualShockPad.md#righttrigger)

### Methods

- [\_setButtonValue](DualShockPad.md#_setbuttonvalue)
- [\_setDPadValue](DualShockPad.md#_setdpadvalue)
- [dispose](DualShockPad.md#dispose)
- [onbuttondown](DualShockPad.md#onbuttondown)
- [onbuttonup](DualShockPad.md#onbuttonup)
- [ondpaddown](DualShockPad.md#ondpaddown)
- [ondpadup](DualShockPad.md#ondpadup)
- [onleftstickchanged](DualShockPad.md#onleftstickchanged)
- [onlefttriggerchanged](DualShockPad.md#onlefttriggerchanged)
- [onrightstickchanged](DualShockPad.md#onrightstickchanged)
- [onrighttriggerchanged](DualShockPad.md#onrighttriggerchanged)
- [update](DualShockPad.md#update)

## Constructors

### constructor

• **new DualShockPad**(`id`, `index`, `gamepad`)

Creates a new DualShock gamepad object

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | defines the id of this gamepad |
| `index` | `number` | defines its index |
| `gamepad` | `any` | defines the internal HTML gamepad object |

#### Overrides

[Gamepad](Gamepad.md).[constructor](Gamepad.md#constructor)

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:88

## Properties

### \_buttonCircle

• `Private` **\_buttonCircle**: `number` = `0`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:67

___

### \_buttonCross

• `Private` **\_buttonCross**: `number` = `0`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:66

___

### \_buttonL1

• `Private` **\_buttonL1**: `number` = `0`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:72

___

### \_buttonLeftStick

• `Private` **\_buttonLeftStick**: `number` = `0`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:75

___

### \_buttonOptions

• `Private` **\_buttonOptions**: `number` = `0`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:71

___

### \_buttonR1

• `Private` **\_buttonR1**: `number` = `0`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:73

___

### \_buttonRightStick

• `Private` **\_buttonRightStick**: `number` = `0`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:76

___

### \_buttonShare

• `Private` **\_buttonShare**: `number` = `0`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:70

___

### \_buttonSquare

• `Private` **\_buttonSquare**: `number` = `0`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:68

___

### \_buttonTriangle

• `Private` **\_buttonTriangle**: `number` = `0`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:69

___

### \_dPadDown

• `Private` **\_dPadDown**: `number` = `0`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:78

___

### \_dPadLeft

• `Private` **\_dPadLeft**: `number` = `0`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:79

___

### \_dPadRight

• `Private` **\_dPadRight**: `number` = `0`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:80

___

### \_dPadUp

• `Private` **\_dPadUp**: `number` = `0`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:77

___

### \_invertLeftStickY

• `Protected` **\_invertLeftStickY**: `boolean` = `false`

Specifies whether the left control stick should be Y-inverted

#### Inherited from

[Gamepad](Gamepad.md).[_invertLeftStickY](Gamepad.md#_invertleftsticky)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:100

___

### \_leftTrigger

• `Private` **\_leftTrigger**: `number` = `0`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:46

___

### \_onbuttondown

• `Private` **\_onbuttondown**: (`buttonPressed`: [`DualShockButton`](../enums/DualShockButton.md)) => `void`

#### Type declaration

▸ (`buttonPressed`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `buttonPressed` | [`DualShockButton`](../enums/DualShockButton.md) |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:52

___

### \_onbuttonup

• `Private` **\_onbuttonup**: (`buttonReleased`: [`DualShockButton`](../enums/DualShockButton.md)) => `void`

#### Type declaration

▸ (`buttonReleased`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `buttonReleased` | [`DualShockButton`](../enums/DualShockButton.md) |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:53

___

### \_ondpaddown

• `Private` **\_ondpaddown**: (`dPadPressed`: [`DualShockDpad`](../enums/DualShockDpad.md)) => `void`

#### Type declaration

▸ (`dPadPressed`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `dPadPressed` | [`DualShockDpad`](../enums/DualShockDpad.md) |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:54

___

### \_ondpadup

• `Private` **\_ondpadup**: (`dPadReleased`: [`DualShockDpad`](../enums/DualShockDpad.md)) => `void`

#### Type declaration

▸ (`dPadReleased`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `dPadReleased` | [`DualShockDpad`](../enums/DualShockDpad.md) |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:55

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

packages/dev/core/src/Gamepads/dualShockGamepad.ts:49

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

packages/dev/core/src/Gamepads/dualShockGamepad.ts:50

___

### \_rightTrigger

• `Private` **\_rightTrigger**: `number` = `0`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:47

___

### browserGamepad

• **browserGamepad**: `any`

#### Inherited from

[Gamepad](Gamepad.md).[browserGamepad](Gamepad.md#browsergamepad)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:131

___

### id

• **id**: `string`

#### Inherited from

[Gamepad](Gamepad.md).[id](Gamepad.md#id)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:123

___

### index

• **index**: `number`

#### Inherited from

[Gamepad](Gamepad.md).[index](Gamepad.md#index)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:127

___

### onButtonDownObservable

• **onButtonDownObservable**: [`Observable`](Observable.md)[`DualShockButton`](../enums/DualShockButton.md)

Observable raised when a button is pressed

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:58

___

### onButtonUpObservable

• **onButtonUpObservable**: [`Observable`](Observable.md)[`DualShockButton`](../enums/DualShockButton.md)

Observable raised when a button is released

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:60

___

### onPadDownObservable

• **onPadDownObservable**: [`Observable`](Observable.md)[`DualShockDpad`](../enums/DualShockDpad.md)

Observable raised when a pad is pressed

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:62

___

### onPadUpObservable

• **onPadUpObservable**: [`Observable`](Observable.md)[`DualShockDpad`](../enums/DualShockDpad.md)

Observable raised when a pad is released

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:64

___

### type

• **type**: `number`

Specifies what type of gamepad this represents

#### Inherited from

[Gamepad](Gamepad.md).[type](Gamepad.md#type)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:53

___

### DUALSHOCK

▪ `Static` **DUALSHOCK**: `number` = `4`

Represents an Dual Shock controller

#### Inherited from

[Gamepad](Gamepad.md).[DUALSHOCK](Gamepad.md#dualshock)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:95

___

### GAMEPAD

▪ `Static` **GAMEPAD**: `number` = `0`

Represents a gamepad controller

#### Inherited from

[Gamepad](Gamepad.md).[GAMEPAD](Gamepad.md#gamepad)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:79

___

### GENERIC

▪ `Static` **GENERIC**: `number` = `1`

Represents a generic controller

#### Inherited from

[Gamepad](Gamepad.md).[GENERIC](Gamepad.md#generic)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:83

___

### POSE\_ENABLED

▪ `Static` **POSE\_ENABLED**: `number` = `3`

Represents a pose-enabled controller

#### Inherited from

[Gamepad](Gamepad.md).[POSE_ENABLED](Gamepad.md#pose_enabled)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:91

___

### XBOX

▪ `Static` **XBOX**: `number` = `2`

Represents an XBox controller

#### Inherited from

[Gamepad](Gamepad.md).[XBOX](Gamepad.md#xbox)

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:87

## Accessors

### buttonCircle

• `get` **buttonCircle**(): `number`

Gets the value of the `Circle` button

#### Returns

`number`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:229

• `set` **buttonCircle**(`value`): `void`

Sets the value of the `Circle` button

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:235

___

### buttonCross

• `get` **buttonCross**(): `number`

Gets the value of the `Cross` button

#### Returns

`number`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:216

• `set` **buttonCross**(`value`): `void`

Sets the value of the `Cross` button

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:222

___

### buttonL1

• `get` **buttonL1**(): `number`

Gets the value of the `L1` button

#### Returns

`number`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:294

• `set` **buttonL1**(`value`): `void`

Sets the value of the `L1` button

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:300

___

### buttonLeftStick

• `get` **buttonLeftStick**(): `number`

Gets the value of the Left joystick

#### Returns

`number`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:320

• `set` **buttonLeftStick**(`value`): `void`

Sets the value of the Left joystick

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:326

___

### buttonOptions

• `get` **buttonOptions**(): `number`

Gets the value of the `Options` button

#### Returns

`number`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:268

• `set` **buttonOptions**(`value`): `void`

Sets the value of the `Options` button

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:274

___

### buttonR1

• `get` **buttonR1**(): `number`

Gets the value of the `R1` button

#### Returns

`number`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:307

• `set` **buttonR1**(`value`): `void`

Sets the value of the `R1` button

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:313

___

### buttonRightStick

• `get` **buttonRightStick**(): `number`

Gets the value of the Right joystick

#### Returns

`number`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:333

• `set` **buttonRightStick**(`value`): `void`

Sets the value of the Right joystick

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:339

___

### buttonShare

• `get` **buttonShare**(): `number`

Gets the value of the `Share` button

#### Returns

`number`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:281

• `set` **buttonShare**(`value`): `void`

Sets the value of the `Share` button

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:287

___

### buttonSquare

• `get` **buttonSquare**(): `number`

Gets the value of the `Square` button

#### Returns

`number`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:242

• `set` **buttonSquare**(`value`): `void`

Sets the value of the `Square` button

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:248

___

### buttonTriangle

• `get` **buttonTriangle**(): `number`

Gets the value of the `Triangle` button

#### Returns

`number`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:255

• `set` **buttonTriangle**(`value`): `void`

Sets the value of the `Triangle` button

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:261

___

### dPadDown

• `get` **dPadDown**(): `number`

Gets the value of D-pad down

#### Returns

`number`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:359

• `set` **dPadDown**(`value`): `void`

Sets the value of D-pad down

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:365

___

### dPadLeft

• `get` **dPadLeft**(): `number`

Gets the value of D-pad left

#### Returns

`number`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:372

• `set` **dPadLeft**(`value`): `void`

Sets the value of D-pad left

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:378

___

### dPadRight

• `get` **dPadRight**(): `number`

Gets the value of D-pad right

#### Returns

`number`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:385

• `set` **dPadRight**(`value`): `void`

Sets the value of D-pad right

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:391

___

### dPadUp

• `get` **dPadUp**(): `number`

Gets the value of D-pad up

#### Returns

`number`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:346

• `set` **dPadUp**(`value`): `void`

Sets the value of D-pad up

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:352

___

### isConnected

• `get` **isConnected**(): `boolean`

Specifies if the gamepad has been connected

#### Returns

`boolean`

#### Inherited from

Gamepad.isConnected

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:105

___

### leftStick

• `get` **leftStick**(): [`StickValues`](StickValues.md)

Gets the left joystick

#### Returns

[`StickValues`](StickValues.md)

#### Inherited from

Gamepad.leftStick

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

#### Inherited from

Gamepad.leftStick

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:175

___

### leftTrigger

• `get` **leftTrigger**(): `number`

Gets the left trigger value

#### Returns

`number`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:112

• `set` **leftTrigger**(`newValue`): `void`

Sets the left trigger value

#### Parameters

| Name | Type |
| :------ | :------ |
| `newValue` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:118

___

### rightStick

• `get` **rightStick**(): [`StickValues`](StickValues.md)

Gets the right joystick

#### Returns

[`StickValues`](StickValues.md)

#### Inherited from

Gamepad.rightStick

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

#### Inherited from

Gamepad.rightStick

#### Defined in

packages/dev/core/src/Gamepads/gamepad.ts:190

___

### rightTrigger

• `get` **rightTrigger**(): `number`

Gets the right trigger value

#### Returns

`number`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:128

• `set` **rightTrigger**(`newValue`): `void`

Sets the right trigger value

#### Parameters

| Name | Type |
| :------ | :------ |
| `newValue` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:134

## Methods

### \_setButtonValue

▸ `Private` **_setButtonValue**(`newValue`, `currentValue`, `buttonType`): `number`

#### Parameters

| Name | Type |
| :------ | :------ |
| `newValue` | `number` |
| `currentValue` | `number` |
| `buttonType` | [`DualShockButton`](../enums/DualShockButton.md) |

#### Returns

`number`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:173

___

### \_setDPadValue

▸ `Private` **_setDPadValue**(`newValue`, `currentValue`, `buttonType`): `number`

#### Parameters

| Name | Type |
| :------ | :------ |
| `newValue` | `number` |
| `currentValue` | `number` |
| `buttonType` | [`DualShockDpad`](../enums/DualShockDpad.md) |

#### Returns

`number`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:193

___

### dispose

▸ **dispose**(): `void`

Disposes the gamepad

#### Returns

`void`

#### Overrides

[Gamepad](Gamepad.md).[dispose](Gamepad.md#dispose)

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:421

___

### onbuttondown

▸ **onbuttondown**(`callback`): `void`

Defines the callback to call when a button is pressed

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callback` | (`buttonPressed`: [`DualShockButton`](../enums/DualShockButton.md)) => `void` | defines the callback to use |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:145

___

### onbuttonup

▸ **onbuttonup**(`callback`): `void`

Defines the callback to call when a button is released

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callback` | (`buttonReleased`: [`DualShockButton`](../enums/DualShockButton.md)) => `void` | defines the callback to use |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:153

___

### ondpaddown

▸ **ondpaddown**(`callback`): `void`

Defines the callback to call when a pad is pressed

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callback` | (`dPadPressed`: [`DualShockDpad`](../enums/DualShockDpad.md)) => `void` | defines the callback to use |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:161

___

### ondpadup

▸ **ondpadup**(`callback`): `void`

Defines the callback to call when a pad is released

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callback` | (`dPadReleased`: [`DualShockDpad`](../enums/DualShockDpad.md)) => `void` | defines the callback to use |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:169

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

packages/dev/core/src/Gamepads/gamepad.ts:154

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

packages/dev/core/src/Gamepads/dualShockGamepad.ts:97

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

packages/dev/core/src/Gamepads/gamepad.ts:162

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

packages/dev/core/src/Gamepads/dualShockGamepad.ts:105

___

### update

▸ **update**(): `void`

Force the gamepad to synchronize with device values

#### Returns

`void`

#### Overrides

[Gamepad](Gamepad.md).[update](Gamepad.md#update)

#### Defined in

packages/dev/core/src/Gamepads/dualShockGamepad.ts:398
