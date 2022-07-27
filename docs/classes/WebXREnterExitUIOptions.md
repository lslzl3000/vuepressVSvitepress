[@dev/core](../README.md) / [Exports](../modules.md) / WebXREnterExitUIOptions

# Class: WebXREnterExitUIOptions

Options to create the webXR UI

## Table of contents

### Constructors

- [constructor](WebXREnterExitUIOptions.md#constructor)

### Properties

- [customButtons](WebXREnterExitUIOptions.md#custombuttons)
- [ignoreSessionGrantedEvent](WebXREnterExitUIOptions.md#ignoresessiongrantedevent)
- [onError](WebXREnterExitUIOptions.md#onerror)
- [optionalFeatures](WebXREnterExitUIOptions.md#optionalfeatures)
- [referenceSpaceType](WebXREnterExitUIOptions.md#referencespacetype)
- [renderTarget](WebXREnterExitUIOptions.md#rendertarget)
- [requiredFeatures](WebXREnterExitUIOptions.md#requiredfeatures)
- [sessionMode](WebXREnterExitUIOptions.md#sessionmode)

## Constructors

### constructor

• **new WebXREnterExitUIOptions**()

## Properties

### customButtons

• `Optional` **customButtons**: [`WebXREnterExitUIButton`](WebXREnterExitUIButton.md)[]

User provided buttons to enable/disable WebXR. The system will provide default if not set

#### Defined in

packages/dev/core/src/XR/webXREnterExitUI.ts:42

___

### ignoreSessionGrantedEvent

• `Optional` **ignoreSessionGrantedEvent**: `boolean`

If set, the `sessiongranted` event will not be registered. `sessiongranted` is used to move seamlessly between WebXR experiences.
If set to true the user will be forced to press the "enter XR" button even if sessiongranted event was triggered.
If not set and a sessiongranted event was triggered, the XR session will start automatically.

#### Defined in

packages/dev/core/src/XR/webXREnterExitUI.ts:73

___

### onError

• `Optional` **onError**: (`error`: `any`) => `void`

#### Type declaration

▸ (`error`): `void`

If defined, this function will be executed if the UI encounters an error when entering XR

##### Parameters

| Name | Type |
| :------ | :------ |
| `error` | `any` |

##### Returns

`void`

#### Defined in

packages/dev/core/src/XR/webXREnterExitUI.ts:78

___

### optionalFeatures

• `Optional` **optionalFeatures**: `string`[]

A list of optional features to init the session with

#### Defined in

packages/dev/core/src/XR/webXREnterExitUI.ts:61

___

### referenceSpaceType

• `Optional` **referenceSpaceType**: `XRReferenceSpaceType`

A reference space type to use when creating the default button.
Default is local-floor

#### Defined in

packages/dev/core/src/XR/webXREnterExitUI.ts:47

___

### renderTarget

• `Optional` **renderTarget**: [`Nullable`](../modules.md#nullable)[`WebXRRenderTarget`](../interfaces/WebXRRenderTarget.md)

Context to enter xr with

#### Defined in

packages/dev/core/src/XR/webXREnterExitUI.ts:51

___

### requiredFeatures

• `Optional` **requiredFeatures**: `string`[]

A list of optional features to init the session with

#### Defined in

packages/dev/core/src/XR/webXREnterExitUI.ts:66

___

### sessionMode

• `Optional` **sessionMode**: `XRSessionMode`

A session mode to use when creating the default button.
Default is immersive-vr

#### Defined in

packages/dev/core/src/XR/webXREnterExitUI.ts:56
