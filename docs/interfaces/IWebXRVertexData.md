[@dev/core](../README.md) / [Exports](../modules.md) / IWebXRVertexData

# Interface: IWebXRVertexData

A babylon interface for a XR mesh's vertex data.

Currently not supported by WebXR, available only with BabylonNative

## Table of contents

### Properties

- [id](IWebXRVertexData.md#id)
- [indices](IWebXRVertexData.md#indices)
- [normals](IWebXRVertexData.md#normals)
- [positions](IWebXRVertexData.md#positions)
- [transformationMatrix](IWebXRVertexData.md#transformationmatrix)
- [worldParentNode](IWebXRVertexData.md#worldparentnode)
- [xrMesh](IWebXRVertexData.md#xrmesh)

## Properties

### id

• **id**: `number`

A babylon-assigned ID for this mesh

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRMeshDetector.ts:42

___

### indices

• `Optional` **indices**: `Uint32Array`

An array of indices in babylon space. Indices have a counterclockwise winding order.
Indices will only be populated if convertCoordinateSystems is set to true in the IWebXRMeshDetectorOptions.

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRMeshDetector.ts:61

___

### normals

• `Optional` **normals**: `Float32Array`

An array of vertex normals in babylon space. right/left hand system is taken into account.
Normals will not be calculated if convertCoordinateSystems is undefined in the IWebXRMeshDetectorOptions.
Different platforms may or may not support mesh normals when convertCoordinateSystems is set to true.

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRMeshDetector.ts:67

___

### positions

• `Optional` **positions**: `Float32Array`

An array of vertex positions in babylon space. right/left hand system is taken into account.
Positions will only be calculated if convertCoordinateSystems is set to true in the IWebXRMeshDetectorOptions.

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRMeshDetector.ts:56

___

### transformationMatrix

• `Optional` **transformationMatrix**: [`Matrix`](../classes/Matrix.md)

A transformation matrix to apply on the mesh that will be built using the meshDefinition.
Local vs. World are decided if worldParentNode was provided or not in the options when constructing the module.
TransformationMatrix will only be calculated if convertCoordinateSystems is set to true in the IWebXRMeshDetectorOptions.

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRMeshDetector.ts:73

___

### worldParentNode

• `Optional` **worldParentNode**: [`TransformNode`](../classes/TransformNode.md)

The node to use to transform the local results to world coordinates.
WorldParentNode will only exist if it was declared in the IWebXRMeshDetectorOptions.

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRMeshDetector.ts:51

___

### xrMesh

• **xrMesh**: `XRMesh`

Data required for constructing a mesh in Babylon.js.

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRMeshDetector.ts:46
