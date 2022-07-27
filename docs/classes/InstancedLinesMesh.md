[@dev/core](../README.md) / [Exports](../modules.md) / InstancedLinesMesh

# Class: InstancedLinesMesh

Creates an instance based on a source LinesMesh

## Hierarchy

- [`InstancedMesh`](InstancedMesh.md)

  ↳ **`InstancedLinesMesh`**

## Table of contents

### Constructors

- [constructor](InstancedLinesMesh.md#constructor)

### Properties

- [\_boundingInfo](InstancedLinesMesh.md#_boundinginfo)
- [\_boundingInfoIsDirty](InstancedLinesMesh.md#_boundinginfoisdirty)
- [\_isDirty](InstancedLinesMesh.md#_isdirty)
- [\_isWorldMatrixFrozen](InstancedLinesMesh.md#_isworldmatrixfrozen)
- [\_parentNode](InstancedLinesMesh.md#_parentnode)
- [\_ranges](InstancedLinesMesh.md#_ranges)
- [\_scaling](InstancedLinesMesh.md#_scaling)
- [actionManager](InstancedLinesMesh.md#actionmanager)
- [alphaIndex](InstancedLinesMesh.md#alphaindex)
- [alwaysSelectAsActiveMesh](InstancedLinesMesh.md#alwaysselectasactivemesh)
- [animations](InstancedLinesMesh.md#animations)
- [cullingStrategy](InstancedLinesMesh.md#cullingstrategy)
- [definedFacingForward](InstancedLinesMesh.md#definedfacingforward)
- [doNotSyncBoundingInfo](InstancedLinesMesh.md#donotsyncboundinginfo)
- [edgesColor](InstancedLinesMesh.md#edgescolor)
- [edgesRenderer](InstancedLinesMesh.md#edgesrenderer)
- [edgesWidth](InstancedLinesMesh.md#edgeswidth)
- [ellipsoid](InstancedLinesMesh.md#ellipsoid)
- [ellipsoidOffset](InstancedLinesMesh.md#ellipsoidoffset)
- [enablePointerMoveEvents](InstancedLinesMesh.md#enablepointermoveevents)
- [forceRenderingWhenOccluded](InstancedLinesMesh.md#forcerenderingwhenoccluded)
- [id](InstancedLinesMesh.md#id)
- [ignoreNonUniformScaling](InstancedLinesMesh.md#ignorenonuniformscaling)
- [inspectableCustomProperties](InstancedLinesMesh.md#inspectablecustomproperties)
- [instancedBuffers](InstancedLinesMesh.md#instancedbuffers)
- [intersectionThreshold](InstancedLinesMesh.md#intersectionthreshold)
- [isBlocker](InstancedLinesMesh.md#isblocker)
- [isNearGrabbable](InstancedLinesMesh.md#isneargrabbable)
- [isNearPickable](InstancedLinesMesh.md#isnearpickable)
- [isOccluded](InstancedLinesMesh.md#isoccluded)
- [isOcclusionQueryInProgress](InstancedLinesMesh.md#isocclusionqueryinprogress)
- [isPickable](InstancedLinesMesh.md#ispickable)
- [isVisible](InstancedLinesMesh.md#isvisible)
- [metadata](InstancedLinesMesh.md#metadata)
- [name](InstancedLinesMesh.md#name)
- [occlusionQueryAlgorithmType](InstancedLinesMesh.md#occlusionqueryalgorithmtype)
- [occlusionRetryCount](InstancedLinesMesh.md#occlusionretrycount)
- [occlusionType](InstancedLinesMesh.md#occlusiontype)
- [onAfterWorldMatrixUpdateObservable](InstancedLinesMesh.md#onafterworldmatrixupdateobservable)
- [onCollideObservable](InstancedLinesMesh.md#oncollideobservable)
- [onCollisionPositionChangeObservable](InstancedLinesMesh.md#oncollisionpositionchangeobservable)
- [onDisposeObservable](InstancedLinesMesh.md#ondisposeobservable)
- [onMaterialChangedObservable](InstancedLinesMesh.md#onmaterialchangedobservable)
- [onReady](InstancedLinesMesh.md#onready)
- [onRebuildObservable](InstancedLinesMesh.md#onrebuildobservable)
- [outlineColor](InstancedLinesMesh.md#outlinecolor)
- [outlineWidth](InstancedLinesMesh.md#outlinewidth)
- [overlayAlpha](InstancedLinesMesh.md#overlayalpha)
- [overlayColor](InstancedLinesMesh.md#overlaycolor)
- [physicsImpostor](InstancedLinesMesh.md#physicsimpostor)
- [reIntegrateRotationIntoRotationQuaternion](InstancedLinesMesh.md#reintegraterotationintorotationquaternion)
- [renderOutline](InstancedLinesMesh.md#renderoutline)
- [renderOverlay](InstancedLinesMesh.md#renderoverlay)
- [reservedDataStore](InstancedLinesMesh.md#reserveddatastore)
- [scalingDeterminant](InstancedLinesMesh.md#scalingdeterminant)
- [showBoundingBox](InstancedLinesMesh.md#showboundingbox)
- [showSubMeshesBoundingBox](InstancedLinesMesh.md#showsubmeshesboundingbox)
- [state](InstancedLinesMesh.md#state)
- [subMeshes](InstancedLinesMesh.md#submeshes)
- [uniqueId](InstancedLinesMesh.md#uniqueid)
- [useOctreeForCollisions](InstancedLinesMesh.md#useoctreeforcollisions)
- [useOctreeForPicking](InstancedLinesMesh.md#useoctreeforpicking)
- [useOctreeForRenderingSelection](InstancedLinesMesh.md#useoctreeforrenderingselection)
- [CULLINGSTRATEGY\_BOUNDINGSPHERE\_ONLY](InstancedLinesMesh.md#cullingstrategy_boundingsphere_only)
- [CULLINGSTRATEGY\_OPTIMISTIC\_INCLUSION](InstancedLinesMesh.md#cullingstrategy_optimistic_inclusion)
- [CULLINGSTRATEGY\_OPTIMISTIC\_INCLUSION\_THEN\_BSPHERE\_ONLY](InstancedLinesMesh.md#cullingstrategy_optimistic_inclusion_then_bsphere_only)
- [CULLINGSTRATEGY\_STANDARD](InstancedLinesMesh.md#cullingstrategy_standard)
- [OCCLUSION\_ALGORITHM\_TYPE\_ACCURATE](InstancedLinesMesh.md#occlusion_algorithm_type_accurate)
- [OCCLUSION\_ALGORITHM\_TYPE\_CONSERVATIVE](InstancedLinesMesh.md#occlusion_algorithm_type_conservative)
- [OCCLUSION\_TYPE\_NONE](InstancedLinesMesh.md#occlusion_type_none)
- [OCCLUSION\_TYPE\_OPTIMISTIC](InstancedLinesMesh.md#occlusion_type_optimistic)
- [OCCLUSION\_TYPE\_STRICT](InstancedLinesMesh.md#occlusion_type_strict)

### Accessors

- [\_positions](InstancedLinesMesh.md#_positions)
- [absolutePosition](InstancedLinesMesh.md#absoluteposition)
- [absoluteRotationQuaternion](InstancedLinesMesh.md#absoluterotationquaternion)
- [absoluteScaling](InstancedLinesMesh.md#absolutescaling)
- [animationPropertiesOverride](InstancedLinesMesh.md#animationpropertiesoverride)
- [applyFog](InstancedLinesMesh.md#applyfog)
- [bakedVertexAnimationManager](InstancedLinesMesh.md#bakedvertexanimationmanager)
- [behaviors](InstancedLinesMesh.md#behaviors)
- [billboardMode](InstancedLinesMesh.md#billboardmode)
- [checkCollisions](InstancedLinesMesh.md#checkcollisions)
- [collider](InstancedLinesMesh.md#collider)
- [collisionGroup](InstancedLinesMesh.md#collisiongroup)
- [collisionMask](InstancedLinesMesh.md#collisionmask)
- [collisionResponse](InstancedLinesMesh.md#collisionresponse)
- [collisionRetryCount](InstancedLinesMesh.md#collisionretrycount)
- [computeBonesUsingShaders](InstancedLinesMesh.md#computebonesusingshaders)
- [doNotSerialize](InstancedLinesMesh.md#donotserialize)
- [enableDistantPicking](InstancedLinesMesh.md#enabledistantpicking)
- [facetDepthSortFrom](InstancedLinesMesh.md#facetdepthsortfrom)
- [facetNb](InstancedLinesMesh.md#facetnb)
- [forward](InstancedLinesMesh.md#forward)
- [hasBoundingInfo](InstancedLinesMesh.md#hasboundinginfo)
- [hasInstances](InstancedLinesMesh.md#hasinstances)
- [hasThinInstances](InstancedLinesMesh.md#hasthininstances)
- [hasVertexAlpha](InstancedLinesMesh.md#hasvertexalpha)
- [infiniteDistance](InstancedLinesMesh.md#infinitedistance)
- [isAnInstance](InstancedLinesMesh.md#isaninstance)
- [isBlocked](InstancedLinesMesh.md#isblocked)
- [isFacetDataEnabled](InstancedLinesMesh.md#isfacetdataenabled)
- [isWorldMatrixFrozen](InstancedLinesMesh.md#isworldmatrixfrozen)
- [layerMask](InstancedLinesMesh.md#layermask)
- [lightSources](InstancedLinesMesh.md#lightsources)
- [material](InstancedLinesMesh.md#material)
- [morphTargetManager](InstancedLinesMesh.md#morphtargetmanager)
- [mustDepthSortFacets](InstancedLinesMesh.md#mustdepthsortfacets)
- [nonUniformScaling](InstancedLinesMesh.md#nonuniformscaling)
- [numBoneInfluencers](InstancedLinesMesh.md#numboneinfluencers)
- [onClonedObservable](InstancedLinesMesh.md#onclonedobservable)
- [onCollide](InstancedLinesMesh.md#oncollide)
- [onCollisionPositionChange](InstancedLinesMesh.md#oncollisionpositionchange)
- [onDispose](InstancedLinesMesh.md#ondispose)
- [onEnabledStateChangedObservable](InstancedLinesMesh.md#onenabledstatechangedobservable)
- [parent](InstancedLinesMesh.md#parent)
- [partitioningBBoxRatio](InstancedLinesMesh.md#partitioningbboxratio)
- [partitioningSubdivisions](InstancedLinesMesh.md#partitioningsubdivisions)
- [position](InstancedLinesMesh.md#position)
- [preserveParentRotationForBillboard](InstancedLinesMesh.md#preserveparentrotationforbillboard)
- [receiveShadows](InstancedLinesMesh.md#receiveshadows)
- [renderingGroupId](InstancedLinesMesh.md#renderinggroupid)
- [right](InstancedLinesMesh.md#right)
- [rotation](InstancedLinesMesh.md#rotation)
- [rotationQuaternion](InstancedLinesMesh.md#rotationquaternion)
- [scaling](InstancedLinesMesh.md#scaling)
- [skeleton](InstancedLinesMesh.md#skeleton)
- [sourceMesh](InstancedLinesMesh.md#sourcemesh)
- [surroundingMeshes](InstancedLinesMesh.md#surroundingmeshes)
- [up](InstancedLinesMesh.md#up)
- [useBones](InstancedLinesMesh.md#usebones)
- [useVertexColors](InstancedLinesMesh.md#usevertexcolors)
- [visibility](InstancedLinesMesh.md#visibility)
- [worldMatrixFromCache](InstancedLinesMesh.md#worldmatrixfromcache)
- [BILLBOARDMODE\_ALL](InstancedLinesMesh.md#billboardmode_all)
- [BILLBOARDMODE\_NONE](InstancedLinesMesh.md#billboardmode_none)
- [BILLBOARDMODE\_USE\_POSITION](InstancedLinesMesh.md#billboardmode_use_position)
- [BILLBOARDMODE\_X](InstancedLinesMesh.md#billboardmode_x)
- [BILLBOARDMODE\_Y](InstancedLinesMesh.md#billboardmode_y)
- [BILLBOARDMODE\_Z](InstancedLinesMesh.md#billboardmode_z)

### Methods

- [\_buildUniformLayout](InstancedLinesMesh.md#_builduniformlayout)
- [\_removeLightSource](InstancedLinesMesh.md#_removelightsource)
- [\_resyncLightSource](InstancedLinesMesh.md#_resynclightsource)
- [\_resyncLightSources](InstancedLinesMesh.md#_resynclightsources)
- [addBehavior](InstancedLinesMesh.md#addbehavior)
- [addChild](InstancedLinesMesh.md#addchild)
- [addRotation](InstancedLinesMesh.md#addrotation)
- [alignWithNormal](InstancedLinesMesh.md#alignwithnormal)
- [applyImpulse](InstancedLinesMesh.md#applyimpulse)
- [attachToBone](InstancedLinesMesh.md#attachtobone)
- [beginAnimation](InstancedLinesMesh.md#beginanimation)
- [buildBoundingInfo](InstancedLinesMesh.md#buildboundinginfo)
- [calcMovePOV](InstancedLinesMesh.md#calcmovepov)
- [calcRotatePOV](InstancedLinesMesh.md#calcrotatepov)
- [clone](InstancedLinesMesh.md#clone)
- [computeWorldMatrix](InstancedLinesMesh.md#computeworldmatrix)
- [createAnimationRange](InstancedLinesMesh.md#createanimationrange)
- [createInstance](InstancedLinesMesh.md#createinstance)
- [createNormals](InstancedLinesMesh.md#createnormals)
- [createOrUpdateSubmeshesOctree](InstancedLinesMesh.md#createorupdatesubmeshesoctree)
- [deleteAnimationRange](InstancedLinesMesh.md#deleteanimationrange)
- [detachFromBone](InstancedLinesMesh.md#detachfrombone)
- [disableEdgesRendering](InstancedLinesMesh.md#disableedgesrendering)
- [disableFacetData](InstancedLinesMesh.md#disablefacetdata)
- [dispose](InstancedLinesMesh.md#dispose)
- [enableEdgesRendering](InstancedLinesMesh.md#enableedgesrendering)
- [freezeWorldMatrix](InstancedLinesMesh.md#freezeworldmatrix)
- [getAbsolutePivotPoint](InstancedLinesMesh.md#getabsolutepivotpoint)
- [getAbsolutePivotPointToRef](InstancedLinesMesh.md#getabsolutepivotpointtoref)
- [getAbsolutePosition](InstancedLinesMesh.md#getabsoluteposition)
- [getAnimationByName](InstancedLinesMesh.md#getanimationbyname)
- [getAnimationRange](InstancedLinesMesh.md#getanimationrange)
- [getAnimationRanges](InstancedLinesMesh.md#getanimationranges)
- [getBehaviorByName](InstancedLinesMesh.md#getbehaviorbyname)
- [getBoundingInfo](InstancedLinesMesh.md#getboundinginfo)
- [getChildMeshes](InstancedLinesMesh.md#getchildmeshes)
- [getChildTransformNodes](InstancedLinesMesh.md#getchildtransformnodes)
- [getChildren](InstancedLinesMesh.md#getchildren)
- [getClassName](InstancedLinesMesh.md#getclassname)
- [getClosestFacetAtCoordinates](InstancedLinesMesh.md#getclosestfacetatcoordinates)
- [getClosestFacetAtLocalCoordinates](InstancedLinesMesh.md#getclosestfacetatlocalcoordinates)
- [getConnectedParticleSystems](InstancedLinesMesh.md#getconnectedparticlesystems)
- [getDescendants](InstancedLinesMesh.md#getdescendants)
- [getDirection](InstancedLinesMesh.md#getdirection)
- [getDirectionToRef](InstancedLinesMesh.md#getdirectiontoref)
- [getDistanceToCamera](InstancedLinesMesh.md#getdistancetocamera)
- [getEngine](InstancedLinesMesh.md#getengine)
- [getFacetDataParameters](InstancedLinesMesh.md#getfacetdataparameters)
- [getFacetLocalNormals](InstancedLinesMesh.md#getfacetlocalnormals)
- [getFacetLocalPartitioning](InstancedLinesMesh.md#getfacetlocalpartitioning)
- [getFacetLocalPositions](InstancedLinesMesh.md#getfacetlocalpositions)
- [getFacetNormal](InstancedLinesMesh.md#getfacetnormal)
- [getFacetNormalToRef](InstancedLinesMesh.md#getfacetnormaltoref)
- [getFacetPosition](InstancedLinesMesh.md#getfacetposition)
- [getFacetPositionToRef](InstancedLinesMesh.md#getfacetpositiontoref)
- [getFacetsAtLocalCoordinates](InstancedLinesMesh.md#getfacetsatlocalcoordinates)
- [getHierarchyBoundingVectors](InstancedLinesMesh.md#gethierarchyboundingvectors)
- [getIndices](InstancedLinesMesh.md#getindices)
- [getLOD](InstancedLinesMesh.md#getlod)
- [getMaterialForRenderPass](InstancedLinesMesh.md#getmaterialforrenderpass)
- [getMeshUniformBuffer](InstancedLinesMesh.md#getmeshuniformbuffer)
- [getNormalsData](InstancedLinesMesh.md#getnormalsdata)
- [getPhysicsImpostor](InstancedLinesMesh.md#getphysicsimpostor)
- [getPivotMatrix](InstancedLinesMesh.md#getpivotmatrix)
- [getPivotPoint](InstancedLinesMesh.md#getpivotpoint)
- [getPivotPointToRef](InstancedLinesMesh.md#getpivotpointtoref)
- [getPoseMatrix](InstancedLinesMesh.md#getposematrix)
- [getPositionData](InstancedLinesMesh.md#getpositiondata)
- [getPositionExpressedInLocalSpace](InstancedLinesMesh.md#getpositionexpressedinlocalspace)
- [getPositionInCameraSpace](InstancedLinesMesh.md#getpositionincameraspace)
- [getScene](InstancedLinesMesh.md#getscene)
- [getTotalIndices](InstancedLinesMesh.md#gettotalindices)
- [getTotalVertices](InstancedLinesMesh.md#gettotalvertices)
- [getVerticesData](InstancedLinesMesh.md#getverticesdata)
- [getWorldMatrix](InstancedLinesMesh.md#getworldmatrix)
- [instantiateHierarchy](InstancedLinesMesh.md#instantiatehierarchy)
- [intersects](InstancedLinesMesh.md#intersects)
- [intersectsMesh](InstancedLinesMesh.md#intersectsmesh)
- [intersectsPoint](InstancedLinesMesh.md#intersectspoint)
- [isCompletelyInFrustum](InstancedLinesMesh.md#iscompletelyinfrustum)
- [isDescendantOf](InstancedLinesMesh.md#isdescendantof)
- [isDisposed](InstancedLinesMesh.md#isdisposed)
- [isEnabled](InstancedLinesMesh.md#isenabled)
- [isInFrustum](InstancedLinesMesh.md#isinfrustum)
- [isReady](InstancedLinesMesh.md#isready)
- [isUsingPivotMatrix](InstancedLinesMesh.md#isusingpivotmatrix)
- [isVerticesDataPresent](InstancedLinesMesh.md#isverticesdatapresent)
- [locallyTranslate](InstancedLinesMesh.md#locallytranslate)
- [lookAt](InstancedLinesMesh.md#lookat)
- [markAsDirty](InstancedLinesMesh.md#markasdirty)
- [movePOV](InstancedLinesMesh.md#movepov)
- [moveWithCollisions](InstancedLinesMesh.md#movewithcollisions)
- [normalizeToUnitCube](InstancedLinesMesh.md#normalizetounitcube)
- [refreshBoundingInfo](InstancedLinesMesh.md#refreshboundinginfo)
- [registerAfterWorldMatrixUpdate](InstancedLinesMesh.md#registerafterworldmatrixupdate)
- [releaseSubMeshes](InstancedLinesMesh.md#releasesubmeshes)
- [removeBehavior](InstancedLinesMesh.md#removebehavior)
- [removeChild](InstancedLinesMesh.md#removechild)
- [resetDrawCache](InstancedLinesMesh.md#resetdrawcache)
- [resetLocalMatrix](InstancedLinesMesh.md#resetlocalmatrix)
- [rotate](InstancedLinesMesh.md#rotate)
- [rotateAround](InstancedLinesMesh.md#rotatearound)
- [rotatePOV](InstancedLinesMesh.md#rotatepov)
- [serialize](InstancedLinesMesh.md#serialize)
- [serializeAnimationRanges](InstancedLinesMesh.md#serializeanimationranges)
- [setAbsolutePosition](InstancedLinesMesh.md#setabsoluteposition)
- [setBoundingInfo](InstancedLinesMesh.md#setboundinginfo)
- [setDirection](InstancedLinesMesh.md#setdirection)
- [setEnabled](InstancedLinesMesh.md#setenabled)
- [setIndices](InstancedLinesMesh.md#setindices)
- [setMaterialForRenderPass](InstancedLinesMesh.md#setmaterialforrenderpass)
- [setParent](InstancedLinesMesh.md#setparent)
- [setPhysicsLinkWith](InstancedLinesMesh.md#setphysicslinkwith)
- [setPivotMatrix](InstancedLinesMesh.md#setpivotmatrix)
- [setPivotPoint](InstancedLinesMesh.md#setpivotpoint)
- [setPositionWithLocalVector](InstancedLinesMesh.md#setpositionwithlocalvector)
- [setPreTransformMatrix](InstancedLinesMesh.md#setpretransformmatrix)
- [setVerticesData](InstancedLinesMesh.md#setverticesdata)
- [toString](InstancedLinesMesh.md#tostring)
- [transferToEffect](InstancedLinesMesh.md#transfertoeffect)
- [translate](InstancedLinesMesh.md#translate)
- [unfreezeWorldMatrix](InstancedLinesMesh.md#unfreezeworldmatrix)
- [unregisterAfterWorldMatrixUpdate](InstancedLinesMesh.md#unregisterafterworldmatrixupdate)
- [updateFacetData](InstancedLinesMesh.md#updatefacetdata)
- [updateIndices](InstancedLinesMesh.md#updateindices)
- [updatePoseMatrix](InstancedLinesMesh.md#updateposematrix)
- [updateVerticesData](InstancedLinesMesh.md#updateverticesdata)
- [AddNodeConstructor](InstancedLinesMesh.md#addnodeconstructor)
- [Construct](InstancedLinesMesh.md#construct)
- [Parse](InstancedLinesMesh.md#parse)
- [ParseAnimationRanges](InstancedLinesMesh.md#parseanimationranges)

## Constructors

### constructor

• **new InstancedLinesMesh**(`name`, `source`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `source` | [`LinesMesh`](LinesMesh.md) |

#### Overrides

[InstancedMesh](InstancedMesh.md).[constructor](InstancedMesh.md#constructor)

#### Defined in

packages/dev/core/src/Meshes/linesMesh.ts:286

## Properties

### \_boundingInfo

• `Protected` **\_boundingInfo**: [`Nullable`](../modules.md#nullable)[`BoundingInfo`](BoundingInfo.md) = `null`

#### Inherited from

[InstancedMesh](InstancedMesh.md).[_boundingInfo](InstancedMesh.md#_boundinginfo)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:729

___

### \_boundingInfoIsDirty

• `Protected` **\_boundingInfoIsDirty**: `boolean` = `true`

#### Inherited from

[InstancedMesh](InstancedMesh.md).[_boundingInfoIsDirty](InstancedMesh.md#_boundinginfoisdirty)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:730

___

### \_isDirty

• `Protected` **\_isDirty**: `boolean` = `false`

#### Inherited from

[InstancedMesh](InstancedMesh.md).[_isDirty](InstancedMesh.md#_isdirty)

#### Defined in

packages/dev/core/src/node.ts:43

___

### \_isWorldMatrixFrozen

• `Protected` **\_isWorldMatrixFrozen**: `boolean` = `false`

#### Inherited from

[InstancedMesh](InstancedMesh.md).[_isWorldMatrixFrozen](InstancedMesh.md#_isworldmatrixfrozen)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:161

___

### \_parentNode

• `Protected` **\_parentNode**: [`Nullable`](../modules.md#nullable)[`Node`](Node.md) = `null`

#### Inherited from

[InstancedMesh](InstancedMesh.md).[_parentNode](InstancedMesh.md#_parentnode)

#### Defined in

packages/dev/core/src/node.ts:176

___

### \_ranges

• `Protected` **\_ranges**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: [`Nullable`](../modules.md#nullable)`AnimationRange`

#### Inherited from

[InstancedMesh](InstancedMesh.md).[_ranges](InstancedMesh.md#_ranges)

#### Defined in

packages/dev/core/src/node.ts:154

___

### \_scaling

• `Protected` **\_scaling**: [`Vector3`](Vector3.md)

#### Inherited from

[InstancedMesh](InstancedMesh.md).[_scaling](InstancedMesh.md#_scaling)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:62

___

### actionManager

• **actionManager**: [`Nullable`](../modules.md#nullable)[`AbstractActionManager`](AbstractActionManager.md) = `null`

Gets or sets the current action manager

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions

#### Inherited from

[InstancedMesh](InstancedMesh.md).[actionManager](InstancedMesh.md#actionmanager)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:646

___

### alphaIndex

• **alphaIndex**: `number` = `Number.MAX_VALUE`

Gets or sets the alpha index used to sort transparent meshes

**`See`**

https://doc.babylonjs.com/resources/transparency_and_how_meshes_are_rendered#alpha-index

#### Inherited from

[InstancedMesh](InstancedMesh.md).[alphaIndex](InstancedMesh.md#alphaindex)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:406

___

### alwaysSelectAsActiveMesh

• **alwaysSelectAsActiveMesh**: `boolean` = `false`

True if the mesh must be rendered in any case (this will shortcut the frustum clipping phase)

#### Inherited from

[InstancedMesh](InstancedMesh.md).[alwaysSelectAsActiveMesh](InstancedMesh.md#alwaysselectasactivemesh)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:635

___

### animations

• **animations**: [`Animation`](Animation.md)[]

Gets a list of Animations associated with the node

#### Inherited from

[InstancedMesh](InstancedMesh.md).[animations](InstancedMesh.md#animations)

#### Defined in

packages/dev/core/src/node.ts:153

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[cullingStrategy](InstancedMesh.md#cullingstrategy)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:214

___

### definedFacingForward

• **definedFacingForward**: `boolean` = `true`

Gets or sets the orientation for POV movement & rotation

#### Inherited from

[InstancedMesh](InstancedMesh.md).[definedFacingForward](InstancedMesh.md#definedfacingforward)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:371

___

### doNotSyncBoundingInfo

• **doNotSyncBoundingInfo**: `boolean` = `false`

Gets or sets a boolean indicating that the bounding info does not need to be kept in sync (for performance reason)

#### Inherited from

[InstancedMesh](InstancedMesh.md).[doNotSyncBoundingInfo](InstancedMesh.md#donotsyncboundinginfo)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:640

___

### edgesColor

• **edgesColor**: [`Color4`](Color4.md)

Defines edge color used when edgesRenderer is enabled

**`See`**

https://www.babylonjs-playground.com/#10OJSG#13

#### Inherited from

[InstancedMesh](InstancedMesh.md).[edgesColor](InstancedMesh.md#edgescolor)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:723

___

### edgesRenderer

• **edgesRenderer**: [`Nullable`](../modules.md#nullable)[`EdgesRenderer`](EdgesRenderer.md)

Gets the edgesRenderer associated with the mesh

#### Inherited from

[InstancedMesh](InstancedMesh.md).[edgesRenderer](InstancedMesh.md#edgesrenderer)

#### Defined in

packages/dev/core/src/Rendering/edgesRenderer.ts:35

___

### edgesWidth

• **edgesWidth**: `number` = `1`

Defines edge width used when edgesRenderer is enabled

**`See`**

https://www.babylonjs-playground.com/#10OJSG#13

#### Inherited from

[InstancedMesh](InstancedMesh.md).[edgesWidth](InstancedMesh.md#edgeswidth)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:718

___

### ellipsoid

• **ellipsoid**: [`Vector3`](Vector3.md)

Gets or sets the ellipsoid used to impersonate this mesh when using collision engine (default is (0.5, 1, 0.5))

**`See`**

https://doc.babylonjs.com/babylon101/cameras,_mesh_collisions_and_gravity

#### Inherited from

[InstancedMesh](InstancedMesh.md).[ellipsoid](InstancedMesh.md#ellipsoid)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:652

___

### ellipsoidOffset

• **ellipsoidOffset**: [`Vector3`](Vector3.md)

Gets or sets the ellipsoid offset used to impersonate this mesh when using collision engine (default is (0, 0, 0))

**`See`**

https://doc.babylonjs.com/babylon101/cameras,_mesh_collisions_and_gravity

#### Inherited from

[InstancedMesh](InstancedMesh.md).[ellipsoidOffset](InstancedMesh.md#ellipsoidoffset)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:657

___

### enablePointerMoveEvents

• **enablePointerMoveEvents**: `boolean` = `false`

Gets or sets a boolean indicating that pointer move events must be supported on this mesh (false by default)

#### Inherited from

[InstancedMesh](InstancedMesh.md).[enablePointerMoveEvents](InstancedMesh.md#enablepointermoveevents)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:439

___

### forceRenderingWhenOccluded

• **forceRenderingWhenOccluded**: `boolean`

Flag to force rendering the mesh even if occluded

**`See`**

https://doc.babylonjs.com/features/occlusionquery

#### Inherited from

[InstancedMesh](InstancedMesh.md).[forceRenderingWhenOccluded](InstancedMesh.md#forcerenderingwhenoccluded)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.query.ts:405

___

### id

• **id**: `string`

Gets or sets the id of the node

#### Inherited from

[InstancedMesh](InstancedMesh.md).[id](InstancedMesh.md#id)

#### Defined in

packages/dev/core/src/node.ts:97

___

### ignoreNonUniformScaling

• **ignoreNonUniformScaling**: `boolean` = `false`

Gets or sets a boolean indicating that non uniform scaling (when at least one component is different from others) should be ignored.
By default the system will update normals to compensate

#### Inherited from

[InstancedMesh](InstancedMesh.md).[ignoreNonUniformScaling](InstancedMesh.md#ignorenonuniformscaling)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:138

___

### inspectableCustomProperties

• **inspectableCustomProperties**: [`IInspectable`](../interfaces/IInspectable.md)[]

List of inspectable custom properties (used by the Inspector)

**`See`**

https://doc.babylonjs.com/how_to/debug_layer#extensibility

#### Inherited from

[InstancedMesh](InstancedMesh.md).[inspectableCustomProperties](InstancedMesh.md#inspectablecustomproperties)

#### Defined in

packages/dev/core/src/node.ts:126

___

### instancedBuffers

• **instancedBuffers**: `Object`

Object used to store instanced buffers defined by user

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_instances#custom-buffers

#### Index signature

▪ [key: `string`]: `any`

#### Inherited from

[InstancedMesh](InstancedMesh.md).[instancedBuffers](InstancedMesh.md#instancedbuffers)

#### Defined in

packages/dev/core/src/Meshes/instancedMesh.ts:594

___

### intersectionThreshold

• **intersectionThreshold**: `number`

The intersection Threshold is the margin applied when intersection a segment of the LinesMesh with a Ray.
This margin is expressed in world space coordinates, so its value may vary.
Initialized with the intersectionThreshold value of the source LinesMesh

#### Defined in

packages/dev/core/src/Meshes/linesMesh.ts:284

___

### isBlocker

• **isBlocker**: `boolean` = `false`

Gets or sets a boolean indicating if the mesh must be considered as a ray blocker for lens flares (false by default)

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_lens_flares

#### Inherited from

[InstancedMesh](InstancedMesh.md).[isBlocker](InstancedMesh.md#isblocker)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:434

___

### isNearGrabbable

• **isNearGrabbable**: `boolean` = `false`

Gets or sets a boolean indicating if the mesh can be near grabbed. Default is false

#### Inherited from

[InstancedMesh](InstancedMesh.md).[isNearGrabbable](InstancedMesh.md#isneargrabbable)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:426

___

### isNearPickable

• **isNearPickable**: `boolean` = `false`

Gets or sets a boolean indicating if the mesh can be near picked. Default is false

#### Inherited from

[InstancedMesh](InstancedMesh.md).[isNearPickable](InstancedMesh.md#isnearpickable)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:421

___

### isOccluded

• **isOccluded**: `boolean`

Gets or sets whether the mesh is occluded or not, it is used also to set the initial state of the mesh to be occluded or not

**`See`**

https://doc.babylonjs.com/features/occlusionquery

#### Inherited from

[InstancedMesh](InstancedMesh.md).[isOccluded](InstancedMesh.md#isoccluded)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.query.ts:393

___

### isOcclusionQueryInProgress

• **isOcclusionQueryInProgress**: `boolean`

Flag to check the progress status of the query

**`See`**

https://doc.babylonjs.com/features/occlusionquery

#### Inherited from

[InstancedMesh](InstancedMesh.md).[isOcclusionQueryInProgress](InstancedMesh.md#isocclusionqueryinprogress)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.query.ts:399

___

### isPickable

• **isPickable**: `boolean` = `true`

Gets or sets a boolean indicating if the mesh can be picked (by scene.pick for instance or through actions). Default is true

#### Inherited from

[InstancedMesh](InstancedMesh.md).[isPickable](InstancedMesh.md#ispickable)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:416

___

### isVisible

• **isVisible**: `boolean` = `true`

Gets or sets a boolean indicating if the mesh is visible (renderable). Default is true

#### Inherited from

[InstancedMesh](InstancedMesh.md).[isVisible](InstancedMesh.md#isvisible)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:411

___

### metadata

• **metadata**: `any` = `null`

Gets or sets an object used to store user defined information for the node

#### Inherited from

[InstancedMesh](InstancedMesh.md).[metadata](InstancedMesh.md#metadata)

#### Defined in

packages/dev/core/src/node.ts:115

___

### name

• **name**: `string`

Gets or sets the name of the node

#### Inherited from

[InstancedMesh](InstancedMesh.md).[name](InstancedMesh.md#name)

#### Defined in

packages/dev/core/src/node.ts:91

___

### occlusionQueryAlgorithmType

• **occlusionQueryAlgorithmType**: `number`

This property determines the type of occlusion query algorithm to run in WebGl, you can use:
* AbstractMesh.OCCLUSION_ALGORITHM_TYPE_ACCURATE which is mapped to GL_ANY_SAMPLES_PASSED.
* AbstractMesh.OCCLUSION_ALGORITHM_TYPE_CONSERVATIVE (Default Value) which is mapped to GL_ANY_SAMPLES_PASSED_CONSERVATIVE which is a false positive algorithm that is faster than GL_ANY_SAMPLES_PASSED but less accurate.

**`See`**

https://doc.babylonjs.com/features/occlusionquery

#### Inherited from

[InstancedMesh](InstancedMesh.md).[occlusionQueryAlgorithmType](InstancedMesh.md#occlusionqueryalgorithmtype)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.query.ts:387

___

### occlusionRetryCount

• **occlusionRetryCount**: `number`

This number indicates the number of allowed retries before stop the occlusion query, this is useful if the occlusion query is taking long time before to the query result is retrieved, the query result indicates if the object is visible within the scene or not and based on that Babylon.Js engine decides to show or hide the object.
The default value is -1 which means don't break the query and wait till the result

**`See`**

https://doc.babylonjs.com/features/occlusionquery

#### Inherited from

[InstancedMesh](InstancedMesh.md).[occlusionRetryCount](InstancedMesh.md#occlusionretrycount)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.query.ts:370

___

### occlusionType

• **occlusionType**: `number`

This property is responsible for starting the occlusion query within the Mesh or not, this property is also used to determine what should happen when the occlusionRetryCount is reached. It has supports 3 values:
* OCCLUSION_TYPE_NONE (Default Value): this option means no occlusion query within the Mesh.
* OCCLUSION_TYPE_OPTIMISTIC: this option is means use occlusion query and if occlusionRetryCount is reached and the query is broken show the mesh.
* OCCLUSION_TYPE_STRICT: this option is means use occlusion query and if occlusionRetryCount is reached and the query is broken restore the last state of the mesh occlusion if the mesh was visible then show the mesh if was hidden then hide don't show.

**`See`**

https://doc.babylonjs.com/features/occlusionquery

#### Inherited from

[InstancedMesh](InstancedMesh.md).[occlusionType](InstancedMesh.md#occlusiontype)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.query.ts:379

___

### onAfterWorldMatrixUpdateObservable

• **onAfterWorldMatrixUpdateObservable**: [`Observable`](Observable.md)[`TransformNode`](TransformNode.md)

An event triggered after the world matrix is updated

#### Inherited from

[InstancedMesh](InstancedMesh.md).[onAfterWorldMatrixUpdateObservable](InstancedMesh.md#onafterworldmatrixupdateobservable)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:169

___

### onCollideObservable

• **onCollideObservable**: [`Observable`](Observable.md)[`AbstractMesh`](AbstractMesh.md)

An event triggered when this mesh collides with another one

#### Inherited from

[InstancedMesh](InstancedMesh.md).[onCollideObservable](InstancedMesh.md#oncollideobservable)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:338

___

### onCollisionPositionChangeObservable

• **onCollisionPositionChangeObservable**: [`Observable`](Observable.md)[`Vector3`](Vector3.md)

An event triggered when the collision's position changes

#### Inherited from

[InstancedMesh](InstancedMesh.md).[onCollisionPositionChangeObservable](InstancedMesh.md#oncollisionpositionchangeobservable)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:351

___

### onDisposeObservable

• **onDisposeObservable**: [`Observable`](Observable.md)[`Node`](Node.md)

An event triggered when the mesh is disposed

#### Inherited from

[InstancedMesh](InstancedMesh.md).[onDisposeObservable](InstancedMesh.md#ondisposeobservable)

#### Defined in

packages/dev/core/src/node.ts:300

___

### onMaterialChangedObservable

• **onMaterialChangedObservable**: [`Observable`](Observable.md)[`AbstractMesh`](AbstractMesh.md)

An event triggered when material is changed

#### Inherited from

[InstancedMesh](InstancedMesh.md).[onMaterialChangedObservable](InstancedMesh.md#onmaterialchangedobservable)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:364

___

### onReady

• **onReady**: [`Nullable`](../modules.md#nullable)(`node`: [`Node`](Node.md)) => `void` = `null`

Callback raised when the node is ready to be used

#### Inherited from

[InstancedMesh](InstancedMesh.md).[onReady](InstancedMesh.md#onready)

#### Defined in

packages/dev/core/src/node.ts:159

___

### onRebuildObservable

• **onRebuildObservable**: [`Observable`](Observable.md)[`AbstractMesh`](AbstractMesh.md)

An event triggered when the mesh is rebuilt.

#### Inherited from

[InstancedMesh](InstancedMesh.md).[onRebuildObservable](InstancedMesh.md#onrebuildobservable)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:807

___

### outlineColor

• **outlineColor**: [`Color3`](Color3.md)

Defines color to use when rendering outline

#### Inherited from

[InstancedMesh](InstancedMesh.md).[outlineColor](InstancedMesh.md#outlinecolor)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:524

___

### outlineWidth

• **outlineWidth**: `number` = `0.02`

Define width to use when rendering outline

#### Inherited from

[InstancedMesh](InstancedMesh.md).[outlineWidth](InstancedMesh.md#outlinewidth)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:526

___

### overlayAlpha

• **overlayAlpha**: `number` = `0.5`

Defines alpha to use when rendering overlay

#### Inherited from

[InstancedMesh](InstancedMesh.md).[overlayAlpha](InstancedMesh.md#overlayalpha)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:531

___

### overlayColor

• **overlayColor**: [`Color3`](Color3.md)

Defines color to use when rendering overlay

#### Inherited from

[InstancedMesh](InstancedMesh.md).[overlayColor](InstancedMesh.md#overlaycolor)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:529

___

### physicsImpostor

• **physicsImpostor**: [`Nullable`](../modules.md#nullable)[`PhysicsImpostor`](PhysicsImpostor.md)

Gets or sets impostor used for physic simulation

**`See`**

https://doc.babylonjs.com/features/physics_engine

#### Inherited from

[InstancedMesh](InstancedMesh.md).[physicsImpostor](InstancedMesh.md#physicsimpostor)

#### Defined in

packages/dev/core/src/Physics/physicsEngineComponent.ts:169

___

### reIntegrateRotationIntoRotationQuaternion

• **reIntegrateRotationIntoRotationQuaternion**: `boolean` = `false`

Gets or sets a boolean indicating that even if rotationQuaternion is defined, you can keep updating rotation property and Babylon.js will just mix both

#### Inherited from

[InstancedMesh](InstancedMesh.md).[reIntegrateRotationIntoRotationQuaternion](InstancedMesh.md#reintegraterotationintorotationquaternion)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:144

___

### renderOutline

• **renderOutline**: `boolean`

Gets or sets a boolean indicating if the outline must be rendered as well

**`See`**

https://www.babylonjs-playground.com/#10WJ5S#3

#### Inherited from

[InstancedMesh](InstancedMesh.md).[renderOutline](InstancedMesh.md#renderoutline)

#### Defined in

packages/dev/core/src/Rendering/outlineRenderer.ts:48

___

### renderOverlay

• **renderOverlay**: `boolean`

Gets or sets a boolean indicating if the overlay must be rendered as well

**`See`**

https://www.babylonjs-playground.com/#10WJ5S#2

#### Inherited from

[InstancedMesh](InstancedMesh.md).[renderOverlay](InstancedMesh.md#renderoverlay)

#### Defined in

packages/dev/core/src/Rendering/outlineRenderer.ts:56

___

### reservedDataStore

• **reservedDataStore**: `any` = `null`

For internal use only. Please do not use.

#### Inherited from

[InstancedMesh](InstancedMesh.md).[reservedDataStore](InstancedMesh.md#reserveddatastore)

#### Defined in

packages/dev/core/src/node.ts:120

___

### scalingDeterminant

• **scalingDeterminant**: `number` = `1`

Multiplication factor on scale x/y/z when computing the world matrix. Eg. for a 1x1x1 cube setting this to 2 will make it a 2x2x2 cube

#### Inherited from

[InstancedMesh](InstancedMesh.md).[scalingDeterminant](InstancedMesh.md#scalingdeterminant)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:113

___

### showBoundingBox

• **showBoundingBox**: `boolean`

Gets or sets a boolean indicating if the bounding box must be rendered as well (false by default)

#### Inherited from

[InstancedMesh](InstancedMesh.md).[showBoundingBox](InstancedMesh.md#showboundingbox)

#### Defined in

packages/dev/core/src/Rendering/boundingBoxRenderer.ts:76

___

### showSubMeshesBoundingBox

• **showSubMeshesBoundingBox**: `boolean` = `false`

Gets or sets a boolean indicating that bounding boxes of subMeshes must be rendered as well (false by default)

#### Inherited from

[InstancedMesh](InstancedMesh.md).[showSubMeshesBoundingBox](InstancedMesh.md#showsubmeshesboundingbox)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:429

___

### state

• **state**: `string` = `""`

Gets or sets a string used to store user defined state for the node

#### Inherited from

[InstancedMesh](InstancedMesh.md).[state](InstancedMesh.md#state)

#### Defined in

packages/dev/core/src/node.ts:109

___

### subMeshes

• **subMeshes**: [`SubMesh`](SubMesh.md)[]

Gets or sets the list of subMeshes

**`See`**

https://doc.babylonjs.com/how_to/multi_materials

#### Inherited from

[InstancedMesh](InstancedMesh.md).[subMeshes](InstancedMesh.md#submeshes)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:738

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the node

#### Inherited from

[InstancedMesh](InstancedMesh.md).[uniqueId](InstancedMesh.md#uniqueid)

#### Defined in

packages/dev/core/src/node.ts:103

___

### useOctreeForCollisions

• **useOctreeForCollisions**: `boolean` = `true`

Gets or sets a boolean indicating that internal octree (if available) can be used to boost submeshes collision (true by default)

#### Inherited from

[InstancedMesh](InstancedMesh.md).[useOctreeForCollisions](InstancedMesh.md#useoctreeforcollisions)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:614

___

### useOctreeForPicking

• **useOctreeForPicking**: `boolean` = `true`

Gets or sets a boolean indicating that internal octree (if available) can be used to boost submeshes picking (true by default)

#### Inherited from

[InstancedMesh](InstancedMesh.md).[useOctreeForPicking](InstancedMesh.md#useoctreeforpicking)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:612

___

### useOctreeForRenderingSelection

• **useOctreeForRenderingSelection**: `boolean` = `true`

Gets or sets a boolean indicating that internal octree (if available) can be used to boost submeshes selection (true by default)

#### Inherited from

[InstancedMesh](InstancedMesh.md).[useOctreeForRenderingSelection](InstancedMesh.md#useoctreeforrenderingselection)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:610

___

### CULLINGSTRATEGY\_BOUNDINGSPHERE\_ONLY

▪ `Static` `Readonly` **CULLINGSTRATEGY\_BOUNDINGSPHERE\_ONLY**: ``1``

Culling strategy : Bounding Sphere Only.
 This is an exclusion test. It's faster than the standard strategy because the bounding box is not tested.
 It's also less accurate than the standard because some not visible objects can still be selected.
 Test : is the bounding sphere outside the frustum ?
 If not, then the cullable object is in the frustum.

#### Inherited from

[InstancedMesh](InstancedMesh.md).[CULLINGSTRATEGY_BOUNDINGSPHERE_ONLY](InstancedMesh.md#cullingstrategy_boundingsphere_only)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:143

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[CULLINGSTRATEGY_OPTIMISTIC_INCLUSION](InstancedMesh.md#cullingstrategy_optimistic_inclusion)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:153

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[CULLINGSTRATEGY_OPTIMISTIC_INCLUSION_THEN_BSPHERE_ONLY](InstancedMesh.md#cullingstrategy_optimistic_inclusion_then_bsphere_only)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:163

___

### CULLINGSTRATEGY\_STANDARD

▪ `Static` `Readonly` **CULLINGSTRATEGY\_STANDARD**: ``0``

Default culling strategy : this is an exclusion test and it's the more accurate.
 Test order :
 Is the bounding sphere outside the frustum ?
 If not, are the bounding box vertices outside the frustum ?
 It not, then the cullable object is in the frustum.

#### Inherited from

[InstancedMesh](InstancedMesh.md).[CULLINGSTRATEGY_STANDARD](InstancedMesh.md#cullingstrategy_standard)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:136

___

### OCCLUSION\_ALGORITHM\_TYPE\_ACCURATE

▪ `Static` **OCCLUSION\_ALGORITHM\_TYPE\_ACCURATE**: `number` = `0`

Use an accurate occlusion algorithm

#### Inherited from

[InstancedMesh](InstancedMesh.md).[OCCLUSION_ALGORITHM_TYPE_ACCURATE](InstancedMesh.md#occlusion_algorithm_type_accurate)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:126

___

### OCCLUSION\_ALGORITHM\_TYPE\_CONSERVATIVE

▪ `Static` **OCCLUSION\_ALGORITHM\_TYPE\_CONSERVATIVE**: `number` = `1`

Use a conservative occlusion algorithm

#### Inherited from

[InstancedMesh](InstancedMesh.md).[OCCLUSION_ALGORITHM_TYPE_CONSERVATIVE](InstancedMesh.md#occlusion_algorithm_type_conservative)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:128

___

### OCCLUSION\_TYPE\_NONE

▪ `Static` **OCCLUSION\_TYPE\_NONE**: `number` = `0`

No occlusion

#### Inherited from

[InstancedMesh](InstancedMesh.md).[OCCLUSION_TYPE_NONE](InstancedMesh.md#occlusion_type_none)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:120

___

### OCCLUSION\_TYPE\_OPTIMISTIC

▪ `Static` **OCCLUSION\_TYPE\_OPTIMISTIC**: `number` = `1`

Occlusion set to optimistic

#### Inherited from

[InstancedMesh](InstancedMesh.md).[OCCLUSION_TYPE_OPTIMISTIC](InstancedMesh.md#occlusion_type_optimistic)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:122

___

### OCCLUSION\_TYPE\_STRICT

▪ `Static` **OCCLUSION\_TYPE\_STRICT**: `number` = `2`

Occlusion set to strict

#### Inherited from

[InstancedMesh](InstancedMesh.md).[OCCLUSION_TYPE_STRICT](InstancedMesh.md#occlusion_type_strict)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:124

## Accessors

### \_positions

• `get` **_positions**(): [`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md)[]

#### Returns

[`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md)[]

#### Inherited from

InstancedMesh.\_positions

#### Defined in

packages/dev/core/src/Meshes/instancedMesh.ts:299

___

### absolutePosition

• `get` **absolutePosition**(): [`Vector3`](Vector3.md)

Returns the current mesh absolute position.
Returns a Vector3.

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

InstancedMesh.absolutePosition

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:344

___

### absoluteRotationQuaternion

• `get` **absoluteRotationQuaternion**(): [`Quaternion`](Quaternion.md)

Returns the current mesh absolute rotation.
Returns a Quaternion.

#### Returns

[`Quaternion`](Quaternion.md)

#### Inherited from

InstancedMesh.absoluteRotationQuaternion

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:361

___

### absoluteScaling

• `get` **absoluteScaling**(): [`Vector3`](Vector3.md)

Returns the current mesh absolute scaling.
Returns a Vector3.

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

InstancedMesh.absoluteScaling

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:352

___

### animationPropertiesOverride

• `get` **animationPropertiesOverride**(): [`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md)

Gets or sets the animation properties override

#### Returns

[`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md)

#### Inherited from

InstancedMesh.animationPropertiesOverride

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

InstancedMesh.animationPropertiesOverride

#### Defined in

packages/dev/core/src/node.ts:282

___

### applyFog

• `get` **applyFog**(): `boolean`

Gets or sets a boolean indicating that this mesh will allow fog to be rendered on it (true by default)

#### Returns

`boolean`

#### Inherited from

InstancedMesh.applyFog

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:589

• `set` **applyFog**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

InstancedMesh.applyFog

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:592

___

### bakedVertexAnimationManager

• `get` **bakedVertexAnimationManager**(): [`Nullable`](../modules.md#nullable)[`IBakedVertexAnimationManager`](../interfaces/IBakedVertexAnimationManager.md)

Gets or sets the baked vertex animation manager

**`See`**

https://doc.babylonjs.com/divingDeeper/animation/baked_texture_animations

#### Returns

[`Nullable`](../modules.md#nullable)[`IBakedVertexAnimationManager`](../interfaces/IBakedVertexAnimationManager.md)

#### Inherited from

InstancedMesh.bakedVertexAnimationManager

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:306

• `set` **bakedVertexAnimationManager**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`IBakedVertexAnimationManager`](../interfaces/IBakedVertexAnimationManager.md) |

#### Returns

`void`

#### Inherited from

InstancedMesh.bakedVertexAnimationManager

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:310

___

### behaviors

• `get` **behaviors**(): [`Behavior`](../interfaces/Behavior.md)[`Node`](Node.md)[]

Gets the list of attached behaviors

**`See`**

https://doc.babylonjs.com/features/behaviour

#### Returns

[`Behavior`](../interfaces/Behavior.md)[`Node`](Node.md)[]

#### Inherited from

InstancedMesh.behaviors

#### Defined in

packages/dev/core/src/node.ts:410

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

InstancedMesh.billboardMode

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:82

• `set` **billboardMode**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

InstancedMesh.billboardMode

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:86

___

### checkCollisions

• `get` **checkCollisions**(): `boolean`

Gets or sets a boolean indicating that this mesh can be used in the collision engine

**`See`**

https://doc.babylonjs.com/babylon101/cameras,_mesh_collisions_and_gravity

#### Returns

`boolean`

#### Inherited from

InstancedMesh.checkCollisions

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1686

• `set` **checkCollisions**(`collisionEnabled`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `collisionEnabled` | `boolean` |

#### Returns

`void`

#### Inherited from

InstancedMesh.checkCollisions

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1690

___

### collider

• `get` **collider**(): [`Nullable`](../modules.md#nullable)`Collider`

Gets Collider object used to compute collisions (not physics)

**`See`**

https://doc.babylonjs.com/babylon101/cameras,_mesh_collisions_and_gravity

#### Returns

[`Nullable`](../modules.md#nullable)`Collider`

#### Inherited from

InstancedMesh.collider

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1698

___

### collisionGroup

• `get` **collisionGroup**(): `number`

Gets or sets the current collision group mask (-1 by default).
A collision between A and B will happen if A.collisionGroup & b.collisionMask !== 0

#### Returns

`number`

#### Inherited from

InstancedMesh.collisionGroup

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:688

• `set` **collisionGroup**(`mask`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `mask` | `number` |

#### Returns

`void`

#### Inherited from

InstancedMesh.collisionGroup

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:692

___

### collisionMask

• `get` **collisionMask**(): `number`

Gets or sets a collision mask used to mask collisions (default is -1).
A collision between A and B will happen if A.collisionGroup & b.collisionMask !== 0

#### Returns

`number`

#### Inherited from

InstancedMesh.collisionMask

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:663

• `set` **collisionMask**(`mask`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `mask` | `number` |

#### Returns

`void`

#### Inherited from

InstancedMesh.collisionMask

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:667

___

### collisionResponse

• `get` **collisionResponse**(): `boolean`

Gets or sets a collision response flag (default is true).
when collisionResponse is false, events are still triggered but colliding entity has no response
This helps creating trigger volume when user wants collision feedback events but not position/velocity
to respond to the collision.

#### Returns

`boolean`

#### Inherited from

InstancedMesh.collisionResponse

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:677

• `set` **collisionResponse**(`response`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `response` | `boolean` |

#### Returns

`void`

#### Inherited from

InstancedMesh.collisionResponse

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:681

___

### collisionRetryCount

• `get` **collisionRetryCount**(): `number`

number of collision detection tries. Change this value if not all collisions are detected and handled properly

#### Returns

`number`

#### Inherited from

InstancedMesh.collisionRetryCount

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:272

• `set` **collisionRetryCount**(`retryCount`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `retryCount` | `number` |

#### Returns

`void`

#### Inherited from

InstancedMesh.collisionRetryCount

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:275

___

### computeBonesUsingShaders

• `get` **computeBonesUsingShaders**(): `boolean`

Gets or sets a boolean indicating that bone animations must be computed by the CPU (false by default)

#### Returns

`boolean`

#### Inherited from

InstancedMesh.computeBonesUsingShaders

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:563

• `set` **computeBonesUsingShaders**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

InstancedMesh.computeBonesUsingShaders

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:566

___

### doNotSerialize

• `get` **doNotSerialize**(): `boolean`

Gets or sets a boolean used to define if the node must be serialized

#### Returns

`boolean`

#### Inherited from

InstancedMesh.doNotSerialize

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

InstancedMesh.doNotSerialize

#### Defined in

packages/dev/core/src/node.ts:143

___

### enableDistantPicking

• `get` **enableDistantPicking**(): `boolean`

When enabled, decompose picking matrices for better precision with large values for mesh position and scling

#### Returns

`boolean`

#### Inherited from

InstancedMesh.enableDistantPicking

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:602

• `set` **enableDistantPicking**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

InstancedMesh.enableDistantPicking

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:605

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

#### Inherited from

InstancedMesh.facetDepthSortFrom

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:264

• `set` **facetDepthSortFrom**(`location`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `location` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Inherited from

InstancedMesh.facetDepthSortFrom

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:267

___

### facetNb

• `get` **facetNb**(): `number`

Gets the number of facets in the mesh

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_facetdata#what-is-a-mesh-facet

#### Returns

`number`

#### Inherited from

InstancedMesh.facetNb

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:220

___

### forward

• `get` **forward**(): [`Vector3`](Vector3.md)

The forward direction of that transform in world space.

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

InstancedMesh.forward

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:253

___

### hasBoundingInfo

• `get` **hasBoundingInfo**(): `boolean`

Returns true if there is already a bounding info

#### Returns

`boolean`

#### Inherited from

InstancedMesh.hasBoundingInfo

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1230

___

### hasInstances

• `get` **hasInstances**(): `boolean`

Gets a boolean indicating if this mesh has instances

#### Returns

`boolean`

#### Inherited from

InstancedMesh.hasInstances

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1334

___

### hasThinInstances

• `get` **hasThinInstances**(): `boolean`

Gets a boolean indicating if this mesh has thin instances

#### Returns

`boolean`

#### Inherited from

InstancedMesh.hasThinInstances

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1341

___

### hasVertexAlpha

• `get` **hasVertexAlpha**(): `boolean`

Gets or sets a boolean indicating that this mesh contains vertex color data with alpha values

#### Returns

`boolean`

#### Inherited from

InstancedMesh.hasVertexAlpha

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:534

• `set` **hasVertexAlpha**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

InstancedMesh.hasVertexAlpha

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:537

___

### infiniteDistance

• `get` **infiniteDistance**(): `boolean`

Gets or sets the distance of the object to max, often used by skybox

#### Returns

`boolean`

#### Inherited from

InstancedMesh.infiniteDistance

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:121

• `set` **infiniteDistance**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

InstancedMesh.infiniteDistance

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:125

___

### isAnInstance

• `get` **isAnInstance**(): `boolean`

Gets a boolean indicating if this mesh is an instance or a regular mesh

#### Returns

`boolean`

#### Inherited from

InstancedMesh.isAnInstance

#### Defined in

packages/dev/core/src/Meshes/instancedMesh.ts:395

___

### isBlocked

• `get` **isBlocked**(): `boolean`

Returns true if the mesh is blocked. Implemented by child classes

#### Returns

`boolean`

#### Inherited from

InstancedMesh.isBlocked

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1073

___

### isFacetDataEnabled

• `get` **isFacetDataEnabled**(): `boolean`

gets a boolean indicating if facetData is enabled

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_facetdata#what-is-a-mesh-facet

#### Returns

`boolean`

#### Inherited from

InstancedMesh.isFacetDataEnabled

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:282

___

### isWorldMatrixFrozen

• `get` **isWorldMatrixFrozen**(): `boolean`

True if the World matrix has been frozen.

#### Returns

`boolean`

#### Inherited from

InstancedMesh.isWorldMatrixFrozen

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:476

___

### layerMask

• `get` **layerMask**(): `number`

Gets or sets the current layer mask (default is 0x0FFFFFFF)

**`See`**

https://doc.babylonjs.com/divingDeeper/cameras/layerMasksAndMultiCam

#### Returns

`number`

#### Inherited from

InstancedMesh.layerMask

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:619

• `set` **layerMask**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

InstancedMesh.layerMask

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:623

___

### lightSources

• `get` **lightSources**(): [`Light`](Light.md)[]

Gets the list of lights affecting that mesh

#### Returns

[`Light`](Light.md)[]

#### Inherited from

InstancedMesh.lightSources

#### Defined in

packages/dev/core/src/Meshes/instancedMesh.ts:85

___

### material

• `get` **material**(): [`Nullable`](../modules.md#nullable)[`Material`](Material.md)

The material of the source mesh

#### Returns

[`Nullable`](../modules.md#nullable)[`Material`](Material.md)

#### Inherited from

InstancedMesh.material

#### Defined in

packages/dev/core/src/Meshes/instancedMesh.ts:112

___

### morphTargetManager

• `get` **morphTargetManager**(): [`Nullable`](../modules.md#nullable)[`MorphTargetManager`](MorphTargetManager.md)

Gets or sets the morph target manager

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_morphtargets

#### Returns

[`Nullable`](../modules.md#nullable)[`MorphTargetManager`](MorphTargetManager.md)

#### Inherited from

InstancedMesh.morphTargetManager

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:290

• `set` **morphTargetManager**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`MorphTargetManager`](MorphTargetManager.md) |

#### Returns

`void`

#### Inherited from

InstancedMesh.morphTargetManager

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:294

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

#### Inherited from

InstancedMesh.mustDepthSortFacets

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:251

• `set` **mustDepthSortFacets**(`sort`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `sort` | `boolean` |

#### Returns

`void`

#### Inherited from

InstancedMesh.mustDepthSortFacets

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:254

___

### nonUniformScaling

• `get` **nonUniformScaling**(): `boolean`

True if the scaling property of this object is non uniform eg. (1,2,1)

#### Returns

`boolean`

#### Inherited from

InstancedMesh.nonUniformScaling

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:799

___

### numBoneInfluencers

• `get` **numBoneInfluencers**(): `number`

Gets or sets the number of allowed bone influences per vertex (4 by default)

#### Returns

`number`

#### Inherited from

InstancedMesh.numBoneInfluencers

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:576

• `set` **numBoneInfluencers**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

InstancedMesh.numBoneInfluencers

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:579

___

### onClonedObservable

• `get` **onClonedObservable**(): [`Observable`](Observable.md)[`Node`](Node.md)

An event triggered when the node is cloned

#### Returns

[`Observable`](Observable.md)[`Node`](Node.md)

#### Inherited from

InstancedMesh.onClonedObservable

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

#### Inherited from

InstancedMesh.onCollide

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

#### Inherited from

InstancedMesh.onCollisionPositionChange

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

InstancedMesh.onDispose

#### Defined in

packages/dev/core/src/node.ts:306

___

### onEnabledStateChangedObservable

• `get` **onEnabledStateChangedObservable**(): [`Observable`](Observable.md)`boolean`

An event triggered when the enabled state of the node changes

#### Returns

[`Observable`](Observable.md)`boolean`

#### Inherited from

InstancedMesh.onEnabledStateChangedObservable

#### Defined in

packages/dev/core/src/node.ts:316

___

### parent

• `get` **parent**(): [`Nullable`](../modules.md#nullable)[`Node`](Node.md)

#### Returns

[`Nullable`](../modules.md#nullable)[`Node`](Node.md)

#### Inherited from

InstancedMesh.parent

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

InstancedMesh.parent

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

#### Inherited from

InstancedMesh.partitioningBBoxRatio

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:238

• `set` **partitioningBBoxRatio**(`ratio`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `ratio` | `number` |

#### Returns

`void`

#### Inherited from

InstancedMesh.partitioningBBoxRatio

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

#### Inherited from

InstancedMesh.partitioningSubdivisions

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:227

• `set` **partitioningSubdivisions**(`nb`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `nb` | `number` |

#### Returns

`void`

#### Inherited from

InstancedMesh.partitioningSubdivisions

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:230

___

### position

• `get` **position**(): [`Vector3`](Vector3.md)

Gets or set the node position (default is (0.0, 0.0, 0.0))

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

InstancedMesh.position

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

InstancedMesh.position

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

InstancedMesh.preserveParentRotationForBillboard

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

InstancedMesh.preserveParentRotationForBillboard

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:102

___

### receiveShadows

• `get` **receiveShadows**(): `boolean`

If the source mesh receives shadows

#### Returns

`boolean`

#### Inherited from

InstancedMesh.receiveShadows

#### Defined in

packages/dev/core/src/Meshes/instancedMesh.ts:105

___

### renderingGroupId

• `get` **renderingGroupId**(): `number`

Rendering ground id of the source mesh

#### Returns

`number`

#### Inherited from

InstancedMesh.renderingGroupId

#### Defined in

packages/dev/core/src/Meshes/instancedMesh.ts:133

• `set` **renderingGroupId**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

InstancedMesh.renderingGroupId

#### Defined in

packages/dev/core/src/Meshes/instancedMesh.ts:137

___

### right

• `get` **right**(): [`Vector3`](Vector3.md)

The right direction of that transform in world space.

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

InstancedMesh.right

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

InstancedMesh.rotation

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

InstancedMesh.rotation

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

InstancedMesh.rotationQuaternion

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

InstancedMesh.rotationQuaternion

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:241

___

### scaling

• `get` **scaling**(): [`Vector3`](Vector3.md)

Gets or sets the scaling property : a Vector3 defining the node scaling along each local axis X, Y, Z (default is (1.0, 1.0, 1.0)).

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

InstancedMesh.scaling

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

InstancedMesh.scaling

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:228

___

### skeleton

• `get` **skeleton**(): [`Nullable`](../modules.md#nullable)[`Skeleton`](Skeleton.md)

Skeleton of the source mesh

#### Returns

[`Nullable`](../modules.md#nullable)[`Skeleton`](Skeleton.md)

#### Inherited from

InstancedMesh.skeleton

#### Defined in

packages/dev/core/src/Meshes/instancedMesh.ts:126

___

### sourceMesh

• `get` **sourceMesh**(): [`Mesh`](Mesh.md)

The source mesh of the instance

#### Returns

[`Mesh`](Mesh.md)

#### Inherited from

InstancedMesh.sourceMesh

#### Defined in

packages/dev/core/src/Meshes/instancedMesh.ts:164

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

#### Inherited from

InstancedMesh.surroundingMeshes

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:705

• `set` **surroundingMeshes**(`meshes`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `meshes` | [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)[] |

#### Returns

`void`

#### Inherited from

InstancedMesh.surroundingMeshes

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:709

___

### up

• `get` **up**(): [`Vector3`](Vector3.md)

The up direction of that transform in world space.

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

InstancedMesh.up

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:261

___

### useBones

• `get` **useBones**(): `boolean`

Gets a boolean indicating if this mesh has skinning data and an attached skeleton

#### Returns

`boolean`

#### Inherited from

InstancedMesh.useBones

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1258

___

### useVertexColors

• `get` **useVertexColors**(): `boolean`

Gets or sets a boolean indicating that this mesh needs to use vertex color data to render (if this kind of vertex data is available in the geometry)

#### Returns

`boolean`

#### Inherited from

InstancedMesh.useVertexColors

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:548

• `set` **useVertexColors**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

InstancedMesh.useVertexColors

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:551

___

### visibility

• `get` **visibility**(): `number`

Visibility of the source mesh

#### Returns

`number`

#### Inherited from

InstancedMesh.visibility

#### Defined in

packages/dev/core/src/Meshes/instancedMesh.ts:119

___

### worldMatrixFromCache

• `get` **worldMatrixFromCache**(): [`Matrix`](Matrix.md)

Returns directly the latest state of the mesh World matrix.
A Matrix is returned.

#### Returns

[`Matrix`](Matrix.md)

#### Inherited from

InstancedMesh.worldMatrixFromCache

#### Defined in

packages/dev/core/src/node.ts:454

___

### BILLBOARDMODE\_ALL

• `Static` `get` **BILLBOARDMODE_ALL**(): `number`

Billboard on all axes

#### Returns

`number`

#### Inherited from

InstancedMesh.BILLBOARDMODE\_ALL

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:188

___

### BILLBOARDMODE\_NONE

• `Static` `get` **BILLBOARDMODE_NONE**(): `number`

No billboard

#### Returns

`number`

#### Inherited from

InstancedMesh.BILLBOARDMODE\_NONE

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:168

___

### BILLBOARDMODE\_USE\_POSITION

• `Static` `get` **BILLBOARDMODE_USE_POSITION**(): `number`

Billboard on using position instead of orientation

#### Returns

`number`

#### Inherited from

InstancedMesh.BILLBOARDMODE\_USE\_POSITION

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:193

___

### BILLBOARDMODE\_X

• `Static` `get` **BILLBOARDMODE_X**(): `number`

Billboard on X axis

#### Returns

`number`

#### Inherited from

InstancedMesh.BILLBOARDMODE\_X

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:173

___

### BILLBOARDMODE\_Y

• `Static` `get` **BILLBOARDMODE_Y**(): `number`

Billboard on Y axis

#### Returns

`number`

#### Inherited from

InstancedMesh.BILLBOARDMODE\_Y

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:178

___

### BILLBOARDMODE\_Z

• `Static` `get` **BILLBOARDMODE_Z**(): `number`

Billboard on Z axis

#### Returns

`number`

#### Inherited from

InstancedMesh.BILLBOARDMODE\_Z

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:183

## Methods

### \_buildUniformLayout

▸ `Protected` **_buildUniformLayout**(): `void`

#### Returns

`void`

#### Inherited from

[InstancedMesh](InstancedMesh.md).[_buildUniformLayout](InstancedMesh.md#_builduniformlayout)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:834

___

### \_removeLightSource

▸ **_removeLightSource**(): `void`

#### Returns

`void`

#### Inherited from

[InstancedMesh](InstancedMesh.md).[_removeLightSource](InstancedMesh.md#_removelightsource)

#### Defined in

packages/dev/core/src/Meshes/instancedMesh.ts:97

___

### \_resyncLightSource

▸ **_resyncLightSource**(): `void`

#### Returns

`void`

#### Inherited from

[InstancedMesh](InstancedMesh.md).[_resyncLightSource](InstancedMesh.md#_resynclightsource)

#### Defined in

packages/dev/core/src/Meshes/instancedMesh.ts:93

___

### \_resyncLightSources

▸ **_resyncLightSources**(): `void`

#### Returns

`void`

#### Inherited from

[InstancedMesh](InstancedMesh.md).[_resyncLightSources](InstancedMesh.md#_resynclightsources)

#### Defined in

packages/dev/core/src/Meshes/instancedMesh.ts:89

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

[InstancedMesh](InstancedMesh.md).[addBehavior](InstancedMesh.md#addbehavior)

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[addChild](InstancedMesh.md#addchild)

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

[InstancedMesh](InstancedMesh.md).[addRotation](InstancedMesh.md#addrotation)

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[alignWithNormal](InstancedMesh.md#alignwithnormal)

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[applyImpulse](InstancedMesh.md#applyimpulse)

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

[InstancedMesh](InstancedMesh.md).[attachToBone](InstancedMesh.md#attachtobone)

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

[InstancedMesh](InstancedMesh.md).[beginAnimation](InstancedMesh.md#beginanimation)

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[buildBoundingInfo](InstancedMesh.md#buildboundinginfo)

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[calcMovePOV](InstancedMesh.md#calcmovepov)

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[calcRotatePOV](InstancedMesh.md#calcrotatepov)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1402

___

### clone

▸ **clone**(`name`, `newParent?`, `doNotCloneChildren?`): [`InstancedMesh`](InstancedMesh.md)

Creates a new InstancedMesh from the current mesh.
- name (string) : the cloned mesh name
- newParent (optional Node) : the optional Node to parent the clone to.
- doNotCloneChildren (optional boolean, default `false`) : if `true` the model children aren't cloned.

Returns the clone.

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `name` | `string` | `undefined` |
| `newParent` | [`Nullable`](../modules.md#nullable)[`Node`](Node.md) | `null` |
| `doNotCloneChildren?` | `boolean` | `undefined` |

#### Returns

[`InstancedMesh`](InstancedMesh.md)

#### Inherited from

[InstancedMesh](InstancedMesh.md).[clone](InstancedMesh.md#clone)

#### Defined in

packages/dev/core/src/Meshes/instancedMesh.ts:465

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

[InstancedMesh](InstancedMesh.md).[computeWorldMatrix](InstancedMesh.md#computeworldmatrix)

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

[InstancedMesh](InstancedMesh.md).[createAnimationRange](InstancedMesh.md#createanimationrange)

#### Defined in

packages/dev/core/src/node.ts:777

___

### createInstance

▸ **createInstance**(`name`): [`InstancedMesh`](InstancedMesh.md)

Creates a new InstancedMesh object from the mesh model.

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_instances

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the name of the new instance |

#### Returns

[`InstancedMesh`](InstancedMesh.md)

a new InstancedMesh

#### Inherited from

[InstancedMesh](InstancedMesh.md).[createInstance](InstancedMesh.md#createinstance)

#### Defined in

packages/dev/core/src/Meshes/instancedMesh.ts:174

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[createNormals](InstancedMesh.md#createnormals)

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[createOrUpdateSubmeshesOctree](InstancedMesh.md#createorupdatesubmeshesoctree)

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

[InstancedMesh](InstancedMesh.md).[deleteAnimationRange](InstancedMesh.md#deleteanimationrange)

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

[InstancedMesh](InstancedMesh.md).[detachFromBone](InstancedMesh.md#detachfrombone)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:840

___

### disableEdgesRendering

▸ **disableEdgesRendering**(): [`AbstractMesh`](AbstractMesh.md)

Disables the mesh edge rendering mode

#### Returns

[`AbstractMesh`](AbstractMesh.md)

the currentAbstractMesh

#### Inherited from

[InstancedMesh](InstancedMesh.md).[disableEdgesRendering](InstancedMesh.md#disableedgesrendering)

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[disableFacetData](InstancedMesh.md#disablefacetdata)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:2505

___

### dispose

▸ **dispose**(`doNotRecurse?`, `disposeMaterialAndTextures?`): `void`

Disposes the InstancedMesh.
Returns nothing.

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `doNotRecurse?` | `boolean` | `undefined` |
| `disposeMaterialAndTextures` | `boolean` | `false` |

#### Returns

`void`

#### Inherited from

[InstancedMesh](InstancedMesh.md).[dispose](InstancedMesh.md#dispose)

#### Defined in

packages/dev/core/src/Meshes/instancedMesh.ts:539

___

### enableEdgesRendering

▸ **enableEdgesRendering**(`epsilon?`, `checkVerticesInsteadOfIndices?`): [`InstancedLinesMesh`](InstancedLinesMesh.md)

Enables the edge rendering mode on the mesh.
This mode makes the mesh edges visible

**`See`**

https://www.babylonjs-playground.com/#19O9TU#0

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `epsilon?` | `number` | defines the maximal distance between two angles to detect a face |
| `checkVerticesInsteadOfIndices?` | `boolean` | indicates that we should check vertex list directly instead of faces |

#### Returns

[`InstancedLinesMesh`](InstancedLinesMesh.md)

the current InstancedLinesMesh

#### Inherited from

[InstancedMesh](InstancedMesh.md).[enableEdgesRendering](InstancedMesh.md#enableedgesrendering)

#### Defined in

packages/dev/core/src/Rendering/edgesRenderer.ts:89

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

[InstancedMesh](InstancedMesh.md).[freezeWorldMatrix](InstancedMesh.md#freezeworldmatrix)

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

[InstancedMesh](InstancedMesh.md).[getAbsolutePivotPoint](InstancedMesh.md#getabsolutepivotpoint)

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

[InstancedMesh](InstancedMesh.md).[getAbsolutePivotPointToRef](InstancedMesh.md#getabsolutepivotpointtoref)

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

[InstancedMesh](InstancedMesh.md).[getAbsolutePosition](InstancedMesh.md#getabsoluteposition)

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

[InstancedMesh](InstancedMesh.md).[getAnimationByName](InstancedMesh.md#getanimationbyname)

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

[InstancedMesh](InstancedMesh.md).[getAnimationRange](InstancedMesh.md#getanimationrange)

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

[InstancedMesh](InstancedMesh.md).[getAnimationRanges](InstancedMesh.md#getanimationranges)

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

[InstancedMesh](InstancedMesh.md).[getBehaviorByName](InstancedMesh.md#getbehaviorbyname)

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[getBoundingInfo](InstancedMesh.md#getboundinginfo)

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

[InstancedMesh](InstancedMesh.md).[getChildMeshes](InstancedMesh.md#getchildmeshes)

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

[InstancedMesh](InstancedMesh.md).[getChildMeshes](InstancedMesh.md#getchildmeshes)

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

[InstancedMesh](InstancedMesh.md).[getChildTransformNodes](InstancedMesh.md#getchildtransformnodes)

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

[InstancedMesh](InstancedMesh.md).[getChildren](InstancedMesh.md#getchildren)

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

[InstancedMesh](InstancedMesh.md).[getChildren](InstancedMesh.md#getchildren)

#### Defined in

packages/dev/core/src/node.ts:722

___

### getClassName

▸ **getClassName**(): `string`

Returns the string "InstancedLinesMesh".

#### Returns

`string`

#### Overrides

[InstancedMesh](InstancedMesh.md).[getClassName](InstancedMesh.md#getclassname)

#### Defined in

packages/dev/core/src/Meshes/linesMesh.ts:294

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[getClosestFacetAtCoordinates](InstancedMesh.md#getclosestfacetatcoordinates)

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[getClosestFacetAtLocalCoordinates](InstancedMesh.md#getclosestfacetatlocalcoordinates)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:2434

___

### getConnectedParticleSystems

▸ **getConnectedParticleSystems**(): [`IParticleSystem`](../interfaces/IParticleSystem.md)[]

This function returns all of the particle systems in the scene that use the mesh as an emitter.

#### Returns

[`IParticleSystem`](../interfaces/IParticleSystem.md)[]

an array of particle systems in the scene that use the mesh as an emitter

#### Inherited from

[InstancedMesh](InstancedMesh.md).[getConnectedParticleSystems](InstancedMesh.md#getconnectedparticlesystems)

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

[InstancedMesh](InstancedMesh.md).[getDescendants](InstancedMesh.md#getdescendants)

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

[InstancedMesh](InstancedMesh.md).[getDescendants](InstancedMesh.md#getdescendants)

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

[InstancedMesh](InstancedMesh.md).[getDirection](InstancedMesh.md#getdirection)

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

[InstancedMesh](InstancedMesh.md).[getDirectionToRef](InstancedMesh.md#getdirectiontoref)

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

[InstancedMesh](InstancedMesh.md).[getDistanceToCamera](InstancedMesh.md#getdistancetocamera)

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

[InstancedMesh](InstancedMesh.md).[getEngine](InstancedMesh.md#getengine)

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[getFacetDataParameters](InstancedMesh.md#getfacetdataparameters)

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[getFacetLocalNormals](InstancedMesh.md#getfacetlocalnormals)

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[getFacetLocalPartitioning](InstancedMesh.md#getfacetlocalpartitioning)

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[getFacetLocalPositions](InstancedMesh.md#getfacetlocalpositions)

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[getFacetNormal](InstancedMesh.md#getfacetnormal)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:2358

___

### getFacetNormalToRef

▸ **getFacetNormalToRef**(`i`, `ref`): [`InstancedLinesMesh`](InstancedLinesMesh.md)

Sets the reference Vector3 with the i-th facet normal in the world system

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_facetdata

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `i` | `number` | defines the facet index |
| `ref` | [`Vector3`](Vector3.md) | defines the target vector |

#### Returns

[`InstancedLinesMesh`](InstancedLinesMesh.md)

the current mesh

#### Inherited from

[InstancedMesh](InstancedMesh.md).[getFacetNormalToRef](InstancedMesh.md#getfacetnormaltoref)

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[getFacetPosition](InstancedMesh.md#getfacetposition)

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[getFacetPositionToRef](InstancedMesh.md#getfacetpositiontoref)

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[getFacetsAtLocalCoordinates](InstancedMesh.md#getfacetsatlocalcoordinates)

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

[InstancedMesh](InstancedMesh.md).[getHierarchyBoundingVectors](InstancedMesh.md#gethierarchyboundingvectors)

#### Defined in

packages/dev/core/src/node.ts:933

___

### getIndices

▸ **getIndices**(): [`Nullable`](../modules.md#nullable)[`IndicesArray`](../modules.md#indicesarray)

Returns an array of indices (IndicesArray).

#### Returns

[`Nullable`](../modules.md#nullable)[`IndicesArray`](../modules.md#indicesarray)

#### Inherited from

[InstancedMesh](InstancedMesh.md).[getIndices](InstancedMesh.md#getindices)

#### Defined in

packages/dev/core/src/Meshes/instancedMesh.ts:295

___

### getLOD

▸ **getLOD**(`camera`): [`AbstractMesh`](AbstractMesh.md)

Returns the current associated LOD AbstractMesh.

#### Parameters

| Name | Type |
| :------ | :------ |
| `camera` | [`Camera`](Camera.md) |

#### Returns

[`AbstractMesh`](AbstractMesh.md)

#### Inherited from

[InstancedMesh](InstancedMesh.md).[getLOD](InstancedMesh.md#getlod)

#### Defined in

packages/dev/core/src/Meshes/instancedMesh.ts:403

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[getMaterialForRenderPass](InstancedMesh.md#getmaterialforrenderpass)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:490

___

### getMeshUniformBuffer

▸ **getMeshUniformBuffer**(): [`UniformBuffer`](UniformBuffer.md)

Gets the mesh uniform buffer.

#### Returns

[`UniformBuffer`](UniformBuffer.md)

the uniform buffer of the mesh.

#### Inherited from

[InstancedMesh](InstancedMesh.md).[getMeshUniformBuffer](InstancedMesh.md#getmeshuniformbuffer)

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[getNormalsData](InstancedMesh.md#getnormalsdata)

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[getPhysicsImpostor](InstancedMesh.md#getphysicsimpostor)

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

[InstancedMesh](InstancedMesh.md).[getPivotMatrix](InstancedMesh.md#getpivotmatrix)

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

[InstancedMesh](InstancedMesh.md).[getPivotPoint](InstancedMesh.md#getpivotpoint)

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

[InstancedMesh](InstancedMesh.md).[getPivotPointToRef](InstancedMesh.md#getpivotpointtoref)

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

[InstancedMesh](InstancedMesh.md).[getPoseMatrix](InstancedMesh.md#getposematrix)

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[getPositionData](InstancedMesh.md#getpositiondata)

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

[InstancedMesh](InstancedMesh.md).[getPositionExpressedInLocalSpace](InstancedMesh.md#getpositionexpressedinlocalspace)

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

[InstancedMesh](InstancedMesh.md).[getPositionInCameraSpace](InstancedMesh.md#getpositionincameraspace)

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

[InstancedMesh](InstancedMesh.md).[getScene](InstancedMesh.md#getscene)

#### Defined in

packages/dev/core/src/node.ts:344

___

### getTotalIndices

▸ **getTotalIndices**(): `number`

Returns a positive integer : the total number of indices in this mesh geometry.

#### Returns

`number`

the number of indices or zero if the mesh has no geometry.

#### Inherited from

[InstancedMesh](InstancedMesh.md).[getTotalIndices](InstancedMesh.md#gettotalindices)

#### Defined in

packages/dev/core/src/Meshes/instancedMesh.ts:157

___

### getTotalVertices

▸ **getTotalVertices**(): `number`

Returns the total number of vertices (integer).

#### Returns

`number`

#### Inherited from

[InstancedMesh](InstancedMesh.md).[getTotalVertices](InstancedMesh.md#gettotalvertices)

#### Defined in

packages/dev/core/src/Meshes/instancedMesh.ts:149

___

### getVerticesData

▸ **getVerticesData**(`kind`, `copyWhenShared?`): [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray)

Returns an array of integers or a typed array (Int32Array, Uint32Array, Uint16Array) populated with the mesh indices.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `kind` | `string` | kind of verticies to retrieve (eg. positions, normals, uvs, etc.) |
| `copyWhenShared?` | `boolean` | If true (default false) and and if the mesh geometry is shared among some other meshes, the returned array is a copy of the internal one. |

#### Returns

[`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray)

a float array or a Float32Array of the requested kind of data : positions, normals, uvs, etc.

#### Inherited from

[InstancedMesh](InstancedMesh.md).[getVerticesData](InstancedMesh.md#getverticesdata)

#### Defined in

packages/dev/core/src/Meshes/instancedMesh.ts:193

___

### getWorldMatrix

▸ **getWorldMatrix**(): [`Matrix`](Matrix.md)

Gets the current world matrix

#### Returns

[`Matrix`](Matrix.md)

a Matrix

#### Inherited from

[InstancedMesh](InstancedMesh.md).[getWorldMatrix](InstancedMesh.md#getworldmatrix)

#### Defined in

packages/dev/core/src/Meshes/instancedMesh.ts:377

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

[InstancedMesh](InstancedMesh.md).[instantiateHierarchy](InstancedMesh.md#instantiatehierarchy)

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[intersects](InstancedMesh.md#intersects)

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[intersectsMesh](InstancedMesh.md#intersectsmesh)

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[intersectsPoint](InstancedMesh.md#intersectspoint)

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[isCompletelyInFrustum](InstancedMesh.md#iscompletelyinfrustum)

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

[InstancedMesh](InstancedMesh.md).[isDescendantOf](InstancedMesh.md#isdescendantof)

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

[InstancedMesh](InstancedMesh.md).[isDisposed](InstancedMesh.md#isdisposed)

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

[InstancedMesh](InstancedMesh.md).[isEnabled](InstancedMesh.md#isenabled)

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[isInFrustum](InstancedMesh.md#isinfrustum)

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

is it ready

#### Inherited from

[InstancedMesh](InstancedMesh.md).[isReady](InstancedMesh.md#isready)

#### Defined in

packages/dev/core/src/Meshes/instancedMesh.ts:183

___

### isUsingPivotMatrix

▸ **isUsingPivotMatrix**(): `boolean`

return true if a pivot has been set

#### Returns

`boolean`

true if a pivot matrix is used

#### Inherited from

[InstancedMesh](InstancedMesh.md).[isUsingPivotMatrix](InstancedMesh.md#isusingpivotmatrix)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:203

___

### isVerticesDataPresent

▸ **isVerticesDataPresent**(`kind`): `boolean`

Boolean : True if the mesh owns the requested kind of data.

#### Parameters

| Name | Type |
| :------ | :------ |
| `kind` | `string` |

#### Returns

`boolean`

#### Inherited from

[InstancedMesh](InstancedMesh.md).[isVerticesDataPresent](InstancedMesh.md#isverticesdatapresent)

#### Defined in

packages/dev/core/src/Meshes/instancedMesh.ts:288

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

[InstancedMesh](InstancedMesh.md).[locallyTranslate](InstancedMesh.md#locallytranslate)

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

[InstancedMesh](InstancedMesh.md).[lookAt](InstancedMesh.md#lookat)

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[markAsDirty](InstancedMesh.md#markasdirty)

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[movePOV](InstancedMesh.md#movepov)

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[moveWithCollisions](InstancedMesh.md#movewithcollisions)

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[normalizeToUnitCube](InstancedMesh.md#normalizetounitcube)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1253

___

### refreshBoundingInfo

▸ **refreshBoundingInfo**(`applySkeleton?`, `applyMorph?`): [`InstancedMesh`](InstancedMesh.md)

This method recomputes and sets a new BoundingInfo to the mesh unless it is locked.
This means the mesh underlying bounding box and sphere are recomputed.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `applySkeleton` | `boolean` | `false` | defines whether to apply the skeleton before computing the bounding info |
| `applyMorph` | `boolean` | `false` | defines whether to apply the morph target before computing the bounding info |

#### Returns

[`InstancedMesh`](InstancedMesh.md)

the current mesh

#### Inherited from

[InstancedMesh](InstancedMesh.md).[refreshBoundingInfo](InstancedMesh.md#refreshboundinginfo)

#### Defined in

packages/dev/core/src/Meshes/instancedMesh.ts:310

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

[InstancedMesh](InstancedMesh.md).[registerAfterWorldMatrixUpdate](InstancedMesh.md#registerafterworldmatrixupdate)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:1283

___

### releaseSubMeshes

▸ **releaseSubMeshes**(): [`AbstractMesh`](AbstractMesh.md)

Disposes all the submeshes of the current meshnp

#### Returns

[`AbstractMesh`](AbstractMesh.md)

the current mesh

#### Inherited from

[InstancedMesh](InstancedMesh.md).[releaseSubMeshes](InstancedMesh.md#releasesubmeshes)

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

[InstancedMesh](InstancedMesh.md).[removeBehavior](InstancedMesh.md#removebehavior)

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[removeChild](InstancedMesh.md#removechild)

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[resetDrawCache](InstancedMesh.md#resetdrawcache)

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

[InstancedMesh](InstancedMesh.md).[resetLocalMatrix](InstancedMesh.md#resetlocalmatrix)

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

[InstancedMesh](InstancedMesh.md).[rotate](InstancedMesh.md#rotate)

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

[InstancedMesh](InstancedMesh.md).[rotateAround](InstancedMesh.md#rotatearound)

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[rotatePOV](InstancedMesh.md#rotatepov)

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

[InstancedMesh](InstancedMesh.md).[serialize](InstancedMesh.md#serialize)

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

[InstancedMesh](InstancedMesh.md).[serializeAnimationRanges](InstancedMesh.md#serializeanimationranges)

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

[InstancedMesh](InstancedMesh.md).[setAbsolutePosition](InstancedMesh.md#setabsoluteposition)

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[setBoundingInfo](InstancedMesh.md#setboundinginfo)

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

[InstancedMesh](InstancedMesh.md).[setDirection](InstancedMesh.md#setdirection)

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

[InstancedMesh](InstancedMesh.md).[setEnabled](InstancedMesh.md#setenabled)

#### Defined in

packages/dev/core/src/node.ts:596

___

### setIndices

▸ **setIndices**(`indices`, `totalVertices?`): [`Mesh`](Mesh.md)

Sets the mesh indices.
Expects an array populated with integers or a typed array (Int32Array, Uint32Array, Uint16Array).
If the mesh has no geometry, a new Geometry object is created and set to the mesh.
This method creates a new index buffer each call.
Returns the Mesh.

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `indices` | [`IndicesArray`](../modules.md#indicesarray) | `undefined` |
| `totalVertices` | [`Nullable`](../modules.md#nullable)`number` | `null` |

#### Returns

[`Mesh`](Mesh.md)

#### Inherited from

[InstancedMesh](InstancedMesh.md).[setIndices](InstancedMesh.md#setindices)

#### Defined in

packages/dev/core/src/Meshes/instancedMesh.ts:277

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[setMaterialForRenderPass](InstancedMesh.md#setmaterialforrenderpass)

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

[InstancedMesh](InstancedMesh.md).[setParent](InstancedMesh.md#setparent)

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[setPhysicsLinkWith](InstancedMesh.md#setphysicslinkwith)

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

[InstancedMesh](InstancedMesh.md).[setPivotMatrix](InstancedMesh.md#setpivotmatrix)

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

[InstancedMesh](InstancedMesh.md).[setPivotPoint](InstancedMesh.md#setpivotpoint)

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

[InstancedMesh](InstancedMesh.md).[setPositionWithLocalVector](InstancedMesh.md#setpositionwithlocalvector)

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

[InstancedMesh](InstancedMesh.md).[setPreTransformMatrix](InstancedMesh.md#setpretransformmatrix)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:371

___

### setVerticesData

▸ **setVerticesData**(`kind`, `data`, `updatable?`, `stride?`): [`AbstractMesh`](AbstractMesh.md)

Sets the vertex data of the mesh geometry for the requested `kind`.
If the mesh has no geometry, a new Geometry object is set to the mesh and then passed this vertex data.
The `data` are either a numeric array either a Float32Array.
The parameter `updatable` is passed as is to the underlying Geometry object constructor (if initially none) or updater.
The parameter `stride` is an optional positive integer, it is usually automatically deducted from the `kind` (3 for positions or normals, 2 for UV, etc).
Note that a new underlying VertexBuffer object is created each call.
If the `kind` is the `PositionKind`, the mesh BoundingInfo is renewed, so the bounding box and sphere, and the mesh World Matrix is recomputed.

Possible `kind` values :
- VertexBuffer.PositionKind
- VertexBuffer.UVKind
- VertexBuffer.UV2Kind
- VertexBuffer.UV3Kind
- VertexBuffer.UV4Kind
- VertexBuffer.UV5Kind
- VertexBuffer.UV6Kind
- VertexBuffer.ColorKind
- VertexBuffer.MatricesIndicesKind
- VertexBuffer.MatricesIndicesExtraKind
- VertexBuffer.MatricesWeightsKind
- VertexBuffer.MatricesWeightsExtraKind

Returns the Mesh.

#### Parameters

| Name | Type |
| :------ | :------ |
| `kind` | `string` |
| `data` | [`FloatArray`](../modules.md#floatarray) |
| `updatable?` | `boolean` |
| `stride?` | `number` |

#### Returns

[`AbstractMesh`](AbstractMesh.md)

#### Inherited from

[InstancedMesh](InstancedMesh.md).[setVerticesData](InstancedMesh.md#setverticesdata)

#### Defined in

packages/dev/core/src/Meshes/instancedMesh.ts:226

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[toString](InstancedMesh.md#tostring)

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[transferToEffect](InstancedMesh.md#transfertoeffect)

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

[InstancedMesh](InstancedMesh.md).[translate](InstancedMesh.md#translate)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:945

___

### unfreezeWorldMatrix

▸ **unfreezeWorldMatrix**(): [`InstancedLinesMesh`](InstancedLinesMesh.md)

Allows back the World matrix computation.

#### Returns

[`InstancedLinesMesh`](InstancedLinesMesh.md)

the TransformNode.

#### Inherited from

[InstancedMesh](InstancedMesh.md).[unfreezeWorldMatrix](InstancedMesh.md#unfreezeworldmatrix)

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

[InstancedMesh](InstancedMesh.md).[unregisterAfterWorldMatrixUpdate](InstancedMesh.md#unregisterafterworldmatrixupdate)

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[updateFacetData](InstancedMesh.md#updatefacetdata)

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

#### Inherited from

[InstancedMesh](InstancedMesh.md).[updateIndices](InstancedMesh.md#updateindices)

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

[InstancedMesh](InstancedMesh.md).[updatePoseMatrix](InstancedMesh.md#updateposematrix)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:279

___

### updateVerticesData

▸ **updateVerticesData**(`kind`, `data`, `updateExtends?`, `makeItUnique?`): [`Mesh`](Mesh.md)

Updates the existing vertex data of the mesh geometry for the requested `kind`.
If the mesh has no geometry, it is simply returned as it is.
The `data` are either a numeric array either a Float32Array.
No new underlying VertexBuffer object is created.
If the `kind` is the `PositionKind` and if `updateExtends` is true, the mesh BoundingInfo is renewed, so the bounding box and sphere, and the mesh World Matrix is recomputed.
If the parameter `makeItUnique` is true, a new global geometry is created from this positions and is set to the mesh.

Possible `kind` values :
- VertexBuffer.PositionKind
- VertexBuffer.UVKind
- VertexBuffer.UV2Kind
- VertexBuffer.UV3Kind
- VertexBuffer.UV4Kind
- VertexBuffer.UV5Kind
- VertexBuffer.UV6Kind
- VertexBuffer.ColorKind
- VertexBuffer.MatricesIndicesKind
- VertexBuffer.MatricesIndicesExtraKind
- VertexBuffer.MatricesWeightsKind
- VertexBuffer.MatricesWeightsExtraKind

Returns the Mesh.

#### Parameters

| Name | Type |
| :------ | :------ |
| `kind` | `string` |
| `data` | [`FloatArray`](../modules.md#floatarray) |
| `updateExtends?` | `boolean` |
| `makeItUnique?` | `boolean` |

#### Returns

[`Mesh`](Mesh.md)

#### Inherited from

[InstancedMesh](InstancedMesh.md).[updateVerticesData](InstancedMesh.md#updateverticesdata)

#### Defined in

packages/dev/core/src/Meshes/instancedMesh.ts:261

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

[InstancedMesh](InstancedMesh.md).[AddNodeConstructor](InstancedMesh.md#addnodeconstructor)

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

[InstancedMesh](InstancedMesh.md).[Construct](InstancedMesh.md#construct)

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

[InstancedMesh](InstancedMesh.md).[Parse](InstancedMesh.md#parse)

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

[InstancedMesh](InstancedMesh.md).[ParseAnimationRanges](InstancedMesh.md#parseanimationranges)

#### Defined in

packages/dev/core/src/node.ts:919
