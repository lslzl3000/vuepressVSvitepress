[@dev/core](../README.md) / [Exports](../modules.md) / DeviceSource

# Class: DeviceSourceT

Class that handles all input for a specific device

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`DeviceType`](../enums/DeviceType.md) |

## Table of contents

### Constructors

- [constructor](DeviceSource.md#constructor)

### Properties

- [\_deviceInputSystem](DeviceSource.md#_deviceinputsystem)
- [deviceSlot](DeviceSource.md#deviceslot)
- [deviceType](DeviceSource.md#devicetype)
- [onInputChangedObservable](DeviceSource.md#oninputchangedobservable)

### Methods

- [getInput](DeviceSource.md#getinput)

## Constructors

### constructor

• **new DeviceSource**`T`(`deviceInputSystem`, `deviceType`, `deviceSlot?`)

Default Constructor

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`DeviceType`](../enums/DeviceType.md) |

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `deviceInputSystem` | `IDeviceInputSystem` | `undefined` | Reference to DeviceInputSystem |
| `deviceType` | `T` | `undefined` | Type of device |
| `deviceSlot` | `number` | `0` | "Slot" or index that device is referenced in |

#### Defined in

https://github.com/babylon.js/core/src/DeviceInput/InputDevices/deviceSource.ts:37

## Properties

### \_deviceInputSystem

• `Private` `Readonly` **\_deviceInputSystem**: `IDeviceInputSystem`

#### Defined in

https://github.com/babylon.js/core/src/DeviceInput/InputDevices/deviceSource.ts:29

___

### deviceSlot

• `Readonly` **deviceSlot**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/DeviceInput/InputDevices/deviceSource.ts:42

___

### deviceType

• `Readonly` **deviceType**: `T`

#### Defined in

https://github.com/babylon.js/core/src/DeviceInput/InputDevices/deviceSource.ts:40

___

### onInputChangedObservable

• `Readonly` **onInputChangedObservable**: [`Observable`](Observable.md)[`DeviceSourceEvent`](../modules.md#devicesourceevent)`T`

Observable to handle device input changes per device

#### Defined in

https://github.com/babylon.js/core/src/DeviceInput/InputDevices/deviceSource.ts:26

## Methods

### getInput

▸ **getInput**(`inputIndex`): `number`

Get input for specific input

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `inputIndex` | [`DeviceInput`](../modules.md#deviceinput)`T` | index of specific input on device |

#### Returns

`number`

Input value from DeviceInputSystem

#### Defined in

https://github.com/babylon.js/core/src/DeviceInput/InputDevices/deviceSource.ts:52
