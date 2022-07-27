[@dev/core](../README.md) / [Exports](../modules.md) / IWebXRWalkingLocomotionOptions

# Interface: IWebXRWalkingLocomotionOptions

Options for the walking locomotion feature.

## Table of contents

### Properties

- [locomotionTarget](IWebXRWalkingLocomotionOptions.md#locomotiontarget)

## Properties

### locomotionTarget

• **locomotionTarget**: [`TransformNode`](../classes/TransformNode.md) \| [`WebXRCamera`](../classes/WebXRCamera.md)

The target to be moved by walking locomotion. This should be the transform node
which is the root of the XR space (i.e., the WebXRCamera's parent node). However,
for simple cases and legacy purposes, articulating the WebXRCamera itself is also
supported as a deprecated feature.

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRWalkingLocomotion.ts:339
