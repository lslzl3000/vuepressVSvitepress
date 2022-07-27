[@dev/core](../README.md) / [Exports](../modules.md) / VRExperienceHelper

# Class: VRExperienceHelper

Helps to quickly add VR support to an existing scene.
See https://doc.babylonjs.com/divingDeeper/cameras/webVRHelper

**`Deprecated`**

## Table of contents

### Constructors

- [constructor](VRExperienceHelper.md#constructor)

### Properties

- [\_btnVR](VRExperienceHelper.md#_btnvr)
- [\_btnVRDisplayed](VRExperienceHelper.md#_btnvrdisplayed)
- [\_cachedAngularSensibility](VRExperienceHelper.md#_cachedangularsensibility)
- [\_cameraGazer](VRExperienceHelper.md#_cameragazer)
- [\_circleEase](VRExperienceHelper.md#_circleease)
- [\_defaultHeight](VRExperienceHelper.md#_defaultheight)
- [\_deviceOrientationCamera](VRExperienceHelper.md#_deviceorientationcamera)
- [\_displayGaze](VRExperienceHelper.md#_displaygaze)
- [\_displayLaserPointer](VRExperienceHelper.md#_displaylaserpointer)
- [\_existingCamera](VRExperienceHelper.md#_existingcamera)
- [\_floorMeshName](VRExperienceHelper.md#_floormeshname)
- [\_floorMeshesCollection](VRExperienceHelper.md#_floormeshescollection)
- [\_fullscreenVRpresenting](VRExperienceHelper.md#_fullscreenvrpresenting)
- [\_gazeColor](VRExperienceHelper.md#_gazecolor)
- [\_haloCenter](VRExperienceHelper.md#_halocenter)
- [\_hasEnteredVR](VRExperienceHelper.md#_hasenteredvr)
- [\_inputElement](VRExperienceHelper.md#_inputelement)
- [\_interactionsEnabled](VRExperienceHelper.md#_interactionsenabled)
- [\_interactionsRequested](VRExperienceHelper.md#_interactionsrequested)
- [\_isDefaultTeleportationTarget](VRExperienceHelper.md#_isdefaultteleportationtarget)
- [\_laserColor](VRExperienceHelper.md#_lasercolor)
- [\_leftController](VRExperienceHelper.md#_leftcontroller)
- [\_onKeyDown](VRExperienceHelper.md#_onkeydown)
- [\_onVRDisplayChangedBind](VRExperienceHelper.md#_onvrdisplaychangedbind)
- [\_onVRRequestPresentComplete](VRExperienceHelper.md#_onvrrequestpresentcomplete)
- [\_onVRRequestPresentStart](VRExperienceHelper.md#_onvrrequestpresentstart)
- [\_onVrDisplayPresentChangeBind](VRExperienceHelper.md#_onvrdisplaypresentchangebind)
- [\_padSensibilityDown](VRExperienceHelper.md#_padsensibilitydown)
- [\_padSensibilityUp](VRExperienceHelper.md#_padsensibilityup)
- [\_pickedGazeColor](VRExperienceHelper.md#_pickedgazecolor)
- [\_pickedLaserColor](VRExperienceHelper.md#_pickedlasercolor)
- [\_position](VRExperienceHelper.md#_position)
- [\_postProcessMove](VRExperienceHelper.md#_postprocessmove)
- [\_rayLength](VRExperienceHelper.md#_raylength)
- [\_raySelectionPredicate](VRExperienceHelper.md#_rayselectionpredicate)
- [\_rightController](VRExperienceHelper.md#_rightcontroller)
- [\_rotationAllowed](VRExperienceHelper.md#_rotationallowed)
- [\_rotationAngle](VRExperienceHelper.md#_rotationangle)
- [\_scene](VRExperienceHelper.md#_scene)
- [\_teleportActive](VRExperienceHelper.md#_teleportactive)
- [\_teleportBackwardsVector](VRExperienceHelper.md#_teleportbackwardsvector)
- [\_teleportationBorderColor](VRExperienceHelper.md#_teleportationbordercolor)
- [\_teleportationEasing](VRExperienceHelper.md#_teleportationeasing)
- [\_teleportationFillColor](VRExperienceHelper.md#_teleportationfillcolor)
- [\_teleportationInitialized](VRExperienceHelper.md#_teleportationinitialized)
- [\_teleportationMode](VRExperienceHelper.md#_teleportationmode)
- [\_teleportationRequested](VRExperienceHelper.md#_teleportationrequested)
- [\_teleportationSpeed](VRExperienceHelper.md#_teleportationspeed)
- [\_teleportationTarget](VRExperienceHelper.md#_teleportationtarget)
- [\_teleportationTime](VRExperienceHelper.md#_teleportationtime)
- [\_useCustomVRButton](VRExperienceHelper.md#_usecustomvrbutton)
- [\_vrDeviceOrientationCamera](VRExperienceHelper.md#_vrdeviceorientationcamera)
- [\_webVRCamera](VRExperienceHelper.md#_webvrcamera)
- [\_webVRpresenting](VRExperienceHelper.md#_webvrpresenting)
- [\_webVRready](VRExperienceHelper.md#_webvrready)
- [\_webVRrequesting](VRExperienceHelper.md#_webvrrequesting)
- [\_webVRsupported](VRExperienceHelper.md#_webvrsupported)
- [\_workingMatrix](VRExperienceHelper.md#_workingmatrix)
- [\_workingQuaternion](VRExperienceHelper.md#_workingquaternion)
- [\_workingVector](VRExperienceHelper.md#_workingvector)
- [enableGazeEvenWhenNoPointerLock](VRExperienceHelper.md#enablegazeevenwhennopointerlock)
- [exitVROnDoubleTap](VRExperienceHelper.md#exitvrondoubletap)
- [meshSelectionPredicate](VRExperienceHelper.md#meshselectionpredicate)
- [onAfterCameraTeleport](VRExperienceHelper.md#onaftercamerateleport)
- [onAfterEnteringVRObservable](VRExperienceHelper.md#onafterenteringvrobservable)
- [onBeforeCameraTeleport](VRExperienceHelper.md#onbeforecamerateleport)
- [onControllerMeshLoadedObservable](VRExperienceHelper.md#oncontrollermeshloadedobservable)
- [onEnteringVRObservable](VRExperienceHelper.md#onenteringvrobservable)
- [onExitingVRObservable](VRExperienceHelper.md#onexitingvrobservable)
- [onMeshSelectedWithController](VRExperienceHelper.md#onmeshselectedwithcontroller)
- [onNewMeshPicked](VRExperienceHelper.md#onnewmeshpicked)
- [onNewMeshSelected](VRExperienceHelper.md#onnewmeshselected)
- [onSelectedMeshUnselected](VRExperienceHelper.md#onselectedmeshunselected)
- [raySelectionPredicate](VRExperienceHelper.md#rayselectionpredicate)
- [requestPointerLockOnFullScreen](VRExperienceHelper.md#requestpointerlockonfullscreen)
- [teleportationEnabled](VRExperienceHelper.md#teleportationenabled)
- [updateControllerLaserColor](VRExperienceHelper.md#updatecontrollerlasercolor)
- [updateGazeTrackerColor](VRExperienceHelper.md#updategazetrackercolor)
- [updateGazeTrackerScale](VRExperienceHelper.md#updategazetrackerscale)
- [webVROptions](VRExperienceHelper.md#webvroptions)
- [xr](VRExperienceHelper.md#xr)
- [xrTestDone](VRExperienceHelper.md#xrtestdone)
- [TELEPORTATIONMODE\_CONSTANTSPEED](VRExperienceHelper.md#teleportationmode_constantspeed)
- [TELEPORTATIONMODE\_CONSTANTTIME](VRExperienceHelper.md#teleportationmode_constanttime)

### Accessors

- [\_noControllerIsActive](VRExperienceHelper.md#_nocontrollerisactive)
- [\_teleportationRequestInitiated](VRExperienceHelper.md#_teleportationrequestinitiated)
- [currentVRCamera](VRExperienceHelper.md#currentvrcamera)
- [deviceOrientationCamera](VRExperienceHelper.md#deviceorientationcamera)
- [displayGaze](VRExperienceHelper.md#displaygaze)
- [displayLaserPointer](VRExperienceHelper.md#displaylaserpointer)
- [gazeTrackerMesh](VRExperienceHelper.md#gazetrackermesh)
- [isInVRMode](VRExperienceHelper.md#isinvrmode)
- [leftControllerGazeTrackerMesh](VRExperienceHelper.md#leftcontrollergazetrackermesh)
- [onControllerMeshLoaded](VRExperienceHelper.md#oncontrollermeshloaded)
- [onEnteringVR](VRExperienceHelper.md#onenteringvr)
- [onExitingVR](VRExperienceHelper.md#onexitingvr)
- [position](VRExperienceHelper.md#position)
- [rightControllerGazeTrackerMesh](VRExperienceHelper.md#rightcontrollergazetrackermesh)
- [teleportationTarget](VRExperienceHelper.md#teleportationtarget)
- [vrButton](VRExperienceHelper.md#vrbutton)
- [vrDeviceOrientationCamera](VRExperienceHelper.md#vrdeviceorientationcamera)
- [webVRCamera](VRExperienceHelper.md#webvrcamera)

### Methods

- [\_beforeRender](VRExperienceHelper.md#_beforerender)
- [\_castRayAndSelectObject](VRExperienceHelper.md#_castrayandselectobject)
- [\_checkRotate](VRExperienceHelper.md#_checkrotate)
- [\_checkTeleportBackwards](VRExperienceHelper.md#_checkteleportbackwards)
- [\_checkTeleportWithRay](VRExperienceHelper.md#_checkteleportwithray)
- [\_completeVRInit](VRExperienceHelper.md#_completevrinit)
- [\_convertNormalToDirectionOfRay](VRExperienceHelper.md#_convertnormaltodirectionofray)
- [\_createTeleportationCircles](VRExperienceHelper.md#_createteleportationcircles)
- [\_displayTeleportationTarget](VRExperienceHelper.md#_displayteleportationtarget)
- [\_displayVRButton](VRExperienceHelper.md#_displayvrbutton)
- [\_enableInteractionOnController](VRExperienceHelper.md#_enableinteractiononcontroller)
- [\_enableTeleportationOnController](VRExperienceHelper.md#_enableteleportationoncontroller)
- [\_hideTeleportationTarget](VRExperienceHelper.md#_hideteleportationtarget)
- [\_isTeleportationFloor](VRExperienceHelper.md#_isteleportationfloor)
- [\_moveButtonToBottomRight](VRExperienceHelper.md#_movebuttontobottomright)
- [\_moveTeleportationSelectorTo](VRExperienceHelper.md#_moveteleportationselectorto)
- [\_notifySelectedMeshUnselected](VRExperienceHelper.md#_notifyselectedmeshunselected)
- [\_onDefaultMeshLoaded](VRExperienceHelper.md#_ondefaultmeshloaded)
- [\_onFullscreenChange](VRExperienceHelper.md#_onfullscreenchange)
- [\_onNewGamepadConnected](VRExperienceHelper.md#_onnewgamepadconnected)
- [\_onNewGamepadDisconnected](VRExperienceHelper.md#_onnewgamepaddisconnected)
- [\_onResize](VRExperienceHelper.md#_onresize)
- [\_onVRDisplayChanged](VRExperienceHelper.md#_onvrdisplaychanged)
- [\_onVrDisplayPresentChange](VRExperienceHelper.md#_onvrdisplaypresentchange)
- [\_rotateCamera](VRExperienceHelper.md#_rotatecamera)
- [\_tryEnableInteractionOnController](VRExperienceHelper.md#_tryenableinteractiononcontroller)
- [\_updateButtonVisibility](VRExperienceHelper.md#_updatebuttonvisibility)
- [addFloorMesh](VRExperienceHelper.md#addfloormesh)
- [changeGazeColor](VRExperienceHelper.md#changegazecolor)
- [changeLaserColor](VRExperienceHelper.md#changelasercolor)
- [dispose](VRExperienceHelper.md#dispose)
- [enableInteractions](VRExperienceHelper.md#enableinteractions)
- [enableTeleportation](VRExperienceHelper.md#enableteleportation)
- [enterVR](VRExperienceHelper.md#entervr)
- [exitVR](VRExperienceHelper.md#exitvr)
- [getClassName](VRExperienceHelper.md#getclassname)
- [removeFloorMesh](VRExperienceHelper.md#removefloormesh)
- [setGazeColor](VRExperienceHelper.md#setgazecolor)
- [setLaserColor](VRExperienceHelper.md#setlasercolor)
- [setLaserLightingState](VRExperienceHelper.md#setlaserlightingstate)
- [teleportCamera](VRExperienceHelper.md#teleportcamera)

## Constructors

### constructor

• **new VRExperienceHelper**(`scene`, `webVROptions?`)

Instantiates a VRExperienceHelper.
Helps to quickly add VR support to an existing scene.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | The scene the VRExperienceHelper belongs to. |
| `webVROptions` | [`VRExperienceHelperOptions`](../interfaces/VRExperienceHelperOptions.md) | Options to modify the vr experience helper's behavior. |

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:753

## Properties

### \_btnVR

• `Private` **\_btnVR**: [`Nullable`](../modules.md#nullable)`HTMLButtonElement`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:368

___

### \_btnVRDisplayed

• `Private` **\_btnVRDisplayed**: `boolean`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:369

___

### \_cachedAngularSensibility

• `Private` **\_cachedAngularSensibility**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `angularSensibility` | ``null`` |
| `angularSensibilityX` | ``null`` |
| `angularSensibilityY` | ``null`` |

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:1169

___

### \_cameraGazer

• `Private` **\_cameraGazer**: `VRExperienceHelperCameraGazer`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:467

___

### \_circleEase

• `Private` **\_circleEase**: [`CircleEase`](CircleEase.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:495

___

### \_defaultHeight

• `Private` **\_defaultHeight**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:529

___

### \_deviceOrientationCamera

• `Private` **\_deviceOrientationCamera**: [`Nullable`](../modules.md#nullable)[`DeviceOrientationCamera`](DeviceOrientationCamera.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:388

___

### \_displayGaze

• `Private` **\_displayGaze**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:533

___

### \_displayLaserPointer

• `Private` **\_displayLaserPointer**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:534

___

### \_existingCamera

• `Private` **\_existingCamera**: [`Camera`](Camera.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:389

___

### \_floorMeshName

• `Private` **\_floorMeshName**: `string`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:452

___

### \_floorMeshesCollection

• `Private` **\_floorMeshesCollection**: [`Mesh`](Mesh.md)[] = `[]`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:453

___

### \_fullscreenVRpresenting

• `Private` **\_fullscreenVRpresenting**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:383

___

### \_gazeColor

• `Private` **\_gazeColor**: [`Color3`](Color3.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:474

___

### \_haloCenter

• `Private` **\_haloCenter**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:466

___

### \_hasEnteredVR

• `Private` **\_hasEnteredVR**: `boolean`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:380

___

### \_inputElement

• `Private` **\_inputElement**: [`Nullable`](../modules.md#nullable)`HTMLElement`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:385

___

### \_interactionsEnabled

• `Private` **\_interactionsEnabled**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:531

___

### \_interactionsRequested

• `Private` **\_interactionsRequested**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:532

___

### \_isDefaultTeleportationTarget

• `Private` **\_isDefaultTeleportationTarget**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:461

___

### \_laserColor

• `Private` **\_laserColor**: [`Color3`](Color3.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:475

___

### \_leftController

• `Private` **\_leftController**: [`Nullable`](../modules.md#nullable)`VRExperienceHelperControllerGazer` = `null`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:471

___

### \_onKeyDown

• `Private` **\_onKeyDown**: (`event`: `KeyboardEvent`) => `void`

#### Type declaration

▸ (`event`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `event` | `KeyboardEvent` |

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:391

___

### \_onVRDisplayChangedBind

• `Private` **\_onVRDisplayChangedBind**: (`eventArgs`: [`IDisplayChangedEventArgs`](../interfaces/IDisplayChangedEventArgs.md)) => `void`

#### Type declaration

▸ (`eventArgs`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `eventArgs` | [`IDisplayChangedEventArgs`](../interfaces/IDisplayChangedEventArgs.md) |

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:393

___

### \_onVRRequestPresentComplete

• `Private` **\_onVRRequestPresentComplete**: (`success`: `boolean`) => `void`

#### Type declaration

▸ (`success`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `success` | `boolean` |

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:395

___

### \_onVRRequestPresentStart

• `Private` **\_onVRRequestPresentStart**: () => `void`

#### Type declaration

▸ (): `void`

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:394

___

### \_onVrDisplayPresentChangeBind

• `Private` **\_onVrDisplayPresentChangeBind**: `any`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:392

___

### \_padSensibilityDown

• `Private` **\_padSensibilityDown**: `number` = `0.35`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:469

___

### \_padSensibilityUp

• `Private` **\_padSensibilityUp**: `number` = `0.65`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:468

___

### \_pickedGazeColor

• `Private` **\_pickedGazeColor**: [`Color3`](Color3.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:477

___

### \_pickedLaserColor

• `Private` **\_pickedLaserColor**: [`Color3`](Color3.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:476

___

### \_position

• `Private` **\_position**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:367

___

### \_postProcessMove

• `Private` **\_postProcessMove**: [`ImageProcessingPostProcess`](ImageProcessingPostProcess.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:462

___

### \_rayLength

• `Private` **\_rayLength**: `number`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:448

___

### \_raySelectionPredicate

• `Private` **\_raySelectionPredicate**: (`mesh`: [`AbstractMesh`](AbstractMesh.md)) => `boolean`

#### Type declaration

▸ (`mesh`): `boolean`

##### Parameters

| Name | Type |
| :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) |

##### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:512

___

### \_rightController

• `Private` **\_rightController**: [`Nullable`](../modules.md#nullable)`VRExperienceHelperControllerGazer` = `null`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:472

___

### \_rotationAllowed

• `Private` **\_rotationAllowed**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:458

___

### \_rotationAngle

• `Private` **\_rotationAngle**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:465

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:366

___

### \_teleportActive

• `Private` **\_teleportActive**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:451

___

### \_teleportBackwardsVector

• `Private` **\_teleportBackwardsVector**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:459

___

### \_teleportationBorderColor

• `Private` **\_teleportationBorderColor**: `string` = `"#FFFFFF"`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:464

___

### \_teleportationEasing

• `Private` **\_teleportationEasing**: [`EasingFunction`](EasingFunction.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:457

___

### \_teleportationFillColor

• `Private` **\_teleportationFillColor**: `string` = `"#444444"`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:463

___

### \_teleportationInitialized

• `Private` **\_teleportationInitialized**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:530

___

### \_teleportationMode

• `Private` **\_teleportationMode**: `number` = `VRExperienceHelper.TELEPORTATIONMODE_CONSTANTTIME`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:454

___

### \_teleportationRequested

• `Private` **\_teleportationRequested**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:450

___

### \_teleportationSpeed

• `Private` **\_teleportationSpeed**: `number` = `20`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:456

___

### \_teleportationTarget

• `Private` **\_teleportationTarget**: [`Mesh`](Mesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:460

___

### \_teleportationTime

• `Private` **\_teleportationTime**: `number` = `122`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:455

___

### \_useCustomVRButton

• `Private` **\_useCustomVRButton**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:449

___

### \_vrDeviceOrientationCamera

• `Private` **\_vrDeviceOrientationCamera**: [`Nullable`](../modules.md#nullable)[`VRDeviceOrientationFreeCamera`](VRDeviceOrientationFreeCamera.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:387

___

### \_webVRCamera

• `Private` **\_webVRCamera**: [`WebVRFreeCamera`](WebVRFreeCamera.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:386

___

### \_webVRpresenting

• `Private` **\_webVRpresenting**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:378

___

### \_webVRready

• `Private` **\_webVRready**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:374

___

### \_webVRrequesting

• `Private` **\_webVRrequesting**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:376

___

### \_webVRsupported

• `Private` **\_webVRsupported**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:372

___

### \_workingMatrix

• `Private` **\_workingMatrix**: [`Matrix`](Matrix.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:2018

___

### \_workingQuaternion

• `Private` **\_workingQuaternion**: [`Quaternion`](Quaternion.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:2017

___

### \_workingVector

• `Private` **\_workingVector**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:2016

___

### enableGazeEvenWhenNoPointerLock

• **enableGazeEvenWhenNoPointerLock**: `boolean` = `false`

Gets or sets a boolean indicating that gaze can be enabled even if pointer lock is not engage (useful on iOS where fullscreen mode and pointer lock are not supported)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:400

___

### exitVROnDoubleTap

• **exitVROnDoubleTap**: `boolean` = `true`

Gets or sets a boolean indicating that the VREXperienceHelper will exit VR if double tap is detected

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:405

___

### meshSelectionPredicate

• **meshSelectionPredicate**: (`mesh`: [`AbstractMesh`](AbstractMesh.md)) => `boolean`

#### Type declaration

▸ (`mesh`): `boolean`

To be optionally changed by user to define custom selection logic (after ray selection)

##### Parameters

| Name | Type |
| :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) |

##### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:522

___

### onAfterCameraTeleport

• **onAfterCameraTeleport**: [`Observable`](Observable.md)[`Vector3`](Vector3.md)

Observable raised after camera teleportation

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:505

___

### onAfterEnteringVRObservable

• **onAfterEnteringVRObservable**: [`Observable`](Observable.md)[`OnAfterEnteringVRObservableEvent`](OnAfterEnteringVRObservableEvent.md)

Observable raised when entering VR has completed.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:415

___

### onBeforeCameraTeleport

• **onBeforeCameraTeleport**: [`Observable`](Observable.md)[`Vector3`](Vector3.md)

Observable raised before camera teleportation

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:500

___

### onControllerMeshLoadedObservable

• **onControllerMeshLoadedObservable**: [`Observable`](Observable.md)[`WebVRController`](WebVRController.md)

Observable raised when controller mesh is loaded.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:425

___

### onEnteringVRObservable

• **onEnteringVRObservable**: [`Observable`](Observable.md)[`VRExperienceHelper`](VRExperienceHelper.md)

Observable raised right before entering VR.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:410

___

### onExitingVRObservable

• **onExitingVRObservable**: [`Observable`](Observable.md)[`VRExperienceHelper`](VRExperienceHelper.md)

Observable raised when exiting VR.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:420

___

### onMeshSelectedWithController

• **onMeshSelectedWithController**: [`Observable`](Observable.md){ `controller`: [`WebVRController`](WebVRController.md) ; `mesh`: [`AbstractMesh`](AbstractMesh.md)  }

Observable raised when a new mesh is selected based on meshSelectionPredicate.
This observable will provide the mesh and the controller used to select the mesh

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:488

___

### onNewMeshPicked

• **onNewMeshPicked**: [`Observable`](Observable.md)[`PickingInfo`](PickingInfo.md)

Observable raised when a new mesh is picked based on meshSelectionPredicate

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:493

___

### onNewMeshSelected

• **onNewMeshSelected**: [`Observable`](Observable.md)[`AbstractMesh`](AbstractMesh.md)

Observable raised when a new mesh is selected based on meshSelectionPredicate

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:482

___

### onSelectedMeshUnselected

• **onSelectedMeshUnselected**: [`Observable`](Observable.md)[`AbstractMesh`](AbstractMesh.md)

Observable raised when current selected mesh gets unselected

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:510

___

### raySelectionPredicate

• **raySelectionPredicate**: (`mesh`: [`AbstractMesh`](AbstractMesh.md)) => `boolean`

#### Type declaration

▸ (`mesh`): `boolean`

To be optionally changed by user to define custom ray selection

##### Parameters

| Name | Type |
| :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) |

##### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:517

___

### requestPointerLockOnFullScreen

• **requestPointerLockOnFullScreen**: `boolean` = `true`

Defines whether or not Pointer lock should be requested when switching to
full screen.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:732

___

### teleportationEnabled

• **teleportationEnabled**: `boolean` = `true`

Set teleportation enabled. If set to false camera teleportation will be disabled but camera rotation will be kept.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:527

___

### updateControllerLaserColor

• **updateControllerLaserColor**: `boolean` = `true`

If the controller laser color should be updated when selecting meshes

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:603

___

### updateGazeTrackerColor

• **updateGazeTrackerColor**: `boolean` = `true`

If the gaze trackers color should be updated when selecting meshes

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:599

___

### updateGazeTrackerScale

• **updateGazeTrackerScale**: `boolean` = `true`

If the gaze trackers scale should be updated to be constant size when pointing at near/far meshes

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:595

___

### webVROptions

• **webVROptions**: [`VRExperienceHelperOptions`](../interfaces/VRExperienceHelperOptions.md) = `{}`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:756

___

### xr

• **xr**: [`WebXRDefaultExperience`](WebXRDefaultExperience.md)

If asking to force XR, this will be populated with the default xr experience

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:739

___

### xrTestDone

• **xrTestDone**: `boolean` = `false`

Was the XR test done already. If this is true AND this.xr exists, xr is initialized.
If this is true and no this.xr, xr exists but is not supported, using WebVR.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:745

___

### TELEPORTATIONMODE\_CONSTANTSPEED

▪ `Static` `Readonly` **TELEPORTATIONMODE\_CONSTANTSPEED**: ``1``

Speed Constant Teleportation Mode

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:2027

___

### TELEPORTATIONMODE\_CONSTANTTIME

▪ `Static` `Readonly` **TELEPORTATIONMODE\_CONSTANTTIME**: ``0``

Time Constant Teleportation Mode

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:2023

## Accessors

### \_noControllerIsActive

• `Private` `get` **_noControllerIsActive**(): `boolean`

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:1426

___

### \_teleportationRequestInitiated

• `Private` `get` **_teleportationRequestInitiated**(): `boolean`

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:720

___

### currentVRCamera

• `get` **currentVRCamera**(): [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md)

Based on the current WebVR support, returns the current VR camera used.

#### Returns

[`Nullable`](../modules.md#nullable)[`Camera`](Camera.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:691

___

### deviceOrientationCamera

• `get` **deviceOrientationCamera**(): [`Nullable`](../modules.md#nullable)[`DeviceOrientationCamera`](DeviceOrientationCamera.md)

The deviceOrientationCamera used as the camera when not in VR.

#### Returns

[`Nullable`](../modules.md#nullable)[`DeviceOrientationCamera`](DeviceOrientationCamera.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:684

___

### displayGaze

• `get` **displayGaze**(): `boolean`

If the ray of the gaze should be displayed.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:628

• `set` **displayGaze**(`value`): `void`

Sets if the ray of the gaze should be displayed.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:635

___

### displayLaserPointer

• `get` **displayLaserPointer**(): `boolean`

If the ray of the LaserPointer should be displayed.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:653

• `set` **displayLaserPointer**(`value`): `void`

Sets if the ray of the LaserPointer should be displayed.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:660

___

### gazeTrackerMesh

• `get` **gazeTrackerMesh**(): [`Mesh`](Mesh.md)

The mesh used to display where the user is selecting, this mesh will be cloned and set as the gazeTracker for the left and right controller
when set bakeCurrentTransformIntoVertices will be called on the mesh.
See https://doc.babylonjs.com/resources/baking_transformations

#### Returns

[`Mesh`](Mesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:559

• `set` **gazeTrackerMesh**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Mesh`](Mesh.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:563

___

### isInVRMode

• `get` **isInVRMode**(): `boolean`

Gets a value indicating if we are currently in VR mode.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:1106

___

### leftControllerGazeTrackerMesh

• `get` **leftControllerGazeTrackerMesh**(): [`Nullable`](../modules.md#nullable)[`Mesh`](Mesh.md)

The gaze tracking mesh corresponding to the left controller

#### Returns

[`Nullable`](../modules.md#nullable)[`Mesh`](Mesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:608

___

### onControllerMeshLoaded

• `get` **onControllerMeshLoaded**(): [`Observable`](Observable.md)[`WebVRController`](WebVRController.md)

Return this.onControllerMeshLoadedObservable
Note: This one is for backward compatibility. Please use onControllerMeshLoadedObservable directly

#### Returns

[`Observable`](Observable.md)[`WebVRController`](WebVRController.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:444

___

### onEnteringVR

• `get` **onEnteringVR**(): [`Observable`](Observable.md)[`VRExperienceHelper`](VRExperienceHelper.md)

Return this.onEnteringVRObservable
Note: This one is for backward compatibility. Please use onEnteringVRObservable directly

#### Returns

[`Observable`](Observable.md)[`VRExperienceHelper`](VRExperienceHelper.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:430

___

### onExitingVR

• `get` **onExitingVR**(): [`Observable`](Observable.md)[`VRExperienceHelper`](VRExperienceHelper.md)

Return this.onExitingVRObservable
Note: This one is for backward compatibility. Please use onExitingVRObservable directly

#### Returns

[`Observable`](Observable.md)[`VRExperienceHelper`](VRExperienceHelper.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:437

___

### position

• `get` **position**(): [`Vector3`](Vector3.md)

The position of the vr experience helper.

#### Returns

[`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:1366

• `set` **position**(`value`): `void`

Sets the position of the vr experience helper.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:1373

___

### rightControllerGazeTrackerMesh

• `get` **rightControllerGazeTrackerMesh**(): [`Nullable`](../modules.md#nullable)[`Mesh`](Mesh.md)

The gaze tracking mesh corresponding to the right controller

#### Returns

[`Nullable`](../modules.md#nullable)[`Mesh`](Mesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:618

___

### teleportationTarget

• `get` **teleportationTarget**(): [`Mesh`](Mesh.md)

The mesh used to display where the user is going to teleport.

#### Returns

[`Mesh`](Mesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:539

• `set` **teleportationTarget**(`value`): `void`

Sets the mesh to be used to display where the user is going to teleport.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Mesh`](Mesh.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:546

___

### vrButton

• `get` **vrButton**(): [`Nullable`](../modules.md#nullable)`HTMLButtonElement`

The html button that is used to trigger entering into VR.

#### Returns

[`Nullable`](../modules.md#nullable)`HTMLButtonElement`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:716

___

### vrDeviceOrientationCamera

• `get` **vrDeviceOrientationCamera**(): [`Nullable`](../modules.md#nullable)[`VRDeviceOrientationFreeCamera`](VRDeviceOrientationFreeCamera.md)

The deviceOrientationCamera that is used as a fallback when vr device is not connected.

#### Returns

[`Nullable`](../modules.md#nullable)[`VRDeviceOrientationFreeCamera`](VRDeviceOrientationFreeCamera.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:709

___

### webVRCamera

• `get` **webVRCamera**(): [`WebVRFreeCamera`](WebVRFreeCamera.md)

The webVRCamera which is used when in VR.

#### Returns

[`WebVRFreeCamera`](WebVRFreeCamera.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:702

## Methods

### \_beforeRender

▸ `Private` **_beforeRender**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:1430

___

### \_castRayAndSelectObject

▸ `Private` **_castRayAndSelectObject**(`gazer`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `gazer` | `VRExperienceHelperGazer` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:2153

___

### \_checkRotate

▸ `Private` **_checkRotate**(`stateObject`, `gazer`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `stateObject` | [`StickValues`](StickValues.md) |
| `gazer` | `VRExperienceHelperGazer` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:1717

___

### \_checkTeleportBackwards

▸ `Private` **_checkTeleportBackwards**(`stateObject`, `gazer`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `stateObject` | [`StickValues`](StickValues.md) |
| `gazer` | `VRExperienceHelperGazer` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:1749

___

### \_checkTeleportWithRay

▸ `Private` **_checkTeleportWithRay**(`stateObject`, `gazer`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `stateObject` | [`StickValues`](StickValues.md) |
| `gazer` | `VRExperienceHelperGazer` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:1696

___

### \_completeVRInit

▸ `Private` **_completeVRInit**(`scene`, `webVROptions`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `scene` | [`Scene`](Scene.md) |
| `webVROptions` | [`VRExperienceHelperOptions`](../interfaces/VRExperienceHelperOptions.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:893

___

### \_convertNormalToDirectionOfRay

▸ `Private` **_convertNormalToDirectionOfRay**(`normal`, `ray`): [`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `normal` | [`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md) |
| `ray` | [`Ray`](Ray.md) |

#### Returns

[`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:2143

___

### \_createTeleportationCircles

▸ `Private` **_createTeleportationCircles**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:1824

___

### \_displayTeleportationTarget

▸ `Private` **_displayTeleportationTarget**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:1894

___

### \_displayVRButton

▸ `Private` **_displayVRButton**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:1142

___

### \_enableInteractionOnController

▸ `Private` **_enableInteractionOnController**(`controller`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `controller` | `VRExperienceHelperControllerGazer` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:1658

___

### \_enableTeleportationOnController

▸ `Private` **_enableTeleportationOnController**(`controller`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `controller` | `VRExperienceHelperControllerGazer` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:1795

___

### \_hideTeleportationTarget

▸ `Private` **_hideTeleportationTarget**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:1904

___

### \_isTeleportationFloor

▸ `Private` **_isTeleportationFloor**(`mesh`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) |

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:1446

___

### \_moveButtonToBottomRight

▸ `Private` **_moveButtonToBottomRight**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:1134

___

### \_moveTeleportationSelectorTo

▸ `Private` **_moveTeleportationSelectorTo**(`hit`, `gazer`, `ray`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `hit` | [`PickingInfo`](PickingInfo.md) |
| `gazer` | `VRExperienceHelperGazer` |
| `ray` | [`Ray`](Ray.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:1999

___

### \_notifySelectedMeshUnselected

▸ `Private` **_notifySelectedMeshUnselected**(`mesh`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `mesh` | [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:2273

___

### \_onDefaultMeshLoaded

▸ `Private` **_onDefaultMeshLoaded**(`webVRController`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `webVRController` | [`WebVRController`](WebVRController.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:1053

___

### \_onFullscreenChange

▸ `Private` **_onFullscreenChange**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:1079

___

### \_onNewGamepadConnected

▸ `Private` **_onNewGamepadConnected**(`gamepad`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `gamepad` | [`Gamepad`](Gamepad.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:1586

___

### \_onNewGamepadDisconnected

▸ `Private` **_onNewGamepadDisconnected**(`gamepad`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `gamepad` | [`Gamepad`](Gamepad.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:1645

___

### \_onResize

▸ `Private` **_onResize**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:1072

___

### \_onVRDisplayChanged

▸ `Private` **_onVRDisplayChanged**(`eventArgs`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `eventArgs` | [`IDisplayChangedEventArgs`](../interfaces/IDisplayChangedEventArgs.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:1126

___

### \_onVrDisplayPresentChange

▸ `Private` **_onVrDisplayPresentChange**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:1110

___

### \_rotateCamera

▸ `Private` **_rotateCamera**(`right`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `right` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:1914

___

### \_tryEnableInteractionOnController

▸ `Private` **_tryEnableInteractionOnController**(`controller`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `controller` | `VRExperienceHelperControllerGazer` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:1636

___

### \_updateButtonVisibility

▸ `Private` **_updateButtonVisibility**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:1149

___

### addFloorMesh

▸ **addFloorMesh**(`floorMesh`): `void`

Adds a floor mesh to be used for teleportation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `floorMesh` | [`Mesh`](Mesh.md) | the mesh to be used for teleportation. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:1462

___

### changeGazeColor

▸ **changeGazeColor**(`color`): `void`

Sets the color of the ray from the vr headsets gaze.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `color` | [`Color3`](Color3.md) | new color for the ray. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:2333

___

### changeLaserColor

▸ **changeLaserColor**(`color`): `void`

Sets the color of the laser ray from the vr controllers.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `color` | [`Color3`](Color3.md) | new color for the ray. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:2316

___

### dispose

▸ **dispose**(): `void`

Exits VR and disposes of the vr experience helper

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:2352

___

### enableInteractions

▸ **enableInteractions**(): `void`

Enables controllers and user interactions such as selecting and object or clicking on an object.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:1384

___

### enableTeleportation

▸ **enableTeleportation**(`vrTeleportationOptions?`): `void`

Enables interactions and teleportation using the VR controllers and gaze.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vrTeleportationOptions` | [`VRTeleportationOptions`](../interfaces/VRTeleportationOptions.md) | options to modify teleportation behavior. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:1493

___

### enterVR

▸ **enterVR**(): `void`

Attempt to enter VR. If a headset is connected and ready, will request present on that.
Otherwise, will use the fullscreen API.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:1174

___

### exitVR

▸ **exitVR**(): `void`

Attempt to exit VR, or fullscreen.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:1268

___

### getClassName

▸ **getClassName**(): `string`

Gets the name of the VRExperienceHelper class

#### Returns

`string`

"VRExperienceHelper"

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:2419

___

### removeFloorMesh

▸ **removeFloorMesh**(`floorMesh`): `void`

Removes a floor mesh from being used for teleportation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `floorMesh` | [`Mesh`](Mesh.md) | the mesh to be removed. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:1478

___

### setGazeColor

▸ **setGazeColor**(`color`, `pickedColor?`): `void`

Permanently set new colors for the gaze pointer

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `color` | [`Color3`](Color3.md) | the new gaze color |
| `pickedColor` | [`Color3`](Color3.md) | the new gaze color when picked mesh detected |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:2307

___

### setLaserColor

▸ **setLaserColor**(`color`, `pickedColor?`): `void`

Permanently set new colors for the laser pointer

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `color` | [`Color3`](Color3.md) | the new laser color |
| `pickedColor` | [`Color3`](Color3.md) | the new laser color when picked mesh detected |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:2284

___

### setLaserLightingState

▸ **setLaserLightingState**(`enabled?`): `void`

Set lighting enabled / disabled on the laser pointer of both controllers

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `enabled` | `boolean` | `true` | should the lighting be enabled on the laser pointer |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:2293

___

### teleportCamera

▸ **teleportCamera**(`location`): `void`

Teleports the users feet to the desired location

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `location` | [`Vector3`](Vector3.md) | The location where the user's feet should be placed |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/VR/vrExperienceHelper.ts:2033
