[@dev/core](../README.md) / [Exports](../modules.md) / VRExperienceHelperOptions

# Interface: VRExperienceHelperOptions

Options to modify the vr experience helper's behavior.

## Hierarchy

- [`WebVROptions`](WebVROptions.md)

  ↳ **`VRExperienceHelperOptions`**

## Table of contents

### Properties

- [controllerMeshes](VRExperienceHelperOptions.md#controllermeshes)
- [createDeviceOrientationCamera](VRExperienceHelperOptions.md#createdeviceorientationcamera)
- [createFallbackVRDeviceOrientationFreeCamera](VRExperienceHelperOptions.md#createfallbackvrdeviceorientationfreecamera)
- [customVRButton](VRExperienceHelperOptions.md#customvrbutton)
- [defaultHeight](VRExperienceHelperOptions.md#defaultheight)
- [defaultLightingOnControllers](VRExperienceHelperOptions.md#defaultlightingoncontrollers)
- [displayName](VRExperienceHelperOptions.md#displayname)
- [floorMeshes](VRExperienceHelperOptions.md#floormeshes)
- [laserToggle](VRExperienceHelperOptions.md#lasertoggle)
- [positionScale](VRExperienceHelperOptions.md#positionscale)
- [rayLength](VRExperienceHelperOptions.md#raylength)
- [trackPosition](VRExperienceHelperOptions.md#trackposition)
- [useCustomVRButton](VRExperienceHelperOptions.md#usecustomvrbutton)
- [useMultiview](VRExperienceHelperOptions.md#usemultiview)
- [useXR](VRExperienceHelperOptions.md#usexr)
- [vrDeviceOrientationCameraMetrics](VRExperienceHelperOptions.md#vrdeviceorientationcamerametrics)

## Properties

### controllerMeshes

• `Optional` **controllerMeshes**: `boolean`

Should the native controller meshes be initialized. (default: true)

#### Inherited from

[WebVROptions](WebVROptions.md).[controllerMeshes](WebVROptions.md#controllermeshes)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/webVRCamera.ts:123

___

### createDeviceOrientationCamera

• `Optional` **createDeviceOrientationCamera**: `boolean`

Create a DeviceOrientationCamera to be used as your out of vr camera. (default: true)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:83

___

### createFallbackVRDeviceOrientationFreeCamera

• `Optional` **createFallbackVRDeviceOrientationFreeCamera**: `boolean`

Create a VRDeviceOrientationFreeCamera to be used for VR when no external HMD is found. (default: true)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:87

___

### customVRButton

• `Optional` **customVRButton**: `HTMLButtonElement`

If you'd like to provide your own button to the VRHelper. (default: standard babylon vr button)

#### Inherited from

[WebVROptions](WebVROptions.md).[customVRButton](WebVROptions.md#customvrbutton)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/webVRCamera.ts:136

___

### defaultHeight

• `Optional` **defaultHeight**: `number`

To change the default offset from the ground to account for user's height in meters. Will be scaled by positionScale. (default: 1.7)

#### Inherited from

[WebVROptions](WebVROptions.md).[defaultHeight](WebVROptions.md#defaultheight)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/webVRCamera.ts:146

___

### defaultLightingOnControllers

• `Optional` **defaultLightingOnControllers**: `boolean`

Creating a default HemiLight only on controllers. (default: true)

#### Inherited from

[WebVROptions](WebVROptions.md).[defaultLightingOnControllers](WebVROptions.md#defaultlightingoncontrollers)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/webVRCamera.ts:127

___

### displayName

• `Optional` **displayName**: `string`

If there are more than one VRDisplays, this will choose the display matching this name. (default: pick first vrDisplay)

#### Inherited from

[WebVROptions](WebVROptions.md).[displayName](WebVROptions.md#displayname)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/webVRCamera.ts:119

___

### floorMeshes

• `Optional` **floorMeshes**: [`Mesh`](../classes/Mesh.md)[]

A list of meshes to be used as the teleportation floor. If specified, teleportation will be enabled (default: undefined)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:95

___

### laserToggle

• `Optional` **laserToggle**: `boolean`

Uses the main button on the controller to toggle the laser casted. (default: true)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:91

___

### positionScale

• `Optional` **positionScale**: `number`

Sets the scale of the vrDevice in babylon space. (default: 1)

#### Inherited from

[WebVROptions](WebVROptions.md).[positionScale](WebVROptions.md#positionscale)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/webVRCamera.ts:115

___

### rayLength

• `Optional` **rayLength**: `number`

To change the length of the ray for gaze/controllers. Will be scaled by positionScale. (default: 100)

#### Inherited from

[WebVROptions](WebVROptions.md).[rayLength](WebVROptions.md#raylength)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/webVRCamera.ts:141

___

### trackPosition

• `Optional` **trackPosition**: `boolean`

Sets if the webVR camera should be tracked to the vrDevice. (default: true)

#### Inherited from

[WebVROptions](WebVROptions.md).[trackPosition](WebVROptions.md#trackposition)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/webVRCamera.ts:111

___

### useCustomVRButton

• `Optional` **useCustomVRButton**: `boolean`

If you don't want to use the default VR button of the helper. (default: false)

#### Inherited from

[WebVROptions](WebVROptions.md).[useCustomVRButton](WebVROptions.md#usecustomvrbutton)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/webVRCamera.ts:131

___

### useMultiview

• `Optional` **useMultiview**: `boolean`

If multiview should be used if available (default: false)

#### Inherited from

[WebVROptions](WebVROptions.md).[useMultiview](WebVROptions.md#usemultiview)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/webVRCamera.ts:151

___

### useXR

• `Optional` **useXR**: `boolean`

Defines if WebXR should be used instead of WebVR (if available)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:103

___

### vrDeviceOrientationCameraMetrics

• `Optional` **vrDeviceOrientationCameraMetrics**: [`VRCameraMetrics`](../classes/VRCameraMetrics.md)

Distortion metrics for the fallback vrDeviceOrientationCamera (default: VRCameraMetrics.Default)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:99
