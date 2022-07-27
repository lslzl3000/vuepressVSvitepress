[@dev/core](../README.md) / [Exports](../modules.md) / Camera

# Class: Camera

This is the base class of all the camera used in the application.

**`See`**

https://doc.babylonjs.com/features/cameras

## Hierarchy

- [`Node`](Node.md)

  ↳ **`Camera`**

  ↳↳ [`TargetCamera`](TargetCamera.md)

## Table of contents

### Constructors

- [constructor](Camera.md#constructor)

### Properties

- [\_absoluteRotation](Camera.md#_absoluterotation)
- [\_doNotComputeProjectionMatrix](Camera.md#_donotcomputeprojectionmatrix)
- [\_frustumPlanes](Camera.md#_frustumplanes)
- [\_globalPosition](Camera.md#_globalposition)
- [\_isDirty](Camera.md#_isdirty)
- [\_mode](Camera.md#_mode)
- [\_orthoBottom](Camera.md#_orthobottom)
- [\_orthoLeft](Camera.md#_ortholeft)
- [\_orthoRight](Camera.md#_orthoright)
- [\_orthoTop](Camera.md#_orthotop)
- [\_parentNode](Camera.md#_parentnode)
- [\_ranges](Camera.md#_ranges)
- [\_refreshFrustumPlanes](Camera.md#_refreshfrustumplanes)
- [\_stateStored](Camera.md#_statestored)
- [\_storedFov](Camera.md#_storedfov)
- [\_transformMatrix](Camera.md#_transformmatrix)
- [\_upVector](Camera.md#_upvector)
- [\_webvrViewMatrix](Camera.md#_webvrviewmatrix)
- [animations](Camera.md#animations)
- [cameraRigMode](Camera.md#camerarigmode)
- [customRenderTargets](Camera.md#customrendertargets)
- [fov](Camera.md#fov)
- [fovMode](Camera.md#fovmode)
- [id](Camera.md#id)
- [inertia](Camera.md#inertia)
- [inputs](Camera.md#inputs)
- [inspectableCustomProperties](Camera.md#inspectablecustomproperties)
- [interaxialDistance](Camera.md#interaxialdistance)
- [isIntermediate](Camera.md#isintermediate)
- [isRigCamera](Camera.md#isrigcamera)
- [isStereoscopicSideBySide](Camera.md#isstereoscopicsidebyside)
- [layerMask](Camera.md#layermask)
- [maxZ](Camera.md#maxz)
- [metadata](Camera.md#metadata)
- [minZ](Camera.md#minz)
- [name](Camera.md#name)
- [onAfterCheckInputsObservable](Camera.md#onaftercheckinputsobservable)
- [onDisposeObservable](Camera.md#ondisposeobservable)
- [onProjectionMatrixChangedObservable](Camera.md#onprojectionmatrixchangedobservable)
- [onReady](Camera.md#onready)
- [onRestoreStateObservable](Camera.md#onrestorestateobservable)
- [onViewMatrixChangedObservable](Camera.md#onviewmatrixchangedobservable)
- [outputRenderTarget](Camera.md#outputrendertarget)
- [projectionPlaneTilt](Camera.md#projectionplanetilt)
- [renderPassId](Camera.md#renderpassid)
- [reservedDataStore](Camera.md#reserveddatastore)
- [rigParent](Camera.md#rigparent)
- [state](Camera.md#state)
- [uniqueId](Camera.md#uniqueid)
- [viewport](Camera.md#viewport)
- [FOVMODE\_HORIZONTAL\_FIXED](Camera.md#fovmode_horizontal_fixed)
- [FOVMODE\_VERTICAL\_FIXED](Camera.md#fovmode_vertical_fixed)
- [ForceAttachControlToAlwaysPreventDefault](Camera.md#forceattachcontroltoalwayspreventdefault)
- [ORTHOGRAPHIC\_CAMERA](Camera.md#orthographic_camera)
- [PERSPECTIVE\_CAMERA](Camera.md#perspective_camera)
- [RIG\_MODE\_CUSTOM](Camera.md#rig_mode_custom)
- [RIG\_MODE\_NONE](Camera.md#rig_mode_none)
- [RIG\_MODE\_STEREOSCOPIC\_ANAGLYPH](Camera.md#rig_mode_stereoscopic_anaglyph)
- [RIG\_MODE\_STEREOSCOPIC\_INTERLACED](Camera.md#rig_mode_stereoscopic_interlaced)
- [RIG\_MODE\_STEREOSCOPIC\_OVERUNDER](Camera.md#rig_mode_stereoscopic_overunder)
- [RIG\_MODE\_STEREOSCOPIC\_SIDEBYSIDE\_CROSSEYED](Camera.md#rig_mode_stereoscopic_sidebyside_crosseyed)
- [RIG\_MODE\_STEREOSCOPIC\_SIDEBYSIDE\_PARALLEL](Camera.md#rig_mode_stereoscopic_sidebyside_parallel)
- [RIG\_MODE\_VR](Camera.md#rig_mode_vr)
- [RIG\_MODE\_WEBVR](Camera.md#rig_mode_webvr)

### Accessors

- [absoluteRotation](Camera.md#absoluterotation)
- [animationPropertiesOverride](Camera.md#animationpropertiesoverride)
- [behaviors](Camera.md#behaviors)
- [doNotSerialize](Camera.md#donotserialize)
- [globalPosition](Camera.md#globalposition)
- [isLeftCamera](Camera.md#isleftcamera)
- [isRightCamera](Camera.md#isrightcamera)
- [leftCamera](Camera.md#leftcamera)
- [mode](Camera.md#mode)
- [onClonedObservable](Camera.md#onclonedobservable)
- [onDispose](Camera.md#ondispose)
- [onEnabledStateChangedObservable](Camera.md#onenabledstatechangedobservable)
- [orthoBottom](Camera.md#orthobottom)
- [orthoLeft](Camera.md#ortholeft)
- [orthoRight](Camera.md#orthoright)
- [orthoTop](Camera.md#orthotop)
- [parent](Camera.md#parent)
- [position](Camera.md#position)
- [rigPostProcess](Camera.md#rigpostprocess)
- [rightCamera](Camera.md#rightcamera)
- [screenArea](Camera.md#screenarea)
- [upVector](Camera.md#upvector)
- [worldMatrixFromCache](Camera.md#worldmatrixfromcache)

### Methods

- [\_cascadePostProcessesToRigCams](Camera.md#_cascadepostprocessestorigcams)
- [\_getFirstPostProcess](Camera.md#_getfirstpostprocess)
- [\_restoreStateValues](Camera.md#_restorestatevalues)
- [\_setRigMode](Camera.md#_setrigmode)
- [\_updateCameraRotationMatrix](Camera.md#_updatecamerarotationmatrix)
- [\_updateFrustumPlanes](Camera.md#_updatefrustumplanes)
- [\_updateWebVRCameraRotationMatrix](Camera.md#_updatewebvrcamerarotationmatrix)
- [addBehavior](Camera.md#addbehavior)
- [applyVerticalCorrection](Camera.md#applyverticalcorrection)
- [attachControl](Camera.md#attachcontrol)
- [attachPostProcess](Camera.md#attachpostprocess)
- [beginAnimation](Camera.md#beginanimation)
- [clone](Camera.md#clone)
- [computeWorldMatrix](Camera.md#computeworldmatrix)
- [createAnimationRange](Camera.md#createanimationrange)
- [deleteAnimationRange](Camera.md#deleteanimationrange)
- [detachControl](Camera.md#detachcontrol)
- [detachPostProcess](Camera.md#detachpostprocess)
- [dispose](Camera.md#dispose)
- [freezeProjectionMatrix](Camera.md#freezeprojectionmatrix)
- [getActiveMeshes](Camera.md#getactivemeshes)
- [getAnimationByName](Camera.md#getanimationbyname)
- [getAnimationRange](Camera.md#getanimationrange)
- [getAnimationRanges](Camera.md#getanimationranges)
- [getBehaviorByName](Camera.md#getbehaviorbyname)
- [getChildMeshes](Camera.md#getchildmeshes)
- [getChildren](Camera.md#getchildren)
- [getClassName](Camera.md#getclassname)
- [getDescendants](Camera.md#getdescendants)
- [getDirection](Camera.md#getdirection)
- [getDirectionToRef](Camera.md#getdirectiontoref)
- [getEngine](Camera.md#getengine)
- [getForwardRay](Camera.md#getforwardray)
- [getForwardRayToRef](Camera.md#getforwardraytoref)
- [getHierarchyBoundingVectors](Camera.md#gethierarchyboundingvectors)
- [getLeftTarget](Camera.md#getlefttarget)
- [getProjectionMatrix](Camera.md#getprojectionmatrix)
- [getRightTarget](Camera.md#getrighttarget)
- [getScene](Camera.md#getscene)
- [getTransformationMatrix](Camera.md#gettransformationmatrix)
- [getViewMatrix](Camera.md#getviewmatrix)
- [getWorldMatrix](Camera.md#getworldmatrix)
- [isActiveMesh](Camera.md#isactivemesh)
- [isCompletelyInFrustum](Camera.md#iscompletelyinfrustum)
- [isDescendantOf](Camera.md#isdescendantof)
- [isDisposed](Camera.md#isdisposed)
- [isEnabled](Camera.md#isenabled)
- [isInFrustum](Camera.md#isinfrustum)
- [isReady](Camera.md#isready)
- [markAsDirty](Camera.md#markasdirty)
- [removeBehavior](Camera.md#removebehavior)
- [restoreState](Camera.md#restorestate)
- [serialize](Camera.md#serialize)
- [serializeAnimationRanges](Camera.md#serializeanimationranges)
- [setEnabled](Camera.md#setenabled)
- [storeState](Camera.md#storestate)
- [toString](Camera.md#tostring)
- [unfreezeProjectionMatrix](Camera.md#unfreezeprojectionmatrix)
- [update](Camera.md#update)
- [AddNodeConstructor](Camera.md#addnodeconstructor)
- [Construct](Camera.md#construct)
- [GetConstructorFromName](Camera.md#getconstructorfromname)
- [Parse](Camera.md#parse)
- [ParseAnimationRanges](Camera.md#parseanimationranges)

## Constructors

### constructor

• **new Camera**(`name`, `position`, `scene?`, `setActiveOnSceneIfNoneActive?`)

Instantiates a new camera object.
This should not be used directly but through the inherited cameras: ArcRotate, Free...

**`See`**

https://doc.babylonjs.com/features/cameras

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | Defines the name of the camera in the scene |
| `position` | [`Vector3`](Vector3.md) | `undefined` | Defines the position of the camera |
| `scene?` | [`Scene`](Scene.md) | `undefined` | Defines the scene the camera belongs too |
| `setActiveOnSceneIfNoneActive` | `boolean` | `true` | Defines if the camera should be set as active after creation if no other camera have been defined in the scene |

#### Overrides

[Node](Node.md).[constructor](Node.md#constructor)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:433

## Properties

### \_absoluteRotation

• `Private` **\_absoluteRotation**: [`Quaternion`](Quaternion.md)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:422

___

### \_doNotComputeProjectionMatrix

• `Private` **\_doNotComputeProjectionMatrix**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Cameras/camera.ts:416

___

### \_frustumPlanes

• `Private` **\_frustumPlanes**: [`Plane`](Plane.md)[]

#### Defined in

packages/dev/core/src/Cameras/camera.ts:418

___

### \_globalPosition

• `Protected` **\_globalPosition**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:412

___

### \_isDirty

• `Protected` **\_isDirty**: `boolean` = `false`

#### Inherited from

[Node](Node.md).[_isDirty](Node.md#_isdirty)

#### Defined in

packages/dev/core/src/node.ts:43

___

### \_mode

• `Private` **\_mode**: `number` = `Camera.PERSPECTIVE_CAMERA`

Define the mode of the camera (Camera.PERSPECTIVE_CAMERA or Camera.ORTHOGRAPHIC_CAMERA)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:284

___

### \_orthoBottom

• `Private` **\_orthoBottom**: [`Nullable`](../modules.md#nullable)`number` = `null`

Define the current limit on the bottom side for an orthographic camera
In scene unit

#### Defined in

packages/dev/core/src/Cameras/camera.ts:210

___

### \_orthoLeft

• `Private` **\_orthoLeft**: [`Nullable`](../modules.md#nullable)`number` = `null`

Define the current limit on the left side for an orthographic camera
In scene unit

#### Defined in

packages/dev/core/src/Cameras/camera.ts:172

___

### \_orthoRight

• `Private` **\_orthoRight**: [`Nullable`](../modules.md#nullable)`number` = `null`

Define the current limit on the right side for an orthographic camera
In scene unit

#### Defined in

packages/dev/core/src/Cameras/camera.ts:191

___

### \_orthoTop

• `Private` **\_orthoTop**: [`Nullable`](../modules.md#nullable)`number` = `null`

Define the current limit on the top side for an orthographic camera
In scene unit

#### Defined in

packages/dev/core/src/Cameras/camera.ts:229

___

### \_parentNode

• `Protected` **\_parentNode**: [`Nullable`](../modules.md#nullable)[`Node`](Node.md) = `null`

#### Inherited from

[Node](Node.md).[_parentNode](Node.md#_parentnode)

#### Defined in

packages/dev/core/src/node.ts:176

___

### \_ranges

• `Protected` **\_ranges**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: [`Nullable`](../modules.md#nullable)`AnimationRange`

#### Inherited from

[Node](Node.md).[_ranges](Node.md#_ranges)

#### Defined in

packages/dev/core/src/node.ts:154

___

### \_refreshFrustumPlanes

• `Private` **\_refreshFrustumPlanes**: `boolean` = `true`

#### Defined in

packages/dev/core/src/Cameras/camera.ts:419

___

### \_stateStored

• `Private` **\_stateStored**: `boolean`

#### Defined in

packages/dev/core/src/Cameras/camera.ts:421

___

### \_storedFov

• `Private` **\_storedFov**: `number`

#### Defined in

packages/dev/core/src/Cameras/camera.ts:420

___

### \_transformMatrix

• `Private` **\_transformMatrix**: [`Matrix`](Matrix.md)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:417

___

### \_upVector

• `Protected` **\_upVector**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:129

___

### \_webvrViewMatrix

• `Protected` **\_webvrViewMatrix**: [`Matrix`](Matrix.md)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:399

___

### animations

• **animations**: [`Animation`](Animation.md)[]

Gets a list of Animations associated with the node

#### Inherited from

[Node](Node.md).[animations](Node.md#animations)

#### Defined in

packages/dev/core/src/node.ts:153

___

### cameraRigMode

• **cameraRigMode**: `number` = `Camera.RIG_MODE_NONE`

Rig mode of the camera.
This is useful to create the camera with two "eyes" instead of one to create VR or stereoscopic scenes.
This is normally controlled byt the camera themselves as internal use.

#### Defined in

packages/dev/core/src/Cameras/camera.ts:330

___

### customRenderTargets

• **customRenderTargets**: [`RenderTargetTexture`](RenderTargetTexture.md)[]

Defines the list of custom render target which are rendered to and then used as the input to this camera's render. Eg. display another camera view on a TV in the main scene
This is pretty helpful if you wish to make a camera render to a texture you could reuse somewhere
else in the scene. (Eg. security camera)

To change the final output target of the camera, camera.outputRenderTarget should be used instead (eg. webXR renders to a render target corresponding to an HMD)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:351

___

### fov

• **fov**: `number` = `0.8`

Field Of View is set in Radians. (default is 0.8)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:248

___

### fovMode

• **fovMode**: `number` = `Camera.FOVMODE_VERTICAL_FIXED`

fovMode sets the camera frustum bounds to the viewport bounds. (default is FOVMODE_VERTICAL_FIXED)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:322

___

### id

• **id**: `string`

Gets or sets the id of the node

#### Inherited from

[Node](Node.md).[id](Node.md#id)

#### Defined in

packages/dev/core/src/node.ts:97

___

### inertia

• **inertia**: `number` = `0.9`

Define the default inertia of the camera.
This helps giving a smooth feeling to the camera movement.

#### Defined in

packages/dev/core/src/Cameras/camera.ts:279

___

### inputs

• **inputs**: [`CameraInputsManager`](CameraInputsManager.md)[`Camera`](Camera.md)

Define the input manager associated with the camera.

#### Defined in

packages/dev/core/src/Cameras/camera.ts:111

___

### inspectableCustomProperties

• **inspectableCustomProperties**: [`IInspectable`](../interfaces/IInspectable.md)[]

List of inspectable custom properties (used by the Inspector)

**`See`**

https://doc.babylonjs.com/how_to/debug_layer#extensibility

#### Inherited from

[Node](Node.md).[inspectableCustomProperties](Node.md#inspectablecustomproperties)

#### Defined in

packages/dev/core/src/node.ts:126

___

### interaxialDistance

• **interaxialDistance**: `number`

Defines the distance between both "eyes" in case of a RIG

#### Defined in

packages/dev/core/src/Cameras/camera.ts:336

___

### isIntermediate

• **isIntermediate**: `boolean` = `false`

Define whether the camera is intermediate.
This is useful to not present the output directly to the screen in case of rig without post process for instance

#### Defined in

packages/dev/core/src/Cameras/camera.ts:303

___

### isRigCamera

• **isRigCamera**: `boolean` = `false`

Is this camera a part of a rig system?

#### Defined in

packages/dev/core/src/Cameras/camera.ts:379

___

### isStereoscopicSideBySide

• **isStereoscopicSideBySide**: `boolean`

Defines if stereoscopic rendering is done side by side or over under.

#### Defined in

packages/dev/core/src/Cameras/camera.ts:342

___

### layerMask

• **layerMask**: `number` = `0x0fffffff`

Restricts the camera to viewing objects with the same layerMask.
A camera with a layerMask of 1 will render mesh.layerMask & camera.layerMask!== 0

#### Defined in

packages/dev/core/src/Cameras/camera.ts:316

___

### maxZ

• **maxZ**: `number` = `10000.0`

Define the maximum distance the camera can see to.
This is important to note that the depth buffer are not infinite and the further it end
the more your scene might encounter depth fighting issue.

#### Defined in

packages/dev/core/src/Cameras/camera.ts:272

___

### metadata

• **metadata**: `any` = `null`

Gets or sets an object used to store user defined information for the node

#### Inherited from

[Node](Node.md).[metadata](Node.md#metadata)

#### Defined in

packages/dev/core/src/node.ts:115

___

### minZ

• **minZ**: `number` = `1`

Define the minimum distance the camera can see from.
This is important to note that the depth buffer are not infinite and the closer it starts
the more your scene might encounter depth fighting issue.

#### Defined in

packages/dev/core/src/Cameras/camera.ts:264

___

### name

• **name**: `string`

Gets or sets the name of the node

#### Inherited from

[Node](Node.md).[name](Node.md#name)

#### Defined in

packages/dev/core/src/node.ts:91

___

### onAfterCheckInputsObservable

• **onAfterCheckInputsObservable**: [`Observable`](Observable.md)[`Camera`](Camera.md)

Observable triggered when the inputs have been processed.

#### Defined in

packages/dev/core/src/Cameras/camera.ts:370

___

### onDisposeObservable

• **onDisposeObservable**: [`Observable`](Observable.md)[`Node`](Node.md)

An event triggered when the mesh is disposed

#### Inherited from

[Node](Node.md).[onDisposeObservable](Node.md#ondisposeobservable)

#### Defined in

packages/dev/core/src/node.ts:300

___

### onProjectionMatrixChangedObservable

• **onProjectionMatrixChangedObservable**: [`Observable`](Observable.md)[`Camera`](Camera.md)

Observable triggered when the camera Projection matrix has changed.

#### Defined in

packages/dev/core/src/Cameras/camera.ts:366

___

### onReady

• **onReady**: [`Nullable`](../modules.md#nullable)(`node`: [`Node`](Node.md)) => `void` = `null`

Callback raised when the node is ready to be used

#### Inherited from

[Node](Node.md).[onReady](Node.md#onready)

#### Defined in

packages/dev/core/src/node.ts:159

___

### onRestoreStateObservable

• **onRestoreStateObservable**: [`Observable`](Observable.md)[`Camera`](Camera.md)

Observable triggered when reset has been called and applied to the camera.

#### Defined in

packages/dev/core/src/Cameras/camera.ts:374

___

### onViewMatrixChangedObservable

• **onViewMatrixChangedObservable**: [`Observable`](Observable.md)[`Camera`](Camera.md)

Observable triggered when the camera view matrix has changed.

#### Defined in

packages/dev/core/src/Cameras/camera.ts:362

___

### outputRenderTarget

• **outputRenderTarget**: [`Nullable`](../modules.md#nullable)[`RenderTargetTexture`](RenderTargetTexture.md) = `null`

When set, the camera will render to this render target instead of the default canvas

If the desire is to use the output of a camera as a texture in the scene consider using camera.customRenderTargets instead

#### Defined in

packages/dev/core/src/Cameras/camera.ts:357

___

### projectionPlaneTilt

• **projectionPlaneTilt**: `number` = `0`

Projection plane tilt around the X axis (horizontal), set in Radians. (default is 0)
Can be used to make vertical lines in world space actually vertical on the screen.
See https://forum.babylonjs.com/t/add-vertical-shift-to-3ds-max-exporter-babylon-cameras/17480

#### Defined in

packages/dev/core/src/Cameras/camera.ts:256

___

### renderPassId

• **renderPassId**: `number`

Render pass id used by the camera to render into the main framebuffer

#### Defined in

packages/dev/core/src/Cameras/camera.ts:390

___

### reservedDataStore

• **reservedDataStore**: `any` = `null`

For internal use only. Please do not use.

#### Inherited from

[Node](Node.md).[reservedDataStore](Node.md#reserveddatastore)

#### Defined in

packages/dev/core/src/node.ts:120

___

### rigParent

• `Optional` **rigParent**: [`Camera`](Camera.md)

If isRigCamera set to true this will be set with the parent camera.
The parent camera is not (!) necessarily the .parent of this camera (like in the case of XR)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:385

___

### state

• **state**: `string` = `""`

Gets or sets a string used to store user defined state for the node

#### Inherited from

[Node](Node.md).[state](Node.md#state)

#### Defined in

packages/dev/core/src/node.ts:109

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the node

#### Inherited from

[Node](Node.md).[uniqueId](Node.md#uniqueid)

#### Defined in

packages/dev/core/src/node.ts:103

___

### viewport

• **viewport**: [`Viewport`](Viewport.md)

Define the viewport of the camera.
This correspond to the portion of the screen the camera will render to in normalized 0 to 1 unit.

#### Defined in

packages/dev/core/src/Cameras/camera.ts:309

___

### FOVMODE\_HORIZONTAL\_FIXED

▪ `Static` `Readonly` **FOVMODE\_HORIZONTAL\_FIXED**: ``1``

This setting aligns the left and right bounds of the viewport to the left and right bounds of the camera frustum.

#### Defined in

packages/dev/core/src/Cameras/camera.ts:62

___

### FOVMODE\_VERTICAL\_FIXED

▪ `Static` `Readonly` **FOVMODE\_VERTICAL\_FIXED**: ``0``

This is the default FOV mode for perspective cameras.
This setting aligns the upper and lower bounds of the viewport to the upper and lower bounds of the camera frustum.

#### Defined in

packages/dev/core/src/Cameras/camera.ts:58

___

### ForceAttachControlToAlwaysPreventDefault

▪ `Static` **ForceAttachControlToAlwaysPreventDefault**: `boolean` = `false`

Defines if by default attaching controls should prevent the default javascript event to continue.

#### Defined in

packages/dev/core/src/Cameras/camera.ts:106

___

### ORTHOGRAPHIC\_CAMERA

▪ `Static` `Readonly` **ORTHOGRAPHIC\_CAMERA**: ``1``

This helps creating camera with an orthographic mode.
Orthographic is commonly used in engineering as a means to produce object specifications that communicate dimensions unambiguously, each line of 1 unit length (cm, meter..whatever) will appear to have the same length everywhere on the drawing. This allows the drafter to dimension only a subset of lines and let the reader know that other lines of that length on the drawing are also that length in reality. Every parallel line in the drawing is also parallel in the object.

#### Defined in

packages/dev/core/src/Cameras/camera.ts:52

___

### PERSPECTIVE\_CAMERA

▪ `Static` `Readonly` **PERSPECTIVE\_CAMERA**: ``0``

This is the default projection mode used by the cameras.
It helps recreating a feeling of perspective and better appreciate depth.
This is the best way to simulate real life cameras.

#### Defined in

packages/dev/core/src/Cameras/camera.ts:47

___

### RIG\_MODE\_CUSTOM

▪ `Static` `Readonly` **RIG\_MODE\_CUSTOM**: ``22``

Custom rig mode allowing rig cameras to be populated manually with any number of cameras

#### Defined in

packages/dev/core/src/Cameras/camera.ts:101

___

### RIG\_MODE\_NONE

▪ `Static` `Readonly` **RIG\_MODE\_NONE**: ``0``

This specifies there is no need for a camera rig.
Basically only one eye is rendered corresponding to the camera.

#### Defined in

packages/dev/core/src/Cameras/camera.ts:68

___

### RIG\_MODE\_STEREOSCOPIC\_ANAGLYPH

▪ `Static` `Readonly` **RIG\_MODE\_STEREOSCOPIC\_ANAGLYPH**: ``10``

Simulates a camera Rig with one blue eye and one red eye.
This can be use with 3d blue and red glasses.

#### Defined in

packages/dev/core/src/Cameras/camera.ts:73

___

### RIG\_MODE\_STEREOSCOPIC\_INTERLACED

▪ `Static` `Readonly` **RIG\_MODE\_STEREOSCOPIC\_INTERLACED**: ``14``

Defines that both eyes of the camera will be rendered on successive lines interlaced for passive 3d monitors.

#### Defined in

packages/dev/core/src/Cameras/camera.ts:89

___

### RIG\_MODE\_STEREOSCOPIC\_OVERUNDER

▪ `Static` `Readonly` **RIG\_MODE\_STEREOSCOPIC\_OVERUNDER**: ``13``

Defines that both eyes of the camera will be rendered over under each other.

#### Defined in

packages/dev/core/src/Cameras/camera.ts:85

___

### RIG\_MODE\_STEREOSCOPIC\_SIDEBYSIDE\_CROSSEYED

▪ `Static` `Readonly` **RIG\_MODE\_STEREOSCOPIC\_SIDEBYSIDE\_CROSSEYED**: ``12``

Defines that both eyes of the camera will be rendered side by side with a none parallel target.

#### Defined in

packages/dev/core/src/Cameras/camera.ts:81

___

### RIG\_MODE\_STEREOSCOPIC\_SIDEBYSIDE\_PARALLEL

▪ `Static` `Readonly` **RIG\_MODE\_STEREOSCOPIC\_SIDEBYSIDE\_PARALLEL**: ``11``

Defines that both eyes of the camera will be rendered side by side with a parallel target.

#### Defined in

packages/dev/core/src/Cameras/camera.ts:77

___

### RIG\_MODE\_VR

▪ `Static` `Readonly` **RIG\_MODE\_VR**: ``20``

Defines that both eyes of the camera should be renderered in a VR mode (carbox).

#### Defined in

packages/dev/core/src/Cameras/camera.ts:93

___

### RIG\_MODE\_WEBVR

▪ `Static` `Readonly` **RIG\_MODE\_WEBVR**: ``21``

Defines that both eyes of the camera should be renderered in a VR mode (webVR).

#### Defined in

packages/dev/core/src/Cameras/camera.ts:97

## Accessors

### absoluteRotation

• `get` **absoluteRotation**(): [`Quaternion`](Quaternion.md)

Returns the current camera absolute rotation

#### Returns

[`Quaternion`](Quaternion.md)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:1378

___

### animationPropertiesOverride

• `get` **animationPropertiesOverride**(): [`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md)

Gets or sets the animation properties override

#### Returns

[`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md)

#### Inherited from

Node.animationPropertiesOverride

#### Defined in

packages/dev/core/src/node.ts:275

• `set` **animationPropertiesOverride**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md) |

#### Returns

`void`

#### Inherited from

Node.animationPropertiesOverride

#### Defined in

packages/dev/core/src/node.ts:282

___

### behaviors

• `get` **behaviors**(): [`Behavior`](../interfaces/Behavior.md)[`Node`](Node.md)[]

Gets the list of attached behaviors

**`See`**

https://doc.babylonjs.com/features/behaviour

#### Returns

[`Behavior`](../interfaces/Behavior.md)[`Node`](Node.md)[]

#### Inherited from

Node.behaviors

#### Defined in

packages/dev/core/src/node.ts:410

___

### doNotSerialize

• `get` **doNotSerialize**(): `boolean`

Gets or sets a boolean used to define if the node must be serialized

#### Returns

`boolean`

#### Inherited from

Node.doNotSerialize

#### Defined in

packages/dev/core/src/node.ts:131

• `set` **doNotSerialize**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

Node.doNotSerialize

#### Defined in

packages/dev/core/src/node.ts:143

___

### globalPosition

• `get` **globalPosition**(): [`Vector3`](Vector3.md)

Gets the current world space position of the camera.

#### Returns

[`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:522

___

### isLeftCamera

• `get` **isLeftCamera**(): `boolean`

Gets the left camera of a rig setup in case of Rigged Camera

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Cameras/camera.ts:1120

___

### isRightCamera

• `get` **isRightCamera**(): `boolean`

Gets the right camera of a rig setup in case of Rigged Camera

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Cameras/camera.ts:1129

___

### leftCamera

• `get` **leftCamera**(): [`Nullable`](../modules.md#nullable)[`FreeCamera`](FreeCamera.md)

Gets the left camera of a rig setup in case of Rigged Camera

#### Returns

[`Nullable`](../modules.md#nullable)[`FreeCamera`](FreeCamera.md)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:1136

___

### mode

• `get` **mode**(): `number`

#### Returns

`number`

#### Defined in

packages/dev/core/src/Cameras/camera.ts:294

• `set` **mode**(`mode`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `mode` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/camera.ts:285

___

### onClonedObservable

• `get` **onClonedObservable**(): [`Observable`](Observable.md)[`Node`](Node.md)

An event triggered when the node is cloned

#### Returns

[`Observable`](Observable.md)[`Node`](Node.md)

#### Inherited from

Node.onClonedObservable

#### Defined in

packages/dev/core/src/node.ts:323

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

Node.onDispose

#### Defined in

packages/dev/core/src/node.ts:306

___

### onEnabledStateChangedObservable

• `get` **onEnabledStateChangedObservable**(): [`Observable`](Observable.md)`boolean`

An event triggered when the enabled state of the node changes

#### Returns

[`Observable`](Observable.md)`boolean`

#### Inherited from

Node.onEnabledStateChangedObservable

#### Defined in

packages/dev/core/src/node.ts:316

___

### orthoBottom

• `get` **orthoBottom**(): [`Nullable`](../modules.md#nullable)`number`

#### Returns

[`Nullable`](../modules.md#nullable)`number`

#### Defined in

packages/dev/core/src/Cameras/camera.ts:220

• `set` **orthoBottom**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)`number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/camera.ts:212

___

### orthoLeft

• `get` **orthoLeft**(): [`Nullable`](../modules.md#nullable)`number`

#### Returns

[`Nullable`](../modules.md#nullable)`number`

#### Defined in

packages/dev/core/src/Cameras/camera.ts:182

• `set` **orthoLeft**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)`number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/camera.ts:174

___

### orthoRight

• `get` **orthoRight**(): [`Nullable`](../modules.md#nullable)`number`

#### Returns

[`Nullable`](../modules.md#nullable)`number`

#### Defined in

packages/dev/core/src/Cameras/camera.ts:201

• `set` **orthoRight**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)`number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/camera.ts:193

___

### orthoTop

• `get` **orthoTop**(): [`Nullable`](../modules.md#nullable)`number`

#### Returns

[`Nullable`](../modules.md#nullable)`number`

#### Defined in

packages/dev/core/src/Cameras/camera.ts:239

• `set` **orthoTop**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)`number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/camera.ts:231

___

### parent

• `get` **parent**(): [`Nullable`](../modules.md#nullable)[`Node`](Node.md)

#### Returns

[`Nullable`](../modules.md#nullable)[`Node`](Node.md)

#### Inherited from

Node.parent

#### Defined in

packages/dev/core/src/node.ts:238

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

Node.parent

#### Defined in

packages/dev/core/src/node.ts:200

___

### position

• `get` **position**(): [`Vector3`](Vector3.md)

Define the current local position of the camera in the scene

#### Returns

[`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:120

• `set` **position**(`newPosition`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `newPosition` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/camera.ts:124

___

### rigPostProcess

• `get` **rigPostProcess**(): [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)

Gets the post process used by the rig cameras

#### Returns

[`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:697

___

### rightCamera

• `get` **rightCamera**(): [`Nullable`](../modules.md#nullable)[`FreeCamera`](FreeCamera.md)

Gets the right camera of a rig setup in case of Rigged Camera

#### Returns

[`Nullable`](../modules.md#nullable)[`FreeCamera`](FreeCamera.md)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:1146

___

### screenArea

• `get` **screenArea**(): `number`

The screen area in scene units squared

#### Returns

`number`

#### Defined in

packages/dev/core/src/Cameras/camera.ts:146

___

### upVector

• `get` **upVector**(): [`Vector3`](Vector3.md)

#### Returns

[`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:139

• `set` **upVector**(`vec`): `void`

The vector the camera should consider as up.
(default is Vector3(0, 1, 0) aka Vector3.Up())

#### Parameters

| Name | Type |
| :------ | :------ |
| `vec` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/camera.ts:135

___

### worldMatrixFromCache

• `get` **worldMatrixFromCache**(): [`Matrix`](Matrix.md)

Returns directly the latest state of the mesh World matrix.
A Matrix is returned.

#### Returns

[`Matrix`](Matrix.md)

#### Inherited from

Node.worldMatrixFromCache

#### Defined in

packages/dev/core/src/node.ts:454

## Methods

### \_cascadePostProcessesToRigCams

▸ `Private` **_cascadePostProcessesToRigCams**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/camera.ts:714

___

### \_getFirstPostProcess

▸ **_getFirstPostProcess**(): [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)

Internal, gets the first post process.

#### Returns

[`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)

the first post process to be run on this camera.

#### Defined in

packages/dev/core/src/Cameras/camera.ts:705

___

### \_restoreStateValues

▸ `Protected` **_restoreStateValues**(): `boolean`

Restores the camera state values if it has been stored. You must call storeState() first

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Cameras/camera.ts:460

___

### \_setRigMode

▸ `Protected` **_setRigMode**(`rigParams`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `rigParams` | `any` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/camera.ts:1222

___

### \_updateCameraRotationMatrix

▸ `Protected` **_updateCameraRotationMatrix**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/camera.ts:1241

___

### \_updateFrustumPlanes

▸ `Private` **_updateFrustumPlanes**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/camera.ts:970

___

### \_updateWebVRCameraRotationMatrix

▸ `Protected` **_updateWebVRCameraRotationMatrix**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/camera.ts:1245

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

[Node](Node.md).[addBehavior](Node.md#addbehavior)

#### Defined in

packages/dev/core/src/node.ts:366

___

### applyVerticalCorrection

▸ **applyVerticalCorrection**(): `void`

Automatically tilts the projection plane, using `projectionPlaneTilt`, to correct the perspective effect on vertical lines.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/camera.ts:513

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

#### Defined in

packages/dev/core/src/Cameras/camera.ts:642

▸ **attachControl**(`ignored`, `noPreventDefault?`): `void`

Attach the input controls to a specific dom element to get the input from.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ignored` | `any` | defines an ignored parameter kept for backward compatibility. |
| `noPreventDefault?` | `boolean` | Defines whether event caught by the controls should call preventdefault() (https://developer.mozilla.org/en-US/docs/Web/API/Event/preventDefault)  BACK COMPAT SIGNATURE ONLY. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/camera.ts:649

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

#### Defined in

packages/dev/core/src/Cameras/camera.ts:748

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

[Node](Node.md).[beginAnimation](Node.md#beginanimation)

#### Defined in

packages/dev/core/src/node.ts:833

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

#### Defined in

packages/dev/core/src/Cameras/camera.ts:1349

___

### computeWorldMatrix

▸ **computeWorldMatrix**(): [`Matrix`](Matrix.md)

Compute the world  matrix of the camera.

#### Returns

[`Matrix`](Matrix.md)

the camera world matrix

#### Overrides

[Node](Node.md).[computeWorldMatrix](Node.md#computeworldmatrix)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:1422

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

[Node](Node.md).[createAnimationRange](Node.md#createanimationrange)

#### Defined in

packages/dev/core/src/node.ts:777

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

[Node](Node.md).[deleteAnimationRange](Node.md#deleteanimationrange)

#### Defined in

packages/dev/core/src/node.ts:794

___

### detachControl

▸ **detachControl**(): `void`

Detach the current controls from the specified dom element.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/camera.ts:661

▸ **detachControl**(`ignored?`): `void`

Detach the current controls from the specified dom element.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ignored?` | `any` | defines an ignored parameter kept for backward compatibility. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/camera.ts:666

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

#### Defined in

packages/dev/core/src/Cameras/camera.ts:776

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

#### Overrides

[Node](Node.md).[dispose](Node.md#dispose)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:1050

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

#### Defined in

packages/dev/core/src/Cameras/camera.ts:848

___

### getActiveMeshes

▸ **getActiveMeshes**(): [`SmartArray`](SmartArray.md)[`AbstractMesh`](AbstractMesh.md)

Gets the list of active meshes this frame (meshes no culled or excluded by lod s in the frame)

#### Returns

[`SmartArray`](SmartArray.md)[`AbstractMesh`](AbstractMesh.md)

the active meshe list

#### Defined in

packages/dev/core/src/Cameras/camera.ts:530

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

[Node](Node.md).[getAnimationByName](Node.md#getanimationbyname)

#### Defined in

packages/dev/core/src/node.ts:759

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

[Node](Node.md).[getAnimationRange](Node.md#getanimationrange)

#### Defined in

packages/dev/core/src/node.ts:808

___

### getAnimationRanges

▸ **getAnimationRanges**(): [`Nullable`](../modules.md#nullable)[`AnimationRange`](AnimationRange.md)[]

Gets the list of all animation ranges defined on this node

#### Returns

[`Nullable`](../modules.md#nullable)[`AnimationRange`](AnimationRange.md)[]

an array

#### Inherited from

[Node](Node.md).[getAnimationRanges](Node.md#getanimationranges)

#### Defined in

packages/dev/core/src/node.ts:816

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

[Node](Node.md).[getBehaviorByName](Node.md#getbehaviorbyname)

#### Defined in

packages/dev/core/src/node.ts:420

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

[Node](Node.md).[getChildMeshes](Node.md#getchildmeshes)

#### Defined in

packages/dev/core/src/node.ts:684

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

[Node](Node.md).[getChildMeshes](Node.md#getchildmeshes)

#### Defined in

packages/dev/core/src/node.ts:692

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

[Node](Node.md).[getChildren](Node.md#getchildren)

#### Defined in

packages/dev/core/src/node.ts:714

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

[Node](Node.md).[getChildren](Node.md#getchildren)

#### Defined in

packages/dev/core/src/node.ts:722

___

### getClassName

▸ **getClassName**(): `string`

Gets the class name of the camera.

#### Returns

`string`

the class name

#### Overrides

[Node](Node.md).[getClassName](Node.md#getclassname)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:487

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

[Node](Node.md).[getDescendants](Node.md#getdescendants)

#### Defined in

packages/dev/core/src/node.ts:654

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

[Node](Node.md).[getDescendants](Node.md#getdescendants)

#### Defined in

packages/dev/core/src/node.ts:662

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

#### Defined in

packages/dev/core/src/Cameras/camera.ts:1367

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

#### Defined in

packages/dev/core/src/Cameras/camera.ts:1389

___

### getEngine

▸ **getEngine**(): [`Engine`](Engine.md)

Gets the engine of the node

#### Returns

[`Engine`](Engine.md)

a Engine

#### Inherited from

[Node](Node.md).[getEngine](Node.md#getengine)

#### Defined in

packages/dev/core/src/node.ts:352

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

#### Defined in

packages/dev/core/src/Cameras/camera.ts:1028

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

#### Defined in

packages/dev/core/src/Cameras/camera.ts:1041

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

[Node](Node.md).[getHierarchyBoundingVectors](Node.md#gethierarchyboundingvectors)

#### Defined in

packages/dev/core/src/node.ts:933

___

### getLeftTarget

▸ **getLeftTarget**(): [`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md)

Gets the left camera target of a rig setup in case of Rigged Camera

#### Returns

[`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md)

the target position

#### Defined in

packages/dev/core/src/Cameras/camera.ts:1157

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

#### Defined in

packages/dev/core/src/Cameras/camera.ts:867

___

### getRightTarget

▸ **getRightTarget**(): [`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md)

Gets the right camera target of a rig setup in case of Rigged Camera

#### Returns

[`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md)

the target position

#### Defined in

packages/dev/core/src/Cameras/camera.ts:1168

___

### getScene

▸ **getScene**(): [`Scene`](Scene.md)

Gets the scene of the node

#### Returns

[`Scene`](Scene.md)

a scene

#### Inherited from

[Node](Node.md).[getScene](Node.md#getscene)

#### Defined in

packages/dev/core/src/node.ts:344

___

### getTransformationMatrix

▸ **getTransformationMatrix**(): [`Matrix`](Matrix.md)

Gets the transformation matrix (ie. the multiplication of view by projection matrices)

#### Returns

[`Matrix`](Matrix.md)

a Matrix

#### Defined in

packages/dev/core/src/Cameras/camera.ts:965

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

#### Defined in

packages/dev/core/src/Cameras/camera.ts:814

___

### getWorldMatrix

▸ **getWorldMatrix**(): [`Matrix`](Matrix.md)

Gets the current world matrix of the camera

#### Returns

[`Matrix`](Matrix.md)

#### Overrides

[Node](Node.md).[getWorldMatrix](Node.md#getworldmatrix)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:793

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

#### Defined in

packages/dev/core/src/Cameras/camera.ts:539

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

#### Defined in

packages/dev/core/src/Cameras/camera.ts:1014

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

[Node](Node.md).[isDescendantOf](Node.md#isdescendantof)

#### Defined in

packages/dev/core/src/node.ts:613

___

### isDisposed

▸ **isDisposed**(): `boolean`

Gets a boolean indicating if the node has been disposed

#### Returns

`boolean`

true if the node was disposed

#### Inherited from

[Node](Node.md).[isDisposed](Node.md#isdisposed)

#### Defined in

packages/dev/core/src/node.ts:192

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

[Node](Node.md).[isEnabled](Node.md#isenabled)

#### Defined in

packages/dev/core/src/node.ts:569

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

#### Defined in

packages/dev/core/src/Cameras/camera.ts:993

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

#### Overrides

[Node](Node.md).[isReady](Node.md#isready)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:548

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

[Node](Node.md).[markAsDirty](Node.md#markasdirty)

#### Defined in

packages/dev/core/src/node.ts:557

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

[Node](Node.md).[removeBehavior](Node.md#removebehavior)

#### Defined in

packages/dev/core/src/node.ts:393

___

### restoreState

▸ **restoreState**(): `boolean`

Restored camera state. You must call storeState() first.

#### Returns

`boolean`

true if restored and false otherwise

#### Defined in

packages/dev/core/src/Cameras/camera.ts:474

___

### serialize

▸ **serialize**(): `any`

Serialiaze the camera setup to a json representation

#### Returns

`any`

the JSON representation

#### Defined in

packages/dev/core/src/Cameras/camera.ts:1319

___

### serializeAnimationRanges

▸ **serializeAnimationRanges**(): `any`

Serialize animation ranges into a JSON compatible object

#### Returns

`any`

serialization object

#### Inherited from

[Node](Node.md).[serializeAnimationRanges](Node.md#serializeanimationranges)

#### Defined in

packages/dev/core/src/node.ts:847

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

[Node](Node.md).[setEnabled](Node.md#setenabled)

#### Defined in

packages/dev/core/src/node.ts:596

___

### storeState

▸ **storeState**(): [`Camera`](Camera.md)

Store current camera state (fov, position, etc..)

#### Returns

[`Camera`](Camera.md)

the camera

#### Defined in

packages/dev/core/src/Cameras/camera.ts:450

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

#### Defined in

packages/dev/core/src/Cameras/camera.ts:499

___

### unfreezeProjectionMatrix

▸ **unfreezeProjectionMatrix**(): `void`

Unfreeze the projection matrix if it has previously been freezed by freezeProjectionMatrix.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/camera.ts:858

___

### update

▸ **update**(): `void`

Update the camera state according to the different inputs gathered during the frame.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/camera.ts:677

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

[Node](Node.md).[AddNodeConstructor](Node.md#addnodeconstructor)

#### Defined in

packages/dev/core/src/node.ts:63

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

[Node](Node.md).[Construct](Node.md#construct)

#### Defined in

packages/dev/core/src/node.ts:75

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

#### Defined in

packages/dev/core/src/Cameras/camera.ts:1403

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

#### Defined in

packages/dev/core/src/Cameras/camera.ts:1432

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

[Node](Node.md).[ParseAnimationRanges](Node.md#parseanimationranges)

#### Defined in

packages/dev/core/src/node.ts:919
