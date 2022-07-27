[@dev/core](../README.md) / [Exports](../modules.md) / StereoscopicArcRotateCamera

# Class: StereoscopicArcRotateCamera

Camera used to simulate stereoscopic rendering (based on ArcRotateCamera)

**`See`**

https://doc.babylonjs.com/features/cameras

## Hierarchy

- [`ArcRotateCamera`](ArcRotateCamera.md)

  ↳ **`StereoscopicArcRotateCamera`**

## Table of contents

### Constructors

- [constructor](StereoscopicArcRotateCamera.md#constructor)

### Properties

- [\_collider](StereoscopicArcRotateCamera.md#_collider)
- [\_collisionTriggered](StereoscopicArcRotateCamera.md#_collisiontriggered)
- [\_collisionVelocity](StereoscopicArcRotateCamera.md#_collisionvelocity)
- [\_globalPosition](StereoscopicArcRotateCamera.md#_globalposition)
- [\_isDirty](StereoscopicArcRotateCamera.md#_isdirty)
- [\_newPosition](StereoscopicArcRotateCamera.md#_newposition)
- [\_parentNode](StereoscopicArcRotateCamera.md#_parentnode)
- [\_previousAlpha](StereoscopicArcRotateCamera.md#_previousalpha)
- [\_previousBeta](StereoscopicArcRotateCamera.md#_previousbeta)
- [\_previousPosition](StereoscopicArcRotateCamera.md#_previousposition)
- [\_previousRadius](StereoscopicArcRotateCamera.md#_previousradius)
- [\_ranges](StereoscopicArcRotateCamera.md#_ranges)
- [\_setRigMode](StereoscopicArcRotateCamera.md#_setrigmode)
- [\_target](StereoscopicArcRotateCamera.md#_target)
- [\_targetBoundingCenter](StereoscopicArcRotateCamera.md#_targetboundingcenter)
- [\_targetHost](StereoscopicArcRotateCamera.md#_targethost)
- [\_transformedDirection](StereoscopicArcRotateCamera.md#_transformeddirection)
- [\_upToYMatrix](StereoscopicArcRotateCamera.md#_uptoymatrix)
- [\_upVector](StereoscopicArcRotateCamera.md#_upvector)
- [\_webvrViewMatrix](StereoscopicArcRotateCamera.md#_webvrviewmatrix)
- [\_yToUpMatrix](StereoscopicArcRotateCamera.md#_ytoupmatrix)
- [allowUpsideDown](StereoscopicArcRotateCamera.md#allowupsidedown)
- [alpha](StereoscopicArcRotateCamera.md#alpha)
- [animations](StereoscopicArcRotateCamera.md#animations)
- [beta](StereoscopicArcRotateCamera.md#beta)
- [cameraDirection](StereoscopicArcRotateCamera.md#cameradirection)
- [cameraRigMode](StereoscopicArcRotateCamera.md#camerarigmode)
- [cameraRotation](StereoscopicArcRotateCamera.md#camerarotation)
- [checkCollisions](StereoscopicArcRotateCamera.md#checkcollisions)
- [collisionRadius](StereoscopicArcRotateCamera.md#collisionradius)
- [customRenderTargets](StereoscopicArcRotateCamera.md#customrendertargets)
- [fov](StereoscopicArcRotateCamera.md#fov)
- [fovMode](StereoscopicArcRotateCamera.md#fovmode)
- [id](StereoscopicArcRotateCamera.md#id)
- [ignoreParentScaling](StereoscopicArcRotateCamera.md#ignoreparentscaling)
- [inertia](StereoscopicArcRotateCamera.md#inertia)
- [inertialAlphaOffset](StereoscopicArcRotateCamera.md#inertialalphaoffset)
- [inertialBetaOffset](StereoscopicArcRotateCamera.md#inertialbetaoffset)
- [inertialPanningX](StereoscopicArcRotateCamera.md#inertialpanningx)
- [inertialPanningY](StereoscopicArcRotateCamera.md#inertialpanningy)
- [inertialRadiusOffset](StereoscopicArcRotateCamera.md#inertialradiusoffset)
- [inputs](StereoscopicArcRotateCamera.md#inputs)
- [inspectableCustomProperties](StereoscopicArcRotateCamera.md#inspectablecustomproperties)
- [interaxialDistance](StereoscopicArcRotateCamera.md#interaxialdistance)
- [inverseRotationSpeed](StereoscopicArcRotateCamera.md#inverserotationspeed)
- [invertRotation](StereoscopicArcRotateCamera.md#invertrotation)
- [isIntermediate](StereoscopicArcRotateCamera.md#isintermediate)
- [isRigCamera](StereoscopicArcRotateCamera.md#isrigcamera)
- [isStereoscopicSideBySide](StereoscopicArcRotateCamera.md#isstereoscopicsidebyside)
- [layerMask](StereoscopicArcRotateCamera.md#layermask)
- [lockedTarget](StereoscopicArcRotateCamera.md#lockedtarget)
- [lowerAlphaLimit](StereoscopicArcRotateCamera.md#loweralphalimit)
- [lowerBetaLimit](StereoscopicArcRotateCamera.md#lowerbetalimit)
- [lowerRadiusLimit](StereoscopicArcRotateCamera.md#lowerradiuslimit)
- [mapPanning](StereoscopicArcRotateCamera.md#mappanning)
- [maxZ](StereoscopicArcRotateCamera.md#maxz)
- [metadata](StereoscopicArcRotateCamera.md#metadata)
- [minZ](StereoscopicArcRotateCamera.md#minz)
- [name](StereoscopicArcRotateCamera.md#name)
- [noRotationConstraint](StereoscopicArcRotateCamera.md#norotationconstraint)
- [onAfterCheckInputsObservable](StereoscopicArcRotateCamera.md#onaftercheckinputsobservable)
- [onCollide](StereoscopicArcRotateCamera.md#oncollide)
- [onDisposeObservable](StereoscopicArcRotateCamera.md#ondisposeobservable)
- [onMeshTargetChangedObservable](StereoscopicArcRotateCamera.md#onmeshtargetchangedobservable)
- [onProjectionMatrixChangedObservable](StereoscopicArcRotateCamera.md#onprojectionmatrixchangedobservable)
- [onReady](StereoscopicArcRotateCamera.md#onready)
- [onRestoreStateObservable](StereoscopicArcRotateCamera.md#onrestorestateobservable)
- [onViewMatrixChangedObservable](StereoscopicArcRotateCamera.md#onviewmatrixchangedobservable)
- [outputRenderTarget](StereoscopicArcRotateCamera.md#outputrendertarget)
- [overrideCloneAlphaBetaRadius](StereoscopicArcRotateCamera.md#overrideclonealphabetaradius)
- [panningAxis](StereoscopicArcRotateCamera.md#panningaxis)
- [panningDistanceLimit](StereoscopicArcRotateCamera.md#panningdistancelimit)
- [panningInertia](StereoscopicArcRotateCamera.md#panninginertia)
- [panningOriginTarget](StereoscopicArcRotateCamera.md#panningorigintarget)
- [pinchToPanMaxDistance](StereoscopicArcRotateCamera.md#pinchtopanmaxdistance)
- [projectionPlaneTilt](StereoscopicArcRotateCamera.md#projectionplanetilt)
- [radius](StereoscopicArcRotateCamera.md#radius)
- [renderPassId](StereoscopicArcRotateCamera.md#renderpassid)
- [reservedDataStore](StereoscopicArcRotateCamera.md#reserveddatastore)
- [rigParent](StereoscopicArcRotateCamera.md#rigparent)
- [rotation](StereoscopicArcRotateCamera.md#rotation)
- [rotationQuaternion](StereoscopicArcRotateCamera.md#rotationquaternion)
- [speed](StereoscopicArcRotateCamera.md#speed)
- [state](StereoscopicArcRotateCamera.md#state)
- [targetScreenOffset](StereoscopicArcRotateCamera.md#targetscreenoffset)
- [uniqueId](StereoscopicArcRotateCamera.md#uniqueid)
- [updateUpVectorFromRotation](StereoscopicArcRotateCamera.md#updateupvectorfromrotation)
- [upperAlphaLimit](StereoscopicArcRotateCamera.md#upperalphalimit)
- [upperBetaLimit](StereoscopicArcRotateCamera.md#upperbetalimit)
- [upperRadiusLimit](StereoscopicArcRotateCamera.md#upperradiuslimit)
- [useInputToRestoreState](StereoscopicArcRotateCamera.md#useinputtorestorestate)
- [viewport](StereoscopicArcRotateCamera.md#viewport)
- [zoomOnFactor](StereoscopicArcRotateCamera.md#zoomonfactor)
- [FOVMODE\_HORIZONTAL\_FIXED](StereoscopicArcRotateCamera.md#fovmode_horizontal_fixed)
- [FOVMODE\_VERTICAL\_FIXED](StereoscopicArcRotateCamera.md#fovmode_vertical_fixed)
- [ForceAttachControlToAlwaysPreventDefault](StereoscopicArcRotateCamera.md#forceattachcontroltoalwayspreventdefault)
- [ORTHOGRAPHIC\_CAMERA](StereoscopicArcRotateCamera.md#orthographic_camera)
- [PERSPECTIVE\_CAMERA](StereoscopicArcRotateCamera.md#perspective_camera)
- [RIG\_MODE\_CUSTOM](StereoscopicArcRotateCamera.md#rig_mode_custom)
- [RIG\_MODE\_NONE](StereoscopicArcRotateCamera.md#rig_mode_none)
- [RIG\_MODE\_STEREOSCOPIC\_ANAGLYPH](StereoscopicArcRotateCamera.md#rig_mode_stereoscopic_anaglyph)
- [RIG\_MODE\_STEREOSCOPIC\_INTERLACED](StereoscopicArcRotateCamera.md#rig_mode_stereoscopic_interlaced)
- [RIG\_MODE\_STEREOSCOPIC\_OVERUNDER](StereoscopicArcRotateCamera.md#rig_mode_stereoscopic_overunder)
- [RIG\_MODE\_STEREOSCOPIC\_SIDEBYSIDE\_CROSSEYED](StereoscopicArcRotateCamera.md#rig_mode_stereoscopic_sidebyside_crosseyed)
- [RIG\_MODE\_STEREOSCOPIC\_SIDEBYSIDE\_PARALLEL](StereoscopicArcRotateCamera.md#rig_mode_stereoscopic_sidebyside_parallel)
- [RIG\_MODE\_VR](StereoscopicArcRotateCamera.md#rig_mode_vr)
- [RIG\_MODE\_WEBVR](StereoscopicArcRotateCamera.md#rig_mode_webvr)

### Accessors

- [absoluteRotation](StereoscopicArcRotateCamera.md#absoluterotation)
- [angularSensibilityX](StereoscopicArcRotateCamera.md#angularsensibilityx)
- [angularSensibilityY](StereoscopicArcRotateCamera.md#angularsensibilityy)
- [animationPropertiesOverride](StereoscopicArcRotateCamera.md#animationpropertiesoverride)
- [autoRotationBehavior](StereoscopicArcRotateCamera.md#autorotationbehavior)
- [behaviors](StereoscopicArcRotateCamera.md#behaviors)
- [bouncingBehavior](StereoscopicArcRotateCamera.md#bouncingbehavior)
- [doNotSerialize](StereoscopicArcRotateCamera.md#donotserialize)
- [framingBehavior](StereoscopicArcRotateCamera.md#framingbehavior)
- [globalPosition](StereoscopicArcRotateCamera.md#globalposition)
- [isLeftCamera](StereoscopicArcRotateCamera.md#isleftcamera)
- [isRightCamera](StereoscopicArcRotateCamera.md#isrightcamera)
- [keysDown](StereoscopicArcRotateCamera.md#keysdown)
- [keysLeft](StereoscopicArcRotateCamera.md#keysleft)
- [keysRight](StereoscopicArcRotateCamera.md#keysright)
- [keysUp](StereoscopicArcRotateCamera.md#keysup)
- [leftCamera](StereoscopicArcRotateCamera.md#leftcamera)
- [mode](StereoscopicArcRotateCamera.md#mode)
- [onClonedObservable](StereoscopicArcRotateCamera.md#onclonedobservable)
- [onDispose](StereoscopicArcRotateCamera.md#ondispose)
- [onEnabledStateChangedObservable](StereoscopicArcRotateCamera.md#onenabledstatechangedobservable)
- [orthoBottom](StereoscopicArcRotateCamera.md#orthobottom)
- [orthoLeft](StereoscopicArcRotateCamera.md#ortholeft)
- [orthoRight](StereoscopicArcRotateCamera.md#orthoright)
- [orthoTop](StereoscopicArcRotateCamera.md#orthotop)
- [panningSensibility](StereoscopicArcRotateCamera.md#panningsensibility)
- [parent](StereoscopicArcRotateCamera.md#parent)
- [pinchDeltaPercentage](StereoscopicArcRotateCamera.md#pinchdeltapercentage)
- [pinchPrecision](StereoscopicArcRotateCamera.md#pinchprecision)
- [position](StereoscopicArcRotateCamera.md#position)
- [rigPostProcess](StereoscopicArcRotateCamera.md#rigpostprocess)
- [rightCamera](StereoscopicArcRotateCamera.md#rightcamera)
- [screenArea](StereoscopicArcRotateCamera.md#screenarea)
- [target](StereoscopicArcRotateCamera.md#target)
- [targetHost](StereoscopicArcRotateCamera.md#targethost)
- [upVector](StereoscopicArcRotateCamera.md#upvector)
- [useAutoRotationBehavior](StereoscopicArcRotateCamera.md#useautorotationbehavior)
- [useBouncingBehavior](StereoscopicArcRotateCamera.md#usebouncingbehavior)
- [useFramingBehavior](StereoscopicArcRotateCamera.md#useframingbehavior)
- [useNaturalPinchZoom](StereoscopicArcRotateCamera.md#usenaturalpinchzoom)
- [wheelDeltaPercentage](StereoscopicArcRotateCamera.md#wheeldeltapercentage)
- [wheelPrecision](StereoscopicArcRotateCamera.md#wheelprecision)
- [worldMatrixFromCache](StereoscopicArcRotateCamera.md#worldmatrixfromcache)
- [zoomToMouseLocation](StereoscopicArcRotateCamera.md#zoomtomouselocation)

### Methods

- [\_checkLimits](StereoscopicArcRotateCamera.md#_checklimits)
- [\_computeViewMatrix](StereoscopicArcRotateCamera.md#_computeviewmatrix)
- [\_getFirstPostProcess](StereoscopicArcRotateCamera.md#_getfirstpostprocess)
- [\_getTargetPosition](StereoscopicArcRotateCamera.md#_gettargetposition)
- [\_onCollisionPositionChange](StereoscopicArcRotateCamera.md#_oncollisionpositionchange)
- [\_updateCameraRotationMatrix](StereoscopicArcRotateCamera.md#_updatecamerarotationmatrix)
- [\_updateWebVRCameraRotationMatrix](StereoscopicArcRotateCamera.md#_updatewebvrcamerarotationmatrix)
- [addBehavior](StereoscopicArcRotateCamera.md#addbehavior)
- [applyVerticalCorrection](StereoscopicArcRotateCamera.md#applyverticalcorrection)
- [attachControl](StereoscopicArcRotateCamera.md#attachcontrol)
- [attachPostProcess](StereoscopicArcRotateCamera.md#attachpostprocess)
- [beginAnimation](StereoscopicArcRotateCamera.md#beginanimation)
- [clone](StereoscopicArcRotateCamera.md#clone)
- [computeWorldMatrix](StereoscopicArcRotateCamera.md#computeworldmatrix)
- [createAnimationRange](StereoscopicArcRotateCamera.md#createanimationrange)
- [createRigCamera](StereoscopicArcRotateCamera.md#createrigcamera)
- [deleteAnimationRange](StereoscopicArcRotateCamera.md#deleteanimationrange)
- [detachControl](StereoscopicArcRotateCamera.md#detachcontrol)
- [detachPostProcess](StereoscopicArcRotateCamera.md#detachpostprocess)
- [dispose](StereoscopicArcRotateCamera.md#dispose)
- [focusOn](StereoscopicArcRotateCamera.md#focuson)
- [freezeProjectionMatrix](StereoscopicArcRotateCamera.md#freezeprojectionmatrix)
- [getActiveMeshes](StereoscopicArcRotateCamera.md#getactivemeshes)
- [getAnimationByName](StereoscopicArcRotateCamera.md#getanimationbyname)
- [getAnimationRange](StereoscopicArcRotateCamera.md#getanimationrange)
- [getAnimationRanges](StereoscopicArcRotateCamera.md#getanimationranges)
- [getBehaviorByName](StereoscopicArcRotateCamera.md#getbehaviorbyname)
- [getChildMeshes](StereoscopicArcRotateCamera.md#getchildmeshes)
- [getChildren](StereoscopicArcRotateCamera.md#getchildren)
- [getClassName](StereoscopicArcRotateCamera.md#getclassname)
- [getDescendants](StereoscopicArcRotateCamera.md#getdescendants)
- [getDirection](StereoscopicArcRotateCamera.md#getdirection)
- [getDirectionToRef](StereoscopicArcRotateCamera.md#getdirectiontoref)
- [getEngine](StereoscopicArcRotateCamera.md#getengine)
- [getForwardRay](StereoscopicArcRotateCamera.md#getforwardray)
- [getForwardRayToRef](StereoscopicArcRotateCamera.md#getforwardraytoref)
- [getFrontPosition](StereoscopicArcRotateCamera.md#getfrontposition)
- [getHierarchyBoundingVectors](StereoscopicArcRotateCamera.md#gethierarchyboundingvectors)
- [getLeftTarget](StereoscopicArcRotateCamera.md#getlefttarget)
- [getProjectionMatrix](StereoscopicArcRotateCamera.md#getprojectionmatrix)
- [getRightTarget](StereoscopicArcRotateCamera.md#getrighttarget)
- [getScene](StereoscopicArcRotateCamera.md#getscene)
- [getTarget](StereoscopicArcRotateCamera.md#gettarget)
- [getTransformationMatrix](StereoscopicArcRotateCamera.md#gettransformationmatrix)
- [getViewMatrix](StereoscopicArcRotateCamera.md#getviewmatrix)
- [getWorldMatrix](StereoscopicArcRotateCamera.md#getworldmatrix)
- [isActiveMesh](StereoscopicArcRotateCamera.md#isactivemesh)
- [isCompletelyInFrustum](StereoscopicArcRotateCamera.md#iscompletelyinfrustum)
- [isDescendantOf](StereoscopicArcRotateCamera.md#isdescendantof)
- [isDisposed](StereoscopicArcRotateCamera.md#isdisposed)
- [isEnabled](StereoscopicArcRotateCamera.md#isenabled)
- [isInFrustum](StereoscopicArcRotateCamera.md#isinfrustum)
- [isReady](StereoscopicArcRotateCamera.md#isready)
- [markAsDirty](StereoscopicArcRotateCamera.md#markasdirty)
- [rebuildAnglesAndRadius](StereoscopicArcRotateCamera.md#rebuildanglesandradius)
- [removeBehavior](StereoscopicArcRotateCamera.md#removebehavior)
- [restoreState](StereoscopicArcRotateCamera.md#restorestate)
- [serialize](StereoscopicArcRotateCamera.md#serialize)
- [serializeAnimationRanges](StereoscopicArcRotateCamera.md#serializeanimationranges)
- [setEnabled](StereoscopicArcRotateCamera.md#setenabled)
- [setMatUp](StereoscopicArcRotateCamera.md#setmatup)
- [setPosition](StereoscopicArcRotateCamera.md#setposition)
- [setTarget](StereoscopicArcRotateCamera.md#settarget)
- [storeState](StereoscopicArcRotateCamera.md#storestate)
- [toString](StereoscopicArcRotateCamera.md#tostring)
- [unfreezeProjectionMatrix](StereoscopicArcRotateCamera.md#unfreezeprojectionmatrix)
- [update](StereoscopicArcRotateCamera.md#update)
- [zoomOn](StereoscopicArcRotateCamera.md#zoomon)
- [AddNodeConstructor](StereoscopicArcRotateCamera.md#addnodeconstructor)
- [Construct](StereoscopicArcRotateCamera.md#construct)
- [GetConstructorFromName](StereoscopicArcRotateCamera.md#getconstructorfromname)
- [Parse](StereoscopicArcRotateCamera.md#parse)
- [ParseAnimationRanges](StereoscopicArcRotateCamera.md#parseanimationranges)

## Constructors

### constructor

• **new StereoscopicArcRotateCamera**(`name`, `alpha`, `beta`, `radius`, `target`, `interaxialDistance`, `isStereoscopicSideBySide`, `scene?`)

Creates a new StereoscopicArcRotateCamera

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines camera name |
| `alpha` | `number` | defines alpha angle (in radians) |
| `beta` | `number` | defines beta angle (in radians) |
| `radius` | `number` | defines radius |
| `target` | [`Vector3`](Vector3.md) | defines camera target |
| `interaxialDistance` | `number` | defines distance between each color axis |
| `isStereoscopicSideBySide` | `boolean` | defines is stereoscopic is done side by side or over under |
| `scene?` | [`Scene`](Scene.md) | defines the hosting scene |

#### Overrides

[ArcRotateCamera](ArcRotateCamera.md).[constructor](ArcRotateCamera.md#constructor)

#### Defined in

packages/dev/core/src/Cameras/Stereoscopic/stereoscopicArcRotateCamera.ts:28

## Properties

### \_collider

• `Protected` **\_collider**: `Collider`

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[_collider](ArcRotateCamera.md#_collider)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:680

___

### \_collisionTriggered

• `Protected` **\_collisionTriggered**: `boolean`

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[_collisionTriggered](ArcRotateCamera.md#_collisiontriggered)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:688

___

### \_collisionVelocity

• `Protected` **\_collisionVelocity**: [`Vector3`](Vector3.md)

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[_collisionVelocity](ArcRotateCamera.md#_collisionvelocity)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:682

___

### \_globalPosition

• `Protected` **\_globalPosition**: [`Vector3`](Vector3.md)

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[_globalPosition](ArcRotateCamera.md#_globalposition)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:412

___

### \_isDirty

• `Protected` **\_isDirty**: `boolean` = `false`

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[_isDirty](ArcRotateCamera.md#_isdirty)

#### Defined in

packages/dev/core/src/node.ts:43

___

### \_newPosition

• `Protected` **\_newPosition**: [`Vector3`](Vector3.md)

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[_newPosition](ArcRotateCamera.md#_newposition)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:683

___

### \_parentNode

• `Protected` **\_parentNode**: [`Nullable`](../modules.md#nullable)[`Node`](Node.md) = `null`

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[_parentNode](ArcRotateCamera.md#_parentnode)

#### Defined in

packages/dev/core/src/node.ts:176

___

### \_previousAlpha

• `Protected` **\_previousAlpha**: `number`

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[_previousAlpha](ArcRotateCamera.md#_previousalpha)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:684

___

### \_previousBeta

• `Protected` **\_previousBeta**: `number`

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[_previousBeta](ArcRotateCamera.md#_previousbeta)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:685

___

### \_previousPosition

• `Protected` **\_previousPosition**: [`Vector3`](Vector3.md)

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[_previousPosition](ArcRotateCamera.md#_previousposition)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:681

___

### \_previousRadius

• `Protected` **\_previousRadius**: `number`

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[_previousRadius](ArcRotateCamera.md#_previousradius)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:686

___

### \_ranges

• `Protected` **\_ranges**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: [`Nullable`](../modules.md#nullable)`AnimationRange`

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[_ranges](ArcRotateCamera.md#_ranges)

#### Defined in

packages/dev/core/src/node.ts:154

___

### \_setRigMode

• `Protected` **\_setRigMode**: `any`

#### Overrides

[ArcRotateCamera](ArcRotateCamera.md).[_setRigMode](ArcRotateCamera.md#_setrigmode)

#### Defined in

packages/dev/core/src/Cameras/Stereoscopic/stereoscopicArcRotateCamera.ts:45

___

### \_target

• `Protected` **\_target**: [`Vector3`](Vector3.md)

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[_target](ArcRotateCamera.md#_target)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:61

___

### \_targetBoundingCenter

• `Protected` **\_targetBoundingCenter**: [`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md)

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[_targetBoundingCenter](ArcRotateCamera.md#_targetboundingcenter)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:690

___

### \_targetHost

• `Protected` **\_targetHost**: [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[_targetHost](ArcRotateCamera.md#_targethost)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:63

___

### \_transformedDirection

• `Protected` **\_transformedDirection**: [`Vector3`](Vector3.md)

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[_transformedDirection](ArcRotateCamera.md#_transformeddirection)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:553

___

### \_upToYMatrix

• `Protected` **\_upToYMatrix**: [`Matrix`](Matrix.md)

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[_upToYMatrix](ArcRotateCamera.md#_uptoymatrix)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:109

___

### \_upVector

• `Protected` **\_upVector**: [`Vector3`](Vector3.md)

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[_upVector](ArcRotateCamera.md#_upvector)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:129

___

### \_webvrViewMatrix

• `Protected` **\_webvrViewMatrix**: [`Matrix`](Matrix.md)

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[_webvrViewMatrix](ArcRotateCamera.md#_webvrviewmatrix)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:399

___

### \_yToUpMatrix

• `Protected` **\_yToUpMatrix**: [`Matrix`](Matrix.md)

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[_yToUpMatrix](ArcRotateCamera.md#_ytoupmatrix)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:110

___

### allowUpsideDown

• **allowUpsideDown**: `boolean` = `true`

Allows the camera to be completely reversed.
If false the camera can not arrive upside down.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[allowUpsideDown](ArcRotateCamera.md#allowupsidedown)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:526

___

### alpha

• **alpha**: `number`

Defines the rotation angle of the camera along the longitudinal axis.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[alpha](ArcRotateCamera.md#alpha)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:39

___

### animations

• **animations**: [`Animation`](Animation.md)[]

Gets a list of Animations associated with the node

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[animations](ArcRotateCamera.md#animations)

#### Defined in

packages/dev/core/src/node.ts:153

___

### beta

• **beta**: `number`

Defines the rotation angle of the camera along the latitudinal axis.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[beta](ArcRotateCamera.md#beta)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:45

___

### cameraDirection

• **cameraDirection**: [`Vector3`](Vector3.md)

Define the current direction the camera is moving to

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[cameraDirection](ArcRotateCamera.md#cameradirection)

#### Defined in

packages/dev/core/src/Cameras/targetCamera.ts:24

___

### cameraRigMode

• **cameraRigMode**: `number` = `Camera.RIG_MODE_NONE`

Rig mode of the camera.
This is useful to create the camera with two "eyes" instead of one to create VR or stereoscopic scenes.
This is normally controlled byt the camera themselves as internal use.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[cameraRigMode](ArcRotateCamera.md#camerarigmode)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:330

___

### cameraRotation

• **cameraRotation**: [`Vector2`](Vector2.md)

Define the current rotation the camera is rotating to

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[cameraRotation](ArcRotateCamera.md#camerarotation)

#### Defined in

packages/dev/core/src/Cameras/targetCamera.ts:28

___

### checkCollisions

• **checkCollisions**: `boolean` = `false`

Defines whether the camera should check collision with the objects oh the scene.

**`See`**

https://doc.babylonjs.com/babylon101/cameras,_mesh_collisions_and_gravity#how-can-i-do-this

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[checkCollisions](ArcRotateCamera.md#checkcollisions)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:671

___

### collisionRadius

• **collisionRadius**: [`Vector3`](Vector3.md)

Defines the collision radius of the camera.
This simulates a sphere around the camera.

**`See`**

https://doc.babylonjs.com/babylon101/cameras,_mesh_collisions_and_gravity#arcrotatecamera

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[collisionRadius](ArcRotateCamera.md#collisionradius)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:678

___

### customRenderTargets

• **customRenderTargets**: [`RenderTargetTexture`](RenderTargetTexture.md)[]

Defines the list of custom render target which are rendered to and then used as the input to this camera's render. Eg. display another camera view on a TV in the main scene
This is pretty helpful if you wish to make a camera render to a texture you could reuse somewhere
else in the scene. (Eg. security camera)

To change the final output target of the camera, camera.outputRenderTarget should be used instead (eg. webXR renders to a render target corresponding to an HMD)

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[customRenderTargets](ArcRotateCamera.md#customrendertargets)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:351

___

### fov

• **fov**: `number` = `0.8`

Field Of View is set in Radians. (default is 0.8)

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[fov](ArcRotateCamera.md#fov)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:248

___

### fovMode

• **fovMode**: `number` = `Camera.FOVMODE_VERTICAL_FIXED`

fovMode sets the camera frustum bounds to the viewport bounds. (default is FOVMODE_VERTICAL_FIXED)

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[fovMode](ArcRotateCamera.md#fovmode)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:322

___

### id

• **id**: `string`

Gets or sets the id of the node

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[id](ArcRotateCamera.md#id)

#### Defined in

packages/dev/core/src/node.ts:97

___

### ignoreParentScaling

• **ignoreParentScaling**: `boolean` = `false`

Gets or sets a boolean indicating that the scaling of the parent hierarchy will not be taken in account by the camera

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[ignoreParentScaling](ArcRotateCamera.md#ignoreparentscaling)

#### Defined in

packages/dev/core/src/Cameras/targetCamera.ts:31

___

### inertia

• **inertia**: `number` = `0.9`

Define the default inertia of the camera.
This helps giving a smooth feeling to the camera movement.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[inertia](ArcRotateCamera.md#inertia)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:279

___

### inertialAlphaOffset

• **inertialAlphaOffset**: `number` = `0`

Current inertia value on the longitudinal axis.
The bigger this number the longer it will take for the camera to stop.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[inertialAlphaOffset](ArcRotateCamera.md#inertialalphaoffset)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:150

___

### inertialBetaOffset

• **inertialBetaOffset**: `number` = `0`

Current inertia value on the latitudinal axis.
The bigger this number the longer it will take for the camera to stop.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[inertialBetaOffset](ArcRotateCamera.md#inertialbetaoffset)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:157

___

### inertialPanningX

• **inertialPanningX**: `number` = `0`

Defines the current inertia value used during panning of the camera along the X axis.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[inertialPanningX](ArcRotateCamera.md#inertialpanningx)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:212

___

### inertialPanningY

• **inertialPanningY**: `number` = `0`

Defines the current inertia value used during panning of the camera along the Y axis.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[inertialPanningY](ArcRotateCamera.md#inertialpanningy)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:218

___

### inertialRadiusOffset

• **inertialRadiusOffset**: `number` = `0`

Current inertia value on the radius axis.
The bigger this number the longer it will take for the camera to stop.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[inertialRadiusOffset](ArcRotateCamera.md#inertialradiusoffset)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:164

___

### inputs

• **inputs**: [`ArcRotateCameraInputsManager`](ArcRotateCameraInputsManager.md)

Defines the input associated to the camera.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[inputs](ArcRotateCamera.md#inputs)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:544

___

### inspectableCustomProperties

• **inspectableCustomProperties**: [`IInspectable`](../interfaces/IInspectable.md)[]

List of inspectable custom properties (used by the Inspector)

**`See`**

https://doc.babylonjs.com/how_to/debug_layer#extensibility

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[inspectableCustomProperties](ArcRotateCamera.md#inspectablecustomproperties)

#### Defined in

packages/dev/core/src/node.ts:126

___

### interaxialDistance

• **interaxialDistance**: `number`

Defines the distance between both "eyes" in case of a RIG

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[interaxialDistance](ArcRotateCamera.md#interaxialdistance)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:336

___

### inverseRotationSpeed

• **inverseRotationSpeed**: `number` = `0.2`

Speed multiplier for inverse camera panning

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[inverseRotationSpeed](ArcRotateCamera.md#inverserotationspeed)

#### Defined in

packages/dev/core/src/Cameras/targetCamera.ts:71

___

### invertRotation

• **invertRotation**: `boolean` = `false`

Reverses mouselook direction to 'natural' panning as opposed to traditional direct
panning

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[invertRotation](ArcRotateCamera.md#invertrotation)

#### Defined in

packages/dev/core/src/Cameras/targetCamera.ts:66

___

### isIntermediate

• **isIntermediate**: `boolean` = `false`

Define whether the camera is intermediate.
This is useful to not present the output directly to the screen in case of rig without post process for instance

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[isIntermediate](ArcRotateCamera.md#isintermediate)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:303

___

### isRigCamera

• **isRigCamera**: `boolean` = `false`

Is this camera a part of a rig system?

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[isRigCamera](ArcRotateCamera.md#isrigcamera)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:379

___

### isStereoscopicSideBySide

• **isStereoscopicSideBySide**: `boolean`

Defines if stereoscopic rendering is done side by side or over under.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[isStereoscopicSideBySide](ArcRotateCamera.md#isstereoscopicsidebyside)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:342

___

### layerMask

• **layerMask**: `number` = `0x0fffffff`

Restricts the camera to viewing objects with the same layerMask.
A camera with a layerMask of 1 will render mesh.layerMask & camera.layerMask!== 0

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[layerMask](ArcRotateCamera.md#layermask)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:316

___

### lockedTarget

• **lockedTarget**: `any` = `null`

Define the current target of the camera as an object or a position.
Please note that locking a target will disable panning.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[lockedTarget](ArcRotateCamera.md#lockedtarget)

#### Defined in

packages/dev/core/src/Cameras/targetCamera.ts:78

___

### lowerAlphaLimit

• **lowerAlphaLimit**: [`Nullable`](../modules.md#nullable)`number` = `null`

Minimum allowed angle on the longitudinal axis.
This can help limiting how the Camera is able to move in the scene.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[lowerAlphaLimit](ArcRotateCamera.md#loweralphalimit)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:171

___

### lowerBetaLimit

• **lowerBetaLimit**: `number` = `0.01`

Minimum allowed angle on the latitudinal axis.
This can help limiting how the Camera is able to move in the scene.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[lowerBetaLimit](ArcRotateCamera.md#lowerbetalimit)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:185

___

### lowerRadiusLimit

• **lowerRadiusLimit**: [`Nullable`](../modules.md#nullable)`number` = `null`

Minimum allowed distance of the camera to the target (The camera can not get closer).
This can help limiting how the Camera is able to move in the scene.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[lowerRadiusLimit](ArcRotateCamera.md#lowerradiuslimit)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:199

___

### mapPanning

• **mapPanning**: `boolean` = `false`

Defines if camera will eliminate transform on y axis.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[mapPanning](ArcRotateCamera.md#mappanning)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:558

___

### maxZ

• **maxZ**: `number` = `10000.0`

Define the maximum distance the camera can see to.
This is important to note that the depth buffer are not infinite and the further it end
the more your scene might encounter depth fighting issue.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[maxZ](ArcRotateCamera.md#maxz)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:272

___

### metadata

• **metadata**: `any` = `null`

Gets or sets an object used to store user defined information for the node

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[metadata](ArcRotateCamera.md#metadata)

#### Defined in

packages/dev/core/src/node.ts:115

___

### minZ

• **minZ**: `number` = `1`

Define the minimum distance the camera can see from.
This is important to note that the depth buffer are not infinite and the closer it starts
the more your scene might encounter depth fighting issue.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[minZ](ArcRotateCamera.md#minz)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:264

___

### name

• **name**: `string`

Gets or sets the name of the node

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[name](ArcRotateCamera.md#name)

#### Defined in

packages/dev/core/src/node.ts:91

___

### noRotationConstraint

• **noRotationConstraint**: `boolean` = `false`

Add constraint to the camera to prevent it to move freely in all directions and
around all axis.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[noRotationConstraint](ArcRotateCamera.md#norotationconstraint)

#### Defined in

packages/dev/core/src/Cameras/targetCamera.ts:60

___

### onAfterCheckInputsObservable

• **onAfterCheckInputsObservable**: [`Observable`](Observable.md)[`Camera`](Camera.md)

Observable triggered when the inputs have been processed.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[onAfterCheckInputsObservable](ArcRotateCamera.md#onaftercheckinputsobservable)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:370

___

### onCollide

• **onCollide**: (`collidedMesh`: [`AbstractMesh`](AbstractMesh.md)) => `void`

#### Type declaration

▸ (`collidedMesh`): `void`

Event raised when the camera is colliding with a mesh.

##### Parameters

| Name | Type |
| :------ | :------ |
| `collidedMesh` | [`AbstractMesh`](AbstractMesh.md) |

##### Returns

`void`

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[onCollide](ArcRotateCamera.md#oncollide)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:665

___

### onDisposeObservable

• **onDisposeObservable**: [`Observable`](Observable.md)[`Node`](Node.md)

An event triggered when the mesh is disposed

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[onDisposeObservable](ArcRotateCamera.md#ondisposeobservable)

#### Defined in

packages/dev/core/src/node.ts:300

___

### onMeshTargetChangedObservable

• **onMeshTargetChangedObservable**: [`Observable`](Observable.md)[`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

Observable triggered when the mesh target has been changed on the camera.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[onMeshTargetChangedObservable](ArcRotateCamera.md#onmeshtargetchangedobservable)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:660

___

### onProjectionMatrixChangedObservable

• **onProjectionMatrixChangedObservable**: [`Observable`](Observable.md)[`Camera`](Camera.md)

Observable triggered when the camera Projection matrix has changed.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[onProjectionMatrixChangedObservable](ArcRotateCamera.md#onprojectionmatrixchangedobservable)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:366

___

### onReady

• **onReady**: [`Nullable`](../modules.md#nullable)(`node`: [`Node`](Node.md)) => `void` = `null`

Callback raised when the node is ready to be used

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[onReady](ArcRotateCamera.md#onready)

#### Defined in

packages/dev/core/src/node.ts:159

___

### onRestoreStateObservable

• **onRestoreStateObservable**: [`Observable`](Observable.md)[`Camera`](Camera.md)

Observable triggered when reset has been called and applied to the camera.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[onRestoreStateObservable](ArcRotateCamera.md#onrestorestateobservable)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:374

___

### onViewMatrixChangedObservable

• **onViewMatrixChangedObservable**: [`Observable`](Observable.md)[`Camera`](Camera.md)

Observable triggered when the camera view matrix has changed.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[onViewMatrixChangedObservable](ArcRotateCamera.md#onviewmatrixchangedobservable)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:362

___

### outputRenderTarget

• **outputRenderTarget**: [`Nullable`](../modules.md#nullable)[`RenderTargetTexture`](RenderTargetTexture.md) = `null`

When set, the camera will render to this render target instead of the default canvas

If the desire is to use the output of a camera as a texture in the scene consider using camera.customRenderTargets instead

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[outputRenderTarget](ArcRotateCamera.md#outputrendertarget)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:357

___

### overrideCloneAlphaBetaRadius

• **overrideCloneAlphaBetaRadius**: [`Nullable`](../modules.md#nullable)`boolean`

Defines an override value to use as the parameter to setTarget.
This allows the parameter to be specified when animating the target (e.g. using FramingBehavior).

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[overrideCloneAlphaBetaRadius](ArcRotateCamera.md#overrideclonealphabetaradius)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:58

___

### panningAxis

• **panningAxis**: [`Vector3`](Vector3.md)

Defines the allowed panning axis.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[panningAxis](ArcRotateCamera.md#panningaxis)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:552

___

### panningDistanceLimit

• **panningDistanceLimit**: [`Nullable`](../modules.md#nullable)`number` = `null`

Defines the maximum distance the camera can pan.
This could help keeping the camera always in your scene.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[panningDistanceLimit](ArcRotateCamera.md#panningdistancelimit)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:233

___

### panningInertia

• **panningInertia**: `number` = `0.9`

Defines the value of the inertia used during panning.
0 would mean stop inertia and one would mean no deceleration at all.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[panningInertia](ArcRotateCamera.md#panninginertia)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:246

___

### panningOriginTarget

• **panningOriginTarget**: [`Vector3`](Vector3.md)

Defines the target of the camera before panning.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[panningOriginTarget](ArcRotateCamera.md#panningorigintarget)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:239

___

### pinchToPanMaxDistance

• **pinchToPanMaxDistance**: `number` = `20`

Defines the distance used to consider the camera in pan mode vs pinch/zoom.
Basically if your fingers moves away from more than this distance you will be considered
in pinch mode.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[pinchToPanMaxDistance](ArcRotateCamera.md#pinchtopanmaxdistance)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:226

___

### projectionPlaneTilt

• **projectionPlaneTilt**: `number` = `0`

Projection plane tilt around the X axis (horizontal), set in Radians. (default is 0)
Can be used to make vertical lines in world space actually vertical on the screen.
See https://forum.babylonjs.com/t/add-vertical-shift-to-3ds-max-exporter-babylon-cameras/17480

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[projectionPlaneTilt](ArcRotateCamera.md#projectionplanetilt)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:256

___

### radius

• **radius**: `number`

Defines the radius of the camera from it s target point.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[radius](ArcRotateCamera.md#radius)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:51

___

### renderPassId

• **renderPassId**: `number`

Render pass id used by the camera to render into the main framebuffer

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[renderPassId](ArcRotateCamera.md#renderpassid)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:390

___

### reservedDataStore

• **reservedDataStore**: `any` = `null`

For internal use only. Please do not use.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[reservedDataStore](ArcRotateCamera.md#reserveddatastore)

#### Defined in

packages/dev/core/src/node.ts:120

___

### rigParent

• `Optional` **rigParent**: [`Camera`](Camera.md)

If isRigCamera set to true this will be set with the parent camera.
The parent camera is not (!) necessarily the .parent of this camera (like in the case of XR)

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[rigParent](ArcRotateCamera.md#rigparent)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:385

___

### rotation

• **rotation**: [`Vector3`](Vector3.md)

Define the current rotation of the camera

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[rotation](ArcRotateCamera.md#rotation)

#### Defined in

packages/dev/core/src/Cameras/targetCamera.ts:43

___

### rotationQuaternion

• **rotationQuaternion**: [`Quaternion`](Quaternion.md)

Define the current rotation of the camera as a quaternion to prevent Gimbal lock

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[rotationQuaternion](ArcRotateCamera.md#rotationquaternion)

#### Defined in

packages/dev/core/src/Cameras/targetCamera.ts:48

___

### speed

• **speed**: `number` = `2.0`

Define the current speed of the camera

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[speed](ArcRotateCamera.md#speed)

#### Defined in

packages/dev/core/src/Cameras/targetCamera.ts:54

___

### state

• **state**: `string` = `""`

Gets or sets a string used to store user defined state for the node

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[state](ArcRotateCamera.md#state)

#### Defined in

packages/dev/core/src/node.ts:109

___

### targetScreenOffset

• **targetScreenOffset**: [`Vector2`](Vector2.md)

Defines a screen offset for the camera position.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[targetScreenOffset](ArcRotateCamera.md#targetscreenoffset)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:519

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the node

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[uniqueId](ArcRotateCamera.md#uniqueid)

#### Defined in

packages/dev/core/src/node.ts:103

___

### updateUpVectorFromRotation

• **updateUpVectorFromRotation**: `boolean` = `false`

When set, the up vector of the camera will be updated by the rotation of the camera

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[updateUpVectorFromRotation](ArcRotateCamera.md#updateupvectorfromrotation)

#### Defined in

packages/dev/core/src/Cameras/targetCamera.ts:36

___

### upperAlphaLimit

• **upperAlphaLimit**: [`Nullable`](../modules.md#nullable)`number` = `null`

Maximum allowed angle on the longitudinal axis.
This can help limiting how the Camera is able to move in the scene.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[upperAlphaLimit](ArcRotateCamera.md#upperalphalimit)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:178

___

### upperBetaLimit

• **upperBetaLimit**: `number`

Maximum allowed angle on the latitudinal axis.
This can help limiting how the Camera is able to move in the scene.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[upperBetaLimit](ArcRotateCamera.md#upperbetalimit)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:192

___

### upperRadiusLimit

• **upperRadiusLimit**: [`Nullable`](../modules.md#nullable)`number` = `null`

Maximum allowed distance of the camera to the target (The camera can not get further).
This can help limiting how the Camera is able to move in the scene.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[upperRadiusLimit](ArcRotateCamera.md#upperradiuslimit)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:206

___

### useInputToRestoreState

• **useInputToRestoreState**: `boolean` = `true`

Define if double tap/click is used to restore the previously saved state of the camera.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[useInputToRestoreState](ArcRotateCamera.md#useinputtorestorestate)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:532

___

### viewport

• **viewport**: [`Viewport`](Viewport.md)

Define the viewport of the camera.
This correspond to the portion of the screen the camera will render to in normalized 0 to 1 unit.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[viewport](ArcRotateCamera.md#viewport)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:309

___

### zoomOnFactor

• **zoomOnFactor**: `number` = `1`

Defines how much the radius should be scaled while zooming on a particular mesh (through the zoomOn function)

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[zoomOnFactor](ArcRotateCamera.md#zoomonfactor)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:513

___

### FOVMODE\_HORIZONTAL\_FIXED

▪ `Static` `Readonly` **FOVMODE\_HORIZONTAL\_FIXED**: ``1``

This setting aligns the left and right bounds of the viewport to the left and right bounds of the camera frustum.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[FOVMODE_HORIZONTAL_FIXED](ArcRotateCamera.md#fovmode_horizontal_fixed)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:62

___

### FOVMODE\_VERTICAL\_FIXED

▪ `Static` `Readonly` **FOVMODE\_VERTICAL\_FIXED**: ``0``

This is the default FOV mode for perspective cameras.
This setting aligns the upper and lower bounds of the viewport to the upper and lower bounds of the camera frustum.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[FOVMODE_VERTICAL_FIXED](ArcRotateCamera.md#fovmode_vertical_fixed)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:58

___

### ForceAttachControlToAlwaysPreventDefault

▪ `Static` **ForceAttachControlToAlwaysPreventDefault**: `boolean` = `false`

Defines if by default attaching controls should prevent the default javascript event to continue.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[ForceAttachControlToAlwaysPreventDefault](ArcRotateCamera.md#forceattachcontroltoalwayspreventdefault)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:106

___

### ORTHOGRAPHIC\_CAMERA

▪ `Static` `Readonly` **ORTHOGRAPHIC\_CAMERA**: ``1``

This helps creating camera with an orthographic mode.
Orthographic is commonly used in engineering as a means to produce object specifications that communicate dimensions unambiguously, each line of 1 unit length (cm, meter..whatever) will appear to have the same length everywhere on the drawing. This allows the drafter to dimension only a subset of lines and let the reader know that other lines of that length on the drawing are also that length in reality. Every parallel line in the drawing is also parallel in the object.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[ORTHOGRAPHIC_CAMERA](ArcRotateCamera.md#orthographic_camera)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:52

___

### PERSPECTIVE\_CAMERA

▪ `Static` `Readonly` **PERSPECTIVE\_CAMERA**: ``0``

This is the default projection mode used by the cameras.
It helps recreating a feeling of perspective and better appreciate depth.
This is the best way to simulate real life cameras.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[PERSPECTIVE_CAMERA](ArcRotateCamera.md#perspective_camera)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:47

___

### RIG\_MODE\_CUSTOM

▪ `Static` `Readonly` **RIG\_MODE\_CUSTOM**: ``22``

Custom rig mode allowing rig cameras to be populated manually with any number of cameras

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[RIG_MODE_CUSTOM](ArcRotateCamera.md#rig_mode_custom)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:101

___

### RIG\_MODE\_NONE

▪ `Static` `Readonly` **RIG\_MODE\_NONE**: ``0``

This specifies there is no need for a camera rig.
Basically only one eye is rendered corresponding to the camera.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[RIG_MODE_NONE](ArcRotateCamera.md#rig_mode_none)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:68

___

### RIG\_MODE\_STEREOSCOPIC\_ANAGLYPH

▪ `Static` `Readonly` **RIG\_MODE\_STEREOSCOPIC\_ANAGLYPH**: ``10``

Simulates a camera Rig with one blue eye and one red eye.
This can be use with 3d blue and red glasses.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[RIG_MODE_STEREOSCOPIC_ANAGLYPH](ArcRotateCamera.md#rig_mode_stereoscopic_anaglyph)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:73

___

### RIG\_MODE\_STEREOSCOPIC\_INTERLACED

▪ `Static` `Readonly` **RIG\_MODE\_STEREOSCOPIC\_INTERLACED**: ``14``

Defines that both eyes of the camera will be rendered on successive lines interlaced for passive 3d monitors.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[RIG_MODE_STEREOSCOPIC_INTERLACED](ArcRotateCamera.md#rig_mode_stereoscopic_interlaced)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:89

___

### RIG\_MODE\_STEREOSCOPIC\_OVERUNDER

▪ `Static` `Readonly` **RIG\_MODE\_STEREOSCOPIC\_OVERUNDER**: ``13``

Defines that both eyes of the camera will be rendered over under each other.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[RIG_MODE_STEREOSCOPIC_OVERUNDER](ArcRotateCamera.md#rig_mode_stereoscopic_overunder)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:85

___

### RIG\_MODE\_STEREOSCOPIC\_SIDEBYSIDE\_CROSSEYED

▪ `Static` `Readonly` **RIG\_MODE\_STEREOSCOPIC\_SIDEBYSIDE\_CROSSEYED**: ``12``

Defines that both eyes of the camera will be rendered side by side with a none parallel target.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[RIG_MODE_STEREOSCOPIC_SIDEBYSIDE_CROSSEYED](ArcRotateCamera.md#rig_mode_stereoscopic_sidebyside_crosseyed)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:81

___

### RIG\_MODE\_STEREOSCOPIC\_SIDEBYSIDE\_PARALLEL

▪ `Static` `Readonly` **RIG\_MODE\_STEREOSCOPIC\_SIDEBYSIDE\_PARALLEL**: ``11``

Defines that both eyes of the camera will be rendered side by side with a parallel target.

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[RIG_MODE_STEREOSCOPIC_SIDEBYSIDE_PARALLEL](ArcRotateCamera.md#rig_mode_stereoscopic_sidebyside_parallel)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:77

___

### RIG\_MODE\_VR

▪ `Static` `Readonly` **RIG\_MODE\_VR**: ``20``

Defines that both eyes of the camera should be renderered in a VR mode (carbox).

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[RIG_MODE_VR](ArcRotateCamera.md#rig_mode_vr)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:93

___

### RIG\_MODE\_WEBVR

▪ `Static` `Readonly` **RIG\_MODE\_WEBVR**: ``21``

Defines that both eyes of the camera should be renderered in a VR mode (webVR).

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[RIG_MODE_WEBVR](ArcRotateCamera.md#rig_mode_webvr)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:97

## Accessors

### absoluteRotation

• `get` **absoluteRotation**(): [`Quaternion`](Quaternion.md)

Returns the current camera absolute rotation

#### Returns

[`Quaternion`](Quaternion.md)

#### Inherited from

ArcRotateCamera.absoluteRotation

#### Defined in

packages/dev/core/src/Cameras/camera.ts:1378

___

### angularSensibilityX

• `get` **angularSensibilityX**(): `number`

Gets or Set the pointer angular sensibility  along the X axis or how fast is the camera rotating.

#### Returns

`number`

#### Inherited from

ArcRotateCamera.angularSensibilityX

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:253

• `set` **angularSensibilityX**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

ArcRotateCamera.angularSensibilityX

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:262

___

### angularSensibilityY

• `get` **angularSensibilityY**(): `number`

Gets or Set the pointer angular sensibility along the Y axis or how fast is the camera rotating.

#### Returns

`number`

#### Inherited from

ArcRotateCamera.angularSensibilityY

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:272

• `set` **angularSensibilityY**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

ArcRotateCamera.angularSensibilityY

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:281

___

### animationPropertiesOverride

• `get` **animationPropertiesOverride**(): [`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md)

Gets or sets the animation properties override

#### Returns

[`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md)

#### Inherited from

ArcRotateCamera.animationPropertiesOverride

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

ArcRotateCamera.animationPropertiesOverride

#### Defined in

packages/dev/core/src/node.ts:282

___

### autoRotationBehavior

• `get` **autoRotationBehavior**(): [`Nullable`](../modules.md#nullable)[`AutoRotationBehavior`](AutoRotationBehavior.md)

Gets the auto rotation behavior of the camera if it has been enabled.

**`See`**

https://doc.babylonjs.com/how_to/camera_behaviors#autorotation-behavior

#### Returns

[`Nullable`](../modules.md#nullable)[`AutoRotationBehavior`](AutoRotationBehavior.md)

#### Inherited from

ArcRotateCamera.autoRotationBehavior

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:631

___

### behaviors

• `get` **behaviors**(): [`Behavior`](../interfaces/Behavior.md)[`Node`](Node.md)[]

Gets the list of attached behaviors

**`See`**

https://doc.babylonjs.com/features/behaviour

#### Returns

[`Behavior`](../interfaces/Behavior.md)[`Node`](Node.md)[]

#### Inherited from

ArcRotateCamera.behaviors

#### Defined in

packages/dev/core/src/node.ts:410

___

### bouncingBehavior

• `get` **bouncingBehavior**(): [`Nullable`](../modules.md#nullable)[`BouncingBehavior`](BouncingBehavior.md)

Gets the bouncing behavior of the camera if it has been enabled.

**`See`**

https://doc.babylonjs.com/how_to/camera_behaviors#bouncing-behavior

#### Returns

[`Nullable`](../modules.md#nullable)[`BouncingBehavior`](BouncingBehavior.md)

#### Inherited from

ArcRotateCamera.bouncingBehavior

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:567

___

### doNotSerialize

• `get` **doNotSerialize**(): `boolean`

Gets or sets a boolean used to define if the node must be serialized

#### Returns

`boolean`

#### Inherited from

ArcRotateCamera.doNotSerialize

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

ArcRotateCamera.doNotSerialize

#### Defined in

packages/dev/core/src/node.ts:143

___

### framingBehavior

• `get` **framingBehavior**(): [`Nullable`](../modules.md#nullable)[`FramingBehavior`](FramingBehavior.md)

Gets the framing behavior of the camera if it has been enabled.

**`See`**

https://doc.babylonjs.com/how_to/camera_behaviors#framing-behavior

#### Returns

[`Nullable`](../modules.md#nullable)[`FramingBehavior`](FramingBehavior.md)

#### Inherited from

ArcRotateCamera.framingBehavior

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:599

___

### globalPosition

• `get` **globalPosition**(): [`Vector3`](Vector3.md)

Gets the current world space position of the camera.

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

ArcRotateCamera.globalPosition

#### Defined in

packages/dev/core/src/Cameras/camera.ts:522

___

### isLeftCamera

• `get` **isLeftCamera**(): `boolean`

Gets the left camera of a rig setup in case of Rigged Camera

#### Returns

`boolean`

#### Inherited from

ArcRotateCamera.isLeftCamera

#### Defined in

packages/dev/core/src/Cameras/camera.ts:1120

___

### isRightCamera

• `get` **isRightCamera**(): `boolean`

Gets the right camera of a rig setup in case of Rigged Camera

#### Returns

`boolean`

#### Inherited from

ArcRotateCamera.isRightCamera

#### Defined in

packages/dev/core/src/Cameras/camera.ts:1129

___

### keysDown

• `get` **keysDown**(): `number`[]

Gets or Set the list of keyboard keys used to control beta angle in a negative direction.

#### Returns

`number`[]

#### Inherited from

ArcRotateCamera.keysDown

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:392

• `set` **keysDown**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number`[] |

#### Returns

`void`

#### Inherited from

ArcRotateCamera.keysDown

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:401

___

### keysLeft

• `get` **keysLeft**(): `number`[]

Gets or Set the list of keyboard keys used to control alpha angle in a negative direction.

#### Returns

`number`[]

#### Inherited from

ArcRotateCamera.keysLeft

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:411

• `set` **keysLeft**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number`[] |

#### Returns

`void`

#### Inherited from

ArcRotateCamera.keysLeft

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:420

___

### keysRight

• `get` **keysRight**(): `number`[]

Gets or Set the list of keyboard keys used to control alpha angle in a positive direction.

#### Returns

`number`[]

#### Inherited from

ArcRotateCamera.keysRight

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:430

• `set` **keysRight**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number`[] |

#### Returns

`void`

#### Inherited from

ArcRotateCamera.keysRight

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:439

___

### keysUp

• `get` **keysUp**(): `number`[]

Gets or Set the list of keyboard keys used to control beta angle in a positive direction.

#### Returns

`number`[]

#### Inherited from

ArcRotateCamera.keysUp

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:373

• `set` **keysUp**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number`[] |

#### Returns

`void`

#### Inherited from

ArcRotateCamera.keysUp

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:382

___

### leftCamera

• `get` **leftCamera**(): [`Nullable`](../modules.md#nullable)[`FreeCamera`](FreeCamera.md)

Gets the left camera of a rig setup in case of Rigged Camera

#### Returns

[`Nullable`](../modules.md#nullable)[`FreeCamera`](FreeCamera.md)

#### Inherited from

ArcRotateCamera.leftCamera

#### Defined in

packages/dev/core/src/Cameras/camera.ts:1136

___

### mode

• `get` **mode**(): `number`

#### Returns

`number`

#### Inherited from

ArcRotateCamera.mode

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

ArcRotateCamera.mode

#### Defined in

packages/dev/core/src/Cameras/camera.ts:285

___

### onClonedObservable

• `get` **onClonedObservable**(): [`Observable`](Observable.md)[`Node`](Node.md)

An event triggered when the node is cloned

#### Returns

[`Observable`](Observable.md)[`Node`](Node.md)

#### Inherited from

ArcRotateCamera.onClonedObservable

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

ArcRotateCamera.onDispose

#### Defined in

packages/dev/core/src/node.ts:306

___

### onEnabledStateChangedObservable

• `get` **onEnabledStateChangedObservable**(): [`Observable`](Observable.md)`boolean`

An event triggered when the enabled state of the node changes

#### Returns

[`Observable`](Observable.md)`boolean`

#### Inherited from

ArcRotateCamera.onEnabledStateChangedObservable

#### Defined in

packages/dev/core/src/node.ts:316

___

### orthoBottom

• `get` **orthoBottom**(): [`Nullable`](../modules.md#nullable)`number`

#### Returns

[`Nullable`](../modules.md#nullable)`number`

#### Inherited from

ArcRotateCamera.orthoBottom

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

ArcRotateCamera.orthoBottom

#### Defined in

packages/dev/core/src/Cameras/camera.ts:212

___

### orthoLeft

• `get` **orthoLeft**(): [`Nullable`](../modules.md#nullable)`number`

#### Returns

[`Nullable`](../modules.md#nullable)`number`

#### Inherited from

ArcRotateCamera.orthoLeft

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

ArcRotateCamera.orthoLeft

#### Defined in

packages/dev/core/src/Cameras/camera.ts:174

___

### orthoRight

• `get` **orthoRight**(): [`Nullable`](../modules.md#nullable)`number`

#### Returns

[`Nullable`](../modules.md#nullable)`number`

#### Inherited from

ArcRotateCamera.orthoRight

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

ArcRotateCamera.orthoRight

#### Defined in

packages/dev/core/src/Cameras/camera.ts:193

___

### orthoTop

• `get` **orthoTop**(): [`Nullable`](../modules.md#nullable)`number`

#### Returns

[`Nullable`](../modules.md#nullable)`number`

#### Inherited from

ArcRotateCamera.orthoTop

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

ArcRotateCamera.orthoTop

#### Defined in

packages/dev/core/src/Cameras/camera.ts:231

___

### panningSensibility

• `get` **panningSensibility**(): `number`

Gets or Set the pointer panning sensibility or how fast is the camera moving.

#### Returns

`number`

#### Inherited from

ArcRotateCamera.panningSensibility

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:354

• `set` **panningSensibility**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

ArcRotateCamera.panningSensibility

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:363

___

### parent

• `get` **parent**(): [`Nullable`](../modules.md#nullable)[`Node`](Node.md)

#### Returns

[`Nullable`](../modules.md#nullable)[`Node`](Node.md)

#### Inherited from

ArcRotateCamera.parent

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

ArcRotateCamera.parent

#### Defined in

packages/dev/core/src/node.ts:200

___

### pinchDeltaPercentage

• `get` **pinchDeltaPercentage**(): `number`

Gets or Set the pointer pinch delta percentage or how fast is the camera zooming.
It will be used instead of pinchDeltaPrecision if different from 0.
It defines the percentage of current camera.radius to use as delta when pinch zoom is used.

#### Returns

`number`

#### Inherited from

ArcRotateCamera.pinchDeltaPercentage

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:312

• `set` **pinchDeltaPercentage**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

ArcRotateCamera.pinchDeltaPercentage

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:321

___

### pinchPrecision

• `get` **pinchPrecision**(): `number`

Gets or Set the pointer pinch precision or how fast is the camera zooming.

#### Returns

`number`

#### Inherited from

ArcRotateCamera.pinchPrecision

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:291

• `set` **pinchPrecision**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

ArcRotateCamera.pinchPrecision

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:300

___

### position

• `get` **position**(): [`Vector3`](Vector3.md)

Define the current local position of the camera in the scene

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

ArcRotateCamera.position

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:101

• `set` **position**(`newPosition`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `newPosition` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Inherited from

ArcRotateCamera.position

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:105

___

### rigPostProcess

• `get` **rigPostProcess**(): [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)

Gets the post process used by the rig cameras

#### Returns

[`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)

#### Inherited from

ArcRotateCamera.rigPostProcess

#### Defined in

packages/dev/core/src/Cameras/camera.ts:697

___

### rightCamera

• `get` **rightCamera**(): [`Nullable`](../modules.md#nullable)[`FreeCamera`](FreeCamera.md)

Gets the right camera of a rig setup in case of Rigged Camera

#### Returns

[`Nullable`](../modules.md#nullable)[`FreeCamera`](FreeCamera.md)

#### Inherited from

ArcRotateCamera.rightCamera

#### Defined in

packages/dev/core/src/Cameras/camera.ts:1146

___

### screenArea

• `get` **screenArea**(): `number`

The screen area in scene units squared

#### Returns

`number`

#### Inherited from

ArcRotateCamera.screenArea

#### Defined in

packages/dev/core/src/Cameras/camera.ts:146

___

### target

• `get` **target**(): [`Vector3`](Vector3.md)

Defines the target point of the camera.
The camera looks towards it from the radius distance.

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

ArcRotateCamera.target

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:69

• `set` **target**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Inherited from

ArcRotateCamera.target

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:72

___

### targetHost

• `get` **targetHost**(): [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

Defines the target mesh of the camera.
The camera looks towards it from the radius distance.
Please note that setting a target host will disable panning.

#### Returns

[`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

#### Inherited from

ArcRotateCamera.targetHost

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:81

• `set` **targetHost**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md) |

#### Returns

`void`

#### Inherited from

ArcRotateCamera.targetHost

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:84

___

### upVector

• `get` **upVector**(): [`Vector3`](Vector3.md)

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

ArcRotateCamera.upVector

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:130

• `set` **upVector**(`vec`): `void`

The vector the camera should consider as up. (default is Vector3(0, 1, 0) as returned by Vector3.Up())
Setting this will copy the given vector to the camera's upVector, and set rotation matrices to and from Y up.
DO NOT set the up vector using copyFrom or copyFromFloats, as this bypasses setting the above matrices.

#### Parameters

| Name | Type |
| :------ | :------ |
| `vec` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Inherited from

ArcRotateCamera.upVector

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:117

___

### useAutoRotationBehavior

• `get` **useAutoRotationBehavior**(): `boolean`

Defines if the auto rotation behavior of the camera is enabled on the camera.

**`See`**

https://doc.babylonjs.com/how_to/camera_behaviors#autorotation-behavior

#### Returns

`boolean`

#### Inherited from

ArcRotateCamera.useAutoRotationBehavior

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:639

• `set` **useAutoRotationBehavior**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

ArcRotateCamera.useAutoRotationBehavior

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:643

___

### useBouncingBehavior

• `get` **useBouncingBehavior**(): `boolean`

Defines if the bouncing behavior of the camera is enabled on the camera.

**`See`**

https://doc.babylonjs.com/how_to/camera_behaviors#bouncing-behavior

#### Returns

`boolean`

#### Inherited from

ArcRotateCamera.useBouncingBehavior

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:575

• `set` **useBouncingBehavior**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

ArcRotateCamera.useBouncingBehavior

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:579

___

### useFramingBehavior

• `get` **useFramingBehavior**(): `boolean`

Defines if the framing behavior of the camera is enabled on the camera.

**`See`**

https://doc.babylonjs.com/how_to/camera_behaviors#framing-behavior

#### Returns

`boolean`

#### Inherited from

ArcRotateCamera.useFramingBehavior

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:607

• `set` **useFramingBehavior**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

ArcRotateCamera.useFramingBehavior

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:611

___

### useNaturalPinchZoom

• `get` **useNaturalPinchZoom**(): `boolean`

Gets or Set the pointer use natural pinch zoom to override the pinch precision
and pinch delta percentage.
When useNaturalPinchZoom is true, multi touch zoom will zoom in such
that any object in the plane at the camera's target point will scale
perfectly with finger motion.

#### Returns

`boolean`

#### Inherited from

ArcRotateCamera.useNaturalPinchZoom

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:335

• `set` **useNaturalPinchZoom**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

ArcRotateCamera.useNaturalPinchZoom

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:344

___

### wheelDeltaPercentage

• `get` **wheelDeltaPercentage**(): `number`

Gets or Set the mouse wheel delta percentage or how fast is the camera zooming.
It will be used instead of pinchDeltaPrecision if different from 0.
It defines the percentage of current camera.radius to use as delta when pinch zoom is used.

#### Returns

`number`

#### Inherited from

ArcRotateCamera.wheelDeltaPercentage

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:491

• `set` **wheelDeltaPercentage**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

ArcRotateCamera.wheelDeltaPercentage

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:500

___

### wheelPrecision

• `get` **wheelPrecision**(): `number`

Gets or Set the mouse wheel precision or how fast is the camera zooming.

#### Returns

`number`

#### Inherited from

ArcRotateCamera.wheelPrecision

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:449

• `set` **wheelPrecision**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

ArcRotateCamera.wheelPrecision

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:458

___

### worldMatrixFromCache

• `get` **worldMatrixFromCache**(): [`Matrix`](Matrix.md)

Returns directly the latest state of the mesh World matrix.
A Matrix is returned.

#### Returns

[`Matrix`](Matrix.md)

#### Inherited from

ArcRotateCamera.worldMatrixFromCache

#### Defined in

packages/dev/core/src/node.ts:454

___

### zoomToMouseLocation

• `get` **zoomToMouseLocation**(): `boolean`

Gets or Set the boolean value that controls whether or not the mouse wheel
zooms to the location of the mouse pointer or not.  The default is false.

#### Returns

`boolean`

#### Inherited from

ArcRotateCamera.zoomToMouseLocation

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:469

• `set` **zoomToMouseLocation**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

ArcRotateCamera.zoomToMouseLocation

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:479

## Methods

### \_checkLimits

▸ `Protected` **_checkLimits**(): `void`

#### Returns

`void`

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[_checkLimits](ArcRotateCamera.md#_checklimits)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:985

___

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

[ArcRotateCamera](ArcRotateCamera.md).[_computeViewMatrix](ArcRotateCamera.md#_computeviewmatrix)

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

[ArcRotateCamera](ArcRotateCamera.md).[_getFirstPostProcess](ArcRotateCamera.md#_getfirstpostprocess)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:705

___

### \_getTargetPosition

▸ `Protected` **_getTargetPosition**(): [`Vector3`](Vector3.md)

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[_getTargetPosition](ArcRotateCamera.md#_gettargetposition)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:748

___

### \_onCollisionPositionChange

▸ `Protected` **_onCollisionPositionChange**(`collisionId`, `newPosition`, `collidedMesh?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `collisionId` | `number` | `undefined` |
| `newPosition` | [`Vector3`](Vector3.md) | `undefined` |
| `collidedMesh` | [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md) | `null` |

#### Returns

`void`

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[_onCollisionPositionChange](ArcRotateCamera.md#_oncollisionpositionchange)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:1167

___

### \_updateCameraRotationMatrix

▸ `Protected` **_updateCameraRotationMatrix**(): `void`

#### Returns

`void`

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[_updateCameraRotationMatrix](ArcRotateCamera.md#_updatecamerarotationmatrix)

#### Defined in

packages/dev/core/src/Cameras/targetCamera.ts:395

___

### \_updateWebVRCameraRotationMatrix

▸ `Protected` **_updateWebVRCameraRotationMatrix**(): `void`

#### Returns

`void`

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[_updateWebVRCameraRotationMatrix](ArcRotateCamera.md#_updatewebvrcamerarotationmatrix)

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

[ArcRotateCamera](ArcRotateCamera.md).[addBehavior](ArcRotateCamera.md#addbehavior)

#### Defined in

packages/dev/core/src/node.ts:366

___

### applyVerticalCorrection

▸ **applyVerticalCorrection**(): `void`

Automatically tilts the projection plane, using `projectionPlaneTilt`, to correct the perspective effect on vertical lines.

#### Returns

`void`

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[applyVerticalCorrection](ArcRotateCamera.md#applyverticalcorrection)

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

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[attachControl](ArcRotateCamera.md#attachcontrol)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:831

▸ **attachControl**(`ignored`, `noPreventDefault?`): `void`

Attach the input controls to a specific dom element to get the input from.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ignored` | `any` | defines an ignored parameter kept for backward compatibility. |
| `noPreventDefault?` | `boolean` | Defines whether event caught by the controls should call preventdefault() (https://developer.mozilla.org/en-US/docs/Web/API/Event/preventDefault) |

#### Returns

`void`

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[attachControl](ArcRotateCamera.md#attachcontrol)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:837

▸ **attachControl**(`noPreventDefault`, `useCtrlForPanning`): `void`

Attached controls to the current camera.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `noPreventDefault` | `boolean` | Defines whether event caught by the controls should call preventdefault() (https://developer.mozilla.org/en-US/docs/Web/API/Event/preventDefault) |
| `useCtrlForPanning` | `boolean` | Defines whether ctrl is used for panning within the controls |

#### Returns

`void`

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[attachControl](ArcRotateCamera.md#attachcontrol)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:843

▸ **attachControl**(`ignored`, `noPreventDefault`, `useCtrlForPanning`): `void`

Attached controls to the current camera.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ignored` | `any` | defines an ignored parameter kept for backward compatibility. |
| `noPreventDefault` | `boolean` | Defines whether event caught by the controls should call preventdefault() (https://developer.mozilla.org/en-US/docs/Web/API/Event/preventDefault) |
| `useCtrlForPanning` | `boolean` | Defines whether ctrl is used for panning within the controls |

#### Returns

`void`

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[attachControl](ArcRotateCamera.md#attachcontrol)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:850

▸ **attachControl**(`noPreventDefault`, `useCtrlForPanning`, `panningMouseButton`): `void`

Attached controls to the current camera.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `noPreventDefault` | `boolean` | Defines whether event caught by the controls should call preventdefault() (https://developer.mozilla.org/en-US/docs/Web/API/Event/preventDefault) |
| `useCtrlForPanning` | `boolean` | Defines whether ctrl is used for panning within the controls |
| `panningMouseButton` | `number` | Defines whether panning is allowed through mouse click button |

#### Returns

`void`

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[attachControl](ArcRotateCamera.md#attachcontrol)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:857

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

[ArcRotateCamera](ArcRotateCamera.md).[attachPostProcess](ArcRotateCamera.md#attachpostprocess)

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

[ArcRotateCamera](ArcRotateCamera.md).[beginAnimation](ArcRotateCamera.md#beginanimation)

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

[ArcRotateCamera](ArcRotateCamera.md).[clone](ArcRotateCamera.md#clone)

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

[ArcRotateCamera](ArcRotateCamera.md).[computeWorldMatrix](ArcRotateCamera.md#computeworldmatrix)

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

[ArcRotateCamera](ArcRotateCamera.md).[createAnimationRange](ArcRotateCamera.md#createanimationrange)

#### Defined in

packages/dev/core/src/node.ts:777

___

### createRigCamera

▸ **createRigCamera**(`name`, `cameraIndex`): [`Camera`](Camera.md)

Override Camera.createRigCamera

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `cameraIndex` | `number` |

#### Returns

[`Camera`](Camera.md)

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[createRigCamera](ArcRotateCamera.md#createrigcamera)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:1255

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

[ArcRotateCamera](ArcRotateCamera.md).[deleteAnimationRange](ArcRotateCamera.md#deleteanimationrange)

#### Defined in

packages/dev/core/src/node.ts:794

___

### detachControl

▸ **detachControl**(): `void`

Detach the current controls from the specified dom element.

#### Returns

`void`

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[detachControl](ArcRotateCamera.md#detachcontrol)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:896

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

[ArcRotateCamera](ArcRotateCamera.md).[detachPostProcess](ArcRotateCamera.md#detachpostprocess)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:776

___

### dispose

▸ **dispose**(): `void`

Destroy the camera and release the current resources hold by it.

#### Returns

`void`

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[dispose](ArcRotateCamera.md#dispose)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:1315

___

### focusOn

▸ **focusOn**(`meshesOrMinMaxVectorAndDistance`, `doNotUpdateMaxZ?`): `void`

Focus on a mesh or a bounding box. This adapts the target and maxRadius if necessary but does not update the current radius.
The target will be changed but the radius

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `meshesOrMinMaxVectorAndDistance` | [`AbstractMesh`](AbstractMesh.md)[] \| { `distance`: `number` ; `max`: [`Vector3`](Vector3.md) ; `min`: [`Vector3`](Vector3.md)  } | `undefined` | Defines the mesh or bounding info to focus on |
| `doNotUpdateMaxZ` | `boolean` | `false` | Defines whether or not maxZ should be updated whilst zooming on the mesh (this can happen if the mesh is big and the maxradius pretty small for instance) |

#### Returns

`void`

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[focusOn](ArcRotateCamera.md#focuson)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:1228

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

[ArcRotateCamera](ArcRotateCamera.md).[freezeProjectionMatrix](ArcRotateCamera.md#freezeprojectionmatrix)

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

[ArcRotateCamera](ArcRotateCamera.md).[getActiveMeshes](ArcRotateCamera.md#getactivemeshes)

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

[ArcRotateCamera](ArcRotateCamera.md).[getAnimationByName](ArcRotateCamera.md#getanimationbyname)

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

[ArcRotateCamera](ArcRotateCamera.md).[getAnimationRange](ArcRotateCamera.md#getanimationrange)

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

[ArcRotateCamera](ArcRotateCamera.md).[getAnimationRanges](ArcRotateCamera.md#getanimationranges)

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

[ArcRotateCamera](ArcRotateCamera.md).[getBehaviorByName](ArcRotateCamera.md#getbehaviorbyname)

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

[ArcRotateCamera](ArcRotateCamera.md).[getChildMeshes](ArcRotateCamera.md#getchildmeshes)

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

[ArcRotateCamera](ArcRotateCamera.md).[getChildMeshes](ArcRotateCamera.md#getchildmeshes)

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

[ArcRotateCamera](ArcRotateCamera.md).[getChildren](ArcRotateCamera.md#getchildren)

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

[ArcRotateCamera](ArcRotateCamera.md).[getChildren](ArcRotateCamera.md#getchildren)

#### Defined in

packages/dev/core/src/node.ts:722

___

### getClassName

▸ **getClassName**(): `string`

Gets camera class name

#### Returns

`string`

StereoscopicArcRotateCamera

#### Overrides

[ArcRotateCamera](ArcRotateCamera.md).[getClassName](ArcRotateCamera.md#getclassname)

#### Defined in

packages/dev/core/src/Cameras/Stereoscopic/stereoscopicArcRotateCamera.ts:41

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

[ArcRotateCamera](ArcRotateCamera.md).[getDescendants](ArcRotateCamera.md#getdescendants)

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

[ArcRotateCamera](ArcRotateCamera.md).[getDescendants](ArcRotateCamera.md#getdescendants)

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

[ArcRotateCamera](ArcRotateCamera.md).[getDirection](ArcRotateCamera.md#getdirection)

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

[ArcRotateCamera](ArcRotateCamera.md).[getDirectionToRef](ArcRotateCamera.md#getdirectiontoref)

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

[ArcRotateCamera](ArcRotateCamera.md).[getEngine](ArcRotateCamera.md#getengine)

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

[ArcRotateCamera](ArcRotateCamera.md).[getForwardRay](ArcRotateCamera.md#getforwardray)

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

[ArcRotateCamera](ArcRotateCamera.md).[getForwardRayToRef](ArcRotateCamera.md#getforwardraytoref)

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

[ArcRotateCamera](ArcRotateCamera.md).[getFrontPosition](ArcRotateCamera.md#getfrontposition)

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

[ArcRotateCamera](ArcRotateCamera.md).[getHierarchyBoundingVectors](ArcRotateCamera.md#gethierarchyboundingvectors)

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

[ArcRotateCamera](ArcRotateCamera.md).[getLeftTarget](ArcRotateCamera.md#getlefttarget)

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

[ArcRotateCamera](ArcRotateCamera.md).[getProjectionMatrix](ArcRotateCamera.md#getprojectionmatrix)

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

[ArcRotateCamera](ArcRotateCamera.md).[getRightTarget](ArcRotateCamera.md#getrighttarget)

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

[ArcRotateCamera](ArcRotateCamera.md).[getScene](ArcRotateCamera.md#getscene)

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

[ArcRotateCamera](ArcRotateCamera.md).[getTarget](ArcRotateCamera.md#gettarget)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:94

___

### getTransformationMatrix

▸ **getTransformationMatrix**(): [`Matrix`](Matrix.md)

Gets the transformation matrix (ie. the multiplication of view by projection matrices)

#### Returns

[`Matrix`](Matrix.md)

a Matrix

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[getTransformationMatrix](ArcRotateCamera.md#gettransformationmatrix)

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

[ArcRotateCamera](ArcRotateCamera.md).[getViewMatrix](ArcRotateCamera.md#getviewmatrix)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:814

___

### getWorldMatrix

▸ **getWorldMatrix**(): [`Matrix`](Matrix.md)

Gets the current world matrix of the camera

#### Returns

[`Matrix`](Matrix.md)

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[getWorldMatrix](ArcRotateCamera.md#getworldmatrix)

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

[ArcRotateCamera](ArcRotateCamera.md).[isActiveMesh](ArcRotateCamera.md#isactivemesh)

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

[ArcRotateCamera](ArcRotateCamera.md).[isCompletelyInFrustum](ArcRotateCamera.md#iscompletelyinfrustum)

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

[ArcRotateCamera](ArcRotateCamera.md).[isDescendantOf](ArcRotateCamera.md#isdescendantof)

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

[ArcRotateCamera](ArcRotateCamera.md).[isDisposed](ArcRotateCamera.md#isdisposed)

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

[ArcRotateCamera](ArcRotateCamera.md).[isEnabled](ArcRotateCamera.md#isenabled)

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

[ArcRotateCamera](ArcRotateCamera.md).[isInFrustum](ArcRotateCamera.md#isinfrustum)

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

[ArcRotateCamera](ArcRotateCamera.md).[isReady](ArcRotateCamera.md#isready)

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

[ArcRotateCamera](ArcRotateCamera.md).[markAsDirty](ArcRotateCamera.md#markasdirty)

#### Defined in

packages/dev/core/src/node.ts:557

___

### rebuildAnglesAndRadius

▸ **rebuildAnglesAndRadius**(): `void`

Rebuilds angles (alpha, beta) and radius from the give position and target

#### Returns

`void`

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[rebuildAnglesAndRadius](ArcRotateCamera.md#rebuildanglesandradius)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:1026

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

[ArcRotateCamera](ArcRotateCamera.md).[removeBehavior](ArcRotateCamera.md#removebehavior)

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

[ArcRotateCamera](ArcRotateCamera.md).[restoreState](ArcRotateCamera.md#restorestate)

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

[ArcRotateCamera](ArcRotateCamera.md).[serialize](ArcRotateCamera.md#serialize)

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

[ArcRotateCamera](ArcRotateCamera.md).[serializeAnimationRanges](ArcRotateCamera.md#serializeanimationranges)

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

[ArcRotateCamera](ArcRotateCamera.md).[setEnabled](ArcRotateCamera.md#setenabled)

#### Defined in

packages/dev/core/src/node.ts:596

___

### setMatUp

▸ **setMatUp**(): `void`

Sets the Y-up to camera up-vector rotation matrix, and the up-vector to Y-up rotation matrix.

#### Returns

`void`

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[setMatUp](ArcRotateCamera.md#setmatup)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:137

___

### setPosition

▸ **setPosition**(`position`): `void`

Use a position to define the current camera related information like alpha, beta and radius

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | [`Vector3`](Vector3.md) | Defines the position to set the camera at |

#### Returns

`void`

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[setPosition](ArcRotateCamera.md#setposition)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:1067

___

### setTarget

▸ **setTarget**(`target`, `toBoundingCenter?`, `allowSamePosition?`, `cloneAlphaBetaRadius?`): `void`

Defines the target the camera should look at.
This will automatically adapt alpha beta and radius to fit within the new target.
Please note that setting a target as a mesh will disable panning.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `target` | [`AbstractMesh`](AbstractMesh.md) \| [`Vector3`](Vector3.md) | `undefined` | Defines the new target as a Vector or a mesh |
| `toBoundingCenter` | `boolean` | `false` | In case of a mesh target, defines whether to target the mesh position or its bounding information center |
| `allowSamePosition` | `boolean` | `false` | If false, prevents reapplying the new computed position if it is identical to the current one (optim) |
| `cloneAlphaBetaRadius` | `boolean` | `false` | If true, replicate the current setup (alpha, beta, radius) on the new target |

#### Returns

`void`

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[setTarget](ArcRotateCamera.md#settarget)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:1085

___

### storeState

▸ **storeState**(): [`Camera`](Camera.md)

Stores the current state of the camera (alpha, beta, radius and target)

#### Returns

[`Camera`](Camera.md)

the camera itself

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[storeState](ArcRotateCamera.md#storestate)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:777

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

[ArcRotateCamera](ArcRotateCamera.md).[toString](ArcRotateCamera.md#tostring)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:499

___

### unfreezeProjectionMatrix

▸ **unfreezeProjectionMatrix**(): `void`

Unfreeze the projection matrix if it has previously been freezed by freezeProjectionMatrix.

#### Returns

`void`

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[unfreezeProjectionMatrix](ArcRotateCamera.md#unfreezeprojectionmatrix)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:858

___

### update

▸ **update**(): `void`

Update the camera state according to the different inputs gathered during the frame.

#### Returns

`void`

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[update](ArcRotateCamera.md#update)

#### Defined in

packages/dev/core/src/Cameras/camera.ts:677

___

### zoomOn

▸ **zoomOn**(`meshes?`, `doNotUpdateMaxZ?`): `void`

Zooms on a mesh to be at the min distance where we could see it fully in the current viewport.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `meshes?` | [`AbstractMesh`](AbstractMesh.md)[] | `undefined` | Defines the mesh to zoom on |
| `doNotUpdateMaxZ` | `boolean` | `false` | Defines whether or not maxZ should be updated whilst zooming on the mesh (this can happen if the mesh is big and the maxradius pretty small for instance) |

#### Returns

`void`

#### Inherited from

[ArcRotateCamera](ArcRotateCamera.md).[zoomOn](ArcRotateCamera.md#zoomon)

#### Defined in

packages/dev/core/src/Cameras/arcRotateCamera.ts:1211

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

[ArcRotateCamera](ArcRotateCamera.md).[AddNodeConstructor](ArcRotateCamera.md#addnodeconstructor)

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

[ArcRotateCamera](ArcRotateCamera.md).[Construct](ArcRotateCamera.md#construct)

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

[ArcRotateCamera](ArcRotateCamera.md).[GetConstructorFromName](ArcRotateCamera.md#getconstructorfromname)

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

[ArcRotateCamera](ArcRotateCamera.md).[Parse](ArcRotateCamera.md#parse)

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

[ArcRotateCamera](ArcRotateCamera.md).[ParseAnimationRanges](ArcRotateCamera.md#parseanimationranges)

#### Defined in

packages/dev/core/src/node.ts:919
