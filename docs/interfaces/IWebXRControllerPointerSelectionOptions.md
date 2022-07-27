[@dev/core](../README.md) / [Exports](../modules.md) / IWebXRControllerPointerSelectionOptions

# Interface: IWebXRControllerPointerSelectionOptions

Options interface for the pointer selection module

## Table of contents

### Properties

- [customLasterPointerMeshGenerator](IWebXRControllerPointerSelectionOptions.md#customlasterpointermeshgenerator)
- [customSelectionMeshGenerator](IWebXRControllerPointerSelectionOptions.md#customselectionmeshgenerator)
- [customUtilityLayerScene](IWebXRControllerPointerSelectionOptions.md#customutilitylayerscene)
- [disablePointerUpOnTouchOut](IWebXRControllerPointerSelectionOptions.md#disablepointerupontouchout)
- [disableScenePointerVectorUpdate](IWebXRControllerPointerSelectionOptions.md#disablescenepointervectorupdate)
- [disableSwitchOnClick](IWebXRControllerPointerSelectionOptions.md#disableswitchonclick)
- [enablePointerSelectionOnAllControllers](IWebXRControllerPointerSelectionOptions.md#enablepointerselectiononallcontrollers)
- [forceGazeMode](IWebXRControllerPointerSelectionOptions.md#forcegazemode)
- [gazeCamera](IWebXRControllerPointerSelectionOptions.md#gazecamera)
- [gazeModePointerMovedFactor](IWebXRControllerPointerSelectionOptions.md#gazemodepointermovedfactor)
- [maxPointerDistance](IWebXRControllerPointerSelectionOptions.md#maxpointerdistance)
- [overrideButtonId](IWebXRControllerPointerSelectionOptions.md#overridebuttonid)
- [preferredHandedness](IWebXRControllerPointerSelectionOptions.md#preferredhandedness)
- [renderingGroupId](IWebXRControllerPointerSelectionOptions.md#renderinggroupid)
- [timeToSelect](IWebXRControllerPointerSelectionOptions.md#timetoselect)
- [useUtilityLayer](IWebXRControllerPointerSelectionOptions.md#useutilitylayer)
- [xrInput](IWebXRControllerPointerSelectionOptions.md#xrinput)

## Properties

### customLasterPointerMeshGenerator

• `Optional` **customLasterPointerMeshGenerator**: () => [`AbstractMesh`](../classes/AbstractMesh.md)

#### Type declaration

▸ (): [`AbstractMesh`](../classes/AbstractMesh.md)

A function that will be called when a new laser pointer mesh is generated.
This function should return a mesh that will be used as the laser pointer mesh.
The height (y) of the mesh must be 1.

##### Returns

[`AbstractMesh`](../classes/AbstractMesh.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:121

___

### customSelectionMeshGenerator

• `Optional` **customSelectionMeshGenerator**: () => [`Mesh`](../classes/Mesh.md)

#### Type declaration

▸ (): [`Mesh`](../classes/Mesh.md)

A function that will be called when a new selection mesh is generated.
This function should return a mesh that will be used as the selection mesh.
The default is a torus with a 0.01 diameter and 0.0075 thickness .

##### Returns

[`Mesh`](../classes/Mesh.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:114

___

### customUtilityLayerScene

• `Optional` **customUtilityLayerScene**: [`Scene`](../classes/Scene.md)

if provided, this scene will be used to render meshes.

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:34

___

### disablePointerUpOnTouchOut

• **disablePointerUpOnTouchOut**: `boolean`

Disable the pointer up event when the xr controller in screen and gaze mode is disposed (meaning - when the user removed the finger from the screen)
If not disabled, the last picked point will be used to execute a pointer up event
If disabled, pointer up event will be triggered right after the pointer down event.
Used in screen and gaze target ray mode only

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:41

___

### disableScenePointerVectorUpdate

• **disableScenePointerVectorUpdate**: `boolean`

Should the scene pointerX and pointerY update be disabled
This is required for fullscreen AR GUI, but might slow down other experiences.
Disable in VR, if not needed.
The first rig camera (left eye) will be used to calculate the projection

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:85

___

### disableSwitchOnClick

• `Optional` **disableSwitchOnClick**: `boolean`

Disable switching the pointer selection from one controller to the other.
If the preferred hand is set it will be fixed on this hand, and if not it will be fixed on the first controller added to the scene

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:102

___

### enablePointerSelectionOnAllControllers

• `Optional` **enablePointerSelectionOnAllControllers**: `boolean`

Enable pointer selection on all controllers instead of switching between them

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:90

___

### forceGazeMode

• **forceGazeMode**: `boolean`

For gaze mode for tracked-pointer / controllers (time to select instead of button press)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:45

___

### gazeCamera

• `Optional` **gazeCamera**: [`WebXRCamera`](../classes/WebXRCamera.md)

Optional WebXR camera to be used for gaze selection

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:73

___

### gazeModePointerMovedFactor

• `Optional` **gazeModePointerMovedFactor**: `number`

Factor to be applied to the pointer-moved function in the gaze mode. How sensitive should the gaze mode be when checking if the pointer moved
to start a new countdown to the pointer down event.
Defaults to 1.

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:51

___

### maxPointerDistance

• `Optional` **maxPointerDistance**: `number`

The maximum distance of the pointer selection feature. Defaults to 100.

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:107

___

### overrideButtonId

• `Optional` **overrideButtonId**: `string`

Different button type to use instead of the main component

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:55

___

### preferredHandedness

• `Optional` **preferredHandedness**: `XRHandedness`

The preferred hand to give the pointer selection to. This will be prioritized when the controller initialize.
If switch is enabled, it will still allow the user to switch between the different controllers

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:96

___

### renderingGroupId

• `Optional` **renderingGroupId**: `number`

use this rendering group id for the meshes (optional)

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:59

___

### timeToSelect

• `Optional` **timeToSelect**: `number`

The amount of time in milliseconds it takes between pick found something to a pointer down event.
Used in gaze modes. Tracked pointer uses the trigger, screen uses touch events
3000 means 3 seconds between pointing at something and selecting it

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:65

___

### useUtilityLayer

• `Optional` **useUtilityLayer**: `boolean`

Should meshes created here be added to a utility layer or the main scene

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:69

___

### xrInput

• **xrInput**: [`WebXRInput`](../classes/WebXRInput.md)

the xr input to use with this pointer selection

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRControllerPointerSelection.ts:77
