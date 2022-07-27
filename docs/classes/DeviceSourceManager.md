[@dev/core](../README.md) / [Exports](../modules.md) / DeviceSourceManager

# Class: DeviceSourceManager

Class to keep track of devices

## Implements

- [`IDisposable`](../interfaces/IDisposable.md)
- `IObservableManager`

## Table of contents

### Constructors

- [constructor](DeviceSourceManager.md#constructor)

### Properties

- [\_devices](DeviceSourceManager.md#_devices)
- [\_engine](DeviceSourceManager.md#_engine)
- [\_firstDevice](DeviceSourceManager.md#_firstdevice)
- [\_onDisposeObserver](DeviceSourceManager.md#_ondisposeobserver)
- [onDeviceConnectedObservable](DeviceSourceManager.md#ondeviceconnectedobservable)
- [onDeviceDisconnectedObservable](DeviceSourceManager.md#ondevicedisconnectedobservable)

### Methods

- [\_updateFirstDevices](DeviceSourceManager.md#_updatefirstdevices)
- [dispose](DeviceSourceManager.md#dispose)
- [getDeviceSource](DeviceSourceManager.md#getdevicesource)
- [getDeviceSources](DeviceSourceManager.md#getdevicesources)

## Constructors

### constructor

• **new DeviceSourceManager**(`engine`)

Default constructor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `engine` | [`Engine`](Engine.md) | Used to get canvas (if applicable) |

#### Defined in

packages/dev/core/src/DeviceInput/InputDevices/deviceSourceManager.ts:75

## Properties

### \_devices

• `Private` `Readonly` **\_devices**: [`DeviceSource`](DeviceSource.md)[`DeviceType`](../enums/DeviceType.md)[][]

#### Defined in

packages/dev/core/src/DeviceInput/InputDevices/deviceSourceManager.ts:31

___

### \_engine

• `Private` **\_engine**: [`Engine`](Engine.md)

#### Defined in

packages/dev/core/src/DeviceInput/InputDevices/deviceSourceManager.ts:29

___

### \_firstDevice

• `Private` `Readonly` **\_firstDevice**: `number`[]

#### Defined in

packages/dev/core/src/DeviceInput/InputDevices/deviceSourceManager.ts:32

___

### \_onDisposeObserver

• `Private` **\_onDisposeObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`ThinEngine`](ThinEngine.md)

#### Defined in

packages/dev/core/src/DeviceInput/InputDevices/deviceSourceManager.ts:30

___

### onDeviceConnectedObservable

• `Readonly` **onDeviceConnectedObservable**: [`Observable`](Observable.md)`DeviceSourceType`

Observable to be triggered when after a device is connected, any new observers added will be triggered against already connected devices

#### Implementation of

IObservableManager.onDeviceConnectedObservable

#### Defined in

packages/dev/core/src/DeviceInput/InputDevices/deviceSourceManager.ts:21

___

### onDeviceDisconnectedObservable

• `Readonly` **onDeviceDisconnectedObservable**: [`Observable`](Observable.md)`DeviceSourceType`

Observable to be triggered when after a device is disconnected

#### Implementation of

IObservableManager.onDeviceDisconnectedObservable

#### Defined in

packages/dev/core/src/DeviceInput/InputDevices/deviceSourceManager.ts:26

## Methods

### \_updateFirstDevices

▸ `Private` **_updateFirstDevices**(`type`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `type` | [`DeviceType`](../enums/DeviceType.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/DeviceInput/InputDevices/deviceSourceManager.ts:169

___

### dispose

▸ **dispose**(): `void`

Dispose of DeviceSourceManager

#### Returns

`void`

#### Implementation of

[IDisposable](../interfaces/IDisposable.md).[dispose](../interfaces/IDisposable.md#dispose)

#### Defined in

packages/dev/core/src/DeviceInput/InputDevices/deviceSourceManager.ts:110

___

### getDeviceSource

▸ **getDeviceSource**`T`(`deviceType`, `deviceSlot?`): [`Nullable`](../modules.md#nullable)[`DeviceSource`](DeviceSource.md)`T`

Gets a DeviceSource, given a type and slot

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`DeviceType`](../enums/DeviceType.md) |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `deviceType` | `T` | Type of Device |
| `deviceSlot?` | `number` | Slot or ID of device |

#### Returns

[`Nullable`](../modules.md#nullable)[`DeviceSource`](DeviceSource.md)`T`

DeviceSource

#### Defined in

packages/dev/core/src/DeviceInput/InputDevices/deviceSourceManager.ts:41

___

### getDeviceSources

▸ **getDeviceSources**`T`(`deviceType`): readonly [`DeviceSource`](DeviceSource.md)`T`[]

Gets an array of DeviceSource objects for a given device type

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`DeviceType`](../enums/DeviceType.md) |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `deviceType` | `T` | Type of Device |

#### Returns

readonly [`DeviceSource`](DeviceSource.md)`T`[]

All available DeviceSources of a given type

#### Defined in

packages/dev/core/src/DeviceInput/InputDevices/deviceSourceManager.ts:61
