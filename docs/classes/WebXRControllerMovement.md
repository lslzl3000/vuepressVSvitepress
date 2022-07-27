[@dev/core](../README.md) / [Exports](../modules.md) / WebXRControllerMovement

# Class: WebXRControllerMovement

This is a movement feature to be used with WebXR-enabled motion controllers.
When enabled and attached, the feature will allow a user to move around and rotate in the scene using
the input of the attached controllers.

## Hierarchy

- [`WebXRAbstractFeature`](WebXRAbstractFeature.md)

  ↳ **`WebXRControllerMovement`**

## Table of contents

### Constructors

- [constructor](WebXRControllerMovement.md#constructor)

### Properties

- [\_controllers](WebXRControllerMovement.md#_controllers)
- [\_currentRegistrationConfigurations](WebXRControllerMovement.md#_currentregistrationconfigurations)
- [\_featureContext](WebXRControllerMovement.md#_featurecontext)
- [\_movementDirection](WebXRControllerMovement.md#_movementdirection)
- [\_movementState](WebXRControllerMovement.md#_movementstate)
- [\_tmpMovementTranslation](WebXRControllerMovement.md#_tmpmovementtranslation)
- [\_tmpRotationMatrix](WebXRControllerMovement.md#_tmprotationmatrix)
- [\_tmpTranslationDirection](WebXRControllerMovement.md#_tmptranslationdirection)
- [\_xrInput](WebXRControllerMovement.md#_xrinput)
- [\_xrSessionManager](WebXRControllerMovement.md#_xrsessionmanager)
- [disableAutoAttach](WebXRControllerMovement.md#disableautoattach)
- [isDisposed](WebXRControllerMovement.md#isdisposed)
- [xrNativeFeatureName](WebXRControllerMovement.md#xrnativefeaturename)
- [Name](WebXRControllerMovement.md#name)
- [REGISTRATIONS](WebXRControllerMovement.md#registrations)
- [Version](WebXRControllerMovement.md#version)

### Accessors

- [attached](WebXRControllerMovement.md#attached)
- [movementDirection](WebXRControllerMovement.md#movementdirection)
- [movementEnabled](WebXRControllerMovement.md#movementenabled)
- [movementOrientationFollowsViewerPose](WebXRControllerMovement.md#movementorientationfollowsviewerpose)
- [movementSpeed](WebXRControllerMovement.md#movementspeed)
- [movementThreshold](WebXRControllerMovement.md#movementthreshold)
- [rotationEnabled](WebXRControllerMovement.md#rotationenabled)
- [rotationSpeed](WebXRControllerMovement.md#rotationspeed)
- [rotationThreshold](WebXRControllerMovement.md#rotationthreshold)

### Methods

- [\_addNewAttachObserver](WebXRControllerMovement.md#_addnewattachobserver)
- [\_attachController](WebXRControllerMovement.md#_attachcontroller)
- [\_detachController](WebXRControllerMovement.md#_detachcontroller)
- [\_onXRFrame](WebXRControllerMovement.md#_onxrframe)
- [attach](WebXRControllerMovement.md#attach)
- [detach](WebXRControllerMovement.md#detach)
- [dispose](WebXRControllerMovement.md#dispose)
- [isCompatible](WebXRControllerMovement.md#iscompatible)

## Constructors

### constructor

• **new WebXRControllerMovement**(`_xrSessionManager`, `options`)

constructs a new movement controller system

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `_xrSessionManager` | [`WebXRSessionManager`](WebXRSessionManager.md) | an instance of WebXRSessionManager |
| `options` | [`IWebXRControllerMovementOptions`](../interfaces/IWebXRControllerMovementOptions.md) | configuration object for this feature |

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[constructor](WebXRAbstractFeature.md#constructor)

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerMovement.ts:309

## Properties

### \_controllers

• `Private` **\_controllers**: `Object` = `{}`

#### Index signature

▪ [controllerUniqueId: `string`]: { `registeredComponents`: `RegisteredComponent`[] ; `xrController`: [`WebXRInputSource`](WebXRInputSource.md)  }

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerMovement.ts:137

___

### \_currentRegistrationConfigurations

• `Private` **\_currentRegistrationConfigurations**: [`WebXRControllerMovementRegistrationConfiguration`](../modules.md#webxrcontrollermovementregistrationconfiguration)[] = `[]`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerMovement.ts:144

___

### \_featureContext

• `Private` **\_featureContext**: [`WebXRControllerMovementFeatureContext`](../modules.md#webxrcontrollermovementfeaturecontext)

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerMovement.ts:146

___

### \_movementDirection

• `Private` **\_movementDirection**: [`Nullable`](../modules.md#nullable)[`Quaternion`](Quaternion.md) = `null`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerMovement.ts:148

___

### \_movementState

• `Private` **\_movementState**: [`WebXRControllerMovementState`](../modules.md#webxrcontrollermovementstate)

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerMovement.ts:149

___

### \_tmpMovementTranslation

• `Private` **\_tmpMovementTranslation**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerMovement.ts:155

___

### \_tmpRotationMatrix

• `Private` **\_tmpRotationMatrix**: [`Matrix`](Matrix.md)

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerMovement.ts:153

___

### \_tmpTranslationDirection

• `Private` **\_tmpTranslationDirection**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerMovement.ts:154

___

### \_xrInput

• `Private` **\_xrInput**: [`WebXRInput`](WebXRInput.md)

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerMovement.ts:150

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

▪ `Static` `Readonly` **Name**: ``"xr-controller-movement"``

The module's name

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerMovement.ts:160

___

### REGISTRATIONS

▪ `Static` `Readonly` **REGISTRATIONS**: `Object`

Standard controller configurations.

#### Index signature

▪ [key: `string`]: [`WebXRControllerMovementRegistrationConfiguration`](../modules.md#webxrcontrollermovementregistrationconfiguration)[]

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerMovement.ts:165

___

### Version

▪ `Static` `Readonly` **Version**: ``1``

The (Babylon) version of this module.
This is an integer representing the implementation version.
This number does not correspond to the webxr specs version

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerMovement.ts:191

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

___

### movementDirection

• `get` **movementDirection**(): [`Nullable`](../modules.md#nullable)[`Quaternion`](Quaternion.md)

Current movement direction.  Will be null before XR Frames have been processed.

#### Returns

[`Nullable`](../modules.md#nullable)[`Quaternion`](Quaternion.md)

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerMovement.ts:196

___

### movementEnabled

• `get` **movementEnabled**(): `boolean`

Is movement enabled

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerMovement.ts:203

• `set` **movementEnabled**(`enabled`): `void`

Sets whether movement is enabled or not

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `enabled` | `boolean` | is movement enabled |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerMovement.ts:211

___

### movementOrientationFollowsViewerPose

• `get` **movementOrientationFollowsViewerPose**(): `boolean`

If movement follows viewer pose

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerMovement.ts:218

• `set` **movementOrientationFollowsViewerPose**(`followsPose`): `void`

Sets whether movement follows viewer pose

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `followsPose` | `boolean` | is movement should follow viewer pose |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerMovement.ts:226

___

### movementSpeed

• `get` **movementSpeed**(): `number`

Gets movement speed

#### Returns

`number`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerMovement.ts:233

• `set` **movementSpeed**(`movementSpeed`): `void`

Sets movement speed

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `movementSpeed` | `number` | movement speed |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerMovement.ts:241

___

### movementThreshold

• `get` **movementThreshold**(): `number`

Gets minimum threshold the controller's thumbstick/touchpad must pass before being recognized for movement (avoids jitter/unintentional movement)

#### Returns

`number`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerMovement.ts:248

• `set` **movementThreshold**(`movementThreshold`): `void`

Sets minimum threshold the controller's thumbstick/touchpad must pass before being recognized for movement (avoids jitter/unintentional movement)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `movementThreshold` | `number` | new threshold |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerMovement.ts:256

___

### rotationEnabled

• `get` **rotationEnabled**(): `boolean`

Is rotation enabled

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerMovement.ts:263

• `set` **rotationEnabled**(`enabled`): `void`

Sets whether rotation is enabled or not

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `enabled` | `boolean` | is rotation enabled |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerMovement.ts:271

___

### rotationSpeed

• `get` **rotationSpeed**(): `number`

Gets rotation speed factor

#### Returns

`number`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerMovement.ts:278

• `set` **rotationSpeed**(`rotationSpeed`): `void`

Sets rotation speed factor (1.0 is default)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `rotationSpeed` | `number` | new rotation speed factor |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerMovement.ts:286

___

### rotationThreshold

• `get` **rotationThreshold**(): `number`

Gets minimum threshold the controller's thumbstick/touchpad must pass before being recognized for rotation (avoids jitter/unintentional rotation)

#### Returns

`number`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerMovement.ts:293

• `set` **rotationThreshold**(`threshold`): `void`

Sets minimum threshold the controller's thumbstick/touchpad must pass before being recognized for rotation (avoids jitter/unintentional rotation)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `threshold` | `number` | new threshold |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerMovement.ts:301

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

packages/dev/core/src/XR/features/WebXRControllerMovement.ts:414

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

packages/dev/core/src/XR/features/WebXRControllerMovement.ts:500

___

### \_onXRFrame

▸ `Protected` **_onXRFrame**(`_xrFrame`): `void`

Occurs on every XR frame.

#### Parameters

| Name | Type |
| :------ | :------ |
| `_xrFrame` | `XRFrame` |

#### Returns

`void`

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[_onXRFrame](WebXRAbstractFeature.md#_onxrframe)

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerMovement.ts:377

___

### attach

▸ **attach**(): `boolean`

attach this feature

#### Returns

`boolean`

true if successful, false is failed or already attached

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[attach](WebXRAbstractFeature.md#attach)

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerMovement.ts:344

___

### detach

▸ **detach**(): `boolean`

detach this feature.

#### Returns

`boolean`

true if successful, false if failed or already detached

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[detach](WebXRAbstractFeature.md#detach)

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerMovement.ts:359

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
