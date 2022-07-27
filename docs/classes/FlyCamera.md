[@dev/core](../README.md) / [Exports](../modules.md) / FlyCamera

# Class: FlyCamera

This is a flying camera, designed for 3D movement and rotation in all directions,
such as in a 3D Space Shooter or a Flight Simulator.

## Hierarchy

- [`TargetCamera`](TargetCamera.md)

  ↳ **`FlyCamera`**

## Table of contents

### Constructors

- [constructor](FlyCamera.md#constructor)

### Properties

- [\_collider](FlyCamera.md#_collider)
- [\_collisionMask](FlyCamera.md#_collisionmask)
- [\_diffPosition](FlyCamera.md#_diffposition)
- [\_globalPosition](FlyCamera.md#_globalposition)
- [\_isDirty](FlyCamera.md#_isdirty)
- [\_needMoveForGravity](FlyCamera.md#_needmoveforgravity)
- [\_newPosition](FlyCamera.md#_newposition)
- [\_oldPosition](FlyCamera.md#_oldposition)
- [\_parentNode](FlyCamera.md#_parentnode)
- [\_ranges](FlyCamera.md#_ranges)
- [\_trackRoll](FlyCamera.md#_trackroll)
- [\_upVector](FlyCamera.md#_upvector)
- [\_webvrViewMatrix](FlyCamera.md#_webvrviewmatrix)
- [animations](FlyCamera.md#animations)
- [applyGravity](FlyCamera.md#applygravity)
- [bankedTurn](FlyCamera.md#bankedturn)
- [bankedTurnLimit](FlyCamera.md#bankedturnlimit)
- [bankedTurnMultiplier](FlyCamera.md#bankedturnmultiplier)
- [cameraDirection](FlyCamera.md#cameradirection)
- [cameraRigMode](FlyCamera.md#camerarigmode)
- [cameraRotation](FlyCamera.md#camerarotation)
- [checkCollisions](FlyCamera.md#checkcollisions)
- [customRenderTargets](FlyCamera.md#customrendertargets)
- [ellipsoid](FlyCamera.md#ellipsoid)
- [ellipsoidOffset](FlyCamera.md#ellipsoidoffset)
- [fov](FlyCamera.md#fov)
- [fovMode](FlyCamera.md#fovmode)
- [id](FlyCamera.md#id)
- [ignoreParentScaling](FlyCamera.md#ignoreparentscaling)
- [inertia](FlyCamera.md#inertia)
- [inputs](FlyCamera.md#inputs)
- [inspectableCustomProperties](FlyCamera.md#inspectablecustomproperties)
- [interaxialDistance](FlyCamera.md#interaxialdistance)
- [inverseRotationSpeed](FlyCamera.md#inverserotationspeed)
- [invertRotation](FlyCamera.md#invertrotation)
- [isIntermediate](FlyCamera.md#isintermediate)
- [isRigCamera](FlyCamera.md#isrigcamera)
- [isStereoscopicSideBySide](FlyCamera.md#isstereoscopicsidebyside)
- [layerMask](FlyCamera.md#layermask)
- [lockedTarget](FlyCamera.md#lockedtarget)
- [maxZ](FlyCamera.md#maxz)
- [metadata](FlyCamera.md#metadata)
- [minZ](FlyCamera.md#minz)
- [name](FlyCamera.md#name)
- [noRotationConstraint](FlyCamera.md#norotationconstraint)
- [onAfterCheckInputsObservable](FlyCamera.md#onaftercheckinputsobservable)
- [onCollide](FlyCamera.md#oncollide)
- [onDisposeObservable](FlyCamera.md#ondisposeobservable)
- [onProjectionMatrixChangedObservable](FlyCamera.md#onprojectionmatrixchangedobservable)
- [onReady](FlyCamera.md#onready)
- [onRestoreStateObservable](FlyCamera.md#onrestorestateobservable)
- [onViewMatrixChangedObservable](FlyCamera.md#onviewmatrixchangedobservable)
- [outputRenderTarget](FlyCamera.md#outputrendertarget)
- [projectionPlaneTilt](FlyCamera.md#projectionplanetilt)
- [renderPassId](FlyCamera.md#renderpassid)
- [reservedDataStore](FlyCamera.md#reserveddatastore)
- [rigParent](FlyCamera.md#rigparent)
- [rollCorrect](FlyCamera.md#rollcorrect)
- [rotation](FlyCamera.md#rotation)
- [rotationQuaternion](FlyCamera.md#rotationquaternion)
- [speed](FlyCamera.md#speed)
- [state](FlyCamera.md#state)
- [uniqueId](FlyCamera.md#uniqueid)
- [updateUpVectorFromRotation](FlyCamera.md#updateupvectorfromrotation)
- [viewport](FlyCamera.md#viewport)
- [FOVMODE\_HORIZONTAL\_FIXED](FlyCamera.md#fovmode_horizontal_fixed)
- [FOVMODE\_VERTICAL\_FIXED](FlyCamera.md#fovmode_vertical_fixed)
- [ForceAttachControlToAlwaysPreventDefault](FlyCamera.md#forceattachcontroltoalwayspreventdefault)
- [ORTHOGRAPHIC\_CAMERA](FlyCamera.md#orthographic_camera)
- [PERSPECTIVE\_CAMERA](FlyCamera.md#perspective_camera)
- [RIG\_MODE\_CUSTOM](FlyCamera.md#rig_mode_custom)
- [RIG\_MODE\_NONE](FlyCamera.md#rig_mode_none)
- [RIG\_MODE\_STEREOSCOPIC\_ANAGLYPH](FlyCamera.md#rig_mode_stereoscopic_anaglyph)
- [RIG\_MODE\_STEREOSCOPIC\_INTERLACED](FlyCamera.md#rig_mode_stereoscopic_interlaced)
- [RIG\_MODE\_STEREOSCOPIC\_OVERUNDER](FlyCamera.md#rig_mode_stereoscopic_overunder)
- [RIG\_MODE\_STEREOSCOPIC\_SIDEBYSIDE\_CROSSEYED](FlyCamera.md#rig_mode_stereoscopic_sidebyside_crosseyed)
- [RIG\_MODE\_STEREOSCOPIC\_SIDEBYSIDE\_PARALLEL](FlyCamera.md#rig_mode_stereoscopic_sidebyside_parallel)
- [RIG\_MODE\_VR](FlyCamera.md#rig_mode_vr)
- [RIG\_MODE\_WEBVR](FlyCamera.md#rig_mode_webvr)

### Accessors

- [absoluteRotation](FlyCamera.md#absoluterotation)
- [angularSensibility](FlyCamera.md#angularsensibility)
- [animationPropertiesOverride](FlyCamera.md#animationpropertiesoverride)
- [behaviors](FlyCamera.md#behaviors)
- [collisionMask](FlyCamera.md#collisionmask)
- [doNotSerialize](FlyCamera.md#donotserialize)
- [globalPosition](FlyCamera.md#globalposition)
- [isLeftCamera](FlyCamera.md#isleftcamera)
- [isRightCamera](FlyCamera.md#isrightcamera)
- [keysBackward](FlyCamera.md#keysbackward)
- [keysDown](FlyCamera.md#keysdown)
- [keysForward](FlyCamera.md#keysforward)
- [keysLeft](FlyCamera.md#keysleft)
- [keysRight](FlyCamera.md#keysright)
- [keysUp](FlyCamera.md#keysup)
- [leftCamera](FlyCamera.md#leftcamera)
- [mode](FlyCamera.md#mode)
- [onClonedObservable](FlyCamera.md#onclonedobservable)
- [onDispose](FlyCamera.md#ondispose)
- [onEnabledStateChangedObservable](FlyCamera.md#onenabledstatechangedobservable)
- [orthoBottom](FlyCamera.md#orthobottom)
- [orthoLeft](FlyCamera.md#ortholeft)
- [orthoRight](FlyCamera.md#orthoright)
- [orthoTop](FlyCamera.md#orthotop)
- [parent](FlyCamera.md#parent)
- [position](FlyCamera.md#position)
- [rigPostProcess](FlyCamera.md#rigpostprocess)
- [rightCamera](FlyCamera.md#rightcamera)
- [screenArea](FlyCamera.md#screenarea)
- [target](FlyCamera.md#target)
- [upVector](FlyCamera.md#upvector)
- [worldMatrixFromCache](FlyCamera.md#worldmatrixfromcache)

### Methods

- [\_computeViewMatrix](FlyCamera.md#_computeviewmatrix)
- [\_getFirstPostProcess](FlyCamera.md#_getfirstpostprocess)
- [\_setRigMode](FlyCamera.md#_setrigmode)
- [\_updateCameraRotationMatrix](FlyCamera.md#_updatecamerarotationmatrix)
- [\_updateWebVRCameraRotationMatrix](FlyCamera.md#_updatewebvrcamerarotationmatrix)
- [addBehavior](FlyCamera.md#addbehavior)
- [applyVerticalCorrection](FlyCamera.md#applyverticalcorrection)
- [attachControl](FlyCamera.md#attachcontrol)
- [attachPostProcess](FlyCamera.md#attachpostprocess)
- [beginAnimation](FlyCamera.md#beginanimation)
- [clone](FlyCamera.md#clone)
- [computeWorldMatrix](FlyCamera.md#computeworldmatrix)
- [createAnimationRange](FlyCamera.md#createanimationrange)
- [deleteAnimationRange](FlyCamera.md#deleteanimationrange)
- [detachControl](FlyCamera.md#detachcontrol)
- [detachPostProcess](FlyCamera.md#detachpostprocess)
- [dispose](FlyCamera.md#dispose)
- [freezeProjectionMatrix](FlyCamera.md#freezeprojectionmatrix)
- [getActiveMeshes](FlyCamera.md#getactivemeshes)
- [getAnimationByName](FlyCamera.md#getanimationbyname)
- [getAnimationRange](FlyCamera.md#getanimationrange)
- [getAnimationRanges](FlyCamera.md#getanimationranges)
- [getBehaviorByName](FlyCamera.md#getbehaviorbyname)
- [getChildMeshes](FlyCamera.md#getchildmeshes)
- [getChildren](FlyCamera.md#getchildren)
- [getClassName](FlyCamera.md#getclassname)
- [getDescendants](FlyCamera.md#getdescendants)
- [getDirection](FlyCamera.md#getdirection)
- [getDirectionToRef](FlyCamera.md#getdirectiontoref)
- [getEngine](FlyCamera.md#getengine)
- [getForwardRay](FlyCamera.md#getforwardray)
- [getForwardRayToRef](FlyCamera.md#getforwardraytoref)
- [getFrontPosition](FlyCamera.md#getfrontposition)
- [getHierarchyBoundingVectors](FlyCamera.md#gethierarchyboundingvectors)
- [getLeftTarget](FlyCamera.md#getlefttarget)
- [getProjectionMatrix](FlyCamera.md#getprojectionmatrix)
- [getRightTarget](FlyCamera.md#getrighttarget)
- [getScene](FlyCamera.md#getscene)
- [getTarget](FlyCamera.md#gettarget)
- [getTransformationMatrix](FlyCamera.md#gettransformationmatrix)
- [getViewMatrix](FlyCamera.md#getviewmatrix)
- [getWorldMatrix](FlyCamera.md#getworldmatrix)
- [isActiveMesh](FlyCamera.md#isactivemesh)
- [isCompletelyInFrustum](FlyCamera.md#iscompletelyinfrustum)
- [isDescendantOf](FlyCamera.md#isdescendantof)
- [isDisposed](FlyCamera.md#isdisposed)
- [isEnabled](FlyCamera.md#isenabled)
- [isInFrustum](FlyCamera.md#isinfrustum)
- [isReady](FlyCamera.md#isready)
- [markAsDirty](FlyCamera.md#markasdirty)
- [removeBehavior](FlyCamera.md#removebehavior)
- [restoreState](FlyCamera.md#restorestate)
- [serialize](FlyCamera.md#serialize)
- [serializeAnimationRanges](FlyCamera.md#serializeanimationranges)
- [setEnabled](FlyCamera.md#setenabled)
- [setTarget](FlyCamera.md#settarget)
- [storeState](FlyCamera.md#storestate)
- [toString](FlyCamera.md#tostring)
- [unfreezeProjectionMatrix](FlyCamera.md#unfreezeprojectionmatrix)
- [update](FlyCamera.md#update)
- [AddNodeConstructor](FlyCamera.md#addnodeconstructor)
- [Construct](FlyCamera.md#construct)
- [GetConstructorFromName](FlyCamera.md#getconstructorfromname)
- [Parse](FlyCamera.md#parse)
- [ParseAnimationRanges](FlyCamera.md#parseanimationranges)

## Constructors

### constructor

• **new FlyCamera**(`name`, `position`, `scene?`, `setActiveOnSceneIfNoneActive?`)

Instantiates a FlyCamera.
This is a flying camera, designed for 3D movement and rotation in all directions,
such as in a 3D Space Shooter or a Flight Simulator.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | Define the name of the camera in the scene. |
| `position` | [`Vector3`](Vector3.md) | `undefined` | Define the starting position of the camera in the scene. |
| `scene?` | [`Scene`](Scene.md) | `undefined` | Define the scene the camera belongs to. |
| `setActiveOnSceneIfNoneActive` | `boolean` | `true` | Defines whether the camera should be marked as active, if no other camera has been defined as active. |

#### Overrides

[TargetCamera](TargetCamera.md).[constructor](TargetCamera.md#constructor)

#### Defined in

packages/dev/core/src/Cameras/flyCamera.ts:270

## Properties

### \_collider

• `Private` **\_collider**: `Collider`

#### Defined in

packages/dev/core/src/Cameras/flyCamera.ts:250

___

### \_collisionMask

• `Private` **\_collisionMask**: `number` = `-1`

#### Defined in

packages/dev/core/src/Cameras/flyCamera.ts:303

___

### \_diffPosition

• `Private` **\_diffPosition**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Cameras/flyCamera.ts:253

___

### \_globalPosition

• `Protected` **\_globalPosition**: [`Vector3`](Vector3.md)

#### Inherited from

[TargetCamera](TargetCamera.md).[_globalPosition](TargetCamera.md#_globalposition)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:412

___

### \_isDirty

• `Protected` **\_isDirty**: `boolean` = `false`

#### Inherited from

[TargetCamera](TargetCamera.md).[_isDirty](TargetCamera.md#_isdirty)

#### Defined in

packages/dev/core/src/node.ts:43

___

### \_needMoveForGravity

• `Private` **\_needMoveForGravity**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Cameras/flyCamera.ts:251

___

### \_newPosition

• `Private` **\_newPosition**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Cameras/flyCamera.ts:254

___

### \_oldPosition

• `Private` **\_oldPosition**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Cameras/flyCamera.ts:252

___

### \_parentNode

• `Protected` **\_parentNode**: [`Nullable`](../modules.md#nullable)[`Node`](Node.md) = `null`

#### Inherited from

[TargetCamera](TargetCamera.md).[_parentNode](TargetCamera.md#_parentnode)

#### Defined in

packages/dev/core/src/node.ts:176

___

### \_ranges

• `Protected` **\_ranges**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: [`Nullable`](../modules.md#nullable)`AnimationRange`

#### Inherited from

[TargetCamera](TargetCamera.md).[_ranges](TargetCamera.md#_ranges)

#### Defined in

packages/dev/core/src/node.ts:154

___

### \_trackRoll

• **\_trackRoll**: `number` = `0`

Track Roll to maintain the wanted Rolling when looking around.

#### Defined in

packages/dev/core/src/Cameras/flyCamera.ts:63

___

### \_upVector

• `Protected` **\_upVector**: [`Vector3`](Vector3.md)

#### Inherited from

[TargetCamera](TargetCamera.md).[_upVector](TargetCamera.md#_upvector)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:129

___

### \_webvrViewMatrix

• `Protected` **\_webvrViewMatrix**: [`Matrix`](Matrix.md)

#### Inherited from

[TargetCamera](TargetCamera.md).[_webvrViewMatrix](TargetCamera.md#_webvrviewmatrix)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:399

___

### animations

• **animations**: [`Animation`](Animation.md)[]

Gets a list of Animations associated with the node

#### Inherited from

[TargetCamera](TargetCamera.md).[animations](TargetCamera.md#animations)

#### Defined in

packages/dev/core/src/node.ts:153

___

### applyGravity

• **applyGravity**: `boolean` = `false`

Enable or disable gravity on the camera.

#### Defined in

packages/dev/core/src/Cameras/flyCamera.ts:47

___

### bankedTurn

• **bankedTurn**: `boolean` = `false`

Mimic a banked turn, Rolling the camera when Yawing.
It's recommended to use rollCorrect = 10 for faster banking correction.

#### Defined in

packages/dev/core/src/Cameras/flyCamera.ts:74

___

### bankedTurnLimit

• **bankedTurnLimit**: `number`

Limit in radians for how much Roll banking will add. (Default: 90°)

#### Defined in

packages/dev/core/src/Cameras/flyCamera.ts:79

___

### bankedTurnMultiplier

• **bankedTurnMultiplier**: `number` = `1`

Value of 0 disables the banked Roll.
Value of 1 is equal to the Yaw angle in radians.

#### Defined in

packages/dev/core/src/Cameras/flyCamera.ts:85

___

### cameraDirection

• **cameraDirection**: [`Vector3`](Vector3.md)

Define the current direction the camera is moving to.

#### Overrides

[TargetCamera](TargetCamera.md).[cameraDirection](TargetCamera.md#cameradirection)

#### Defined in

packages/dev/core/src/Cameras/flyCamera.ts:52

___

### cameraRigMode

• **cameraRigMode**: `number` = `Camera.RIG_MODE_NONE`

Rig mode of the camera.
This is useful to create the camera with two "eyes" instead of one to create VR or stereoscopic scenes.
This is normally controlled byt the camera themselves as internal use.

#### Inherited from

[TargetCamera](TargetCamera.md).[cameraRigMode](TargetCamera.md#camerarigmode)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:330

___

### cameraRotation

• **cameraRotation**: [`Vector2`](Vector2.md)

Define the current rotation the camera is rotating to

#### Inherited from

[TargetCamera](TargetCamera.md).[cameraRotation](TargetCamera.md#camerarotation)

#### Defined in

packages/dev/core/src/Cameras/targetCamera.ts:28

___

### checkCollisions

• **checkCollisions**: `boolean` = `false`

Enable or disable collisions of the camera with the rest of the scene objects.

#### Defined in

packages/dev/core/src/Cameras/flyCamera.ts:41

___

### customRenderTargets

• **customRenderTargets**: [`RenderTargetTexture`](RenderTargetTexture.md)[]

Defines the list of custom render target which are rendered to and then used as the input to this camera's render. Eg. display another camera view on a TV in the main scene
This is pretty helpful if you wish to make a camera render to a texture you could reuse somewhere
else in the scene. (Eg. security camera)

To change the final output target of the camera, camera.outputRenderTarget should be used instead (eg. webXR renders to a render target corresponding to an HMD)

#### Inherited from

[TargetCamera](TargetCamera.md).[customRenderTargets](TargetCamera.md#customrendertargets)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:351

___

### ellipsoid

• **ellipsoid**: [`Vector3`](Vector3.md)

Define the collision ellipsoid of the camera.
This is helpful for simulating a camera body, like a player's body.

**`See`**

https://doc.babylonjs.com/babylon101/cameras,_mesh_collisions_and_gravity#arcrotatecamera

#### Defined in

packages/dev/core/src/Cameras/flyCamera.ts:27

___

### ellipsoidOffset

• **ellipsoidOffset**: [`Vector3`](Vector3.md)

Define an offset for the position of the ellipsoid around the camera.
This can be helpful if the camera is attached away from the player's body center,
such as at its head.

#### Defined in

packages/dev/core/src/Cameras/flyCamera.ts:35

___

### fov

• **fov**: `number` = `0.8`

Field Of View is set in Radians. (default is 0.8)

#### Inherited from

[TargetCamera](TargetCamera.md).[fov](TargetCamera.md#fov)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:248

___

### fovMode

• **fovMode**: `number` = `Camera.FOVMODE_VERTICAL_FIXED`

fovMode sets the camera frustum bounds to the viewport bounds. (default is FOVMODE_VERTICAL_FIXED)

#### Inherited from

[TargetCamera](TargetCamera.md).[fovMode](TargetCamera.md#fovmode)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:322

___

### id

• **id**: `string`

Gets or sets the id of the node

#### Inherited from

[TargetCamera](TargetCamera.md).[id](TargetCamera.md#id)

#### Defined in

packages/dev/core/src/node.ts:97

___

### ignoreParentScaling

• **ignoreParentScaling**: `boolean` = `false`

Gets or sets a boolean indicating that the scaling of the parent hierarchy will not be taken in account by the camera

#### Inherited from

[TargetCamera](TargetCamera.md).[ignoreParentScaling](TargetCamera.md#ignoreparentscaling)

#### Defined in

packages/dev/core/src/Cameras/targetCamera.ts:31

___

### inertia

• **inertia**: `number` = `0.9`

Define the default inertia of the camera.
This helps giving a smooth feeling to the camera movement.

#### Inherited from

[TargetCamera](TargetCamera.md).[inertia](TargetCamera.md#inertia)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:279

___

### inputs

• **inputs**: [`FlyCameraInputsManager`](FlyCameraInputsManager.md)

The inputs manager loads all the input sources, such as keyboard and mouse.

#### Overrides

[TargetCamera](TargetCamera.md).[inputs](TargetCamera.md#inputs)

#### Defined in

packages/dev/core/src/Cameras/flyCamera.ts:90

___

### inspectableCustomProperties

• **inspectableCustomProperties**: [`IInspectable`](../interfaces/IInspectable.md)[]

List of inspectable custom properties (used by the Inspector)

**`See`**

https://doc.babylonjs.com/how_to/debug_layer#extensibility

#### Inherited from

[TargetCamera](TargetCamera.md).[inspectableCustomProperties](TargetCamera.md#inspectablecustomproperties)

#### Defined in

packages/dev/core/src/node.ts:126

___

### interaxialDistance

• **interaxialDistance**: `number`

Defines the distance between both "eyes" in case of a RIG

#### Inherited from

[TargetCamera](TargetCamera.md).[interaxialDistance](TargetCamera.md#interaxialdistance)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:336

___

### inverseRotationSpeed

• **inverseRotationSpeed**: `number` = `0.2`

Speed multiplier for inverse camera panning

#### Inherited from

[TargetCamera](TargetCamera.md).[inverseRotationSpeed](TargetCamera.md#inverserotationspeed)

#### Defined in

packages/dev/core/src/Cameras/targetCamera.ts:71

___

### invertRotation

• **invertRotation**: `boolean` = `false`

Reverses mouselook direction to 'natural' panning as opposed to traditional direct
panning

#### Inherited from

[TargetCamera](TargetCamera.md).[invertRotation](TargetCamera.md#invertrotation)

#### Defined in

packages/dev/core/src/Cameras/targetCamera.ts:66

___

### isIntermediate

• **isIntermediate**: `boolean` = `false`

Define whether the camera is intermediate.
This is useful to not present the output directly to the screen in case of rig without post process for instance

#### Inherited from

[TargetCamera](TargetCamera.md).[isIntermediate](TargetCamera.md#isintermediate)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:303

___

### isRigCamera

• **isRigCamera**: `boolean` = `false`

Is this camera a part of a rig system?

#### Inherited from

[TargetCamera](TargetCamera.md).[isRigCamera](TargetCamera.md#isrigcamera)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:379

___

### isStereoscopicSideBySide

• **isStereoscopicSideBySide**: `boolean`

Defines if stereoscopic rendering is done side by side or over under.

#### Inherited from

[TargetCamera](TargetCamera.md).[isStereoscopicSideBySide](TargetCamera.md#isstereoscopicsidebyside)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:342

___

### layerMask

• **layerMask**: `number` = `0x0fffffff`

Restricts the camera to viewing objects with the same layerMask.
A camera with a layerMask of 1 will render mesh.layerMask & camera.layerMask!== 0

#### Inherited from

[TargetCamera](TargetCamera.md).[layerMask](TargetCamera.md#layermask)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:316

___

### lockedTarget

• **lockedTarget**: `any` = `null`

Define the current target of the camera as an object or a position.
Please note that locking a target will disable panning.

#### Inherited from

[TargetCamera](TargetCamera.md).[lockedTarget](TargetCamera.md#lockedtarget)

#### Defined in

packages/dev/core/src/Cameras/targetCamera.ts:78

___

### maxZ

• **maxZ**: `number` = `10000.0`

Define the maximum distance the camera can see to.
This is important to note that the depth buffer are not infinite and the further it end
the more your scene might encounter depth fighting issue.

#### Inherited from

[TargetCamera](TargetCamera.md).[maxZ](TargetCamera.md#maxz)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:272

___

### metadata

• **metadata**: `any` = `null`

Gets or sets an object used to store user defined information for the node

#### Inherited from

[TargetCamera](TargetCamera.md).[metadata](TargetCamera.md#metadata)

#### Defined in

packages/dev/core/src/node.ts:115

___

### minZ

• **minZ**: `number` = `1`

Define the minimum distance the camera can see from.
This is important to note that the depth buffer are not infinite and the closer it starts
the more your scene might encounter depth fighting issue.

#### Inherited from

[TargetCamera](TargetCamera.md).[minZ](TargetCamera.md#minz)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:264

___

### name

• **name**: `string`

Gets or sets the name of the node

#### Inherited from

[TargetCamera](TargetCamera.md).[name](TargetCamera.md#name)

#### Defined in

packages/dev/core/src/node.ts:91

___

### noRotationConstraint

• **noRotationConstraint**: `boolean` = `false`

Add constraint to the camera to prevent it to move freely in all directions and
around all axis.

#### Inherited from

[TargetCamera](TargetCamera.md).[noRotationConstraint](TargetCamera.md#norotationconstraint)

#### Defined in

packages/dev/core/src/Cameras/targetCamera.ts:60

___

### onAfterCheckInputsObservable

• **onAfterCheckInputsObservable**: [`Observable`](Observable.md)[`Camera`](Camera.md)

Observable triggered when the inputs have been processed.

#### Inherited from

[TargetCamera](TargetCamera.md).[onAfterCheckInputsObservable](TargetCamera.md#onaftercheckinputsobservable)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:370

___

### onCollide

• **onCollide**: (`collidedMesh`: [`AbstractMesh`](AbstractMesh.md)) => `void`

#### Type declaration

▸ (`collidedMesh`): `void`

Event raised when the camera collides with a mesh in the scene.

##### Parameters

| Name | Type |
| :------ | :------ |
| `collidedMesh` | [`AbstractMesh`](AbstractMesh.md) |

##### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/flyCamera.ts:248

___

### onDisposeObservable

• **onDisposeObservable**: [`Observable`](Observable.md)[`Node`](Node.md)

An event triggered when the mesh is disposed

#### Inherited from

[TargetCamera](TargetCamera.md).[onDisposeObservable](TargetCamera.md#ondisposeobservable)

#### Defined in

packages/dev/core/src/node.ts:300

___

### onProjectionMatrixChangedObservable

• **onProjectionMatrixChangedObservable**: [`Observable`](Observable.md)[`Camera`](Camera.md)

Observable triggered when the camera Projection matrix has changed.

#### Inherited from

[TargetCamera](TargetCamera.md).[onProjectionMatrixChangedObservable](TargetCamera.md#onprojectionmatrixchangedobservable)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:366

___

### onReady

• **onReady**: [`Nullable`](../modules.md#nullable)(`node`: [`Node`](Node.md)) => `void` = `null`

Callback raised when the node is ready to be used

#### Inherited from

[TargetCamera](TargetCamera.md).[onReady](TargetCamera.md#onready)

#### Defined in

packages/dev/core/src/node.ts:159

___

### onRestoreStateObservable

• **onRestoreStateObservable**: [`Observable`](Observable.md)[`Camera`](Camera.md)

Observable triggered when reset has been called and applied to the camera.

#### Inherited from

[TargetCamera](TargetCamera.md).[onRestoreStateObservable](TargetCamera.md#onrestorestateobservable)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:374

___

### onViewMatrixChangedObservable

• **onViewMatrixChangedObservable**: [`Observable`](Observable.md)[`Camera`](Camera.md)

Observable triggered when the camera view matrix has changed.

#### Inherited from

[TargetCamera](TargetCamera.md).[onViewMatrixChangedObservable](TargetCamera.md#onviewmatrixchangedobservable)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:362

___

### outputRenderTarget

• **outputRenderTarget**: [`Nullable`](../modules.md#nullable)[`RenderTargetTexture`](RenderTargetTexture.md) = `null`

When set, the camera will render to this render target instead of the default canvas

If the desire is to use the output of a camera as a texture in the scene consider using camera.customRenderTargets instead

#### Inherited from

[TargetCamera](TargetCamera.md).[outputRenderTarget](TargetCamera.md#outputrendertarget)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:357

___

### projectionPlaneTilt

• **projectionPlaneTilt**: `number` = `0`

Projection plane tilt around the X axis (horizontal), set in Radians. (default is 0)
Can be used to make vertical lines in world space actually vertical on the screen.
See https://forum.babylonjs.com/t/add-vertical-shift-to-3ds-max-exporter-babylon-cameras/17480

#### Inherited from

[TargetCamera](TargetCamera.md).[projectionPlaneTilt](TargetCamera.md#projectionplanetilt)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:256

___

### renderPassId

• **renderPassId**: `number`

Render pass id used by the camera to render into the main framebuffer

#### Inherited from

[TargetCamera](TargetCamera.md).[renderPassId](TargetCamera.md#renderpassid)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:390

___

### reservedDataStore

• **reservedDataStore**: `any` = `null`

For internal use only. Please do not use.

#### Inherited from

[TargetCamera](TargetCamera.md).[reservedDataStore](TargetCamera.md#reserveddatastore)

#### Defined in

packages/dev/core/src/node.ts:120

___

### rigParent

• `Optional` **rigParent**: [`Camera`](Camera.md)

If isRigCamera set to true this will be set with the parent camera.
The parent camera is not (!) necessarily the .parent of this camera (like in the case of XR)

#### Inherited from

[TargetCamera](TargetCamera.md).[rigParent](TargetCamera.md#rigparent)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:385

___

### rollCorrect

• **rollCorrect**: `number` = `100`

Slowly correct the Roll to its original value after a Pitch+Yaw rotation.

#### Defined in

packages/dev/core/src/Cameras/flyCamera.ts:68

___

### rotation

• **rotation**: [`Vector3`](Vector3.md)

Define the current rotation of the camera

#### Inherited from

[TargetCamera](TargetCamera.md).[rotation](TargetCamera.md#rotation)

#### Defined in

packages/dev/core/src/Cameras/targetCamera.ts:43

___

### rotationQuaternion

• **rotationQuaternion**: [`Quaternion`](Quaternion.md)

Define the current local rotation of the camera as a quaternion to prevent Gimbal lock.
This overrides and empties cameraRotation.

#### Overrides

[TargetCamera](TargetCamera.md).[rotationQuaternion](TargetCamera.md#rotationquaternion)

#### Defined in

packages/dev/core/src/Cameras/flyCamera.ts:58

___

### speed

• **speed**: `number` = `2.0`

Define the current speed of the camera

#### Inherited from

[TargetCamera](TargetCamera.md).[speed](TargetCamera.md#speed)

#### Defined in

packages/dev/core/src/Cameras/targetCamera.ts:54

___

### state

• **state**: `string` = `""`

Gets or sets a string used to store user defined state for the node

#### Inherited from

[TargetCamera](TargetCamera.md).[state](TargetCamera.md#state)

#### Defined in

packages/dev/core/src/node.ts:109

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the node

#### Inherited from

[TargetCamera](TargetCamera.md).[uniqueId](TargetCamera.md#uniqueid)

#### Defined in

packages/dev/core/src/node.ts:103

___

### updateUpVectorFromRotation

• **updateUpVectorFromRotation**: `boolean` = `false`

When set, the up vector of the camera will be updated by the rotation of the camera

#### Inherited from

[TargetCamera](TargetCamera.md).[updateUpVectorFromRotation](TargetCamera.md#updateupvectorfromrotation)

#### Defined in

packages/dev/core/src/Cameras/targetCamera.ts:36

___

### viewport

• **viewport**: [`Viewport`](Viewport.md)

Define the viewport of the camera.
This correspond to the portion of the screen the camera will render to in normalized 0 to 1 unit.

#### Inherited from

[TargetCamera](TargetCamera.md).[viewport](TargetCamera.md#viewport)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:309

___

### FOVMODE\_HORIZONTAL\_FIXED

▪ `Static` `Readonly` **FOVMODE\_HORIZONTAL\_FIXED**: ``1``

This setting aligns the left and right bounds of the viewport to the left and right bounds of the camera frustum.

#### Inherited from

[TargetCamera](TargetCamera.md).[FOVMODE_HORIZONTAL_FIXED](TargetCamera.md#fovmode_horizontal_fixed)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:62

___

### FOVMODE\_VERTICAL\_FIXED

▪ `Static` `Readonly` **FOVMODE\_VERTICAL\_FIXED**: ``0``

This is the default FOV mode for perspective cameras.
This setting aligns the upper and lower bounds of the viewport to the upper and lower bounds of the camera frustum.

#### Inherited from

[TargetCamera](TargetCamera.md).[FOVMODE_VERTICAL_FIXED](TargetCamera.md#fovmode_vertical_fixed)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:58

___

### ForceAttachControlToAlwaysPreventDefault

▪ `Static` **ForceAttachControlToAlwaysPreventDefault**: `boolean` = `false`

Defines if by default attaching controls should prevent the default javascript event to continue.

#### Inherited from

[TargetCamera](TargetCamera.md).[ForceAttachControlToAlwaysPreventDefault](TargetCamera.md#forceattachcontroltoalwayspreventdefault)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:106

___

### ORTHOGRAPHIC\_CAMERA

▪ `Static` `Readonly` **ORTHOGRAPHIC\_CAMERA**: ``1``

This helps creating camera with an orthographic mode.
Orthographic is commonly used in engineering as a means to produce object specifications that communicate dimensions unambiguously, each line of 1 unit length (cm, meter..whatever) will appear to have the same length everywhere on the drawing. This allows the drafter to dimension only a subset of lines and let the reader know that other lines of that length on the drawing are also that length in reality. Every parallel line in the drawing is also parallel in the object.

#### Inherited from

[TargetCamera](TargetCamera.md).[ORTHOGRAPHIC_CAMERA](TargetCamera.md#orthographic_camera)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:52

___

### PERSPECTIVE\_CAMERA

▪ `Static` `Readonly` **PERSPECTIVE\_CAMERA**: ``0``

This is the default projection mode used by the cameras.
It helps recreating a feeling of perspective and better appreciate depth.
This is the best way to simulate real life cameras.

#### Inherited from

[TargetCamera](TargetCamera.md).[PERSPECTIVE_CAMERA](TargetCamera.md#perspective_camera)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:47

___

### RIG\_MODE\_CUSTOM

▪ `Static` `Readonly` **RIG\_MODE\_CUSTOM**: ``22``

Custom rig mode allowing rig cameras to be populated manually with any number of cameras

#### Inherited from

[TargetCamera](TargetCamera.md).[RIG_MODE_CUSTOM](TargetCamera.md#rig_mode_custom)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:101

___

### RIG\_MODE\_NONE

▪ `Static` `Readonly` **RIG\_MODE\_NONE**: ``0``

This specifies there is no need for a camera rig.
Basically only one eye is rendered corresponding to the camera.

#### Inherited from

[TargetCamera](TargetCamera.md).[RIG_MODE_NONE](TargetCamera.md#rig_mode_none)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:68

___

### RIG\_MODE\_STEREOSCOPIC\_ANAGLYPH

▪ `Static` `Readonly` **RIG\_MODE\_STEREOSCOPIC\_ANAGLYPH**: ``10``

Simulates a camera Rig with one blue eye and one red eye.
This can be use with 3d blue and red glasses.

#### Inherited from

[TargetCamera](TargetCamera.md).[RIG_MODE_STEREOSCOPIC_ANAGLYPH](TargetCamera.md#rig_mode_stereoscopic_anaglyph)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:73

___

### RIG\_MODE\_STEREOSCOPIC\_INTERLACED

▪ `Static` `Readonly` **RIG\_MODE\_STEREOSCOPIC\_INTERLACED**: ``14``

Defines that both eyes of the camera will be rendered on successive lines interlaced for passive 3d monitors.

#### Inherited from

[TargetCamera](TargetCamera.md).[RIG_MODE_STEREOSCOPIC_INTERLACED](TargetCamera.md#rig_mode_stereoscopic_interlaced)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:89

___

### RIG\_MODE\_STEREOSCOPIC\_OVERUNDER

▪ `Static` `Readonly` **RIG\_MODE\_STEREOSCOPIC\_OVERUNDER**: ``13``

Defines that both eyes of the camera will be rendered over under each other.

#### Inherited from

[TargetCamera](TargetCamera.md).[RIG_MODE_STEREOSCOPIC_OVERUNDER](TargetCamera.md#rig_mode_stereoscopic_overunder)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:85

___

### RIG\_MODE\_STEREOSCOPIC\_SIDEBYSIDE\_CROSSEYED

▪ `Static` `Readonly` **RIG\_MODE\_STEREOSCOPIC\_SIDEBYSIDE\_CROSSEYED**: ``12``

Defines that both eyes of the camera will be rendered side by side with a none parallel target.

#### Inherited from

[TargetCamera](TargetCamera.md).[RIG_MODE_STEREOSCOPIC_SIDEBYSIDE_CROSSEYED](TargetCamera.md#rig_mode_stereoscopic_sidebyside_crosseyed)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:81

___

### RIG\_MODE\_STEREOSCOPIC\_SIDEBYSIDE\_PARALLEL

▪ `Static` `Readonly` **RIG\_MODE\_STEREOSCOPIC\_SIDEBYSIDE\_PARALLEL**: ``11``

Defines that both eyes of the camera will be rendered side by side with a parallel target.

#### Inherited from

[TargetCamera](TargetCamera.md).[RIG_MODE_STEREOSCOPIC_SIDEBYSIDE_PARALLEL](TargetCamera.md#rig_mode_stereoscopic_sidebyside_parallel)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:77

___

### RIG\_MODE\_VR

▪ `Static` `Readonly` **RIG\_MODE\_VR**: ``20``

Defines that both eyes of the camera should be renderered in a VR mode (carbox).

#### Inherited from

[TargetCamera](TargetCamera.md).[RIG_MODE_VR](TargetCamera.md#rig_mode_vr)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:93

___

### RIG\_MODE\_WEBVR

▪ `Static` `Readonly` **RIG\_MODE\_WEBVR**: ``21``

Defines that both eyes of the camera should be renderered in a VR mode (webVR).

#### Inherited from

[TargetCamera](TargetCamera.md).[RIG_MODE_WEBVR](TargetCamera.md#rig_mode_webvr)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:97

## Accessors

### absoluteRotation

• `get` **absoluteRotation**(): [`Quaternion`](Quaternion.md)

Returns the current camera absolute rotation

#### Returns

[`Quaternion`](Quaternion.md)

#### Inherited from

TargetCamera.absoluteRotation

#### Defined in

packages/dev/core/src/Cameras/camera.ts:1378

___

### angularSensibility

• `get` **angularSensibility**(): `number`

Gets the input sensibility for mouse input.
Higher values reduce sensitivity.

#### Returns

`number`

#### Defined in

packages/dev/core/src/Cameras/flyCamera.ts:96

• `set` **angularSensibility**(`value`): `void`

Sets the input sensibility for a mouse input.
Higher values reduce sensitivity.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/flyCamera.ts:109

___

### animationPropertiesOverride

• `get` **animationPropertiesOverride**(): [`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md)

Gets or sets the animation properties override

#### Returns

[`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md)

#### Inherited from

TargetCamera.animationPropertiesOverride

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

TargetCamera.animationPropertiesOverride

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

TargetCamera.behaviors

#### Defined in

packages/dev/core/src/node.ts:410

___

### collisionMask

• `get` **collisionMask**(): `number`

Get the mask that the camera ignores in collision events.

#### Returns

`number`

#### Defined in

packages/dev/core/src/Cameras/flyCamera.ts:308

• `set` **collisionMask**(`mask`): `void`

Set the mask that the camera ignores in collision events.

#### Parameters

| Name | Type |
| :------ | :------ |
| `mask` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/flyCamera.ts:315

___

### doNotSerialize

• `get` **doNotSerialize**(): `boolean`

Gets or sets a boolean used to define if the node must be serialized

#### Returns

`boolean`

#### Inherited from

TargetCamera.doNotSerialize

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

TargetCamera.doNotSerialize

#### Defined in

packages/dev/core/src/node.ts:143

___

### globalPosition

• `get` **globalPosition**(): [`Vector3`](Vector3.md)

Gets the current world space position of the camera.

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

TargetCamera.globalPosition

#### Defined in

packages/dev/core/src/Cameras/camera.ts:522

___

### isLeftCamera

• `get` **isLeftCamera**(): `boolean`

Gets the left camera of a rig setup in case of Rigged Camera

#### Returns

`boolean`

#### Inherited from

TargetCamera.isLeftCamera

#### Defined in

packages/dev/core/src/Cameras/camera.ts:1120

___

### isRightCamera

• `get` **isRightCamera**(): `boolean`

Gets the right camera of a rig setup in case of Rigged Camera

#### Returns

`boolean`

#### Inherited from

TargetCamera.isRightCamera

#### Defined in

packages/dev/core/src/Cameras/camera.ts:1129

___

### keysBackward

• `get` **keysBackward**(): `number`[]

Get the keys for camera movement backward.

#### Returns

`number`[]

#### Defined in

packages/dev/core/src/Cameras/flyCamera.ts:141

• `set` **keysBackward**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number`[] |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/flyCamera.ts:150

___

### keysDown

• `get` **keysDown**(): `number`[]

Get the keys for camera movement down.

#### Returns

`number`[]

#### Defined in

packages/dev/core/src/Cameras/flyCamera.ts:182

• `set` **keysDown**(`value`): `void`

Set the keys for camera movement down.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number`[] |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/flyCamera.ts:194

___

### keysForward

• `get` **keysForward**(): `number`[]

Get the keys for camera movement forward.

#### Returns

`number`[]

#### Defined in

packages/dev/core/src/Cameras/flyCamera.ts:119

• `set` **keysForward**(`value`): `void`

Set the keys for camera movement forward.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number`[] |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/flyCamera.ts:131

___

### keysLeft

• `get` **keysLeft**(): `number`[]

Get the keys for camera movement left.

#### Returns

`number`[]

#### Defined in

packages/dev/core/src/Cameras/flyCamera.ts:204

• `set` **keysLeft**(`value`): `void`

Set the keys for camera movement left.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number`[] |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/flyCamera.ts:216

___

### keysRight

• `get` **keysRight**(): `number`[]

Set the keys for camera movement right.

#### Returns

`number`[]

#### Defined in

packages/dev/core/src/Cameras/flyCamera.ts:226

• `set` **keysRight**(`value`): `void`

Set the keys for camera movement right.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number`[] |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/flyCamera.ts:238

___

### keysUp

• `get` **keysUp**(): `number`[]

Get the keys for camera movement up.

#### Returns

`number`[]

#### Defined in

packages/dev/core/src/Cameras/flyCamera.ts:160

• `set` **keysUp**(`value`): `void`

Set the keys for camera movement up.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number`[] |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Cameras/flyCamera.ts:172

___

### leftCamera

• `get` **leftCamera**(): [`Nullable`](../modules.md#nullable)[`FreeCamera`](FreeCamera.md)

Gets the left camera of a rig setup in case of Rigged Camera

#### Returns

[`Nullable`](../modules.md#nullable)[`FreeCamera`](FreeCamera.md)

#### Inherited from

TargetCamera.leftCamera

#### Defined in

packages/dev/core/src/Cameras/camera.ts:1136

___

### mode

• `get` **mode**(): `number`

#### Returns

`number`

#### Inherited from

TargetCamera.mode

#### Defined in

packages/dev/core/src/Cameras/camera.ts:294

• `set` **mode**(`mode`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `mode` | `number` |

#### Returns

`void`

#### Inherited from

TargetCamera.mode

#### Defined in

packages/dev/core/src/Cameras/camera.ts:285

___

### onClonedObservable

• `get` **onClonedObservable**(): [`Observable`](Observable.md)[`Node`](Node.md)

An event triggered when the node is cloned

#### Returns

[`Observable`](Observable.md)[`Node`](Node.md)

#### Inherited from

TargetCamera.onClonedObservable

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

TargetCamera.onDispose

#### Defined in

packages/dev/core/src/node.ts:306

___

### onEnabledStateChangedObservable

• `get` **onEnabledStateChangedObservable**(): [`Observable`](Observable.md)`boolean`

An event triggered when the enabled state of the node changes

#### Returns

[`Observable`](Observable.md)`boolean`

#### Inherited from

TargetCamera.onEnabledStateChangedObservable

#### Defined in

packages/dev/core/src/node.ts:316

___

### orthoBottom

• `get` **orthoBottom**(): [`Nullable`](../modules.md#nullable)`number`

#### Returns

[`Nullable`](../modules.md#nullable)`number`

#### Inherited from

TargetCamera.orthoBottom

#### Defined in

packages/dev/core/src/Cameras/camera.ts:220

• `set` **orthoBottom**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)`number` |

#### Returns

`void`

#### Inherited from

TargetCamera.orthoBottom

#### Defined in

packages/dev/core/src/Cameras/camera.ts:212

___

### orthoLeft

• `get` **orthoLeft**(): [`Nullable`](../modules.md#nullable)`number`

#### Returns

[`Nullable`](../modules.md#nullable)`number`

#### Inherited from

TargetCamera.orthoLeft

#### Defined in

packages/dev/core/src/Cameras/camera.ts:182

• `set` **orthoLeft**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)`number` |

#### Returns

`void`

#### Inherited from

TargetCamera.orthoLeft

#### Defined in

packages/dev/core/src/Cameras/camera.ts:174

___

### orthoRight

• `get` **orthoRight**(): [`Nullable`](../modules.md#nullable)`number`

#### Returns

[`Nullable`](../modules.md#nullable)`number`

#### Inherited from

TargetCamera.orthoRight

#### Defined in

packages/dev/core/src/Cameras/camera.ts:201

• `set` **orthoRight**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)`number` |

#### Returns

`void`

#### Inherited from

TargetCamera.orthoRight

#### Defined in

packages/dev/core/src/Cameras/camera.ts:193

___

### orthoTop

• `get` **orthoTop**(): [`Nullable`](../modules.md#nullable)`number`

#### Returns

[`Nullable`](../modules.md#nullable)`number`

#### Inherited from

TargetCamera.orthoTop

#### Defined in

packages/dev/core/src/Cameras/camera.ts:239

• `set` **orthoTop**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)`number` |

#### Returns

`void`

#### Inherited from

TargetCamera.orthoTop

#### Defined in

packages/dev/core/src/Cameras/camera.ts:231

___

### parent

• `get` **parent**(): [`Nullable`](../modules.md#nullable)[`Node`](Node.md)

#### Returns

[`Nullable`](../modules.md#nullable)[`Node`](Node.md)

#### Inherited from

TargetCamera.parent

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

TargetCamera.parent

#### Defined in

packages/dev/core/src/node.ts:200

___

### position

• `get` **position**(): [`Vector3`](Vector3.md)

Define the current local position of the camera in the scene

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

TargetCamera.position

#### Defined in

packages/dev/core/src/Cameras/camera.ts:120

• `set` **position**(`newPosition`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `newPosition` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Inherited from

TargetCamera.position

#### Defined in

packages/dev/core/src/Cameras/camera.ts:124

___

### rigPostProcess

• `get` **rigPostProcess**(): [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)

Gets the post process used by the rig cameras

#### Returns

[`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)

#### Inherited from

TargetCamera.rigPostProcess

#### Defined in

packages/dev/core/src/Cameras/camera.ts:697

___

### rightCamera

• `get` **rightCamera**(): [`Nullable`](../modules.md#nullable)[`FreeCamera`](FreeCamera.md)

Gets the right camera of a rig setup in case of Rigged Camera

#### Returns

[`Nullable`](../modules.md#nullable)[`FreeCamera`](FreeCamera.md)

#### Inherited from

TargetCamera.rightCamera

#### Defined in

packages/dev/core/src/Cameras/camera.ts:1146

___

### screenArea

• `get` **screenArea**(): `number`

The screen area in scene units squared

#### Returns

`number`

#### Inherited from

TargetCamera.screenArea

#### Defined in

packages/dev/core/src/Cameras/camera.ts:146

___

### target

• `get` **target**(): [`Vector3`](Vector3.md)

Defines the target point of the camera.
The camera looks towards it form the radius distance.

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

TargetCamera.target

#### Defined in

packages/dev/core/src/Cameras/targetCamera.ts:292

• `set` **target**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Inherited from

TargetCamera.target

#### Defined in

packages/dev/core/src/Cameras/targetCamera.ts:295

___

### upVector

• `get` **upVector**(): [`Vector3`](Vector3.md)

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

TargetCamera.upVector

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

#### Inherited from

TargetCamera.upVector

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

TargetCamera.worldMatrixFromCache

#### Defined in

packages/dev/core/src/node.ts:454

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

#### Inherited from

[TargetCamera](TargetCamera.md).[_computeViewMatrix](TargetCamera.md#_computeviewmatrix)

#### Defined in

packages/dev/core/src/Cameras/targetCamera.ts:448

___

### \_getFirstPostProcess

▸ **_getFirstPostProcess**(): [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)

Internal, gets the first post process.

#### Returns

[`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)

the first post process to be run on this camera.

#### Inherited from

[TargetCamera](TargetCamera.md).[_getFirstPostProcess](TargetCamera.md#_getfirstpostprocess)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:705

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

[TargetCamera](TargetCamera.md).[_setRigMode](TargetCamera.md#_setrigmode)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:1222

___

### \_updateCameraRotationMatrix

▸ `Protected` **_updateCameraRotationMatrix**(): `void`

#### Returns

`void`

#### Inherited from

[TargetCamera](TargetCamera.md).[_updateCameraRotationMatrix](TargetCamera.md#_updatecamerarotationmatrix)

#### Defined in

packages/dev/core/src/Cameras/targetCamera.ts:395

___

### \_updateWebVRCameraRotationMatrix

▸ `Protected` **_updateWebVRCameraRotationMatrix**(): `void`

#### Returns

`void`

#### Inherited from

[TargetCamera](TargetCamera.md).[_updateWebVRCameraRotationMatrix](TargetCamera.md#_updatewebvrcamerarotationmatrix)

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

[TargetCamera](TargetCamera.md).[addBehavior](TargetCamera.md#addbehavior)

#### Defined in

packages/dev/core/src/node.ts:366

___

### applyVerticalCorrection

▸ **applyVerticalCorrection**(): `void`

Automatically tilts the projection plane, using `projectionPlaneTilt`, to correct the perspective effect on vertical lines.

#### Returns

`void`

#### Inherited from

[TargetCamera](TargetCamera.md).[applyVerticalCorrection](TargetCamera.md#applyverticalcorrection)

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

#### Overrides

[TargetCamera](TargetCamera.md).[attachControl](TargetCamera.md#attachcontrol)

#### Defined in

packages/dev/core/src/Cameras/flyCamera.ts:280

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

[TargetCamera](TargetCamera.md).[attachPostProcess](TargetCamera.md#attachpostprocess)

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

[TargetCamera](TargetCamera.md).[beginAnimation](TargetCamera.md#beginanimation)

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

#### Inherited from

[TargetCamera](TargetCamera.md).[clone](TargetCamera.md#clone)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:1349

___

### computeWorldMatrix

▸ **computeWorldMatrix**(): [`Matrix`](Matrix.md)

Compute the world  matrix of the camera.

#### Returns

[`Matrix`](Matrix.md)

the camera world matrix

#### Inherited from

[TargetCamera](TargetCamera.md).[computeWorldMatrix](TargetCamera.md#computeworldmatrix)

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

[TargetCamera](TargetCamera.md).[createAnimationRange](TargetCamera.md#createanimationrange)

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

[TargetCamera](TargetCamera.md).[deleteAnimationRange](TargetCamera.md#deleteanimationrange)

#### Defined in

packages/dev/core/src/node.ts:794

___

### detachControl

▸ **detachControl**(): `void`

Detach a control from the HTML DOM element.
The camera will stop reacting to that input.

#### Returns

`void`

#### Overrides

[TargetCamera](TargetCamera.md).[detachControl](TargetCamera.md#detachcontrol)

#### Defined in

packages/dev/core/src/Cameras/flyCamera.ts:296

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

[TargetCamera](TargetCamera.md).[detachPostProcess](TargetCamera.md#detachpostprocess)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:776

___

### dispose

▸ **dispose**(): `void`

Destroy the camera and release the current resources held by it.

#### Returns

`void`

#### Overrides

[TargetCamera](TargetCamera.md).[dispose](TargetCamera.md#dispose)

#### Defined in

packages/dev/core/src/Cameras/flyCamera.ts:431

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

[TargetCamera](TargetCamera.md).[freezeProjectionMatrix](TargetCamera.md#freezeprojectionmatrix)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:848

___

### getActiveMeshes

▸ **getActiveMeshes**(): [`SmartArray`](SmartArray.md)[`AbstractMesh`](AbstractMesh.md)

Gets the list of active meshes this frame (meshes no culled or excluded by lod s in the frame)

#### Returns

[`SmartArray`](SmartArray.md)[`AbstractMesh`](AbstractMesh.md)

the active meshe list

#### Inherited from

[TargetCamera](TargetCamera.md).[getActiveMeshes](TargetCamera.md#getactivemeshes)

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

[TargetCamera](TargetCamera.md).[getAnimationByName](TargetCamera.md#getanimationbyname)

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

[TargetCamera](TargetCamera.md).[getAnimationRange](TargetCamera.md#getanimationrange)

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

[TargetCamera](TargetCamera.md).[getAnimationRanges](TargetCamera.md#getanimationranges)

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

[TargetCamera](TargetCamera.md).[getBehaviorByName](TargetCamera.md#getbehaviorbyname)

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

[TargetCamera](TargetCamera.md).[getChildMeshes](TargetCamera.md#getchildmeshes)

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

[TargetCamera](TargetCamera.md).[getChildMeshes](TargetCamera.md#getchildmeshes)

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

[TargetCamera](TargetCamera.md).[getChildren](TargetCamera.md#getchildren)

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

[TargetCamera](TargetCamera.md).[getChildren](TargetCamera.md#getchildren)

#### Defined in

packages/dev/core/src/node.ts:722

___

### getClassName

▸ **getClassName**(): `string`

Get the current object class name.

#### Returns

`string`

the class name.

#### Overrides

[TargetCamera](TargetCamera.md).[getClassName](TargetCamera.md#getclassname)

#### Defined in

packages/dev/core/src/Cameras/flyCamera.ts:440

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

[TargetCamera](TargetCamera.md).[getDescendants](TargetCamera.md#getdescendants)

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

[TargetCamera](TargetCamera.md).[getDescendants](TargetCamera.md#getdescendants)

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

#### Inherited from

[TargetCamera](TargetCamera.md).[getDirection](TargetCamera.md#getdirection)

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

#### Inherited from

[TargetCamera](TargetCamera.md).[getDirectionToRef](TargetCamera.md#getdirectiontoref)

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

[TargetCamera](TargetCamera.md).[getEngine](TargetCamera.md#getengine)

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

#### Inherited from

[TargetCamera](TargetCamera.md).[getForwardRay](TargetCamera.md#getforwardray)

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

#### Inherited from

[TargetCamera](TargetCamera.md).[getForwardRayToRef](TargetCamera.md#getforwardraytoref)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:1041

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

#### Inherited from

[TargetCamera](TargetCamera.md).[getFrontPosition](TargetCamera.md#getfrontposition)

#### Defined in

packages/dev/core/src/Cameras/targetCamera.ts:121

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

[TargetCamera](TargetCamera.md).[getHierarchyBoundingVectors](TargetCamera.md#gethierarchyboundingvectors)

#### Defined in

packages/dev/core/src/node.ts:933

___

### getLeftTarget

▸ **getLeftTarget**(): [`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md)

Gets the left camera target of a rig setup in case of Rigged Camera

#### Returns

[`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md)

the target position

#### Inherited from

[TargetCamera](TargetCamera.md).[getLeftTarget](TargetCamera.md#getlefttarget)

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

#### Inherited from

[TargetCamera](TargetCamera.md).[getProjectionMatrix](TargetCamera.md#getprojectionmatrix)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:867

___

### getRightTarget

▸ **getRightTarget**(): [`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md)

Gets the right camera target of a rig setup in case of Rigged Camera

#### Returns

[`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md)

the target position

#### Inherited from

[TargetCamera](TargetCamera.md).[getRightTarget](TargetCamera.md#getrighttarget)

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

[TargetCamera](TargetCamera.md).[getScene](TargetCamera.md#getscene)

#### Defined in

packages/dev/core/src/node.ts:344

___

### getTarget

▸ **getTarget**(): [`Vector3`](Vector3.md)

Return the current target position of the camera. This value is expressed in local space.

#### Returns

[`Vector3`](Vector3.md)

the target position

#### Inherited from

[TargetCamera](TargetCamera.md).[getTarget](TargetCamera.md#gettarget)

#### Defined in

packages/dev/core/src/Cameras/targetCamera.ts:303

___

### getTransformationMatrix

▸ **getTransformationMatrix**(): [`Matrix`](Matrix.md)

Gets the transformation matrix (ie. the multiplication of view by projection matrices)

#### Returns

[`Matrix`](Matrix.md)

a Matrix

#### Inherited from

[TargetCamera](TargetCamera.md).[getTransformationMatrix](TargetCamera.md#gettransformationmatrix)

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

#### Inherited from

[TargetCamera](TargetCamera.md).[getViewMatrix](TargetCamera.md#getviewmatrix)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:814

___

### getWorldMatrix

▸ **getWorldMatrix**(): [`Matrix`](Matrix.md)

Gets the current world matrix of the camera

#### Returns

[`Matrix`](Matrix.md)

#### Inherited from

[TargetCamera](TargetCamera.md).[getWorldMatrix](TargetCamera.md#getworldmatrix)

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

#### Inherited from

[TargetCamera](TargetCamera.md).[isActiveMesh](TargetCamera.md#isactivemesh)

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

#### Inherited from

[TargetCamera](TargetCamera.md).[isCompletelyInFrustum](TargetCamera.md#iscompletelyinfrustum)

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

[TargetCamera](TargetCamera.md).[isDescendantOf](TargetCamera.md#isdescendantof)

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

[TargetCamera](TargetCamera.md).[isDisposed](TargetCamera.md#isdisposed)

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

[TargetCamera](TargetCamera.md).[isEnabled](TargetCamera.md#isenabled)

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

#### Inherited from

[TargetCamera](TargetCamera.md).[isInFrustum](TargetCamera.md#isinfrustum)

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

#### Inherited from

[TargetCamera](TargetCamera.md).[isReady](TargetCamera.md#isready)

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

[TargetCamera](TargetCamera.md).[markAsDirty](TargetCamera.md#markasdirty)

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

[TargetCamera](TargetCamera.md).[removeBehavior](TargetCamera.md#removebehavior)

#### Defined in

packages/dev/core/src/node.ts:393

___

### restoreState

▸ **restoreState**(): `boolean`

Restored camera state. You must call storeState() first.

#### Returns

`boolean`

true if restored and false otherwise

#### Inherited from

[TargetCamera](TargetCamera.md).[restoreState](TargetCamera.md#restorestate)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:474

___

### serialize

▸ **serialize**(): `any`

Serialiaze the camera setup to a json representation

#### Returns

`any`

the JSON representation

#### Inherited from

[TargetCamera](TargetCamera.md).[serialize](TargetCamera.md#serialize)

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

[TargetCamera](TargetCamera.md).[serializeAnimationRanges](TargetCamera.md#serializeanimationranges)

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

[TargetCamera](TargetCamera.md).[setEnabled](TargetCamera.md#setenabled)

#### Defined in

packages/dev/core/src/node.ts:596

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

#### Inherited from

[TargetCamera](TargetCamera.md).[setTarget](TargetCamera.md#settarget)

#### Defined in

packages/dev/core/src/Cameras/targetCamera.ts:245

___

### storeState

▸ **storeState**(): [`Camera`](Camera.md)

Store current camera state of the camera (fov, position, rotation, etc..)

#### Returns

[`Camera`](Camera.md)

the camera

#### Inherited from

[TargetCamera](TargetCamera.md).[storeState](TargetCamera.md#storestate)

#### Defined in

packages/dev/core/src/Cameras/targetCamera.ts:150

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

[TargetCamera](TargetCamera.md).[toString](TargetCamera.md#tostring)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:499

___

### unfreezeProjectionMatrix

▸ **unfreezeProjectionMatrix**(): `void`

Unfreeze the projection matrix if it has previously been freezed by freezeProjectionMatrix.

#### Returns

`void`

#### Inherited from

[TargetCamera](TargetCamera.md).[unfreezeProjectionMatrix](TargetCamera.md#unfreezeprojectionmatrix)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:858

___

### update

▸ **update**(): `void`

Update the camera state according to the different inputs gathered during the frame.

#### Returns

`void`

#### Inherited from

[TargetCamera](TargetCamera.md).[update](TargetCamera.md#update)

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

[TargetCamera](TargetCamera.md).[AddNodeConstructor](TargetCamera.md#addnodeconstructor)

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

[TargetCamera](TargetCamera.md).[Construct](TargetCamera.md#construct)

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

#### Inherited from

[TargetCamera](TargetCamera.md).[GetConstructorFromName](TargetCamera.md#getconstructorfromname)

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

#### Inherited from

[TargetCamera](TargetCamera.md).[Parse](TargetCamera.md#parse)

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

[TargetCamera](TargetCamera.md).[ParseAnimationRanges](TargetCamera.md#parseanimationranges)

#### Defined in

packages/dev/core/src/node.ts:919
