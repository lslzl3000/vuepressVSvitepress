[@dev/core](../README.md) / [Exports](../modules.md) / WebVROptions

# Interface: WebVROptions

Set of options to customize the webVRCamera

## Hierarchy

- **`WebVROptions`**

  ↳ [`VRExperienceHelperOptions`](VRExperienceHelperOptions.md)

## Table of contents

### Properties

- [controllerMeshes](WebVROptions.md#controllermeshes)
- [customVRButton](WebVROptions.md#customvrbutton)
- [defaultHeight](WebVROptions.md#defaultheight)
- [defaultLightingOnControllers](WebVROptions.md#defaultlightingoncontrollers)
- [displayName](WebVROptions.md#displayname)
- [positionScale](WebVROptions.md#positionscale)
- [rayLength](WebVROptions.md#raylength)
- [trackPosition](WebVROptions.md#trackposition)
- [useCustomVRButton](WebVROptions.md#usecustomvrbutton)
- [useMultiview](WebVROptions.md#usemultiview)

## Properties

### controllerMeshes

• `Optional` **controllerMeshes**: `boolean`

Should the native controller meshes be initialized. (default: true)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/webVRCamera.ts:123

___

### customVRButton

• `Optional` **customVRButton**: `HTMLButtonElement`

If you'd like to provide your own button to the VRHelper. (default: standard babylon vr button)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/webVRCamera.ts:136

___

### defaultHeight

• `Optional` **defaultHeight**: `number`

To change the default offset from the ground to account for user's height in meters. Will be scaled by positionScale. (default: 1.7)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/webVRCamera.ts:146

___

### defaultLightingOnControllers

• `Optional` **defaultLightingOnControllers**: `boolean`

Creating a default HemiLight only on controllers. (default: true)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/webVRCamera.ts:127

___

### displayName

• `Optional` **displayName**: `string`

If there are more than one VRDisplays, this will choose the display matching this name. (default: pick first vrDisplay)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/webVRCamera.ts:119

___

### positionScale

• `Optional` **positionScale**: `number`

Sets the scale of the vrDevice in babylon space. (default: 1)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/webVRCamera.ts:115

___

### rayLength

• `Optional` **rayLength**: `number`

To change the length of the ray for gaze/controllers. Will be scaled by positionScale. (default: 100)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/webVRCamera.ts:141

___

### trackPosition

• `Optional` **trackPosition**: `boolean`

Sets if the webVR camera should be tracked to the vrDevice. (default: true)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/webVRCamera.ts:111

___

### useCustomVRButton

• `Optional` **useCustomVRButton**: `boolean`

If you don't want to use the default VR button of the helper. (default: false)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/webVRCamera.ts:131

___

### useMultiview

• `Optional` **useMultiview**: `boolean`

If multiview should be used if available (default: false)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/webVRCamera.ts:151
