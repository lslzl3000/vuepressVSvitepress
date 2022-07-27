[@dev/core](../README.md) / [Exports](../modules.md) / WebXRMotionControllerManager

# Class: WebXRMotionControllerManager

Motion controller manager is managing the different webxr profiles and makes sure the right
controller is being loaded.

## Table of contents

### Constructors

- [constructor](WebXRMotionControllerManager.md#constructor)

### Properties

- [BaseRepositoryUrl](WebXRMotionControllerManager.md#baserepositoryurl)
- [DisableControllerCache](WebXRMotionControllerManager.md#disablecontrollercache)
- [PrioritizeOnlineRepository](WebXRMotionControllerManager.md#prioritizeonlinerepository)
- [UseOnlineRepository](WebXRMotionControllerManager.md#useonlinerepository)
- [\_AvailableControllers](WebXRMotionControllerManager.md#_availablecontrollers)
- [\_Fallbacks](WebXRMotionControllerManager.md#_fallbacks)
- [\_ProfileLoadingPromises](WebXRMotionControllerManager.md#_profileloadingpromises)
- [\_ProfilesList](WebXRMotionControllerManager.md#_profileslist)

### Methods

- [ClearControllerCache](WebXRMotionControllerManager.md#clearcontrollercache)
- [ClearProfilesCache](WebXRMotionControllerManager.md#clearprofilescache)
- [DefaultFallbacks](WebXRMotionControllerManager.md#defaultfallbacks)
- [FindFallbackWithProfileId](WebXRMotionControllerManager.md#findfallbackwithprofileid)
- [GetMotionControllerWithXRInput](WebXRMotionControllerManager.md#getmotioncontrollerwithxrinput)
- [RegisterController](WebXRMotionControllerManager.md#registercontroller)
- [RegisterFallbacksForProfileId](WebXRMotionControllerManager.md#registerfallbacksforprofileid)
- [UpdateProfilesList](WebXRMotionControllerManager.md#updateprofileslist)
- [\_LoadProfileFromRepository](WebXRMotionControllerManager.md#_loadprofilefromrepository)
- [\_LoadProfilesFromAvailableControllers](WebXRMotionControllerManager.md#_loadprofilesfromavailablecontrollers)

## Constructors

### constructor

• **new WebXRMotionControllerManager**()

## Properties

### BaseRepositoryUrl

▪ `Static` **BaseRepositoryUrl**: `string` = `"https://immersive-web.github.io/webxr-input-profiles/packages/viewer/dist"`

The base URL of the online controller repository. Can be changed at any time.

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRMotionControllerManager.ts:43

___

### DisableControllerCache

▪ `Static` **DisableControllerCache**: `boolean` = `true`

Disable the controller cache and load the models each time a new WebXRProfileMotionController is loaded.
Defaults to true.

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRMotionControllerManager.ts:57

___

### PrioritizeOnlineRepository

▪ `Static` **PrioritizeOnlineRepository**: `boolean` = `true`

Which repository gets priority - local or online

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRMotionControllerManager.ts:47

___

### UseOnlineRepository

▪ `Static` **UseOnlineRepository**: `boolean` = `true`

Use the online repository, or use only locally-defined controllers

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRMotionControllerManager.ts:51

___

### \_AvailableControllers

▪ `Static` `Private` **\_AvailableControllers**: `Object` = `{}`

#### Index signature

▪ [type: `string`]: [`MotionControllerConstructor`](../modules.md#motioncontrollerconstructor)

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRMotionControllerManager.ts:34

___

### \_Fallbacks

▪ `Static` `Private` **\_Fallbacks**: `Object` = `{}`

#### Index signature

▪ [profileId: `string`]: `string`[]

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRMotionControllerManager.ts:35

___

### \_ProfileLoadingPromises

▪ `Static` `Private` **\_ProfileLoadingPromises**: `Object` = `{}`

#### Index signature

▪ [profileName: `string`]: `Promise`[`IMotionControllerProfile`](../interfaces/IMotionControllerProfile.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRMotionControllerManager.ts:37

___

### \_ProfilesList

▪ `Static` `Private` **\_ProfilesList**: [`Nullable`](../modules.md#nullable)`Promise`{ `[profile: string]`: `string`;  }

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRMotionControllerManager.ts:38

## Methods

### ClearControllerCache

▸ `Static` **ClearControllerCache**(): `void`

Clear the controller's cache (usually happens at the end of a session)

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRMotionControllerManager.ts:198

___

### ClearProfilesCache

▸ `Static` **ClearProfilesCache**(): `void`

Clear the cache used for profile loading and reload when requested again

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRMotionControllerManager.ts:62

___

### DefaultFallbacks

▸ `Static` **DefaultFallbacks**(): `void`

Register the default fallbacks.
This function is called automatically when this file is imported.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRMotionControllerManager.ts:71

___

### FindFallbackWithProfileId

▸ `Static` **FindFallbackWithProfileId**(`profileId`): `string`[]

Find a fallback profile if the profile was not found. There are a few predefined generic profiles.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `profileId` | `string` | the profile to which a fallback needs to be found |

#### Returns

`string`[]

an array with corresponding fallback profiles

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRMotionControllerManager.ts:92

___

### GetMotionControllerWithXRInput

▸ `Static` **GetMotionControllerWithXRInput**(`xrInput`, `scene`, `forceProfile?`): `Promise`[`WebXRAbstractMotionController`](WebXRAbstractMotionController.md)

When acquiring a new xrInput object (usually by the WebXRInput class), match it with the correct profile.
The order of search:

1) Iterate the profiles array of the xr input and try finding a corresponding motion controller
2) (If not found) search in the gamepad id and try using it (legacy versions only)
3) search for registered fallbacks (should be redundant, nonetheless it makes sense to check)
4) return the generic trigger controller if none were found

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `xrInput` | `XRInputSource` | the xrInput to which a new controller is initialized |
| `scene` | [`Scene`](Scene.md) | the scene to which the model will be added |
| `forceProfile?` | `string` | force a certain profile for this controller |

#### Returns

`Promise`[`WebXRAbstractMotionController`](WebXRAbstractMotionController.md)

A promise that fulfils with the motion controller class for this profile id or the generic standard class if none was found

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRMotionControllerManager.ts:113

___

### RegisterController

▸ `Static` **RegisterController**(`type`, `constructFunction`): `void`

Register a new controller based on its profile. This function will be called by the controller classes themselves.

If you are missing a profile, make sure it is imported in your source, otherwise it will not register.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | `string` | the profile type to register |
| `constructFunction` | [`MotionControllerConstructor`](../modules.md#motioncontrollerconstructor) | the function to be called when loading this profile |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRMotionControllerManager.ts:167

___

### RegisterFallbacksForProfileId

▸ `Static` **RegisterFallbacksForProfileId**(`profileId`, `fallbacks`): `void`

Register a fallback to a specific profile.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `profileId` | `string` | the profileId that will receive the fallbacks |
| `fallbacks` | `string`[] | A list of fallback profiles |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRMotionControllerManager.ts:176

___

### UpdateProfilesList

▸ `Static` **UpdateProfilesList**(): `Promise`{ `[profile: string]`: `string`;  }

Will update the list of profiles available in the repository

#### Returns

`Promise`{ `[profile: string]`: `string`;  }

a promise that resolves to a map of profiles available online

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRMotionControllerManager.ts:188

___

### \_LoadProfileFromRepository

▸ `Static` `Private` **_LoadProfileFromRepository**(`profileArray`, `xrInput`, `scene`): `Promise`[`WebXRAbstractMotionController`](WebXRAbstractMotionController.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `profileArray` | `string`[] |
| `xrInput` | `XRInputSource` |
| `scene` | [`Scene`](Scene.md) |

#### Returns

`Promise`[`WebXRAbstractMotionController`](WebXRAbstractMotionController.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRMotionControllerManager.ts:207

___

### \_LoadProfilesFromAvailableControllers

▸ `Static` `Private` **_LoadProfilesFromAvailableControllers**(`profileArray`, `xrInput`, `scene`): `Promise`[`WebXRAbstractMotionController`](WebXRAbstractMotionController.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `profileArray` | `string`[] |
| `xrInput` | `XRInputSource` |
| `scene` | [`Scene`](Scene.md) |

#### Returns

`Promise`[`WebXRAbstractMotionController`](WebXRAbstractMotionController.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRMotionControllerManager.ts:244
