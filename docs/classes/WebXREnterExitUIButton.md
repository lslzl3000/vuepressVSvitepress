[@dev/core](../README.md) / [Exports](../modules.md) / WebXREnterExitUIButton

# Class: WebXREnterExitUIButton

Button which can be used to enter a different mode of XR

## Table of contents

### Constructors

- [constructor](WebXREnterExitUIButton.md#constructor)

### Properties

- [element](WebXREnterExitUIButton.md#element)
- [referenceSpaceType](WebXREnterExitUIButton.md#referencespacetype)
- [sessionMode](WebXREnterExitUIButton.md#sessionmode)

### Methods

- [update](WebXREnterExitUIButton.md#update)

## Constructors

### constructor

• **new WebXREnterExitUIButton**(`element`, `sessionMode`, `referenceSpaceType`)

Creates a WebXREnterExitUIButton

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `element` | `HTMLElement` | button element |
| `sessionMode` | `XRSessionMode` | XR initialization session mode |
| `referenceSpaceType` | `XRReferenceSpaceType` | the type of reference space to be used |

#### Defined in

https://github.com/babylon.js/core/src/XR/webXREnterExitUI.ts:18

## Properties

### element

• **element**: `HTMLElement`

#### Defined in

https://github.com/babylon.js/core/src/XR/webXREnterExitUI.ts:20

___

### referenceSpaceType

• **referenceSpaceType**: `XRReferenceSpaceType`

#### Defined in

https://github.com/babylon.js/core/src/XR/webXREnterExitUI.ts:24

___

### sessionMode

• **sessionMode**: `XRSessionMode`

#### Defined in

https://github.com/babylon.js/core/src/XR/webXREnterExitUI.ts:22

## Methods

### update

▸ **update**(`activeButton`): `void`

Extendable function which can be used to update the button's visuals when the state changes

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `activeButton` | [`Nullable`](../modules.md#nullable)[`WebXREnterExitUIButton`](WebXREnterExitUIButton.md) | the current active button in the UI |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/XR/webXREnterExitUI.ts:32
