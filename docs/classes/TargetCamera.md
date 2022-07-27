[@dev/core](../README.md) / [Exports](../modules.md) / TargetCamera

# Class: TargetCamera

A target camera takes a mesh or position as a target and continues to look at it while it moves.
This is the base of the follow, arc rotate cameras and Free camera

**`See`**

https://doc.babylonjs.com/features/cameras

## Hierarchy

- [`Camera`](Camera.md)

  ↳ **`TargetCamera`**

  ↳↳ [`FreeCamera`](FreeCamera.md)

  ↳↳ [`ArcRotateCamera`](ArcRotateCamera.md)

  ↳↳ [`FlyCamera`](FlyCamera.md)

  ↳↳ [`FollowCamera`](FollowCamera.md)

  ↳↳ [`ArcFollowCamera`](ArcFollowCamera.md)

## Table of contents

### Constructors

- [constructor](TargetCamera.md#constructor)

### Properties

- [\_cachedQuaternionRotationZ](TargetCamera.md#_cachedquaternionrotationz)
- [\_cachedRotationZ](TargetCamera.md#_cachedrotationz)
- [\_defaultUp](TargetCamera.md#_defaultup)
- [\_globalPosition](TargetCamera.md#_globalposition)
- [\_isDirty](TargetCamera.md#_isdirty)
- [\_parentNode](TargetCamera.md#_parentnode)
- [\_ranges](TargetCamera.md#_ranges)
- [\_storedPosition](TargetCamera.md#_storedposition)
- [\_storedRotation](TargetCamera.md#_storedrotation)
- [\_storedRotationQuaternion](TargetCamera.md#_storedrotationquaternion)
- [\_tmpQuaternion](TargetCamera.md#_tmpquaternion)
- [\_tmpTargetVector](TargetCamera.md#_tmptargetvector)
- [\_tmpUpVector](TargetCamera.md#_tmpupvector)
- [\_upVector](TargetCamera.md#_upvector)
- [\_webvrViewMatrix](TargetCamera.md#_webvrviewmatrix)
- [animations](TargetCamera.md#animations)
- [cameraDirection](TargetCamera.md#cameradirection)
- [cameraRigMode](TargetCamera.md#camerarigmode)
- [cameraRotation](TargetCamera.md#camerarotation)
- [customRenderTargets](TargetCamera.md#customrendertargets)
- [fov](TargetCamera.md#fov)
- [fovMode](TargetCamera.md#fovmode)
- [id](TargetCamera.md#id)
- [ignoreParentScaling](TargetCamera.md#ignoreparentscaling)
- [inertia](TargetCamera.md#inertia)
- [inputs](TargetCamera.md#inputs)
- [inspectableCustomProperties](TargetCamera.md#inspectablecustomproperties)
- [interaxialDistance](TargetCamera.md#interaxialdistance)
- [inverseRotationSpeed](TargetCamera.md#inverserotationspeed)
- [invertRotation](TargetCamera.md#invertrotation)
- [isIntermediate](TargetCamera.md#isintermediate)
- [isRigCamera](TargetCamera.md#isrigcamera)
- [isStereoscopicSideBySide](TargetCamera.md#isstereoscopicsidebyside)
- [layerMask](TargetCamera.md#layermask)
- [lockedTarget](TargetCamera.md#lockedtarget)
- [maxZ](TargetCamera.md#maxz)
- [metadata](TargetCamera.md#metadata)
- [minZ](TargetCamera.md#minz)
- [name](TargetCamera.md#name)
- [noRotationConstraint](TargetCamera.md#norotationconstraint)
- [onAfterCheckInputsObservable](TargetCamera.md#onaftercheckinputsobservable)
- [onDisposeObservable](TargetCamera.md#ondisposeobservable)
- [onProjectionMatrixChangedObservable](TargetCamera.md#onprojectionmatrixchangedobservable)
- [onReady](TargetCamera.md#onready)
- [onRestoreStateObservable](TargetCamera.md#onrestorestateobservable)
- [onViewMatrixChangedObservable](TargetCamera.md#onviewmatrixchangedobservable)
- [outputRenderTarget](TargetCamera.md#outputrendertarget)
- [projectionPlaneTilt](TargetCamera.md#projectionplanetilt)
- [renderPassId](TargetCamera.md#renderpassid)
- [reservedDataStore](TargetCamera.md#reserveddatastore)
- [rigParent](TargetCamera.md#rigparent)
- [rotation](TargetCamera.md#rotation)
- [rotationQuaternion](TargetCamera.md#rotationquaternion)
- [speed](TargetCamera.md#speed)
- [state](TargetCamera.md#state)
- [uniqueId](TargetCamera.md#uniqueid)
- [updateUpVectorFromRotation](TargetCamera.md#updateupvectorfromrotation)
- [viewport](TargetCamera.md#viewport)
- [FOVMODE\_HORIZONTAL\_FIXED](TargetCamera.md#fovmode_horizontal_fixed)
- [FOVMODE\_VERTICAL\_FIXED](TargetCamera.md#fovmode_vertical_fixed)
- [ForceAttachControlToAlwaysPreventDefault](TargetCamera.md#forceattachcontroltoalwayspreventdefault)
- [ORTHOGRAPHIC\_CAMERA](TargetCamera.md#orthographic_camera)
- [PERSPECTIVE\_CAMERA](TargetCamera.md#perspective_camera)
- [RIG\_MODE\_CUSTOM](TargetCamera.md#rig_mode_custom)
- [RIG\_MODE\_NONE](TargetCamera.md#rig_mode_none)
- [RIG\_MODE\_STEREOSCOPIC\_ANAGLYPH](TargetCamera.md#rig_mode_stereoscopic_anaglyph)
- [RIG\_MODE\_STEREOSCOPIC\_INTERLACED](TargetCamera.md#rig_mode_stereoscopic_interlaced)
- [RIG\_MODE\_STEREOSCOPIC\_OVERUNDER](TargetCamera.md#rig_mode_stereoscopic_overunder)
- [RIG\_MODE\_STEREOSCOPIC\_SIDEBYSIDE\_CROSSEYED](TargetCamera.md#rig_mode_stereoscopic_sidebyside_crosseyed)
- [RIG\_MODE\_STEREOSCOPIC\_SIDEBYSIDE\_PARALLEL](TargetCamera.md#rig_mode_stereoscopic_sidebyside_parallel)
- [RIG\_MODE\_VR](TargetCamera.md#rig_mode_vr)
- [RIG\_MODE\_WEBVR](TargetCamera.md#rig_mode_webvr)
- [\_RigCamTransformMatrix](TargetCamera.md#_rigcamtransformmatrix)
- [\_TargetFocalPoint](TargetCamera.md#_targetfocalpoint)
- [\_TargetTransformMatrix](TargetCamera.md#_targettransformmatrix)

### Accessors

- [absoluteRotation](TargetCamera.md#absoluterotation)
- [animationPropertiesOverride](TargetCamera.md#animationpropertiesoverride)
- [behaviors](TargetCamera.md#behaviors)
- [doNotSerialize](TargetCamera.md#donotserialize)
- [globalPosition](TargetCamera.md#globalposition)
- [isLeftCamera](TargetCamera.md#isleftcamera)
- [isRightCamera](TargetCamera.md#isrightcamera)
- [leftCamera](TargetCamera.md#leftcamera)
- [mode](TargetCamera.md#mode)
- [onClonedObservable](TargetCamera.md#onclonedobservable)
- [onDispose](TargetCamera.md#ondispose)
- [onEnabledStateChangedObservable](TargetCamera.md#onenabledstatechangedobservable)
- [orthoBottom](TargetCamera.md#orthobottom)
- [orthoLeft](TargetCamera.md#ortholeft)
- [orthoRight](TargetCamera.md#orthoright)
- [orthoTop](TargetCamera.md#orthotop)
- [parent](TargetCamera.md#parent)
- [position](TargetCamera.md#position)
- [rigPostProcess](TargetCamera.md#rigpostprocess)
- [rightCamera](TargetCamera.md#rightcamera)
- [screenArea](TargetCamera.md#screenarea)
- [target](TargetCamera.md#target)
- [upVector](TargetCamera.md#upvector)
- [worldMatrixFromCache](TargetCamera.md#worldmatrixfromcache)

### Methods

- [\_computeViewMatrix](TargetCamera.md#_computeviewmatrix)
- [\_getFirstPostProcess](TargetCamera.md#_getfirstpostprocess)
- [\_getRigCamPositionAndTarget](TargetCamera.md#_getrigcampositionandtarget)
- [\_rotateUpVectorWithCameraRotationMatrix](TargetCamera.md#_rotateupvectorwithcamerarotationmatrix)
- [\_setRigMode](TargetCamera.md#_setrigmode)
- [\_updateCameraRotationMatrix](TargetCamera.md#_updatecamerarotationmatrix)
- [\_updateWebVRCameraRotationMatrix](TargetCamera.md#_updatewebvrcamerarotationmatrix)
- [addBehavior](TargetCamera.md#addbehavior)
- [applyVerticalCorrection](TargetCamera.md#applyverticalcorrection)
- [attachControl](TargetCamera.md#attachcontrol)
- [attachPostProcess](TargetCamera.md#attachpostprocess)
- [beginAnimation](TargetCamera.md#beginanimation)
- [clone](TargetCamera.md#clone)
- [computeWorldMatrix](TargetCamera.md#computeworldmatrix)
- [createAnimationRange](TargetCamera.md#createanimationrange)
- [deleteAnimationRange](TargetCamera.md#deleteanimationrange)
- [detachControl](TargetCamera.md#detachcontrol)
- [detachPostProcess](TargetCamera.md#detachpostprocess)
- [dispose](TargetCamera.md#dispose)
- [freezeProjectionMatrix](TargetCamera.md#freezeprojectionmatrix)
- [getActiveMeshes](TargetCamera.md#getactivemeshes)
- [getAnimationByName](TargetCamera.md#getanimationbyname)
- [getAnimationRange](TargetCamera.md#getanimationrange)
- [getAnimationRanges](TargetCamera.md#getanimationranges)
- [getBehaviorByName](TargetCamera.md#getbehaviorbyname)
- [getChildMeshes](TargetCamera.md#getchildmeshes)
- [getChildren](TargetCamera.md#getchildren)
- [getClassName](TargetCamera.md#getclassname)
- [getDescendants](TargetCamera.md#getdescendants)
- [getDirection](TargetCamera.md#getdirection)
- [getDirectionToRef](TargetCamera.md#getdirectiontoref)
- [getEngine](TargetCamera.md#getengine)
- [getForwardRay](TargetCamera.md#getforwardray)
- [getForwardRayToRef](TargetCamera.md#getforwardraytoref)
- [getFrontPosition](TargetCamera.md#getfrontposition)
- [getHierarchyBoundingVectors](TargetCamera.md#gethierarchyboundingvectors)
- [getLeftTarget](TargetCamera.md#getlefttarget)
- [getProjectionMatrix](TargetCamera.md#getprojectionmatrix)
- [getRightTarget](TargetCamera.md#getrighttarget)
- [getScene](TargetCamera.md#getscene)
- [getTarget](TargetCamera.md#gettarget)
- [getTransformationMatrix](TargetCamera.md#gettransformationmatrix)
- [getViewMatrix](TargetCamera.md#getviewmatrix)
- [getWorldMatrix](TargetCamera.md#getworldmatrix)
- [isActiveMesh](TargetCamera.md#isactivemesh)
- [isCompletelyInFrustum](TargetCamera.md#iscompletelyinfrustum)
- [isDescendantOf](TargetCamera.md#isdescendantof)
- [isDisposed](TargetCamera.md#isdisposed)
- [isEnabled](TargetCamera.md#isenabled)
- [isInFrustum](TargetCamera.md#isinfrustum)
- [isReady](TargetCamera.md#isready)
- [markAsDirty](TargetCamera.md#markasdirty)
- [removeBehavior](TargetCamera.md#removebehavior)
- [restoreState](TargetCamera.md#restorestate)
- [serialize](TargetCamera.md#serialize)
- [serializeAnimationRanges](TargetCamera.md#serializeanimationranges)
- [setEnabled](TargetCamera.md#setenabled)
- [setTarget](TargetCamera.md#settarget)
- [storeState](TargetCamera.md#storestate)
- [toString](TargetCamera.md#tostring)
- [unfreezeProjectionMatrix](TargetCamera.md#unfreezeprojectionmatrix)
- [update](TargetCamera.md#update)
- [AddNodeConstructor](TargetCamera.md#addnodeconstructor)
- [Construct](TargetCamera.md#construct)
- [GetConstructorFromName](TargetCamera.md#getconstructorfromname)
- [Parse](TargetCamera.md#parse)
- [ParseAnimationRanges](TargetCamera.md#parseanimationranges)

## Constructors

### constructor

• **new TargetCamera**(`name`, `position`, `scene?`, `setActiveOnSceneIfNoneActive?`)

Instantiates a target camera that takes a mesh or position as a target and continues to look at it while it moves.
This is the base of the follow, arc rotate cameras and Free camera

**`See`**

https://doc.babylonjs.com/features/cameras

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | Defines the name of the camera in the scene |
| `position` | [`Vector3`](Vector3.md) | `undefined` | Defines the start position of the camera in the scene |
| `scene?` | [`Scene`](Scene.md) | `undefined` | Defines the scene the camera belongs to |
| `setActiveOnSceneIfNoneActive` | `boolean` | `true` | Defines whether the camera should be marked as active if not other active cameras have been defined |

#### Overrides

[Camera](Camera.md).[constructor](Camera.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/targetCamera.ts:112

## Properties

### \_cachedQuaternionRotationZ

• `Private` **\_cachedQuaternionRotationZ**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/targetCamera.ts:413

___

### \_cachedRotationZ

• `Private` **\_cachedRotationZ**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/targetCamera.ts:412

___

### \_defaultUp

• `Private` **\_defaultUp**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/targetCamera.ts:101

___

### \_globalPosition

• `Protected` **\_globalPosition**: [`Vector3`](Vector3.md)

#### Inherited from

[Camera](Camera.md).[_globalPosition](Camera.md#_globalposition)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:412

___

### \_isDirty

• `Protected` **\_isDirty**: `boolean` = `false`

#### Inherited from

[Camera](Camera.md).[_isDirty](Camera.md#_isdirty)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:43

___

### \_parentNode

• `Protected` **\_parentNode**: [`Nullable`](../modules.md#nullable)[`Node`](Node.md) = `null`

#### Inherited from

[Camera](Camera.md).[_parentNode](Camera.md#_parentnode)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:176

___

### \_ranges

• `Protected` **\_ranges**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: [`Nullable`](../modules.md#nullable)`AnimationRange`

#### Inherited from

[Camera](Camera.md).[_ranges](Camera.md#_ranges)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:154

___

### \_storedPosition

• `Private` **\_storedPosition**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/targetCamera.ts:142

___

### \_storedRotation

• `Private` **\_storedRotation**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/targetCamera.ts:143

___

### \_storedRotationQuaternion

• `Private` **\_storedRotationQuaternion**: [`Quaternion`](Quaternion.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/targetCamera.ts:144

___

### \_tmpQuaternion

• `Private` **\_tmpQuaternion**: [`Quaternion`](Quaternion.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/targetCamera.ts:37

___

### \_tmpTargetVector

• `Private` **\_tmpTargetVector**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/targetCamera.ts:19

___

### \_tmpUpVector

• `Private` **\_tmpUpVector**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/targetCamera.ts:18

___

### \_upVector

• `Protected` **\_upVector**: [`Vector3`](Vector3.md)

#### Inherited from

[Camera](Camera.md).[_upVector](Camera.md#_upvector)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:129

___

### \_webvrViewMatrix

• `Protected` **\_webvrViewMatrix**: [`Matrix`](Matrix.md)

#### Inherited from

[Camera](Camera.md).[_webvrViewMatrix](Camera.md#_webvrviewmatrix)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:399

___

### animations

• **animations**: [`Animation`](Animation.md)[]

Gets a list of Animations associated with the node

#### Inherited from

[Camera](Camera.md).[animations](Camera.md#animations)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:153

___

### cameraDirection

• **cameraDirection**: [`Vector3`](Vector3.md)

Define the current direction the camera is moving to

#### Defined in

https://github.com/babylon.js/core/src/Cameras/targetCamera.ts:24

___

### cameraRigMode

• **cameraRigMode**: `number` = `Camera.RIG_MODE_NONE`

Rig mode of the camera.
This is useful to create the camera with two "eyes" instead of one to create VR or stereoscopic scenes.
This is normally controlled byt the camera themselves as internal use.

#### Inherited from

[Camera](Camera.md).[cameraRigMode](Camera.md#camerarigmode)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:330

___

### cameraRotation

• **cameraRotation**: [`Vector2`](Vector2.md)

Define the current rotation the camera is rotating to

#### Defined in

https://github.com/babylon.js/core/src/Cameras/targetCamera.ts:28

___

### customRenderTargets

• **customRenderTargets**: [`RenderTargetTexture`](RenderTargetTexture.md)[]

Defines the list of custom render target which are rendered to and then used as the input to this camera's render. Eg. display another camera view on a TV in the main scene
This is pretty helpful if you wish to make a camera render to a texture you could reuse somewhere
else in the scene. (Eg. security camera)

To change the final output target of the camera, camera.outputRenderTarget should be used instead (eg. webXR renders to a render target corresponding to an HMD)

#### Inherited from

[Camera](Camera.md).[customRenderTargets](Camera.md#customrendertargets)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:351

___

### fov

• **fov**: `number` = `0.8`

Field Of View is set in Radians. (default is 0.8)

#### Inherited from

[Camera](Camera.md).[fov](Camera.md#fov)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:248

___

### fovMode

• **fovMode**: `number` = `Camera.FOVMODE_VERTICAL_FIXED`

fovMode sets the camera frustum bounds to the viewport bounds. (default is FOVMODE_VERTICAL_FIXED)

#### Inherited from

[Camera](Camera.md).[fovMode](Camera.md#fovmode)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:322

___

### id

• **id**: `string`

Gets or sets the id of the node

#### Inherited from

[Camera](Camera.md).[id](Camera.md#id)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:97

___

### ignoreParentScaling

• **ignoreParentScaling**: `boolean` = `false`

Gets or sets a boolean indicating that the scaling of the parent hierarchy will not be taken in account by the camera

#### Defined in

https://github.com/babylon.js/core/src/Cameras/targetCamera.ts:31

___

### inertia

• **inertia**: `number` = `0.9`

Define the default inertia of the camera.
This helps giving a smooth feeling to the camera movement.

#### Inherited from

[Camera](Camera.md).[inertia](Camera.md#inertia)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:279

___

### inputs

• **inputs**: [`CameraInputsManager`](CameraInputsManager.md)[`Camera`](Camera.md)

Define the input manager associated with the camera.

#### Inherited from

[Camera](Camera.md).[inputs](Camera.md#inputs)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:111

___

### inspectableCustomProperties

• **inspectableCustomProperties**: [`IInspectable`](../interfaces/IInspectable.md)[]

List of inspectable custom properties (used by the Inspector)

**`See`**

https://doc.babylonjs.com/how_to/debug_layer#extensibility

#### Inherited from

[Camera](Camera.md).[inspectableCustomProperties](Camera.md#inspectablecustomproperties)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:126

___

### interaxialDistance

• **interaxialDistance**: `number`

Defines the distance between both "eyes" in case of a RIG

#### Inherited from

[Camera](Camera.md).[interaxialDistance](Camera.md#interaxialdistance)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:336

___

### inverseRotationSpeed

• **inverseRotationSpeed**: `number` = `0.2`

Speed multiplier for inverse camera panning

#### Defined in

https://github.com/babylon.js/core/src/Cameras/targetCamera.ts:71

___

### invertRotation

• **invertRotation**: `boolean` = `false`

Reverses mouselook direction to 'natural' panning as opposed to traditional direct
panning

#### Defined in

https://github.com/babylon.js/core/src/Cameras/targetCamera.ts:66

___

### isIntermediate

• **isIntermediate**: `boolean` = `false`

Define whether the camera is intermediate.
This is useful to not present the output directly to the screen in case of rig without post process for instance

#### Inherited from

[Camera](Camera.md).[isIntermediate](Camera.md#isintermediate)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:303

___

### isRigCamera

• **isRigCamera**: `boolean` = `false`

Is this camera a part of a rig system?

#### Inherited from

[Camera](Camera.md).[isRigCamera](Camera.md#isrigcamera)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:379

___

### isStereoscopicSideBySide

• **isStereoscopicSideBySide**: `boolean`

Defines if stereoscopic rendering is done side by side or over under.

#### Inherited from

[Camera](Camera.md).[isStereoscopicSideBySide](Camera.md#isstereoscopicsidebyside)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:342

___

### layerMask

• **layerMask**: `number` = `0x0fffffff`

Restricts the camera to viewing objects with the same layerMask.
A camera with a layerMask of 1 will render mesh.layerMask & camera.layerMask!== 0

#### Inherited from

[Camera](Camera.md).[layerMask](Camera.md#layermask)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:316

___

### lockedTarget

• **lockedTarget**: `any` = `null`

Define the current target of the camera as an object or a position.
Please note that locking a target will disable panning.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/targetCamera.ts:78

___

### maxZ

• **maxZ**: `number` = `10000.0`

Define the maximum distance the camera can see to.
This is important to note that the depth buffer are not infinite and the further it end
the more your scene might encounter depth fighting issue.

#### Inherited from

[Camera](Camera.md).[maxZ](Camera.md#maxz)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:272

___

### metadata

• **metadata**: `any` = `null`

Gets or sets an object used to store user defined information for the node

#### Inherited from

[Camera](Camera.md).[metadata](Camera.md#metadata)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:115

___

### minZ

• **minZ**: `number` = `1`

Define the minimum distance the camera can see from.
This is important to note that the depth buffer are not infinite and the closer it starts
the more your scene might encounter depth fighting issue.

#### Inherited from

[Camera](Camera.md).[minZ](Camera.md#minz)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:264

___

### name

• **name**: `string`

Gets or sets the name of the node

#### Inherited from

[Camera](Camera.md).[name](Camera.md#name)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:91

___

### noRotationConstraint

• **noRotationConstraint**: `boolean` = `false`

Add constraint to the camera to prevent it to move freely in all directions and
around all axis.

#### Defined in

https://github.com/babylon.js/core/src/Cameras/targetCamera.ts:60

___

### onAfterCheckInputsObservable

• **onAfterCheckInputsObservable**: [`Observable`](Observable.md)[`Camera`](Camera.md)

Observable triggered when the inputs have been processed.

#### Inherited from

[Camera](Camera.md).[onAfterCheckInputsObservable](Camera.md#onaftercheckinputsobservable)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:370

___

### onDisposeObservable

• **onDisposeObservable**: [`Observable`](Observable.md)[`Node`](Node.md)

An event triggered when the mesh is disposed

#### Inherited from

[Camera](Camera.md).[onDisposeObservable](Camera.md#ondisposeobservable)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:300

___

### onProjectionMatrixChangedObservable

• **onProjectionMatrixChangedObservable**: [`Observable`](Observable.md)[`Camera`](Camera.md)

Observable triggered when the camera Projection matrix has changed.

#### Inherited from

[Camera](Camera.md).[onProjectionMatrixChangedObservable](Camera.md#onprojectionmatrixchangedobservable)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:366

___

### onReady

• **onReady**: [`Nullable`](../modules.md#nullable)(`node`: [`Node`](Node.md)) => `void` = `null`

Callback raised when the node is ready to be used

#### Inherited from

[Camera](Camera.md).[onReady](Camera.md#onready)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:159

___

### onRestoreStateObservable

• **onRestoreStateObservable**: [`Observable`](Observable.md)[`Camera`](Camera.md)

Observable triggered when reset has been called and applied to the camera.

#### Inherited from

[Camera](Camera.md).[onRestoreStateObservable](Camera.md#onrestorestateobservable)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:374

___

### onViewMatrixChangedObservable

• **onViewMatrixChangedObservable**: [`Observable`](Observable.md)[`Camera`](Camera.md)

Observable triggered when the camera view matrix has changed.

#### Inherited from

[Camera](Camera.md).[onViewMatrixChangedObservable](Camera.md#onviewmatrixchangedobservable)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:362

___

### outputRenderTarget

• **outputRenderTarget**: [`Nullable`](../modules.md#nullable)[`RenderTargetTexture`](RenderTargetTexture.md) = `null`

When set, the camera will render to this render target instead of the default canvas

If the desire is to use the output of a camera as a texture in the scene consider using camera.customRenderTargets instead

#### Inherited from

[Camera](Camera.md).[outputRenderTarget](Camera.md#outputrendertarget)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:357

___

### projectionPlaneTilt

• **projectionPlaneTilt**: `number` = `0`

Projection plane tilt around the X axis (horizontal), set in Radians. (default is 0)
Can be used to make vertical lines in world space actually vertical on the screen.
See https://forum.babylonjs.com/t/add-vertical-shift-to-3ds-max-exporter-babylon-cameras/17480

#### Inherited from

[Camera](Camera.md).[projectionPlaneTilt](Camera.md#projectionplanetilt)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:256

___

### renderPassId

• **renderPassId**: `number`

Render pass id used by the camera to render into the main framebuffer

#### Inherited from

[Camera](Camera.md).[renderPassId](Camera.md#renderpassid)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:390

___

### reservedDataStore

• **reservedDataStore**: `any` = `null`

For internal use only. Please do not use.

#### Inherited from

[Camera](Camera.md).[reservedDataStore](Camera.md#reserveddatastore)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:120

___

### rigParent

• `Optional` **rigParent**: [`Camera`](Camera.md)

If isRigCamera set to true this will be set with the parent camera.
The parent camera is not (!) necessarily the .parent of this camera (like in the case of XR)

#### Inherited from

[Camera](Camera.md).[rigParent](Camera.md#rigparent)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:385

___

### rotation

• **rotation**: [`Vector3`](Vector3.md)

Define the current rotation of the camera

#### Defined in

https://github.com/babylon.js/core/src/Cameras/targetCamera.ts:43

___

### rotationQuaternion

• **rotationQuaternion**: [`Quaternion`](Quaternion.md)

Define the current rotation of the camera as a quaternion to prevent Gimbal lock

#### Defined in

https://github.com/babylon.js/core/src/Cameras/targetCamera.ts:48

___

### speed

• **speed**: `number` = `2.0`

Define the current speed of the camera

#### Defined in

https://github.com/babylon.js/core/src/Cameras/targetCamera.ts:54

___

### state

• **state**: `string` = `""`

Gets or sets a string used to store user defined state for the node

#### Inherited from

[Camera](Camera.md).[state](Camera.md#state)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:109

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the node

#### Inherited from

[Camera](Camera.md).[uniqueId](Camera.md#uniqueid)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:103

___

### updateUpVectorFromRotation

• **updateUpVectorFromRotation**: `boolean` = `false`

When set, the up vector of the camera will be updated by the rotation of the camera

#### Defined in

https://github.com/babylon.js/core/src/Cameras/targetCamera.ts:36

___

### viewport

• **viewport**: [`Viewport`](Viewport.md)

Define the viewport of the camera.
This correspond to the portion of the screen the camera will render to in normalized 0 to 1 unit.

#### Inherited from

[Camera](Camera.md).[viewport](Camera.md#viewport)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:309

___

### FOVMODE\_HORIZONTAL\_FIXED

▪ `Static` `Readonly` **FOVMODE\_HORIZONTAL\_FIXED**: ``1``

This setting aligns the left and right bounds of the viewport to the left and right bounds of the camera frustum.

#### Inherited from

[Camera](Camera.md).[FOVMODE_HORIZONTAL_FIXED](Camera.md#fovmode_horizontal_fixed)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:62

___

### FOVMODE\_VERTICAL\_FIXED

▪ `Static` `Readonly` **FOVMODE\_VERTICAL\_FIXED**: ``0``

This is the default FOV mode for perspective cameras.
This setting aligns the upper and lower bounds of the viewport to the upper and lower bounds of the camera frustum.

#### Inherited from

[Camera](Camera.md).[FOVMODE_VERTICAL_FIXED](Camera.md#fovmode_vertical_fixed)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:58

___

### ForceAttachControlToAlwaysPreventDefault

▪ `Static` **ForceAttachControlToAlwaysPreventDefault**: `boolean` = `false`

Defines if by default attaching controls should prevent the default javascript event to continue.

#### Inherited from

[Camera](Camera.md).[ForceAttachControlToAlwaysPreventDefault](Camera.md#forceattachcontroltoalwayspreventdefault)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:106

___

### ORTHOGRAPHIC\_CAMERA

▪ `Static` `Readonly` **ORTHOGRAPHIC\_CAMERA**: ``1``

This helps creating camera with an orthographic mode.
Orthographic is commonly used in engineering as a means to produce object specifications that communicate dimensions unambiguously, each line of 1 unit length (cm, meter..whatever) will appear to have the same length everywhere on the drawing. This allows the drafter to dimension only a subset of lines and let the reader know that other lines of that length on the drawing are also that length in reality. Every parallel line in the drawing is also parallel in the object.

#### Inherited from

[Camera](Camera.md).[ORTHOGRAPHIC_CAMERA](Camera.md#orthographic_camera)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:52

___

### PERSPECTIVE\_CAMERA

▪ `Static` `Readonly` **PERSPECTIVE\_CAMERA**: ``0``

This is the default projection mode used by the cameras.
It helps recreating a feeling of perspective and better appreciate depth.
This is the best way to simulate real life cameras.

#### Inherited from

[Camera](Camera.md).[PERSPECTIVE_CAMERA](Camera.md#perspective_camera)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:47

___

### RIG\_MODE\_CUSTOM

▪ `Static` `Readonly` **RIG\_MODE\_CUSTOM**: ``22``

Custom rig mode allowing rig cameras to be populated manually with any number of cameras

#### Inherited from

[Camera](Camera.md).[RIG_MODE_CUSTOM](Camera.md#rig_mode_custom)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:101

___

### RIG\_MODE\_NONE

▪ `Static` `Readonly` **RIG\_MODE\_NONE**: ``0``

This specifies there is no need for a camera rig.
Basically only one eye is rendered corresponding to the camera.

#### Inherited from

[Camera](Camera.md).[RIG_MODE_NONE](Camera.md#rig_mode_none)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:68

___

### RIG\_MODE\_STEREOSCOPIC\_ANAGLYPH

▪ `Static` `Readonly` **RIG\_MODE\_STEREOSCOPIC\_ANAGLYPH**: ``10``

Simulates a camera Rig with one blue eye and one red eye.
This can be use with 3d blue and red glasses.

#### Inherited from

[Camera](Camera.md).[RIG_MODE_STEREOSCOPIC_ANAGLYPH](Camera.md#rig_mode_stereoscopic_anaglyph)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:73

___

### RIG\_MODE\_STEREOSCOPIC\_INTERLACED

▪ `Static` `Readonly` **RIG\_MODE\_STEREOSCOPIC\_INTERLACED**: ``14``

Defines that both eyes of the camera will be rendered on successive lines interlaced for passive 3d monitors.

#### Inherited from

[Camera](Camera.md).[RIG_MODE_STEREOSCOPIC_INTERLACED](Camera.md#rig_mode_stereoscopic_interlaced)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:89

___

### RIG\_MODE\_STEREOSCOPIC\_OVERUNDER

▪ `Static` `Readonly` **RIG\_MODE\_STEREOSCOPIC\_OVERUNDER**: ``13``

Defines that both eyes of the camera will be rendered over under each other.

#### Inherited from

[Camera](Camera.md).[RIG_MODE_STEREOSCOPIC_OVERUNDER](Camera.md#rig_mode_stereoscopic_overunder)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:85

___

### RIG\_MODE\_STEREOSCOPIC\_SIDEBYSIDE\_CROSSEYED

▪ `Static` `Readonly` **RIG\_MODE\_STEREOSCOPIC\_SIDEBYSIDE\_CROSSEYED**: ``12``

Defines that both eyes of the camera will be rendered side by side with a none parallel target.

#### Inherited from

[Camera](Camera.md).[RIG_MODE_STEREOSCOPIC_SIDEBYSIDE_CROSSEYED](Camera.md#rig_mode_stereoscopic_sidebyside_crosseyed)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:81

___

### RIG\_MODE\_STEREOSCOPIC\_SIDEBYSIDE\_PARALLEL

▪ `Static` `Readonly` **RIG\_MODE\_STEREOSCOPIC\_SIDEBYSIDE\_PARALLEL**: ``11``

Defines that both eyes of the camera will be rendered side by side with a parallel target.

#### Inherited from

[Camera](Camera.md).[RIG_MODE_STEREOSCOPIC_SIDEBYSIDE_PARALLEL](Camera.md#rig_mode_stereoscopic_sidebyside_parallel)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:77

___

### RIG\_MODE\_VR

▪ `Static` `Readonly` **RIG\_MODE\_VR**: ``20``

Defines that both eyes of the camera should be renderered in a VR mode (carbox).

#### Inherited from

[Camera](Camera.md).[RIG_MODE_VR](Camera.md#rig_mode_vr)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:93

___

### RIG\_MODE\_WEBVR

▪ `Static` `Readonly` **RIG\_MODE\_WEBVR**: ``21``

Defines that both eyes of the camera should be renderered in a VR mode (webVR).

#### Inherited from

[Camera](Camera.md).[RIG_MODE_WEBVR](Camera.md#rig_mode_webvr)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:97

___

### \_RigCamTransformMatrix

▪ `Static` `Private` **\_RigCamTransformMatrix**: [`Matrix`](Matrix.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/targetCamera.ts:14

___

### \_TargetFocalPoint

▪ `Static` `Private` **\_TargetFocalPoint**: [`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/targetCamera.ts:16

___

### \_TargetTransformMatrix

▪ `Static` `Private` **\_TargetTransformMatrix**: [`Matrix`](Matrix.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/targetCamera.ts:15

## Accessors

### absoluteRotation

• `get` **absoluteRotation**(): [`Quaternion`](Quaternion.md)

Returns the current camera absolute rotation

#### Returns

[`Quaternion`](Quaternion.md)

#### Inherited from

Camera.absoluteRotation

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:1378

___

### animationPropertiesOverride

• `get` **animationPropertiesOverride**(): [`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md)

Gets or sets the animation properties override

#### Returns

[`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md)

#### Inherited from

Camera.animationPropertiesOverride

#### Defined in

https://github.com/babylon.js/core/src/node.ts:275

• `set` **animationPropertiesOverride**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md) |

#### Returns

`void`

#### Inherited from

Camera.animationPropertiesOverride

#### Defined in

https://github.com/babylon.js/core/src/node.ts:282

___

### behaviors

• `get` **behaviors**(): [`Behavior`](../interfaces/Behavior.md)[`Node`](Node.md)[]

Gets the list of attached behaviors

**`See`**

https://doc.babylonjs.com/features/behaviour

#### Returns

[`Behavior`](../interfaces/Behavior.md)[`Node`](Node.md)[]

#### Inherited from

Camera.behaviors

#### Defined in

https://github.com/babylon.js/core/src/node.ts:410

___

### doNotSerialize

• `get` **doNotSerialize**(): `boolean`

Gets or sets a boolean used to define if the node must be serialized

#### Returns

`boolean`

#### Inherited from

Camera.doNotSerialize

#### Defined in

https://github.com/babylon.js/core/src/node.ts:131

• `set` **doNotSerialize**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

Camera.doNotSerialize

#### Defined in

https://github.com/babylon.js/core/src/node.ts:143

___

### globalPosition

• `get` **globalPosition**(): [`Vector3`](Vector3.md)

Gets the current world space position of the camera.

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

Camera.globalPosition

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:522

___

### isLeftCamera

• `get` **isLeftCamera**(): `boolean`

Gets the left camera of a rig setup in case of Rigged Camera

#### Returns

`boolean`

#### Inherited from

Camera.isLeftCamera

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:1120

___

### isRightCamera

• `get` **isRightCamera**(): `boolean`

Gets the right camera of a rig setup in case of Rigged Camera

#### Returns

`boolean`

#### Inherited from

Camera.isRightCamera

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:1129

___

### leftCamera

• `get` **leftCamera**(): [`Nullable`](../modules.md#nullable)[`FreeCamera`](FreeCamera.md)

Gets the left camera of a rig setup in case of Rigged Camera

#### Returns

[`Nullable`](../modules.md#nullable)[`FreeCamera`](FreeCamera.md)

#### Inherited from

Camera.leftCamera

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:1136

___

### mode

• `get` **mode**(): `number`

#### Returns

`number`

#### Inherited from

Camera.mode

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:294

• `set` **mode**(`mode`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `mode` | `number` |

#### Returns

`void`

#### Inherited from

Camera.mode

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:285

___

### onClonedObservable

• `get` **onClonedObservable**(): [`Observable`](Observable.md)[`Node`](Node.md)

An event triggered when the node is cloned

#### Returns

[`Observable`](Observable.md)[`Node`](Node.md)

#### Inherited from

Camera.onClonedObservable

#### Defined in

https://github.com/babylon.js/core/src/node.ts:323

___

### onDispose

• `set` **onDispose**(`callback`): `void`

Sets a callback that will be raised when the node will be disposed

#### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | () => `void` |

#### Returns

`void`

#### Inherited from

Camera.onDispose

#### Defined in

https://github.com/babylon.js/core/src/node.ts:306

___

### onEnabledStateChangedObservable

• `get` **onEnabledStateChangedObservable**(): [`Observable`](Observable.md)`boolean`

An event triggered when the enabled state of the node changes

#### Returns

[`Observable`](Observable.md)`boolean`

#### Inherited from

Camera.onEnabledStateChangedObservable

#### Defined in

https://github.com/babylon.js/core/src/node.ts:316

___

### orthoBottom

• `get` **orthoBottom**(): [`Nullable`](../modules.md#nullable)`number`

#### Returns

[`Nullable`](../modules.md#nullable)`number`

#### Inherited from

Camera.orthoBottom

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:220

• `set` **orthoBottom**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)`number` |

#### Returns

`void`

#### Inherited from

Camera.orthoBottom

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:212

___

### orthoLeft

• `get` **orthoLeft**(): [`Nullable`](../modules.md#nullable)`number`

#### Returns

[`Nullable`](../modules.md#nullable)`number`

#### Inherited from

Camera.orthoLeft

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:182

• `set` **orthoLeft**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)`number` |

#### Returns

`void`

#### Inherited from

Camera.orthoLeft

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:174

___

### orthoRight

• `get` **orthoRight**(): [`Nullable`](../modules.md#nullable)`number`

#### Returns

[`Nullable`](../modules.md#nullable)`number`

#### Inherited from

Camera.orthoRight

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:201

• `set` **orthoRight**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)`number` |

#### Returns

`void`

#### Inherited from

Camera.orthoRight

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:193

___

### orthoTop

• `get` **orthoTop**(): [`Nullable`](../modules.md#nullable)`number`

#### Returns

[`Nullable`](../modules.md#nullable)`number`

#### Inherited from

Camera.orthoTop

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:239

• `set` **orthoTop**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)`number` |

#### Returns

`void`

#### Inherited from

Camera.orthoTop

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:231

___

### parent

• `get` **parent**(): [`Nullable`](../modules.md#nullable)[`Node`](Node.md)

#### Returns

[`Nullable`](../modules.md#nullable)[`Node`](Node.md)

#### Inherited from

Camera.parent

#### Defined in

https://github.com/babylon.js/core/src/node.ts:238

• `set` **parent**(`parent`): `void`

Gets or sets the parent of the node (without keeping the current position in the scene)

**`See`**

https://doc.babylonjs.com/how_to/parenting

#### Parameters

| Name | Type |
| :------ | :------ |
| `parent` | [`Nullable`](../modules.md#nullable)[`Node`](Node.md) |

#### Returns

`void`

#### Inherited from

Camera.parent

#### Defined in

https://github.com/babylon.js/core/src/node.ts:200

___

### position

• `get` **position**(): [`Vector3`](Vector3.md)

Define the current local position of the camera in the scene

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

Camera.position

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:120

• `set` **position**(`newPosition`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `newPosition` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Inherited from

Camera.position

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:124

___

### rigPostProcess

• `get` **rigPostProcess**(): [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)

Gets the post process used by the rig cameras

#### Returns

[`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)

#### Inherited from

Camera.rigPostProcess

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:697

___

### rightCamera

• `get` **rightCamera**(): [`Nullable`](../modules.md#nullable)[`FreeCamera`](FreeCamera.md)

Gets the right camera of a rig setup in case of Rigged Camera

#### Returns

[`Nullable`](../modules.md#nullable)[`FreeCamera`](FreeCamera.md)

#### Inherited from

Camera.rightCamera

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:1146

___

### screenArea

• `get` **screenArea**(): `number`

The screen area in scene units squared

#### Returns

`number`

#### Inherited from

Camera.screenArea

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:146

___

### target

• `get` **target**(): [`Vector3`](Vector3.md)

Defines the target point of the camera.
The camera looks towards it form the radius distance.

#### Returns

[`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/targetCamera.ts:292

• `set` **target**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/targetCamera.ts:295

___

### upVector

• `get` **upVector**(): [`Vector3`](Vector3.md)

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

Camera.upVector

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:139

• `set` **upVector**(`vec`): `void`

The vector the camera should consider as up.
(default is Vector3(0, 1, 0) aka Vector3.Up())

#### Parameters

| Name | Type |
| :------ | :------ |
| `vec` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Inherited from

Camera.upVector

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:135

___

### worldMatrixFromCache

• `get` **worldMatrixFromCache**(): [`Matrix`](Matrix.md)

Returns directly the latest state of the mesh World matrix.
A Matrix is returned.

#### Returns

[`Matrix`](Matrix.md)

#### Inherited from

Camera.worldMatrixFromCache

#### Defined in

https://github.com/babylon.js/core/src/node.ts:454

## Methods

### \_computeViewMatrix

▸ `Protected` **_computeViewMatrix**(`position`, `target`, `up`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `position` | [`Vector3`](Vector3.md) |
| `target` | [`Vector3`](Vector3.md) |
| `up` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/targetCamera.ts:448

___

### \_getFirstPostProcess

▸ **_getFirstPostProcess**(): [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)

Internal, gets the first post process.

#### Returns

[`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)

the first post process to be run on this camera.

#### Inherited from

[Camera](Camera.md).[_getFirstPostProcess](Camera.md#_getfirstpostprocess)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:705

___

### \_getRigCamPositionAndTarget

▸ `Private` **_getRigCamPositionAndTarget**(`halfSpace`, `rigCamera`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `halfSpace` | `number` |
| `rigCamera` | [`TargetCamera`](TargetCamera.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/targetCamera.ts:556

___

### \_rotateUpVectorWithCameraRotationMatrix

▸ `Private` **_rotateUpVectorWithCameraRotationMatrix**(): [`TargetCamera`](TargetCamera.md)

Update the up vector to apply the rotation of the camera (So if you changed the camera rotation.z this will let you update the up vector as well)

#### Returns

[`TargetCamera`](TargetCamera.md)

the current camera

#### Defined in

https://github.com/babylon.js/core/src/Cameras/targetCamera.ts:407

___

### \_setRigMode

▸ `Protected` **_setRigMode**(`rigParams`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `rigParams` | `any` |

#### Returns

`void`

#### Inherited from

[Camera](Camera.md).[_setRigMode](Camera.md#_setrigmode)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:1222

___

### \_updateCameraRotationMatrix

▸ `Protected` **_updateCameraRotationMatrix**(): `void`

#### Returns

`void`

#### Overrides

[Camera](Camera.md).[_updateCameraRotationMatrix](Camera.md#_updatecamerarotationmatrix)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/targetCamera.ts:395

___

### \_updateWebVRCameraRotationMatrix

▸ `Protected` **_updateWebVRCameraRotationMatrix**(): `void`

#### Returns

`void`

#### Inherited from

[Camera](Camera.md).[_updateWebVRCameraRotationMatrix](Camera.md#_updatewebvrcamerarotationmatrix)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:1245

___

### addBehavior

▸ **addBehavior**(`behavior`, `attachImmediately?`): [`Node`](Node.md)

Attach a behavior to the node

**`See`**

https://doc.babylonjs.com/features/behaviour

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `behavior` | [`Behavior`](../interfaces/Behavior.md)[`Node`](Node.md) | `undefined` | defines the behavior to attach |
| `attachImmediately` | `boolean` | `false` | defines that the behavior must be attached even if the scene is still loading |

#### Returns

[`Node`](Node.md)

the current Node

#### Inherited from

[Camera](Camera.md).[addBehavior](Camera.md#addbehavior)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:366

___

### applyVerticalCorrection

▸ **applyVerticalCorrection**(): `void`

Automatically tilts the projection plane, using `projectionPlaneTilt`, to correct the perspective effect on vertical lines.

#### Returns

`void`

#### Inherited from

[Camera](Camera.md).[applyVerticalCorrection](Camera.md#applyverticalcorrection)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:513

___

### attachControl

▸ **attachControl**(`noPreventDefault?`): `void`

Attach the input controls to a specific dom element to get the input from.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `noPreventDefault?` | `boolean` | Defines whether event caught by the controls should call preventdefault() (https://developer.mozilla.org/en-US/docs/Web/API/Event/preventDefault) |

#### Returns

`void`

#### Inherited from

[Camera](Camera.md).[attachControl](Camera.md#attachcontrol)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:642

▸ **attachControl**(`ignored`, `noPreventDefault?`): `void`

Attach the input controls to a specific dom element to get the input from.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ignored` | `any` | defines an ignored parameter kept for backward compatibility. |
| `noPreventDefault?` | `boolean` | Defines whether event caught by the controls should call preventdefault() (https://developer.mozilla.org/en-US/docs/Web/API/Event/preventDefault)  BACK COMPAT SIGNATURE ONLY. |

#### Returns

`void`

#### Inherited from

[Camera](Camera.md).[attachControl](Camera.md#attachcontrol)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:649

___

### attachPostProcess

▸ **attachPostProcess**(`postProcess`, `insertAt?`): `number`

Attach a post process to the camera.

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_postprocesses#attach-postprocess

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `postProcess` | [`PostProcess`](PostProcess.md) | `undefined` | The post process to attach to the camera |
| `insertAt` | [`Nullable`](../modules.md#nullable)`number` | `null` | The position of the post process in case several of them are in use in the scene |

#### Returns

`number`

the position the post process has been inserted at

#### Inherited from

[Camera](Camera.md).[attachPostProcess](Camera.md#attachpostprocess)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:748

___

### beginAnimation

▸ **beginAnimation**(`name`, `loop?`, `speedRatio?`, `onAnimationEnd?`): [`Nullable`](../modules.md#nullable)[`Animatable`](Animatable.md)

Will start the animation sequence

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the range frames for animation sequence |
| `loop?` | `boolean` | defines if the animation should loop (false by default) |
| `speedRatio?` | `number` | defines the speed factor in which to run the animation (1 by default) |
| `onAnimationEnd?` | () => `void` | defines a function to be executed when the animation ended (undefined by default) |

#### Returns

[`Nullable`](../modules.md#nullable)[`Animatable`](Animatable.md)

the object created for this animation. If range does not exist, it will return null

#### Inherited from

[Camera](Camera.md).[beginAnimation](Camera.md#beginanimation)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:833

___

### clone

▸ **clone**(`name`, `newParent?`): [`Camera`](Camera.md)

Clones the current camera.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | The cloned camera name |
| `newParent` | [`Nullable`](../modules.md#nullable)[`Node`](Node.md) | `null` | The cloned camera's new parent (none by default) |

#### Returns

[`Camera`](Camera.md)

the cloned camera

#### Inherited from

[Camera](Camera.md).[clone](Camera.md#clone)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:1349

___

### computeWorldMatrix

▸ **computeWorldMatrix**(): [`Matrix`](Matrix.md)

Compute the world  matrix of the camera.

#### Returns

[`Matrix`](Matrix.md)

the camera world matrix

#### Inherited from

[Camera](Camera.md).[computeWorldMatrix](Camera.md#computeworldmatrix)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:1422

___

### createAnimationRange

▸ **createAnimationRange**(`name`, `from`, `to`): `void`

Creates an animation range for this node

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the name of the range |
| `from` | `number` | defines the starting key |
| `to` | `number` | defines the end key |

#### Returns

`void`

#### Inherited from

[Camera](Camera.md).[createAnimationRange](Camera.md#createanimationrange)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:777

___

### deleteAnimationRange

▸ **deleteAnimationRange**(`name`, `deleteFrames?`): `void`

Delete a specific animation range

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | defines the name of the range to delete |
| `deleteFrames` | `boolean` | `true` | defines if animation frames from the range must be deleted as well |

#### Returns

`void`

#### Inherited from

[Camera](Camera.md).[deleteAnimationRange](Camera.md#deleteanimationrange)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:794

___

### detachControl

▸ **detachControl**(): `void`

Detach the current controls from the specified dom element.

#### Returns

`void`

#### Inherited from

[Camera](Camera.md).[detachControl](Camera.md#detachcontrol)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:661

▸ **detachControl**(`ignored?`): `void`

Detach the current controls from the specified dom element.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ignored?` | `any` | defines an ignored parameter kept for backward compatibility. |

#### Returns

`void`

#### Inherited from

[Camera](Camera.md).[detachControl](Camera.md#detachcontrol)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:666

___

### detachPostProcess

▸ **detachPostProcess**(`postProcess`): `void`

Detach a post process to the camera.

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_postprocesses#attach-postprocess

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `postProcess` | [`PostProcess`](PostProcess.md) | The post process to detach from the camera |

#### Returns

`void`

#### Inherited from

[Camera](Camera.md).[detachPostProcess](Camera.md#detachpostprocess)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:776

___

### dispose

▸ **dispose**(`doNotRecurse?`, `disposeMaterialAndTextures?`): `void`

Releases resources associated with this node.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `doNotRecurse?` | `boolean` | `undefined` | Set to true to not recurse into each children (recurse into each children by default) |
| `disposeMaterialAndTextures` | `boolean` | `false` | Set to true to also dispose referenced materials and textures (false by default) |

#### Returns

`void`

#### Inherited from

[Camera](Camera.md).[dispose](Camera.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:1050

___

### freezeProjectionMatrix

▸ **freezeProjectionMatrix**(`projection?`): `void`

Freeze the projection matrix.
It will prevent the cache check of the camera projection compute and can speed up perf
if no parameter of the camera are meant to change

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `projection?` | [`Matrix`](Matrix.md) | Defines manually a projection if necessary |

#### Returns

`void`

#### Inherited from

[Camera](Camera.md).[freezeProjectionMatrix](Camera.md#freezeprojectionmatrix)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:848

___

### getActiveMeshes

▸ **getActiveMeshes**(): [`SmartArray`](SmartArray.md)[`AbstractMesh`](AbstractMesh.md)

Gets the list of active meshes this frame (meshes no culled or excluded by lod s in the frame)

#### Returns

[`SmartArray`](SmartArray.md)[`AbstractMesh`](AbstractMesh.md)

the active meshe list

#### Inherited from

[Camera](Camera.md).[getActiveMeshes](Camera.md#getactivemeshes)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:530

___

### getAnimationByName

▸ **getAnimationByName**(`name`): [`Nullable`](../modules.md#nullable)[`Animation`](Animation.md)

Get an animation by name

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the name of the animation to look for |

#### Returns

[`Nullable`](../modules.md#nullable)[`Animation`](Animation.md)

null if not found else the requested animation

#### Inherited from

[Camera](Camera.md).[getAnimationByName](Camera.md#getanimationbyname)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:759

___

### getAnimationRange

▸ **getAnimationRange**(`name`): [`Nullable`](../modules.md#nullable)[`AnimationRange`](AnimationRange.md)

Get an animation range by name

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the name of the animation range to look for |

#### Returns

[`Nullable`](../modules.md#nullable)[`AnimationRange`](AnimationRange.md)

null if not found else the requested animation range

#### Inherited from

[Camera](Camera.md).[getAnimationRange](Camera.md#getanimationrange)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:808

___

### getAnimationRanges

▸ **getAnimationRanges**(): [`Nullable`](../modules.md#nullable)[`AnimationRange`](AnimationRange.md)[]

Gets the list of all animation ranges defined on this node

#### Returns

[`Nullable`](../modules.md#nullable)[`AnimationRange`](AnimationRange.md)[]

an array

#### Inherited from

[Camera](Camera.md).[getAnimationRanges](Camera.md#getanimationranges)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:816

___

### getBehaviorByName

▸ **getBehaviorByName**(`name`): [`Nullable`](../modules.md#nullable)[`Behavior`](../interfaces/Behavior.md)[`Node`](Node.md)

Gets an attached behavior by name

**`See`**

https://doc.babylonjs.com/features/behaviour

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the name of the behavior to look for |

#### Returns

[`Nullable`](../modules.md#nullable)[`Behavior`](../interfaces/Behavior.md)[`Node`](Node.md)

null if behavior was not found else the requested behavior

#### Inherited from

[Camera](Camera.md).[getBehaviorByName](Camera.md#getbehaviorbyname)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:420

___

### getChildMeshes

▸ **getChildMeshes**`T`(`directDescendantsOnly?`, `predicate?`): `T`[]

Get all child-meshes of this node

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`AbstractMesh`](AbstractMesh.md)`T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `directDescendantsOnly?` | `boolean` | defines if true only direct descendants of 'this' will be considered, if false direct and also indirect (children of children, an so on in a recursive manner) descendants of 'this' will be considered (Default: false) |
| `predicate?` | (`node`: [`Node`](Node.md)) => node is T | defines an optional predicate that will be called on every evaluated child, the predicate must return true for a given child to be part of the result, otherwise it will be ignored |

#### Returns

`T`[]

an array of AbstractMesh

#### Inherited from

[Camera](Camera.md).[getChildMeshes](Camera.md#getchildmeshes)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:684

▸ **getChildMeshes**(`directDescendantsOnly?`, `predicate?`): [`AbstractMesh`](AbstractMesh.md)[]

Get all child-meshes of this node

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `directDescendantsOnly?` | `boolean` | defines if true only direct descendants of 'this' will be considered, if false direct and also indirect (children of children, an so on in a recursive manner) descendants of 'this' will be considered (Default: false) |
| `predicate?` | (`node`: [`Node`](Node.md)) => `boolean` | defines an optional predicate that will be called on every evaluated child, the predicate must return true for a given child to be part of the result, otherwise it will be ignored |

#### Returns

[`AbstractMesh`](AbstractMesh.md)[]

an array of AbstractMesh

#### Inherited from

[Camera](Camera.md).[getChildMeshes](Camera.md#getchildmeshes)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:692

___

### getChildren

▸ **getChildren**`T`(`predicate?`, `directDescendantsOnly?`): `T`[]

Get all direct children of this node

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`Node`](Node.md)`T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `predicate?` | (`node`: [`Node`](Node.md)) => node is T | defines an optional predicate that will be called on every evaluated child, the predicate must return true for a given child to be part of the result, otherwise it will be ignored |
| `directDescendantsOnly?` | `boolean` | defines if true only direct descendants of 'this' will be considered, if false direct and also indirect (children of children, an so on in a recursive manner) descendants of 'this' will be considered (Default: true) |

#### Returns

`T`[]

an array of Node

#### Inherited from

[Camera](Camera.md).[getChildren](Camera.md#getchildren)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:714

▸ **getChildren**(`predicate?`, `directDescendantsOnly?`): [`Node`](Node.md)[]

Get all direct children of this node

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `predicate?` | (`node`: [`Node`](Node.md)) => `boolean` | defines an optional predicate that will be called on every evaluated child, the predicate must return true for a given child to be part of the result, otherwise it will be ignored |
| `directDescendantsOnly?` | `boolean` | defines if true only direct descendants of 'this' will be considered, if false direct and also indirect (children of children, an so on in a recursive manner) descendants of 'this' will be considered (Default: true) |

#### Returns

[`Node`](Node.md)[]

an array of Node

#### Inherited from

[Camera](Camera.md).[getChildren](Camera.md#getchildren)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:722

___

### getClassName

▸ **getClassName**(): `string`

Gets the current object class name.

#### Returns

`string`

the class name

#### Overrides

[Camera](Camera.md).[getClassName](Camera.md#getclassname)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/targetCamera.ts:577

___

### getDescendants

▸ **getDescendants**`T`(`directDescendantsOnly?`, `predicate?`): `T`[]

Will return all nodes that have this node as ascendant

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`Node`](Node.md)`T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `directDescendantsOnly?` | `boolean` | defines if true only direct descendants of 'this' will be considered, if false direct and also indirect (children of children, an so on in a recursive manner) descendants of 'this' will be considered |
| `predicate?` | (`node`: [`Node`](Node.md)) => node is T | defines an optional predicate that will be called on every evaluated child, the predicate must return true for a given child to be part of the result, otherwise it will be ignored |

#### Returns

`T`[]

all children nodes of all types

#### Inherited from

[Camera](Camera.md).[getDescendants](Camera.md#getdescendants)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:654

▸ **getDescendants**(`directDescendantsOnly?`, `predicate?`): [`Node`](Node.md)[]

Will return all nodes that have this node as ascendant

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `directDescendantsOnly?` | `boolean` | defines if true only direct descendants of 'this' will be considered, if false direct and also indirect (children of children, an so on in a recursive manner) descendants of 'this' will be considered |
| `predicate?` | (`node`: [`Node`](Node.md)) => `boolean` | defines an optional predicate that will be called on every evaluated child, the predicate must return true for a given child to be part of the result, otherwise it will be ignored |

#### Returns

[`Node`](Node.md)[]

all children nodes of all types

#### Inherited from

[Camera](Camera.md).[getDescendants](Camera.md#getdescendants)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:662

___

### getDirection

▸ **getDirection**(`localAxis`): [`Vector3`](Vector3.md)

Gets the direction of the camera relative to a given local axis.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `localAxis` | [`Vector3`](Vector3.md) | Defines the reference axis to provide a relative direction. |

#### Returns

[`Vector3`](Vector3.md)

the direction

#### Inherited from

[Camera](Camera.md).[getDirection](Camera.md#getdirection)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:1367

___

### getDirectionToRef

▸ **getDirectionToRef**(`localAxis`, `result`): `void`

Gets the direction of the camera relative to a given local axis into a passed vector.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `localAxis` | [`Vector3`](Vector3.md) | Defines the reference axis to provide a relative direction. |
| `result` | [`Vector3`](Vector3.md) | Defines the vector to store the result in |

#### Returns

`void`

#### Inherited from

[Camera](Camera.md).[getDirectionToRef](Camera.md#getdirectiontoref)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:1389

___

### getEngine

▸ **getEngine**(): [`Engine`](Engine.md)

Gets the engine of the node

#### Returns

[`Engine`](Engine.md)

a Engine

#### Inherited from

[Camera](Camera.md).[getEngine](Camera.md#getengine)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:352

___

### getForwardRay

▸ **getForwardRay**(`length?`, `transform?`, `origin?`): [`Ray`](Ray.md)

Gets a ray in the forward direction from the camera.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `length` | `number` | `100` | Defines the length of the ray to create |
| `transform?` | [`Matrix`](Matrix.md) | `undefined` | Defines the transform to apply to the ray, by default the world matrix is used to create a workd space ray |
| `origin?` | [`Vector3`](Vector3.md) | `undefined` | Defines the start point of the ray which defaults to the camera position |

#### Returns

[`Ray`](Ray.md)

the forward ray

#### Inherited from

[Camera](Camera.md).[getForwardRay](Camera.md#getforwardray)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:1028

___

### getForwardRayToRef

▸ **getForwardRayToRef**(`refRay`, `length?`, `transform?`, `origin?`): [`Ray`](Ray.md)

Gets a ray in the forward direction from the camera.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `refRay` | [`Ray`](Ray.md) | `undefined` | the ray to (re)use when setting the values |
| `length` | `number` | `100` | Defines the length of the ray to create |
| `transform?` | [`Matrix`](Matrix.md) | `undefined` | Defines the transform to apply to the ray, by default the world matrx is used to create a workd space ray |
| `origin?` | [`Vector3`](Vector3.md) | `undefined` | Defines the start point of the ray which defaults to the camera position |

#### Returns

[`Ray`](Ray.md)

the forward ray

#### Inherited from

[Camera](Camera.md).[getForwardRayToRef](Camera.md#getforwardraytoref)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:1041

___

### getFrontPosition

▸ **getFrontPosition**(`distance`): [`Vector3`](Vector3.md)

Gets the position in front of the camera at a given distance.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `distance` | `number` | The distance from the camera we want the position to be |

#### Returns

[`Vector3`](Vector3.md)

the position

#### Defined in

https://github.com/babylon.js/core/src/Cameras/targetCamera.ts:121

___

### getHierarchyBoundingVectors

▸ **getHierarchyBoundingVectors**(`includeDescendants?`, `predicate?`): `Object`

Return the minimum and maximum world vectors of the entire hierarchy under current node

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `includeDescendants` | `boolean` | `true` | Include bounding info from descendants as well (true by default) |
| `predicate` | [`Nullable`](../modules.md#nullable)(`abstractMesh`: [`AbstractMesh`](AbstractMesh.md)) => `boolean` | `null` | defines a callback function that can be customize to filter what meshes should be included in the list used to compute the bounding vectors |

#### Returns

`Object`

the new bounding vectors

| Name | Type |
| :------ | :------ |
| `max` | [`Vector3`](Vector3.md) |
| `min` | [`Vector3`](Vector3.md) |

#### Inherited from

[Camera](Camera.md).[getHierarchyBoundingVectors](Camera.md#gethierarchyboundingvectors)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:933

___

### getLeftTarget

▸ **getLeftTarget**(): [`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md)

Gets the left camera target of a rig setup in case of Rigged Camera

#### Returns

[`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md)

the target position

#### Inherited from

[Camera](Camera.md).[getLeftTarget](Camera.md#getlefttarget)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:1157

___

### getProjectionMatrix

▸ **getProjectionMatrix**(`force?`): [`Matrix`](Matrix.md)

Gets the current projection matrix of the camera.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `force?` | `boolean` | forces the camera to recompute the matrix without looking at the cached state |

#### Returns

[`Matrix`](Matrix.md)

the projection matrix

#### Inherited from

[Camera](Camera.md).[getProjectionMatrix](Camera.md#getprojectionmatrix)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:867

___

### getRightTarget

▸ **getRightTarget**(): [`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md)

Gets the right camera target of a rig setup in case of Rigged Camera

#### Returns

[`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md)

the target position

#### Inherited from

[Camera](Camera.md).[getRightTarget](Camera.md#getrighttarget)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:1168

___

### getScene

▸ **getScene**(): [`Scene`](Scene.md)

Gets the scene of the node

#### Returns

[`Scene`](Scene.md)

a scene

#### Inherited from

[Camera](Camera.md).[getScene](Camera.md#getscene)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:344

___

### getTarget

▸ **getTarget**(): [`Vector3`](Vector3.md)

Return the current target position of the camera. This value is expressed in local space.

#### Returns

[`Vector3`](Vector3.md)

the target position

#### Defined in

https://github.com/babylon.js/core/src/Cameras/targetCamera.ts:303

___

### getTransformationMatrix

▸ **getTransformationMatrix**(): [`Matrix`](Matrix.md)

Gets the transformation matrix (ie. the multiplication of view by projection matrices)

#### Returns

[`Matrix`](Matrix.md)

a Matrix

#### Inherited from

[Camera](Camera.md).[getTransformationMatrix](Camera.md#gettransformationmatrix)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:965

___

### getViewMatrix

▸ **getViewMatrix**(`force?`): [`Matrix`](Matrix.md)

Gets the current view matrix of the camera.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `force?` | `boolean` | forces the camera to recompute the matrix without looking at the cached state |

#### Returns

[`Matrix`](Matrix.md)

the view matrix

#### Inherited from

[Camera](Camera.md).[getViewMatrix](Camera.md#getviewmatrix)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:814

___

### getWorldMatrix

▸ **getWorldMatrix**(): [`Matrix`](Matrix.md)

Gets the current world matrix of the camera

#### Returns

[`Matrix`](Matrix.md)

#### Inherited from

[Camera](Camera.md).[getWorldMatrix](Camera.md#getworldmatrix)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:793

___

### isActiveMesh

▸ **isActiveMesh**(`mesh`): `boolean`

Check whether a mesh is part of the current active mesh list of the camera

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`Mesh`](Mesh.md) | Defines the mesh to check |

#### Returns

`boolean`

true if active, false otherwise

#### Inherited from

[Camera](Camera.md).[isActiveMesh](Camera.md#isactivemesh)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:539

___

### isCompletelyInFrustum

▸ **isCompletelyInFrustum**(`target`): `boolean`

Checks if a cullable object (mesh...) is in the camera frustum
Unlike isInFrustum this checks the full bounding box

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `target` | [`ICullable`](../interfaces/ICullable.md) | The object to check |

#### Returns

`boolean`

true if the object is in frustum otherwise false

#### Inherited from

[Camera](Camera.md).[isCompletelyInFrustum](Camera.md#iscompletelyinfrustum)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:1014

___

### isDescendantOf

▸ **isDescendantOf**(`ancestor`): `boolean`

Is this node a descendant of the given node?
The function will iterate up the hierarchy until the ancestor was found or no more parents defined

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ancestor` | [`Node`](Node.md) | defines the parent node to inspect |

#### Returns

`boolean`

a boolean indicating if this node is a descendant of the given node

#### Inherited from

[Camera](Camera.md).[isDescendantOf](Camera.md#isdescendantof)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:613

___

### isDisposed

▸ **isDisposed**(): `boolean`

Gets a boolean indicating if the node has been disposed

#### Returns

`boolean`

true if the node was disposed

#### Inherited from

[Camera](Camera.md).[isDisposed](Camera.md#isdisposed)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:192

___

### isEnabled

▸ **isEnabled**(`checkAncestors?`): `boolean`

Is this node enabled?
If the node has a parent, all ancestors will be checked and false will be returned if any are false (not enabled), otherwise will return true

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `checkAncestors` | `boolean` | `true` | indicates if this method should check the ancestors. The default is to check the ancestors. If set to false, the method will return the value of this node without checking ancestors |

#### Returns

`boolean`

whether this node (and its parent) is enabled

#### Inherited from

[Camera](Camera.md).[isEnabled](Camera.md#isenabled)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:569

___

### isInFrustum

▸ **isInFrustum**(`target`, `checkRigCameras?`): `boolean`

Checks if a cullable object (mesh...) is in the camera frustum
This checks the bounding box center. See isCompletelyInFrustum for a full bounding check

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `target` | [`ICullable`](../interfaces/ICullable.md) | `undefined` | The object to check |
| `checkRigCameras` | `boolean` | `false` | If the rig cameras should be checked (eg. with webVR camera both eyes should be checked) (Default: false) |

#### Returns

`boolean`

true if the object is in frustum otherwise false

#### Inherited from

[Camera](Camera.md).[isInFrustum](Camera.md#isinfrustum)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:993

___

### isReady

▸ **isReady**(`completeCheck?`): `boolean`

Is this camera ready to be used/rendered

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `completeCheck` | `boolean` | `false` | defines if a complete check (including post processes) has to be done (false by default) |

#### Returns

`boolean`

true if the camera is ready

#### Inherited from

[Camera](Camera.md).[isReady](Camera.md#isready)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:548

___

### markAsDirty

▸ **markAsDirty**(`property?`): [`Node`](Node.md)

Flag the  node as dirty (Forcing it to update everything)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `property?` | `string` | helps children apply precise "dirtyfication" |

#### Returns

[`Node`](Node.md)

this node

#### Inherited from

[Camera](Camera.md).[markAsDirty](Camera.md#markasdirty)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:557

___

### removeBehavior

▸ **removeBehavior**(`behavior`): [`Node`](Node.md)

Remove an attached behavior

**`See`**

https://doc.babylonjs.com/features/behaviour

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `behavior` | [`Behavior`](../interfaces/Behavior.md)[`Node`](Node.md) | defines the behavior to attach |

#### Returns

[`Node`](Node.md)

the current Node

#### Inherited from

[Camera](Camera.md).[removeBehavior](Camera.md#removebehavior)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:393

___

### restoreState

▸ **restoreState**(): `boolean`

Restored camera state. You must call storeState() first.

#### Returns

`boolean`

true if restored and false otherwise

#### Inherited from

[Camera](Camera.md).[restoreState](Camera.md#restorestate)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:474

___

### serialize

▸ **serialize**(): `any`

Serialiaze the camera setup to a json representation

#### Returns

`any`

the JSON representation

#### Inherited from

[Camera](Camera.md).[serialize](Camera.md#serialize)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:1319

___

### serializeAnimationRanges

▸ **serializeAnimationRanges**(): `any`

Serialize animation ranges into a JSON compatible object

#### Returns

`any`

serialization object

#### Inherited from

[Camera](Camera.md).[serializeAnimationRanges](Camera.md#serializeanimationranges)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:847

___

### setEnabled

▸ **setEnabled**(`value`): `void`

Set the enabled state of this node

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `boolean` | defines the new enabled state |

#### Returns

`void`

#### Inherited from

[Camera](Camera.md).[setEnabled](Camera.md#setenabled)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:596

___

### setTarget

▸ **setTarget**(`target`): `void`

Defines the target the camera should look at.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `target` | [`Vector3`](Vector3.md) | Defines the new target as a Vector |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Cameras/targetCamera.ts:245

___

### storeState

▸ **storeState**(): [`Camera`](Camera.md)

Store current camera state of the camera (fov, position, rotation, etc..)

#### Returns

[`Camera`](Camera.md)

the camera

#### Overrides

[Camera](Camera.md).[storeState](Camera.md#storestate)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/targetCamera.ts:150

___

### toString

▸ **toString**(`fullDetails?`): `string`

Gets a string representation of the camera useful for debug purpose.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fullDetails?` | `boolean` | Defines that a more verbose level of logging is required |

#### Returns

`string`

the string representation

#### Inherited from

[Camera](Camera.md).[toString](Camera.md#tostring)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:499

___

### unfreezeProjectionMatrix

▸ **unfreezeProjectionMatrix**(): `void`

Unfreeze the projection matrix if it has previously been freezed by freezeProjectionMatrix.

#### Returns

`void`

#### Inherited from

[Camera](Camera.md).[unfreezeProjectionMatrix](Camera.md#unfreezeprojectionmatrix)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:858

___

### update

▸ **update**(): `void`

Update the camera state according to the different inputs gathered during the frame.

#### Returns

`void`

#### Inherited from

[Camera](Camera.md).[update](Camera.md#update)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:677

___

### AddNodeConstructor

▸ `Static` **AddNodeConstructor**(`type`, `constructorFunc`): `void`

Add a new node constructor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | `string` | defines the type name of the node to construct |
| `constructorFunc` | [`NodeConstructor`](../modules.md#nodeconstructor) | defines the constructor function |

#### Returns

`void`

#### Inherited from

[Camera](Camera.md).[AddNodeConstructor](Camera.md#addnodeconstructor)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:63

___

### Construct

▸ `Static` **Construct**(`type`, `name`, `scene`, `options?`): [`Nullable`](../modules.md#nullable)() => [`Node`](Node.md)

Returns a node constructor based on type name

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | `string` | defines the type name |
| `name` | `string` | defines the new node name |
| `scene` | [`Scene`](Scene.md) | defines the hosting scene |
| `options?` | `any` | defines optional options to transmit to constructors |

#### Returns

[`Nullable`](../modules.md#nullable)() => [`Node`](Node.md)

the new constructor or null

#### Inherited from

[Camera](Camera.md).[Construct](Camera.md#construct)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:75

___

### GetConstructorFromName

▸ `Static` **GetConstructorFromName**(`type`, `name`, `scene`, `interaxial_distance?`, `isStereoscopicSideBySide?`): () => [`Camera`](Camera.md)

Gets a camera constructor for a given camera type

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `type` | `string` | `undefined` | The type of the camera to construct (should be equal to one of the camera class name) |
| `name` | `string` | `undefined` | The name of the camera the result will be able to instantiate |
| `scene` | [`Scene`](Scene.md) | `undefined` | The scene the result will construct the camera in |
| `interaxial_distance` | `number` | `0` | In case of stereoscopic setup, the distance between both eyes |
| `isStereoscopicSideBySide` | `boolean` | `true` | In case of stereoscopic setup, should the sereo be side b side |

#### Returns

`fn`

a factory method to construct the camera

▸ (): [`Camera`](Camera.md)

Gets a camera constructor for a given camera type

##### Returns

[`Camera`](Camera.md)

a factory method to construct the camera

#### Inherited from

[Camera](Camera.md).[GetConstructorFromName](Camera.md#getconstructorfromname)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:1403

___

### Parse

▸ `Static` **Parse**(`parsedCamera`, `scene`): [`Camera`](Camera.md)

Parse a JSON and creates the camera from the parsed information

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `parsedCamera` | `any` | The JSON to parse |
| `scene` | [`Scene`](Scene.md) | The scene to instantiate the camera in |

#### Returns

[`Camera`](Camera.md)

the newly constructed camera

#### Inherited from

[Camera](Camera.md).[Parse](Camera.md#parse)

#### Defined in

https://github.com/babylon.js/core/src/Cameras/camera.ts:1432

___

### ParseAnimationRanges

▸ `Static` **ParseAnimationRanges**(`node`, `parsedNode`, `scene`): `void`

Parse animation range data from a serialization object and store them into a given node

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `node` | [`Node`](Node.md) | defines where to store the animation ranges |
| `parsedNode` | `any` | defines the serialization object to read data from |
| `scene` | [`Scene`](Scene.md) | defines the hosting scene |

#### Returns

`void`

#### Inherited from

[Camera](Camera.md).[ParseAnimationRanges](Camera.md#parseanimationranges)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:919
