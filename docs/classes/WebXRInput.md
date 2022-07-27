[@dev/core](../README.md) / [Exports](../modules.md) / WebXRInput

# Class: WebXRInput

XR input used to track XR inputs such as controllers/rays

## Implements

- [`IDisposable`](../interfaces/IDisposable.md)

## Table of contents

### Constructors

- [constructor](WebXRInput.md#constructor)

### Properties

- [\_frameObserver](WebXRInput.md#_frameobserver)
- [\_sessionEndedObserver](WebXRInput.md#_sessionendedobserver)
- [\_sessionInitObserver](WebXRInput.md#_sessioninitobserver)
- [controllers](WebXRInput.md#controllers)
- [onControllerAddedObservable](WebXRInput.md#oncontrolleraddedobservable)
- [onControllerRemovedObservable](WebXRInput.md#oncontrollerremovedobservable)
- [xrCamera](WebXRInput.md#xrcamera)
- [xrSessionManager](WebXRInput.md#xrsessionmanager)

### Methods

- [\_addAndRemoveControllers](WebXRInput.md#_addandremovecontrollers)
- [\_onInputSourcesChange](WebXRInput.md#_oninputsourceschange)
- [dispose](WebXRInput.md#dispose)

## Constructors

### constructor

• **new WebXRInput**(`xrSessionManager`, `xrCamera`, `_options?`)

Initializes the WebXRInput

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `xrSessionManager` | [`WebXRSessionManager`](WebXRSessionManager.md) | the xr session manager for this session |
| `xrCamera` | [`WebXRCamera`](WebXRCamera.md) | the WebXR camera for this session. Mainly used for teleportation |
| `_options` | [`IWebXRInputOptions`](../interfaces/IWebXRInputOptions.md) | = initialization options for this xr input |

#### Defined in

packages/dev/core/src/XR/webXRInput.ts:75

## Properties

### \_frameObserver

• `Private` **\_frameObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)`any`

#### Defined in

packages/dev/core/src/XR/webXRInput.ts:57

___

### \_sessionEndedObserver

• `Private` **\_sessionEndedObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)`any`

#### Defined in

packages/dev/core/src/XR/webXRInput.ts:58

___

### \_sessionInitObserver

• `Private` **\_sessionInitObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)`any`

#### Defined in

packages/dev/core/src/XR/webXRInput.ts:59

___

### controllers

• **controllers**: [`WebXRInputSource`](WebXRInputSource.md)[] = `[]`

XR controllers being tracked

#### Defined in

packages/dev/core/src/XR/webXRInput.ts:56

___

### onControllerAddedObservable

• **onControllerAddedObservable**: [`Observable`](Observable.md)[`WebXRInputSource`](WebXRInputSource.md)

Event when a controller has been connected/added

#### Defined in

packages/dev/core/src/XR/webXRInput.ts:63

___

### onControllerRemovedObservable

• **onControllerRemovedObservable**: [`Observable`](Observable.md)[`WebXRInputSource`](WebXRInputSource.md)

Event when a controller has been removed/disconnected

#### Defined in

packages/dev/core/src/XR/webXRInput.ts:67

___

### xrCamera

• **xrCamera**: [`WebXRCamera`](WebXRCamera.md)

#### Defined in

packages/dev/core/src/XR/webXRInput.ts:83

___

### xrSessionManager

• **xrSessionManager**: [`WebXRSessionManager`](WebXRSessionManager.md)

#### Defined in

packages/dev/core/src/XR/webXRInput.ts:79

## Methods

### \_addAndRemoveControllers

▸ `Private` **_addAndRemoveControllers**(`addInputs`, `removeInputs`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `addInputs` | `XRInputSource`[] |
| `removeInputs` | `XRInputSource`[] |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/webXRInput.ts:128

___

### \_onInputSourcesChange

▸ `Private` **_onInputSourcesChange**(`event`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | `XRInputSourceChangeEvent` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/webXRInput.ts:124

___

### dispose

▸ **dispose**(): `void`

Disposes of the object

#### Returns

`void`

#### Implementation of

[IDisposable](../interfaces/IDisposable.md).[dispose](../interfaces/IDisposable.md#dispose)

#### Defined in

packages/dev/core/src/XR/webXRInput.ts:166
