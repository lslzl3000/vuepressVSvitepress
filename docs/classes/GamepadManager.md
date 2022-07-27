[@dev/core](../README.md) / [Exports](../modules.md) / GamepadManager

# Class: GamepadManager

Manager for handling gamepads

## Table of contents

### Constructors

- [constructor](GamepadManager.md#constructor)

### Properties

- [\_babylonGamepads](GamepadManager.md#_babylongamepads)
- [\_gamepadEventSupported](GamepadManager.md#_gamepadeventsupported)
- [\_gamepadSupport](GamepadManager.md#_gamepadsupport)
- [\_loggedErrors](GamepadManager.md#_loggederrors)
- [\_onGamepadConnectedEvent](GamepadManager.md#_ongamepadconnectedevent)
- [\_onGamepadDisconnectedEvent](GamepadManager.md#_ongamepaddisconnectedevent)
- [\_oneGamepadConnected](GamepadManager.md#_onegamepadconnected)
- [onGamepadConnectedObservable](GamepadManager.md#ongamepadconnectedobservable)
- [onGamepadDisconnectedObservable](GamepadManager.md#ongamepaddisconnectedobservable)

### Accessors

- [gamepads](GamepadManager.md#gamepads)

### Methods

- [\_addNewGamepad](GamepadManager.md#_addnewgamepad)
- [\_startMonitoringGamepads](GamepadManager.md#_startmonitoringgamepads)
- [\_stopMonitoringGamepads](GamepadManager.md#_stopmonitoringgamepads)
- [\_updateGamepadObjects](GamepadManager.md#_updategamepadobjects)
- [dispose](GamepadManager.md#dispose)
- [getGamepadByType](GamepadManager.md#getgamepadbytype)

## Constructors

### constructor

• **new GamepadManager**(`_scene?`)

Initializes the gamepad manager

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `_scene?` | [`Scene`](Scene.md) | BabylonJS scene |

#### Defined in

packages/dev/core/src/Gamepads/gamepadManager.ts:40

## Properties

### \_babylonGamepads

• `Private` **\_babylonGamepads**: [`Gamepad`](Gamepad.md)[] = `[]`

#### Defined in

packages/dev/core/src/Gamepads/gamepadManager.ts:15

___

### \_gamepadEventSupported

• `Private` **\_gamepadEventSupported**: `boolean`

#### Defined in

packages/dev/core/src/Gamepads/gamepadManager.ts:20

___

### \_gamepadSupport

• `Private` `Optional` **\_gamepadSupport**: () => `any`[]

#### Type declaration

▸ (): `any`[]

##### Returns

`any`[]

#### Defined in

packages/dev/core/src/Gamepads/gamepadManager.ts:21

___

### \_loggedErrors

• `Private` **\_loggedErrors**: `number`[]

#### Defined in

packages/dev/core/src/Gamepads/gamepadManager.ts:209

___

### \_onGamepadConnectedEvent

• `Private` **\_onGamepadConnectedEvent**: [`Nullable`](../modules.md#nullable)(`evt`: `any`) => `void`

#### Defined in

packages/dev/core/src/Gamepads/gamepadManager.ts:33

___

### \_onGamepadDisconnectedEvent

• `Private` **\_onGamepadDisconnectedEvent**: [`Nullable`](../modules.md#nullable)(`evt`: `any`) => `void`

#### Defined in

packages/dev/core/src/Gamepads/gamepadManager.ts:34

___

### \_oneGamepadConnected

• `Private` **\_oneGamepadConnected**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Gamepads/gamepadManager.ts:16

___

### onGamepadConnectedObservable

• **onGamepadConnectedObservable**: [`Observable`](Observable.md)[`Gamepad`](Gamepad.md)

observable to be triggered when the gamepad controller has been connected

#### Defined in

packages/dev/core/src/Gamepads/gamepadManager.ts:26

___

### onGamepadDisconnectedObservable

• **onGamepadDisconnectedObservable**: [`Observable`](Observable.md)[`Gamepad`](Gamepad.md)

observable to be triggered when the gamepad controller has been disconnected

#### Defined in

packages/dev/core/src/Gamepads/gamepadManager.ts:31

## Accessors

### gamepads

• `get` **gamepads**(): [`Gamepad`](Gamepad.md)[]

The gamepads in the game pad manager

#### Returns

[`Gamepad`](Gamepad.md)[]

#### Defined in

packages/dev/core/src/Gamepads/gamepadManager.ts:119

## Methods

### \_addNewGamepad

▸ `Private` **_addNewGamepad**(`gamepad`): [`Gamepad`](Gamepad.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `gamepad` | `any` |

#### Returns

[`Gamepad`](Gamepad.md)

#### Defined in

packages/dev/core/src/Gamepads/gamepadManager.ts:166

___

### \_startMonitoringGamepads

▸ `Private` **_startMonitoringGamepads**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gamepads/gamepadManager.ts:195

___

### \_stopMonitoringGamepads

▸ `Private` **_stopMonitoringGamepads**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gamepads/gamepadManager.ts:205

___

### \_updateGamepadObjects

▸ `Private` **_updateGamepadObjects**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gamepads/gamepadManager.ts:240

___

### dispose

▸ **dispose**(): `void`

Disposes the gamepad manager

#### Returns

`void`

#### Defined in

packages/dev/core/src/Gamepads/gamepadManager.ts:141

___

### getGamepadByType

▸ **getGamepadByType**(`type?`): [`Nullable`](../modules.md#nullable)[`Gamepad`](Gamepad.md)

Get the gamepad controllers based on type

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `type` | `number` | `Gamepad.XBOX` | The type of gamepad controller |

#### Returns

[`Nullable`](../modules.md#nullable)[`Gamepad`](Gamepad.md)

Nullable gamepad

#### Defined in

packages/dev/core/src/Gamepads/gamepadManager.ts:128
