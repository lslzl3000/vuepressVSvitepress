[@dev/core](../README.md) / [Exports](../modules.md) / WebXRDefaultExperienceOptions

# Class: WebXRDefaultExperienceOptions

Options for the default xr helper

## Table of contents

### Constructors

- [constructor](WebXRDefaultExperienceOptions.md#constructor)

### Properties

- [disableDefaultUI](WebXRDefaultExperienceOptions.md#disabledefaultui)
- [disableNearInteraction](WebXRDefaultExperienceOptions.md#disablenearinteraction)
- [disablePointerSelection](WebXRDefaultExperienceOptions.md#disablepointerselection)
- [disableTeleportation](WebXRDefaultExperienceOptions.md#disableteleportation)
- [floorMeshes](WebXRDefaultExperienceOptions.md#floormeshes)
- [ignoreNativeCameraTransformation](WebXRDefaultExperienceOptions.md#ignorenativecameratransformation)
- [inputOptions](WebXRDefaultExperienceOptions.md#inputoptions)
- [optionalFeatures](WebXRDefaultExperienceOptions.md#optionalfeatures)
- [outputCanvasOptions](WebXRDefaultExperienceOptions.md#outputcanvasoptions)
- [pointerSelectionOptions](WebXRDefaultExperienceOptions.md#pointerselectionoptions)
- [renderingGroupId](WebXRDefaultExperienceOptions.md#renderinggroupid)
- [uiOptions](WebXRDefaultExperienceOptions.md#uioptions)
- [useStablePlugins](WebXRDefaultExperienceOptions.md#usestableplugins)

## Constructors

### constructor

• **new WebXRDefaultExperienceOptions**()

## Properties

### disableDefaultUI

• `Optional` **disableDefaultUI**: `boolean`

Enable or disable default UI to enter XR

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRDefaultExperience.ts:25

___

### disableNearInteraction

• `Optional` **disableNearInteraction**: `boolean`

Should nearInteraction not initialize. Defaults to false.

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRDefaultExperience.ts:39

___

### disablePointerSelection

• `Optional` **disablePointerSelection**: `boolean`

Should pointer selection not initialize.
Note that disabling pointer selection also disables teleportation.
Defaults to false.

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRDefaultExperience.ts:31

___

### disableTeleportation

• `Optional` **disableTeleportation**: `boolean`

Should teleportation not initialize. Defaults to false.

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRDefaultExperience.ts:35

___

### floorMeshes

• `Optional` **floorMeshes**: [`AbstractMesh`](AbstractMesh.md)[]

Floor meshes that will be used for teleport

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRDefaultExperience.ts:43

___

### ignoreNativeCameraTransformation

• `Optional` **ignoreNativeCameraTransformation**: `boolean`

If set to true, the first frame will not be used to reset position
The first frame is mainly used when copying transformation from the old camera
Mainly used in AR

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRDefaultExperience.ts:49

___

### inputOptions

• `Optional` **inputOptions**: [`IWebXRInputOptions`](../interfaces/IWebXRInputOptions.md)

Disable the controller mesh-loading. Can be used if you want to load your own meshes

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRDefaultExperience.ts:53

___

### optionalFeatures

• `Optional` **optionalFeatures**: `boolean` \| `string`[]

A list of optional features to init the session with
If set to true, all features we support will be added

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRDefaultExperience.ts:80

___

### outputCanvasOptions

• `Optional` **outputCanvasOptions**: [`WebXRManagedOutputCanvasOptions`](WebXRManagedOutputCanvasOptions.md)

optional configuration for the output canvas

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRDefaultExperience.ts:61

___

### pointerSelectionOptions

• `Optional` **pointerSelectionOptions**: [`IWebXRControllerPointerSelectionOptions`](../interfaces/IWebXRControllerPointerSelectionOptions.md)

optional configuration for pointer selection

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRDefaultExperience.ts:57

___

### renderingGroupId

• `Optional` **renderingGroupId**: `number`

An optional rendering group id that will be set globally for teleportation, pointer selection and default controller meshes

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRDefaultExperience.ts:74

___

### uiOptions

• `Optional` **uiOptions**: [`WebXREnterExitUIOptions`](WebXREnterExitUIOptions.md)

optional UI options. This can be used among other to change session mode and reference space type

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRDefaultExperience.ts:65

___

### useStablePlugins

• `Optional` **useStablePlugins**: `boolean`

When loading teleportation and pointer select, use stable versions instead of latest.

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRDefaultExperience.ts:69
