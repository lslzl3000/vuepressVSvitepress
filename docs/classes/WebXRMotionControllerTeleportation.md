[@dev/core](../README.md) / [Exports](../modules.md) / WebXRMotionControllerTeleportation

# Class: WebXRMotionControllerTeleportation

This is a teleportation feature to be used with WebXR-enabled motion controllers.
When enabled and attached, the feature will allow a user to move around and rotate in the scene using
the input of the attached controllers.

## Hierarchy

- [`WebXRAbstractFeature`](WebXRAbstractFeature.md)

  ↳ **`WebXRMotionControllerTeleportation`**

## Table of contents

### Constructors

- [constructor](WebXRMotionControllerTeleportation.md#constructor)

### Properties

- [\_controllers](WebXRMotionControllerTeleportation.md#_controllers)
- [\_currentTeleportationControllerId](WebXRMotionControllerTeleportation.md#_currentteleportationcontrollerid)
- [\_floorMeshes](WebXRMotionControllerTeleportation.md#_floormeshes)
- [\_quadraticBezierCurve](WebXRMotionControllerTeleportation.md#_quadraticbeziercurve)
- [\_rotationEnabled](WebXRMotionControllerTeleportation.md#_rotationenabled)
- [\_selectionFeature](WebXRMotionControllerTeleportation.md#_selectionfeature)
- [\_snapToPositions](WebXRMotionControllerTeleportation.md#_snaptopositions)
- [\_snappedToPoint](WebXRMotionControllerTeleportation.md#_snappedtopoint)
- [\_teleportationRingMaterial](WebXRMotionControllerTeleportation.md#_teleportationringmaterial)
- [\_tmpQuaternion](WebXRMotionControllerTeleportation.md#_tmpquaternion)
- [\_tmpRay](WebXRMotionControllerTeleportation.md#_tmpray)
- [\_tmpVector](WebXRMotionControllerTeleportation.md#_tmpvector)
- [\_xrSessionManager](WebXRMotionControllerTeleportation.md#_xrsessionmanager)
- [backwardsMovementEnabled](WebXRMotionControllerTeleportation.md#backwardsmovementenabled)
- [backwardsTeleportationDistance](WebXRMotionControllerTeleportation.md#backwardsteleportationdistance)
- [disableAutoAttach](WebXRMotionControllerTeleportation.md#disableautoattach)
- [isDisposed](WebXRMotionControllerTeleportation.md#isdisposed)
- [onTargetMeshPositionUpdatedObservable](WebXRMotionControllerTeleportation.md#ontargetmeshpositionupdatedobservable)
- [parabolicCheckRadius](WebXRMotionControllerTeleportation.md#paraboliccheckradius)
- [parabolicRayEnabled](WebXRMotionControllerTeleportation.md#parabolicrayenabled)
- [rotationAngle](WebXRMotionControllerTeleportation.md#rotationangle)
- [skipNextTeleportation](WebXRMotionControllerTeleportation.md#skipnextteleportation)
- [straightRayEnabled](WebXRMotionControllerTeleportation.md#straightrayenabled)
- [teleportationEnabled](WebXRMotionControllerTeleportation.md#teleportationenabled)
- [xrNativeFeatureName](WebXRMotionControllerTeleportation.md#xrnativefeaturename)
- [Name](WebXRMotionControllerTeleportation.md#name)
- [Version](WebXRMotionControllerTeleportation.md#version)

### Accessors

- [attached](WebXRMotionControllerTeleportation.md#attached)
- [rotationEnabled](WebXRMotionControllerTeleportation.md#rotationenabled)
- [snapPointsOnly](WebXRMotionControllerTeleportation.md#snappointsonly)
- [teleportationTargetMesh](WebXRMotionControllerTeleportation.md#teleportationtargetmesh)

### Methods

- [\_addNewAttachObserver](WebXRMotionControllerTeleportation.md#_addnewattachobserver)
- [\_attachController](WebXRMotionControllerTeleportation.md#_attachcontroller)
- [\_createDefaultTargetMesh](WebXRMotionControllerTeleportation.md#_createdefaulttargetmesh)
- [\_detachController](WebXRMotionControllerTeleportation.md#_detachcontroller)
- [\_findClosestSnapPointWithRadius](WebXRMotionControllerTeleportation.md#_findclosestsnappointwithradius)
- [\_onXRFrame](WebXRMotionControllerTeleportation.md#_onxrframe)
- [\_setTargetMeshPosition](WebXRMotionControllerTeleportation.md#_settargetmeshposition)
- [\_setTargetMeshVisibility](WebXRMotionControllerTeleportation.md#_settargetmeshvisibility)
- [\_showParabolicPath](WebXRMotionControllerTeleportation.md#_showparabolicpath)
- [\_teleportForward](WebXRMotionControllerTeleportation.md#_teleportforward)
- [addBlockerMesh](WebXRMotionControllerTeleportation.md#addblockermesh)
- [addFloorMesh](WebXRMotionControllerTeleportation.md#addfloormesh)
- [addSnapPoint](WebXRMotionControllerTeleportation.md#addsnappoint)
- [attach](WebXRMotionControllerTeleportation.md#attach)
- [detach](WebXRMotionControllerTeleportation.md#detach)
- [dispose](WebXRMotionControllerTeleportation.md#dispose)
- [isCompatible](WebXRMotionControllerTeleportation.md#iscompatible)
- [removeBlockerMesh](WebXRMotionControllerTeleportation.md#removeblockermesh)
- [removeFloorMesh](WebXRMotionControllerTeleportation.md#removefloormesh)
- [removeFloorMeshByName](WebXRMotionControllerTeleportation.md#removefloormeshbyname)
- [removeSnapPoint](WebXRMotionControllerTeleportation.md#removesnappoint)
- [setSelectionFeature](WebXRMotionControllerTeleportation.md#setselectionfeature)

## Constructors

### constructor

• **new WebXRMotionControllerTeleportation**(`_xrSessionManager`, `_options`)

constructs a new teleportation system

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `_xrSessionManager` | [`WebXRSessionManager`](WebXRSessionManager.md) | an instance of WebXRSessionManager |
| `_options` | [`IWebXRTeleportationOptions`](../interfaces/IWebXRTeleportationOptions.md) | configuration object for this feature |

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[constructor](WebXRAbstractFeature.md#constructor)

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:261

## Properties

### \_controllers

• `Private` **\_controllers**: `Object` = `{}`

#### Index signature

▪ [controllerUniqueId: `string`]: { `onAxisChangedObserver?`: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`IWebXRMotionControllerAxesValue`](../interfaces/IWebXRMotionControllerAxesValue.md) ; `onButtonChangedObserver?`: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`WebXRControllerComponent`](WebXRControllerComponent.md) ; `teleportationComponent?`: [`WebXRControllerComponent`](WebXRControllerComponent.md) ; `teleportationState`: { `backwards`: `boolean` ; `baseRotation`: `number` ; `currentRotation`: `number` ; `forward`: `boolean` ; `rotating`: `boolean`  } ; `xrController`: [`WebXRInputSource`](WebXRInputSource.md)  }

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:139

___

### \_currentTeleportationControllerId

• `Private` **\_currentTeleportationControllerId**: `string`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:154

___

### \_floorMeshes

• `Private` **\_floorMeshes**: [`AbstractMesh`](AbstractMesh.md)[]

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:155

___

### \_quadraticBezierCurve

• `Private` **\_quadraticBezierCurve**: [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:156

___

### \_rotationEnabled

• `Private` **\_rotationEnabled**: `boolean` = `true`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:224

___

### \_selectionFeature

• `Private` **\_selectionFeature**: [`Nullable`](../modules.md#nullable)[`IWebXRFeature`](../interfaces/IWebXRFeature.md)

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:157

___

### \_snapToPositions

• `Private` **\_snapToPositions**: [`Vector3`](Vector3.md)[]

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:158

___

### \_snappedToPoint

• `Private` **\_snappedToPoint**: `boolean` = `false`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:159

___

### \_teleportationRingMaterial

• `Private` `Optional` **\_teleportationRingMaterial**: [`StandardMaterial`](StandardMaterial.md)

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:160

___

### \_tmpQuaternion

• `Private` **\_tmpQuaternion**: [`Quaternion`](Quaternion.md)

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:163

___

### \_tmpRay

• `Private` **\_tmpRay**: [`Ray`](Ray.md)

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:161

___

### \_tmpVector

• `Private` **\_tmpVector**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:162

___

### \_xrSessionManager

• `Protected` **\_xrSessionManager**: [`WebXRSessionManager`](WebXRSessionManager.md)

#### Inherited from

[WebXRAbstractFeature](WebXRAbstractFeature.md).[_xrSessionManager](WebXRAbstractFeature.md#_xrsessionmanager)

#### Defined in

packages/dev/core/src/XR/features/WebXRAbstractFeature.ts:37

___

### backwardsMovementEnabled

• **backwardsMovementEnabled**: `boolean` = `true`

Is movement backwards enabled

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:185

___

### backwardsTeleportationDistance

• **backwardsTeleportationDistance**: `number` = `0.7`

Distance to travel when moving backwards

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:189

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

### onTargetMeshPositionUpdatedObservable

• **onTargetMeshPositionUpdatedObservable**: [`Observable`](Observable.md)[`PickingInfo`](PickingInfo.md)

This observable will notify when the target mesh position was updated.
The picking info it provides contains the point to which the target mesh will move ()

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:217

___

### parabolicCheckRadius

• **parabolicCheckRadius**: `number` = `5`

The distance from the user to the inspection point in the direction of the controller
A higher number will allow the user to move further
defaults to 5 (meters, in xr units)

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:195

___

### parabolicRayEnabled

• **parabolicRayEnabled**: `boolean` = `true`

Should the module support parabolic ray on top of direct ray
If enabled, the user will be able to point "at the sky" and move according to predefined radius distance
Very helpful when moving between floors / different heights

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:201

___

### rotationAngle

• **rotationAngle**: `number`

How much rotation should be applied when rotating right and left

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:211

___

### skipNextTeleportation

• **skipNextTeleportation**: `boolean` = `false`

Skip the next teleportation. This can be controlled by the user to prevent the user from teleportation
to sections that are not yet "unlocked", but should still show the teleportation mesh.

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:169

___

### straightRayEnabled

• **straightRayEnabled**: `boolean` = `true`

The second type of ray - straight line.
Should it be enabled or should the parabolic line be the only one.

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:207

___

### teleportationEnabled

• **teleportationEnabled**: `boolean` = `true`

Is teleportation enabled. Can be used to allow rotation only.

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:222

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

▪ `Static` `Readonly` **Name**: ``"xr-controller-teleportation"``

The module's name

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:174

___

### Version

▪ `Static` `Readonly` **Version**: ``1``

The (Babylon) version of this module.
This is an integer representing the implementation version.
This number does not correspond to the webxr specs version

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:180

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

### rotationEnabled

• `get` **rotationEnabled**(): `boolean`

Is rotation enabled when moving forward?
Disabling this feature will prevent the user from deciding the direction when teleporting

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:230

• `set` **rotationEnabled**(`enabled`): `void`

Sets whether rotation is enabled or not

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `enabled` | `boolean` | is rotation enabled when teleportation is shown |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:238

___

### snapPointsOnly

• `get` **snapPointsOnly**(): `boolean`

Get the snapPointsOnly flag

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:277

• `set` **snapPointsOnly**(`snapToPoints`): `void`

Sets the snapPointsOnly flag

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `snapToPoints` | `boolean` | should teleportation be exclusively to snap points |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:285

___

### teleportationTargetMesh

• `get` **teleportationTargetMesh**(): [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

Exposes the currently set teleportation target mesh.

#### Returns

[`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:252

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

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:513

___

### \_createDefaultTargetMesh

▸ `Private` **_createDefaultTargetMesh**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:692

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

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:789

___

### \_findClosestSnapPointWithRadius

▸ `Private` **_findClosestSnapPointWithRadius**(`realPosition`, `radius?`): ``null``

#### Parameters

| Name | Type |
| :------ | :------ |
| `realPosition` | [`Vector3`](Vector3.md) |
| `radius` | `number` |

#### Returns

``null``

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:806

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

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:423

___

### \_setTargetMeshPosition

▸ `Private` **_setTargetMeshPosition**(`pickInfo`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `pickInfo` | [`PickingInfo`](PickingInfo.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:822

___

### \_setTargetMeshVisibility

▸ `Private` **_setTargetMeshVisibility**(`visible`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `visible` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:839

___

### \_showParabolicPath

▸ `Private` **_showParabolicPath**(`pickInfo`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `pickInfo` | [`PickingInfo`](PickingInfo.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:866

___

### \_teleportForward

▸ `Private` **_teleportForward**(`controllerId`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `controllerId` | `string` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:893

___

### addBlockerMesh

▸ **addBlockerMesh**(`mesh`): `void`

Add a mesh to the list of meshes blocking the teleportation ray

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | The mesh to add to the teleportation-blocking meshes |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:301

___

### addFloorMesh

▸ **addFloorMesh**(`mesh`): `void`

Add a new mesh to the floor meshes array

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | the mesh to use as floor mesh |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:293

___

### addSnapPoint

▸ **addSnapPoint**(`newSnapPoint`): `void`

Add a new snap-to point to fix teleportation to this position

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newSnapPoint` | [`Vector3`](Vector3.md) | The new Snap-To point |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:310

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

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:314

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

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:332

___

### dispose

▸ **dispose**(): `void`

Dispose this feature and all of the resources attached

#### Returns

`void`

#### Overrides

[WebXRAbstractFeature](WebXRAbstractFeature.md).[dispose](WebXRAbstractFeature.md#dispose)

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:348

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

### removeBlockerMesh

▸ **removeBlockerMesh**(`mesh`): `void`

Remove a mesh from the blocker meshes array

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | the mesh to remove |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:368

___

### removeFloorMesh

▸ **removeFloorMesh**(`mesh`): `void`

Remove a mesh from the floor meshes array

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | the mesh to remove |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:357

___

### removeFloorMeshByName

▸ **removeFloorMeshByName**(`name`): `void`

Remove a mesh from the floor meshes array using its name

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | the mesh name to remove |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:380

___

### removeSnapPoint

▸ **removeSnapPoint**(`snapPointToRemove`): `boolean`

This function will iterate through the array, searching for this point or equal to it. It will then remove it from the snap-to array

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `snapPointToRemove` | [`Vector3`](Vector3.md) | the point (or a clone of it) to be removed from the array |

#### Returns

`boolean`

was the point found and removed or not

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:392

___

### setSelectionFeature

▸ **setSelectionFeature**(`selectionFeature`): `void`

This function sets a selection feature that will be disabled when
the forward ray is shown and will be reattached when hidden.
This is used to remove the selection rays when moving.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selectionFeature` | [`Nullable`](../modules.md#nullable)[`IWebXRFeature`](../interfaces/IWebXRFeature.md) | the feature to disable when forward movement is enabled |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/features/WebXRControllerTeleportation.ts:419
