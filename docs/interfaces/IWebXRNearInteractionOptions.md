[@dev/core](../README.md) / [Exports](../modules.md) / IWebXRNearInteractionOptions

# Interface: IWebXRNearInteractionOptions

Options interface for the near interaction module

## Table of contents

### Properties

- [customUtilityLayerScene](IWebXRNearInteractionOptions.md#customutilitylayerscene)
- [disableSwitchOnClick](IWebXRNearInteractionOptions.md#disableswitchonclick)
- [enableNearInteractionOnAllControllers](IWebXRNearInteractionOptions.md#enablenearinteractiononallcontrollers)
- [farInteractionFeature](IWebXRNearInteractionOptions.md#farinteractionfeature)
- [motionControllerOrbMaterial](IWebXRNearInteractionOptions.md#motioncontrollerorbmaterial)
- [nearInteractionControllerMode](IWebXRNearInteractionOptions.md#nearinteractioncontrollermode)
- [preferredHandedness](IWebXRNearInteractionOptions.md#preferredhandedness)
- [useUtilityLayer](IWebXRNearInteractionOptions.md#useutilitylayer)
- [xrInput](IWebXRNearInteractionOptions.md#xrinput)

## Properties

### customUtilityLayerScene

• `Optional` **customUtilityLayerScene**: [`Scene`](../classes/Scene.md)

If provided, this scene will be used to render meshes.

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:95

___

### disableSwitchOnClick

• `Optional` **disableSwitchOnClick**: `boolean`

Disable switching the near interaction from one controller to the other.
If the preferred hand is set it will be fixed on this hand, and if not it will be fixed on the first controller added to the scene

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:117

___

### enableNearInteractionOnAllControllers

• `Optional` **enableNearInteractionOnAllControllers**: `boolean`

Enable near interaction on all controllers instead of switching between them

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:107

___

### farInteractionFeature

• `Optional` **farInteractionFeature**: [`WebXRControllerPointerSelection`](../classes/WebXRControllerPointerSelection.md)

Far interaction feature to toggle when near interaction takes precedence

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:122

___

### motionControllerOrbMaterial

• `Optional` **motionControllerOrbMaterial**: [`Material`](../classes/Material.md)

Optional material for the motion controller orb, if enabled

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:132

___

### nearInteractionControllerMode

• `Optional` **nearInteractionControllerMode**: [`WebXRNearControllerMode`](../enums/WebXRNearControllerMode.md)

Near interaction mode for motion controllers

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:127

___

### preferredHandedness

• `Optional` **preferredHandedness**: `XRHandedness`

The preferred hand to give the near interaction to. This will be prioritized when the controller initialize.
If switch is enabled, it will still allow the user to switch between the different controllers

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:112

___

### useUtilityLayer

• `Optional` **useUtilityLayer**: `boolean`

Should meshes created here be added to a utility layer or the main scene

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:99

___

### xrInput

• **xrInput**: [`WebXRInput`](../classes/WebXRInput.md)

The xr input to use with this near interaction

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRNearInteraction.ts:103
