[@dev/core](../README.md) / [Exports](../modules.md) / WebXRWalkingLocomotion

# Class: WebXRWalkingLocomotion

A module that will enable VR locomotion by detecting when the user walks in place.

## Hierarchy

- [`WebXRAbstractFeature`](WebXRAbstractFeature.md)

  ↳ **`WebXRWalkingLocomotion`**

## Table of contents

### Constructors

- [constructor](WebXRWalkingLocomotion.md#constructor)

### Properties

- [\_forward](WebXRWalkingLocomotion.md#_forward)
- [\_isLocomotionTargetWebXRCamera](WebXRWalkingLocomotion.md#_islocomotiontargetwebxrcamera)
- [\_locomotionTarget](WebXRWalkingLocomotion.md#_locomotiontarget)
- [\_movement](WebXRWalkingLocomotion.md#_movement)
- [\_position](WebXRWalkingLocomotion.md#_position)
- [\_sessionManager](WebXRWalkingLocomotion.md#_sessionmanager)
- [\_up](WebXRWalkingLocomotion.md#_up)
- [\_walker](WebXRWalkingLocomotion.md#_walker)
- [\_xrSessionManager](WebXRWalkingLocomotion.md#_xrsessionmanager)
- [disableAutoAttach](WebXRWalkingLocomotion.md#disableautoattach)
- [isDisposed](WebXRWalkingLocomotion.md#isdisposed)
- [xrNativeFeatureName](WebXRWalkingLocomotion.md#xrnativefeaturename)

### Accessors

- [attached](WebXRWalkingLocomotion.md#attached)
- [locomotionTarget](WebXRWalkingLocomotion.md#locomotiontarget)
- [Name](WebXRWalkingLocomotion.md#name)
- [Version](WebXRWalkingLocomotion.md#version)

### Methods

- [\_addNewAttachObserver](WebXRWalkingLocomotion.md#_addnewattachobserver)
- [\_onXRFrame](WebXRWalkingLocomotion.md#_onxrframe)
- [attach](WebXRWalkingLocomotion.md#attach)
- [detach](WebXRWalkingLocomotion.md#detach)
- [dispose](WebXRWalkingLocomotion.md#dispose)
- [isCompatible](WebXRWalkingLocomotion.md#iscompatible)

## Constructors

### constructor

• **new WebXRWalkingLocomotion**(`sessionManager`, `options`)

Construct a new Walking Locomotion feature.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sessionManager` | [`WebXRSessionManager`](WebXRSessionManager.md) | manager for the current XR session |
| `options` | [`IWebXRWalkingLocomotionOptions`](../interfaces/IWebXRWalkingLocomotionOptions.md) | creation options, prominently including the vector target for locomotion |

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[constructor](WebXRAbstractFeature.md#constructor)

#### Defined in

packages/dev/core/src/XR/features/WebXRWalkingLocomotion.ts:402

## Properties

### \_forward

• `Private` **\_forward**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/XR/features/WebXRWalkingLocomotion.ts:364

___

### \_isLocomotionTargetWebXRCamera

• `Private` **\_isLocomotionTargetWebXRCamera**: `boolean`

#### Defined in

packages/dev/core/src/XR/features/WebXRWalkingLocomotion.ts:370

___

### \_locomotionTarget

• `Private` **\_locomotionTarget**: [`TransformNode`](TransformNode.md) \| [`WebXRCamera`](WebXRCamera.md)

#### Defined in

packages/dev/core/src/XR/features/WebXRWalkingLocomotion.ts:369

___

### \_movement

• `Private` **\_movement**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/XR/features/WebXRWalkingLocomotion.ts:366

___

### \_position

• `Private` **\_position**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/XR/features/WebXRWalkingLocomotion.ts:365

___

### \_sessionManager

• `Private` **\_sessionManager**: [`WebXRSessionManager`](WebXRSessionManager.md)

#### Defined in

packages/dev/core/src/XR/features/WebXRWalkingLocomotion.ts:362

___

### \_up

• `Private` **\_up**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/XR/features/WebXRWalkingLocomotion.ts:363

___

### \_walker

• `Private` **\_walker**: [`Nullable`](../modules.md#nullable)`Walker`

#### Defined in

packages/dev/core/src/XR/features/WebXRWalkingLocomotion.ts:367

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

### locomotionTarget

• `get` **locomotionTarget**(): [`TransformNode`](TransformNode.md) \| [`WebXRCamera`](WebXRCamera.md)

The target to be articulated by walking locomotion.
When the walking locomotion feature detects walking in place, this element's
X and Z coordinates will be modified to reflect locomotion. This target should
be either the XR space's origin (i.e., the parent node of the WebXRCamera) or
the WebXRCamera itself. Note that the WebXRCamera path will modify the position
of the WebXRCamera directly and is thus discouraged.

#### Returns

[`TransformNode`](TransformNode.md) \| [`WebXRCamera`](WebXRCamera.md)

#### Defined in

packages/dev/core/src/XR/features/WebXRWalkingLocomotion.ts:380

• `set` **locomotionTarget**(`locomotionTarget`): `void`

The target to be articulated by walking locomotion.
When the walking locomotion feature detects walking in place, this element's
X and Z coordinates will be modified to reflect locomotion. This target should
be either the XR space's origin (i.e., the parent node of the WebXRCamera) or
the WebXRCamera itself. Note that the WebXRCamera path will modify the position
of the WebXRCamera directly and is thus discouraged.

#### Parameters

| Name | Type |
| :------ | :------ |
| `locomotionTarget` | [`TransformNode`](TransformNode.md) \| [`WebXRCamera`](WebXRCamera.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/features/WebXRWalkingLocomotion.ts:392

___

### Name

• `Static` `get` **Name**(): `string`

The module's name.

#### Returns

`string`

#### Defined in

packages/dev/core/src/XR/features/WebXRWalkingLocomotion.ts:349

___

### Version

• `Static` `get` **Version**(): `number`

The (Babylon) version of this module.
This is an integer representing the implementation version.
This number has no external basis.

#### Returns

`number`

#### Defined in

packages/dev/core/src/XR/features/WebXRWalkingLocomotion.ts:358

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

### \_onXRFrame

▸ `Protected` **_onXRFrame**(`frame`): `void`

Code in this function will be executed on each xrFrame received from the browser.
This function will not execute after the feature is detached.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `frame` | `XRFrame` | the current frame |

#### Returns

`void`

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[_onXRFrame](WebXRAbstractFeature.md#_onxrframe)

#### Defined in

packages/dev/core/src/XR/features/WebXRWalkingLocomotion.ts:450

___

### attach

▸ **attach**(): `boolean`

Attaches the feature.
Typically called automatically by the features manager.

#### Returns

`boolean`

true if attach succeeded, false otherwise

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[attach](WebXRAbstractFeature.md#attach)

#### Defined in

packages/dev/core/src/XR/features/WebXRWalkingLocomotion.ts:427

___

### detach

▸ **detach**(): `boolean`

Detaches the feature.
Typically called automatically by the features manager.

#### Returns

`boolean`

true if detach succeeded, false otherwise

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[detach](WebXRAbstractFeature.md#detach)

#### Defined in

packages/dev/core/src/XR/features/WebXRWalkingLocomotion.ts:441

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

Checks whether this feature is compatible with the current WebXR session.
Walking locomotion is only compatible with "immersive-vr" sessions.

#### Returns

`boolean`

true if compatible, false otherwise

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[isCompatible](WebXRAbstractFeature.md#iscompatible)

#### Defined in

packages/dev/core/src/XR/features/WebXRWalkingLocomotion.ts:418
