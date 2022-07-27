[@dev/core](../README.md) / [Exports](../modules.md) / IMotionControllerMeshMap

# Interface: IMotionControllerMeshMap

A helper-interface for the 3 meshes needed for controller axis animation.
This will be expanded when touchpad animations are fully supported
The meshes are provided to the _lerpAxisTransform function to calculate the current position of the value mesh

## Table of contents

### Properties

- [maxMesh](IMotionControllerMeshMap.md#maxmesh)
- [minMesh](IMotionControllerMeshMap.md#minmesh)
- [valueMesh](IMotionControllerMeshMap.md#valuemesh)

## Properties

### maxMesh

• `Optional` **maxMesh**: [`AbstractMesh`](../classes/AbstractMesh.md)

the mesh that defines the maximum value mesh position.

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:181

___

### minMesh

• `Optional` **minMesh**: [`AbstractMesh`](../classes/AbstractMesh.md)

the mesh that defines the minimum value mesh position.

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:185

___

### valueMesh

• `Optional` **valueMesh**: [`AbstractMesh`](../classes/AbstractMesh.md)

The mesh that will be changed when axis value changes

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:189
