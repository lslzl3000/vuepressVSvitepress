[@dev/core](../README.md) / [Exports](../modules.md) / IWebXRInputOptions

# Interface: IWebXRInputOptions

The schema for initialization options of the XR Input class

## Table of contents

### Properties

- [controllerOptions](IWebXRInputOptions.md#controlleroptions)
- [customControllersRepositoryURL](IWebXRInputOptions.md#customcontrollersrepositoryurl)
- [disableControllerAnimation](IWebXRInputOptions.md#disablecontrolleranimation)
- [disableOnlineControllerRepository](IWebXRInputOptions.md#disableonlinecontrollerrepository)
- [doNotLoadControllerMeshes](IWebXRInputOptions.md#donotloadcontrollermeshes)
- [forceInputProfile](IWebXRInputOptions.md#forceinputprofile)

## Properties

### controllerOptions

• `Optional` **controllerOptions**: [`IWebXRControllerOptions`](IWebXRControllerOptions.md)

Optional options to pass to the controller. Will be overridden by the Input options where applicable

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRInput.ts:47

___

### customControllersRepositoryURL

• `Optional` **customControllersRepositoryURL**: `string`

A custom URL for the controllers repository

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRInput.ts:37

___

### disableControllerAnimation

• `Optional` **disableControllerAnimation**: `boolean`

Should the controller model's components not move according to the user input

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRInput.ts:42

___

### disableOnlineControllerRepository

• `Optional` **disableOnlineControllerRepository**: `boolean`

Do not send a request to the controller repository to load the profile.

Instead, use the controllers available in babylon itself.

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRInput.ts:32

___

### doNotLoadControllerMeshes

• `Optional` **doNotLoadControllerMeshes**: `boolean`

If set to true no model will be automatically loaded

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRInput.ts:18

___

### forceInputProfile

• `Optional` **forceInputProfile**: `string`

If set, this profile will be used for all controllers loaded (for example "microsoft-mixed-reality")
If not found, the xr input profile data will be used.
Profiles are defined here - https://github.com/immersive-web/webxr-input-profiles/

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRInput.ts:25
