[@dev/core](../README.md) / [Exports](../modules.md) / WebXRControllerPhysics

# Class: WebXRControllerPhysics

Add physics impostor to your webxr controllers,
including naive calculation of their linear and angular velocity

## Hierarchy

- [`WebXRAbstractFeature`](WebXRAbstractFeature.md)

  ↳ **`WebXRControllerPhysics`**

## Table of contents

### Constructors

- [constructor](WebXRControllerPhysics.md#constructor)

### Properties

- [\_controllers](WebXRControllerPhysics.md#_controllers)
- [\_debugMode](WebXRControllerPhysics.md#_debugmode)
- [\_delta](WebXRControllerPhysics.md#_delta)
- [\_headsetImpostor](WebXRControllerPhysics.md#_headsetimpostor)
- [\_headsetMesh](WebXRControllerPhysics.md#_headsetmesh)
- [\_lastTimestamp](WebXRControllerPhysics.md#_lasttimestamp)
- [\_tmpQuaternion](WebXRControllerPhysics.md#_tmpquaternion)
- [\_tmpVector](WebXRControllerPhysics.md#_tmpvector)
- [\_xrSessionManager](WebXRControllerPhysics.md#_xrsessionmanager)
- [disableAutoAttach](WebXRControllerPhysics.md#disableautoattach)
- [isDisposed](WebXRControllerPhysics.md#isdisposed)
- [xrNativeFeatureName](WebXRControllerPhysics.md#xrnativefeaturename)
- [Name](WebXRControllerPhysics.md#name)
- [Version](WebXRControllerPhysics.md#version)

### Accessors

- [attached](WebXRControllerPhysics.md#attached)

### Methods

- [\_addNewAttachObserver](WebXRControllerPhysics.md#_addnewattachobserver)
- [\_attachController](WebXRControllerPhysics.md#_attachcontroller)
- [\_createPhysicsImpostor](WebXRControllerPhysics.md#_createphysicsimpostor)
- [\_detachController](WebXRControllerPhysics.md#_detachcontroller)
- [\_onXRFrame](WebXRControllerPhysics.md#_onxrframe)
- [addController](WebXRControllerPhysics.md#addcontroller)
- [attach](WebXRControllerPhysics.md#attach)
- [detach](WebXRControllerPhysics.md#detach)
- [dispose](WebXRControllerPhysics.md#dispose)
- [getHeadsetImpostor](WebXRControllerPhysics.md#getheadsetimpostor)
- [getImpostorForController](WebXRControllerPhysics.md#getimpostorforcontroller)
- [isCompatible](WebXRControllerPhysics.md#iscompatible)
- [setPhysicsProperties](WebXRControllerPhysics.md#setphysicsproperties)

## Constructors

### constructor

• **new WebXRControllerPhysics**(`_xrSessionManager`, `_options`)

Construct a new Controller Physics Feature

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `_xrSessionManager` | [`WebXRSessionManager`](WebXRSessionManager.md) | the corresponding xr session manager |
| `_options` | [`IWebXRControllerPhysicsOptions`](IWebXRControllerPhysicsOptions.md) | options to create this feature with |

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[constructor](WebXRAbstractFeature.md#constructor)

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerPhysics.ts:174

## Properties

### \_controllers

• `Private` **\_controllers**: `Object` = `{}`

#### Index signature

▪ [id: `string`]: { `impostor`: [`PhysicsImpostor`](PhysicsImpostor.md) ; `impostorMesh?`: [`AbstractMesh`](AbstractMesh.md) ; `oldPos?`: [`Vector3`](Vector3.md) ; `oldRotation?`: [`Quaternion`](Quaternion.md) ; `oldSpeed?`: [`Vector3`](Vector3.md) ; `xrController`: [`WebXRInputSource`](WebXRInputSource.md)  }

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerPhysics.ts:140

___

### \_debugMode

• `Private` **\_debugMode**: `boolean` = `false`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerPhysics.ts:150

___

### \_delta

• `Private` **\_delta**: `number` = `0`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerPhysics.ts:151

___

### \_headsetImpostor

• `Private` `Optional` **\_headsetImpostor**: [`PhysicsImpostor`](PhysicsImpostor.md)

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerPhysics.ts:152

___

### \_headsetMesh

• `Private` `Optional` **\_headsetMesh**: [`AbstractMesh`](AbstractMesh.md)

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerPhysics.ts:153

___

### \_lastTimestamp

• `Private` **\_lastTimestamp**: `number` = `0`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerPhysics.ts:154

___

### \_tmpQuaternion

• `Private` **\_tmpQuaternion**: [`Quaternion`](Quaternion.md)

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerPhysics.ts:155

___

### \_tmpVector

• `Private` **\_tmpVector**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerPhysics.ts:156

___

### \_xrSessionManager

• `Protected` **\_xrSessionManager**: [`WebXRSessionManager`](WebXRSessionManager.md)

#### Inherited from

[WebXRAbstractFeature](WebXRAbstractFeature.md).[_xrSessionManager](WebXRAbstractFeature.md#_xrsessionmanager)

#### Defined in

packages/dev/core/src/XR/features/WebXRAbstractFeature.ts:37

___

### disableAutoAttach

• **disableAutoAttach**: `boolean` = `false`

Should auto-attach be disabled?

#### Inherited from

[WebXRAbstractFeature](WebXRAbstractFeature.md).[disableAutoAttach](WebXRAbstractFeature.md#disableautoattach)

#### Defined in

packages/dev/core/src/XR/features/WebXRAbstractFeature.ts:26

___

### isDisposed

• **isDisposed**: `boolean` = `false`

Is this feature disposed?

#### Inherited from

[WebXRAbstractFeature](WebXRAbstractFeature.md).[isDisposed](WebXRAbstractFeature.md#isdisposed)

#### Defined in

packages/dev/core/src/XR/features/WebXRAbstractFeature.ts:21

___

### xrNativeFeatureName

• **xrNativeFeatureName**: `string` = `""`

The name of the native xr feature name (like anchor, hit-test, or hand-tracking)

#### Inherited from

[WebXRAbstractFeature](WebXRAbstractFeature.md).[xrNativeFeatureName](WebXRAbstractFeature.md#xrnativefeaturename)

#### Defined in

packages/dev/core/src/XR/features/WebXRAbstractFeature.ts:31

___

### Name

▪ `Static` `Readonly` **Name**: ``"xr-physics-controller"``

The module's name

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerPhysics.ts:161

___

### Version

▪ `Static` `Readonly` **Version**: ``1``

The (Babylon) version of this module.
This is an integer representing the implementation version.
This number does not correspond to the webxr specs version

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerPhysics.ts:167

## Accessors

### attached

• `get` **attached**(): `boolean`

Is this feature attached

#### Returns

`boolean`

#### Inherited from

WebXRAbstractFeature.attached

#### Defined in

packages/dev/core/src/XR/features/WebXRAbstractFeature.ts:42

## Methods

### \_addNewAttachObserver

▸ `Protected` **_addNewAttachObserver**`T`(`observable`, `callback`): `void`

This is used to register callbacks that will automatically be removed when detach is called.

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `observable` | [`Observable`](Observable.md)`T` | the observable to which the observer will be attached |
| `callback` | (`eventData`: `T`, `eventState`: [`EventState`](EventState.md)) => `void` | the callback to register |

#### Returns

`void`

#### Inherited from

[WebXRAbstractFeature](WebXRAbstractFeature.md).[_addNewAttachObserver](WebXRAbstractFeature.md#_addnewattachobserver)

#### Defined in

packages/dev/core/src/XR/features/WebXRAbstractFeature.ts:113

___

### \_attachController

▸ `Private` **_attachController**(`xrController`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `xrController` | [`WebXRInputSource`](WebXRInputSource.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerPhysics.ts:79

___

### \_createPhysicsImpostor

▸ `Private` **_createPhysicsImpostor**(`xrController`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `xrController` | [`WebXRInputSource`](WebXRInputSource.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerPhysics.ts:115

___

### \_detachController

▸ `Private` **_detachController**(`xrControllerUniqueId`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `xrControllerUniqueId` | `string` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerPhysics.ts:375

___

### \_onXRFrame

▸ `Protected` **_onXRFrame**(`_xrFrame`): `void`

Code in this function will be executed on each xrFrame received from the browser.
This function will not execute after the feature is detached.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `_xrFrame` | `any` | the current frame |

#### Returns

`void`

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[_onXRFrame](WebXRAbstractFeature.md#_onxrframe)

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerPhysics.ts:310

___

### addController

▸ **addController**(`xrController`): `void`

Manually add a controller (if no xrInput was provided or physics engine was not enabled)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `xrController` | [`WebXRInputSource`](WebXRInputSource.md) | the controller to add |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerPhysics.ts:199

___

### attach

▸ **attach**(): `boolean`

attach this feature
Will usually be called by the features manager

#### Returns

`boolean`

true if successful.

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[attach](WebXRAbstractFeature.md#attach)

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerPhysics.ts:209

___

### detach

▸ **detach**(): `boolean`

detach this feature.
Will usually be called by the features manager

#### Returns

`boolean`

true if successful.

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[detach](WebXRAbstractFeature.md#detach)

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerPhysics.ts:251

___

### dispose

▸ **dispose**(): `void`

Dispose this feature and all of the resources attached

#### Returns

`void`

#### Inherited from

[WebXRAbstractFeature](WebXRAbstractFeature.md).[dispose](WebXRAbstractFeature.md#dispose)

#### Defined in

packages/dev/core/src/XR/features/WebXRAbstractFeature.ts:93

___

### getHeadsetImpostor

▸ **getHeadsetImpostor**(): `undefined` \| [`PhysicsImpostor`](PhysicsImpostor.md)

Get the headset impostor, if enabled

#### Returns

`undefined` \| [`PhysicsImpostor`](PhysicsImpostor.md)

the impostor

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerPhysics.ts:271

___

### getImpostorForController

▸ **getImpostorForController**(`controller`): [`Nullable`](../modules.md#nullable)[`PhysicsImpostor`](PhysicsImpostor.md)

Get the physics impostor of a specific controller.
The impostor is not attached to a mesh because a mesh for each controller is not obligatory

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `controller` | `string` \| [`WebXRInputSource`](WebXRInputSource.md) | the controller or the controller id of which to get the impostor |

#### Returns

[`Nullable`](../modules.md#nullable)[`PhysicsImpostor`](PhysicsImpostor.md)

the impostor or null

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerPhysics.ts:281

___

### isCompatible

▸ **isCompatible**(): `boolean`

This function will be executed during before enabling the feature and can be used to not-allow enabling it.
Note that at this point the session has NOT started, so this is purely checking if the browser supports it

#### Returns

`boolean`

whether or not the feature is compatible in this environment

#### Inherited from

[WebXRAbstractFeature](WebXRAbstractFeature.md).[isCompatible](WebXRAbstractFeature.md#iscompatible)

#### Defined in

packages/dev/core/src/XR/features/WebXRAbstractFeature.ts:104

___

### setPhysicsProperties

▸ **setPhysicsProperties**(`newProperties`): `void`

Update the physics properties provided in the constructor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newProperties` | `Object` | the new properties object |
| `newProperties.friction?` | `number` |  |
| `newProperties.impostorSize?` | `number` \| { `depth`: `number` ; `height`: `number` ; `width`: `number`  } |  |
| `newProperties.impostorType?` | `number` |  |
| `newProperties.restitution?` | `number` |  |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerPhysics.ts:298
