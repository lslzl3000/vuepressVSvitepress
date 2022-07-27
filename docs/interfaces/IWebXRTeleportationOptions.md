[@dev/core](../README.md) / [Exports](../modules.md) / IWebXRTeleportationOptions

# Interface: IWebXRTeleportationOptions

The options container for the teleportation module

## Table of contents

### Properties

- [customUtilityLayerScene](IWebXRTeleportationOptions.md#customutilitylayerscene)
- [defaultTargetMeshOptions](IWebXRTeleportationOptions.md#defaulttargetmeshoptions)
- [floorMeshes](IWebXRTeleportationOptions.md#floormeshes)
- [forceHandedness](IWebXRTeleportationOptions.md#forcehandedness)
- [generateRayPathMesh](IWebXRTeleportationOptions.md#generateraypathmesh)
- [pickBlockerMeshes](IWebXRTeleportationOptions.md#pickblockermeshes)
- [renderingGroupId](IWebXRTeleportationOptions.md#renderinggroupid)
- [snapPointsOnly](IWebXRTeleportationOptions.md#snappointsonly)
- [snapPositions](IWebXRTeleportationOptions.md#snappositions)
- [snapToPositionRadius](IWebXRTeleportationOptions.md#snaptopositionradius)
- [teleportationTargetMesh](IWebXRTeleportationOptions.md#teleportationtargetmesh)
- [timeToTeleport](IWebXRTeleportationOptions.md#timetoteleport)
- [useMainComponentOnly](IWebXRTeleportationOptions.md#usemaincomponentonly)
- [useUtilityLayer](IWebXRTeleportationOptions.md#useutilitylayer)
- [xrInput](IWebXRTeleportationOptions.md#xrinput)

## Properties

### customUtilityLayerScene

• `Optional` **customUtilityLayerScene**: [`Scene`](../classes/Scene.md)

if provided, this scene will be used to render meshes.

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerTeleportation.ts:41

___

### defaultTargetMeshOptions

• `Optional` **defaultTargetMeshOptions**: `Object`

Values to configure the default target mesh

#### Type declaration

| Name | Type | Description |
| :------ | :------ | :------ |
| `disableAnimation?` | `boolean` | Disable the mesh's animation sequence |
| `disableLighting?` | `boolean` | Disable lighting on the material or the ring and arrow |
| `teleportationBorderColor?` | `string` | Border color for the teleportation area |
| `teleportationFillColor?` | `string` | Fill color of the teleportation area |
| `torusArrowMaterial?` | [`Material`](../classes/Material.md) | Override the default material of the torus and arrow |

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerTeleportation.ts:45

___

### floorMeshes

• `Optional` **floorMeshes**: [`AbstractMesh`](../classes/AbstractMesh.md)[]

A list of meshes to use as floor meshes.
Meshes can be added and removed after initializing the feature using the
addFloorMesh and removeFloorMesh functions
If empty, rotation will still work

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerTeleportation.ts:73

___

### forceHandedness

• `Optional` **forceHandedness**: `XRHandedness`

Should teleport work only on a specific hand?

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerTeleportation.ts:125

___

### generateRayPathMesh

• `Optional` **generateRayPathMesh**: (`points`: [`Vector3`](../classes/Vector3.md)[], `pickingInfo`: [`PickingInfo`](../classes/PickingInfo.md)) => [`AbstractMesh`](../classes/AbstractMesh.md)

#### Type declaration

▸ (`points`, `pickingInfo`): [`AbstractMesh`](../classes/AbstractMesh.md)

If provided, this function will be used to generate the ray mesh instead of the lines mesh being used per default

##### Parameters

| Name | Type |
| :------ | :------ |
| `points` | [`Vector3`](../classes/Vector3.md)[] |
| `pickingInfo` | [`PickingInfo`](../classes/PickingInfo.md) |

##### Returns

[`AbstractMesh`](../classes/AbstractMesh.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerTeleportation.ts:130

___

### pickBlockerMeshes

• `Optional` **pickBlockerMeshes**: [`AbstractMesh`](../classes/AbstractMesh.md)[]

Meshes that the teleportation ray cannot go through

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerTeleportation.ts:120

___

### renderingGroupId

• `Optional` **renderingGroupId**: `number`

use this rendering group id for the meshes (optional)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerTeleportation.ts:77

___

### snapPointsOnly

• `Optional` **snapPointsOnly**: `boolean`

Should teleportation move only to snap points

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerTeleportation.ts:81

___

### snapPositions

• `Optional` **snapPositions**: [`Vector3`](../classes/Vector3.md)[]

An array of points to which the teleportation will snap to.
If the teleportation ray is in the proximity of one of those points, it will be corrected to this point.

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerTeleportation.ts:86

___

### snapToPositionRadius

• `Optional` **snapToPositionRadius**: `number`

How close should the teleportation ray be in order to snap to position.
Default to 0.8 units (meters)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerTeleportation.ts:91

___

### teleportationTargetMesh

• `Optional` **teleportationTargetMesh**: [`AbstractMesh`](../classes/AbstractMesh.md)

Provide your own teleportation mesh instead of babylon's wonderful doughnut.
If you want to support rotation, make sure your mesh has a direction indicator.

When left untouched, the default mesh will be initialized.

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerTeleportation.ts:98

___

### timeToTeleport

• `Optional` **timeToTeleport**: `number`

If main component is used (no thumbstick), how long should the "long press" take before teleport

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerTeleportation.ts:102

___

### useMainComponentOnly

• `Optional` **useMainComponentOnly**: `boolean`

Disable using the thumbstick and use the main component (usually trigger) on long press.
This will be automatically true if the controller doesn't have a thumbstick or touchpad.

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerTeleportation.ts:107

___

### useUtilityLayer

• `Optional` **useUtilityLayer**: `boolean`

Should meshes created here be added to a utility layer or the main scene

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerTeleportation.ts:111

___

### xrInput

• **xrInput**: [`WebXRInput`](../classes/WebXRInput.md)

Babylon XR Input class for controller

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerTeleportation.ts:115
