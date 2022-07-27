[@dev/core](../README.md) / [Exports](../modules.md) / IWebXRControllerMovementOptions

# Interface: IWebXRControllerMovementOptions

The options container for the controller movement module

## Table of contents

### Properties

- [customRegistrationConfigurations](IWebXRControllerMovementOptions.md#customregistrationconfigurations)
- [movementEnabled](IWebXRControllerMovementOptions.md#movementenabled)
- [movementOrientationFollowsViewerPose](IWebXRControllerMovementOptions.md#movementorientationfollowsviewerpose)
- [movementSpeed](IWebXRControllerMovementOptions.md#movementspeed)
- [movementThreshold](IWebXRControllerMovementOptions.md#movementthreshold)
- [rotationEnabled](IWebXRControllerMovementOptions.md#rotationenabled)
- [rotationSpeed](IWebXRControllerMovementOptions.md#rotationspeed)
- [rotationThreshold](IWebXRControllerMovementOptions.md#rotationthreshold)
- [xrInput](IWebXRControllerMovementOptions.md#xrinput)

## Properties

### customRegistrationConfigurations

• `Optional` **customRegistrationConfigurations**: [`WebXRControllerMovementRegistrationConfiguration`](../modules.md#webxrcontrollermovementregistrationconfiguration)[]

Override default behaviour and provide your own movement controls

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerMovement.ts:21

___

### movementEnabled

• `Optional` **movementEnabled**: `boolean`

Is movement enabled

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerMovement.ts:25

___

### movementOrientationFollowsViewerPose

• **movementOrientationFollowsViewerPose**: `boolean`

Camera direction follows view pose and movement by default will move independently of the viewer's pose.

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerMovement.ts:29

___

### movementSpeed

• `Optional` **movementSpeed**: `number`

Movement speed factor (default is 1.0)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerMovement.ts:33

___

### movementThreshold

• `Optional` **movementThreshold**: `number`

Minimum threshold the controller's thumbstick/touchpad must pass before being recognized for movement (avoids jitter/unintentional movement)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerMovement.ts:37

___

### rotationEnabled

• `Optional` **rotationEnabled**: `boolean`

Is rotation enabled

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerMovement.ts:41

___

### rotationSpeed

• `Optional` **rotationSpeed**: `number`

Movement speed factor (default is 1.0)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerMovement.ts:49

___

### rotationThreshold

• `Optional` **rotationThreshold**: `number`

Minimum threshold the controller's thumstick/touchpad must pass before being recognized for rotation (avoids jitter/unintentional rotation)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerMovement.ts:45

___

### xrInput

• **xrInput**: [`WebXRInput`](../classes/WebXRInput.md)

Babylon XR Input class for controller

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerMovement.ts:53
