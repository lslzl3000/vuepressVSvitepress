[@dev/core](../README.md) / [Exports](../modules.md) / WebXRHand

# Class: WebXRHand

Representing a single hand (with its corresponding native XRHand object)

## Implements

- [`IDisposable`](../interfaces/IDisposable.md)

## Table of contents

### Constructors

- [constructor](WebXRHand.md#constructor)

### Properties

- [\_jointRadii](WebXRHand.md#_jointradii)
- [\_jointTransformMatrices](WebXRHand.md#_jointtransformmatrices)
- [\_jointTransforms](WebXRHand.md#_jointtransforms)
- [\_scene](WebXRHand.md#_scene)
- [\_tempJointMatrix](WebXRHand.md#_tempjointmatrix)
- [rigMapping](WebXRHand.md#rigmapping)
- [xrController](WebXRHand.md#xrcontroller)

### Accessors

- [handMesh](WebXRHand.md#handmesh)

### Methods

- [dispose](WebXRHand.md#dispose)
- [getHandPartMeshes](WebXRHand.md#gethandpartmeshes)
- [getJointMesh](WebXRHand.md#getjointmesh)
- [setHandMesh](WebXRHand.md#sethandmesh)
- [updateFromXRFrame](WebXRHand.md#updatefromxrframe)

## Constructors

### constructor

• **new WebXRHand**(`xrController`, `_jointMeshes`, `_handMesh`, `rigMapping`, `_leftHandedMeshes?`, `_jointsInvisible?`, `_jointScaleFactor?`)

Construct a new hand object

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `xrController` | [`WebXRInputSource`](WebXRInputSource.md) | `undefined` | The controller to which the hand correlates. |
| `_jointMeshes` | [`AbstractMesh`](AbstractMesh.md)[] | `undefined` | The meshes to be used to track the hand joints. |
| `_handMesh` | [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md) | `undefined` | An optional hand mesh. |
| `rigMapping` | [`Nullable`](../modules.md#nullable)[`XRHandMeshRigMapping`](../modules.md#xrhandmeshrigmapping) | `undefined` | An optional rig mapping for the hand mesh.                    If not provided (but a hand mesh is provided),                    it will be assumed that the hand mesh's bones are named                    directly after the WebXR bone names. |
| `_leftHandedMeshes` | `boolean` | `false` | Are the hand meshes left-handed-system meshes |
| `_jointsInvisible` | `boolean` | `false` | Are the tracked joint meshes visible |
| `_jointScaleFactor` | `number` | `1` | Scale factor for all joint meshes |

#### Defined in

packages/dev/core/src/XR/features/WebXRHandTracking.ts:335

## Properties

### \_jointRadii

• `Private` **\_jointRadii**: `Float32Array`

The float array that will directly receive the joint radii from WebXR.

#### Defined in

packages/dev/core/src/XR/features/WebXRHandTracking.ts:295

___

### \_jointTransformMatrices

• `Private` **\_jointTransformMatrices**: `Float32Array`

The float array that will directly receive the transform matrix data from WebXR.

#### Defined in

packages/dev/core/src/XR/features/WebXRHandTracking.ts:288

___

### \_jointTransforms

• `Private` **\_jointTransforms**: [`TransformNode`](TransformNode.md)[]

Transform nodes that will directly receive the transforms from the WebXR matrix data.

#### Defined in

packages/dev/core/src/XR/features/WebXRHandTracking.ts:283

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/XR/features/WebXRHandTracking.ts:278

___

### \_tempJointMatrix

• `Private` **\_tempJointMatrix**: [`Matrix`](Matrix.md)

#### Defined in

packages/dev/core/src/XR/features/WebXRHandTracking.ts:290

___

### rigMapping

• `Readonly` **rigMapping**: [`Nullable`](../modules.md#nullable)[`XRHandMeshRigMapping`](../modules.md#xrhandmeshrigmapping)

#### Defined in

packages/dev/core/src/XR/features/WebXRHandTracking.ts:342

___

### xrController

• `Readonly` **xrController**: [`WebXRInputSource`](WebXRInputSource.md)

#### Defined in

packages/dev/core/src/XR/features/WebXRHandTracking.ts:337

## Accessors

### handMesh

• `get` **handMesh**(): [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

Get the hand mesh.

#### Returns

[`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

#### Defined in

packages/dev/core/src/XR/features/WebXRHandTracking.ts:300

## Methods

### dispose

▸ **dispose**(): `void`

Dispose this Hand object

#### Returns

`void`

#### Implementation of

[IDisposable](../interfaces/IDisposable.md).[dispose](../interfaces/IDisposable.md#dispose)

#### Defined in

packages/dev/core/src/XR/features/WebXRHandTracking.ts:485

___

### getHandPartMeshes

▸ **getHandPartMeshes**(`part`): [`AbstractMesh`](AbstractMesh.md)[]

Get meshes of part of the hand.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `part` | [`HandPart`](../enums/HandPart.md) | The part of hand to get. |

#### Returns

[`AbstractMesh`](AbstractMesh.md)[]

An array of meshes that correlate to the hand part requested.

#### Defined in

packages/dev/core/src/XR/features/WebXRHandTracking.ts:309

___

### getJointMesh

▸ **getJointMesh**(`jointName`): [`AbstractMesh`](AbstractMesh.md)

Retrieves a mesh linked to a named joint in the hand.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `jointName` | [`XRHandJoint`](../enums/XRHandJoint.md) | The name of the joint. |

#### Returns

[`AbstractMesh`](AbstractMesh.md)

An AbstractMesh whose position corresponds with the joint position.

#### Defined in

packages/dev/core/src/XR/features/WebXRHandTracking.ts:318

___

### setHandMesh

▸ **setHandMesh**(`handMesh`, `rigMapping`): `void`

Sets the current hand mesh to render for the WebXRHand.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `handMesh` | [`AbstractMesh`](AbstractMesh.md) | The rigged hand mesh that will be tracked to the user's hand. |
| `rigMapping` | [`Nullable`](../modules.md#nullable)[`XRHandMeshRigMapping`](../modules.md#xrhandmeshrigmapping) | The mapping from XRHandJoint to bone names to use with the mesh. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/features/WebXRHandTracking.ts:393

___

### updateFromXRFrame

▸ **updateFromXRFrame**(`xrFrame`, `referenceSpace`): `void`

Update this hand from the latest xr frame.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `xrFrame` | `XRFrame` | The latest frame received from WebXR. |
| `referenceSpace` | `XRReferenceSpace` | The current viewer reference space. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/XR/features/WebXRHandTracking.ts:417
