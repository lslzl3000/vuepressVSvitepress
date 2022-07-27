[@dev/core](../README.md) / [Exports](../modules.md) / IWebXRPlane

# Interface: IWebXRPlane

A babylon interface for a WebXR plane.
A Plane is actually a polygon, built from N points in space

Supported in chrome 79, not supported in canary 81 ATM

## Table of contents

### Properties

- [id](IWebXRPlane.md#id)
- [polygonDefinition](IWebXRPlane.md#polygondefinition)
- [transformationMatrix](IWebXRPlane.md#transformationmatrix)
- [xrPlane](IWebXRPlane.md#xrplane)

## Properties

### id

• **id**: `number`

a babylon-assigned ID for this polygon

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRPlaneDetector.ts:39

___

### polygonDefinition

• **polygonDefinition**: [`Vector3`](../classes/Vector3.md)[]

an array of vector3 points in babylon space. right/left hand system is taken into account.

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRPlaneDetector.ts:43

___

### transformationMatrix

• **transformationMatrix**: [`Matrix`](../classes/Matrix.md)

A transformation matrix to apply on the mesh that will be built using the polygonDefinition
Local vs. World are decided if worldParentNode was provided or not in the options when constructing the module

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRPlaneDetector.ts:48

___

### xrPlane

• **xrPlane**: `XRPlane`

the native xr-plane object

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRPlaneDetector.ts:52
