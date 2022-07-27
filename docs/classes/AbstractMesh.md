[@dev/core](../README.md) / [Exports](../modules.md) / AbstractMesh

# Class: AbstractMesh

Class used to store all common mesh properties

## Hierarchy

- [`TransformNode`](TransformNode.md)

  ↳ **`AbstractMesh`**

  ↳↳ [`InstancedMesh`](InstancedMesh.md)

  ↳↳ [`Mesh`](Mesh.md)

## Implements

- [`IDisposable`](../interfaces/IDisposable.md)
- [`ICullable`](../interfaces/ICullable.md)
- [`IGetSetVerticesData`](../interfaces/IGetSetVerticesData.md)

## Table of contents

### Constructors

- [constructor](AbstractMesh.md#constructor)

### Properties

- [\_boundingInfo](AbstractMesh.md#_boundinginfo)
- [\_boundingInfoIsDirty](AbstractMesh.md#_boundinginfoisdirty)
- [\_isDirty](AbstractMesh.md#_isdirty)
- [\_isWorldMatrixFrozen](AbstractMesh.md#_isworldmatrixfrozen)
- [\_parentNode](AbstractMesh.md#_parentnode)
- [\_ranges](AbstractMesh.md#_ranges)
- [\_scaling](AbstractMesh.md#_scaling)
- [actionManager](AbstractMesh.md#actionmanager)
- [alphaIndex](AbstractMesh.md#alphaindex)
- [alwaysSelectAsActiveMesh](AbstractMesh.md#alwaysselectasactivemesh)
- [animations](AbstractMesh.md#animations)
- [cullingStrategy](AbstractMesh.md#cullingstrategy)
- [definedFacingForward](AbstractMesh.md#definedfacingforward)
- [doNotSyncBoundingInfo](AbstractMesh.md#donotsyncboundinginfo)
- [edgesColor](AbstractMesh.md#edgescolor)
- [edgesRenderer](AbstractMesh.md#edgesrenderer)
- [edgesWidth](AbstractMesh.md#edgeswidth)
- [ellipsoid](AbstractMesh.md#ellipsoid)
- [ellipsoidOffset](AbstractMesh.md#ellipsoidoffset)
- [enablePointerMoveEvents](AbstractMesh.md#enablepointermoveevents)
- [forceRenderingWhenOccluded](AbstractMesh.md#forcerenderingwhenoccluded)
- [id](AbstractMesh.md#id)
- [ignoreNonUniformScaling](AbstractMesh.md#ignorenonuniformscaling)
- [inspectableCustomProperties](AbstractMesh.md#inspectablecustomproperties)
- [instancedBuffers](AbstractMesh.md#instancedbuffers)
- [isBlocker](AbstractMesh.md#isblocker)
- [isNearGrabbable](AbstractMesh.md#isneargrabbable)
- [isNearPickable](AbstractMesh.md#isnearpickable)
- [isOccluded](AbstractMesh.md#isoccluded)
- [isOcclusionQueryInProgress](AbstractMesh.md#isocclusionqueryinprogress)
- [isPickable](AbstractMesh.md#ispickable)
- [isVisible](AbstractMesh.md#isvisible)
- [metadata](AbstractMesh.md#metadata)
- [name](AbstractMesh.md#name)
- [occlusionQueryAlgorithmType](AbstractMesh.md#occlusionqueryalgorithmtype)
- [occlusionRetryCount](AbstractMesh.md#occlusionretrycount)
- [occlusionType](AbstractMesh.md#occlusiontype)
- [onAfterWorldMatrixUpdateObservable](AbstractMesh.md#onafterworldmatrixupdateobservable)
- [onCollideObservable](AbstractMesh.md#oncollideobservable)
- [onCollisionPositionChangeObservable](AbstractMesh.md#oncollisionpositionchangeobservable)
- [onDisposeObservable](AbstractMesh.md#ondisposeobservable)
- [onMaterialChangedObservable](AbstractMesh.md#onmaterialchangedobservable)
- [onReady](AbstractMesh.md#onready)
- [onRebuildObservable](AbstractMesh.md#onrebuildobservable)
- [outlineColor](AbstractMesh.md#outlinecolor)
- [outlineWidth](AbstractMesh.md#outlinewidth)
- [overlayAlpha](AbstractMesh.md#overlayalpha)
- [overlayColor](AbstractMesh.md#overlaycolor)
- [physicsImpostor](AbstractMesh.md#physicsimpostor)
- [reIntegrateRotationIntoRotationQuaternion](AbstractMesh.md#reintegraterotationintorotationquaternion)
- [renderOutline](AbstractMesh.md#renderoutline)
- [renderOverlay](AbstractMesh.md#renderoverlay)
- [reservedDataStore](AbstractMesh.md#reserveddatastore)
- [scalingDeterminant](AbstractMesh.md#scalingdeterminant)
- [showBoundingBox](AbstractMesh.md#showboundingbox)
- [showSubMeshesBoundingBox](AbstractMesh.md#showsubmeshesboundingbox)
- [state](AbstractMesh.md#state)
- [subMeshes](AbstractMesh.md#submeshes)
- [uniqueId](AbstractMesh.md#uniqueid)
- [useOctreeForCollisions](AbstractMesh.md#useoctreeforcollisions)
- [useOctreeForPicking](AbstractMesh.md#useoctreeforpicking)
- [useOctreeForRenderingSelection](AbstractMesh.md#useoctreeforrenderingselection)
- [CULLINGSTRATEGY\_BOUNDINGSPHERE\_ONLY](AbstractMesh.md#cullingstrategy_boundingsphere_only)
- [CULLINGSTRATEGY\_OPTIMISTIC\_INCLUSION](AbstractMesh.md#cullingstrategy_optimistic_inclusion)
- [CULLINGSTRATEGY\_OPTIMISTIC\_INCLUSION\_THEN\_BSPHERE\_ONLY](AbstractMesh.md#cullingstrategy_optimistic_inclusion_then_bsphere_only)
- [CULLINGSTRATEGY\_STANDARD](AbstractMesh.md#cullingstrategy_standard)
- [OCCLUSION\_ALGORITHM\_TYPE\_ACCURATE](AbstractMesh.md#occlusion_algorithm_type_accurate)
- [OCCLUSION\_ALGORITHM\_TYPE\_CONSERVATIVE](AbstractMesh.md#occlusion_algorithm_type_conservative)
- [OCCLUSION\_TYPE\_NONE](AbstractMesh.md#occlusion_type_none)
- [OCCLUSION\_TYPE\_OPTIMISTIC](AbstractMesh.md#occlusion_type_optimistic)
- [OCCLUSION\_TYPE\_STRICT](AbstractMesh.md#occlusion_type_strict)

### Accessors

- [absolutePosition](AbstractMesh.md#absoluteposition)
- [absoluteRotationQuaternion](AbstractMesh.md#absoluterotationquaternion)
- [absoluteScaling](AbstractMesh.md#absolutescaling)
- [animationPropertiesOverride](AbstractMesh.md#animationpropertiesoverride)
- [applyFog](AbstractMesh.md#applyfog)
- [bakedVertexAnimationManager](AbstractMesh.md#bakedvertexanimationmanager)
- [behaviors](AbstractMesh.md#behaviors)
- [billboardMode](AbstractMesh.md#billboardmode)
- [checkCollisions](AbstractMesh.md#checkcollisions)
- [collider](AbstractMesh.md#collider)
- [collisionGroup](AbstractMesh.md#collisiongroup)
- [collisionMask](AbstractMesh.md#collisionmask)
- [collisionResponse](AbstractMesh.md#collisionresponse)
- [collisionRetryCount](AbstractMesh.md#collisionretrycount)
- [computeBonesUsingShaders](AbstractMesh.md#computebonesusingshaders)
- [doNotSerialize](AbstractMesh.md#donotserialize)
- [enableDistantPicking](AbstractMesh.md#enabledistantpicking)
- [facetDepthSortFrom](AbstractMesh.md#facetdepthsortfrom)
- [facetNb](AbstractMesh.md#facetnb)
- [forward](AbstractMesh.md#forward)
- [hasBoundingInfo](AbstractMesh.md#hasboundinginfo)
- [hasInstances](AbstractMesh.md#hasinstances)
- [hasThinInstances](AbstractMesh.md#hasthininstances)
- [hasVertexAlpha](AbstractMesh.md#hasvertexalpha)
- [infiniteDistance](AbstractMesh.md#infinitedistance)
- [isAnInstance](AbstractMesh.md#isaninstance)
- [isBlocked](AbstractMesh.md#isblocked)
- [isFacetDataEnabled](AbstractMesh.md#isfacetdataenabled)
- [isWorldMatrixFrozen](AbstractMesh.md#isworldmatrixfrozen)
- [layerMask](AbstractMesh.md#layermask)
- [lightSources](AbstractMesh.md#lightsources)
- [material](AbstractMesh.md#material)
- [morphTargetManager](AbstractMesh.md#morphtargetmanager)
- [mustDepthSortFacets](AbstractMesh.md#mustdepthsortfacets)
- [nonUniformScaling](AbstractMesh.md#nonuniformscaling)
- [numBoneInfluencers](AbstractMesh.md#numboneinfluencers)
- [onClonedObservable](AbstractMesh.md#onclonedobservable)
- [onCollide](AbstractMesh.md#oncollide)
- [onCollisionPositionChange](AbstractMesh.md#oncollisionpositionchange)
- [onDispose](AbstractMesh.md#ondispose)
- [onEnabledStateChangedObservable](AbstractMesh.md#onenabledstatechangedobservable)
- [parent](AbstractMesh.md#parent)
- [partitioningBBoxRatio](AbstractMesh.md#partitioningbboxratio)
- [partitioningSubdivisions](AbstractMesh.md#partitioningsubdivisions)
- [position](AbstractMesh.md#position)
- [preserveParentRotationForBillboard](AbstractMesh.md#preserveparentrotationforbillboard)
- [receiveShadows](AbstractMesh.md#receiveshadows)
- [renderingGroupId](AbstractMesh.md#renderinggroupid)
- [right](AbstractMesh.md#right)
- [rotation](AbstractMesh.md#rotation)
- [rotationQuaternion](AbstractMesh.md#rotationquaternion)
- [scaling](AbstractMesh.md#scaling)
- [skeleton](AbstractMesh.md#skeleton)
- [surroundingMeshes](AbstractMesh.md#surroundingmeshes)
- [up](AbstractMesh.md#up)
- [useBones](AbstractMesh.md#usebones)
- [useVertexColors](AbstractMesh.md#usevertexcolors)
- [visibility](AbstractMesh.md#visibility)
- [worldMatrixFromCache](AbstractMesh.md#worldmatrixfromcache)
- [BILLBOARDMODE\_ALL](AbstractMesh.md#billboardmode_all)
- [BILLBOARDMODE\_NONE](AbstractMesh.md#billboardmode_none)
- [BILLBOARDMODE\_USE\_POSITION](AbstractMesh.md#billboardmode_use_position)
- [BILLBOARDMODE\_X](AbstractMesh.md#billboardmode_x)
- [BILLBOARDMODE\_Y](AbstractMesh.md#billboardmode_y)
- [BILLBOARDMODE\_Z](AbstractMesh.md#billboardmode_z)

### Methods

- [\_buildUniformLayout](AbstractMesh.md#_builduniformlayout)
- [\_getData](AbstractMesh.md#_getdata)
- [\_markSubMeshesAsDirty](AbstractMesh.md#_marksubmeshesasdirty)
- [\_onCollisionPositionChange](AbstractMesh.md#_oncollisionpositionchange)
- [addBehavior](AbstractMesh.md#addbehavior)
- [addChild](AbstractMesh.md#addchild)
- [addRotation](AbstractMesh.md#addrotation)
- [alignWithNormal](AbstractMesh.md#alignwithnormal)
- [applyImpulse](AbstractMesh.md#applyimpulse)
- [attachToBone](AbstractMesh.md#attachtobone)
- [beginAnimation](AbstractMesh.md#beginanimation)
- [buildBoundingInfo](AbstractMesh.md#buildboundinginfo)
- [calcMovePOV](AbstractMesh.md#calcmovepov)
- [calcRotatePOV](AbstractMesh.md#calcrotatepov)
- [clone](AbstractMesh.md#clone)
- [computeWorldMatrix](AbstractMesh.md#computeworldmatrix)
- [createAnimationRange](AbstractMesh.md#createanimationrange)
- [createNormals](AbstractMesh.md#createnormals)
- [createOrUpdateSubmeshesOctree](AbstractMesh.md#createorupdatesubmeshesoctree)
- [deleteAnimationRange](AbstractMesh.md#deleteanimationrange)
- [detachFromBone](AbstractMesh.md#detachfrombone)
- [disableEdgesRendering](AbstractMesh.md#disableedgesrendering)
- [disableFacetData](AbstractMesh.md#disablefacetdata)
- [dispose](AbstractMesh.md#dispose)
- [enableEdgesRendering](AbstractMesh.md#enableedgesrendering)
- [freezeWorldMatrix](AbstractMesh.md#freezeworldmatrix)
- [getAbsolutePivotPoint](AbstractMesh.md#getabsolutepivotpoint)
- [getAbsolutePivotPointToRef](AbstractMesh.md#getabsolutepivotpointtoref)
- [getAbsolutePosition](AbstractMesh.md#getabsoluteposition)
- [getAnimationByName](AbstractMesh.md#getanimationbyname)
- [getAnimationRange](AbstractMesh.md#getanimationrange)
- [getAnimationRanges](AbstractMesh.md#getanimationranges)
- [getBehaviorByName](AbstractMesh.md#getbehaviorbyname)
- [getBoundingInfo](AbstractMesh.md#getboundinginfo)
- [getChildMeshes](AbstractMesh.md#getchildmeshes)
- [getChildTransformNodes](AbstractMesh.md#getchildtransformnodes)
- [getChildren](AbstractMesh.md#getchildren)
- [getClassName](AbstractMesh.md#getclassname)
- [getClosestFacetAtCoordinates](AbstractMesh.md#getclosestfacetatcoordinates)
- [getClosestFacetAtLocalCoordinates](AbstractMesh.md#getclosestfacetatlocalcoordinates)
- [getConnectedParticleSystems](AbstractMesh.md#getconnectedparticlesystems)
- [getDescendants](AbstractMesh.md#getdescendants)
- [getDirection](AbstractMesh.md#getdirection)
- [getDirectionToRef](AbstractMesh.md#getdirectiontoref)
- [getDistanceToCamera](AbstractMesh.md#getdistancetocamera)
- [getEngine](AbstractMesh.md#getengine)
- [getFacetDataParameters](AbstractMesh.md#getfacetdataparameters)
- [getFacetLocalNormals](AbstractMesh.md#getfacetlocalnormals)
- [getFacetLocalPartitioning](AbstractMesh.md#getfacetlocalpartitioning)
- [getFacetLocalPositions](AbstractMesh.md#getfacetlocalpositions)
- [getFacetNormal](AbstractMesh.md#getfacetnormal)
- [getFacetNormalToRef](AbstractMesh.md#getfacetnormaltoref)
- [getFacetPosition](AbstractMesh.md#getfacetposition)
- [getFacetPositionToRef](AbstractMesh.md#getfacetpositiontoref)
- [getFacetsAtLocalCoordinates](AbstractMesh.md#getfacetsatlocalcoordinates)
- [getHierarchyBoundingVectors](AbstractMesh.md#gethierarchyboundingvectors)
- [getIndices](AbstractMesh.md#getindices)
- [getLOD](AbstractMesh.md#getlod)
- [getMaterialForRenderPass](AbstractMesh.md#getmaterialforrenderpass)
- [getMeshUniformBuffer](AbstractMesh.md#getmeshuniformbuffer)
- [getNormalsData](AbstractMesh.md#getnormalsdata)
- [getPhysicsImpostor](AbstractMesh.md#getphysicsimpostor)
- [getPivotMatrix](AbstractMesh.md#getpivotmatrix)
- [getPivotPoint](AbstractMesh.md#getpivotpoint)
- [getPivotPointToRef](AbstractMesh.md#getpivotpointtoref)
- [getPoseMatrix](AbstractMesh.md#getposematrix)
- [getPositionData](AbstractMesh.md#getpositiondata)
- [getPositionExpressedInLocalSpace](AbstractMesh.md#getpositionexpressedinlocalspace)
- [getPositionInCameraSpace](AbstractMesh.md#getpositionincameraspace)
- [getScene](AbstractMesh.md#getscene)
- [getTotalIndices](AbstractMesh.md#gettotalindices)
- [getTotalVertices](AbstractMesh.md#gettotalvertices)
- [getVerticesData](AbstractMesh.md#getverticesdata)
- [getWorldMatrix](AbstractMesh.md#getworldmatrix)
- [instantiateHierarchy](AbstractMesh.md#instantiatehierarchy)
- [intersects](AbstractMesh.md#intersects)
- [intersectsMesh](AbstractMesh.md#intersectsmesh)
- [intersectsPoint](AbstractMesh.md#intersectspoint)
- [isCompletelyInFrustum](AbstractMesh.md#iscompletelyinfrustum)
- [isDescendantOf](AbstractMesh.md#isdescendantof)
- [isDisposed](AbstractMesh.md#isdisposed)
- [isEnabled](AbstractMesh.md#isenabled)
- [isInFrustum](AbstractMesh.md#isinfrustum)
- [isReady](AbstractMesh.md#isready)
- [isUsingPivotMatrix](AbstractMesh.md#isusingpivotmatrix)
- [isVerticesDataPresent](AbstractMesh.md#isverticesdatapresent)
- [locallyTranslate](AbstractMesh.md#locallytranslate)
- [lookAt](AbstractMesh.md#lookat)
- [markAsDirty](AbstractMesh.md#markasdirty)
- [movePOV](AbstractMesh.md#movepov)
- [moveWithCollisions](AbstractMesh.md#movewithcollisions)
- [normalizeToUnitCube](AbstractMesh.md#normalizetounitcube)
- [refreshBoundingInfo](AbstractMesh.md#refreshboundinginfo)
- [registerAfterWorldMatrixUpdate](AbstractMesh.md#registerafterworldmatrixupdate)
- [releaseSubMeshes](AbstractMesh.md#releasesubmeshes)
- [removeBehavior](AbstractMesh.md#removebehavior)
- [removeChild](AbstractMesh.md#removechild)
- [resetDrawCache](AbstractMesh.md#resetdrawcache)
- [resetLocalMatrix](AbstractMesh.md#resetlocalmatrix)
- [rotate](AbstractMesh.md#rotate)
- [rotateAround](AbstractMesh.md#rotatearound)
- [rotatePOV](AbstractMesh.md#rotatepov)
- [serialize](AbstractMesh.md#serialize)
- [serializeAnimationRanges](AbstractMesh.md#serializeanimationranges)
- [setAbsolutePosition](AbstractMesh.md#setabsoluteposition)
- [setBoundingInfo](AbstractMesh.md#setboundinginfo)
- [setDirection](AbstractMesh.md#setdirection)
- [setEnabled](AbstractMesh.md#setenabled)
- [setIndices](AbstractMesh.md#setindices)
- [setMaterialForRenderPass](AbstractMesh.md#setmaterialforrenderpass)
- [setParent](AbstractMesh.md#setparent)
- [setPhysicsLinkWith](AbstractMesh.md#setphysicslinkwith)
- [setPivotMatrix](AbstractMesh.md#setpivotmatrix)
- [setPivotPoint](AbstractMesh.md#setpivotpoint)
- [setPositionWithLocalVector](AbstractMesh.md#setpositionwithlocalvector)
- [setPreTransformMatrix](AbstractMesh.md#setpretransformmatrix)
- [setVerticesData](AbstractMesh.md#setverticesdata)
- [toString](AbstractMesh.md#tostring)
- [transferToEffect](AbstractMesh.md#transfertoeffect)
- [translate](AbstractMesh.md#translate)
- [unfreezeWorldMatrix](AbstractMesh.md#unfreezeworldmatrix)
- [unregisterAfterWorldMatrixUpdate](AbstractMesh.md#unregisterafterworldmatrixupdate)
- [updateFacetData](AbstractMesh.md#updatefacetdata)
- [updateIndices](AbstractMesh.md#updateindices)
- [updatePoseMatrix](AbstractMesh.md#updateposematrix)
- [updateVerticesData](AbstractMesh.md#updateverticesdata)
- [AddNodeConstructor](AbstractMesh.md#addnodeconstructor)
- [Construct](AbstractMesh.md#construct)
- [Parse](AbstractMesh.md#parse)
- [ParseAnimationRanges](AbstractMesh.md#parseanimationranges)

## Constructors

### constructor

• **new AbstractMesh**(`name`, `scene?`)

Creates a new AbstractMesh

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | defines the name of the mesh |
| `scene` | [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) | `null` | defines the hosting scene |

#### Overrides

[TransformNode](TransformNode.md).[constructor](TransformNode.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:822

## Properties

### \_boundingInfo

• `Protected` **\_boundingInfo**: [`Nullable`](../modules.md#nullable)[`BoundingInfo`](BoundingInfo.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:729

___

### \_boundingInfoIsDirty

• `Protected` **\_boundingInfoIsDirty**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:730

___

### \_isDirty

• `Protected` **\_isDirty**: `boolean` = `false`

#### Inherited from

[TransformNode](TransformNode.md).[_isDirty](TransformNode.md#_isdirty)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:43

___

### \_isWorldMatrixFrozen

• `Protected` **\_isWorldMatrixFrozen**: `boolean` = `false`

#### Inherited from

[TransformNode](TransformNode.md).[_isWorldMatrixFrozen](TransformNode.md#_isworldmatrixfrozen)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:161

___

### \_parentNode

• `Protected` **\_parentNode**: [`Nullable`](../modules.md#nullable)[`Node`](Node.md) = `null`

#### Inherited from

[TransformNode](TransformNode.md).[_parentNode](TransformNode.md#_parentnode)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:176

___

### \_ranges

• `Protected` **\_ranges**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: [`Nullable`](../modules.md#nullable)`AnimationRange`

#### Inherited from

[TransformNode](TransformNode.md).[_ranges](TransformNode.md#_ranges)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:154

___

### \_scaling

• `Protected` **\_scaling**: [`Vector3`](Vector3.md)

#### Inherited from

[TransformNode](TransformNode.md).[_scaling](TransformNode.md#_scaling)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:62

___

### actionManager

• **actionManager**: [`Nullable`](../modules.md#nullable)[`AbstractActionManager`](AbstractActionManager.md) = `null`

Gets or sets the current action manager

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:646

___

### alphaIndex

• **alphaIndex**: `number` = `Number.MAX_VALUE`

Gets or sets the alpha index used to sort transparent meshes

**`See`**

https://doc.babylonjs.com/resources/transparency_and_how_meshes_are_rendered#alpha-index

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:406

___

### alwaysSelectAsActiveMesh

• **alwaysSelectAsActiveMesh**: `boolean` = `false`

True if the mesh must be rendered in any case (this will shortcut the frustum clipping phase)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:635

___

### animations

• **animations**: [`Animation`](Animation.md)[]

Gets a list of Animations associated with the node

#### Inherited from

[TransformNode](TransformNode.md).[animations](TransformNode.md#animations)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:153

___

### cullingStrategy

• **cullingStrategy**: `number` = `AbstractMesh.CULLINGSTRATEGY_BOUNDINGSPHERE_ONLY`

The culling strategy to use to check whether the mesh must be rendered or not.
This value can be changed at any time and will be used on the next render mesh selection.
The possible values are :
- AbstractMesh.CULLINGSTRATEGY_STANDARD
- AbstractMesh.CULLINGSTRATEGY_BOUNDINGSPHERE_ONLY
- AbstractMesh.CULLINGSTRATEGY_OPTIMISTIC_INCLUSION
- AbstractMesh.CULLINGSTRATEGY_OPTIMISTIC_INCLUSION_THEN_BSPHERE_ONLY
Please read each static variable documentation to get details about the culling process.

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:214

___

### definedFacingForward

• **definedFacingForward**: `boolean` = `true`

Gets or sets the orientation for POV movement & rotation

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:371

___

### doNotSyncBoundingInfo

• **doNotSyncBoundingInfo**: `boolean` = `false`

Gets or sets a boolean indicating that the bounding info does not need to be kept in sync (for performance reason)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:640

___

### edgesColor

• **edgesColor**: [`Color4`](Color4.md)

Defines edge color used when edgesRenderer is enabled

**`See`**

https://www.babylonjs-playground.com/#10OJSG#13

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:723

___

### edgesRenderer

• **edgesRenderer**: [`Nullable`](../modules.md#nullable)[`EdgesRenderer`](EdgesRenderer.md)

Gets the edgesRenderer associated with the mesh

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:35

___

### edgesWidth

• **edgesWidth**: `number` = `1`

Defines edge width used when edgesRenderer is enabled

**`See`**

https://www.babylonjs-playground.com/#10OJSG#13

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:718

___

### ellipsoid

• **ellipsoid**: [`Vector3`](Vector3.md)

Gets or sets the ellipsoid used to impersonate this mesh when using collision engine (default is (0.5, 1, 0.5))

**`See`**

https://doc.babylonjs.com/babylon101/cameras,_mesh_collisions_and_gravity

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:652

___

### ellipsoidOffset

• **ellipsoidOffset**: [`Vector3`](Vector3.md)

Gets or sets the ellipsoid offset used to impersonate this mesh when using collision engine (default is (0, 0, 0))

**`See`**

https://doc.babylonjs.com/babylon101/cameras,_mesh_collisions_and_gravity

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:657

___

### enablePointerMoveEvents

• **enablePointerMoveEvents**: `boolean` = `false`

Gets or sets a boolean indicating that pointer move events must be supported on this mesh (false by default)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:439

___

### forceRenderingWhenOccluded

• **forceRenderingWhenOccluded**: `boolean`

Flag to force rendering the mesh even if occluded

**`See`**

https://doc.babylonjs.com/features/occlusionquery

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.query.ts:405

___

### id

• **id**: `string`

Gets or sets the id of the node

#### Inherited from

[TransformNode](TransformNode.md).[id](TransformNode.md#id)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:97

___

### ignoreNonUniformScaling

• **ignoreNonUniformScaling**: `boolean` = `false`

Gets or sets a boolean indicating that non uniform scaling (when at least one component is different from others) should be ignored.
By default the system will update normals to compensate

#### Inherited from

[TransformNode](TransformNode.md).[ignoreNonUniformScaling](TransformNode.md#ignorenonuniformscaling)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:138

___

### inspectableCustomProperties

• **inspectableCustomProperties**: [`IInspectable`](../interfaces/IInspectable.md)[]

List of inspectable custom properties (used by the Inspector)

**`See`**

https://doc.babylonjs.com/how_to/debug_layer#extensibility

#### Inherited from

[TransformNode](TransformNode.md).[inspectableCustomProperties](TransformNode.md#inspectablecustomproperties)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:126

___

### instancedBuffers

• **instancedBuffers**: `Object`

Object used to store instanced buffers defined by user

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_instances#custom-buffers

#### Index signature

▪ [key: `string`]: `any`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/instancedMesh.ts:594

___

### isBlocker

• **isBlocker**: `boolean` = `false`

Gets or sets a boolean indicating if the mesh must be considered as a ray blocker for lens flares (false by default)

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_lens_flares

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:434

___

### isNearGrabbable

• **isNearGrabbable**: `boolean` = `false`

Gets or sets a boolean indicating if the mesh can be near grabbed. Default is false

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:426

___

### isNearPickable

• **isNearPickable**: `boolean` = `false`

Gets or sets a boolean indicating if the mesh can be near picked. Default is false

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:421

___

### isOccluded

• **isOccluded**: `boolean`

Gets or sets whether the mesh is occluded or not, it is used also to set the initial state of the mesh to be occluded or not

**`See`**

https://doc.babylonjs.com/features/occlusionquery

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.query.ts:393

___

### isOcclusionQueryInProgress

• **isOcclusionQueryInProgress**: `boolean`

Flag to check the progress status of the query

**`See`**

https://doc.babylonjs.com/features/occlusionquery

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.query.ts:399

___

### isPickable

• **isPickable**: `boolean` = `true`

Gets or sets a boolean indicating if the mesh can be picked (by scene.pick for instance or through actions). Default is true

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:416

___

### isVisible

• **isVisible**: `boolean` = `true`

Gets or sets a boolean indicating if the mesh is visible (renderable). Default is true

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:411

___

### metadata

• **metadata**: `any` = `null`

Gets or sets an object used to store user defined information for the node

#### Inherited from

[TransformNode](TransformNode.md).[metadata](TransformNode.md#metadata)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:115

___

### name

• **name**: `string`

Gets or sets the name of the node

#### Inherited from

[TransformNode](TransformNode.md).[name](TransformNode.md#name)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:91

___

### occlusionQueryAlgorithmType

• **occlusionQueryAlgorithmType**: `number`

This property determines the type of occlusion query algorithm to run in WebGl, you can use:
* AbstractMesh.OCCLUSION_ALGORITHM_TYPE_ACCURATE which is mapped to GL_ANY_SAMPLES_PASSED.
* AbstractMesh.OCCLUSION_ALGORITHM_TYPE_CONSERVATIVE (Default Value) which is mapped to GL_ANY_SAMPLES_PASSED_CONSERVATIVE which is a false positive algorithm that is faster than GL_ANY_SAMPLES_PASSED but less accurate.

**`See`**

https://doc.babylonjs.com/features/occlusionquery

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.query.ts:387

___

### occlusionRetryCount

• **occlusionRetryCount**: `number`

This number indicates the number of allowed retries before stop the occlusion query, this is useful if the occlusion query is taking long time before to the query result is retrieved, the query result indicates if the object is visible within the scene or not and based on that Babylon.Js engine decides to show or hide the object.
The default value is -1 which means don't break the query and wait till the result

**`See`**

https://doc.babylonjs.com/features/occlusionquery

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.query.ts:370

___

### occlusionType

• **occlusionType**: `number`

This property is responsible for starting the occlusion query within the Mesh or not, this property is also used to determine what should happen when the occlusionRetryCount is reached. It has supports 3 values:
* OCCLUSION_TYPE_NONE (Default Value): this option means no occlusion query within the Mesh.
* OCCLUSION_TYPE_OPTIMISTIC: this option is means use occlusion query and if occlusionRetryCount is reached and the query is broken show the mesh.
* OCCLUSION_TYPE_STRICT: this option is means use occlusion query and if occlusionRetryCount is reached and the query is broken restore the last state of the mesh occlusion if the mesh was visible then show the mesh if was hidden then hide don't show.

**`See`**

https://doc.babylonjs.com/features/occlusionquery

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.query.ts:379

___

### onAfterWorldMatrixUpdateObservable

• **onAfterWorldMatrixUpdateObservable**: [`Observable`](Observable.md)[`TransformNode`](TransformNode.md)

An event triggered after the world matrix is updated

#### Inherited from

[TransformNode](TransformNode.md).[onAfterWorldMatrixUpdateObservable](TransformNode.md#onafterworldmatrixupdateobservable)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:169

___

### onCollideObservable

• **onCollideObservable**: [`Observable`](Observable.md)[`AbstractMesh`](AbstractMesh.md)

An event triggered when this mesh collides with another one

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:338

___

### onCollisionPositionChangeObservable

• **onCollisionPositionChangeObservable**: [`Observable`](Observable.md)[`Vector3`](Vector3.md)

An event triggered when the collision's position changes

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:351

___

### onDisposeObservable

• **onDisposeObservable**: [`Observable`](Observable.md)[`Node`](Node.md)

An event triggered when the mesh is disposed

#### Inherited from

[TransformNode](TransformNode.md).[onDisposeObservable](TransformNode.md#ondisposeobservable)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:300

___

### onMaterialChangedObservable

• **onMaterialChangedObservable**: [`Observable`](Observable.md)[`AbstractMesh`](AbstractMesh.md)

An event triggered when material is changed

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:364

___

### onReady

• **onReady**: [`Nullable`](../modules.md#nullable)(`node`: [`Node`](Node.md)) => `void` = `null`

Callback raised when the node is ready to be used

#### Inherited from

[TransformNode](TransformNode.md).[onReady](TransformNode.md#onready)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:159

___

### onRebuildObservable

• **onRebuildObservable**: [`Observable`](Observable.md)[`AbstractMesh`](AbstractMesh.md)

An event triggered when the mesh is rebuilt.

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:807

___

### outlineColor

• **outlineColor**: [`Color3`](Color3.md)

Defines color to use when rendering outline

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:524

___

### outlineWidth

• **outlineWidth**: `number` = `0.02`

Define width to use when rendering outline

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:526

___

### overlayAlpha

• **overlayAlpha**: `number` = `0.5`

Defines alpha to use when rendering overlay

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:531

___

### overlayColor

• **overlayColor**: [`Color3`](Color3.md)

Defines color to use when rendering overlay

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:529

___

### physicsImpostor

• **physicsImpostor**: [`Nullable`](../modules.md#nullable)[`PhysicsImpostor`](PhysicsImpostor.md)

Gets or sets impostor used for physic simulation

**`See`**

https://doc.babylonjs.com/features/physics_engine

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsEngineComponent.ts:169

___

### reIntegrateRotationIntoRotationQuaternion

• **reIntegrateRotationIntoRotationQuaternion**: `boolean` = `false`

Gets or sets a boolean indicating that even if rotationQuaternion is defined, you can keep updating rotation property and Babylon.js will just mix both

#### Inherited from

[TransformNode](TransformNode.md).[reIntegrateRotationIntoRotationQuaternion](TransformNode.md#reintegraterotationintorotationquaternion)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:144

___

### renderOutline

• **renderOutline**: `boolean`

Gets or sets a boolean indicating if the outline must be rendered as well

**`See`**

https://www.babylonjs-playground.com/#10WJ5S#3

#### Defined in

https://github.com/babylon.js/core/src/Rendering/outlineRenderer.ts:48

___

### renderOverlay

• **renderOverlay**: `boolean`

Gets or sets a boolean indicating if the overlay must be rendered as well

**`See`**

https://www.babylonjs-playground.com/#10WJ5S#2

#### Defined in

https://github.com/babylon.js/core/src/Rendering/outlineRenderer.ts:56

___

### reservedDataStore

• **reservedDataStore**: `any` = `null`

For internal use only. Please do not use.

#### Inherited from

[TransformNode](TransformNode.md).[reservedDataStore](TransformNode.md#reserveddatastore)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:120

___

### scalingDeterminant

• **scalingDeterminant**: `number` = `1`

Multiplication factor on scale x/y/z when computing the world matrix. Eg. for a 1x1x1 cube setting this to 2 will make it a 2x2x2 cube

#### Inherited from

[TransformNode](TransformNode.md).[scalingDeterminant](TransformNode.md#scalingdeterminant)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:113

___

### showBoundingBox

• **showBoundingBox**: `boolean`

Gets or sets a boolean indicating if the bounding box must be rendered as well (false by default)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/boundingBoxRenderer.ts:76

___

### showSubMeshesBoundingBox

• **showSubMeshesBoundingBox**: `boolean` = `false`

Gets or sets a boolean indicating that bounding boxes of subMeshes must be rendered as well (false by default)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:429

___

### state

• **state**: `string` = `""`

Gets or sets a string used to store user defined state for the node

#### Inherited from

[TransformNode](TransformNode.md).[state](TransformNode.md#state)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:109

___

### subMeshes

• **subMeshes**: [`SubMesh`](SubMesh.md)[]

Gets or sets the list of subMeshes

**`See`**

https://doc.babylonjs.com/how_to/multi_materials

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:738

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the node

#### Inherited from

[TransformNode](TransformNode.md).[uniqueId](TransformNode.md#uniqueid)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:103

___

### useOctreeForCollisions

• **useOctreeForCollisions**: `boolean` = `true`

Gets or sets a boolean indicating that internal octree (if available) can be used to boost submeshes collision (true by default)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:614

___

### useOctreeForPicking

• **useOctreeForPicking**: `boolean` = `true`

Gets or sets a boolean indicating that internal octree (if available) can be used to boost submeshes picking (true by default)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:612

___

### useOctreeForRenderingSelection

• **useOctreeForRenderingSelection**: `boolean` = `true`

Gets or sets a boolean indicating that internal octree (if available) can be used to boost submeshes selection (true by default)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:610

___

### CULLINGSTRATEGY\_BOUNDINGSPHERE\_ONLY

▪ `Static` `Readonly` **CULLINGSTRATEGY\_BOUNDINGSPHERE\_ONLY**: ``1``

Culling strategy : Bounding Sphere Only.
 This is an exclusion test. It's faster than the standard strategy because the bounding box is not tested.
 It's also less accurate than the standard because some not visible objects can still be selected.
 Test : is the bounding sphere outside the frustum ?
 If not, then the cullable object is in the frustum.

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:143

___

### CULLINGSTRATEGY\_OPTIMISTIC\_INCLUSION

▪ `Static` `Readonly` **CULLINGSTRATEGY\_OPTIMISTIC\_INCLUSION**: ``2``

Culling strategy : Optimistic Inclusion.
 This in an inclusion test first, then the standard exclusion test.
 This can be faster when a cullable object is expected to be almost always in the camera frustum.
 This could also be a little slower than the standard test when the tested object center is not the frustum but one of its bounding box vertex is still inside.
 Anyway, it's as accurate as the standard strategy.
 Test :
 Is the cullable object bounding sphere center in the frustum ?
 If not, apply the default culling strategy.

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:153

___

### CULLINGSTRATEGY\_OPTIMISTIC\_INCLUSION\_THEN\_BSPHERE\_ONLY

▪ `Static` `Readonly` **CULLINGSTRATEGY\_OPTIMISTIC\_INCLUSION\_THEN\_BSPHERE\_ONLY**: ``3``

Culling strategy : Optimistic Inclusion then Bounding Sphere Only.
 This in an inclusion test first, then the bounding sphere only exclusion test.
 This can be the fastest test when a cullable object is expected to be almost always in the camera frustum.
 This could also be a little slower than the BoundingSphereOnly strategy when the tested object center is not in the frustum but its bounding sphere still intersects it.
 It's less accurate than the standard strategy and as accurate as the BoundingSphereOnly strategy.
 Test :
 Is the cullable object bounding sphere center in the frustum ?
 If not, apply the Bounding Sphere Only strategy. No Bounding Box is tested here.

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:163

___

### CULLINGSTRATEGY\_STANDARD

▪ `Static` `Readonly` **CULLINGSTRATEGY\_STANDARD**: ``0``

Default culling strategy : this is an exclusion test and it's the more accurate.
 Test order :
 Is the bounding sphere outside the frustum ?
 If not, are the bounding box vertices outside the frustum ?
 It not, then the cullable object is in the frustum.

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:136

___

### OCCLUSION\_ALGORITHM\_TYPE\_ACCURATE

▪ `Static` **OCCLUSION\_ALGORITHM\_TYPE\_ACCURATE**: `number` = `0`

Use an accurate occlusion algorithm

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:126

___

### OCCLUSION\_ALGORITHM\_TYPE\_CONSERVATIVE

▪ `Static` **OCCLUSION\_ALGORITHM\_TYPE\_CONSERVATIVE**: `number` = `1`

Use a conservative occlusion algorithm

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:128

___

### OCCLUSION\_TYPE\_NONE

▪ `Static` **OCCLUSION\_TYPE\_NONE**: `number` = `0`

No occlusion

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:120

___

### OCCLUSION\_TYPE\_OPTIMISTIC

▪ `Static` **OCCLUSION\_TYPE\_OPTIMISTIC**: `number` = `1`

Occlusion set to optimistic

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:122

___

### OCCLUSION\_TYPE\_STRICT

▪ `Static` **OCCLUSION\_TYPE\_STRICT**: `number` = `2`

Occlusion set to strict

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:124

## Accessors

### absolutePosition

• `get` **absolutePosition**(): [`Vector3`](Vector3.md)

Returns the current mesh absolute position.
Returns a Vector3.

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

TransformNode.absolutePosition

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:344

___

### absoluteRotationQuaternion

• `get` **absoluteRotationQuaternion**(): [`Quaternion`](Quaternion.md)

Returns the current mesh absolute rotation.
Returns a Quaternion.

#### Returns

[`Quaternion`](Quaternion.md)

#### Inherited from

TransformNode.absoluteRotationQuaternion

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:361

___

### absoluteScaling

• `get` **absoluteScaling**(): [`Vector3`](Vector3.md)

Returns the current mesh absolute scaling.
Returns a Vector3.

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

TransformNode.absoluteScaling

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:352

___

### animationPropertiesOverride

• `get` **animationPropertiesOverride**(): [`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md)

Gets or sets the animation properties override

#### Returns

[`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md)

#### Inherited from

TransformNode.animationPropertiesOverride

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

TransformNode.animationPropertiesOverride

#### Defined in

https://github.com/babylon.js/core/src/node.ts:282

___

### applyFog

• `get` **applyFog**(): `boolean`

Gets or sets a boolean indicating that this mesh will allow fog to be rendered on it (true by default)

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:589

• `set` **applyFog**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:592

___

### bakedVertexAnimationManager

• `get` **bakedVertexAnimationManager**(): [`Nullable`](../modules.md#nullable)[`IBakedVertexAnimationManager`](../interfaces/IBakedVertexAnimationManager.md)

Gets or sets the baked vertex animation manager

**`See`**

https://doc.babylonjs.com/divingDeeper/animation/baked_texture_animations

#### Returns

[`Nullable`](../modules.md#nullable)[`IBakedVertexAnimationManager`](../interfaces/IBakedVertexAnimationManager.md)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:306

• `set` **bakedVertexAnimationManager**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`IBakedVertexAnimationManager`](../interfaces/IBakedVertexAnimationManager.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:310

___

### behaviors

• `get` **behaviors**(): [`Behavior`](../interfaces/Behavior.md)[`Node`](Node.md)[]

Gets the list of attached behaviors

**`See`**

https://doc.babylonjs.com/features/behaviour

#### Returns

[`Behavior`](../interfaces/Behavior.md)[`Node`](Node.md)[]

#### Inherited from

TransformNode.behaviors

#### Defined in

https://github.com/babylon.js/core/src/node.ts:410

___

### billboardMode

• `get` **billboardMode**(): `number`

Gets or sets the billboard mode. Default is 0.

| Value | Type | Description |
| --- | --- | --- |
| 0 | BILLBOARDMODE_NONE |  |
| 1 | BILLBOARDMODE_X |  |
| 2 | BILLBOARDMODE_Y |  |
| 4 | BILLBOARDMODE_Z |  |
| 7 | BILLBOARDMODE_ALL |  |

#### Returns

`number`

#### Inherited from

TransformNode.billboardMode

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:82

• `set` **billboardMode**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

TransformNode.billboardMode

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:86

___

### checkCollisions

• `get` **checkCollisions**(): `boolean`

Gets or sets a boolean indicating that this mesh can be used in the collision engine

**`See`**

https://doc.babylonjs.com/babylon101/cameras,_mesh_collisions_and_gravity

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:1686

• `set` **checkCollisions**(`collisionEnabled`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `collisionEnabled` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:1690

___

### collider

• `get` **collider**(): [`Nullable`](../modules.md#nullable)`Collider`

Gets Collider object used to compute collisions (not physics)

**`See`**

https://doc.babylonjs.com/babylon101/cameras,_mesh_collisions_and_gravity

#### Returns

[`Nullable`](../modules.md#nullable)`Collider`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:1698

___

### collisionGroup

• `get` **collisionGroup**(): `number`

Gets or sets the current collision group mask (-1 by default).
A collision between A and B will happen if A.collisionGroup & b.collisionMask !== 0

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:688

• `set` **collisionGroup**(`mask`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `mask` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:692

___

### collisionMask

• `get` **collisionMask**(): `number`

Gets or sets a collision mask used to mask collisions (default is -1).
A collision between A and B will happen if A.collisionGroup & b.collisionMask !== 0

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:663

• `set` **collisionMask**(`mask`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `mask` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:667

___

### collisionResponse

• `get` **collisionResponse**(): `boolean`

Gets or sets a collision response flag (default is true).
when collisionResponse is false, events are still triggered but colliding entity has no response
This helps creating trigger volume when user wants collision feedback events but not position/velocity
to respond to the collision.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:677

• `set` **collisionResponse**(`response`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `response` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:681

___

### collisionRetryCount

• `get` **collisionRetryCount**(): `number`

number of collision detection tries. Change this value if not all collisions are detected and handled properly

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:272

• `set` **collisionRetryCount**(`retryCount`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `retryCount` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:275

___

### computeBonesUsingShaders

• `get` **computeBonesUsingShaders**(): `boolean`

Gets or sets a boolean indicating that bone animations must be computed by the CPU (false by default)

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:563

• `set` **computeBonesUsingShaders**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:566

___

### doNotSerialize

• `get` **doNotSerialize**(): `boolean`

Gets or sets a boolean used to define if the node must be serialized

#### Returns

`boolean`

#### Inherited from

TransformNode.doNotSerialize

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

TransformNode.doNotSerialize

#### Defined in

https://github.com/babylon.js/core/src/node.ts:143

___

### enableDistantPicking

• `get` **enableDistantPicking**(): `boolean`

When enabled, decompose picking matrices for better precision with large values for mesh position and scling

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:602

• `set` **enableDistantPicking**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:605

___

### facetDepthSortFrom

• `get` **facetDepthSortFrom**(): [`Vector3`](Vector3.md)

The location (Vector3) where the facet depth sort must be computed from.
By default, the active camera position.
Used only when facet depth sort is enabled

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_facetdata#facet-depth-sort

#### Returns

[`Vector3`](Vector3.md)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:264

• `set` **facetDepthSortFrom**(`location`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `location` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:267

___

### facetNb

• `get` **facetNb**(): `number`

Gets the number of facets in the mesh

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_facetdata#what-is-a-mesh-facet

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:220

___

### forward

• `get` **forward**(): [`Vector3`](Vector3.md)

The forward direction of that transform in world space.

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

TransformNode.forward

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:253

___

### hasBoundingInfo

• `get` **hasBoundingInfo**(): `boolean`

Returns true if there is already a bounding info

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:1230

___

### hasInstances

• `get` **hasInstances**(): `boolean`

Gets a boolean indicating if this mesh has instances

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:1334

___

### hasThinInstances

• `get` **hasThinInstances**(): `boolean`

Gets a boolean indicating if this mesh has thin instances

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:1341

___

### hasVertexAlpha

• `get` **hasVertexAlpha**(): `boolean`

Gets or sets a boolean indicating that this mesh contains vertex color data with alpha values

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:534

• `set` **hasVertexAlpha**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:537

___

### infiniteDistance

• `get` **infiniteDistance**(): `boolean`

Gets or sets the distance of the object to max, often used by skybox

#### Returns

`boolean`

#### Inherited from

TransformNode.infiniteDistance

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:121

• `set` **infiniteDistance**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

TransformNode.infiniteDistance

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:125

___

### isAnInstance

• `get` **isAnInstance**(): `boolean`

Gets a boolean indicating if this mesh is an instance or a regular mesh

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:1327

___

### isBlocked

• `get` **isBlocked**(): `boolean`

Returns true if the mesh is blocked. Implemented by child classes

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:1073

___

### isFacetDataEnabled

• `get` **isFacetDataEnabled**(): `boolean`

gets a boolean indicating if facetData is enabled

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_facetdata#what-is-a-mesh-facet

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:282

___

### isWorldMatrixFrozen

• `get` **isWorldMatrixFrozen**(): `boolean`

True if the World matrix has been frozen.

#### Returns

`boolean`

#### Inherited from

TransformNode.isWorldMatrixFrozen

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:476

___

### layerMask

• `get` **layerMask**(): `number`

Gets or sets the current layer mask (default is 0x0FFFFFFF)

**`See`**

https://doc.babylonjs.com/divingDeeper/cameras/layerMasksAndMultiCam

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:619

• `set` **layerMask**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:623

___

### lightSources

• `get` **lightSources**(): [`Light`](Light.md)[]

Gets the list of lights affecting that mesh

#### Returns

[`Light`](Light.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:750

___

### material

• `get` **material**(): [`Nullable`](../modules.md#nullable)[`Material`](Material.md)

Gets or sets current material

#### Returns

[`Nullable`](../modules.md#nullable)[`Material`](Material.md)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:454

• `set` **material**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`Material`](Material.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:457

___

### morphTargetManager

• `get` **morphTargetManager**(): [`Nullable`](../modules.md#nullable)[`MorphTargetManager`](MorphTargetManager.md)

Gets or sets the morph target manager

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_morphtargets

#### Returns

[`Nullable`](../modules.md#nullable)[`MorphTargetManager`](MorphTargetManager.md)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:290

• `set` **morphTargetManager**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`MorphTargetManager`](MorphTargetManager.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:294

___

### mustDepthSortFacets

• `get` **mustDepthSortFacets**(): `boolean`

Gets or sets a boolean indicating that the facets must be depth sorted on next call to `updateFacetData()`.
Works only for updatable meshes.
Doesn't work with multi-materials

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_facetdata#facet-depth-sort

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:251

• `set` **mustDepthSortFacets**(`sort`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `sort` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:254

___

### nonUniformScaling

• `get` **nonUniformScaling**(): `boolean`

True if the scaling property of this object is non uniform eg. (1,2,1)

#### Returns

`boolean`

#### Inherited from

TransformNode.nonUniformScaling

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:799

___

### numBoneInfluencers

• `get` **numBoneInfluencers**(): `number`

Gets or sets the number of allowed bone influences per vertex (4 by default)

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:576

• `set` **numBoneInfluencers**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:579

___

### onClonedObservable

• `get` **onClonedObservable**(): [`Observable`](Observable.md)[`Node`](Node.md)

An event triggered when the node is cloned

#### Returns

[`Observable`](Observable.md)[`Node`](Node.md)

#### Inherited from

TransformNode.onClonedObservable

#### Defined in

packages/dev/core/src/node.ts:323

___

### onCollide

• `set` **onCollide**(`callback`): `void`

Set a function to call when this mesh collides with another one

#### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | (`collidedMesh?`: [`AbstractMesh`](AbstractMesh.md)) => `void` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:341

___

### onCollisionPositionChange

• `set` **onCollisionPositionChange**(`callback`): `void`

Set a function to call when the collision's position changes

#### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | () => `void` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:354

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

TransformNode.onDispose

#### Defined in

packages/dev/core/src/node.ts:306

___

### onEnabledStateChangedObservable

• `get` **onEnabledStateChangedObservable**(): [`Observable`](Observable.md)`boolean`

An event triggered when the enabled state of the node changes

#### Returns

[`Observable`](Observable.md)`boolean`

#### Inherited from

TransformNode.onEnabledStateChangedObservable

#### Defined in

packages/dev/core/src/node.ts:316

___

### parent

• `get` **parent**(): [`Nullable`](../modules.md#nullable)[`Node`](Node.md)

#### Returns

[`Nullable`](../modules.md#nullable)[`Node`](Node.md)

#### Inherited from

TransformNode.parent

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

TransformNode.parent

#### Defined in

packages/dev/core/src/node.ts:200

___

### partitioningBBoxRatio

• `get` **partitioningBBoxRatio**(): `number`

The ratio (float) to apply to the bounding box size to set to the partitioning space.
Ex : 1.01 (default) the partitioning space is 1% bigger than the bounding box

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_facetdata#tweaking-the-partitioning

#### Returns

`number`

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:238

• `set` **partitioningBBoxRatio**(`ratio`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `ratio` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:241

___

### partitioningSubdivisions

• `get` **partitioningSubdivisions**(): `number`

Gets or set the number (integer) of subdivisions per axis in the partitioning space

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_facetdata#tweaking-the-partitioning

#### Returns

`number`

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:227

• `set` **partitioningSubdivisions**(`nb`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `nb` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:230

___

### position

• `get` **position**(): [`Vector3`](Vector3.md)

Gets or set the node position (default is (0.0, 0.0, 0.0))

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

TransformNode.position

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:190

• `set` **position**(`newPosition`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `newPosition` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Inherited from

TransformNode.position

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:194

___

### preserveParentRotationForBillboard

• `get` **preserveParentRotationForBillboard**(): `boolean`

Gets or sets a boolean indicating that parent rotation should be preserved when using billboards.
This could be useful for glTF objects where parent rotation helps converting from right handed to left handed

#### Returns

`boolean`

#### Inherited from

TransformNode.preserveParentRotationForBillboard

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:98

• `set` **preserveParentRotationForBillboard**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

TransformNode.preserveParentRotationForBillboard

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:102

___

### receiveShadows

• `get` **receiveShadows**(): `boolean`

Gets or sets a boolean indicating that this mesh can receive realtime shadows

**`See`**

https://doc.babylonjs.com/babylon101/shadows

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:511

• `set` **receiveShadows**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:514

___

### renderingGroupId

• `get` **renderingGroupId**(): `number`

Specifies the rendering group id for this mesh (0 by default)

**`See`**

https://doc.babylonjs.com/resources/transparency_and_how_meshes_are_rendered#rendering-groups

#### Returns

`number`

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:445

• `set` **renderingGroupId**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:449

___

### right

• `get` **right**(): [`Vector3`](Vector3.md)

The right direction of that transform in world space.

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

TransformNode.right

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:269

___

### rotation

• `get` **rotation**(): [`Vector3`](Vector3.md)

Gets or sets the rotation property : a Vector3 defining the rotation value in radians around each local axis X, Y, Z  (default is (0.0, 0.0, 0.0)).
If rotation quaternion is set, this Vector3 will be ignored and copy from the quaternion

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

TransformNode.rotation

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:211

• `set` **rotation**(`newRotation`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `newRotation` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Inherited from

TransformNode.rotation

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:215

___

### rotationQuaternion

• `get` **rotationQuaternion**(): [`Nullable`](../modules.md#nullable)[`Quaternion`](Quaternion.md)

Gets or sets the rotation Quaternion property : this a Quaternion object defining the node rotation by using a unit quaternion (undefined by default, but can be null).
If set, only the rotationQuaternion is then used to compute the node rotation (ie. node.rotation will be ignored)

#### Returns

[`Nullable`](../modules.md#nullable)[`Quaternion`](Quaternion.md)

#### Inherited from

TransformNode.rotationQuaternion

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:237

• `set` **rotationQuaternion**(`quaternion`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `quaternion` | [`Nullable`](../modules.md#nullable)[`Quaternion`](Quaternion.md) |

#### Returns

`void`

#### Inherited from

TransformNode.rotationQuaternion

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:241

___

### scaling

• `get` **scaling**(): [`Vector3`](Vector3.md)

Gets or sets the scaling property : a Vector3 defining the node scaling along each local axis X, Y, Z (default is (1.0, 1.0, 1.0)).

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

TransformNode.scaling

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:224

• `set` **scaling**(`newScaling`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `newScaling` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Inherited from

TransformNode.scaling

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:228

___

### skeleton

• `get` **skeleton**(): [`Nullable`](../modules.md#nullable)[`Skeleton`](Skeleton.md)

#### Returns

[`Nullable`](../modules.md#nullable)[`Skeleton`](Skeleton.md)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:800

• `set` **skeleton**(`value`): `void`

Gets or sets a skeleton to apply skinning transformations

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_bones_and_skeletons

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`Skeleton`](Skeleton.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:781

___

### surroundingMeshes

• `get` **surroundingMeshes**(): [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)[]

Gets or sets current surrounding meshes (null by default).

By default collision detection is tested against every mesh in the scene.
It is possible to set surroundingMeshes to a defined list of meshes and then only these specified
meshes will be tested for the collision.

Note: if set to an empty array no collision will happen when this mesh is moved.

#### Returns

[`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)[]

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:705

• `set` **surroundingMeshes**(`meshes`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `meshes` | [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)[] |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:709

___

### up

• `get` **up**(): [`Vector3`](Vector3.md)

The up direction of that transform in world space.

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

TransformNode.up

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:261

___

### useBones

• `get` **useBones**(): `boolean`

Gets a boolean indicating if this mesh has skinning data and an attached skeleton

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1258

___

### useVertexColors

• `get` **useVertexColors**(): `boolean`

Gets or sets a boolean indicating that this mesh needs to use vertex color data to render (if this kind of vertex data is available in the geometry)

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:548

• `set` **useVertexColors**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:551

___

### visibility

• `get` **visibility**(): `number`

Gets or sets mesh visibility between 0 and 1 (default is 1)

#### Returns

`number`

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:382

• `set` **visibility**(`value`): `void`

Gets or sets mesh visibility between 0 and 1 (default is 1)

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:389

___

### worldMatrixFromCache

• `get` **worldMatrixFromCache**(): [`Matrix`](Matrix.md)

Returns directly the latest state of the mesh World matrix.
A Matrix is returned.

#### Returns

[`Matrix`](Matrix.md)

#### Inherited from

TransformNode.worldMatrixFromCache

#### Defined in

packages/dev/core/src/node.ts:454

___

### BILLBOARDMODE\_ALL

• `Static` `get` **BILLBOARDMODE_ALL**(): `number`

Billboard on all axes

#### Returns

`number`

#### Overrides

TransformNode.BILLBOARDMODE\_ALL

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:188

___

### BILLBOARDMODE\_NONE

• `Static` `get` **BILLBOARDMODE_NONE**(): `number`

No billboard

#### Returns

`number`

#### Overrides

TransformNode.BILLBOARDMODE\_NONE

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:168

___

### BILLBOARDMODE\_USE\_POSITION

• `Static` `get` **BILLBOARDMODE_USE_POSITION**(): `number`

Billboard on using position instead of orientation

#### Returns

`number`

#### Overrides

TransformNode.BILLBOARDMODE\_USE\_POSITION

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:193

___

### BILLBOARDMODE\_X

• `Static` `get` **BILLBOARDMODE_X**(): `number`

Billboard on X axis

#### Returns

`number`

#### Overrides

TransformNode.BILLBOARDMODE\_X

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:173

___

### BILLBOARDMODE\_Y

• `Static` `get` **BILLBOARDMODE_Y**(): `number`

Billboard on Y axis

#### Returns

`number`

#### Overrides

TransformNode.BILLBOARDMODE\_Y

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:178

___

### BILLBOARDMODE\_Z

• `Static` `get` **BILLBOARDMODE_Z**(): `number`

Billboard on Z axis

#### Returns

`number`

#### Overrides

TransformNode.BILLBOARDMODE\_Z

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:183

## Methods

### \_buildUniformLayout

▸ `Protected` **_buildUniformLayout**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:834

___

### \_getData

▸ `Private` **_getData**(`applySkeleton?`, `applyMorph?`, `data?`, `kind?`): [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray)

Internal function to get buffer data and possibly apply morphs and normals

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `applySkeleton` | `boolean` | `false` |  |
| `applyMorph` | `boolean` | `false` |  |
| `data?` | [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray) | `undefined` |  |
| `kind` | `string` | `VertexBuffer.PositionKind` | the kind of data you want. Can be Normal or Position |

#### Returns

[`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1454

___

### \_markSubMeshesAsDirty

▸ `Private` **_markSubMeshesAsDirty**(`func`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `func` | (`defines`: [`MaterialDefines`](MaterialDefines.md)) => `void` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1009

___

### \_onCollisionPositionChange

▸ `Private` **_onCollisionPositionChange**(`collisionId`, `newPosition`, `collidedMesh?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `collisionId` | `number` | `undefined` |
| `newPosition` | [`Vector3`](Vector3.md) | `undefined` |
| `collidedMesh` | [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md) | `null` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1732

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

[TransformNode](TransformNode.md).[addBehavior](TransformNode.md#addbehavior)

#### Defined in

packages/dev/core/src/node.ts:366

___

### addChild

▸ **addChild**(`mesh`, `preserveScalingSign?`): [`AbstractMesh`](AbstractMesh.md)

Adds the passed mesh as a child to the current mesh

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | `undefined` | defines the child mesh |
| `preserveScalingSign` | `boolean` | `false` | if true, keep scaling sign of child. Otherwise, scaling sign might change. |

#### Returns

[`AbstractMesh`](AbstractMesh.md)

the current mesh

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:2141

___

### addRotation

▸ **addRotation**(`x`, `y`, `z`): [`TransformNode`](TransformNode.md)

Adds a rotation step to the mesh current rotation.
x, y, z are Euler angles expressed in radians.
This methods updates the current mesh rotation, either mesh.rotation, either mesh.rotationQuaternion if it's set.
This means this rotation is made in the mesh local space only.
It's useful to set a custom rotation order different from the BJS standard one YXZ.
Example : this rotates the mesh first around its local X axis, then around its local Z axis, finally around its local Y axis.
```javascript
mesh.addRotation(x1, 0, 0).addRotation(0, 0, z2).addRotation(0, 0, y3);
```
Note that `addRotation()` accumulates the passed rotation values to the current ones and computes the .rotation or .rotationQuaternion updated values.
Under the hood, only quaternions are used. So it's a little faster is you use .rotationQuaternion because it doesn't need to translate them back to Euler angles.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | Rotation to add |
| `y` | `number` | Rotation to add |
| `z` | `number` | Rotation to add |

#### Returns

[`TransformNode`](TransformNode.md)

the TransformNode.

#### Inherited from

[TransformNode](TransformNode.md).[addRotation](TransformNode.md#addrotation)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:973

___

### alignWithNormal

▸ **alignWithNormal**(`normal`, `upDirection?`): [`AbstractMesh`](AbstractMesh.md)

Align the mesh with a normal

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `normal` | [`Vector3`](Vector3.md) | defines the normal to use |
| `upDirection?` | [`Vector3`](Vector3.md) | can be used to redefined the up vector to use (will use the (0, 1, 0) by default) |

#### Returns

[`AbstractMesh`](AbstractMesh.md)

the current mesh

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:2557

___

### applyImpulse

▸ **applyImpulse**(`force`, `contactPoint`): [`AbstractMesh`](AbstractMesh.md)

Apply a physic impulse to the mesh

**`See`**

https://doc.babylonjs.com/how_to/using_the_physics_engine

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `force` | [`Vector3`](Vector3.md) | defines the force to apply |
| `contactPoint` | [`Vector3`](Vector3.md) | defines where to apply the force |

#### Returns

[`AbstractMesh`](AbstractMesh.md)

the current mesh

#### Defined in

packages/dev/core/src/Physics/physicsEngineComponent.ts:184

___

### attachToBone

▸ **attachToBone**(`bone`, `affectedTransformNode`): [`TransformNode`](TransformNode.md)

Attach the current TransformNode to another TransformNode associated with a bone

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `bone` | [`Bone`](Bone.md) | Bone affecting the TransformNode |
| `affectedTransformNode` | [`TransformNode`](TransformNode.md) | TransformNode associated with the bone |

#### Returns

[`TransformNode`](TransformNode.md)

this object

#### Inherited from

[TransformNode](TransformNode.md).[attachToBone](TransformNode.md#attachtobone)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:822

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

[TransformNode](TransformNode.md).[beginAnimation](TransformNode.md#beginanimation)

#### Defined in

packages/dev/core/src/node.ts:833

___

### buildBoundingInfo

▸ **buildBoundingInfo**(`minimum`, `maximum`, `worldMatrix?`): [`BoundingInfo`](BoundingInfo.md)

Creates a new bounding info for the mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `minimum` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | min vector of the bounding box/sphere |
| `maximum` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Vector3`](Vector3.md) | max vector of the bounding box/sphere |
| `worldMatrix?` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | defines the new world matrix |

#### Returns

[`BoundingInfo`](BoundingInfo.md)

the new bounding info

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1241

___

### calcMovePOV

▸ **calcMovePOV**(`amountRight`, `amountUp`, `amountForward`): [`Vector3`](Vector3.md)

Calculate relative position change from the point of view of behind the front of the mesh.
This is performed taking into account the meshes current rotation, so you do not have to care.
Supports definition of mesh facing forward or backward

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `amountRight` | `number` | defines the distance on the right axis |
| `amountUp` | `number` | defines the distance on the up axis |
| `amountForward` | `number` | defines the distance on the forward axis |

#### Returns

[`Vector3`](Vector3.md)

the new displacement vector

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1370

___

### calcRotatePOV

▸ **calcRotatePOV**(`flipBack`, `twirlClockwise`, `tiltRight`): [`Vector3`](Vector3.md)

Calculate relative rotation change from the point of view of behind the front of the mesh.
Supports definition of mesh facing forward or backward.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `flipBack` | `number` | defines the flip |
| `twirlClockwise` | `number` | defines the twirl |
| `tiltRight` | `number` | defines the tilt |

#### Returns

[`Vector3`](Vector3.md)

the new rotation vector

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1402

___

### clone

▸ **clone**(`name`, `newParent`, `doNotCloneChildren?`): [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

Clones the current mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the mesh name |
| `newParent` | [`Nullable`](../modules.md#nullable)[`Node`](Node.md) | defines the new mesh parent |
| `doNotCloneChildren?` | `boolean` | defines a boolean indicating that children must not be cloned (false by default) |

#### Returns

[`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

the new mesh

#### Overrides

[TransformNode](TransformNode.md).[clone](TransformNode.md#clone)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1979

___

### computeWorldMatrix

▸ **computeWorldMatrix**(`force?`): [`Matrix`](Matrix.md)

Computes the world matrix of the node

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `force?` | `boolean` | defines if the cache version should be invalidated forcing the world matrix to be created from scratch |

#### Returns

[`Matrix`](Matrix.md)

the world matrix

#### Inherited from

[TransformNode](TransformNode.md).[computeWorldMatrix](TransformNode.md#computeworldmatrix)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:1002

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

[TransformNode](TransformNode.md).[createAnimationRange](TransformNode.md#createanimationrange)

#### Defined in

packages/dev/core/src/node.ts:777

___

### createNormals

▸ **createNormals**(`updatable`): [`AbstractMesh`](AbstractMesh.md)

Creates new normals data for the mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `updatable` | `boolean` | defines if the normal vertex buffer must be flagged as updatable |

#### Returns

[`AbstractMesh`](AbstractMesh.md)

the current mesh

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:2535

___

### createOrUpdateSubmeshesOctree

▸ **createOrUpdateSubmeshesOctree**(`maxCapacity?`, `maxDepth?`): [`Octree`](Octree.md)[`SubMesh`](SubMesh.md)

This function will create an octree to help to select the right submeshes for rendering, picking and collision computations.
Please note that you must have a decent number of submeshes to get performance improvements when using an octree

**`See`**

 - https://www.babylonjs-playground.com/#NA4OQ#12
 - https://doc.babylonjs.com/how_to/optimizing_your_scene_with_octrees

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `maxCapacity?` | `number` | defines the maximum size of each block (64 by default) |
| `maxDepth?` | `number` | defines the maximum depth to use (no more than 2 levels by default) |

#### Returns

[`Octree`](Octree.md)[`SubMesh`](SubMesh.md)

the new octree

#### Defined in

packages/dev/core/src/Culling/Octrees/octreeSceneComponent.ts:83

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

[TransformNode](TransformNode.md).[deleteAnimationRange](TransformNode.md#deleteanimationrange)

#### Defined in

packages/dev/core/src/node.ts:794

___

### detachFromBone

▸ **detachFromBone**(`resetToPreviousParent?`): [`TransformNode`](TransformNode.md)

Detach the transform node if its associated with a bone

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `resetToPreviousParent` | `boolean` | `false` | Indicates if the parent that was in effect when attachToBone was called should be set back or if we should set parent to null instead (defaults to the latter) |

#### Returns

[`TransformNode`](TransformNode.md)

this object

#### Inherited from

[TransformNode](TransformNode.md).[detachFromBone](TransformNode.md#detachfrombone)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:840

___

### disableEdgesRendering

▸ **disableEdgesRendering**(): [`AbstractMesh`](AbstractMesh.md)

Disables the mesh edge rendering mode

#### Returns

[`AbstractMesh`](AbstractMesh.md)

the currentAbstractMesh

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:2585

___

### disableFacetData

▸ **disableFacetData**(): [`AbstractMesh`](AbstractMesh.md)

Disables the feature FacetData and frees the related memory

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_facetdata

#### Returns

[`AbstractMesh`](AbstractMesh.md)

the current mesh

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:2505

___

### dispose

▸ **dispose**(`doNotRecurse?`, `disposeMaterialAndTextures?`): `void`

Releases resources associated with this abstract mesh.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `doNotRecurse?` | `boolean` | `undefined` | Set to true to not recurse into each children (recurse into each children by default) |
| `disposeMaterialAndTextures` | `boolean` | `false` | Set to true to also dispose referenced materials and textures (false by default) |

#### Returns

`void`

#### Implementation of

[IDisposable](../interfaces/IDisposable.md).[dispose](../interfaces/IDisposable.md#dispose)

#### Overrides

[TransformNode](TransformNode.md).[dispose](TransformNode.md#dispose)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:2003

___

### enableEdgesRendering

▸ **enableEdgesRendering**(`epsilon?`, `checkVerticesInsteadOfIndices?`, `options?`): [`AbstractMesh`](AbstractMesh.md)

Enables the edge rendering mode on the mesh.
This mode makes the mesh edges visible

**`See`**

https://www.babylonjs-playground.com/#19O9TU#0

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `epsilon?` | `number` | defines the maximal distance between two angles to detect a face |
| `checkVerticesInsteadOfIndices?` | `boolean` | indicates that we should check vertex list directly instead of faces |
| `options?` | [`IEdgesRendererOptions`](../interfaces/IEdgesRendererOptions.md) | options to the edge renderer |

#### Returns

[`AbstractMesh`](AbstractMesh.md)

the currentAbstractMesh

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:2599

___

### freezeWorldMatrix

▸ **freezeWorldMatrix**(`newWorldMatrix?`, `decompose?`): [`TransformNode`](TransformNode.md)

Prevents the World matrix to be computed any longer

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `newWorldMatrix` | [`Nullable`](../modules.md#nullable)[`Matrix`](Matrix.md) | `null` | defines an optional matrix to use as world matrix |
| `decompose` | `boolean` | `false` | defines whether to decompose the given newWorldMatrix or directly assign |

#### Returns

[`TransformNode`](TransformNode.md)

the TransformNode.

#### Inherited from

[TransformNode](TransformNode.md).[freezeWorldMatrix](TransformNode.md#freezeworldmatrix)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:442

___

### getAbsolutePivotPoint

▸ **getAbsolutePivotPoint**(): [`Vector3`](Vector3.md)

Returns a new Vector3 set with the mesh pivot point World coordinates.

#### Returns

[`Vector3`](Vector3.md)

a new Vector3 set with the mesh pivot point World coordinates.

#### Inherited from

[TransformNode](TransformNode.md).[getAbsolutePivotPoint](TransformNode.md#getabsolutepivotpoint)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:707

___

### getAbsolutePivotPointToRef

▸ **getAbsolutePivotPointToRef**(`result`): [`TransformNode`](TransformNode.md)

Sets the Vector3 "result" coordinates with the mesh pivot point World coordinates.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `result` | [`Vector3`](Vector3.md) | vector3 to store the result |

#### Returns

[`TransformNode`](TransformNode.md)

this TransformNode.

#### Inherited from

[TransformNode](TransformNode.md).[getAbsolutePivotPointToRef](TransformNode.md#getabsolutepivotpointtoref)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:718

___

### getAbsolutePosition

▸ **getAbsolutePosition**(): [`Vector3`](Vector3.md)

Returns the mesh absolute position in the World.

#### Returns

[`Vector3`](Vector3.md)

a Vector3.

#### Inherited from

[TransformNode](TransformNode.md).[getAbsolutePosition](TransformNode.md#getabsoluteposition)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:484

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

[TransformNode](TransformNode.md).[getAnimationByName](TransformNode.md#getanimationbyname)

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

[TransformNode](TransformNode.md).[getAnimationRange](TransformNode.md#getanimationrange)

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

[TransformNode](TransformNode.md).[getAnimationRanges](TransformNode.md#getanimationranges)

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

[TransformNode](TransformNode.md).[getBehaviorByName](TransformNode.md#getbehaviorbyname)

#### Defined in

packages/dev/core/src/node.ts:420

___

### getBoundingInfo

▸ **getBoundingInfo**(): [`BoundingInfo`](BoundingInfo.md)

Returns the mesh BoundingInfo object or creates a new one and returns if it was undefined.
Note that it returns a shallow bounding of the mesh (i.e. it does not include children).
To get the full bounding of all children, call `getHierarchyBoundingVectors` instead.

#### Returns

[`BoundingInfo`](BoundingInfo.md)

a BoundingInfo

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1203

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

[TransformNode](TransformNode.md).[getChildMeshes](TransformNode.md#getchildmeshes)

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

[TransformNode](TransformNode.md).[getChildMeshes](TransformNode.md#getchildmeshes)

#### Defined in

packages/dev/core/src/node.ts:692

___

### getChildTransformNodes

▸ **getChildTransformNodes**(`directDescendantsOnly?`, `predicate?`): [`TransformNode`](TransformNode.md)[]

Get all child-transformNodes of this node

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `directDescendantsOnly?` | `boolean` | defines if true only direct descendants of 'this' will be considered, if false direct and also indirect (children of children, an so on in a recursive manner) descendants of 'this' will be considered |
| `predicate?` | (`node`: [`Node`](Node.md)) => `boolean` | defines an optional predicate that will be called on every evaluated child, the predicate must return true for a given child to be part of the result, otherwise it will be ignored |

#### Returns

[`TransformNode`](TransformNode.md)[]

an array of TransformNode

#### Inherited from

[TransformNode](TransformNode.md).[getChildTransformNodes](TransformNode.md#getchildtransformnodes)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:1414

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

[TransformNode](TransformNode.md).[getChildren](TransformNode.md#getchildren)

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

[TransformNode](TransformNode.md).[getChildren](TransformNode.md#getchildren)

#### Defined in

packages/dev/core/src/node.ts:722

___

### getClassName

▸ **getClassName**(): `string`

Returns the string "AbstractMesh"

#### Returns

`string`

"AbstractMesh"

#### Overrides

[TransformNode](TransformNode.md).[getClassName](TransformNode.md#getclassname)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:865

___

### getClosestFacetAtCoordinates

▸ **getClosestFacetAtCoordinates**(`x`, `y`, `z`, `projected?`, `checkFace?`, `facing?`): [`Nullable`](../modules.md#nullable)`number`

Returns the closest mesh facet index at (x,y,z) World coordinates, null if not found

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_facetdata

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `x` | `number` | `undefined` | defines x coordinate |
| `y` | `number` | `undefined` | defines y coordinate |
| `z` | `number` | `undefined` | defines z coordinate |
| `projected?` | [`Vector3`](Vector3.md) | `undefined` | sets as the (x,y,z) world projection on the facet |
| `checkFace` | `boolean` | `false` | if true (default false), only the facet "facing" to (x,y,z) or only the ones "turning their backs", according to the parameter "facing" are returned |
| `facing` | `boolean` | `true` | if facing and checkFace are true, only the facet "facing" to (x, y, z) are returned : positive dot (x, y, z) * facet position. If facing si false and checkFace is true, only the facet "turning their backs" to (x, y, z) are returned : negative dot (x, y, z) * facet position |

#### Returns

[`Nullable`](../modules.md#nullable)`number`

the face index if found (or null instead)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:2409

___

### getClosestFacetAtLocalCoordinates

▸ **getClosestFacetAtLocalCoordinates**(`x`, `y`, `z`, `projected?`, `checkFace?`, `facing?`): [`Nullable`](../modules.md#nullable)`number`

Returns the closest mesh facet index at (x,y,z) local coordinates, null if not found

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_facetdata

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `x` | `number` | `undefined` | defines x coordinate |
| `y` | `number` | `undefined` | defines y coordinate |
| `z` | `number` | `undefined` | defines z coordinate |
| `projected?` | [`Vector3`](Vector3.md) | `undefined` | sets as the (x,y,z) local projection on the facet |
| `checkFace` | `boolean` | `false` | if true (default false), only the facet "facing" to (x,y,z) or only the ones "turning their backs", according to the parameter "facing" are returned |
| `facing` | `boolean` | `true` | if facing and checkFace are true, only the facet "facing" to (x, y, z) are returned : positive dot (x, y, z) * facet position. If facing si false and checkFace is true, only the facet "turning their backs" to (x, y, z) are returned : negative dot (x, y, z) * facet position |

#### Returns

[`Nullable`](../modules.md#nullable)`number`

the face index if found (or null instead)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:2434

___

### getConnectedParticleSystems

▸ **getConnectedParticleSystems**(): [`IParticleSystem`](../interfaces/IParticleSystem.md)[]

This function returns all of the particle systems in the scene that use the mesh as an emitter.

#### Returns

[`IParticleSystem`](../interfaces/IParticleSystem.md)[]

an array of particle systems in the scene that use the mesh as an emitter

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:2607

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

[TransformNode](TransformNode.md).[getDescendants](TransformNode.md#getdescendants)

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

[TransformNode](TransformNode.md).[getDescendants](TransformNode.md#getdescendants)

#### Defined in

packages/dev/core/src/node.ts:662

___

### getDirection

▸ **getDirection**(`localAxis`): [`Vector3`](Vector3.md)

Returns a new Vector3 that is the localAxis, expressed in the mesh local space, rotated like the mesh.
This Vector3 is expressed in the World space.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `localAxis` | [`Vector3`](Vector3.md) | axis to rotate |

#### Returns

[`Vector3`](Vector3.md)

a new Vector3 that is the localAxis, expressed in the mesh local space, rotated like the mesh.

#### Inherited from

[TransformNode](TransformNode.md).[getDirection](TransformNode.md#getdirection)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:616

___

### getDirectionToRef

▸ **getDirectionToRef**(`localAxis`, `result`): [`TransformNode`](TransformNode.md)

Sets the Vector3 "result" as the rotated Vector3 "localAxis" in the same rotation than the mesh.
localAxis is expressed in the mesh local space.
result is computed in the World space from the mesh World matrix.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `localAxis` | [`Vector3`](Vector3.md) | axis to rotate |
| `result` | [`Vector3`](Vector3.md) | the resulting transformnode |

#### Returns

[`TransformNode`](TransformNode.md)

this TransformNode.

#### Inherited from

[TransformNode](TransformNode.md).[getDirectionToRef](TransformNode.md#getdirectiontoref)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:632

___

### getDistanceToCamera

▸ **getDistanceToCamera**(`camera?`): `number`

Returns the distance from the mesh to the active camera

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `camera` | [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md) | `null` | defines the camera to use |

#### Returns

`number`

the distance

#### Inherited from

[TransformNode](TransformNode.md).[getDistanceToCamera](TransformNode.md#getdistancetocamera)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:1316

___

### getEngine

▸ **getEngine**(): [`Engine`](Engine.md)

Gets the engine of the node

#### Returns

[`Engine`](Engine.md)

a Engine

#### Inherited from

[TransformNode](TransformNode.md).[getEngine](TransformNode.md#getengine)

#### Defined in

packages/dev/core/src/node.ts:352

___

### getFacetDataParameters

▸ **getFacetDataParameters**(): `any`

Returns the object "parameter" set with all the expected parameters for facetData computation by ComputeNormals()

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_facetdata

#### Returns

`any`

the parameters

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:2496

___

### getFacetLocalNormals

▸ **getFacetLocalNormals**(): [`Vector3`](Vector3.md)[]

Returns the facetLocalNormals array.
The normals are expressed in the mesh local spac

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_facetdata

#### Returns

[`Vector3`](Vector3.md)[]

an array of Vector3

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:2288

___

### getFacetLocalPartitioning

▸ **getFacetLocalPartitioning**(): `number`[][]

Returns the facetLocalPartitioning array

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_facetdata

#### Returns

`number`[][]

an array of array of numbers

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:2315

___

### getFacetLocalPositions

▸ **getFacetLocalPositions**(): [`Vector3`](Vector3.md)[]

Returns the facetLocalPositions array.
The facet positions are expressed in the mesh local space

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_facetdata

#### Returns

[`Vector3`](Vector3.md)[]

an array of Vector3

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:2302

___

### getFacetNormal

▸ **getFacetNormal**(`i`): [`Vector3`](Vector3.md)

Returns the i-th facet normal in the world system.
This method allocates a new Vector3 per call

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_facetdata

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `i` | `number` | defines the facet index |

#### Returns

[`Vector3`](Vector3.md)

a new Vector3

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:2358

___

### getFacetNormalToRef

▸ **getFacetNormalToRef**(`i`, `ref`): [`AbstractMesh`](AbstractMesh.md)

Sets the reference Vector3 with the i-th facet normal in the world system

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_facetdata

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `i` | `number` | defines the facet index |
| `ref` | [`Vector3`](Vector3.md) | defines the target vector |

#### Returns

[`AbstractMesh`](AbstractMesh.md)

the current mesh

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:2371

___

### getFacetPosition

▸ **getFacetPosition**(`i`): [`Vector3`](Vector3.md)

Returns the i-th facet position in the world system.
This method allocates a new Vector3 per call

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_facetdata

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `i` | `number` | defines the facet index |

#### Returns

[`Vector3`](Vector3.md)

a new Vector3

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:2331

___

### getFacetPositionToRef

▸ **getFacetPositionToRef**(`i`, `ref`): [`AbstractMesh`](AbstractMesh.md)

Sets the reference Vector3 with the i-th facet position in the world system

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_facetdata

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `i` | `number` | defines the facet index |
| `ref` | [`Vector3`](Vector3.md) | defines the target vector |

#### Returns

[`AbstractMesh`](AbstractMesh.md)

the current mesh

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:2344

___

### getFacetsAtLocalCoordinates

▸ **getFacetsAtLocalCoordinates**(`x`, `y`, `z`): [`Nullable`](../modules.md#nullable)`number`[]

Returns the facets (in an array) in the same partitioning block than the one the passed coordinates are located (expressed in the mesh local system)

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_facetdata

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | defines x coordinate |
| `y` | `number` | defines y coordinate |
| `z` | `number` | defines z coordinate |

#### Returns

[`Nullable`](../modules.md#nullable)`number`[]

the array of facet indexes

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:2385

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

[TransformNode](TransformNode.md).[getHierarchyBoundingVectors](TransformNode.md#gethierarchyboundingvectors)

#### Defined in

packages/dev/core/src/node.ts:933

___

### getIndices

▸ **getIndices**(): [`Nullable`](../modules.md#nullable)[`IndicesArray`](../modules.md#indicesarray)

Returns null by default. Implemented by child classes

#### Returns

[`Nullable`](../modules.md#nullable)[`IndicesArray`](../modules.md#indicesarray)

null

#### Implementation of

[IGetSetVerticesData](../interfaces/IGetSetVerticesData.md).[getIndices](../interfaces/IGetSetVerticesData.md#getindices)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1107

___

### getLOD

▸ **getLOD**(`camera`): [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

Returns the mesh itself by default. Implemented by child classes

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `camera` | [`Camera`](Camera.md) | defines the camera to use to pick the right LOD level |

#### Returns

[`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

the currentAbstractMesh

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1083

___

### getMaterialForRenderPass

▸ **getMaterialForRenderPass**(`renderPassId`): `undefined` \| [`Material`](Material.md)

Gets the material used to render the mesh in a specific render pass

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `renderPassId` | `number` | render pass id |

#### Returns

`undefined` \| [`Material`](Material.md)

material used for the render pass. If no specific material is used for this render pass, undefined is returned (meaning mesh.material is used for this pass)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:490

___

### getMeshUniformBuffer

▸ **getMeshUniformBuffer**(): [`UniformBuffer`](UniformBuffer.md)

Gets the mesh uniform buffer.

#### Returns

[`UniformBuffer`](UniformBuffer.md)

the uniform buffer of the mesh.

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:857

___

### getNormalsData

▸ **getNormalsData**(`applySkeleton?`, `applyMorph?`): [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray)

Get the normals vertex data and optionally apply skeleton and morphing.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `applySkeleton` | `boolean` | `false` | defines whether to apply the skeleton |
| `applyMorph` | `boolean` | `false` | defines whether to apply the morph target |

#### Returns

[`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray)

the normals data

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1544

___

### getPhysicsImpostor

▸ **getPhysicsImpostor**(): [`Nullable`](../modules.md#nullable)[`PhysicsImpostor`](PhysicsImpostor.md)

Gets the current physics impostor

**`See`**

https://doc.babylonjs.com/features/physics_engine

#### Returns

[`Nullable`](../modules.md#nullable)[`PhysicsImpostor`](PhysicsImpostor.md)

a physics impostor or null

#### Defined in

packages/dev/core/src/Physics/physicsEngineComponent.ts:176

___

### getPivotMatrix

▸ **getPivotMatrix**(): [`Matrix`](Matrix.md)

Returns the mesh pivot matrix.
Default : Identity.

#### Returns

[`Matrix`](Matrix.md)

the matrix

#### Inherited from

[TransformNode](TransformNode.md).[getPivotMatrix](TransformNode.md#getpivotmatrix)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:404

___

### getPivotPoint

▸ **getPivotPoint**(): [`Vector3`](Vector3.md)

Returns a new Vector3 set with the mesh pivot point coordinates in the local space.

#### Returns

[`Vector3`](Vector3.md)

the pivot point

#### Inherited from

[TransformNode](TransformNode.md).[getPivotPoint](TransformNode.md#getpivotpoint)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:685

___

### getPivotPointToRef

▸ **getPivotPointToRef**(`result`): [`TransformNode`](TransformNode.md)

Sets the passed Vector3 "result" with the coordinates of the mesh pivot point in the local space.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `result` | [`Vector3`](Vector3.md) | the vector3 to store the result |

#### Returns

[`TransformNode`](TransformNode.md)

this TransformNode.

#### Inherited from

[TransformNode](TransformNode.md).[getPivotPointToRef](TransformNode.md#getpivotpointtoref)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:696

___

### getPoseMatrix

▸ **getPoseMatrix**(): [`Matrix`](Matrix.md)

Returns the mesh Pose matrix.

#### Returns

[`Matrix`](Matrix.md)

the pose matrix

#### Inherited from

[TransformNode](TransformNode.md).[getPoseMatrix](TransformNode.md#getposematrix)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:292

___

### getPositionData

▸ **getPositionData**(`applySkeleton?`, `applyMorph?`, `data?`): [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray)

Get the position vertex data and optionally apply skeleton and morphing.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `applySkeleton` | `boolean` | `false` | defines whether to apply the skeleton |
| `applyMorph` | `boolean` | `false` | defines whether to apply the morph target |
| `data?` | [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray) | `undefined` | defines the position data to apply the skeleton and morph to |

#### Returns

[`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray)

the position data

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1555

___

### getPositionExpressedInLocalSpace

▸ **getPositionExpressedInLocalSpace**(): [`Vector3`](Vector3.md)

Returns the mesh position in the local space from the current World matrix values.

#### Returns

[`Vector3`](Vector3.md)

a new Vector3.

#### Inherited from

[TransformNode](TransformNode.md).[getPositionExpressedInLocalSpace](TransformNode.md#getpositionexpressedinlocalspace)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:542

___

### getPositionInCameraSpace

▸ **getPositionInCameraSpace**(`camera?`): [`Vector3`](Vector3.md)

Gets the position of the current mesh in camera space

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `camera` | [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md) | `null` | defines the camera to use |

#### Returns

[`Vector3`](Vector3.md)

a position

#### Inherited from

[TransformNode](TransformNode.md).[getPositionInCameraSpace](TransformNode.md#getpositionincameraspace)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:1303

___

### getScene

▸ **getScene**(): [`Scene`](Scene.md)

Gets the scene of the node

#### Returns

[`Scene`](Scene.md)

a scene

#### Inherited from

[TransformNode](TransformNode.md).[getScene](TransformNode.md#getscene)

#### Defined in

packages/dev/core/src/node.ts:344

___

### getTotalIndices

▸ **getTotalIndices**(): `number`

Returns a positive integer : the total number of indices in this mesh geometry.

#### Returns

`number`

the number of indices or zero if the mesh has no geometry.

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1099

___

### getTotalVertices

▸ **getTotalVertices**(): `number`

Returns 0 by default. Implemented by child classes

#### Returns

`number`

an integer

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1091

___

### getVerticesData

▸ **getVerticesData**(`kind`): [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray)

Returns the array of the requested vertex data kind. Implemented by child classes

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `kind` | `string` | defines the vertex data kind to use |

#### Returns

[`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray)

null

#### Implementation of

[IGetSetVerticesData](../interfaces/IGetSetVerticesData.md).[getVerticesData](../interfaces/IGetSetVerticesData.md#getverticesdata)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1117

___

### getWorldMatrix

▸ **getWorldMatrix**(): [`Matrix`](Matrix.md)

Gets the current world matrix

#### Returns

[`Matrix`](Matrix.md)

a Matrix

#### Overrides

[TransformNode](TransformNode.md).[getWorldMatrix](TransformNode.md#getworldmatrix)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1307

___

### instantiateHierarchy

▸ **instantiateHierarchy**(`newParent?`, `options?`, `onNewNodeCreated?`): [`Nullable`](../modules.md#nullable)[`TransformNode`](TransformNode.md)

Instantiate (when possible) or clone that node with its hierarchy

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `newParent` | [`Nullable`](../modules.md#nullable)[`TransformNode`](TransformNode.md) | `null` | defines the new parent to use for the instance (or clone) |
| `options?` | `Object` | `undefined` | defines options to configure how copy is done |
| `options.doNotInstantiate` | `boolean` \| (`node`: [`TransformNode`](TransformNode.md)) => `boolean` | `undefined` | defines if the model must be instantiated or just cloned |
| `onNewNodeCreated?` | (`source`: [`TransformNode`](TransformNode.md), `clone`: [`TransformNode`](TransformNode.md)) => `void` | `undefined` | defines an option callback to call when a clone or an instance is created |

#### Returns

[`Nullable`](../modules.md#nullable)[`TransformNode`](TransformNode.md)

an instance (or a clone) of the current node with its hierarchy

#### Inherited from

[TransformNode](TransformNode.md).[instantiateHierarchy](TransformNode.md#instantiatehierarchy)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:416

___

### intersects

▸ **intersects**(`ray`, `fastCheck?`, `trianglePredicate?`, `onlyBoundingInfo?`, `worldToUse?`, `skipBoundingInfo?`): [`PickingInfo`](PickingInfo.md)

Checks if the passed Ray intersects with the mesh

**`See`**

https://doc.babylonjs.com/babylon101/intersect_collisions_-_mesh

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `ray` | [`Ray`](Ray.md) | `undefined` | defines the ray to use |
| `fastCheck?` | `boolean` | `undefined` | defines if fast mode (but less precise) must be used (false by default) |
| `trianglePredicate?` | [`TrianglePickingPredicate`](../modules.md#trianglepickingpredicate) | `undefined` | defines an optional predicate used to select faces when a mesh intersection is detected |
| `onlyBoundingInfo` | `boolean` | `false` | defines a boolean indicating if picking should only happen using bounding info (false by default) |
| `worldToUse?` | [`Matrix`](Matrix.md) | `undefined` | defines the world matrix to use to get the world coordinate of the intersection point |
| `skipBoundingInfo` | `boolean` | `false` | a boolean indicating if we should skip the bounding info check |

#### Returns

[`PickingInfo`](PickingInfo.md)

the picking info

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1854

___

### intersectsMesh

▸ **intersectsMesh**(`mesh`, `precise?`, `includeDescendants?`): `boolean`

True if the mesh intersects another mesh or a SolidParticle object

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) \| [`SolidParticle`](SolidParticle.md) | `undefined` | defines a target mesh or SolidParticle to test |
| `precise` | `boolean` | `false` | Unless the parameter `precise` is set to `true` the intersection is computed according to Axis Aligned Bounding Boxes (AABB), else according to OBB (Oriented BBoxes) |
| `includeDescendants?` | `boolean` | `undefined` | Can be set to true to test if the mesh defined in parameters intersects with the current mesh or any child meshes |

#### Returns

`boolean`

true if there is an intersection

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1652

___

### intersectsPoint

▸ **intersectsPoint**(`point`): `boolean`

Returns true if the passed point (Vector3) is inside the mesh bounding box

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `point` | [`Vector3`](Vector3.md) | defines the point to test |

#### Returns

`boolean`

true if there is an intersection

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1676

___

### isCompletelyInFrustum

▸ **isCompletelyInFrustum**(`frustumPlanes`): `boolean`

Returns `true` if the mesh is completely in the frustum defined be the passed array of planes.
A mesh is completely in the frustum if its bounding box it completely inside the frustum.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `frustumPlanes` | [`Plane`](Plane.md)[] | defines the frustum to test |

#### Returns

`boolean`

true if the mesh is completely in the frustum planes

#### Implementation of

[ICullable](../interfaces/ICullable.md).[isCompletelyInFrustum](../interfaces/ICullable.md#iscompletelyinfrustum)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1641

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

[TransformNode](TransformNode.md).[isDescendantOf](TransformNode.md#isdescendantof)

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

[TransformNode](TransformNode.md).[isDisposed](TransformNode.md#isdisposed)

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

[TransformNode](TransformNode.md).[isEnabled](TransformNode.md#isenabled)

#### Defined in

packages/dev/core/src/node.ts:569

___

### isInFrustum

▸ **isInFrustum**(`frustumPlanes`): `boolean`

Returns `true` if the mesh is within the frustum defined by the passed array of planes.
A mesh is in the frustum if its bounding box intersects the frustum

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `frustumPlanes` | [`Plane`](Plane.md)[] | defines the frustum to test |

#### Returns

`boolean`

true if the mesh is in the frustum planes

#### Implementation of

[ICullable](../interfaces/ICullable.md).[isInFrustum](../interfaces/ICullable.md#isinfrustum)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1631

___

### isReady

▸ **isReady**(`completeCheck?`): `boolean`

Is this node ready to be used/rendered

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `completeCheck` | `boolean` | `false` | defines if a complete check (including materials and lights) has to be done (false by default) |

#### Returns

`boolean`

true if the node is ready

#### Inherited from

[TransformNode](TransformNode.md).[isReady](TransformNode.md#isready)

#### Defined in

packages/dev/core/src/node.ts:548

___

### isUsingPivotMatrix

▸ **isUsingPivotMatrix**(): `boolean`

return true if a pivot has been set

#### Returns

`boolean`

true if a pivot matrix is used

#### Inherited from

[TransformNode](TransformNode.md).[isUsingPivotMatrix](TransformNode.md#isusingpivotmatrix)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:203

___

### isVerticesDataPresent

▸ **isVerticesDataPresent**(`kind`): `boolean`

Gets a boolean indicating if specific vertex data is present

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `kind` | `string` | defines the vertex data kind to use |

#### Returns

`boolean`

true is data kind is present

#### Implementation of

[IGetSetVerticesData](../interfaces/IGetSetVerticesData.md).[isVerticesDataPresent](../interfaces/IGetSetVerticesData.md#isverticesdatapresent)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1193

___

### locallyTranslate

▸ **locallyTranslate**(`vector3`): [`TransformNode`](TransformNode.md)

Translates the mesh along the passed Vector3 in its local space.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vector3` | [`Vector3`](Vector3.md) | the distance to translate in localspace |

#### Returns

[`TransformNode`](TransformNode.md)

the TransformNode.

#### Inherited from

[TransformNode](TransformNode.md).[locallyTranslate](TransformNode.md#locallytranslate)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:554

___

### lookAt

▸ **lookAt**(`targetPoint`, `yawCor?`, `pitchCor?`, `rollCor?`, `space?`): [`TransformNode`](TransformNode.md)

Orients a mesh towards a target point. Mesh must be drawn facing user.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `targetPoint` | [`Vector3`](Vector3.md) | `undefined` | the position (must be in same space as current mesh) to look at |
| `yawCor` | `number` | `0` | optional yaw (y-axis) correction in radians |
| `pitchCor` | `number` | `0` | optional pitch (x-axis) correction in radians |
| `rollCor` | `number` | `0` | optional roll (z-axis) correction in radians |
| `space` | [`Space`](../enums/Space.md) | `Space.LOCAL` | the chosen space of the target |

#### Returns

[`TransformNode`](TransformNode.md)

the TransformNode.

#### Inherited from

[TransformNode](TransformNode.md).[lookAt](TransformNode.md#lookat)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:571

___

### markAsDirty

▸ **markAsDirty**(`property?`): [`AbstractMesh`](AbstractMesh.md)

Flag the AbstractMesh as dirty (Forcing it to update everything)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `property?` | `string` | if set to "rotation" the objects rotationQuaternion will be set to null |

#### Returns

[`AbstractMesh`](AbstractMesh.md)

this AbstractMesh

#### Overrides

[TransformNode](TransformNode.md).[markAsDirty](TransformNode.md#markasdirty)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1049

___

### movePOV

▸ **movePOV**(`amountRight`, `amountUp`, `amountForward`): [`AbstractMesh`](AbstractMesh.md)

Perform relative position change from the point of view of behind the front of the mesh.
This is performed taking into account the meshes current rotation, so you do not have to care.
Supports definition of mesh facing forward or backward

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `amountRight` | `number` | defines the distance on the right axis |
| `amountUp` | `number` | defines the distance on the up axis |
| `amountForward` | `number` | defines the distance on the forward axis |

#### Returns

[`AbstractMesh`](AbstractMesh.md)

the current mesh

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1356

___

### moveWithCollisions

▸ **moveWithCollisions**(`displacement`): [`AbstractMesh`](AbstractMesh.md)

Move the mesh using collision engine

**`See`**

https://doc.babylonjs.com/babylon101/cameras,_mesh_collisions_and_gravity

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `displacement` | [`Vector3`](Vector3.md) | defines the requested displacement vector |

#### Returns

[`AbstractMesh`](AbstractMesh.md)

the current mesh

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1708

___

### normalizeToUnitCube

▸ **normalizeToUnitCube**(`includeDescendants?`, `ignoreRotation?`, `predicate?`): [`AbstractMesh`](AbstractMesh.md)

Uniformly scales the mesh to fit inside of a unit cube (1 X 1 X 1 units)

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `includeDescendants` | `boolean` | `true` | Use the hierarchy's bounding box instead of the mesh's bounding box. Default is false |
| `ignoreRotation` | `boolean` | `false` | ignore rotation when computing the scale (ie. object will be axis aligned). Default is false |
| `predicate?` | [`Nullable`](../modules.md#nullable)(`node`: [`AbstractMesh`](AbstractMesh.md)) => `boolean` | `undefined` | predicate that is passed in to getHierarchyBoundingVectors when selecting which object should be included when scaling |

#### Returns

[`AbstractMesh`](AbstractMesh.md)

the current mesh

#### Overrides

[TransformNode](TransformNode.md).[normalizeToUnitCube](TransformNode.md#normalizetounitcube)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1253

___

### refreshBoundingInfo

▸ **refreshBoundingInfo**(`applySkeleton?`, `applyMorph?`): [`AbstractMesh`](AbstractMesh.md)

This method recomputes and sets a new BoundingInfo to the mesh unless it is locked.
This means the mesh underlying bounding box and sphere are recomputed.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `applySkeleton` | `boolean` | `false` | defines whether to apply the skeleton before computing the bounding info |
| `applyMorph` | `boolean` | `false` | defines whether to apply the morph target before computing the bounding info |

#### Returns

[`AbstractMesh`](AbstractMesh.md)

the current mesh

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1414

___

### registerAfterWorldMatrixUpdate

▸ **registerAfterWorldMatrixUpdate**(`func`): [`TransformNode`](TransformNode.md)

If you'd like to be called back after the mesh position, rotation or scaling has been updated.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `func` | (`mesh`: [`TransformNode`](TransformNode.md)) => `void` | callback function to add |

#### Returns

[`TransformNode`](TransformNode.md)

the TransformNode.

#### Inherited from

[TransformNode](TransformNode.md).[registerAfterWorldMatrixUpdate](TransformNode.md#registerafterworldmatrixupdate)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:1283

___

### releaseSubMeshes

▸ **releaseSubMeshes**(): [`AbstractMesh`](AbstractMesh.md)

Disposes all the submeshes of the current meshnp

#### Returns

[`AbstractMesh`](AbstractMesh.md)

the current mesh

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1987

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

[TransformNode](TransformNode.md).[removeBehavior](TransformNode.md#removebehavior)

#### Defined in

packages/dev/core/src/node.ts:393

___

### removeChild

▸ **removeChild**(`mesh`, `preserveScalingSign?`): [`AbstractMesh`](AbstractMesh.md)

Removes the passed mesh from the current mesh children list

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | `undefined` | defines the child mesh |
| `preserveScalingSign` | `boolean` | `false` | if true, keep scaling sign of child. Otherwise, scaling sign might change. |

#### Returns

[`AbstractMesh`](AbstractMesh.md)

the current mesh

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:2152

___

### resetDrawCache

▸ **resetDrawCache**(`passId?`): `void`

Resets the draw wrappers cache for all submeshes of this abstract mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `passId?` | `number` | If provided, releases only the draw wrapper corresponding to this render pass id |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1059

___

### resetLocalMatrix

▸ **resetLocalMatrix**(`independentOfChildren?`): `void`

Resets this nodeTransform's local matrix to Matrix.Identity().

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `independentOfChildren` | `boolean` | `true` | indicates if all child nodeTransform's world-space transform should be preserved. |

#### Returns

`void`

#### Inherited from

[TransformNode](TransformNode.md).[resetLocalMatrix](TransformNode.md#resetlocalmatrix)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:1244

___

### rotate

▸ **rotate**(`axis`, `amount`, `space?`): [`TransformNode`](TransformNode.md)

Rotates the mesh around the axis vector for the passed angle (amount) expressed in radians, in the given space.
space (default LOCAL) can be either Space.LOCAL, either Space.WORLD.
Note that the property `rotationQuaternion` is then automatically updated and the property `rotation` is set to (0,0,0) and no longer used.
The passed axis is also normalized.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `axis` | [`Vector3`](Vector3.md) | the axis to rotate around |
| `amount` | `number` | the amount to rotate in radians |
| `space?` | [`Space`](../enums/Space.md) | Space to rotate in (Default: local) |

#### Returns

[`TransformNode`](TransformNode.md)

the TransformNode.

#### Inherited from

[TransformNode](TransformNode.md).[rotate](TransformNode.md#rotate)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:871

___

### rotateAround

▸ **rotateAround**(`point`, `axis`, `amount`): [`TransformNode`](TransformNode.md)

Rotates the mesh around the axis vector for the passed angle (amount) expressed in radians, in world space.
Note that the property `rotationQuaternion` is then automatically updated and the property `rotation` is set to (0,0,0) and no longer used.
The passed axis is also normalized. .
Method is based on http://www.euclideanspace.com/maths/geometry/affine/aroundPoint/index.htm

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `point` | [`Vector3`](Vector3.md) | the point to rotate around |
| `axis` | [`Vector3`](Vector3.md) | the axis to rotate around |
| `amount` | `number` | the amount to rotate in radians |

#### Returns

[`TransformNode`](TransformNode.md)

the TransformNode

#### Inherited from

[TransformNode](TransformNode.md).[rotateAround](TransformNode.md#rotatearound)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:903

___

### rotatePOV

▸ **rotatePOV**(`flipBack`, `twirlClockwise`, `tiltRight`): [`AbstractMesh`](AbstractMesh.md)

Perform relative rotation change from the point of view of behind the front of the mesh.
Supports definition of mesh facing forward or backward

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `flipBack` | `number` | defines the flip |
| `twirlClockwise` | `number` | defines the twirl |
| `tiltRight` | `number` | defines the tilt |

#### Returns

[`AbstractMesh`](AbstractMesh.md)

the current mesh

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1389

___

### serialize

▸ **serialize**(`currentSerializationObject?`): `any`

Serializes the objects information.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `currentSerializationObject?` | `any` | defines the object to serialize in |

#### Returns

`any`

the serialized object

#### Inherited from

[TransformNode](TransformNode.md).[serialize](TransformNode.md#serialize)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:1360

___

### serializeAnimationRanges

▸ **serializeAnimationRanges**(): `any`

Serialize animation ranges into a JSON compatible object

#### Returns

`any`

serialization object

#### Inherited from

[TransformNode](TransformNode.md).[serializeAnimationRanges](TransformNode.md#serializeanimationranges)

#### Defined in

packages/dev/core/src/node.ts:847

___

### setAbsolutePosition

▸ **setAbsolutePosition**(`absolutePosition`): [`TransformNode`](TransformNode.md)

Sets the mesh absolute position in the World from a Vector3 or an Array(3).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `absolutePosition` | [`Vector3`](Vector3.md) | the absolute position to set |

#### Returns

[`TransformNode`](TransformNode.md)

the TransformNode.

#### Inherited from

[TransformNode](TransformNode.md).[setAbsolutePosition](TransformNode.md#setabsoluteposition)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:494

___

### setBoundingInfo

▸ **setBoundingInfo**(`boundingInfo`): [`AbstractMesh`](AbstractMesh.md)

Overwrite the current bounding info

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `boundingInfo` | [`BoundingInfo`](BoundingInfo.md) | defines the new bounding info |

#### Returns

[`AbstractMesh`](AbstractMesh.md)

the current mesh

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1222

___

### setDirection

▸ **setDirection**(`localAxis`, `yawCor?`, `pitchCor?`, `rollCor?`): [`TransformNode`](TransformNode.md)

Sets this transform node rotation to the given local axis.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `localAxis` | [`Vector3`](Vector3.md) | `undefined` | the axis in local space |
| `yawCor` | `number` | `0` | optional yaw (y-axis) correction in radians |
| `pitchCor` | `number` | `0` | optional pitch (x-axis) correction in radians |
| `rollCor` | `number` | `0` | optional roll (z-axis) correction in radians |

#### Returns

[`TransformNode`](TransformNode.md)

this TransformNode

#### Inherited from

[TransformNode](TransformNode.md).[setDirection](TransformNode.md#setdirection)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:645

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

[TransformNode](TransformNode.md).[setEnabled](TransformNode.md#setenabled)

#### Defined in

packages/dev/core/src/node.ts:596

___

### setIndices

▸ **setIndices**(`indices`, `totalVertices`): [`AbstractMesh`](AbstractMesh.md)

Sets the mesh indices,
If the mesh has no geometry, a new Geometry object is created and set to the mesh.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `indices` | [`IndicesArray`](../modules.md#indicesarray) | Expects an array populated with integers or a typed array (Int32Array, Uint32Array, Uint16Array) |
| `totalVertices` | [`Nullable`](../modules.md#nullable)`number` | Defines the total number of vertices |

#### Returns

[`AbstractMesh`](AbstractMesh.md)

the current mesh

#### Implementation of

[IGetSetVerticesData](../interfaces/IGetSetVerticesData.md).[setIndices](../interfaces/IGetSetVerticesData.md#setindices)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1183

___

### setMaterialForRenderPass

▸ **setMaterialForRenderPass**(`renderPassId`, `material?`): `void`

Sets the material to be used to render the mesh in a specific render pass

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `renderPassId` | `number` | render pass id |
| `material?` | [`Material`](Material.md) | material to use for this render pass. If undefined is passed, no specific material will be used for this render pass but the regular material will be used instead (mesh.material) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:499

___

### setParent

▸ **setParent**(`node`, `preserveScalingSign?`): [`TransformNode`](TransformNode.md)

Defines the passed node as the parent of the current node.
The node will remain exactly where it is and its position / rotation will be updated accordingly.
Note that if the mesh has a pivot matrix / point defined it will be applied after the parent was updated.
In that case the node will not remain in the same space as it is, as the pivot will be applied.

**`See`**

https://doc.babylonjs.com/how_to/parenting

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `node` | [`Nullable`](../modules.md#nullable)[`Node`](Node.md) | `undefined` | the node ot set as the parent |
| `preserveScalingSign` | `boolean` | `false` | if true, keep scaling sign of child. Otherwise, scaling sign might change. |

#### Returns

[`TransformNode`](TransformNode.md)

this TransformNode.

#### Inherited from

[TransformNode](TransformNode.md).[setParent](TransformNode.md#setparent)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:750

___

### setPhysicsLinkWith

▸ **setPhysicsLinkWith**(`otherMesh`, `pivot1`, `pivot2`, `options?`): [`AbstractMesh`](AbstractMesh.md)

Creates a physic joint between two meshes

**`See`**

https://www.babylonjs-playground.com/#0BS5U0#0

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherMesh` | [`Mesh`](Mesh.md) | defines the other mesh to use |
| `pivot1` | [`Vector3`](Vector3.md) | defines the pivot to use on this mesh |
| `pivot2` | [`Vector3`](Vector3.md) | defines the pivot to use on the other mesh |
| `options?` | `any` | defines additional options (can be plugin dependent) |

#### Returns

[`AbstractMesh`](AbstractMesh.md)

the current mesh

#### Defined in

packages/dev/core/src/Physics/physicsEngineComponent.ts:195

___

### setPivotMatrix

▸ **setPivotMatrix**(`matrix`, `postMultiplyPivotMatrix?`): [`TransformNode`](TransformNode.md)

Sets a new pivot matrix to the current node

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `matrix` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | `undefined` | defines the new pivot matrix to use |
| `postMultiplyPivotMatrix` | `boolean` | `true` | defines if the pivot matrix must be cancelled in the world matrix. When this parameter is set to true (default), the inverse of the pivot matrix is also applied at the end to cancel the transformation effect |

#### Returns

[`TransformNode`](TransformNode.md)

the current TransformNode

#### Inherited from

[TransformNode](TransformNode.md).[setPivotMatrix](TransformNode.md#setpivotmatrix)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:381

___

### setPivotPoint

▸ **setPivotPoint**(`point`, `space?`): [`TransformNode`](TransformNode.md)

Sets a new pivot point to the current node

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `point` | [`Vector3`](Vector3.md) | `undefined` | defines the new pivot point to use |
| `space` | [`Space`](../enums/Space.md) | `Space.LOCAL` | defines if the point is in world or local space (local by default) |

#### Returns

[`TransformNode`](TransformNode.md)

the current TransformNode

#### Inherited from

[TransformNode](TransformNode.md).[setPivotPoint](TransformNode.md#setpivotpoint)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:665

___

### setPositionWithLocalVector

▸ **setPositionWithLocalVector**(`vector3`): [`TransformNode`](TransformNode.md)

Sets the mesh position in its local space.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vector3` | [`Vector3`](Vector3.md) | the position to set in localspace |

#### Returns

[`TransformNode`](TransformNode.md)

the TransformNode.

#### Inherited from

[TransformNode](TransformNode.md).[setPositionWithLocalVector](TransformNode.md#setpositionwithlocalvector)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:532

___

### setPreTransformMatrix

▸ **setPreTransformMatrix**(`matrix`): [`TransformNode`](TransformNode.md)

Sets a new matrix to apply before all other transformation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `matrix` | [`Matrix`](Matrix.md) | defines the transform matrix |

#### Returns

[`TransformNode`](TransformNode.md)

the current TransformNode

#### Inherited from

[TransformNode](TransformNode.md).[setPreTransformMatrix](TransformNode.md#setpretransformmatrix)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:371

___

### setVerticesData

▸ **setVerticesData**(`kind`, `data`, `updatable?`, `stride?`): [`AbstractMesh`](AbstractMesh.md)

Sets the vertex data of the mesh geometry for the requested `kind`.
If the mesh has no geometry, a new Geometry object is set to the mesh and then passed this vertex data.
Note that a new underlying VertexBuffer object is created each call.
If the `kind` is the `PositionKind`, the mesh BoundingInfo is renewed, so the bounding box and sphere, and the mesh World Matrix is recomputed.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `kind` | `string` | defines vertex data kind:  * VertexBuffer.PositionKind  * VertexBuffer.UVKind  * VertexBuffer.UV2Kind  * VertexBuffer.UV3Kind  * VertexBuffer.UV4Kind  * VertexBuffer.UV5Kind  * VertexBuffer.UV6Kind  * VertexBuffer.ColorKind  * VertexBuffer.MatricesIndicesKind  * VertexBuffer.MatricesIndicesExtraKind  * VertexBuffer.MatricesWeightsKind  * VertexBuffer.MatricesWeightsExtraKind |
| `data` | [`FloatArray`](../modules.md#floatarray) | defines the data source |
| `updatable?` | `boolean` | defines if the data must be flagged as updatable (or static) |
| `stride?` | `number` | defines the vertex stride (size of an entire vertex). Can be null and in this case will be deduced from vertex data kind |

#### Returns

[`AbstractMesh`](AbstractMesh.md)

the current mesh

#### Implementation of

[IGetSetVerticesData](../interfaces/IGetSetVerticesData.md).[setVerticesData](../interfaces/IGetSetVerticesData.md#setverticesdata)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1145

___

### toString

▸ **toString**(`fullDetails?`): `string`

Gets a string representation of the current mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fullDetails?` | `boolean` | defines a boolean indicating if full details must be included |

#### Returns

`string`

a string representation of the current mesh

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:874

___

### transferToEffect

▸ **transferToEffect**(`world`): `void`

Transfer the mesh values to its UBO.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `world` | [`Matrix`](Matrix.md) | The world matrix associated with the mesh |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:844

___

### translate

▸ **translate**(`axis`, `distance`, `space?`): [`TransformNode`](TransformNode.md)

Translates the mesh along the axis vector for the passed distance in the given space.
space (default LOCAL) can be either Space.LOCAL, either Space.WORLD.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `axis` | [`Vector3`](Vector3.md) | the axis to translate in |
| `distance` | `number` | the distance to translate |
| `space?` | [`Space`](../enums/Space.md) | Space to rotate in (Default: local) |

#### Returns

[`TransformNode`](TransformNode.md)

the TransformNode.

#### Inherited from

[TransformNode](TransformNode.md).[translate](TransformNode.md#translate)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:945

___

### unfreezeWorldMatrix

▸ **unfreezeWorldMatrix**(): [`AbstractMesh`](AbstractMesh.md)

Allows back the World matrix computation.

#### Returns

[`AbstractMesh`](AbstractMesh.md)

the TransformNode.

#### Inherited from

[TransformNode](TransformNode.md).[unfreezeWorldMatrix](TransformNode.md#unfreezeworldmatrix)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:467

___

### unregisterAfterWorldMatrixUpdate

▸ **unregisterAfterWorldMatrixUpdate**(`func`): [`TransformNode`](TransformNode.md)

Removes a registered callback function.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `func` | (`mesh`: [`TransformNode`](TransformNode.md)) => `void` | callback function to remove |

#### Returns

[`TransformNode`](TransformNode.md)

the TransformNode.

#### Inherited from

[TransformNode](TransformNode.md).[unregisterAfterWorldMatrixUpdate](TransformNode.md#unregisterafterworldmatrixupdate)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:1293

___

### updateFacetData

▸ **updateFacetData**(): [`AbstractMesh`](AbstractMesh.md)

Updates the mesh facetData arrays and the internal partitioning when the mesh is morphed or updated.
This method can be called within the render loop.
You don't need to call this method by yourself in the render loop when you update/morph a mesh with the methods CreateXXX() as they automatically manage this computation

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_facetdata

#### Returns

[`AbstractMesh`](AbstractMesh.md)

the current mesh

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:2188

___

### updateIndices

▸ **updateIndices**(`indices`, `offset?`, `gpuMemoryOnly?`): [`AbstractMesh`](AbstractMesh.md)

Updates the AbstractMesh indices array

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `indices` | [`IndicesArray`](../modules.md#indicesarray) | `undefined` | defines the data source |
| `offset?` | `number` | `undefined` | defines the offset in the index buffer where to store the new data (can be null) |
| `gpuMemoryOnly` | `boolean` | `false` | defines a boolean indicating that only the GPU memory must be updated leaving the CPU version of the indices unchanged (false by default) |

#### Returns

[`AbstractMesh`](AbstractMesh.md)

the current mesh

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:2526

___

### updatePoseMatrix

▸ **updatePoseMatrix**(`matrix`): [`TransformNode`](TransformNode.md)

Copies the parameter passed Matrix into the mesh Pose matrix.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `matrix` | [`Matrix`](Matrix.md) | the matrix to copy the pose from |

#### Returns

[`TransformNode`](TransformNode.md)

this TransformNode.

#### Inherited from

[TransformNode](TransformNode.md).[updatePoseMatrix](TransformNode.md#updateposematrix)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:279

___

### updateVerticesData

▸ **updateVerticesData**(`kind`, `data`, `updateExtends?`, `makeItUnique?`): [`AbstractMesh`](AbstractMesh.md)

Updates the existing vertex data of the mesh geometry for the requested `kind`.
If the mesh has no geometry, it is simply returned as it is.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `kind` | `string` | defines vertex data kind:  * VertexBuffer.PositionKind  * VertexBuffer.UVKind  * VertexBuffer.UV2Kind  * VertexBuffer.UV3Kind  * VertexBuffer.UV4Kind  * VertexBuffer.UV5Kind  * VertexBuffer.UV6Kind  * VertexBuffer.ColorKind  * VertexBuffer.MatricesIndicesKind  * VertexBuffer.MatricesIndicesExtraKind  * VertexBuffer.MatricesWeightsKind  * VertexBuffer.MatricesWeightsExtraKind |
| `data` | [`FloatArray`](../modules.md#floatarray) | defines the data source |
| `updateExtends?` | `boolean` | If `kind` is `PositionKind` and if `updateExtends` is true, the mesh BoundingInfo is renewed, so the bounding box and sphere, and the mesh World Matrix is recomputed |
| `makeItUnique?` | `boolean` | If true, a new global geometry is created from this data and is set to the mesh |

#### Returns

[`AbstractMesh`](AbstractMesh.md)

the current mesh

#### Implementation of

[IGetSetVerticesData](../interfaces/IGetSetVerticesData.md).[updateVerticesData](../interfaces/IGetSetVerticesData.md#updateverticesdata)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1171

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

[TransformNode](TransformNode.md).[AddNodeConstructor](TransformNode.md#addnodeconstructor)

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

[TransformNode](TransformNode.md).[Construct](TransformNode.md#construct)

#### Defined in

packages/dev/core/src/node.ts:75

___

### Parse

▸ `Static` **Parse**(`parsedTransformNode`, `scene`, `rootUrl`): [`TransformNode`](TransformNode.md)

Returns a new TransformNode object parsed from the source provided.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `parsedTransformNode` | `any` | is the source. |
| `scene` | [`Scene`](Scene.md) | the scene the object belongs to |
| `rootUrl` | `string` | is a string, it's the root URL to prefix the `delayLoadingFile` property with |

#### Returns

[`TransformNode`](TransformNode.md)

a new TransformNode object parsed from the source provided.

#### Inherited from

[TransformNode](TransformNode.md).[Parse](TransformNode.md#parse)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:1385

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

[TransformNode](TransformNode.md).[ParseAnimationRanges](TransformNode.md#parseanimationranges)

#### Defined in

packages/dev/core/src/node.ts:919
