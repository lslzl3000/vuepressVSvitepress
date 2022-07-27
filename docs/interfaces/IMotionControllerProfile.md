[@dev/core](../README.md) / [Exports](../modules.md) / IMotionControllerProfile

# Interface: IMotionControllerProfile

The XR Input profile schema
Profiles can be found here:
https://github.com/immersive-web/webxr-input-profiles/tree/master/packages/registry/profiles

## Table of contents

### Properties

- [fallbackProfileIds](IMotionControllerProfile.md#fallbackprofileids)
- [layouts](IMotionControllerProfile.md#layouts)
- [profileId](IMotionControllerProfile.md#profileid)

## Properties

### fallbackProfileIds

• **fallbackProfileIds**: `string`[]

fallback profiles for this profileId

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:139

___

### layouts

• **layouts**: [`IMotionControllerLayoutMap`](IMotionControllerLayoutMap.md)

The layout map, with handedness as key

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:143

___

### profileId

• **profileId**: `string`

The id of this profile
correlates to the profile(s) in the xrInput.profiles array

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRAbstractMotionController.ts:148
