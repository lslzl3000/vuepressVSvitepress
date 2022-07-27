[@dev/core](../README.md) / [Exports](../modules.md) / IWebXRHandTrackingOptions

# Interface: IWebXRHandTrackingOptions

Configuration interface for the hand tracking feature

## Table of contents

### Properties

- [handMeshes](IWebXRHandTrackingOptions.md#handmeshes)
- [jointMeshes](IWebXRHandTrackingOptions.md#jointmeshes)
- [xrInput](IWebXRHandTrackingOptions.md#xrinput)

## Properties

### handMeshes

• `Optional` **handMeshes**: `Object`

Configuration object for the hand meshes.

#### Type declaration

| Name | Type | Description |
| :------ | :------ | :------ |
| `customColors?` | { `base?`: [`Color3`](../classes/Color3.md) ; `fingerColor?`: [`Color3`](../classes/Color3.md) ; `fresnel?`: [`Color3`](../classes/Color3.md) ; `tipFresnel?`: [`Color3`](../classes/Color3.md)  } | Override the colors of the hand meshes. |
| `customColors.base?` | [`Color3`](../classes/Color3.md) | - |
| `customColors.fingerColor?` | [`Color3`](../classes/Color3.md) | - |
| `customColors.fresnel?` | [`Color3`](../classes/Color3.md) | - |
| `customColors.tipFresnel?` | [`Color3`](../classes/Color3.md) | - |
| `customMeshes?` | { `left`: [`AbstractMesh`](../classes/AbstractMesh.md) ; `right`: [`AbstractMesh`](../classes/AbstractMesh.md)  } | Rigged hand meshes that will be tracked to the user's hands. This will override the default hand mesh. |
| `customMeshes.left` | [`AbstractMesh`](../classes/AbstractMesh.md) | - |
| `customMeshes.right` | [`AbstractMesh`](../classes/AbstractMesh.md) | - |
| `customRigMappings?` | { `left`: [`XRHandMeshRigMapping`](../modules.md#xrhandmeshrigmapping) ; `right`: [`XRHandMeshRigMapping`](../modules.md#xrhandmeshrigmapping)  } | If a hand mesh was provided, this array will define what axis will update which node. This will override the default hand mesh |
| `customRigMappings.left` | [`XRHandMeshRigMapping`](../modules.md#xrhandmeshrigmapping) | - |
| `customRigMappings.right` | [`XRHandMeshRigMapping`](../modules.md#xrhandmeshrigmapping) | - |
| `disableDefaultMeshes?` | `boolean` | Should the default hand mesh be disabled. In this case, the spheres will be visible (unless set invisible). |
| `meshesUseLeftHandedCoordinates?` | `boolean` | Are the meshes prepared for a left-handed system. Default hand meshes are right-handed. |

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHandTracking.ts:82

___

### jointMeshes

• `Optional` **jointMeshes**: `Object`

Configuration object for the joint meshes.

#### Type declaration

| Name | Type | Description |
| :------ | :------ | :------ |
| `enablePhysics?` | `boolean` | Should each instance have its own physics impostor |
| `invisible?` | `boolean` | Should the meshes created be invisible (defaults to false). |
| `keepOriginalVisible?` | `boolean` | Should the source mesh stay visible (defaults to false). |
| `onHandJointMeshGenerated?` | (`meshInstance`: [`InstancedMesh`](../classes/InstancedMesh.md), `jointId`: `number`, `hand`: `XRHandedness`) => `undefined` \| [`AbstractMesh`](../classes/AbstractMesh.md) | This function will be called after a mesh was created for a specific joint.  Using this function you can either manipulate the instance or return a new mesh.  When returning a new mesh the instance created before will be disposed. |
| `physicsProps?` | { `friction?`: `number` ; `impostorType?`: `number` ; `restitution?`: `number`  } | If enabled, override default physics properties |
| `physicsProps.friction?` | `number` | - |
| `physicsProps.impostorType?` | `number` | - |
| `physicsProps.restitution?` | `number` | - |
| `scaleFactor?` | `number` | Scale factor for all joint meshes (defaults to 1) |
| `sourceMesh?` | [`Mesh`](../classes/Mesh.md) | A source mesh to be used to create instances. Defaults to an icosphere with two subdivisions and smooth lighting.  This mesh will be the source for all other (25) meshes.  It should have the general size of a single unit, as the instances will be scaled according to the provided radius. |

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHandTracking.ts:41

___

### xrInput

• **xrInput**: [`WebXRInput`](../classes/WebXRInput.md)

The xrInput that will be used as source for new hands

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRHandTracking.ts:36
