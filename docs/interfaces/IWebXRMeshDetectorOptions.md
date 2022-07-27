[@dev/core](../README.md) / [Exports](../modules.md) / IWebXRMeshDetectorOptions

# Interface: IWebXRMeshDetectorOptions

Options used in the mesh detector module

## Table of contents

### Properties

- [convertCoordinateSystems](IWebXRMeshDetectorOptions.md#convertcoordinatesystems)
- [doNotRemoveMeshesOnSessionEnded](IWebXRMeshDetectorOptions.md#donotremovemeshesonsessionended)
- [preferredDetectorOptions](IWebXRMeshDetectorOptions.md#preferreddetectoroptions)
- [worldParentNode](IWebXRMeshDetectorOptions.md#worldparentnode)

## Properties

### convertCoordinateSystems

• `Optional` **convertCoordinateSystems**: `boolean`

If set to true, WebXRMeshDetector will convert coordinate systems for meshes.
If not defined, mesh conversions from right handed to left handed coordinate systems won't be conducted.
Right handed mesh data will be available through IWebXRVertexData.xrMesh.

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRMeshDetector.ts:30

___

### doNotRemoveMeshesOnSessionEnded

• `Optional` **doNotRemoveMeshesOnSessionEnded**: `boolean`

If set to true a reference of the created meshes will be kept until the next session starts
If not defined, meshes will be removed from the array when the feature is detached or the session ended.

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRMeshDetector.ts:20

___

### preferredDetectorOptions

• `Optional` **preferredDetectorOptions**: `XRGeometryDetectorOptions`

Preferred detector configuration, not all preferred options will be supported by all platforms.

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRMeshDetector.ts:24

___

### worldParentNode

• `Optional` **worldParentNode**: [`TransformNode`](../classes/TransformNode.md)

The node to use to transform the local results to world coordinates

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRMeshDetector.ts:15
