[@dev/core](../README.md) / [Exports](../modules.md) / WebXREnterExitUI

# Class: WebXREnterExitUI

UI to allow the user to enter/exit XR mode

## Implements

- [`IDisposable`](../interfaces/IDisposable.md)

## Table of contents

### Constructors

- [constructor](WebXREnterExitUI.md#constructor)

### Properties

- [\_activeButton](WebXREnterExitUI.md#_activebutton)
- [\_buttons](WebXREnterExitUI.md#_buttons)
- [\_helper](WebXREnterExitUI.md#_helper)
- [\_renderTarget](WebXREnterExitUI.md#_rendertarget)
- [activeButtonChangedObservable](WebXREnterExitUI.md#activebuttonchangedobservable)
- [options](WebXREnterExitUI.md#options)
- [overlay](WebXREnterExitUI.md#overlay)

### Methods

- [\_enterXRWithButtonIndex](WebXREnterExitUI.md#_enterxrwithbuttonindex)
- [\_onSessionGranted](WebXREnterExitUI.md#_onsessiongranted)
- [\_updateButtons](WebXREnterExitUI.md#_updatebuttons)
- [dispose](WebXREnterExitUI.md#dispose)
- [setHelperAsync](WebXREnterExitUI.md#sethelperasync)
- [CreateAsync](WebXREnterExitUI.md#createasync)

## Constructors

### constructor

• **new WebXREnterExitUI**(`_scene`, `options`)

Construct a new EnterExit UI class

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `_scene` | [`Scene`](Scene.md) | babylon scene object to use |
| `options` | [`WebXREnterExitUIOptions`](WebXREnterExitUIOptions.md) | (read-only) version of the options passed to this UI |

#### Defined in

packages/dev/core/src/XR/webXREnterExitUI.ts:108

## Properties

### \_activeButton

• `Private` **\_activeButton**: [`Nullable`](../modules.md#nullable)[`WebXREnterExitUIButton`](WebXREnterExitUIButton.md) = `null`

#### Defined in

packages/dev/core/src/XR/webXREnterExitUI.ts:84

___

### \_buttons

• `Private` **\_buttons**: [`WebXREnterExitUIButton`](WebXREnterExitUIButton.md)[] = `[]`

#### Defined in

packages/dev/core/src/XR/webXREnterExitUI.ts:85

___

### \_helper

• `Private` **\_helper**: [`WebXRExperienceHelper`](WebXRExperienceHelper.md)

#### Defined in

packages/dev/core/src/XR/webXREnterExitUI.ts:86

___

### \_renderTarget

• `Private` `Optional` **\_renderTarget**: [`WebXRRenderTarget`](../interfaces/WebXRRenderTarget.md)

#### Defined in

packages/dev/core/src/XR/webXREnterExitUI.ts:87

___

### activeButtonChangedObservable

• **activeButtonChangedObservable**: [`Observable`](Observable.md)[`Nullable`](../modules.md#nullable)[`WebXREnterExitUIButton`](WebXREnterExitUIButton.md)

Fired every time the active button is changed.

When xr is entered via a button that launches xr that button will be the callback parameter

When exiting xr the callback parameter will be null)

#### Defined in

packages/dev/core/src/XR/webXREnterExitUI.ts:100

___

### options

• **options**: [`WebXREnterExitUIOptions`](WebXREnterExitUIOptions.md)

#### Defined in

packages/dev/core/src/XR/webXREnterExitUI.ts:111

___

### overlay

• `Readonly` **overlay**: `HTMLDivElement`

The HTML Div Element to which buttons are added.

#### Defined in

packages/dev/core/src/XR/webXREnterExitUI.ts:91

## Methods

### \_enterXRWithButtonIndex

▸ `Private` **_enterXRWithButtonIndex**(`idx?`): `Promise``void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `idx` | `number` | `0` |

#### Returns

`Promise``void`

#### Defined in

packages/dev/core/src/XR/webXREnterExitUI.ts:212

___

### \_onSessionGranted

▸ `Private` **_onSessionGranted**(`evt`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `evt` | `Object` |
| `evt.session` | `XRSession` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/webXREnterExitUI.ts:250

___

### \_updateButtons

▸ `Private` **_updateButtons**(`activeButton`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `activeButton` | [`Nullable`](../modules.md#nullable)[`WebXREnterExitUIButton`](WebXREnterExitUIButton.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/webXREnterExitUI.ts:271

___

### dispose

▸ **dispose**(): `void`

Disposes of the XR UI component

#### Returns

`void`

#### Implementation of

[IDisposable](../interfaces/IDisposable.md).[dispose](../interfaces/IDisposable.md#dispose)

#### Defined in

packages/dev/core/src/XR/webXREnterExitUI.ts:240

___

### setHelperAsync

▸ **setHelperAsync**(`helper`, `renderTarget?`): `Promise``void`

Set the helper to be used with this UI component.
The UI is bound to an experience helper. If not provided the UI can still be used but the events should be registered by the developer.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `helper` | [`WebXRExperienceHelper`](WebXRExperienceHelper.md) | the experience helper to attach |
| `renderTarget?` | [`WebXRRenderTarget`](../interfaces/WebXRRenderTarget.md) | an optional render target (in case it is created outside of the helper scope) |

#### Returns

`Promise``void`

a promise that resolves when the ui is ready

#### Defined in

packages/dev/core/src/XR/webXREnterExitUI.ts:177

___

### CreateAsync

▸ `Static` **CreateAsync**(`scene`, `helper`, `options`): `Promise`[`WebXREnterExitUI`](WebXREnterExitUI.md)

Creates UI to allow the user to enter/exit XR mode

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | the scene to add the ui to |
| `helper` | [`WebXRExperienceHelper`](WebXRExperienceHelper.md) | the xr experience helper to enter/exit xr with |
| `options` | [`WebXREnterExitUIOptions`](WebXREnterExitUIOptions.md) | options to configure the UI |

#### Returns

`Promise`[`WebXREnterExitUI`](WebXREnterExitUI.md)

the created ui

#### Defined in

packages/dev/core/src/XR/webXREnterExitUI.ts:206
