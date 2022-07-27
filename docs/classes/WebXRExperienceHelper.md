[@dev/core](../README.md) / [Exports](../modules.md) / WebXRExperienceHelper

# Class: WebXRExperienceHelper

Base set of functionality needed to create an XR experience (WebXRSessionManager, Camera, StateManagement, etc.)

**`See`**

https://doc.babylonjs.com/how_to/webxr_experience_helpers

## Implements

- [`IDisposable`](../interfaces/IDisposable.md)

## Table of contents

### Constructors

- [constructor](WebXRExperienceHelper.md#constructor)

### Properties

- [\_attachedToElement](WebXRExperienceHelper.md#_attachedtoelement)
- [\_nonVRCamera](WebXRExperienceHelper.md#_nonvrcamera)
- [\_originalSceneAutoClear](WebXRExperienceHelper.md#_originalsceneautoclear)
- [\_spectatorCamera](WebXRExperienceHelper.md#_spectatorcamera)
- [\_spectatorMode](WebXRExperienceHelper.md#_spectatormode)
- [\_supported](WebXRExperienceHelper.md#_supported)
- [camera](WebXRExperienceHelper.md#camera)
- [featuresManager](WebXRExperienceHelper.md#featuresmanager)
- [onInitialXRPoseSetObservable](WebXRExperienceHelper.md#oninitialxrposesetobservable)
- [onStateChangedObservable](WebXRExperienceHelper.md#onstatechangedobservable)
- [sessionManager](WebXRExperienceHelper.md#sessionmanager)
- [state](WebXRExperienceHelper.md#state)

### Methods

- [\_nonXRToXRCamera](WebXRExperienceHelper.md#_nonxrtoxrcamera)
- [\_setState](WebXRExperienceHelper.md#_setstate)
- [dispose](WebXRExperienceHelper.md#dispose)
- [enableSpectatorMode](WebXRExperienceHelper.md#enablespectatormode)
- [enterXRAsync](WebXRExperienceHelper.md#enterxrasync)
- [exitXRAsync](WebXRExperienceHelper.md#exitxrasync)
- [CreateAsync](WebXRExperienceHelper.md#createasync)

## Constructors

### constructor

• `Private` **new WebXRExperienceHelper**(`_scene`)

Creates a WebXRExperienceHelper

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `_scene` | [`Scene`](Scene.md) | The scene the helper should be created in |

#### Defined in

packages/dev/core/src/XR/webXRExperienceHelper.ts:55

## Properties

### \_attachedToElement

• `Private` **\_attachedToElement**: `boolean` = `false`

#### Defined in

packages/dev/core/src/XR/webXRExperienceHelper.ts:20

___

### \_nonVRCamera

• `Private` **\_nonVRCamera**: [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md) = `null`

#### Defined in

packages/dev/core/src/XR/webXRExperienceHelper.ts:19

___

### \_originalSceneAutoClear

• `Private` **\_originalSceneAutoClear**: `boolean` = `true`

#### Defined in

packages/dev/core/src/XR/webXRExperienceHelper.ts:22

___

### \_spectatorCamera

• `Private` **\_spectatorCamera**: [`Nullable`](../modules.md#nullable)[`UniversalCamera`](UniversalCamera.md) = `null`

#### Defined in

packages/dev/core/src/XR/webXRExperienceHelper.ts:21

___

### \_spectatorMode

• `Private` **\_spectatorMode**: `boolean` = `false`

#### Defined in

packages/dev/core/src/XR/webXRExperienceHelper.ts:24

___

### \_supported

• `Private` **\_supported**: `boolean` = `false`

#### Defined in

packages/dev/core/src/XR/webXRExperienceHelper.ts:23

___

### camera

• **camera**: [`WebXRCamera`](WebXRCamera.md)

Camera used to render xr content

#### Defined in

packages/dev/core/src/XR/webXRExperienceHelper.ts:29

___

### featuresManager

• **featuresManager**: [`WebXRFeaturesManager`](WebXRFeaturesManager.md)

A features manager for this xr session

#### Defined in

packages/dev/core/src/XR/webXRExperienceHelper.ts:31

___

### onInitialXRPoseSetObservable

• **onInitialXRPoseSetObservable**: [`Observable`](Observable.md)[`WebXRCamera`](WebXRCamera.md)

Observers registered here will be triggered after the camera's initial transformation is set
This can be used to set a different ground level or an extra rotation.

Note that ground level is considered to be at 0. The height defined by the XR camera will be added
to the position set after this observable is done executing.

#### Defined in

packages/dev/core/src/XR/webXRExperienceHelper.ts:39

___

### onStateChangedObservable

• **onStateChangedObservable**: [`Observable`](Observable.md)[`WebXRState`](../enums/WebXRState.md)

Fires when the state of the experience helper has changed

#### Defined in

packages/dev/core/src/XR/webXRExperienceHelper.ts:43

___

### sessionManager

• **sessionManager**: [`WebXRSessionManager`](WebXRSessionManager.md)

Session manager used to keep track of xr session

#### Defined in

packages/dev/core/src/XR/webXRExperienceHelper.ts:45

___

### state

• **state**: [`WebXRState`](../enums/WebXRState.md) = `WebXRState.NOT_IN_XR`

The current state of the XR experience (eg. transitioning, in XR or not in XR)

#### Defined in

packages/dev/core/src/XR/webXRExperienceHelper.ts:49

## Methods

### \_nonXRToXRCamera

▸ `Private` **_nonXRToXRCamera**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/webXRExperienceHelper.ts:257

___

### \_setState

▸ `Private` **_setState**(`val`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `val` | [`WebXRState`](../enums/WebXRState.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/webXRExperienceHelper.ts:262

___

### dispose

▸ **dispose**(): `void`

Disposes of the experience helper

#### Returns

`void`

#### Implementation of

[IDisposable](../interfaces/IDisposable.md).[dispose](../interfaces/IDisposable.md#dispose)

#### Defined in

packages/dev/core/src/XR/webXRExperienceHelper.ts:88

___

### enableSpectatorMode

▸ **enableSpectatorMode**(): `void`

Enable spectator mode for desktop VR experiences.
When spectator mode is enabled a camera will be attached to the desktop canvas and will
display the first rig camera's view on the desktop canvas.
Please note that this will degrade performance, as it requires another camera render.
It is also not recommended to enable this in devices like the quest, as it brings no benefit there.

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/webXRExperienceHelper.ts:226

___

### enterXRAsync

▸ **enterXRAsync**(`sessionMode`, `referenceSpaceType`, `renderTarget?`, `sessionCreationOptions?`): `Promise`[`WebXRSessionManager`](WebXRSessionManager.md)

Enters XR mode (This must be done within a user interaction in most browsers eg. button click)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sessionMode` | `XRSessionMode` | options for the XR session |
| `referenceSpaceType` | `XRReferenceSpaceType` | frame of reference of the XR session |
| `renderTarget` | [`WebXRRenderTarget`](../interfaces/WebXRRenderTarget.md) | the output canvas that will be used to enter XR mode |
| `sessionCreationOptions` | `XRSessionInit` | optional XRSessionInit object to init the session with |

#### Returns

`Promise`[`WebXRSessionManager`](WebXRSessionManager.md)

promise that resolves after xr mode has entered

#### Defined in

packages/dev/core/src/XR/webXRExperienceHelper.ts:108

___

### exitXRAsync

▸ **exitXRAsync**(): `Promise``void`

Exits XR mode and returns the scene to its original state

#### Returns

`Promise``void`

promise that resolves after xr mode has exited

#### Defined in

packages/dev/core/src/XR/webXRExperienceHelper.ts:210

___

### CreateAsync

▸ `Static` **CreateAsync**(`scene`): `Promise`[`WebXRExperienceHelper`](WebXRExperienceHelper.md)

Creates the experience helper

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | the scene to attach the experience helper to |

#### Returns

`Promise`[`WebXRExperienceHelper`](WebXRExperienceHelper.md)

a promise for the experience helper

#### Defined in

packages/dev/core/src/XR/webXRExperienceHelper.ts:70
