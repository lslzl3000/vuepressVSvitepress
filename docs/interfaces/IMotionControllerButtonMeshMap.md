[@dev/core](../README.md) / [Exports](../modules.md) / IMotionControllerButtonMeshMap

# Interface: IMotionControllerButtonMeshMap

A helper-interface for the 3 meshes needed for controller button animation
The meshes are provided to the _lerpButtonTransform function to calculate the current position of the value mesh

## Table of contents

### Properties

- [pressedMesh](IMotionControllerButtonMeshMap.md#pressedmesh)
- [unpressedMesh](IMotionControllerButtonMeshMap.md#unpressedmesh)
- [valueMesh](IMotionControllerButtonMeshMap.md#valuemesh)

## Properties

### pressedMesh

• **pressedMesh**: [`AbstractMesh`](../classes/AbstractMesh.md)

the mesh that defines the pressed value mesh position.
This is used to find the max-position of this button

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:160

___

### unpressedMesh

• **unpressedMesh**: [`AbstractMesh`](../classes/AbstractMesh.md)

the mesh that defines the unpressed value mesh position.
This is used to find the min (or initial) position of this button

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:165

___

### valueMesh

• **valueMesh**: [`AbstractMesh`](../classes/AbstractMesh.md)

The mesh that will be changed when value changes

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:169
