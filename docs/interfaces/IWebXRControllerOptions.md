[@dev/core](../README.md) / [Exports](../modules.md) / IWebXRControllerOptions

# Interface: IWebXRControllerOptions

Configuration options for the WebXR controller creation

## Table of contents

### Properties

- [disableMotionControllerAnimation](IWebXRControllerOptions.md#disablemotioncontrolleranimation)
- [doNotLoadControllerMesh](IWebXRControllerOptions.md#donotloadcontrollermesh)
- [forceControllerProfile](IWebXRControllerOptions.md#forcecontrollerprofile)
- [renderingGroupId](IWebXRControllerOptions.md#renderinggroupid)

## Properties

### disableMotionControllerAnimation

• `Optional` **disableMotionControllerAnimation**: `boolean`

Should the controller mesh be animated when a user interacts with it
The pressed buttons / thumbstick and touchpad animations will be disabled

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRInputSource.ts:21

___

### doNotLoadControllerMesh

• `Optional` **doNotLoadControllerMesh**: `boolean`

Do not load the controller mesh, in case a different mesh needs to be loaded.

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRInputSource.ts:25

___

### forceControllerProfile

• `Optional` **forceControllerProfile**: `string`

Force a specific controller type for this controller.
This can be used when creating your own profile or when testing different controllers

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRInputSource.ts:30

___

### renderingGroupId

• `Optional` **renderingGroupId**: `number`

Defines a rendering group ID for meshes that will be loaded.
This is for the default controllers only.

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRInputSource.ts:35
