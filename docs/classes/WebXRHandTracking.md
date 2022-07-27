[@dev/core](../README.md) / [Exports](../modules.md) / WebXRHandTracking

# Class: WebXRHandTracking

WebXR Hand Joint tracking feature, available for selected browsers and devices

## Hierarchy

- [`WebXRAbstractFeature`](WebXRAbstractFeature.md)

  ↳ **`WebXRHandTracking`**

## Table of contents

### Constructors

- [constructor](WebXRHandTracking.md#constructor)

### Properties

- [\_attachedHands](WebXRHandTracking.md#_attachedhands)
- [\_handResources](WebXRHandTracking.md#_handresources)
- [\_trackingHands](WebXRHandTracking.md#_trackinghands)
- [\_xrSessionManager](WebXRHandTracking.md#_xrsessionmanager)
- [disableAutoAttach](WebXRHandTracking.md#disableautoattach)
- [isDisposed](WebXRHandTracking.md#isdisposed)
- [onHandAddedObservable](WebXRHandTracking.md#onhandaddedobservable)
- [onHandRemovedObservable](WebXRHandTracking.md#onhandremovedobservable)
- [options](WebXRHandTracking.md#options)
- [xrNativeFeatureName](WebXRHandTracking.md#xrnativefeaturename)
- [DEFAULT\_HAND\_MODEL\_BASE\_URL](WebXRHandTracking.md#default_hand_model_base_url)
- [DEFAULT\_HAND\_MODEL\_LEFT\_FILENAME](WebXRHandTracking.md#default_hand_model_left_filename)
- [DEFAULT\_HAND\_MODEL\_RIGHT\_FILENAME](WebXRHandTracking.md#default_hand_model_right_filename)
- [DEFAULT\_HAND\_MODEL\_SHADER\_URL](WebXRHandTracking.md#default_hand_model_shader_url)
- [Name](WebXRHandTracking.md#name)
- [Version](WebXRHandTracking.md#version)
- [\_ICOSPHERE\_PARAMS](WebXRHandTracking.md#_icosphere_params)
- [\_LeftHandGLB](WebXRHandTracking.md#_lefthandglb)
- [\_RightHandGLB](WebXRHandTracking.md#_righthandglb)

### Accessors

- [attached](WebXRHandTracking.md#attached)

### Methods

- [\_addNewAttachObserver](WebXRHandTracking.md#_addnewattachobserver)
- [\_attachHand](WebXRHandTracking.md#_attachhand)
- [\_detachHand](WebXRHandTracking.md#_detachhand)
- [\_detachHandById](WebXRHandTracking.md#_detachhandbyid)
- [\_onXRFrame](WebXRHandTracking.md#_onxrframe)
- [attach](WebXRHandTracking.md#attach)
- [detach](WebXRHandTracking.md#detach)
- [dispose](WebXRHandTracking.md#dispose)
- [getHandByControllerId](WebXRHandTracking.md#gethandbycontrollerid)
- [getHandByHandedness](WebXRHandTracking.md#gethandbyhandedness)
- [isCompatible](WebXRHandTracking.md#iscompatible)
- [\_GenerateDefaultHandMeshRigMapping](WebXRHandTracking.md#_generatedefaulthandmeshrigmapping)
- [\_GenerateDefaultHandMeshesAsync](WebXRHandTracking.md#_generatedefaulthandmeshesasync)
- [\_GenerateTrackedJointMeshes](WebXRHandTracking.md#_generatetrackedjointmeshes)

## Constructors

### constructor

• **new WebXRHandTracking**(`_xrSessionManager`, `options`)

Creates a new instance of the XR hand tracking feature.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `_xrSessionManager` | [`WebXRSessionManager`](WebXRSessionManager.md) | An instance of WebXRSessionManager. |
| `options` | [`IWebXRHandTrackingOptions`](../interfaces/IWebXRHandTrackingOptions.md) | Options to use when constructing this feature. |

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[constructor](WebXRAbstractFeature.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHandTracking.ts:729

## Properties

### \_attachedHands

• `Private` **\_attachedHands**: `Object` = `{}`

#### Index signature

▪ [uniqueId: `string`]: [`WebXRHand`](WebXRHand.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHandTracking.ts:671

___

### \_handResources

• `Private` **\_handResources**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `handMeshes` | [`Nullable`](../modules.md#nullable){ `left`: [`AbstractMesh`](AbstractMesh.md) ; `right`: [`AbstractMesh`](AbstractMesh.md)  } |
| `jointMeshes` | [`Nullable`](../modules.md#nullable){ `left`: [`AbstractMesh`](AbstractMesh.md)[] ; `right`: [`AbstractMesh`](AbstractMesh.md)[]  } |
| `rigMappings` | [`Nullable`](../modules.md#nullable){ `left`: [`XRHandMeshRigMapping`](../modules.md#xrhandmeshrigmapping) ; `right`: [`XRHandMeshRigMapping`](../modules.md#xrhandmeshrigmapping)  } |

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHandTracking.ts:680

___

### \_trackingHands

• `Private` **\_trackingHands**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `left` | [`Nullable`](../modules.md#nullable)[`WebXRHand`](WebXRHand.md) |
| `right` | [`Nullable`](../modules.md#nullable)[`WebXRHand`](WebXRHand.md) |

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHandTracking.ts:675

___

### \_xrSessionManager

• `Protected` **\_xrSessionManager**: [`WebXRSessionManager`](WebXRSessionManager.md)

#### Inherited from

[WebXRAbstractFeature](WebXRAbstractFeature.md).[_xrSessionManager](WebXRAbstractFeature.md#_xrsessionmanager)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRAbstractFeature.ts:37

___

### disableAutoAttach

• **disableAutoAttach**: `boolean` = `false`

Should auto-attach be disabled?

#### Inherited from

[WebXRAbstractFeature](WebXRAbstractFeature.md).[disableAutoAttach](WebXRAbstractFeature.md#disableautoattach)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRAbstractFeature.ts:26

___

### isDisposed

• **isDisposed**: `boolean` = `false`

Is this feature disposed?

#### Inherited from

[WebXRAbstractFeature](WebXRAbstractFeature.md).[isDisposed](WebXRAbstractFeature.md#isdisposed)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRAbstractFeature.ts:21

___

### onHandAddedObservable

• **onHandAddedObservable**: [`Observable`](Observable.md)[`WebXRHand`](WebXRHand.md)

This observable will notify registered observers when a new hand object was added and initialized

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHandTracking.ts:689

___

### onHandRemovedObservable

• **onHandRemovedObservable**: [`Observable`](Observable.md)[`WebXRHand`](WebXRHand.md)

This observable will notify its observers right before the hand object is disposed

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHandTracking.ts:693

___

### options

• `Readonly` **options**: [`IWebXRHandTrackingOptions`](../interfaces/IWebXRHandTrackingOptions.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHandTracking.ts:732

___

### xrNativeFeatureName

• **xrNativeFeatureName**: `string` = `""`

The name of the native xr feature name (like anchor, hit-test, or hand-tracking)

#### Inherited from

[WebXRAbstractFeature](WebXRAbstractFeature.md).[xrNativeFeatureName](WebXRAbstractFeature.md#xrnativefeaturename)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRAbstractFeature.ts:31

___

### DEFAULT\_HAND\_MODEL\_BASE\_URL

▪ `Static` **DEFAULT\_HAND\_MODEL\_BASE\_URL**: `string` = `"https://assets.babylonjs.com/meshes/HandMeshes/"`

The base URL for the default hand model.

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHandTracking.ts:508

___

### DEFAULT\_HAND\_MODEL\_LEFT\_FILENAME

▪ `Static` **DEFAULT\_HAND\_MODEL\_LEFT\_FILENAME**: `string` = `"l_hand_rhs.glb"`

The filename to use for the default left hand model.

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHandTracking.ts:512

___

### DEFAULT\_HAND\_MODEL\_RIGHT\_FILENAME

▪ `Static` **DEFAULT\_HAND\_MODEL\_RIGHT\_FILENAME**: `string` = `"r_hand_rhs.glb"`

The filename to use for the default right hand model.

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHandTracking.ts:510

___

### DEFAULT\_HAND\_MODEL\_SHADER\_URL

▪ `Static` **DEFAULT\_HAND\_MODEL\_SHADER\_URL**: `string` = `"https://assets.babylonjs.com/meshes/HandMeshes/handsShader.json"`

The URL pointing to the default hand model NodeMaterial shader.

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHandTracking.ts:514

___

### Name

▪ `Static` `Readonly` **Name**: ``"xr-hand-tracking"``

The module's name

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHandTracking.ts:499

___

### Version

▪ `Static` `Readonly` **Version**: ``1``

The (Babylon) version of this module.
This is an integer representing the implementation version.
This number does not correspond to the WebXR specs version

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHandTracking.ts:505

___

### \_ICOSPHERE\_PARAMS

▪ `Static` `Private` `Readonly` **\_ICOSPHERE\_PARAMS**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `flat` | `boolean` |
| `radius` | `number` |
| `subdivisions` | `number` |

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHandTracking.ts:517

___

### \_LeftHandGLB

▪ `Static` `Private` **\_LeftHandGLB**: [`Nullable`](../modules.md#nullable)[`ISceneLoaderAsyncResult`](../interfaces/ISceneLoaderAsyncResult.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHandTracking.ts:520

___

### \_RightHandGLB

▪ `Static` `Private` **\_RightHandGLB**: [`Nullable`](../modules.md#nullable)[`ISceneLoaderAsyncResult`](../interfaces/ISceneLoaderAsyncResult.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHandTracking.ts:519

## Accessors

### attached

• `get` **attached**(): `boolean`

Is this feature attached

#### Returns

`boolean`

#### Inherited from

WebXRAbstractFeature.attached

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRAbstractFeature.ts:42

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

https://github.com/babylon.js/core/src/XR/features/WebXRAbstractFeature.ts:113

___

### \_attachHand

▸ `Private` **_attachHand**(`xrController`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `xrController` | [`WebXRInputSource`](WebXRInputSource.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHandTracking.ts:819

___

### \_detachHand

▸ `Private` **_detachHand**(`xrController`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `xrController` | [`WebXRInputSource`](WebXRInputSource.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHandTracking.ts:854

___

### \_detachHandById

▸ `Private` **_detachHandById**(`controllerId`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `controllerId` | `string` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHandTracking.ts:841

___

### \_onXRFrame

▸ `Protected` **_onXRFrame**(`_xrFrame`): `void`

Code in this function will be executed on each xrFrame received from the browser.
This function will not execute after the feature is detached.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `_xrFrame` | `XRFrame` | the current frame |

#### Returns

`void`

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[_onXRFrame](WebXRAbstractFeature.md#_onxrframe)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHandTracking.ts:814

___

### attach

▸ **attach**(): `boolean`

Attach this feature.
Will usually be called by the features manager.

#### Returns

`boolean`

true if successful.

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[attach](WebXRAbstractFeature.md#attach)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHandTracking.ts:781

___

### detach

▸ **detach**(): `boolean`

Detach this feature.
Will usually be called by the features manager.

#### Returns

`boolean`

true if successful.

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[detach](WebXRAbstractFeature.md#detach)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHandTracking.ts:864

___

### dispose

▸ **dispose**(): `void`

Dispose this feature and all of the resources attached.

#### Returns

`void`

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[dispose](WebXRAbstractFeature.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHandTracking.ts:877

___

### getHandByControllerId

▸ **getHandByControllerId**(`controllerId`): [`Nullable`](../modules.md#nullable)[`WebXRHand`](WebXRHand.md)

Get the hand object according to the controller id

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `controllerId` | `string` | the controller id to which we want to get the hand |

#### Returns

[`Nullable`](../modules.md#nullable)[`WebXRHand`](WebXRHand.md)

null if not found or the WebXRHand object if found

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHandTracking.ts:708

___

### getHandByHandedness

▸ **getHandByHandedness**(`handedness`): [`Nullable`](../modules.md#nullable)[`WebXRHand`](WebXRHand.md)

Get a hand object according to the requested handedness

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `handedness` | `XRHandedness` | the handedness to request |

#### Returns

[`Nullable`](../modules.md#nullable)[`WebXRHand`](WebXRHand.md)

null if not found or the WebXRHand object if found

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHandTracking.ts:717

___

### isCompatible

▸ **isCompatible**(): `boolean`

Check if the needed objects are defined.
This does not mean that the feature is enabled, but that the objects needed are well defined.

#### Returns

`boolean`

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[isCompatible](WebXRAbstractFeature.md#iscompatible)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHandTracking.ts:699

___

### \_GenerateDefaultHandMeshRigMapping

▸ `Static` `Private` **_GenerateDefaultHandMeshRigMapping**(`handedness`): [`XRHandMeshRigMapping`](../modules.md#xrhandmeshrigmapping)

Generates a mapping from XRHandJoint to bone name for the default hand mesh.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `handedness` | `XRHandedness` | The handedness being mapped for. |

#### Returns

[`XRHandMeshRigMapping`](../modules.md#xrhandmeshrigmapping)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHandTracking.ts:640

___

### \_GenerateDefaultHandMeshesAsync

▸ `Static` `Private` **_GenerateDefaultHandMeshesAsync**(`scene`, `options?`): `Promise`{ `left`: [`AbstractMesh`](AbstractMesh.md) ; `right`: [`AbstractMesh`](AbstractMesh.md)  }

#### Parameters

| Name | Type |
| :------ | :------ |
| `scene` | [`Scene`](Scene.md) |
| `options?` | [`IWebXRHandTrackingOptions`](../interfaces/IWebXRHandTrackingOptions.md) |

#### Returns

`Promise`{ `left`: [`AbstractMesh`](AbstractMesh.md) ; `right`: [`AbstractMesh`](AbstractMesh.md)  }

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHandTracking.ts:557

___

### \_GenerateTrackedJointMeshes

▸ `Static` `Private` **_GenerateTrackedJointMeshes**(`featureOptions`): `Object`

#### Parameters

| Name | Type |
| :------ | :------ |
| `featureOptions` | [`IWebXRHandTrackingOptions`](../interfaces/IWebXRHandTrackingOptions.md) |

#### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `left` | [`AbstractMesh`](AbstractMesh.md)[] |
| `right` | [`AbstractMesh`](AbstractMesh.md)[] |

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHandTracking.ts:522
