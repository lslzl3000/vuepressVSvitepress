[@dev/core](../README.md) / [Exports](../modules.md) / InstancedMesh

# Class: InstancedMesh

Creates an instance based on a source mesh.

## Hierarchy

- [`AbstractMesh`](AbstractMesh.md)

  ↳ **`InstancedMesh`**

  ↳↳ [`InstancedLinesMesh`](InstancedLinesMesh.md)

## Table of contents

### Constructors

- [constructor](InstancedMesh.md#constructor)

### Properties

- [\_billboardWorldMatrix](InstancedMesh.md#_billboardworldmatrix)
- [\_boundingInfo](InstancedMesh.md#_boundinginfo)
- [\_boundingInfoIsDirty](InstancedMesh.md#_boundinginfoisdirty)
- [\_currentLOD](InstancedMesh.md#_currentlod)
- [\_isDirty](InstancedMesh.md#_isdirty)
- [\_isWorldMatrixFrozen](InstancedMesh.md#_isworldmatrixfrozen)
- [\_parentNode](InstancedMesh.md#_parentnode)
- [\_ranges](InstancedMesh.md#_ranges)
- [\_scaling](InstancedMesh.md#_scaling)
- [\_sourceMesh](InstancedMesh.md#_sourcemesh)
- [actionManager](InstancedMesh.md#actionmanager)
- [alphaIndex](InstancedMesh.md#alphaindex)
- [alwaysSelectAsActiveMesh](InstancedMesh.md#alwaysselectasactivemesh)
- [animations](InstancedMesh.md#animations)
- [cullingStrategy](InstancedMesh.md#cullingstrategy)
- [definedFacingForward](InstancedMesh.md#definedfacingforward)
- [doNotSyncBoundingInfo](InstancedMesh.md#donotsyncboundinginfo)
- [edgesColor](InstancedMesh.md#edgescolor)
- [edgesRenderer](InstancedMesh.md#edgesrenderer)
- [edgesWidth](InstancedMesh.md#edgeswidth)
- [ellipsoid](InstancedMesh.md#ellipsoid)
- [ellipsoidOffset](InstancedMesh.md#ellipsoidoffset)
- [enablePointerMoveEvents](InstancedMesh.md#enablepointermoveevents)
- [forceRenderingWhenOccluded](InstancedMesh.md#forcerenderingwhenoccluded)
- [id](InstancedMesh.md#id)
- [ignoreNonUniformScaling](InstancedMesh.md#ignorenonuniformscaling)
- [inspectableCustomProperties](InstancedMesh.md#inspectablecustomproperties)
- [instancedBuffers](InstancedMesh.md#instancedbuffers)
- [isBlocker](InstancedMesh.md#isblocker)
- [isNearGrabbable](InstancedMesh.md#isneargrabbable)
- [isNearPickable](InstancedMesh.md#isnearpickable)
- [isOccluded](InstancedMesh.md#isoccluded)
- [isOcclusionQueryInProgress](InstancedMesh.md#isocclusionqueryinprogress)
- [isPickable](InstancedMesh.md#ispickable)
- [isVisible](InstancedMesh.md#isvisible)
- [metadata](InstancedMesh.md#metadata)
- [name](InstancedMesh.md#name)
- [occlusionQueryAlgorithmType](InstancedMesh.md#occlusionqueryalgorithmtype)
- [occlusionRetryCount](InstancedMesh.md#occlusionretrycount)
- [occlusionType](InstancedMesh.md#occlusiontype)
- [onAfterWorldMatrixUpdateObservable](InstancedMesh.md#onafterworldmatrixupdateobservable)
- [onCollideObservable](InstancedMesh.md#oncollideobservable)
- [onCollisionPositionChangeObservable](InstancedMesh.md#oncollisionpositionchangeobservable)
- [onDisposeObservable](InstancedMesh.md#ondisposeobservable)
- [onMaterialChangedObservable](InstancedMesh.md#onmaterialchangedobservable)
- [onReady](InstancedMesh.md#onready)
- [onRebuildObservable](InstancedMesh.md#onrebuildobservable)
- [outlineColor](InstancedMesh.md#outlinecolor)
- [outlineWidth](InstancedMesh.md#outlinewidth)
- [overlayAlpha](InstancedMesh.md#overlayalpha)
- [overlayColor](InstancedMesh.md#overlaycolor)
- [physicsImpostor](InstancedMesh.md#physicsimpostor)
- [reIntegrateRotationIntoRotationQuaternion](InstancedMesh.md#reintegraterotationintorotationquaternion)
- [renderOutline](InstancedMesh.md#renderoutline)
- [renderOverlay](InstancedMesh.md#renderoverlay)
- [reservedDataStore](InstancedMesh.md#reserveddatastore)
- [scalingDeterminant](InstancedMesh.md#scalingdeterminant)
- [showBoundingBox](InstancedMesh.md#showboundingbox)
- [showSubMeshesBoundingBox](InstancedMesh.md#showsubmeshesboundingbox)
- [state](InstancedMesh.md#state)
- [subMeshes](InstancedMesh.md#submeshes)
- [uniqueId](InstancedMesh.md#uniqueid)
- [useOctreeForCollisions](InstancedMesh.md#useoctreeforcollisions)
- [useOctreeForPicking](InstancedMesh.md#useoctreeforpicking)
- [useOctreeForRenderingSelection](InstancedMesh.md#useoctreeforrenderingselection)
- [CULLINGSTRATEGY\_BOUNDINGSPHERE\_ONLY](InstancedMesh.md#cullingstrategy_boundingsphere_only)
- [CULLINGSTRATEGY\_OPTIMISTIC\_INCLUSION](InstancedMesh.md#cullingstrategy_optimistic_inclusion)
- [CULLINGSTRATEGY\_OPTIMISTIC\_INCLUSION\_THEN\_BSPHERE\_ONLY](InstancedMesh.md#cullingstrategy_optimistic_inclusion_then_bsphere_only)
- [CULLINGSTRATEGY\_STANDARD](InstancedMesh.md#cullingstrategy_standard)
- [OCCLUSION\_ALGORITHM\_TYPE\_ACCURATE](InstancedMesh.md#occlusion_algorithm_type_accurate)
- [OCCLUSION\_ALGORITHM\_TYPE\_CONSERVATIVE](InstancedMesh.md#occlusion_algorithm_type_conservative)
- [OCCLUSION\_TYPE\_NONE](InstancedMesh.md#occlusion_type_none)
- [OCCLUSION\_TYPE\_OPTIMISTIC](InstancedMesh.md#occlusion_type_optimistic)
- [OCCLUSION\_TYPE\_STRICT](InstancedMesh.md#occlusion_type_strict)

### Accessors

- [\_positions](InstancedMesh.md#_positions)
- [absolutePosition](InstancedMesh.md#absoluteposition)
- [absoluteRotationQuaternion](InstancedMesh.md#absoluterotationquaternion)
- [absoluteScaling](InstancedMesh.md#absolutescaling)
- [animationPropertiesOverride](InstancedMesh.md#animationpropertiesoverride)
- [applyFog](InstancedMesh.md#applyfog)
- [bakedVertexAnimationManager](InstancedMesh.md#bakedvertexanimationmanager)
- [behaviors](InstancedMesh.md#behaviors)
- [billboardMode](InstancedMesh.md#billboardmode)
- [checkCollisions](InstancedMesh.md#checkcollisions)
- [collider](InstancedMesh.md#collider)
- [collisionGroup](InstancedMesh.md#collisiongroup)
- [collisionMask](InstancedMesh.md#collisionmask)
- [collisionResponse](InstancedMesh.md#collisionresponse)
- [collisionRetryCount](InstancedMesh.md#collisionretrycount)
- [computeBonesUsingShaders](InstancedMesh.md#computebonesusingshaders)
- [doNotSerialize](InstancedMesh.md#donotserialize)
- [enableDistantPicking](InstancedMesh.md#enabledistantpicking)
- [facetDepthSortFrom](InstancedMesh.md#facetdepthsortfrom)
- [facetNb](InstancedMesh.md#facetnb)
- [forward](InstancedMesh.md#forward)
- [hasBoundingInfo](InstancedMesh.md#hasboundinginfo)
- [hasInstances](InstancedMesh.md#hasinstances)
- [hasThinInstances](InstancedMesh.md#hasthininstances)
- [hasVertexAlpha](InstancedMesh.md#hasvertexalpha)
- [infiniteDistance](InstancedMesh.md#infinitedistance)
- [isAnInstance](InstancedMesh.md#isaninstance)
- [isBlocked](InstancedMesh.md#isblocked)
- [isFacetDataEnabled](InstancedMesh.md#isfacetdataenabled)
- [isWorldMatrixFrozen](InstancedMesh.md#isworldmatrixfrozen)
- [layerMask](InstancedMesh.md#layermask)
- [lightSources](InstancedMesh.md#lightsources)
- [material](InstancedMesh.md#material)
- [morphTargetManager](InstancedMesh.md#morphtargetmanager)
- [mustDepthSortFacets](InstancedMesh.md#mustdepthsortfacets)
- [nonUniformScaling](InstancedMesh.md#nonuniformscaling)
- [numBoneInfluencers](InstancedMesh.md#numboneinfluencers)
- [onClonedObservable](InstancedMesh.md#onclonedobservable)
- [onCollide](InstancedMesh.md#oncollide)
- [onCollisionPositionChange](InstancedMesh.md#oncollisionpositionchange)
- [onDispose](InstancedMesh.md#ondispose)
- [onEnabledStateChangedObservable](InstancedMesh.md#onenabledstatechangedobservable)
- [parent](InstancedMesh.md#parent)
- [partitioningBBoxRatio](InstancedMesh.md#partitioningbboxratio)
- [partitioningSubdivisions](InstancedMesh.md#partitioningsubdivisions)
- [position](InstancedMesh.md#position)
- [preserveParentRotationForBillboard](InstancedMesh.md#preserveparentrotationforbillboard)
- [receiveShadows](InstancedMesh.md#receiveshadows)
- [renderingGroupId](InstancedMesh.md#renderinggroupid)
- [right](InstancedMesh.md#right)
- [rotation](InstancedMesh.md#rotation)
- [rotationQuaternion](InstancedMesh.md#rotationquaternion)
- [scaling](InstancedMesh.md#scaling)
- [skeleton](InstancedMesh.md#skeleton)
- [sourceMesh](InstancedMesh.md#sourcemesh)
- [surroundingMeshes](InstancedMesh.md#surroundingmeshes)
- [up](InstancedMesh.md#up)
- [useBones](InstancedMesh.md#usebones)
- [useVertexColors](InstancedMesh.md#usevertexcolors)
- [visibility](InstancedMesh.md#visibility)
- [worldMatrixFromCache](InstancedMesh.md#worldmatrixfromcache)
- [BILLBOARDMODE\_ALL](InstancedMesh.md#billboardmode_all)
- [BILLBOARDMODE\_NONE](InstancedMesh.md#billboardmode_none)
- [BILLBOARDMODE\_USE\_POSITION](InstancedMesh.md#billboardmode_use_position)
- [BILLBOARDMODE\_X](InstancedMesh.md#billboardmode_x)
- [BILLBOARDMODE\_Y](InstancedMesh.md#billboardmode_y)
- [BILLBOARDMODE\_Z](InstancedMesh.md#billboardmode_z)

### Methods

- [\_buildUniformLayout](InstancedMesh.md#_builduniformlayout)
- [\_removeLightSource](InstancedMesh.md#_removelightsource)
- [\_resyncLightSource](InstancedMesh.md#_resynclightsource)
- [\_resyncLightSources](InstancedMesh.md#_resynclightsources)
- [addBehavior](InstancedMesh.md#addbehavior)
- [addChild](InstancedMesh.md#addchild)
- [addRotation](InstancedMesh.md#addrotation)
- [alignWithNormal](InstancedMesh.md#alignwithnormal)
- [applyImpulse](InstancedMesh.md#applyimpulse)
- [attachToBone](InstancedMesh.md#attachtobone)
- [beginAnimation](InstancedMesh.md#beginanimation)
- [buildBoundingInfo](InstancedMesh.md#buildboundinginfo)
- [calcMovePOV](InstancedMesh.md#calcmovepov)
- [calcRotatePOV](InstancedMesh.md#calcrotatepov)
- [clone](InstancedMesh.md#clone)
- [computeWorldMatrix](InstancedMesh.md#computeworldmatrix)
- [createAnimationRange](InstancedMesh.md#createanimationrange)
- [createInstance](InstancedMesh.md#createinstance)
- [createNormals](InstancedMesh.md#createnormals)
- [createOrUpdateSubmeshesOctree](InstancedMesh.md#createorupdatesubmeshesoctree)
- [deleteAnimationRange](InstancedMesh.md#deleteanimationrange)
- [detachFromBone](InstancedMesh.md#detachfrombone)
- [disableEdgesRendering](InstancedMesh.md#disableedgesrendering)
- [disableFacetData](InstancedMesh.md#disablefacetdata)
- [dispose](InstancedMesh.md#dispose)
- [enableEdgesRendering](InstancedMesh.md#enableedgesrendering)
- [freezeWorldMatrix](InstancedMesh.md#freezeworldmatrix)
- [getAbsolutePivotPoint](InstancedMesh.md#getabsolutepivotpoint)
- [getAbsolutePivotPointToRef](InstancedMesh.md#getabsolutepivotpointtoref)
- [getAbsolutePosition](InstancedMesh.md#getabsoluteposition)
- [getAnimationByName](InstancedMesh.md#getanimationbyname)
- [getAnimationRange](InstancedMesh.md#getanimationrange)
- [getAnimationRanges](InstancedMesh.md#getanimationranges)
- [getBehaviorByName](InstancedMesh.md#getbehaviorbyname)
- [getBoundingInfo](InstancedMesh.md#getboundinginfo)
- [getChildMeshes](InstancedMesh.md#getchildmeshes)
- [getChildTransformNodes](InstancedMesh.md#getchildtransformnodes)
- [getChildren](InstancedMesh.md#getchildren)
- [getClassName](InstancedMesh.md#getclassname)
- [getClosestFacetAtCoordinates](InstancedMesh.md#getclosestfacetatcoordinates)
- [getClosestFacetAtLocalCoordinates](InstancedMesh.md#getclosestfacetatlocalcoordinates)
- [getConnectedParticleSystems](InstancedMesh.md#getconnectedparticlesystems)
- [getDescendants](InstancedMesh.md#getdescendants)
- [getDirection](InstancedMesh.md#getdirection)
- [getDirectionToRef](InstancedMesh.md#getdirectiontoref)
- [getDistanceToCamera](InstancedMesh.md#getdistancetocamera)
- [getEngine](InstancedMesh.md#getengine)
- [getFacetDataParameters](InstancedMesh.md#getfacetdataparameters)
- [getFacetLocalNormals](InstancedMesh.md#getfacetlocalnormals)
- [getFacetLocalPartitioning](InstancedMesh.md#getfacetlocalpartitioning)
- [getFacetLocalPositions](InstancedMesh.md#getfacetlocalpositions)
- [getFacetNormal](InstancedMesh.md#getfacetnormal)
- [getFacetNormalToRef](InstancedMesh.md#getfacetnormaltoref)
- [getFacetPosition](InstancedMesh.md#getfacetposition)
- [getFacetPositionToRef](InstancedMesh.md#getfacetpositiontoref)
- [getFacetsAtLocalCoordinates](InstancedMesh.md#getfacetsatlocalcoordinates)
- [getHierarchyBoundingVectors](InstancedMesh.md#gethierarchyboundingvectors)
- [getIndices](InstancedMesh.md#getindices)
- [getLOD](InstancedMesh.md#getlod)
- [getMaterialForRenderPass](InstancedMesh.md#getmaterialforrenderpass)
- [getMeshUniformBuffer](InstancedMesh.md#getmeshuniformbuffer)
- [getNormalsData](InstancedMesh.md#getnormalsdata)
- [getPhysicsImpostor](InstancedMesh.md#getphysicsimpostor)
- [getPivotMatrix](InstancedMesh.md#getpivotmatrix)
- [getPivotPoint](InstancedMesh.md#getpivotpoint)
- [getPivotPointToRef](InstancedMesh.md#getpivotpointtoref)
- [getPoseMatrix](InstancedMesh.md#getposematrix)
- [getPositionData](InstancedMesh.md#getpositiondata)
- [getPositionExpressedInLocalSpace](InstancedMesh.md#getpositionexpressedinlocalspace)
- [getPositionInCameraSpace](InstancedMesh.md#getpositionincameraspace)
- [getScene](InstancedMesh.md#getscene)
- [getTotalIndices](InstancedMesh.md#gettotalindices)
- [getTotalVertices](InstancedMesh.md#gettotalvertices)
- [getVerticesData](InstancedMesh.md#getverticesdata)
- [getWorldMatrix](InstancedMesh.md#getworldmatrix)
- [instantiateHierarchy](InstancedMesh.md#instantiatehierarchy)
- [intersects](InstancedMesh.md#intersects)
- [intersectsMesh](InstancedMesh.md#intersectsmesh)
- [intersectsPoint](InstancedMesh.md#intersectspoint)
- [isCompletelyInFrustum](InstancedMesh.md#iscompletelyinfrustum)
- [isDescendantOf](InstancedMesh.md#isdescendantof)
- [isDisposed](InstancedMesh.md#isdisposed)
- [isEnabled](InstancedMesh.md#isenabled)
- [isInFrustum](InstancedMesh.md#isinfrustum)
- [isReady](InstancedMesh.md#isready)
- [isUsingPivotMatrix](InstancedMesh.md#isusingpivotmatrix)
- [isVerticesDataPresent](InstancedMesh.md#isverticesdatapresent)
- [locallyTranslate](InstancedMesh.md#locallytranslate)
- [lookAt](InstancedMesh.md#lookat)
- [markAsDirty](InstancedMesh.md#markasdirty)
- [movePOV](InstancedMesh.md#movepov)
- [moveWithCollisions](InstancedMesh.md#movewithcollisions)
- [normalizeToUnitCube](InstancedMesh.md#normalizetounitcube)
- [refreshBoundingInfo](InstancedMesh.md#refreshboundinginfo)
- [registerAfterWorldMatrixUpdate](InstancedMesh.md#registerafterworldmatrixupdate)
- [releaseSubMeshes](InstancedMesh.md#releasesubmeshes)
- [removeBehavior](InstancedMesh.md#removebehavior)
- [removeChild](InstancedMesh.md#removechild)
- [resetDrawCache](InstancedMesh.md#resetdrawcache)
- [resetLocalMatrix](InstancedMesh.md#resetlocalmatrix)
- [rotate](InstancedMesh.md#rotate)
- [rotateAround](InstancedMesh.md#rotatearound)
- [rotatePOV](InstancedMesh.md#rotatepov)
- [serialize](InstancedMesh.md#serialize)
- [serializeAnimationRanges](InstancedMesh.md#serializeanimationranges)
- [setAbsolutePosition](InstancedMesh.md#setabsoluteposition)
- [setBoundingInfo](InstancedMesh.md#setboundinginfo)
- [setDirection](InstancedMesh.md#setdirection)
- [setEnabled](InstancedMesh.md#setenabled)
- [setIndices](InstancedMesh.md#setindices)
- [setMaterialForRenderPass](InstancedMesh.md#setmaterialforrenderpass)
- [setParent](InstancedMesh.md#setparent)
- [setPhysicsLinkWith](InstancedMesh.md#setphysicslinkwith)
- [setPivotMatrix](InstancedMesh.md#setpivotmatrix)
- [setPivotPoint](InstancedMesh.md#setpivotpoint)
- [setPositionWithLocalVector](InstancedMesh.md#setpositionwithlocalvector)
- [setPreTransformMatrix](InstancedMesh.md#setpretransformmatrix)
- [setVerticesData](InstancedMesh.md#setverticesdata)
- [toString](InstancedMesh.md#tostring)
- [transferToEffect](InstancedMesh.md#transfertoeffect)
- [translate](InstancedMesh.md#translate)
- [unfreezeWorldMatrix](InstancedMesh.md#unfreezeworldmatrix)
- [unregisterAfterWorldMatrixUpdate](InstancedMesh.md#unregisterafterworldmatrixupdate)
- [updateFacetData](InstancedMesh.md#updatefacetdata)
- [updateIndices](InstancedMesh.md#updateindices)
- [updatePoseMatrix](InstancedMesh.md#updateposematrix)
- [updateVerticesData](InstancedMesh.md#updateverticesdata)
- [AddNodeConstructor](InstancedMesh.md#addnodeconstructor)
- [Construct](InstancedMesh.md#construct)
- [Parse](InstancedMesh.md#parse)
- [ParseAnimationRanges](InstancedMesh.md#parseanimationranges)

## Constructors

### constructor

• **new InstancedMesh**(`name`, `source`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `source` | [`Mesh`](Mesh.md) |

#### Overrides

[AbstractMesh](AbstractMesh.md).[constructor](AbstractMesh.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/instancedMesh.ts:45

## Properties

### \_billboardWorldMatrix

• `Private` **\_billboardWorldMatrix**: [`Matrix`](Matrix.md)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/instancedMesh.ts:36

___

### \_boundingInfo

• `Protected` **\_boundingInfo**: [`Nullable`](../modules.md#nullable)[`BoundingInfo`](BoundingInfo.md) = `null`

#### Inherited from

[AbstractMesh](AbstractMesh.md).[_boundingInfo](AbstractMesh.md#_boundinginfo)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:729

___

### \_boundingInfoIsDirty

• `Protected` **\_boundingInfoIsDirty**: `boolean` = `true`

#### Inherited from

[AbstractMesh](AbstractMesh.md).[_boundingInfoIsDirty](AbstractMesh.md#_boundinginfoisdirty)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:730

___

### \_currentLOD

• `Private` **\_currentLOD**: [`Mesh`](Mesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/instancedMesh.ts:35

___

### \_isDirty

• `Protected` **\_isDirty**: `boolean` = `false`

#### Inherited from

[AbstractMesh](AbstractMesh.md).[_isDirty](AbstractMesh.md#_isdirty)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:43

___

### \_isWorldMatrixFrozen

• `Protected` **\_isWorldMatrixFrozen**: `boolean` = `false`

#### Inherited from

[AbstractMesh](AbstractMesh.md).[_isWorldMatrixFrozen](AbstractMesh.md#_isworldmatrixfrozen)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:161

___

### \_parentNode

• `Protected` **\_parentNode**: [`Nullable`](../modules.md#nullable)[`Node`](Node.md) = `null`

#### Inherited from

[AbstractMesh](AbstractMesh.md).[_parentNode](AbstractMesh.md#_parentnode)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:176

___

### \_ranges

• `Protected` **\_ranges**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: [`Nullable`](../modules.md#nullable)`AnimationRange`

#### Inherited from

[AbstractMesh](AbstractMesh.md).[_ranges](AbstractMesh.md#_ranges)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:154

___

### \_scaling

• `Protected` **\_scaling**: [`Vector3`](Vector3.md)

#### Inherited from

[AbstractMesh](AbstractMesh.md).[_scaling](AbstractMesh.md#_scaling)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:62

___

### \_sourceMesh

• `Private` **\_sourceMesh**: [`Mesh`](Mesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/instancedMesh.ts:34

___

### actionManager

• **actionManager**: [`Nullable`](../modules.md#nullable)[`AbstractActionManager`](AbstractActionManager.md) = `null`

Gets or sets the current action manager

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions

#### Inherited from

[AbstractMesh](AbstractMesh.md).[actionManager](AbstractMesh.md#actionmanager)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:646

___

### alphaIndex

• **alphaIndex**: `number` = `Number.MAX_VALUE`

Gets or sets the alpha index used to sort transparent meshes

**`See`**

https://doc.babylonjs.com/resources/transparency_and_how_meshes_are_rendered#alpha-index

#### Inherited from

[AbstractMesh](AbstractMesh.md).[alphaIndex](AbstractMesh.md#alphaindex)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:406

___

### alwaysSelectAsActiveMesh

• **alwaysSelectAsActiveMesh**: `boolean` = `false`

True if the mesh must be rendered in any case (this will shortcut the frustum clipping phase)

#### Inherited from

[AbstractMesh](AbstractMesh.md).[alwaysSelectAsActiveMesh](AbstractMesh.md#alwaysselectasactivemesh)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:635

___

### animations

• **animations**: [`Animation`](Animation.md)[]

Gets a list of Animations associated with the node

#### Inherited from

[AbstractMesh](AbstractMesh.md).[animations](AbstractMesh.md#animations)

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

#### Inherited from

[AbstractMesh](AbstractMesh.md).[cullingStrategy](AbstractMesh.md#cullingstrategy)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:214

___

### definedFacingForward

• **definedFacingForward**: `boolean` = `true`

Gets or sets the orientation for POV movement & rotation

#### Inherited from

[AbstractMesh](AbstractMesh.md).[definedFacingForward](AbstractMesh.md#definedfacingforward)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:371

___

### doNotSyncBoundingInfo

• **doNotSyncBoundingInfo**: `boolean` = `false`

Gets or sets a boolean indicating that the bounding info does not need to be kept in sync (for performance reason)

#### Inherited from

[AbstractMesh](AbstractMesh.md).[doNotSyncBoundingInfo](AbstractMesh.md#donotsyncboundinginfo)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:640

___

### edgesColor

• **edgesColor**: [`Color4`](Color4.md)

Defines edge color used when edgesRenderer is enabled

**`See`**

https://www.babylonjs-playground.com/#10OJSG#13

#### Inherited from

[AbstractMesh](AbstractMesh.md).[edgesColor](AbstractMesh.md#edgescolor)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:723

___

### edgesRenderer

• **edgesRenderer**: [`Nullable`](../modules.md#nullable)[`EdgesRenderer`](EdgesRenderer.md)

Gets the edgesRenderer associated with the mesh

#### Inherited from

[AbstractMesh](AbstractMesh.md).[edgesRenderer](AbstractMesh.md#edgesrenderer)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:35

___

### edgesWidth

• **edgesWidth**: `number` = `1`

Defines edge width used when edgesRenderer is enabled

**`See`**

https://www.babylonjs-playground.com/#10OJSG#13

#### Inherited from

[AbstractMesh](AbstractMesh.md).[edgesWidth](AbstractMesh.md#edgeswidth)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:718

___

### ellipsoid

• **ellipsoid**: [`Vector3`](Vector3.md)

Gets or sets the ellipsoid used to impersonate this mesh when using collision engine (default is (0.5, 1, 0.5))

**`See`**

https://doc.babylonjs.com/babylon101/cameras,_mesh_collisions_and_gravity

#### Inherited from

[AbstractMesh](AbstractMesh.md).[ellipsoid](AbstractMesh.md#ellipsoid)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:652

___

### ellipsoidOffset

• **ellipsoidOffset**: [`Vector3`](Vector3.md)

Gets or sets the ellipsoid offset used to impersonate this mesh when using collision engine (default is (0, 0, 0))

**`See`**

https://doc.babylonjs.com/babylon101/cameras,_mesh_collisions_and_gravity

#### Inherited from

[AbstractMesh](AbstractMesh.md).[ellipsoidOffset](AbstractMesh.md#ellipsoidoffset)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:657

___

### enablePointerMoveEvents

• **enablePointerMoveEvents**: `boolean` = `false`

Gets or sets a boolean indicating that pointer move events must be supported on this mesh (false by default)

#### Inherited from

[AbstractMesh](AbstractMesh.md).[enablePointerMoveEvents](AbstractMesh.md#enablepointermoveevents)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:439

___

### forceRenderingWhenOccluded

• **forceRenderingWhenOccluded**: `boolean`

Flag to force rendering the mesh even if occluded

**`See`**

https://doc.babylonjs.com/features/occlusionquery

#### Inherited from

[AbstractMesh](AbstractMesh.md).[forceRenderingWhenOccluded](AbstractMesh.md#forcerenderingwhenoccluded)

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.query.ts:405

___

### id

• **id**: `string`

Gets or sets the id of the node

#### Inherited from

[AbstractMesh](AbstractMesh.md).[id](AbstractMesh.md#id)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:97

___

### ignoreNonUniformScaling

• **ignoreNonUniformScaling**: `boolean` = `false`

Gets or sets a boolean indicating that non uniform scaling (when at least one component is different from others) should be ignored.
By default the system will update normals to compensate

#### Inherited from

[AbstractMesh](AbstractMesh.md).[ignoreNonUniformScaling](AbstractMesh.md#ignorenonuniformscaling)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:138

___

### inspectableCustomProperties

• **inspectableCustomProperties**: [`IInspectable`](../interfaces/IInspectable.md)[]

List of inspectable custom properties (used by the Inspector)

**`See`**

https://doc.babylonjs.com/how_to/debug_layer#extensibility

#### Inherited from

[AbstractMesh](AbstractMesh.md).[inspectableCustomProperties](AbstractMesh.md#inspectablecustomproperties)

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

#### Inherited from

[AbstractMesh](AbstractMesh.md).[instancedBuffers](AbstractMesh.md#instancedbuffers)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/instancedMesh.ts:594

___

### isBlocker

• **isBlocker**: `boolean` = `false`

Gets or sets a boolean indicating if the mesh must be considered as a ray blocker for lens flares (false by default)

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_lens_flares

#### Inherited from

[AbstractMesh](AbstractMesh.md).[isBlocker](AbstractMesh.md#isblocker)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:434

___

### isNearGrabbable

• **isNearGrabbable**: `boolean` = `false`

Gets or sets a boolean indicating if the mesh can be near grabbed. Default is false

#### Inherited from

[AbstractMesh](AbstractMesh.md).[isNearGrabbable](AbstractMesh.md#isneargrabbable)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:426

___

### isNearPickable

• **isNearPickable**: `boolean` = `false`

Gets or sets a boolean indicating if the mesh can be near picked. Default is false

#### Inherited from

[AbstractMesh](AbstractMesh.md).[isNearPickable](AbstractMesh.md#isnearpickable)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:421

___

### isOccluded

• **isOccluded**: `boolean`

Gets or sets whether the mesh is occluded or not, it is used also to set the initial state of the mesh to be occluded or not

**`See`**

https://doc.babylonjs.com/features/occlusionquery

#### Inherited from

[AbstractMesh](AbstractMesh.md).[isOccluded](AbstractMesh.md#isoccluded)

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.query.ts:393

___

### isOcclusionQueryInProgress

• **isOcclusionQueryInProgress**: `boolean`

Flag to check the progress status of the query

**`See`**

https://doc.babylonjs.com/features/occlusionquery

#### Inherited from

[AbstractMesh](AbstractMesh.md).[isOcclusionQueryInProgress](AbstractMesh.md#isocclusionqueryinprogress)

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.query.ts:399

___

### isPickable

• **isPickable**: `boolean` = `true`

Gets or sets a boolean indicating if the mesh can be picked (by scene.pick for instance or through actions). Default is true

#### Inherited from

[AbstractMesh](AbstractMesh.md).[isPickable](AbstractMesh.md#ispickable)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:416

___

### isVisible

• **isVisible**: `boolean` = `true`

Gets or sets a boolean indicating if the mesh is visible (renderable). Default is true

#### Inherited from

[AbstractMesh](AbstractMesh.md).[isVisible](AbstractMesh.md#isvisible)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:411

___

### metadata

• **metadata**: `any` = `null`

Gets or sets an object used to store user defined information for the node

#### Inherited from

[AbstractMesh](AbstractMesh.md).[metadata](AbstractMesh.md#metadata)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:115

___

### name

• **name**: `string`

Gets or sets the name of the node

#### Inherited from

[AbstractMesh](AbstractMesh.md).[name](AbstractMesh.md#name)

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

#### Inherited from

[AbstractMesh](AbstractMesh.md).[occlusionQueryAlgorithmType](AbstractMesh.md#occlusionqueryalgorithmtype)

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.query.ts:387

___

### occlusionRetryCount

• **occlusionRetryCount**: `number`

This number indicates the number of allowed retries before stop the occlusion query, this is useful if the occlusion query is taking long time before to the query result is retrieved, the query result indicates if the object is visible within the scene or not and based on that Babylon.Js engine decides to show or hide the object.
The default value is -1 which means don't break the query and wait till the result

**`See`**

https://doc.babylonjs.com/features/occlusionquery

#### Inherited from

[AbstractMesh](AbstractMesh.md).[occlusionRetryCount](AbstractMesh.md#occlusionretrycount)

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

#### Inherited from

[AbstractMesh](AbstractMesh.md).[occlusionType](AbstractMesh.md#occlusiontype)

#### Defined in

https://github.com/babylon.js/core/src/Engines/Extensions/engine.query.ts:379

___

### onAfterWorldMatrixUpdateObservable

• **onAfterWorldMatrixUpdateObservable**: [`Observable`](Observable.md)[`TransformNode`](TransformNode.md)

An event triggered after the world matrix is updated

#### Inherited from

[AbstractMesh](AbstractMesh.md).[onAfterWorldMatrixUpdateObservable](AbstractMesh.md#onafterworldmatrixupdateobservable)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:169

___

### onCollideObservable

• **onCollideObservable**: [`Observable`](Observable.md)[`AbstractMesh`](AbstractMesh.md)

An event triggered when this mesh collides with another one

#### Inherited from

[AbstractMesh](AbstractMesh.md).[onCollideObservable](AbstractMesh.md#oncollideobservable)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:338

___

### onCollisionPositionChangeObservable

• **onCollisionPositionChangeObservable**: [`Observable`](Observable.md)[`Vector3`](Vector3.md)

An event triggered when the collision's position changes

#### Inherited from

[AbstractMesh](AbstractMesh.md).[onCollisionPositionChangeObservable](AbstractMesh.md#oncollisionpositionchangeobservable)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:351

___

### onDisposeObservable

• **onDisposeObservable**: [`Observable`](Observable.md)[`Node`](Node.md)

An event triggered when the mesh is disposed

#### Inherited from

[AbstractMesh](AbstractMesh.md).[onDisposeObservable](AbstractMesh.md#ondisposeobservable)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:300

___

### onMaterialChangedObservable

• **onMaterialChangedObservable**: [`Observable`](Observable.md)[`AbstractMesh`](AbstractMesh.md)

An event triggered when material is changed

#### Inherited from

[AbstractMesh](AbstractMesh.md).[onMaterialChangedObservable](AbstractMesh.md#onmaterialchangedobservable)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:364

___

### onReady

• **onReady**: [`Nullable`](../modules.md#nullable)(`node`: [`Node`](Node.md)) => `void` = `null`

Callback raised when the node is ready to be used

#### Inherited from

[AbstractMesh](AbstractMesh.md).[onReady](AbstractMesh.md#onready)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:159

___

### onRebuildObservable

• **onRebuildObservable**: [`Observable`](Observable.md)[`AbstractMesh`](AbstractMesh.md)

An event triggered when the mesh is rebuilt.

#### Inherited from

[AbstractMesh](AbstractMesh.md).[onRebuildObservable](AbstractMesh.md#onrebuildobservable)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:807

___

### outlineColor

• **outlineColor**: [`Color3`](Color3.md)

Defines color to use when rendering outline

#### Inherited from

[AbstractMesh](AbstractMesh.md).[outlineColor](AbstractMesh.md#outlinecolor)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:524

___

### outlineWidth

• **outlineWidth**: `number` = `0.02`

Define width to use when rendering outline

#### Inherited from

[AbstractMesh](AbstractMesh.md).[outlineWidth](AbstractMesh.md#outlinewidth)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:526

___

### overlayAlpha

• **overlayAlpha**: `number` = `0.5`

Defines alpha to use when rendering overlay

#### Inherited from

[AbstractMesh](AbstractMesh.md).[overlayAlpha](AbstractMesh.md#overlayalpha)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:531

___

### overlayColor

• **overlayColor**: [`Color3`](Color3.md)

Defines color to use when rendering overlay

#### Inherited from

[AbstractMesh](AbstractMesh.md).[overlayColor](AbstractMesh.md#overlaycolor)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:529

___

### physicsImpostor

• **physicsImpostor**: [`Nullable`](../modules.md#nullable)[`PhysicsImpostor`](PhysicsImpostor.md)

Gets or sets impostor used for physic simulation

**`See`**

https://doc.babylonjs.com/features/physics_engine

#### Inherited from

[AbstractMesh](AbstractMesh.md).[physicsImpostor](AbstractMesh.md#physicsimpostor)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsEngineComponent.ts:169

___

### reIntegrateRotationIntoRotationQuaternion

• **reIntegrateRotationIntoRotationQuaternion**: `boolean` = `false`

Gets or sets a boolean indicating that even if rotationQuaternion is defined, you can keep updating rotation property and Babylon.js will just mix both

#### Inherited from

[AbstractMesh](AbstractMesh.md).[reIntegrateRotationIntoRotationQuaternion](AbstractMesh.md#reintegraterotationintorotationquaternion)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:144

___

### renderOutline

• **renderOutline**: `boolean`

Gets or sets a boolean indicating if the outline must be rendered as well

**`See`**

https://www.babylonjs-playground.com/#10WJ5S#3

#### Inherited from

[AbstractMesh](AbstractMesh.md).[renderOutline](AbstractMesh.md#renderoutline)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/outlineRenderer.ts:48

___

### renderOverlay

• **renderOverlay**: `boolean`

Gets or sets a boolean indicating if the overlay must be rendered as well

**`See`**

https://www.babylonjs-playground.com/#10WJ5S#2

#### Inherited from

[AbstractMesh](AbstractMesh.md).[renderOverlay](AbstractMesh.md#renderoverlay)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/outlineRenderer.ts:56

___

### reservedDataStore

• **reservedDataStore**: `any` = `null`

For internal use only. Please do not use.

#### Inherited from

[AbstractMesh](AbstractMesh.md).[reservedDataStore](AbstractMesh.md#reserveddatastore)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:120

___

### scalingDeterminant

• **scalingDeterminant**: `number` = `1`

Multiplication factor on scale x/y/z when computing the world matrix. Eg. for a 1x1x1 cube setting this to 2 will make it a 2x2x2 cube

#### Inherited from

[AbstractMesh](AbstractMesh.md).[scalingDeterminant](AbstractMesh.md#scalingdeterminant)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:113

___

### showBoundingBox

• **showBoundingBox**: `boolean`

Gets or sets a boolean indicating if the bounding box must be rendered as well (false by default)

#### Inherited from

[AbstractMesh](AbstractMesh.md).[showBoundingBox](AbstractMesh.md#showboundingbox)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/boundingBoxRenderer.ts:76

___

### showSubMeshesBoundingBox

• **showSubMeshesBoundingBox**: `boolean` = `false`

Gets or sets a boolean indicating that bounding boxes of subMeshes must be rendered as well (false by default)

#### Inherited from

[AbstractMesh](AbstractMesh.md).[showSubMeshesBoundingBox](AbstractMesh.md#showsubmeshesboundingbox)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:429

___

### state

• **state**: `string` = `""`

Gets or sets a string used to store user defined state for the node

#### Inherited from

[AbstractMesh](AbstractMesh.md).[state](AbstractMesh.md#state)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:109

___

### subMeshes

• **subMeshes**: [`SubMesh`](SubMesh.md)[]

Gets or sets the list of subMeshes

**`See`**

https://doc.babylonjs.com/how_to/multi_materials

#### Inherited from

[AbstractMesh](AbstractMesh.md).[subMeshes](AbstractMesh.md#submeshes)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:738

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the node

#### Inherited from

[AbstractMesh](AbstractMesh.md).[uniqueId](AbstractMesh.md#uniqueid)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:103

___

### useOctreeForCollisions

• **useOctreeForCollisions**: `boolean` = `true`

Gets or sets a boolean indicating that internal octree (if available) can be used to boost submeshes collision (true by default)

#### Inherited from

[AbstractMesh](AbstractMesh.md).[useOctreeForCollisions](AbstractMesh.md#useoctreeforcollisions)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:614

___

### useOctreeForPicking

• **useOctreeForPicking**: `boolean` = `true`

Gets or sets a boolean indicating that internal octree (if available) can be used to boost submeshes picking (true by default)

#### Inherited from

[AbstractMesh](AbstractMesh.md).[useOctreeForPicking](AbstractMesh.md#useoctreeforpicking)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:612

___

### useOctreeForRenderingSelection

• **useOctreeForRenderingSelection**: `boolean` = `true`

Gets or sets a boolean indicating that internal octree (if available) can be used to boost submeshes selection (true by default)

#### Inherited from

[AbstractMesh](AbstractMesh.md).[useOctreeForRenderingSelection](AbstractMesh.md#useoctreeforrenderingselection)

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

#### Inherited from

[AbstractMesh](AbstractMesh.md).[CULLINGSTRATEGY_BOUNDINGSPHERE_ONLY](AbstractMesh.md#cullingstrategy_boundingsphere_only)

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

#### Inherited from

[AbstractMesh](AbstractMesh.md).[CULLINGSTRATEGY_OPTIMISTIC_INCLUSION](AbstractMesh.md#cullingstrategy_optimistic_inclusion)

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

#### Inherited from

[AbstractMesh](AbstractMesh.md).[CULLINGSTRATEGY_OPTIMISTIC_INCLUSION_THEN_BSPHERE_ONLY](AbstractMesh.md#cullingstrategy_optimistic_inclusion_then_bsphere_only)

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

#### Inherited from

[AbstractMesh](AbstractMesh.md).[CULLINGSTRATEGY_STANDARD](AbstractMesh.md#cullingstrategy_standard)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:136

___

### OCCLUSION\_ALGORITHM\_TYPE\_ACCURATE

▪ `Static` **OCCLUSION\_ALGORITHM\_TYPE\_ACCURATE**: `number` = `0`

Use an accurate occlusion algorithm

#### Inherited from

[AbstractMesh](AbstractMesh.md).[OCCLUSION_ALGORITHM_TYPE_ACCURATE](AbstractMesh.md#occlusion_algorithm_type_accurate)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:126

___

### OCCLUSION\_ALGORITHM\_TYPE\_CONSERVATIVE

▪ `Static` **OCCLUSION\_ALGORITHM\_TYPE\_CONSERVATIVE**: `number` = `1`

Use a conservative occlusion algorithm

#### Inherited from

[AbstractMesh](AbstractMesh.md).[OCCLUSION_ALGORITHM_TYPE_CONSERVATIVE](AbstractMesh.md#occlusion_algorithm_type_conservative)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:128

___

### OCCLUSION\_TYPE\_NONE

▪ `Static` **OCCLUSION\_TYPE\_NONE**: `number` = `0`

No occlusion

#### Inherited from

[AbstractMesh](AbstractMesh.md).[OCCLUSION_TYPE_NONE](AbstractMesh.md#occlusion_type_none)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:120

___

### OCCLUSION\_TYPE\_OPTIMISTIC

▪ `Static` **OCCLUSION\_TYPE\_OPTIMISTIC**: `number` = `1`

Occlusion set to optimistic

#### Inherited from

[AbstractMesh](AbstractMesh.md).[OCCLUSION_TYPE_OPTIMISTIC](AbstractMesh.md#occlusion_type_optimistic)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:122

___

### OCCLUSION\_TYPE\_STRICT

▪ `Static` **OCCLUSION\_TYPE\_STRICT**: `number` = `2`

Occlusion set to strict

#### Inherited from

[AbstractMesh](AbstractMesh.md).[OCCLUSION_TYPE_STRICT](AbstractMesh.md#occlusion_type_strict)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:124

## Accessors

### \_positions

• `get` **_positions**(): [`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md)[]

#### Returns

[`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md)[]

#### Overrides

AbstractMesh.\_positions

#### Defined in

https://github.com/babylon.js/core/src/Meshes/instancedMesh.ts:299

___

### absolutePosition

• `get` **absolutePosition**(): [`Vector3`](Vector3.md)

Returns the current mesh absolute position.
Returns a Vector3.

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

AbstractMesh.absolutePosition

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

AbstractMesh.absoluteRotationQuaternion

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

AbstractMesh.absoluteScaling

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:352

___

### animationPropertiesOverride

• `get` **animationPropertiesOverride**(): [`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md)

Gets or sets the animation properties override

#### Returns

[`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md)

#### Inherited from

AbstractMesh.animationPropertiesOverride

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

AbstractMesh.animationPropertiesOverride

#### Defined in

https://github.com/babylon.js/core/src/node.ts:282

___

### applyFog

• `get` **applyFog**(): `boolean`

Gets or sets a boolean indicating that this mesh will allow fog to be rendered on it (true by default)

#### Returns

`boolean`

#### Inherited from

AbstractMesh.applyFog

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:589

• `set` **applyFog**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

AbstractMesh.applyFog

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

#### Inherited from

AbstractMesh.bakedVertexAnimationManager

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:306

• `set` **bakedVertexAnimationManager**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`IBakedVertexAnimationManager`](../interfaces/IBakedVertexAnimationManager.md) |

#### Returns

`void`

#### Inherited from

AbstractMesh.bakedVertexAnimationManager

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

AbstractMesh.behaviors

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

AbstractMesh.billboardMode

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

AbstractMesh.billboardMode

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

#### Inherited from

AbstractMesh.checkCollisions

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:1686

• `set` **checkCollisions**(`collisionEnabled`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `collisionEnabled` | `boolean` |

#### Returns

`void`

#### Inherited from

AbstractMesh.checkCollisions

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

#### Inherited from

AbstractMesh.collider

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:1698

___

### collisionGroup

• `get` **collisionGroup**(): `number`

Gets or sets the current collision group mask (-1 by default).
A collision between A and B will happen if A.collisionGroup & b.collisionMask !== 0

#### Returns

`number`

#### Inherited from

AbstractMesh.collisionGroup

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:688

• `set` **collisionGroup**(`mask`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `mask` | `number` |

#### Returns

`void`

#### Inherited from

AbstractMesh.collisionGroup

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:692

___

### collisionMask

• `get` **collisionMask**(): `number`

Gets or sets a collision mask used to mask collisions (default is -1).
A collision between A and B will happen if A.collisionGroup & b.collisionMask !== 0

#### Returns

`number`

#### Inherited from

AbstractMesh.collisionMask

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:663

• `set` **collisionMask**(`mask`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `mask` | `number` |

#### Returns

`void`

#### Inherited from

AbstractMesh.collisionMask

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

#### Inherited from

AbstractMesh.collisionResponse

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:677

• `set` **collisionResponse**(`response`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `response` | `boolean` |

#### Returns

`void`

#### Inherited from

AbstractMesh.collisionResponse

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:681

___

### collisionRetryCount

• `get` **collisionRetryCount**(): `number`

number of collision detection tries. Change this value if not all collisions are detected and handled properly

#### Returns

`number`

#### Inherited from

AbstractMesh.collisionRetryCount

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:272

• `set` **collisionRetryCount**(`retryCount`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `retryCount` | `number` |

#### Returns

`void`

#### Inherited from

AbstractMesh.collisionRetryCount

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:275

___

### computeBonesUsingShaders

• `get` **computeBonesUsingShaders**(): `boolean`

Gets or sets a boolean indicating that bone animations must be computed by the CPU (false by default)

#### Returns

`boolean`

#### Inherited from

AbstractMesh.computeBonesUsingShaders

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:563

• `set` **computeBonesUsingShaders**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

AbstractMesh.computeBonesUsingShaders

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:566

___

### doNotSerialize

• `get` **doNotSerialize**(): `boolean`

Gets or sets a boolean used to define if the node must be serialized

#### Returns

`boolean`

#### Inherited from

AbstractMesh.doNotSerialize

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

AbstractMesh.doNotSerialize

#### Defined in

https://github.com/babylon.js/core/src/node.ts:143

___

### enableDistantPicking

• `get` **enableDistantPicking**(): `boolean`

When enabled, decompose picking matrices for better precision with large values for mesh position and scling

#### Returns

`boolean`

#### Inherited from

AbstractMesh.enableDistantPicking

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:602

• `set` **enableDistantPicking**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

AbstractMesh.enableDistantPicking

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

#### Inherited from

AbstractMesh.facetDepthSortFrom

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:264

• `set` **facetDepthSortFrom**(`location`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `location` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Inherited from

AbstractMesh.facetDepthSortFrom

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

#### Inherited from

AbstractMesh.facetNb

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:220

___

### forward

• `get` **forward**(): [`Vector3`](Vector3.md)

The forward direction of that transform in world space.

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

AbstractMesh.forward

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:253

___

### hasBoundingInfo

• `get` **hasBoundingInfo**(): `boolean`

Returns true if there is already a bounding info

#### Returns

`boolean`

#### Inherited from

AbstractMesh.hasBoundingInfo

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:1230

___

### hasInstances

• `get` **hasInstances**(): `boolean`

Gets a boolean indicating if this mesh has instances

#### Returns

`boolean`

#### Inherited from

AbstractMesh.hasInstances

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:1334

___

### hasThinInstances

• `get` **hasThinInstances**(): `boolean`

Gets a boolean indicating if this mesh has thin instances

#### Returns

`boolean`

#### Inherited from

AbstractMesh.hasThinInstances

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:1341

___

### hasVertexAlpha

• `get` **hasVertexAlpha**(): `boolean`

Gets or sets a boolean indicating that this mesh contains vertex color data with alpha values

#### Returns

`boolean`

#### Inherited from

AbstractMesh.hasVertexAlpha

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:534

• `set` **hasVertexAlpha**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

AbstractMesh.hasVertexAlpha

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:537

___

### infiniteDistance

• `get` **infiniteDistance**(): `boolean`

Gets or sets the distance of the object to max, often used by skybox

#### Returns

`boolean`

#### Inherited from

AbstractMesh.infiniteDistance

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

AbstractMesh.infiniteDistance

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:125

___

### isAnInstance

• `get` **isAnInstance**(): `boolean`

Gets a boolean indicating if this mesh is an instance or a regular mesh

#### Returns

`boolean`

#### Overrides

AbstractMesh.isAnInstance

#### Defined in

https://github.com/babylon.js/core/src/Meshes/instancedMesh.ts:395

___

### isBlocked

• `get` **isBlocked**(): `boolean`

Returns true if the mesh is blocked. Implemented by child classes

#### Returns

`boolean`

#### Inherited from

AbstractMesh.isBlocked

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

#### Inherited from

AbstractMesh.isFacetDataEnabled

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:282

___

### isWorldMatrixFrozen

• `get` **isWorldMatrixFrozen**(): `boolean`

True if the World matrix has been frozen.

#### Returns

`boolean`

#### Inherited from

AbstractMesh.isWorldMatrixFrozen

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

#### Inherited from

AbstractMesh.layerMask

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:619

• `set` **layerMask**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

AbstractMesh.layerMask

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:623

___

### lightSources

• `get` **lightSources**(): [`Light`](Light.md)[]

Gets the list of lights affecting that mesh

#### Returns

[`Light`](Light.md)[]

#### Overrides

AbstractMesh.lightSources

#### Defined in

https://github.com/babylon.js/core/src/Meshes/instancedMesh.ts:85

___

### material

• `get` **material**(): [`Nullable`](../modules.md#nullable)[`Material`](Material.md)

The material of the source mesh

#### Returns

[`Nullable`](../modules.md#nullable)[`Material`](Material.md)

#### Overrides

AbstractMesh.material

#### Defined in

https://github.com/babylon.js/core/src/Meshes/instancedMesh.ts:112

___

### morphTargetManager

• `get` **morphTargetManager**(): [`Nullable`](../modules.md#nullable)[`MorphTargetManager`](MorphTargetManager.md)

Gets or sets the morph target manager

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_morphtargets

#### Returns

[`Nullable`](../modules.md#nullable)[`MorphTargetManager`](MorphTargetManager.md)

#### Inherited from

AbstractMesh.morphTargetManager

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:290

• `set` **morphTargetManager**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`MorphTargetManager`](MorphTargetManager.md) |

#### Returns

`void`

#### Inherited from

AbstractMesh.morphTargetManager

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

#### Inherited from

AbstractMesh.mustDepthSortFacets

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:251

• `set` **mustDepthSortFacets**(`sort`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `sort` | `boolean` |

#### Returns

`void`

#### Inherited from

AbstractMesh.mustDepthSortFacets

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:254

___

### nonUniformScaling

• `get` **nonUniformScaling**(): `boolean`

True if the scaling property of this object is non uniform eg. (1,2,1)

#### Returns

`boolean`

#### Inherited from

AbstractMesh.nonUniformScaling

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:799

___

### numBoneInfluencers

• `get` **numBoneInfluencers**(): `number`

Gets or sets the number of allowed bone influences per vertex (4 by default)

#### Returns

`number`

#### Inherited from

AbstractMesh.numBoneInfluencers

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:576

• `set` **numBoneInfluencers**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

AbstractMesh.numBoneInfluencers

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:579

___

### onClonedObservable

• `get` **onClonedObservable**(): [`Observable`](Observable.md)[`Node`](Node.md)

An event triggered when the node is cloned

#### Returns

[`Observable`](Observable.md)[`Node`](Node.md)

#### Inherited from

AbstractMesh.onClonedObservable

#### Defined in

https://github.com/babylon.js/core/src/node.ts:323

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

AbstractMesh.onCollide

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:341

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

AbstractMesh.onCollisionPositionChange

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:354

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

AbstractMesh.onDispose

#### Defined in

https://github.com/babylon.js/core/src/node.ts:306

___

### onEnabledStateChangedObservable

• `get` **onEnabledStateChangedObservable**(): [`Observable`](Observable.md)`boolean`

An event triggered when the enabled state of the node changes

#### Returns

[`Observable`](Observable.md)`boolean`

#### Inherited from

AbstractMesh.onEnabledStateChangedObservable

#### Defined in

https://github.com/babylon.js/core/src/node.ts:316

___

### parent

• `get` **parent**(): [`Nullable`](../modules.md#nullable)[`Node`](Node.md)

#### Returns

[`Nullable`](../modules.md#nullable)[`Node`](Node.md)

#### Inherited from

AbstractMesh.parent

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

AbstractMesh.parent

#### Defined in

https://github.com/babylon.js/core/src/node.ts:200

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

AbstractMesh.partitioningBBoxRatio

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:238

• `set` **partitioningBBoxRatio**(`ratio`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `ratio` | `number` |

#### Returns

`void`

#### Inherited from

AbstractMesh.partitioningBBoxRatio

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:241

___

### partitioningSubdivisions

• `get` **partitioningSubdivisions**(): `number`

Gets or set the number (integer) of subdivisions per axis in the partitioning space

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_facetdata#tweaking-the-partitioning

#### Returns

`number`

#### Inherited from

AbstractMesh.partitioningSubdivisions

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:227

• `set` **partitioningSubdivisions**(`nb`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `nb` | `number` |

#### Returns

`void`

#### Inherited from

AbstractMesh.partitioningSubdivisions

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:230

___

### position

• `get` **position**(): [`Vector3`](Vector3.md)

Gets or set the node position (default is (0.0, 0.0, 0.0))

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

AbstractMesh.position

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:190

• `set` **position**(`newPosition`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `newPosition` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Inherited from

AbstractMesh.position

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:194

___

### preserveParentRotationForBillboard

• `get` **preserveParentRotationForBillboard**(): `boolean`

Gets or sets a boolean indicating that parent rotation should be preserved when using billboards.
This could be useful for glTF objects where parent rotation helps converting from right handed to left handed

#### Returns

`boolean`

#### Inherited from

AbstractMesh.preserveParentRotationForBillboard

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:98

• `set` **preserveParentRotationForBillboard**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

AbstractMesh.preserveParentRotationForBillboard

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:102

___

### receiveShadows

• `get` **receiveShadows**(): `boolean`

If the source mesh receives shadows

#### Returns

`boolean`

#### Overrides

AbstractMesh.receiveShadows

#### Defined in

https://github.com/babylon.js/core/src/Meshes/instancedMesh.ts:105

___

### renderingGroupId

• `get` **renderingGroupId**(): `number`

Rendering ground id of the source mesh

#### Returns

`number`

#### Overrides

AbstractMesh.renderingGroupId

#### Defined in

https://github.com/babylon.js/core/src/Meshes/instancedMesh.ts:133

• `set` **renderingGroupId**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Overrides

AbstractMesh.renderingGroupId

#### Defined in

https://github.com/babylon.js/core/src/Meshes/instancedMesh.ts:137

___

### right

• `get` **right**(): [`Vector3`](Vector3.md)

The right direction of that transform in world space.

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

AbstractMesh.right

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:269

___

### rotation

• `get` **rotation**(): [`Vector3`](Vector3.md)

Gets or sets the rotation property : a Vector3 defining the rotation value in radians around each local axis X, Y, Z  (default is (0.0, 0.0, 0.0)).
If rotation quaternion is set, this Vector3 will be ignored and copy from the quaternion

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

AbstractMesh.rotation

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:211

• `set` **rotation**(`newRotation`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `newRotation` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Inherited from

AbstractMesh.rotation

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:215

___

### rotationQuaternion

• `get` **rotationQuaternion**(): [`Nullable`](../modules.md#nullable)[`Quaternion`](Quaternion.md)

Gets or sets the rotation Quaternion property : this a Quaternion object defining the node rotation by using a unit quaternion (undefined by default, but can be null).
If set, only the rotationQuaternion is then used to compute the node rotation (ie. node.rotation will be ignored)

#### Returns

[`Nullable`](../modules.md#nullable)[`Quaternion`](Quaternion.md)

#### Inherited from

AbstractMesh.rotationQuaternion

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:237

• `set` **rotationQuaternion**(`quaternion`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `quaternion` | [`Nullable`](../modules.md#nullable)[`Quaternion`](Quaternion.md) |

#### Returns

`void`

#### Inherited from

AbstractMesh.rotationQuaternion

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:241

___

### scaling

• `get` **scaling**(): [`Vector3`](Vector3.md)

Gets or sets the scaling property : a Vector3 defining the node scaling along each local axis X, Y, Z (default is (1.0, 1.0, 1.0)).

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

AbstractMesh.scaling

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:224

• `set` **scaling**(`newScaling`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `newScaling` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Inherited from

AbstractMesh.scaling

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:228

___

### skeleton

• `get` **skeleton**(): [`Nullable`](../modules.md#nullable)[`Skeleton`](Skeleton.md)

Skeleton of the source mesh

#### Returns

[`Nullable`](../modules.md#nullable)[`Skeleton`](Skeleton.md)

#### Overrides

AbstractMesh.skeleton

#### Defined in

https://github.com/babylon.js/core/src/Meshes/instancedMesh.ts:126

___

### sourceMesh

• `get` **sourceMesh**(): [`Mesh`](Mesh.md)

The source mesh of the instance

#### Returns

[`Mesh`](Mesh.md)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/instancedMesh.ts:164

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

AbstractMesh.surroundingMeshes

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:705

• `set` **surroundingMeshes**(`meshes`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `meshes` | [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)[] |

#### Returns

`void`

#### Inherited from

AbstractMesh.surroundingMeshes

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:709

___

### up

• `get` **up**(): [`Vector3`](Vector3.md)

The up direction of that transform in world space.

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

AbstractMesh.up

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:261

___

### useBones

• `get` **useBones**(): `boolean`

Gets a boolean indicating if this mesh has skinning data and an attached skeleton

#### Returns

`boolean`

#### Inherited from

AbstractMesh.useBones

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:1258

___

### useVertexColors

• `get` **useVertexColors**(): `boolean`

Gets or sets a boolean indicating that this mesh needs to use vertex color data to render (if this kind of vertex data is available in the geometry)

#### Returns

`boolean`

#### Inherited from

AbstractMesh.useVertexColors

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:548

• `set` **useVertexColors**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

AbstractMesh.useVertexColors

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:551

___

### visibility

• `get` **visibility**(): `number`

Visibility of the source mesh

#### Returns

`number`

#### Overrides

AbstractMesh.visibility

#### Defined in

https://github.com/babylon.js/core/src/Meshes/instancedMesh.ts:119

___

### worldMatrixFromCache

• `get` **worldMatrixFromCache**(): [`Matrix`](Matrix.md)

Returns directly the latest state of the mesh World matrix.
A Matrix is returned.

#### Returns

[`Matrix`](Matrix.md)

#### Inherited from

AbstractMesh.worldMatrixFromCache

#### Defined in

https://github.com/babylon.js/core/src/node.ts:454

___

### BILLBOARDMODE\_ALL

• `Static` `get` **BILLBOARDMODE_ALL**(): `number`

Billboard on all axes

#### Returns

`number`

#### Inherited from

AbstractMesh.BILLBOARDMODE\_ALL

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:188

___

### BILLBOARDMODE\_NONE

• `Static` `get` **BILLBOARDMODE_NONE**(): `number`

No billboard

#### Returns

`number`

#### Inherited from

AbstractMesh.BILLBOARDMODE\_NONE

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:168

___

### BILLBOARDMODE\_USE\_POSITION

• `Static` `get` **BILLBOARDMODE_USE_POSITION**(): `number`

Billboard on using position instead of orientation

#### Returns

`number`

#### Inherited from

AbstractMesh.BILLBOARDMODE\_USE\_POSITION

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:193

___

### BILLBOARDMODE\_X

• `Static` `get` **BILLBOARDMODE_X**(): `number`

Billboard on X axis

#### Returns

`number`

#### Inherited from

AbstractMesh.BILLBOARDMODE\_X

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:173

___

### BILLBOARDMODE\_Y

• `Static` `get` **BILLBOARDMODE_Y**(): `number`

Billboard on Y axis

#### Returns

`number`

#### Inherited from

AbstractMesh.BILLBOARDMODE\_Y

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:178

___

### BILLBOARDMODE\_Z

• `Static` `get` **BILLBOARDMODE_Z**(): `number`

Billboard on Z axis

#### Returns

`number`

#### Inherited from

AbstractMesh.BILLBOARDMODE\_Z

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:183

## Methods

### \_buildUniformLayout

▸ `Protected` **_buildUniformLayout**(): `void`

#### Returns

`void`

#### Inherited from

[AbstractMesh](AbstractMesh.md).[_buildUniformLayout](AbstractMesh.md#_builduniformlayout)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:834

___

### \_removeLightSource

▸ **_removeLightSource**(): `void`

#### Returns

`void`

#### Overrides

AbstractMesh.\_removeLightSource

#### Defined in

https://github.com/babylon.js/core/src/Meshes/instancedMesh.ts:97

___

### \_resyncLightSource

▸ **_resyncLightSource**(): `void`

#### Returns

`void`

#### Overrides

AbstractMesh.\_resyncLightSource

#### Defined in

https://github.com/babylon.js/core/src/Meshes/instancedMesh.ts:93

___

### \_resyncLightSources

▸ **_resyncLightSources**(): `void`

#### Returns

`void`

#### Overrides

AbstractMesh.\_resyncLightSources

#### Defined in

https://github.com/babylon.js/core/src/Meshes/instancedMesh.ts:89

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

[AbstractMesh](AbstractMesh.md).[addBehavior](AbstractMesh.md#addbehavior)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:366

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

[AbstractMesh](AbstractMesh.md).[addChild](AbstractMesh.md#addchild)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:2141

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

[AbstractMesh](AbstractMesh.md).[addRotation](AbstractMesh.md#addrotation)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:973

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

[AbstractMesh](AbstractMesh.md).[alignWithNormal](AbstractMesh.md#alignwithnormal)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:2557

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

[AbstractMesh](AbstractMesh.md).[applyImpulse](AbstractMesh.md#applyimpulse)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsEngineComponent.ts:184

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

[AbstractMesh](AbstractMesh.md).[attachToBone](AbstractMesh.md#attachtobone)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:822

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

[AbstractMesh](AbstractMesh.md).[beginAnimation](AbstractMesh.md#beginanimation)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:833

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

[AbstractMesh](AbstractMesh.md).[buildBoundingInfo](AbstractMesh.md#buildboundinginfo)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:1241

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

[AbstractMesh](AbstractMesh.md).[calcMovePOV](AbstractMesh.md#calcmovepov)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:1370

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

[AbstractMesh](AbstractMesh.md).[calcRotatePOV](AbstractMesh.md#calcrotatepov)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:1402

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

#### Overrides

[AbstractMesh](AbstractMesh.md).[clone](AbstractMesh.md#clone)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/instancedMesh.ts:465

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

[AbstractMesh](AbstractMesh.md).[computeWorldMatrix](AbstractMesh.md#computeworldmatrix)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:1002

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

[AbstractMesh](AbstractMesh.md).[createAnimationRange](AbstractMesh.md#createanimationrange)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:777

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

#### Defined in

https://github.com/babylon.js/core/src/Meshes/instancedMesh.ts:174

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

[AbstractMesh](AbstractMesh.md).[createNormals](AbstractMesh.md#createnormals)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:2535

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

[AbstractMesh](AbstractMesh.md).[createOrUpdateSubmeshesOctree](AbstractMesh.md#createorupdatesubmeshesoctree)

#### Defined in

https://github.com/babylon.js/core/src/Culling/Octrees/octreeSceneComponent.ts:83

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

[AbstractMesh](AbstractMesh.md).[deleteAnimationRange](AbstractMesh.md#deleteanimationrange)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:794

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

[AbstractMesh](AbstractMesh.md).[detachFromBone](AbstractMesh.md#detachfrombone)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:840

___

### disableEdgesRendering

▸ **disableEdgesRendering**(): [`AbstractMesh`](AbstractMesh.md)

Disables the mesh edge rendering mode

#### Returns

[`AbstractMesh`](AbstractMesh.md)

the currentAbstractMesh

#### Inherited from

[AbstractMesh](AbstractMesh.md).[disableEdgesRendering](AbstractMesh.md#disableedgesrendering)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:2585

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

[AbstractMesh](AbstractMesh.md).[disableFacetData](AbstractMesh.md#disablefacetdata)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:2505

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

#### Overrides

[AbstractMesh](AbstractMesh.md).[dispose](AbstractMesh.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/instancedMesh.ts:539

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

#### Inherited from

[AbstractMesh](AbstractMesh.md).[enableEdgesRendering](AbstractMesh.md#enableedgesrendering)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:2599

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

[AbstractMesh](AbstractMesh.md).[freezeWorldMatrix](AbstractMesh.md#freezeworldmatrix)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:442

___

### getAbsolutePivotPoint

▸ **getAbsolutePivotPoint**(): [`Vector3`](Vector3.md)

Returns a new Vector3 set with the mesh pivot point World coordinates.

#### Returns

[`Vector3`](Vector3.md)

a new Vector3 set with the mesh pivot point World coordinates.

#### Inherited from

[AbstractMesh](AbstractMesh.md).[getAbsolutePivotPoint](AbstractMesh.md#getabsolutepivotpoint)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:707

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

[AbstractMesh](AbstractMesh.md).[getAbsolutePivotPointToRef](AbstractMesh.md#getabsolutepivotpointtoref)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:718

___

### getAbsolutePosition

▸ **getAbsolutePosition**(): [`Vector3`](Vector3.md)

Returns the mesh absolute position in the World.

#### Returns

[`Vector3`](Vector3.md)

a Vector3.

#### Inherited from

[AbstractMesh](AbstractMesh.md).[getAbsolutePosition](AbstractMesh.md#getabsoluteposition)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:484

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

[AbstractMesh](AbstractMesh.md).[getAnimationByName](AbstractMesh.md#getanimationbyname)

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

[AbstractMesh](AbstractMesh.md).[getAnimationRange](AbstractMesh.md#getanimationrange)

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

[AbstractMesh](AbstractMesh.md).[getAnimationRanges](AbstractMesh.md#getanimationranges)

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

[AbstractMesh](AbstractMesh.md).[getBehaviorByName](AbstractMesh.md#getbehaviorbyname)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:420

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

[AbstractMesh](AbstractMesh.md).[getBoundingInfo](AbstractMesh.md#getboundinginfo)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:1203

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

[AbstractMesh](AbstractMesh.md).[getChildMeshes](AbstractMesh.md#getchildmeshes)

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

[AbstractMesh](AbstractMesh.md).[getChildMeshes](AbstractMesh.md#getchildmeshes)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:692

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

[AbstractMesh](AbstractMesh.md).[getChildTransformNodes](AbstractMesh.md#getchildtransformnodes)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:1414

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

[AbstractMesh](AbstractMesh.md).[getChildren](AbstractMesh.md#getchildren)

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

[AbstractMesh](AbstractMesh.md).[getChildren](AbstractMesh.md#getchildren)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:722

___

### getClassName

▸ **getClassName**(): `string`

Returns the string "InstancedMesh".

#### Returns

`string`

#### Overrides

[AbstractMesh](AbstractMesh.md).[getClassName](AbstractMesh.md#getclassname)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/instancedMesh.ts:80

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

[AbstractMesh](AbstractMesh.md).[getClosestFacetAtCoordinates](AbstractMesh.md#getclosestfacetatcoordinates)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:2409

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

[AbstractMesh](AbstractMesh.md).[getClosestFacetAtLocalCoordinates](AbstractMesh.md#getclosestfacetatlocalcoordinates)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:2434

___

### getConnectedParticleSystems

▸ **getConnectedParticleSystems**(): [`IParticleSystem`](../interfaces/IParticleSystem.md)[]

This function returns all of the particle systems in the scene that use the mesh as an emitter.

#### Returns

[`IParticleSystem`](../interfaces/IParticleSystem.md)[]

an array of particle systems in the scene that use the mesh as an emitter

#### Inherited from

[AbstractMesh](AbstractMesh.md).[getConnectedParticleSystems](AbstractMesh.md#getconnectedparticlesystems)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:2607

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

[AbstractMesh](AbstractMesh.md).[getDescendants](AbstractMesh.md#getdescendants)

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

[AbstractMesh](AbstractMesh.md).[getDescendants](AbstractMesh.md#getdescendants)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:662

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

[AbstractMesh](AbstractMesh.md).[getDirection](AbstractMesh.md#getdirection)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:616

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

[AbstractMesh](AbstractMesh.md).[getDirectionToRef](AbstractMesh.md#getdirectiontoref)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:632

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

[AbstractMesh](AbstractMesh.md).[getDistanceToCamera](AbstractMesh.md#getdistancetocamera)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:1316

___

### getEngine

▸ **getEngine**(): [`Engine`](Engine.md)

Gets the engine of the node

#### Returns

[`Engine`](Engine.md)

a Engine

#### Inherited from

[AbstractMesh](AbstractMesh.md).[getEngine](AbstractMesh.md#getengine)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:352

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

[AbstractMesh](AbstractMesh.md).[getFacetDataParameters](AbstractMesh.md#getfacetdataparameters)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:2496

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

[AbstractMesh](AbstractMesh.md).[getFacetLocalNormals](AbstractMesh.md#getfacetlocalnormals)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:2288

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

[AbstractMesh](AbstractMesh.md).[getFacetLocalPartitioning](AbstractMesh.md#getfacetlocalpartitioning)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:2315

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

[AbstractMesh](AbstractMesh.md).[getFacetLocalPositions](AbstractMesh.md#getfacetlocalpositions)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:2302

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

[AbstractMesh](AbstractMesh.md).[getFacetNormal](AbstractMesh.md#getfacetnormal)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:2358

___

### getFacetNormalToRef

▸ **getFacetNormalToRef**(`i`, `ref`): [`InstancedMesh`](InstancedMesh.md)

Sets the reference Vector3 with the i-th facet normal in the world system

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_facetdata

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `i` | `number` | defines the facet index |
| `ref` | [`Vector3`](Vector3.md) | defines the target vector |

#### Returns

[`InstancedMesh`](InstancedMesh.md)

the current mesh

#### Inherited from

[AbstractMesh](AbstractMesh.md).[getFacetNormalToRef](AbstractMesh.md#getfacetnormaltoref)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:2371

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

[AbstractMesh](AbstractMesh.md).[getFacetPosition](AbstractMesh.md#getfacetposition)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:2331

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

[AbstractMesh](AbstractMesh.md).[getFacetPositionToRef](AbstractMesh.md#getfacetpositiontoref)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:2344

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

[AbstractMesh](AbstractMesh.md).[getFacetsAtLocalCoordinates](AbstractMesh.md#getfacetsatlocalcoordinates)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:2385

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

[AbstractMesh](AbstractMesh.md).[getHierarchyBoundingVectors](AbstractMesh.md#gethierarchyboundingvectors)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:933

___

### getIndices

▸ **getIndices**(): [`Nullable`](../modules.md#nullable)[`IndicesArray`](../modules.md#indicesarray)

Returns an array of indices (IndicesArray).

#### Returns

[`Nullable`](../modules.md#nullable)[`IndicesArray`](../modules.md#indicesarray)

#### Overrides

[AbstractMesh](AbstractMesh.md).[getIndices](AbstractMesh.md#getindices)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/instancedMesh.ts:295

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

#### Overrides

[AbstractMesh](AbstractMesh.md).[getLOD](AbstractMesh.md#getlod)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/instancedMesh.ts:403

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

[AbstractMesh](AbstractMesh.md).[getMaterialForRenderPass](AbstractMesh.md#getmaterialforrenderpass)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:490

___

### getMeshUniformBuffer

▸ **getMeshUniformBuffer**(): [`UniformBuffer`](UniformBuffer.md)

Gets the mesh uniform buffer.

#### Returns

[`UniformBuffer`](UniformBuffer.md)

the uniform buffer of the mesh.

#### Inherited from

[AbstractMesh](AbstractMesh.md).[getMeshUniformBuffer](AbstractMesh.md#getmeshuniformbuffer)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:857

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

[AbstractMesh](AbstractMesh.md).[getNormalsData](AbstractMesh.md#getnormalsdata)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:1544

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

[AbstractMesh](AbstractMesh.md).[getPhysicsImpostor](AbstractMesh.md#getphysicsimpostor)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsEngineComponent.ts:176

___

### getPivotMatrix

▸ **getPivotMatrix**(): [`Matrix`](Matrix.md)

Returns the mesh pivot matrix.
Default : Identity.

#### Returns

[`Matrix`](Matrix.md)

the matrix

#### Inherited from

[AbstractMesh](AbstractMesh.md).[getPivotMatrix](AbstractMesh.md#getpivotmatrix)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:404

___

### getPivotPoint

▸ **getPivotPoint**(): [`Vector3`](Vector3.md)

Returns a new Vector3 set with the mesh pivot point coordinates in the local space.

#### Returns

[`Vector3`](Vector3.md)

the pivot point

#### Inherited from

[AbstractMesh](AbstractMesh.md).[getPivotPoint](AbstractMesh.md#getpivotpoint)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:685

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

[AbstractMesh](AbstractMesh.md).[getPivotPointToRef](AbstractMesh.md#getpivotpointtoref)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:696

___

### getPoseMatrix

▸ **getPoseMatrix**(): [`Matrix`](Matrix.md)

Returns the mesh Pose matrix.

#### Returns

[`Matrix`](Matrix.md)

the pose matrix

#### Inherited from

[AbstractMesh](AbstractMesh.md).[getPoseMatrix](AbstractMesh.md#getposematrix)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:292

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

[AbstractMesh](AbstractMesh.md).[getPositionData](AbstractMesh.md#getpositiondata)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:1555

___

### getPositionExpressedInLocalSpace

▸ **getPositionExpressedInLocalSpace**(): [`Vector3`](Vector3.md)

Returns the mesh position in the local space from the current World matrix values.

#### Returns

[`Vector3`](Vector3.md)

a new Vector3.

#### Inherited from

[AbstractMesh](AbstractMesh.md).[getPositionExpressedInLocalSpace](AbstractMesh.md#getpositionexpressedinlocalspace)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:542

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

[AbstractMesh](AbstractMesh.md).[getPositionInCameraSpace](AbstractMesh.md#getpositionincameraspace)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:1303

___

### getScene

▸ **getScene**(): [`Scene`](Scene.md)

Gets the scene of the node

#### Returns

[`Scene`](Scene.md)

a scene

#### Inherited from

[AbstractMesh](AbstractMesh.md).[getScene](AbstractMesh.md#getscene)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:344

___

### getTotalIndices

▸ **getTotalIndices**(): `number`

Returns a positive integer : the total number of indices in this mesh geometry.

#### Returns

`number`

the number of indices or zero if the mesh has no geometry.

#### Overrides

[AbstractMesh](AbstractMesh.md).[getTotalIndices](AbstractMesh.md#gettotalindices)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/instancedMesh.ts:157

___

### getTotalVertices

▸ **getTotalVertices**(): `number`

Returns the total number of vertices (integer).

#### Returns

`number`

#### Overrides

[AbstractMesh](AbstractMesh.md).[getTotalVertices](AbstractMesh.md#gettotalvertices)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/instancedMesh.ts:149

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

#### Overrides

[AbstractMesh](AbstractMesh.md).[getVerticesData](AbstractMesh.md#getverticesdata)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/instancedMesh.ts:193

___

### getWorldMatrix

▸ **getWorldMatrix**(): [`Matrix`](Matrix.md)

Gets the current world matrix

#### Returns

[`Matrix`](Matrix.md)

a Matrix

#### Overrides

[AbstractMesh](AbstractMesh.md).[getWorldMatrix](AbstractMesh.md#getworldmatrix)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/instancedMesh.ts:377

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

[AbstractMesh](AbstractMesh.md).[instantiateHierarchy](AbstractMesh.md#instantiatehierarchy)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:416

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

[AbstractMesh](AbstractMesh.md).[intersects](AbstractMesh.md#intersects)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:1854

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

[AbstractMesh](AbstractMesh.md).[intersectsMesh](AbstractMesh.md#intersectsmesh)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:1652

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

[AbstractMesh](AbstractMesh.md).[intersectsPoint](AbstractMesh.md#intersectspoint)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:1676

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

[AbstractMesh](AbstractMesh.md).[isCompletelyInFrustum](AbstractMesh.md#iscompletelyinfrustum)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:1641

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

[AbstractMesh](AbstractMesh.md).[isDescendantOf](AbstractMesh.md#isdescendantof)

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

[AbstractMesh](AbstractMesh.md).[isDisposed](AbstractMesh.md#isdisposed)

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

[AbstractMesh](AbstractMesh.md).[isEnabled](AbstractMesh.md#isenabled)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:569

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

[AbstractMesh](AbstractMesh.md).[isInFrustum](AbstractMesh.md#isinfrustum)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:1631

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

#### Overrides

[AbstractMesh](AbstractMesh.md).[isReady](AbstractMesh.md#isready)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/instancedMesh.ts:183

___

### isUsingPivotMatrix

▸ **isUsingPivotMatrix**(): `boolean`

return true if a pivot has been set

#### Returns

`boolean`

true if a pivot matrix is used

#### Inherited from

[AbstractMesh](AbstractMesh.md).[isUsingPivotMatrix](AbstractMesh.md#isusingpivotmatrix)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:203

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

#### Overrides

[AbstractMesh](AbstractMesh.md).[isVerticesDataPresent](AbstractMesh.md#isverticesdatapresent)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/instancedMesh.ts:288

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

[AbstractMesh](AbstractMesh.md).[locallyTranslate](AbstractMesh.md#locallytranslate)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:554

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

[AbstractMesh](AbstractMesh.md).[lookAt](AbstractMesh.md#lookat)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:571

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

[AbstractMesh](AbstractMesh.md).[markAsDirty](AbstractMesh.md#markasdirty)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:1049

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

[AbstractMesh](AbstractMesh.md).[movePOV](AbstractMesh.md#movepov)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:1356

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

[AbstractMesh](AbstractMesh.md).[moveWithCollisions](AbstractMesh.md#movewithcollisions)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:1708

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

[AbstractMesh](AbstractMesh.md).[normalizeToUnitCube](AbstractMesh.md#normalizetounitcube)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:1253

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

#### Overrides

[AbstractMesh](AbstractMesh.md).[refreshBoundingInfo](AbstractMesh.md#refreshboundinginfo)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/instancedMesh.ts:310

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

[AbstractMesh](AbstractMesh.md).[registerAfterWorldMatrixUpdate](AbstractMesh.md#registerafterworldmatrixupdate)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:1283

___

### releaseSubMeshes

▸ **releaseSubMeshes**(): [`AbstractMesh`](AbstractMesh.md)

Disposes all the submeshes of the current meshnp

#### Returns

[`AbstractMesh`](AbstractMesh.md)

the current mesh

#### Inherited from

[AbstractMesh](AbstractMesh.md).[releaseSubMeshes](AbstractMesh.md#releasesubmeshes)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:1987

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

[AbstractMesh](AbstractMesh.md).[removeBehavior](AbstractMesh.md#removebehavior)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:393

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

[AbstractMesh](AbstractMesh.md).[removeChild](AbstractMesh.md#removechild)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:2152

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

[AbstractMesh](AbstractMesh.md).[resetDrawCache](AbstractMesh.md#resetdrawcache)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:1059

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

[AbstractMesh](AbstractMesh.md).[resetLocalMatrix](AbstractMesh.md#resetlocalmatrix)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:1244

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

[AbstractMesh](AbstractMesh.md).[rotate](AbstractMesh.md#rotate)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:871

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

[AbstractMesh](AbstractMesh.md).[rotateAround](AbstractMesh.md#rotatearound)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:903

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

[AbstractMesh](AbstractMesh.md).[rotatePOV](AbstractMesh.md#rotatepov)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:1389

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

[AbstractMesh](AbstractMesh.md).[serialize](AbstractMesh.md#serialize)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:1360

___

### serializeAnimationRanges

▸ **serializeAnimationRanges**(): `any`

Serialize animation ranges into a JSON compatible object

#### Returns

`any`

serialization object

#### Inherited from

[AbstractMesh](AbstractMesh.md).[serializeAnimationRanges](AbstractMesh.md#serializeanimationranges)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:847

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

[AbstractMesh](AbstractMesh.md).[setAbsolutePosition](AbstractMesh.md#setabsoluteposition)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:494

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

[AbstractMesh](AbstractMesh.md).[setBoundingInfo](AbstractMesh.md#setboundinginfo)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:1222

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

[AbstractMesh](AbstractMesh.md).[setDirection](AbstractMesh.md#setdirection)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:645

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

[AbstractMesh](AbstractMesh.md).[setEnabled](AbstractMesh.md#setenabled)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:596

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

#### Overrides

[AbstractMesh](AbstractMesh.md).[setIndices](AbstractMesh.md#setindices)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/instancedMesh.ts:277

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

[AbstractMesh](AbstractMesh.md).[setMaterialForRenderPass](AbstractMesh.md#setmaterialforrenderpass)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:499

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

[AbstractMesh](AbstractMesh.md).[setParent](AbstractMesh.md#setparent)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:750

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

[AbstractMesh](AbstractMesh.md).[setPhysicsLinkWith](AbstractMesh.md#setphysicslinkwith)

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsEngineComponent.ts:195

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

[AbstractMesh](AbstractMesh.md).[setPivotMatrix](AbstractMesh.md#setpivotmatrix)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:381

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

[AbstractMesh](AbstractMesh.md).[setPivotPoint](AbstractMesh.md#setpivotpoint)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:665

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

[AbstractMesh](AbstractMesh.md).[setPositionWithLocalVector](AbstractMesh.md#setpositionwithlocalvector)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:532

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

[AbstractMesh](AbstractMesh.md).[setPreTransformMatrix](AbstractMesh.md#setpretransformmatrix)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:371

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

#### Overrides

[AbstractMesh](AbstractMesh.md).[setVerticesData](AbstractMesh.md#setverticesdata)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/instancedMesh.ts:226

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

[AbstractMesh](AbstractMesh.md).[toString](AbstractMesh.md#tostring)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:874

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

[AbstractMesh](AbstractMesh.md).[transferToEffect](AbstractMesh.md#transfertoeffect)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:844

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

[AbstractMesh](AbstractMesh.md).[translate](AbstractMesh.md#translate)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:945

___

### unfreezeWorldMatrix

▸ **unfreezeWorldMatrix**(): [`InstancedMesh`](InstancedMesh.md)

Allows back the World matrix computation.

#### Returns

[`InstancedMesh`](InstancedMesh.md)

the TransformNode.

#### Inherited from

[AbstractMesh](AbstractMesh.md).[unfreezeWorldMatrix](AbstractMesh.md#unfreezeworldmatrix)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:467

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

[AbstractMesh](AbstractMesh.md).[unregisterAfterWorldMatrixUpdate](AbstractMesh.md#unregisterafterworldmatrixupdate)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:1293

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

[AbstractMesh](AbstractMesh.md).[updateFacetData](AbstractMesh.md#updatefacetdata)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:2188

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

[AbstractMesh](AbstractMesh.md).[updateIndices](AbstractMesh.md#updateindices)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/abstractMesh.ts:2526

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

[AbstractMesh](AbstractMesh.md).[updatePoseMatrix](AbstractMesh.md#updateposematrix)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:279

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

#### Overrides

[AbstractMesh](AbstractMesh.md).[updateVerticesData](AbstractMesh.md#updateverticesdata)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/instancedMesh.ts:261

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

[AbstractMesh](AbstractMesh.md).[AddNodeConstructor](AbstractMesh.md#addnodeconstructor)

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

[AbstractMesh](AbstractMesh.md).[Construct](AbstractMesh.md#construct)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:75

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

[AbstractMesh](AbstractMesh.md).[Parse](AbstractMesh.md#parse)

#### Defined in

https://github.com/babylon.js/core/src/Meshes/transformNode.ts:1385

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

[AbstractMesh](AbstractMesh.md).[ParseAnimationRanges](AbstractMesh.md#parseanimationranges)

#### Defined in

https://github.com/babylon.js/core/src/node.ts:919
