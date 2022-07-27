[@dev/core](../README.md) / [Exports](../modules.md) / GroundMesh

# Class: GroundMesh

Mesh representing the ground

## Hierarchy

- [`Mesh`](Mesh.md)

  ↳ **`GroundMesh`**

## Table of contents

### Constructors

- [constructor](GroundMesh.md#constructor)

### Properties

- [\_boundingInfo](GroundMesh.md#_boundinginfo)
- [\_boundingInfoIsDirty](GroundMesh.md#_boundinginfoisdirty)
- [\_heightQuads](GroundMesh.md#_heightquads)
- [\_isDirty](GroundMesh.md#_isdirty)
- [\_isWorldMatrixFrozen](GroundMesh.md#_isworldmatrixfrozen)
- [\_parentNode](GroundMesh.md#_parentnode)
- [\_ranges](GroundMesh.md#_ranges)
- [\_scaling](GroundMesh.md#_scaling)
- [actionManager](GroundMesh.md#actionmanager)
- [alphaIndex](GroundMesh.md#alphaindex)
- [alwaysSelectAsActiveMesh](GroundMesh.md#alwaysselectasactivemesh)
- [animations](GroundMesh.md#animations)
- [cullingStrategy](GroundMesh.md#cullingstrategy)
- [definedFacingForward](GroundMesh.md#definedfacingforward)
- [delayLoadState](GroundMesh.md#delayloadstate)
- [delayLoadingFile](GroundMesh.md#delayloadingfile)
- [doNotSyncBoundingInfo](GroundMesh.md#donotsyncboundinginfo)
- [edgesColor](GroundMesh.md#edgescolor)
- [edgesRenderer](GroundMesh.md#edgesrenderer)
- [edgesShareWithInstances](GroundMesh.md#edgessharewithinstances)
- [edgesWidth](GroundMesh.md#edgeswidth)
- [ellipsoid](GroundMesh.md#ellipsoid)
- [ellipsoidOffset](GroundMesh.md#ellipsoidoffset)
- [enablePointerMoveEvents](GroundMesh.md#enablepointermoveevents)
- [forceRenderingWhenOccluded](GroundMesh.md#forcerenderingwhenoccluded)
- [generateOctree](GroundMesh.md#generateoctree)
- [id](GroundMesh.md#id)
- [ignoreCameraMaxZ](GroundMesh.md#ignorecameramaxz)
- [ignoreNonUniformScaling](GroundMesh.md#ignorenonuniformscaling)
- [inspectableCustomProperties](GroundMesh.md#inspectablecustomproperties)
- [instancedBuffers](GroundMesh.md#instancedbuffers)
- [instances](GroundMesh.md#instances)
- [isBlocker](GroundMesh.md#isblocker)
- [isNearGrabbable](GroundMesh.md#isneargrabbable)
- [isNearPickable](GroundMesh.md#isnearpickable)
- [isOccluded](GroundMesh.md#isoccluded)
- [isOcclusionQueryInProgress](GroundMesh.md#isocclusionqueryinprogress)
- [isPickable](GroundMesh.md#ispickable)
- [isVisible](GroundMesh.md#isvisible)
- [metadata](GroundMesh.md#metadata)
- [name](GroundMesh.md#name)
- [occlusionQueryAlgorithmType](GroundMesh.md#occlusionqueryalgorithmtype)
- [occlusionRetryCount](GroundMesh.md#occlusionretrycount)
- [occlusionType](GroundMesh.md#occlusiontype)
- [onAfterWorldMatrixUpdateObservable](GroundMesh.md#onafterworldmatrixupdateobservable)
- [onCollideObservable](GroundMesh.md#oncollideobservable)
- [onCollisionPositionChangeObservable](GroundMesh.md#oncollisionpositionchangeobservable)
- [onDisposeObservable](GroundMesh.md#ondisposeobservable)
- [onLODLevelSelection](GroundMesh.md#onlodlevelselection)
- [onMaterialChangedObservable](GroundMesh.md#onmaterialchangedobservable)
- [onMeshReadyObservable](GroundMesh.md#onmeshreadyobservable)
- [onReady](GroundMesh.md#onready)
- [onRebuildObservable](GroundMesh.md#onrebuildobservable)
- [outlineColor](GroundMesh.md#outlinecolor)
- [outlineWidth](GroundMesh.md#outlinewidth)
- [overlayAlpha](GroundMesh.md#overlayalpha)
- [overlayColor](GroundMesh.md#overlaycolor)
- [overrideMaterialSideOrientation](GroundMesh.md#overridematerialsideorientation)
- [physicsImpostor](GroundMesh.md#physicsimpostor)
- [reIntegrateRotationIntoRotationQuaternion](GroundMesh.md#reintegraterotationintorotationquaternion)
- [renderOutline](GroundMesh.md#renderoutline)
- [renderOverlay](GroundMesh.md#renderoverlay)
- [reservedDataStore](GroundMesh.md#reserveddatastore)
- [scalingDeterminant](GroundMesh.md#scalingdeterminant)
- [showBoundingBox](GroundMesh.md#showboundingbox)
- [showSubMeshesBoundingBox](GroundMesh.md#showsubmeshesboundingbox)
- [state](GroundMesh.md#state)
- [subMeshes](GroundMesh.md#submeshes)
- [thinInstanceCount](GroundMesh.md#thininstancecount)
- [thinInstanceEnablePicking](GroundMesh.md#thininstanceenablepicking)
- [uniqueId](GroundMesh.md#uniqueid)
- [useOctreeForCollisions](GroundMesh.md#useoctreeforcollisions)
- [useOctreeForPicking](GroundMesh.md#useoctreeforpicking)
- [useOctreeForRenderingSelection](GroundMesh.md#useoctreeforrenderingselection)
- [BACKSIDE](GroundMesh.md#backside)
- [BOTTOM](GroundMesh.md#bottom)
- [CAP\_ALL](GroundMesh.md#cap_all)
- [CAP\_END](GroundMesh.md#cap_end)
- [CAP\_START](GroundMesh.md#cap_start)
- [CENTER](GroundMesh.md#center)
- [CULLINGSTRATEGY\_BOUNDINGSPHERE\_ONLY](GroundMesh.md#cullingstrategy_boundingsphere_only)
- [CULLINGSTRATEGY\_OPTIMISTIC\_INCLUSION](GroundMesh.md#cullingstrategy_optimistic_inclusion)
- [CULLINGSTRATEGY\_OPTIMISTIC\_INCLUSION\_THEN\_BSPHERE\_ONLY](GroundMesh.md#cullingstrategy_optimistic_inclusion_then_bsphere_only)
- [CULLINGSTRATEGY\_STANDARD](GroundMesh.md#cullingstrategy_standard)
- [DEFAULTSIDE](GroundMesh.md#defaultside)
- [DOUBLESIDE](GroundMesh.md#doubleside)
- [FLIP\_N\_ROTATE\_ROW](GroundMesh.md#flip_n_rotate_row)
- [FLIP\_N\_ROTATE\_TILE](GroundMesh.md#flip_n_rotate_tile)
- [FLIP\_ROW](GroundMesh.md#flip_row)
- [FLIP\_TILE](GroundMesh.md#flip_tile)
- [FRONTSIDE](GroundMesh.md#frontside)
- [INSTANCEDMESH\_SORT\_TRANSPARENT](GroundMesh.md#instancedmesh_sort_transparent)
- [LEFT](GroundMesh.md#left)
- [NO\_CAP](GroundMesh.md#no_cap)
- [NO\_FLIP](GroundMesh.md#no_flip)
- [OCCLUSION\_ALGORITHM\_TYPE\_ACCURATE](GroundMesh.md#occlusion_algorithm_type_accurate)
- [OCCLUSION\_ALGORITHM\_TYPE\_CONSERVATIVE](GroundMesh.md#occlusion_algorithm_type_conservative)
- [OCCLUSION\_TYPE\_NONE](GroundMesh.md#occlusion_type_none)
- [OCCLUSION\_TYPE\_OPTIMISTIC](GroundMesh.md#occlusion_type_optimistic)
- [OCCLUSION\_TYPE\_STRICT](GroundMesh.md#occlusion_type_strict)
- [RIGHT](GroundMesh.md#right)
- [ROTATE\_ROW](GroundMesh.md#rotate_row)
- [ROTATE\_TILE](GroundMesh.md#rotate_tile)
- [TOP](GroundMesh.md#top)

### Accessors

- [absolutePosition](GroundMesh.md#absoluteposition)
- [absoluteRotationQuaternion](GroundMesh.md#absoluterotationquaternion)
- [absoluteScaling](GroundMesh.md#absolutescaling)
- [animationPropertiesOverride](GroundMesh.md#animationpropertiesoverride)
- [applyFog](GroundMesh.md#applyfog)
- [areNormalsFrozen](GroundMesh.md#arenormalsfrozen)
- [bakedVertexAnimationManager](GroundMesh.md#bakedvertexanimationmanager)
- [behaviors](GroundMesh.md#behaviors)
- [billboardMode](GroundMesh.md#billboardmode)
- [checkCollisions](GroundMesh.md#checkcollisions)
- [cloneMeshMap](GroundMesh.md#clonemeshmap)
- [collider](GroundMesh.md#collider)
- [collisionGroup](GroundMesh.md#collisiongroup)
- [collisionMask](GroundMesh.md#collisionmask)
- [collisionResponse](GroundMesh.md#collisionresponse)
- [collisionRetryCount](GroundMesh.md#collisionretrycount)
- [computeBonesUsingShaders](GroundMesh.md#computebonesusingshaders)
- [doNotSerialize](GroundMesh.md#donotserialize)
- [enableDistantPicking](GroundMesh.md#enabledistantpicking)
- [facetDepthSortFrom](GroundMesh.md#facetdepthsortfrom)
- [facetNb](GroundMesh.md#facetnb)
- [forcedInstanceCount](GroundMesh.md#forcedinstancecount)
- [forward](GroundMesh.md#forward)
- [geometry](GroundMesh.md#geometry)
- [hasBoundingInfo](GroundMesh.md#hasboundinginfo)
- [hasInstances](GroundMesh.md#hasinstances)
- [hasLODLevels](GroundMesh.md#haslodlevels)
- [hasThinInstances](GroundMesh.md#hasthininstances)
- [hasVertexAlpha](GroundMesh.md#hasvertexalpha)
- [infiniteDistance](GroundMesh.md#infinitedistance)
- [isAnInstance](GroundMesh.md#isaninstance)
- [isBlocked](GroundMesh.md#isblocked)
- [isFacetDataEnabled](GroundMesh.md#isfacetdataenabled)
- [isUnIndexed](GroundMesh.md#isunindexed)
- [isWorldMatrixFrozen](GroundMesh.md#isworldmatrixfrozen)
- [layerMask](GroundMesh.md#layermask)
- [lightSources](GroundMesh.md#lightsources)
- [manualUpdateOfPreviousWorldMatrixInstancedBuffer](GroundMesh.md#manualupdateofpreviousworldmatrixinstancedbuffer)
- [manualUpdateOfWorldMatrixInstancedBuffer](GroundMesh.md#manualupdateofworldmatrixinstancedbuffer)
- [material](GroundMesh.md#material)
- [morphTargetManager](GroundMesh.md#morphtargetmanager)
- [mustDepthSortFacets](GroundMesh.md#mustdepthsortfacets)
- [nonUniformScaling](GroundMesh.md#nonuniformscaling)
- [numBoneInfluencers](GroundMesh.md#numboneinfluencers)
- [onAfterRenderObservable](GroundMesh.md#onafterrenderobservable)
- [onBeforeBindObservable](GroundMesh.md#onbeforebindobservable)
- [onBeforeDraw](GroundMesh.md#onbeforedraw)
- [onBeforeDrawObservable](GroundMesh.md#onbeforedrawobservable)
- [onBeforeRenderObservable](GroundMesh.md#onbeforerenderobservable)
- [onBetweenPassObservable](GroundMesh.md#onbetweenpassobservable)
- [onClonedObservable](GroundMesh.md#onclonedobservable)
- [onCollide](GroundMesh.md#oncollide)
- [onCollisionPositionChange](GroundMesh.md#oncollisionpositionchange)
- [onDispose](GroundMesh.md#ondispose)
- [onEnabledStateChangedObservable](GroundMesh.md#onenabledstatechangedobservable)
- [overridenInstanceCount](GroundMesh.md#overrideninstancecount)
- [parent](GroundMesh.md#parent)
- [partitioningBBoxRatio](GroundMesh.md#partitioningbboxratio)
- [partitioningSubdivisions](GroundMesh.md#partitioningsubdivisions)
- [position](GroundMesh.md#position)
- [preserveParentRotationForBillboard](GroundMesh.md#preserveparentrotationforbillboard)
- [previousWorldMatrixInstancedBuffer](GroundMesh.md#previousworldmatrixinstancedbuffer)
- [receiveShadows](GroundMesh.md#receiveshadows)
- [renderingGroupId](GroundMesh.md#renderinggroupid)
- [right](GroundMesh.md#right-1)
- [rotation](GroundMesh.md#rotation)
- [rotationQuaternion](GroundMesh.md#rotationquaternion)
- [scaling](GroundMesh.md#scaling)
- [skeleton](GroundMesh.md#skeleton)
- [source](GroundMesh.md#source)
- [subdivisions](GroundMesh.md#subdivisions)
- [subdivisionsX](GroundMesh.md#subdivisionsx)
- [subdivisionsY](GroundMesh.md#subdivisionsy)
- [surroundingMeshes](GroundMesh.md#surroundingmeshes)
- [up](GroundMesh.md#up)
- [useBones](GroundMesh.md#usebones)
- [useLODScreenCoverage](GroundMesh.md#uselodscreencoverage)
- [useVertexColors](GroundMesh.md#usevertexcolors)
- [visibility](GroundMesh.md#visibility)
- [worldMatrixFromCache](GroundMesh.md#worldmatrixfromcache)
- [worldMatrixInstancedBuffer](GroundMesh.md#worldmatrixinstancedbuffer)
- [BILLBOARDMODE\_ALL](GroundMesh.md#billboardmode_all)
- [BILLBOARDMODE\_NONE](GroundMesh.md#billboardmode_none)
- [BILLBOARDMODE\_USE\_POSITION](GroundMesh.md#billboardmode_use_position)
- [BILLBOARDMODE\_X](GroundMesh.md#billboardmode_x)
- [BILLBOARDMODE\_Y](GroundMesh.md#billboardmode_y)
- [BILLBOARDMODE\_Z](GroundMesh.md#billboardmode_z)

### Methods

- [\_afterComputeWorldMatrix](GroundMesh.md#_aftercomputeworldmatrix)
- [\_buildUniformLayout](GroundMesh.md#_builduniformlayout)
- [\_computeHeightQuads](GroundMesh.md#_computeheightquads)
- [\_getFacetAt](GroundMesh.md#_getfacetat)
- [\_initHeightQuads](GroundMesh.md#_initheightquads)
- [\_invalidateInstanceVertexArrayObject](GroundMesh.md#_invalidateinstancevertexarrayobject)
- [addBehavior](GroundMesh.md#addbehavior)
- [addChild](GroundMesh.md#addchild)
- [addLODLevel](GroundMesh.md#addlodlevel)
- [addRotation](GroundMesh.md#addrotation)
- [alignWithNormal](GroundMesh.md#alignwithnormal)
- [applyDisplacementMap](GroundMesh.md#applydisplacementmap)
- [applyDisplacementMapFromBuffer](GroundMesh.md#applydisplacementmapfrombuffer)
- [applyImpulse](GroundMesh.md#applyimpulse)
- [applySkeleton](GroundMesh.md#applyskeleton)
- [attachToBone](GroundMesh.md#attachtobone)
- [bakeCurrentTransformIntoVertices](GroundMesh.md#bakecurrenttransformintovertices)
- [bakeTransformIntoVertices](GroundMesh.md#baketransformintovertices)
- [beginAnimation](GroundMesh.md#beginanimation)
- [buildBoundingInfo](GroundMesh.md#buildboundinginfo)
- [calcMovePOV](GroundMesh.md#calcmovepov)
- [calcRotatePOV](GroundMesh.md#calcrotatepov)
- [cleanMatrixWeights](GroundMesh.md#cleanmatrixweights)
- [clone](GroundMesh.md#clone)
- [computeWorldMatrix](GroundMesh.md#computeworldmatrix)
- [convertToFlatShadedMesh](GroundMesh.md#converttoflatshadedmesh)
- [convertToUnIndexedMesh](GroundMesh.md#converttounindexedmesh)
- [createAnimationRange](GroundMesh.md#createanimationrange)
- [createInstance](GroundMesh.md#createinstance)
- [createNormals](GroundMesh.md#createnormals)
- [createOrUpdateSubmeshesOctree](GroundMesh.md#createorupdatesubmeshesoctree)
- [deleteAnimationRange](GroundMesh.md#deleteanimationrange)
- [detachFromBone](GroundMesh.md#detachfrombone)
- [disableEdgesRendering](GroundMesh.md#disableedgesrendering)
- [disableFacetData](GroundMesh.md#disablefacetdata)
- [dispose](GroundMesh.md#dispose)
- [enableEdgesRendering](GroundMesh.md#enableedgesrendering)
- [flipFaces](GroundMesh.md#flipfaces)
- [forceSharedVertices](GroundMesh.md#forcesharedvertices)
- [freezeNormals](GroundMesh.md#freezenormals)
- [freezeWorldMatrix](GroundMesh.md#freezeworldmatrix)
- [getAbsolutePivotPoint](GroundMesh.md#getabsolutepivotpoint)
- [getAbsolutePivotPointToRef](GroundMesh.md#getabsolutepivotpointtoref)
- [getAbsolutePosition](GroundMesh.md#getabsoluteposition)
- [getAnimatables](GroundMesh.md#getanimatables)
- [getAnimationByName](GroundMesh.md#getanimationbyname)
- [getAnimationRange](GroundMesh.md#getanimationrange)
- [getAnimationRanges](GroundMesh.md#getanimationranges)
- [getBehaviorByName](GroundMesh.md#getbehaviorbyname)
- [getBoundingInfo](GroundMesh.md#getboundinginfo)
- [getChildMeshes](GroundMesh.md#getchildmeshes)
- [getChildTransformNodes](GroundMesh.md#getchildtransformnodes)
- [getChildren](GroundMesh.md#getchildren)
- [getClassName](GroundMesh.md#getclassname)
- [getClosestFacetAtCoordinates](GroundMesh.md#getclosestfacetatcoordinates)
- [getClosestFacetAtLocalCoordinates](GroundMesh.md#getclosestfacetatlocalcoordinates)
- [getConnectedParticleSystems](GroundMesh.md#getconnectedparticlesystems)
- [getDescendants](GroundMesh.md#getdescendants)
- [getDirection](GroundMesh.md#getdirection)
- [getDirectionToRef](GroundMesh.md#getdirectiontoref)
- [getDistanceToCamera](GroundMesh.md#getdistancetocamera)
- [getEmittedParticleSystems](GroundMesh.md#getemittedparticlesystems)
- [getEngine](GroundMesh.md#getengine)
- [getFacetDataParameters](GroundMesh.md#getfacetdataparameters)
- [getFacetLocalNormals](GroundMesh.md#getfacetlocalnormals)
- [getFacetLocalPartitioning](GroundMesh.md#getfacetlocalpartitioning)
- [getFacetLocalPositions](GroundMesh.md#getfacetlocalpositions)
- [getFacetNormal](GroundMesh.md#getfacetnormal)
- [getFacetNormalToRef](GroundMesh.md#getfacetnormaltoref)
- [getFacetPosition](GroundMesh.md#getfacetposition)
- [getFacetPositionToRef](GroundMesh.md#getfacetpositiontoref)
- [getFacetsAtLocalCoordinates](GroundMesh.md#getfacetsatlocalcoordinates)
- [getHeightAtCoordinates](GroundMesh.md#getheightatcoordinates)
- [getHierarchyBoundingVectors](GroundMesh.md#gethierarchyboundingvectors)
- [getHierarchyEmittedParticleSystems](GroundMesh.md#gethierarchyemittedparticlesystems)
- [getIndices](GroundMesh.md#getindices)
- [getLOD](GroundMesh.md#getlod)
- [getLODLevelAtDistance](GroundMesh.md#getlodlevelatdistance)
- [getLODLevels](GroundMesh.md#getlodlevels)
- [getMaterialForRenderPass](GroundMesh.md#getmaterialforrenderpass)
- [getMeshUniformBuffer](GroundMesh.md#getmeshuniformbuffer)
- [getNormalAtCoordinates](GroundMesh.md#getnormalatcoordinates)
- [getNormalAtCoordinatesToRef](GroundMesh.md#getnormalatcoordinatestoref)
- [getNormalsData](GroundMesh.md#getnormalsdata)
- [getPhysicsImpostor](GroundMesh.md#getphysicsimpostor)
- [getPivotMatrix](GroundMesh.md#getpivotmatrix)
- [getPivotPoint](GroundMesh.md#getpivotpoint)
- [getPivotPointToRef](GroundMesh.md#getpivotpointtoref)
- [getPoseMatrix](GroundMesh.md#getposematrix)
- [getPositionData](GroundMesh.md#getpositiondata)
- [getPositionExpressedInLocalSpace](GroundMesh.md#getpositionexpressedinlocalspace)
- [getPositionInCameraSpace](GroundMesh.md#getpositionincameraspace)
- [getScene](GroundMesh.md#getscene)
- [getTotalIndices](GroundMesh.md#gettotalindices)
- [getTotalVertices](GroundMesh.md#gettotalvertices)
- [getVertexBuffer](GroundMesh.md#getvertexbuffer)
- [getVerticesData](GroundMesh.md#getverticesdata)
- [getVerticesDataKinds](GroundMesh.md#getverticesdatakinds)
- [getWorldMatrix](GroundMesh.md#getworldmatrix)
- [increaseVertices](GroundMesh.md#increasevertices)
- [instantiateHierarchy](GroundMesh.md#instantiatehierarchy)
- [intersects](GroundMesh.md#intersects)
- [intersectsMesh](GroundMesh.md#intersectsmesh)
- [intersectsPoint](GroundMesh.md#intersectspoint)
- [isCompletelyInFrustum](GroundMesh.md#iscompletelyinfrustum)
- [isDescendantOf](GroundMesh.md#isdescendantof)
- [isDisposed](GroundMesh.md#isdisposed)
- [isEnabled](GroundMesh.md#isenabled)
- [isInFrustum](GroundMesh.md#isinfrustum)
- [isReady](GroundMesh.md#isready)
- [isUsingPivotMatrix](GroundMesh.md#isusingpivotmatrix)
- [isVertexBufferUpdatable](GroundMesh.md#isvertexbufferupdatable)
- [isVerticesDataPresent](GroundMesh.md#isverticesdatapresent)
- [locallyTranslate](GroundMesh.md#locallytranslate)
- [lookAt](GroundMesh.md#lookat)
- [makeGeometryUnique](GroundMesh.md#makegeometryunique)
- [markAsDirty](GroundMesh.md#markasdirty)
- [markVerticesDataAsUpdatable](GroundMesh.md#markverticesdataasupdatable)
- [movePOV](GroundMesh.md#movepov)
- [moveWithCollisions](GroundMesh.md#movewithcollisions)
- [normalizeToUnitCube](GroundMesh.md#normalizetounitcube)
- [optimize](GroundMesh.md#optimize)
- [optimizeIndices](GroundMesh.md#optimizeindices)
- [refreshBoundingInfo](GroundMesh.md#refreshboundinginfo)
- [registerAfterRender](GroundMesh.md#registerafterrender)
- [registerAfterWorldMatrixUpdate](GroundMesh.md#registerafterworldmatrixupdate)
- [registerBeforeRender](GroundMesh.md#registerbeforerender)
- [registerInstancedBuffer](GroundMesh.md#registerinstancedbuffer)
- [releaseSubMeshes](GroundMesh.md#releasesubmeshes)
- [removeBehavior](GroundMesh.md#removebehavior)
- [removeChild](GroundMesh.md#removechild)
- [removeLODLevel](GroundMesh.md#removelodlevel)
- [removeVerticesData](GroundMesh.md#removeverticesdata)
- [render](GroundMesh.md#render)
- [resetDrawCache](GroundMesh.md#resetdrawcache)
- [resetLocalMatrix](GroundMesh.md#resetlocalmatrix)
- [rotate](GroundMesh.md#rotate)
- [rotateAround](GroundMesh.md#rotatearound)
- [rotatePOV](GroundMesh.md#rotatepov)
- [serialize](GroundMesh.md#serialize)
- [serializeAnimationRanges](GroundMesh.md#serializeanimationranges)
- [setAbsolutePosition](GroundMesh.md#setabsoluteposition)
- [setBoundingInfo](GroundMesh.md#setboundinginfo)
- [setDirection](GroundMesh.md#setdirection)
- [setEnabled](GroundMesh.md#setenabled)
- [setIndices](GroundMesh.md#setindices)
- [setMaterialById](GroundMesh.md#setmaterialbyid)
- [setMaterialForRenderPass](GroundMesh.md#setmaterialforrenderpass)
- [setNormalsForCPUSkinning](GroundMesh.md#setnormalsforcpuskinning)
- [setParent](GroundMesh.md#setparent)
- [setPhysicsLinkWith](GroundMesh.md#setphysicslinkwith)
- [setPivotMatrix](GroundMesh.md#setpivotmatrix)
- [setPivotPoint](GroundMesh.md#setpivotpoint)
- [setPositionWithLocalVector](GroundMesh.md#setpositionwithlocalvector)
- [setPositionsForCPUSkinning](GroundMesh.md#setpositionsforcpuskinning)
- [setPreTransformMatrix](GroundMesh.md#setpretransformmatrix)
- [setVerticesBuffer](GroundMesh.md#setverticesbuffer)
- [setVerticesData](GroundMesh.md#setverticesdata)
- [simplify](GroundMesh.md#simplify)
- [subdivide](GroundMesh.md#subdivide)
- [synchronizeInstances](GroundMesh.md#synchronizeinstances)
- [thinInstanceAdd](GroundMesh.md#thininstanceadd)
- [thinInstanceAddSelf](GroundMesh.md#thininstanceaddself)
- [thinInstanceBufferUpdated](GroundMesh.md#thininstancebufferupdated)
- [thinInstanceGetWorldMatrices](GroundMesh.md#thininstancegetworldmatrices)
- [thinInstancePartialBufferUpdate](GroundMesh.md#thininstancepartialbufferupdate)
- [thinInstanceRefreshBoundingInfo](GroundMesh.md#thininstancerefreshboundinginfo)
- [thinInstanceRegisterAttribute](GroundMesh.md#thininstanceregisterattribute)
- [thinInstanceSetAttributeAt](GroundMesh.md#thininstancesetattributeat)
- [thinInstanceSetBuffer](GroundMesh.md#thininstancesetbuffer)
- [thinInstanceSetMatrixAt](GroundMesh.md#thininstancesetmatrixat)
- [toLeftHanded](GroundMesh.md#tolefthanded)
- [toString](GroundMesh.md#tostring)
- [transferToEffect](GroundMesh.md#transfertoeffect)
- [translate](GroundMesh.md#translate)
- [unfreezeNormals](GroundMesh.md#unfreezenormals)
- [unfreezeWorldMatrix](GroundMesh.md#unfreezeworldmatrix)
- [unregisterAfterRender](GroundMesh.md#unregisterafterrender)
- [unregisterAfterWorldMatrixUpdate](GroundMesh.md#unregisterafterworldmatrixupdate)
- [unregisterBeforeRender](GroundMesh.md#unregisterbeforerender)
- [updateCoordinateHeights](GroundMesh.md#updatecoordinateheights)
- [updateFacetData](GroundMesh.md#updatefacetdata)
- [updateIndices](GroundMesh.md#updateindices)
- [updateMeshPositions](GroundMesh.md#updatemeshpositions)
- [updatePoseMatrix](GroundMesh.md#updateposematrix)
- [updateVerticesData](GroundMesh.md#updateverticesdata)
- [validateSkinning](GroundMesh.md#validateskinning)
- [AddNodeConstructor](GroundMesh.md#addnodeconstructor)
- [Center](GroundMesh.md#center-1)
- [Construct](GroundMesh.md#construct)
- [MergeMeshes](GroundMesh.md#mergemeshes)
- [MergeMeshesAsync](GroundMesh.md#mergemeshesasync)
- [MinMax](GroundMesh.md#minmax)
- [Parse](GroundMesh.md#parse)
- [ParseAnimationRanges](GroundMesh.md#parseanimationranges)

## Constructors

### constructor

• **new GroundMesh**(`name`, `scene?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `scene?` | [`Scene`](Scene.md) |

#### Overrides

[Mesh](Mesh.md).[constructor](Mesh.md#constructor)

#### Defined in

packages/dev/core/src/Meshes/groundMesh.ts:36

## Properties

### \_boundingInfo

• `Protected` **\_boundingInfo**: [`Nullable`](../modules.md#nullable)[`BoundingInfo`](BoundingInfo.md) = `null`

#### Inherited from

[Mesh](Mesh.md).[_boundingInfo](Mesh.md#_boundinginfo)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:729

___

### \_boundingInfoIsDirty

• `Protected` **\_boundingInfoIsDirty**: `boolean` = `true`

#### Inherited from

[Mesh](Mesh.md).[_boundingInfoIsDirty](Mesh.md#_boundinginfoisdirty)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:730

___

### \_heightQuads

• `Private` **\_heightQuads**: { `facet1`: [`Vector4`](Vector4.md) ; `facet2`: [`Vector4`](Vector4.md) ; `slope`: [`Vector2`](Vector2.md)  }[]

#### Defined in

packages/dev/core/src/Meshes/groundMesh.ts:17

___

### \_isDirty

• `Protected` **\_isDirty**: `boolean` = `false`

#### Inherited from

[Mesh](Mesh.md).[_isDirty](Mesh.md#_isdirty)

#### Defined in

packages/dev/core/src/node.ts:43

___

### \_isWorldMatrixFrozen

• `Protected` **\_isWorldMatrixFrozen**: `boolean` = `false`

#### Inherited from

[Mesh](Mesh.md).[_isWorldMatrixFrozen](Mesh.md#_isworldmatrixfrozen)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:161

___

### \_parentNode

• `Protected` **\_parentNode**: [`Nullable`](../modules.md#nullable)[`Node`](Node.md) = `null`

#### Inherited from

[Mesh](Mesh.md).[_parentNode](Mesh.md#_parentnode)

#### Defined in

packages/dev/core/src/node.ts:176

___

### \_ranges

• `Protected` **\_ranges**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: [`Nullable`](../modules.md#nullable)`AnimationRange`

#### Inherited from

[Mesh](Mesh.md).[_ranges](Mesh.md#_ranges)

#### Defined in

packages/dev/core/src/node.ts:154

___

### \_scaling

• `Protected` **\_scaling**: [`Vector3`](Vector3.md)

#### Inherited from

[Mesh](Mesh.md).[_scaling](Mesh.md#_scaling)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:62

___

### actionManager

• **actionManager**: [`Nullable`](../modules.md#nullable)[`AbstractActionManager`](AbstractActionManager.md) = `null`

Gets or sets the current action manager

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions

#### Inherited from

[Mesh](Mesh.md).[actionManager](Mesh.md#actionmanager)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:646

___

### alphaIndex

• **alphaIndex**: `number` = `Number.MAX_VALUE`

Gets or sets the alpha index used to sort transparent meshes

**`See`**

https://doc.babylonjs.com/resources/transparency_and_how_meshes_are_rendered#alpha-index

#### Inherited from

[Mesh](Mesh.md).[alphaIndex](Mesh.md#alphaindex)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:406

___

### alwaysSelectAsActiveMesh

• **alwaysSelectAsActiveMesh**: `boolean` = `false`

True if the mesh must be rendered in any case (this will shortcut the frustum clipping phase)

#### Inherited from

[Mesh](Mesh.md).[alwaysSelectAsActiveMesh](Mesh.md#alwaysselectasactivemesh)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:635

___

### animations

• **animations**: [`Animation`](Animation.md)[]

Gets a list of Animations associated with the node

#### Inherited from

[Mesh](Mesh.md).[animations](Mesh.md#animations)

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

[Mesh](Mesh.md).[cullingStrategy](Mesh.md#cullingstrategy)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:214

___

### definedFacingForward

• **definedFacingForward**: `boolean` = `true`

Gets or sets the orientation for POV movement & rotation

#### Inherited from

[Mesh](Mesh.md).[definedFacingForward](Mesh.md#definedfacingforward)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:371

___

### delayLoadState

• **delayLoadState**: `number` = `Constants.DELAYLOADSTATE_NONE`

Gets the delay loading state of the mesh (when delay loading is turned on)

**`See`**

https://doc.babylonjs.com/how_to/using_the_incremental_loading_system

#### Inherited from

[Mesh](Mesh.md).[delayLoadState](Mesh.md#delayloadstate)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:372

___

### delayLoadingFile

• **delayLoadingFile**: `string`

Gets the file containing delay loading data for this mesh

#### Inherited from

[Mesh](Mesh.md).[delayLoadingFile](Mesh.md#delayloadingfile)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:385

___

### doNotSyncBoundingInfo

• **doNotSyncBoundingInfo**: `boolean` = `false`

Gets or sets a boolean indicating that the bounding info does not need to be kept in sync (for performance reason)

#### Inherited from

[Mesh](Mesh.md).[doNotSyncBoundingInfo](Mesh.md#donotsyncboundinginfo)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:640

___

### edgesColor

• **edgesColor**: [`Color4`](Color4.md)

Defines edge color used when edgesRenderer is enabled

**`See`**

https://www.babylonjs-playground.com/#10OJSG#13

#### Inherited from

[Mesh](Mesh.md).[edgesColor](Mesh.md#edgescolor)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:723

___

### edgesRenderer

• **edgesRenderer**: [`Nullable`](../modules.md#nullable)[`EdgesRenderer`](EdgesRenderer.md)

Gets the edgesRenderer associated with the mesh

#### Inherited from

[Mesh](Mesh.md).[edgesRenderer](Mesh.md#edgesrenderer)

#### Defined in

packages/dev/core/src/Rendering/edgesRenderer.ts:35

___

### edgesShareWithInstances

• **edgesShareWithInstances**: `boolean`

true to use the edge renderer for all instances of this mesh

#### Inherited from

[Mesh](Mesh.md).[edgesShareWithInstances](Mesh.md#edgessharewithinstances)

#### Defined in

packages/dev/core/src/Meshes/instancedMesh.ts:575

___

### edgesWidth

• **edgesWidth**: `number` = `1`

Defines edge width used when edgesRenderer is enabled

**`See`**

https://www.babylonjs-playground.com/#10OJSG#13

#### Inherited from

[Mesh](Mesh.md).[edgesWidth](Mesh.md#edgeswidth)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:718

___

### ellipsoid

• **ellipsoid**: [`Vector3`](Vector3.md)

Gets or sets the ellipsoid used to impersonate this mesh when using collision engine (default is (0.5, 1, 0.5))

**`See`**

https://doc.babylonjs.com/babylon101/cameras,_mesh_collisions_and_gravity

#### Inherited from

[Mesh](Mesh.md).[ellipsoid](Mesh.md#ellipsoid)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:652

___

### ellipsoidOffset

• **ellipsoidOffset**: [`Vector3`](Vector3.md)

Gets or sets the ellipsoid offset used to impersonate this mesh when using collision engine (default is (0, 0, 0))

**`See`**

https://doc.babylonjs.com/babylon101/cameras,_mesh_collisions_and_gravity

#### Inherited from

[Mesh](Mesh.md).[ellipsoidOffset](Mesh.md#ellipsoidoffset)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:657

___

### enablePointerMoveEvents

• **enablePointerMoveEvents**: `boolean` = `false`

Gets or sets a boolean indicating that pointer move events must be supported on this mesh (false by default)

#### Inherited from

[Mesh](Mesh.md).[enablePointerMoveEvents](Mesh.md#enablepointermoveevents)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:439

___

### forceRenderingWhenOccluded

• **forceRenderingWhenOccluded**: `boolean`

Flag to force rendering the mesh even if occluded

**`See`**

https://doc.babylonjs.com/features/occlusionquery

#### Inherited from

[Mesh](Mesh.md).[forceRenderingWhenOccluded](Mesh.md#forcerenderingwhenoccluded)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.query.ts:405

___

### generateOctree

• **generateOctree**: `boolean` = `false`

If octree should be generated

#### Defined in

packages/dev/core/src/Meshes/groundMesh.ts:15

___

### id

• **id**: `string`

Gets or sets the id of the node

#### Inherited from

[Mesh](Mesh.md).[id](Mesh.md#id)

#### Defined in

packages/dev/core/src/node.ts:97

___

### ignoreCameraMaxZ

• **ignoreCameraMaxZ**: `boolean` = `false`

Gets or sets a boolean indicating whether to render ignoring the active camera's max z setting. (false by default)
Note this will reduce performance when set to true.

#### Inherited from

[Mesh](Mesh.md).[ignoreCameraMaxZ](Mesh.md#ignorecameramaxz)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:442

___

### ignoreNonUniformScaling

• **ignoreNonUniformScaling**: `boolean` = `false`

Gets or sets a boolean indicating that non uniform scaling (when at least one component is different from others) should be ignored.
By default the system will update normals to compensate

#### Inherited from

[Mesh](Mesh.md).[ignoreNonUniformScaling](Mesh.md#ignorenonuniformscaling)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:138

___

### inspectableCustomProperties

• **inspectableCustomProperties**: [`IInspectable`](../interfaces/IInspectable.md)[]

List of inspectable custom properties (used by the Inspector)

**`See`**

https://doc.babylonjs.com/how_to/debug_layer#extensibility

#### Inherited from

[Mesh](Mesh.md).[inspectableCustomProperties](Mesh.md#inspectablecustomproperties)

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

[Mesh](Mesh.md).[instancedBuffers](Mesh.md#instancedbuffers)

#### Defined in

packages/dev/core/src/Meshes/instancedMesh.ts:594

___

### instances

• **instances**: [`InstancedMesh`](InstancedMesh.md)[]

Gets the list of instances created from this mesh
it is not supposed to be modified manually.
Note also that the order of the InstancedMesh wihin the array is not significant and might change.

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_instances

#### Inherited from

[Mesh](Mesh.md).[instances](Mesh.md#instances)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:380

___

### isBlocker

• **isBlocker**: `boolean` = `false`

Gets or sets a boolean indicating if the mesh must be considered as a ray blocker for lens flares (false by default)

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_lens_flares

#### Inherited from

[Mesh](Mesh.md).[isBlocker](Mesh.md#isblocker)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:434

___

### isNearGrabbable

• **isNearGrabbable**: `boolean` = `false`

Gets or sets a boolean indicating if the mesh can be near grabbed. Default is false

#### Inherited from

[Mesh](Mesh.md).[isNearGrabbable](Mesh.md#isneargrabbable)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:426

___

### isNearPickable

• **isNearPickable**: `boolean` = `false`

Gets or sets a boolean indicating if the mesh can be near picked. Default is false

#### Inherited from

[Mesh](Mesh.md).[isNearPickable](Mesh.md#isnearpickable)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:421

___

### isOccluded

• **isOccluded**: `boolean`

Gets or sets whether the mesh is occluded or not, it is used also to set the initial state of the mesh to be occluded or not

**`See`**

https://doc.babylonjs.com/features/occlusionquery

#### Inherited from

[Mesh](Mesh.md).[isOccluded](Mesh.md#isoccluded)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.query.ts:393

___

### isOcclusionQueryInProgress

• **isOcclusionQueryInProgress**: `boolean`

Flag to check the progress status of the query

**`See`**

https://doc.babylonjs.com/features/occlusionquery

#### Inherited from

[Mesh](Mesh.md).[isOcclusionQueryInProgress](Mesh.md#isocclusionqueryinprogress)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.query.ts:399

___

### isPickable

• **isPickable**: `boolean` = `true`

Gets or sets a boolean indicating if the mesh can be picked (by scene.pick for instance or through actions). Default is true

#### Inherited from

[Mesh](Mesh.md).[isPickable](Mesh.md#ispickable)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:416

___

### isVisible

• **isVisible**: `boolean` = `true`

Gets or sets a boolean indicating if the mesh is visible (renderable). Default is true

#### Inherited from

[Mesh](Mesh.md).[isVisible](Mesh.md#isvisible)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:411

___

### metadata

• **metadata**: `any` = `null`

Gets or sets an object used to store user defined information for the node

#### Inherited from

[Mesh](Mesh.md).[metadata](Mesh.md#metadata)

#### Defined in

packages/dev/core/src/node.ts:115

___

### name

• **name**: `string`

Gets or sets the name of the node

#### Inherited from

[Mesh](Mesh.md).[name](Mesh.md#name)

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

[Mesh](Mesh.md).[occlusionQueryAlgorithmType](Mesh.md#occlusionqueryalgorithmtype)

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

[Mesh](Mesh.md).[occlusionRetryCount](Mesh.md#occlusionretrycount)

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

[Mesh](Mesh.md).[occlusionType](Mesh.md#occlusiontype)

#### Defined in

packages/dev/core/src/Engines/Extensions/engine.query.ts:379

___

### onAfterWorldMatrixUpdateObservable

• **onAfterWorldMatrixUpdateObservable**: [`Observable`](Observable.md)[`TransformNode`](TransformNode.md)

An event triggered after the world matrix is updated

#### Inherited from

[Mesh](Mesh.md).[onAfterWorldMatrixUpdateObservable](Mesh.md#onafterworldmatrixupdateobservable)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:169

___

### onCollideObservable

• **onCollideObservable**: [`Observable`](Observable.md)[`AbstractMesh`](AbstractMesh.md)

An event triggered when this mesh collides with another one

#### Inherited from

[Mesh](Mesh.md).[onCollideObservable](Mesh.md#oncollideobservable)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:338

___

### onCollisionPositionChangeObservable

• **onCollisionPositionChangeObservable**: [`Observable`](Observable.md)[`Vector3`](Vector3.md)

An event triggered when the collision's position changes

#### Inherited from

[Mesh](Mesh.md).[onCollisionPositionChangeObservable](Mesh.md#oncollisionpositionchangeobservable)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:351

___

### onDisposeObservable

• **onDisposeObservable**: [`Observable`](Observable.md)[`Node`](Node.md)

An event triggered when the mesh is disposed

#### Inherited from

[Mesh](Mesh.md).[onDisposeObservable](Mesh.md#ondisposeobservable)

#### Defined in

packages/dev/core/src/node.ts:300

___

### onLODLevelSelection

• **onLODLevelSelection**: (`distance`: `number`, `mesh`: [`Mesh`](Mesh.md), `selectedLevel`: [`Nullable`](../modules.md#nullable)[`Mesh`](Mesh.md)) => `void`

#### Type declaration

▸ (`distance`, `mesh`, `selectedLevel`): `void`

User defined function used to change how LOD level selection is done

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_lod

##### Parameters

| Name | Type |
| :------ | :------ |
| `distance` | `number` |
| `mesh` | [`Mesh`](Mesh.md) |
| `selectedLevel` | [`Nullable`](../modules.md#nullable)[`Mesh`](Mesh.md) |

##### Returns

`void`

#### Inherited from

[Mesh](Mesh.md).[onLODLevelSelection](Mesh.md#onlodlevelselection)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:394

___

### onMaterialChangedObservable

• **onMaterialChangedObservable**: [`Observable`](Observable.md)[`AbstractMesh`](AbstractMesh.md)

An event triggered when material is changed

#### Inherited from

[Mesh](Mesh.md).[onMaterialChangedObservable](Mesh.md#onmaterialchangedobservable)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:364

___

### onMeshReadyObservable

• **onMeshReadyObservable**: [`Observable`](Observable.md)[`Mesh`](Mesh.md)

Will notify when the mesh is completely ready, including materials.
Observers added to this observable will be removed once triggered

#### Inherited from

[Mesh](Mesh.md).[onMeshReadyObservable](Mesh.md#onmeshreadyobservable)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:266

___

### onReady

• **onReady**: [`Nullable`](../modules.md#nullable)(`node`: [`Node`](Node.md)) => `void` = `null`

Callback raised when the node is ready to be used

#### Inherited from

[Mesh](Mesh.md).[onReady](Mesh.md#onready)

#### Defined in

packages/dev/core/src/node.ts:159

___

### onRebuildObservable

• **onRebuildObservable**: [`Observable`](Observable.md)[`AbstractMesh`](AbstractMesh.md)

An event triggered when the mesh is rebuilt.

#### Inherited from

[Mesh](Mesh.md).[onRebuildObservable](Mesh.md#onrebuildobservable)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:807

___

### outlineColor

• **outlineColor**: [`Color3`](Color3.md)

Defines color to use when rendering outline

#### Inherited from

[Mesh](Mesh.md).[outlineColor](Mesh.md#outlinecolor)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:524

___

### outlineWidth

• **outlineWidth**: `number` = `0.02`

Define width to use when rendering outline

#### Inherited from

[Mesh](Mesh.md).[outlineWidth](Mesh.md#outlinewidth)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:526

___

### overlayAlpha

• **overlayAlpha**: `number` = `0.5`

Defines alpha to use when rendering overlay

#### Inherited from

[Mesh](Mesh.md).[overlayAlpha](Mesh.md#overlayalpha)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:531

___

### overlayColor

• **overlayColor**: [`Color3`](Color3.md)

Defines color to use when rendering overlay

#### Inherited from

[Mesh](Mesh.md).[overlayColor](Mesh.md#overlaycolor)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:529

___

### overrideMaterialSideOrientation

• **overrideMaterialSideOrientation**: [`Nullable`](../modules.md#nullable)`number` = `null`

Use this property to change the original side orientation defined at construction time

#### Inherited from

[Mesh](Mesh.md).[overrideMaterialSideOrientation](Mesh.md#overridematerialsideorientation)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:436

___

### physicsImpostor

• **physicsImpostor**: [`Nullable`](../modules.md#nullable)[`PhysicsImpostor`](PhysicsImpostor.md)

Gets or sets impostor used for physic simulation

**`See`**

https://doc.babylonjs.com/features/physics_engine

#### Inherited from

[Mesh](Mesh.md).[physicsImpostor](Mesh.md#physicsimpostor)

#### Defined in

packages/dev/core/src/Physics/physicsEngineComponent.ts:169

___

### reIntegrateRotationIntoRotationQuaternion

• **reIntegrateRotationIntoRotationQuaternion**: `boolean` = `false`

Gets or sets a boolean indicating that even if rotationQuaternion is defined, you can keep updating rotation property and Babylon.js will just mix both

#### Inherited from

[Mesh](Mesh.md).[reIntegrateRotationIntoRotationQuaternion](Mesh.md#reintegraterotationintorotationquaternion)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:144

___

### renderOutline

• **renderOutline**: `boolean`

Gets or sets a boolean indicating if the outline must be rendered as well

**`See`**

https://www.babylonjs-playground.com/#10WJ5S#3

#### Inherited from

[Mesh](Mesh.md).[renderOutline](Mesh.md#renderoutline)

#### Defined in

packages/dev/core/src/Rendering/outlineRenderer.ts:48

___

### renderOverlay

• **renderOverlay**: `boolean`

Gets or sets a boolean indicating if the overlay must be rendered as well

**`See`**

https://www.babylonjs-playground.com/#10WJ5S#2

#### Inherited from

[Mesh](Mesh.md).[renderOverlay](Mesh.md#renderoverlay)

#### Defined in

packages/dev/core/src/Rendering/outlineRenderer.ts:56

___

### reservedDataStore

• **reservedDataStore**: `any` = `null`

For internal use only. Please do not use.

#### Inherited from

[Mesh](Mesh.md).[reservedDataStore](Mesh.md#reserveddatastore)

#### Defined in

packages/dev/core/src/node.ts:120

___

### scalingDeterminant

• **scalingDeterminant**: `number` = `1`

Multiplication factor on scale x/y/z when computing the world matrix. Eg. for a 1x1x1 cube setting this to 2 will make it a 2x2x2 cube

#### Inherited from

[Mesh](Mesh.md).[scalingDeterminant](Mesh.md#scalingdeterminant)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:113

___

### showBoundingBox

• **showBoundingBox**: `boolean`

Gets or sets a boolean indicating if the bounding box must be rendered as well (false by default)

#### Inherited from

[Mesh](Mesh.md).[showBoundingBox](Mesh.md#showboundingbox)

#### Defined in

packages/dev/core/src/Rendering/boundingBoxRenderer.ts:76

___

### showSubMeshesBoundingBox

• **showSubMeshesBoundingBox**: `boolean` = `false`

Gets or sets a boolean indicating that bounding boxes of subMeshes must be rendered as well (false by default)

#### Inherited from

[Mesh](Mesh.md).[showSubMeshesBoundingBox](Mesh.md#showsubmeshesboundingbox)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:429

___

### state

• **state**: `string` = `""`

Gets or sets a string used to store user defined state for the node

#### Inherited from

[Mesh](Mesh.md).[state](Mesh.md#state)

#### Defined in

packages/dev/core/src/node.ts:109

___

### subMeshes

• **subMeshes**: [`SubMesh`](SubMesh.md)[]

Gets or sets the list of subMeshes

**`See`**

https://doc.babylonjs.com/how_to/multi_materials

#### Inherited from

[Mesh](Mesh.md).[subMeshes](Mesh.md#submeshes)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:738

___

### thinInstanceCount

• **thinInstanceCount**: `number`

Gets / sets the number of thin instances to display. Note that you can't set a number higher than what the underlying buffer can handle.

#### Inherited from

[Mesh](Mesh.md).[thinInstanceCount](Mesh.md#thininstancecount)

#### Defined in

packages/dev/core/src/Meshes/thinInstanceMesh.ts:55

___

### thinInstanceEnablePicking

• **thinInstanceEnablePicking**: `boolean`

Gets or sets a boolean defining if we want picking to pick thin instances as well

#### Inherited from

[Mesh](Mesh.md).[thinInstanceEnablePicking](Mesh.md#thininstanceenablepicking)

#### Defined in

packages/dev/core/src/Meshes/thinInstanceMesh.ts:12

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the node

#### Inherited from

[Mesh](Mesh.md).[uniqueId](Mesh.md#uniqueid)

#### Defined in

packages/dev/core/src/node.ts:103

___

### useOctreeForCollisions

• **useOctreeForCollisions**: `boolean` = `true`

Gets or sets a boolean indicating that internal octree (if available) can be used to boost submeshes collision (true by default)

#### Inherited from

[Mesh](Mesh.md).[useOctreeForCollisions](Mesh.md#useoctreeforcollisions)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:614

___

### useOctreeForPicking

• **useOctreeForPicking**: `boolean` = `true`

Gets or sets a boolean indicating that internal octree (if available) can be used to boost submeshes picking (true by default)

#### Inherited from

[Mesh](Mesh.md).[useOctreeForPicking](Mesh.md#useoctreeforpicking)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:612

___

### useOctreeForRenderingSelection

• **useOctreeForRenderingSelection**: `boolean` = `true`

Gets or sets a boolean indicating that internal octree (if available) can be used to boost submeshes selection (true by default)

#### Inherited from

[Mesh](Mesh.md).[useOctreeForRenderingSelection](Mesh.md#useoctreeforrenderingselection)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:610

___

### BACKSIDE

▪ `Static` `Readonly` **BACKSIDE**: ``1``

Mesh side orientation : usually the internal or back surface

#### Inherited from

[Mesh](Mesh.md).[BACKSIDE](Mesh.md#backside)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:159

___

### BOTTOM

▪ `Static` `Readonly` **BOTTOM**: ``4``

Mesh tile positioning : part tiles on bottom

#### Inherited from

[Mesh](Mesh.md).[BOTTOM](Mesh.md#bottom)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:231

___

### CAP\_ALL

▪ `Static` `Readonly` **CAP\_ALL**: ``3``

Mesh cap setting : two caps, one at the beginning  and one at the end of the mesh

#### Inherited from

[Mesh](Mesh.md).[CAP_ALL](Mesh.md#cap_all)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:183

___

### CAP\_END

▪ `Static` `Readonly` **CAP\_END**: ``2``

Mesh cap setting : one cap at the end of the mesh

#### Inherited from

[Mesh](Mesh.md).[CAP_END](Mesh.md#cap_end)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:179

___

### CAP\_START

▪ `Static` `Readonly` **CAP\_START**: ``1``

Mesh cap setting : one cap at the beginning of the mesh

#### Inherited from

[Mesh](Mesh.md).[CAP_START](Mesh.md#cap_start)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:175

___

### CENTER

▪ `Static` `Readonly` **CENTER**: ``0``

Mesh tile positioning : part tiles same on left/right or top/bottom

#### Inherited from

[Mesh](Mesh.md).[CENTER](Mesh.md#center)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:215

___

### CULLINGSTRATEGY\_BOUNDINGSPHERE\_ONLY

▪ `Static` `Readonly` **CULLINGSTRATEGY\_BOUNDINGSPHERE\_ONLY**: ``1``

Culling strategy : Bounding Sphere Only.
 This is an exclusion test. It's faster than the standard strategy because the bounding box is not tested.
 It's also less accurate than the standard because some not visible objects can still be selected.
 Test : is the bounding sphere outside the frustum ?
 If not, then the cullable object is in the frustum.

#### Inherited from

[Mesh](Mesh.md).[CULLINGSTRATEGY_BOUNDINGSPHERE_ONLY](Mesh.md#cullingstrategy_boundingsphere_only)

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

[Mesh](Mesh.md).[CULLINGSTRATEGY_OPTIMISTIC_INCLUSION](Mesh.md#cullingstrategy_optimistic_inclusion)

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

[Mesh](Mesh.md).[CULLINGSTRATEGY_OPTIMISTIC_INCLUSION_THEN_BSPHERE_ONLY](Mesh.md#cullingstrategy_optimistic_inclusion_then_bsphere_only)

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

[Mesh](Mesh.md).[CULLINGSTRATEGY_STANDARD](Mesh.md#cullingstrategy_standard)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:136

___

### DEFAULTSIDE

▪ `Static` `Readonly` **DEFAULTSIDE**: ``0``

Mesh side orientation : by default, `FRONTSIDE`

#### Inherited from

[Mesh](Mesh.md).[DEFAULTSIDE](Mesh.md#defaultside)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:167

___

### DOUBLESIDE

▪ `Static` `Readonly` **DOUBLESIDE**: ``2``

Mesh side orientation : both internal and external or front and back surfaces

#### Inherited from

[Mesh](Mesh.md).[DOUBLESIDE](Mesh.md#doubleside)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:163

___

### FLIP\_N\_ROTATE\_ROW

▪ `Static` `Readonly` **FLIP\_N\_ROTATE\_ROW**: ``6``

Mesh pattern setting : rotate pattern and rotate

#### Inherited from

[Mesh](Mesh.md).[FLIP_N_ROTATE_ROW](Mesh.md#flip_n_rotate_row)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:211

___

### FLIP\_N\_ROTATE\_TILE

▪ `Static` `Readonly` **FLIP\_N\_ROTATE\_TILE**: ``5``

Mesh pattern setting : flip and rotate alternate tiles on each row or column

#### Inherited from

[Mesh](Mesh.md).[FLIP_N_ROTATE_TILE](Mesh.md#flip_n_rotate_tile)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:207

___

### FLIP\_ROW

▪ `Static` `Readonly` **FLIP\_ROW**: ``3``

Mesh pattern setting : flip (reflect in y axis) all tiles on alternate rows

#### Inherited from

[Mesh](Mesh.md).[FLIP_ROW](Mesh.md#flip_row)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:199

___

### FLIP\_TILE

▪ `Static` `Readonly` **FLIP\_TILE**: ``1``

Mesh pattern setting : flip (reflect in y axis) alternate tiles on each row or column

#### Inherited from

[Mesh](Mesh.md).[FLIP_TILE](Mesh.md#flip_tile)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:191

___

### FRONTSIDE

▪ `Static` `Readonly` **FRONTSIDE**: ``0``

Mesh side orientation : usually the external or front surface

#### Inherited from

[Mesh](Mesh.md).[FRONTSIDE](Mesh.md#frontside)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:154

___

### INSTANCEDMESH\_SORT\_TRANSPARENT

▪ `Static` **INSTANCEDMESH\_SORT\_TRANSPARENT**: `boolean` = `false`

Indicates that the instanced meshes should be sorted from back to front before rendering if their material is transparent

#### Inherited from

[Mesh](Mesh.md).[INSTANCEDMESH_SORT_TRANSPARENT](Mesh.md#instancedmesh_sort_transparent)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:236

___

### LEFT

▪ `Static` `Readonly` **LEFT**: ``1``

Mesh tile positioning : part tiles on left

#### Inherited from

[Mesh](Mesh.md).[LEFT](Mesh.md#left)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:219

___

### NO\_CAP

▪ `Static` `Readonly` **NO\_CAP**: ``0``

Mesh cap setting : no cap

#### Inherited from

[Mesh](Mesh.md).[NO_CAP](Mesh.md#no_cap)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:171

___

### NO\_FLIP

▪ `Static` `Readonly` **NO\_FLIP**: ``0``

Mesh pattern setting : no flip or rotate

#### Inherited from

[Mesh](Mesh.md).[NO_FLIP](Mesh.md#no_flip)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:187

___

### OCCLUSION\_ALGORITHM\_TYPE\_ACCURATE

▪ `Static` **OCCLUSION\_ALGORITHM\_TYPE\_ACCURATE**: `number` = `0`

Use an accurate occlusion algorithm

#### Inherited from

[Mesh](Mesh.md).[OCCLUSION_ALGORITHM_TYPE_ACCURATE](Mesh.md#occlusion_algorithm_type_accurate)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:126

___

### OCCLUSION\_ALGORITHM\_TYPE\_CONSERVATIVE

▪ `Static` **OCCLUSION\_ALGORITHM\_TYPE\_CONSERVATIVE**: `number` = `1`

Use a conservative occlusion algorithm

#### Inherited from

[Mesh](Mesh.md).[OCCLUSION_ALGORITHM_TYPE_CONSERVATIVE](Mesh.md#occlusion_algorithm_type_conservative)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:128

___

### OCCLUSION\_TYPE\_NONE

▪ `Static` **OCCLUSION\_TYPE\_NONE**: `number` = `0`

No occlusion

#### Inherited from

[Mesh](Mesh.md).[OCCLUSION_TYPE_NONE](Mesh.md#occlusion_type_none)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:120

___

### OCCLUSION\_TYPE\_OPTIMISTIC

▪ `Static` **OCCLUSION\_TYPE\_OPTIMISTIC**: `number` = `1`

Occlusion set to optimistic

#### Inherited from

[Mesh](Mesh.md).[OCCLUSION_TYPE_OPTIMISTIC](Mesh.md#occlusion_type_optimistic)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:122

___

### OCCLUSION\_TYPE\_STRICT

▪ `Static` **OCCLUSION\_TYPE\_STRICT**: `number` = `2`

Occlusion set to strict

#### Inherited from

[Mesh](Mesh.md).[OCCLUSION_TYPE_STRICT](Mesh.md#occlusion_type_strict)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:124

___

### RIGHT

▪ `Static` `Readonly` **RIGHT**: ``2``

Mesh tile positioning : part tiles on right

#### Inherited from

[Mesh](Mesh.md).[RIGHT](Mesh.md#right)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:223

___

### ROTATE\_ROW

▪ `Static` `Readonly` **ROTATE\_ROW**: ``4``

Mesh pattern setting : rotate (180degs) all tiles on alternate rows

#### Inherited from

[Mesh](Mesh.md).[ROTATE_ROW](Mesh.md#rotate_row)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:203

___

### ROTATE\_TILE

▪ `Static` `Readonly` **ROTATE\_TILE**: ``2``

Mesh pattern setting : rotate (180degs) alternate tiles on each row or column

#### Inherited from

[Mesh](Mesh.md).[ROTATE_TILE](Mesh.md#rotate_tile)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:195

___

### TOP

▪ `Static` `Readonly` **TOP**: ``3``

Mesh tile positioning : part tiles on top

#### Inherited from

[Mesh](Mesh.md).[TOP](Mesh.md#top)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:227

## Accessors

### absolutePosition

• `get` **absolutePosition**(): [`Vector3`](Vector3.md)

Returns the current mesh absolute position.
Returns a Vector3.

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

Mesh.absolutePosition

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

Mesh.absoluteRotationQuaternion

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

Mesh.absoluteScaling

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:352

___

### animationPropertiesOverride

• `get` **animationPropertiesOverride**(): [`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md)

Gets or sets the animation properties override

#### Returns

[`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md)

#### Inherited from

Mesh.animationPropertiesOverride

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

Mesh.animationPropertiesOverride

#### Defined in

packages/dev/core/src/node.ts:282

___

### applyFog

• `get` **applyFog**(): `boolean`

Gets or sets a boolean indicating that this mesh will allow fog to be rendered on it (true by default)

#### Returns

`boolean`

#### Inherited from

Mesh.applyFog

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

Mesh.applyFog

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:592

___

### areNormalsFrozen

• `get` **areNormalsFrozen**(): `boolean`

Gets a boolean indicating if the normals aren't to be recomputed on next mesh `positions` array update. This property is pertinent only for updatable parametric shapes.

#### Returns

`boolean`

#### Inherited from

Mesh.areNormalsFrozen

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:1240

___

### bakedVertexAnimationManager

• `get` **bakedVertexAnimationManager**(): [`Nullable`](../modules.md#nullable)[`IBakedVertexAnimationManager`](../interfaces/IBakedVertexAnimationManager.md)

Gets or sets the baked vertex animation manager

**`See`**

https://doc.babylonjs.com/divingDeeper/animation/baked_texture_animations

#### Returns

[`Nullable`](../modules.md#nullable)[`IBakedVertexAnimationManager`](../interfaces/IBakedVertexAnimationManager.md)

#### Inherited from

Mesh.bakedVertexAnimationManager

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

Mesh.bakedVertexAnimationManager

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

Mesh.behaviors

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

Mesh.billboardMode

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

Mesh.billboardMode

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

Mesh.checkCollisions

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

Mesh.checkCollisions

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1690

___

### cloneMeshMap

• `get` **cloneMeshMap**(): [`Nullable`](../modules.md#nullable){ `[id: string]`: [`Mesh`](Mesh.md) \| `undefined`;  }

Gets the list of clones of this mesh
The scene must have been constructed with useClonedMeshMap=true for this to work!
Note that useClonedMeshMap=true is the default setting

#### Returns

[`Nullable`](../modules.md#nullable){ `[id: string]`: [`Mesh`](Mesh.md) \| `undefined`;  }

#### Inherited from

Mesh.cloneMeshMap

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:456

___

### collider

• `get` **collider**(): [`Nullable`](../modules.md#nullable)`Collider`

Gets Collider object used to compute collisions (not physics)

**`See`**

https://doc.babylonjs.com/babylon101/cameras,_mesh_collisions_and_gravity

#### Returns

[`Nullable`](../modules.md#nullable)`Collider`

#### Inherited from

Mesh.collider

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

Mesh.collisionGroup

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

Mesh.collisionGroup

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

Mesh.collisionMask

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

Mesh.collisionMask

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

Mesh.collisionResponse

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

Mesh.collisionResponse

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:681

___

### collisionRetryCount

• `get` **collisionRetryCount**(): `number`

number of collision detection tries. Change this value if not all collisions are detected and handled properly

#### Returns

`number`

#### Inherited from

Mesh.collisionRetryCount

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

Mesh.collisionRetryCount

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:275

___

### computeBonesUsingShaders

• `get` **computeBonesUsingShaders**(): `boolean`

Gets or sets a boolean indicating that bone animations must be computed by the CPU (false by default)

#### Returns

`boolean`

#### Inherited from

Mesh.computeBonesUsingShaders

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:268

• `set` **computeBonesUsingShaders**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

Mesh.computeBonesUsingShaders

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:271

___

### doNotSerialize

• `get` **doNotSerialize**(): `boolean`

Gets or sets a boolean used to define if the node must be serialized

#### Returns

`boolean`

#### Inherited from

Mesh.doNotSerialize

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

Mesh.doNotSerialize

#### Defined in

packages/dev/core/src/node.ts:143

___

### enableDistantPicking

• `get` **enableDistantPicking**(): `boolean`

When enabled, decompose picking matrices for better precision with large values for mesh position and scling

#### Returns

`boolean`

#### Inherited from

Mesh.enableDistantPicking

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

Mesh.enableDistantPicking

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

Mesh.facetDepthSortFrom

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

Mesh.facetDepthSortFrom

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

Mesh.facetNb

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:220

___

### forcedInstanceCount

• `get` **forcedInstanceCount**(): `number`

Gets or sets the forced number of instances to display.
If 0 (default value), the number of instances is not forced and depends on the draw type
(regular / instance / thin instances mesh)

#### Returns

`number`

#### Inherited from

Mesh.forcedInstanceCount

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:412

• `set` **forcedInstanceCount**(`count`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `count` | `number` |

#### Returns

`void`

#### Inherited from

Mesh.forcedInstanceCount

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:416

___

### forward

• `get` **forward**(): [`Vector3`](Vector3.md)

The forward direction of that transform in world space.

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

Mesh.forward

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:253

___

### geometry

• `get` **geometry**(): [`Nullable`](../modules.md#nullable)[`Geometry`](Geometry.md)

Gets the mesh internal Geometry object

#### Returns

[`Nullable`](../modules.md#nullable)[`Geometry`](Geometry.md)

#### Inherited from

Mesh.geometry

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:975

___

### hasBoundingInfo

• `get` **hasBoundingInfo**(): `boolean`

Returns true if there is already a bounding info

#### Returns

`boolean`

#### Inherited from

Mesh.hasBoundingInfo

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1230

___

### hasInstances

• `get` **hasInstances**(): `boolean`

Gets a boolean indicating if this mesh has instances

#### Returns

`boolean`

#### Inherited from

Mesh.hasInstances

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:358

___

### hasLODLevels

• `get` **hasLODLevels**(): `boolean`

Gets a boolean indicating if this mesh has LOD

#### Returns

`boolean`

#### Inherited from

Mesh.hasLODLevels

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:806

___

### hasThinInstances

• `get` **hasThinInstances**(): `boolean`

Gets a boolean indicating if this mesh has thin instances

#### Returns

`boolean`

#### Inherited from

Mesh.hasThinInstances

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:362

___

### hasVertexAlpha

• `get` **hasVertexAlpha**(): `boolean`

Gets or sets a boolean indicating that this mesh contains vertex color data with alpha values

#### Returns

`boolean`

#### Inherited from

Mesh.hasVertexAlpha

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

Mesh.hasVertexAlpha

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:537

___

### infiniteDistance

• `get` **infiniteDistance**(): `boolean`

Gets or sets the distance of the object to max, often used by skybox

#### Returns

`boolean`

#### Inherited from

Mesh.infiniteDistance

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

Mesh.infiniteDistance

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:125

___

### isAnInstance

• `get` **isAnInstance**(): `boolean`

Gets a boolean indicating if this mesh is an instance or a regular mesh

#### Returns

`boolean`

#### Inherited from

Mesh.isAnInstance

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1327

___

### isBlocked

• `get` **isBlocked**(): `boolean`

Returns true if the mesh is blocked. Implemented by child classes

#### Returns

`boolean`

#### Inherited from

Mesh.isBlocked

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:1151

___

### isFacetDataEnabled

• `get` **isFacetDataEnabled**(): `boolean`

gets a boolean indicating if facetData is enabled

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_facetdata#what-is-a-mesh-facet

#### Returns

`boolean`

#### Inherited from

Mesh.isFacetDataEnabled

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:282

___

### isUnIndexed

• `get` **isUnIndexed**(): `boolean`

Gets or sets a boolean indicating that this mesh does not use index buffer

#### Returns

`boolean`

#### Inherited from

Mesh.isUnIndexed

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:463

• `set` **isUnIndexed**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

Mesh.isUnIndexed

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:467

___

### isWorldMatrixFrozen

• `get` **isWorldMatrixFrozen**(): `boolean`

True if the World matrix has been frozen.

#### Returns

`boolean`

#### Inherited from

Mesh.isWorldMatrixFrozen

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

Mesh.layerMask

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

Mesh.layerMask

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:623

___

### lightSources

• `get` **lightSources**(): [`Light`](Light.md)[]

Gets the list of lights affecting that mesh

#### Returns

[`Light`](Light.md)[]

#### Inherited from

Mesh.lightSources

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:750

___

### manualUpdateOfPreviousWorldMatrixInstancedBuffer

• `get` **manualUpdateOfPreviousWorldMatrixInstancedBuffer**(): `boolean`

Gets or sets a boolean indicating that the update of the instance buffer of the world matrices is manual

#### Returns

`boolean`

#### Inherited from

Mesh.manualUpdateOfPreviousWorldMatrixInstancedBuffer

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:494

• `set` **manualUpdateOfPreviousWorldMatrixInstancedBuffer**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

Mesh.manualUpdateOfPreviousWorldMatrixInstancedBuffer

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:498

___

### manualUpdateOfWorldMatrixInstancedBuffer

• `get` **manualUpdateOfWorldMatrixInstancedBuffer**(): `boolean`

Gets or sets a boolean indicating that the update of the instance buffer of the world matrices is manual

#### Returns

`boolean`

#### Inherited from

Mesh.manualUpdateOfWorldMatrixInstancedBuffer

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:485

• `set` **manualUpdateOfWorldMatrixInstancedBuffer**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

Mesh.manualUpdateOfWorldMatrixInstancedBuffer

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:489

___

### material

• `get` **material**(): [`Nullable`](../modules.md#nullable)[`Material`](Material.md)

Gets or sets current material

#### Returns

[`Nullable`](../modules.md#nullable)[`Material`](Material.md)

#### Inherited from

Mesh.material

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:454

• `set` **material**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`Material`](Material.md) |

#### Returns

`void`

#### Inherited from

Mesh.material

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:457

___

### morphTargetManager

• `get` **morphTargetManager**(): [`Nullable`](../modules.md#nullable)[`MorphTargetManager`](MorphTargetManager.md)

Gets or sets the morph target manager

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_morphtargets

#### Returns

[`Nullable`](../modules.md#nullable)[`MorphTargetManager`](MorphTargetManager.md)

#### Inherited from

Mesh.morphTargetManager

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

Mesh.morphTargetManager

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

Mesh.mustDepthSortFacets

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

Mesh.mustDepthSortFacets

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:254

___

### nonUniformScaling

• `get` **nonUniformScaling**(): `boolean`

True if the scaling property of this object is non uniform eg. (1,2,1)

#### Returns

`boolean`

#### Inherited from

Mesh.nonUniformScaling

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:799

___

### numBoneInfluencers

• `get` **numBoneInfluencers**(): `number`

Gets or sets the number of allowed bone influences per vertex (4 by default)

#### Returns

`number`

#### Inherited from

Mesh.numBoneInfluencers

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

Mesh.numBoneInfluencers

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:579

___

### onAfterRenderObservable

• `get` **onAfterRenderObservable**(): [`Observable`](Observable.md)[`Mesh`](Mesh.md)

An event triggered after rendering the mesh

#### Returns

[`Observable`](Observable.md)[`Mesh`](Mesh.md)

#### Inherited from

Mesh.onAfterRenderObservable

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:316

___

### onBeforeBindObservable

• `get` **onBeforeBindObservable**(): [`Observable`](Observable.md)[`Mesh`](Mesh.md)

An event triggered before binding the mesh

#### Returns

[`Observable`](Observable.md)[`Mesh`](Mesh.md)

#### Inherited from

Mesh.onBeforeBindObservable

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:305

___

### onBeforeDraw

• `set` **onBeforeDraw**(`callback`): `void`

Sets a callback to call before drawing the mesh. It is recommended to use onBeforeDrawObservable instead

#### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | () => `void` |

#### Returns

`void`

#### Inherited from

Mesh.onBeforeDraw

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:351

___

### onBeforeDrawObservable

• `get` **onBeforeDrawObservable**(): [`Observable`](Observable.md)[`Mesh`](Mesh.md)

An event triggered before drawing the mesh

#### Returns

[`Observable`](Observable.md)[`Mesh`](Mesh.md)

#### Inherited from

Mesh.onBeforeDrawObservable

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:338

___

### onBeforeRenderObservable

• `get` **onBeforeRenderObservable**(): [`Observable`](Observable.md)[`Mesh`](Mesh.md)

An event triggered before rendering the mesh

#### Returns

[`Observable`](Observable.md)[`Mesh`](Mesh.md)

#### Inherited from

Mesh.onBeforeRenderObservable

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:294

___

### onBetweenPassObservable

• `get` **onBetweenPassObservable**(): [`Observable`](Observable.md)[`SubMesh`](SubMesh.md)

An event triggeredbetween rendering pass when using separateCullingPass = true

#### Returns

[`Observable`](Observable.md)[`SubMesh`](SubMesh.md)

#### Inherited from

Mesh.onBetweenPassObservable

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:327

___

### onClonedObservable

• `get` **onClonedObservable**(): [`Observable`](Observable.md)[`Node`](Node.md)

An event triggered when the node is cloned

#### Returns

[`Observable`](Observable.md)[`Node`](Node.md)

#### Inherited from

Mesh.onClonedObservable

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

Mesh.onCollide

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

Mesh.onCollisionPositionChange

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

Mesh.onDispose

#### Defined in

packages/dev/core/src/node.ts:306

___

### onEnabledStateChangedObservable

• `get` **onEnabledStateChangedObservable**(): [`Observable`](Observable.md)`boolean`

An event triggered when the enabled state of the node changes

#### Returns

[`Observable`](Observable.md)`boolean`

#### Inherited from

Mesh.onEnabledStateChangedObservable

#### Defined in

packages/dev/core/src/node.ts:316

___

### overridenInstanceCount

• `set` **overridenInstanceCount**(`count`): `void`

Sets a value overriding the instance count. Only applicable when custom instanced InterleavedVertexBuffer are used rather than InstancedMeshs

#### Parameters

| Name | Type |
| :------ | :------ |
| `count` | `number` |

#### Returns

`void`

#### Inherited from

Mesh.overridenInstanceCount

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:1265

___

### parent

• `get` **parent**(): [`Nullable`](../modules.md#nullable)[`Node`](Node.md)

#### Returns

[`Nullable`](../modules.md#nullable)[`Node`](Node.md)

#### Inherited from

Mesh.parent

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

Mesh.parent

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

Mesh.partitioningBBoxRatio

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

Mesh.partitioningBBoxRatio

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

Mesh.partitioningSubdivisions

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

Mesh.partitioningSubdivisions

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:230

___

### position

• `get` **position**(): [`Vector3`](Vector3.md)

Gets or set the node position (default is (0.0, 0.0, 0.0))

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

Mesh.position

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

Mesh.position

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

Mesh.preserveParentRotationForBillboard

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

Mesh.preserveParentRotationForBillboard

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:102

___

### previousWorldMatrixInstancedBuffer

• `get` **previousWorldMatrixInstancedBuffer**(): `Float32Array`

Gets the array buffer used to store the instanced buffer used for instances' previous world matrices

#### Returns

`Float32Array`

#### Inherited from

Mesh.previousWorldMatrixInstancedBuffer

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:480

___

### receiveShadows

• `get` **receiveShadows**(): `boolean`

Gets or sets a boolean indicating that this mesh can receive realtime shadows

**`See`**

https://doc.babylonjs.com/babylon101/shadows

#### Returns

`boolean`

#### Inherited from

Mesh.receiveShadows

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:511

• `set` **receiveShadows**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

Mesh.receiveShadows

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

#### Inherited from

Mesh.renderingGroupId

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:445

• `set` **renderingGroupId**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

Mesh.renderingGroupId

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:449

___

### right

• `get` **right**(): [`Vector3`](Vector3.md)

The right direction of that transform in world space.

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

Mesh.right

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

Mesh.rotation

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

Mesh.rotation

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

Mesh.rotationQuaternion

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

Mesh.rotationQuaternion

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:241

___

### scaling

• `get` **scaling**(): [`Vector3`](Vector3.md)

Gets or sets the scaling property : a Vector3 defining the node scaling along each local axis X, Y, Z (default is (1.0, 1.0, 1.0)).

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

Mesh.scaling

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

Mesh.scaling

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:228

___

### skeleton

• `get` **skeleton**(): [`Nullable`](../modules.md#nullable)[`Skeleton`](Skeleton.md)

#### Returns

[`Nullable`](../modules.md#nullable)[`Skeleton`](Skeleton.md)

#### Inherited from

Mesh.skeleton

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

#### Inherited from

Mesh.skeleton

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:781

___

### source

• `get` **source**(): [`Nullable`](../modules.md#nullable)[`Mesh`](Mesh.md)

Gets the source mesh (the one used to clone this one from)

#### Returns

[`Nullable`](../modules.md#nullable)[`Mesh`](Mesh.md)

#### Inherited from

Mesh.source

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:447

___

### subdivisions

• `get` **subdivisions**(): `number`

The minimum of x and y subdivisions

#### Returns

`number`

#### Defined in

packages/dev/core/src/Meshes/groundMesh.ts:51

___

### subdivisionsX

• `get` **subdivisionsX**(): `number`

X subdivisions

#### Returns

`number`

#### Defined in

packages/dev/core/src/Meshes/groundMesh.ts:58

___

### subdivisionsY

• `get` **subdivisionsY**(): `number`

Y subdivisions

#### Returns

`number`

#### Defined in

packages/dev/core/src/Meshes/groundMesh.ts:65

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

Mesh.surroundingMeshes

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

Mesh.surroundingMeshes

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:709

___

### up

• `get` **up**(): [`Vector3`](Vector3.md)

The up direction of that transform in world space.

#### Returns

[`Vector3`](Vector3.md)

#### Inherited from

Mesh.up

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:261

___

### useBones

• `get` **useBones**(): `boolean`

Gets a boolean indicating if this mesh has skinning data and an attached skeleton

#### Returns

`boolean`

#### Inherited from

Mesh.useBones

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1258

___

### useLODScreenCoverage

• `get` **useLODScreenCoverage**(): `boolean`

Determines if the LOD levels are intended to be calculated using screen coverage (surface area ratio) instead of distance

#### Returns

`boolean`

#### Inherited from

Mesh.useLODScreenCoverage

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:254

• `set` **useLODScreenCoverage**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

Mesh.useLODScreenCoverage

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:258

___

### useVertexColors

• `get` **useVertexColors**(): `boolean`

Gets or sets a boolean indicating that this mesh needs to use vertex color data to render (if this kind of vertex data is available in the geometry)

#### Returns

`boolean`

#### Inherited from

Mesh.useVertexColors

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

Mesh.useVertexColors

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:551

___

### visibility

• `get` **visibility**(): `number`

Gets or sets mesh visibility between 0 and 1 (default is 1)

#### Returns

`number`

#### Inherited from

Mesh.visibility

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

#### Inherited from

Mesh.visibility

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

Mesh.worldMatrixFromCache

#### Defined in

packages/dev/core/src/node.ts:454

___

### worldMatrixInstancedBuffer

• `get` **worldMatrixInstancedBuffer**(): `Float32Array`

Gets the array buffer used to store the instanced buffer used for instances' world matrices

#### Returns

`Float32Array`

#### Inherited from

Mesh.worldMatrixInstancedBuffer

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:475

___

### BILLBOARDMODE\_ALL

• `Static` `get` **BILLBOARDMODE_ALL**(): `number`

Billboard on all axes

#### Returns

`number`

#### Inherited from

Mesh.BILLBOARDMODE\_ALL

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:188

___

### BILLBOARDMODE\_NONE

• `Static` `get` **BILLBOARDMODE_NONE**(): `number`

No billboard

#### Returns

`number`

#### Inherited from

Mesh.BILLBOARDMODE\_NONE

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:168

___

### BILLBOARDMODE\_USE\_POSITION

• `Static` `get` **BILLBOARDMODE_USE_POSITION**(): `number`

Billboard on using position instead of orientation

#### Returns

`number`

#### Inherited from

Mesh.BILLBOARDMODE\_USE\_POSITION

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:193

___

### BILLBOARDMODE\_X

• `Static` `get` **BILLBOARDMODE_X**(): `number`

Billboard on X axis

#### Returns

`number`

#### Inherited from

Mesh.BILLBOARDMODE\_X

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:173

___

### BILLBOARDMODE\_Y

• `Static` `get` **BILLBOARDMODE_Y**(): `number`

Billboard on Y axis

#### Returns

`number`

#### Inherited from

Mesh.BILLBOARDMODE\_Y

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:178

___

### BILLBOARDMODE\_Z

• `Static` `get` **BILLBOARDMODE_Z**(): `number`

Billboard on Z axis

#### Returns

`number`

#### Inherited from

Mesh.BILLBOARDMODE\_Z

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:183

## Methods

### \_afterComputeWorldMatrix

▸ `Protected` **_afterComputeWorldMatrix**(): `void`

#### Returns

`void`

#### Inherited from

[Mesh](Mesh.md).[_afterComputeWorldMatrix](Mesh.md#_aftercomputeworldmatrix)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:1319

___

### \_buildUniformLayout

▸ `Protected` **_buildUniformLayout**(): `void`

#### Returns

`void`

#### Inherited from

[Mesh](Mesh.md).[_buildUniformLayout](Mesh.md#_builduniformlayout)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:834

___

### \_computeHeightQuads

▸ `Private` **_computeHeightQuads**(): [`GroundMesh`](GroundMesh.md)

#### Returns

[`GroundMesh`](GroundMesh.md)

#### Defined in

packages/dev/core/src/Meshes/groundMesh.ts:211

___

### \_getFacetAt

▸ `Private` **_getFacetAt**(`x`, `z`): [`Vector4`](Vector4.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `x` | `number` |
| `z` | `number` |

#### Returns

[`Vector4`](Vector4.md)

#### Defined in

packages/dev/core/src/Meshes/groundMesh.ts:173

___

### \_initHeightQuads

▸ `Private` **_initHeightQuads**(): [`GroundMesh`](GroundMesh.md)

#### Returns

[`GroundMesh`](GroundMesh.md)

#### Defined in

packages/dev/core/src/Meshes/groundMesh.ts:193

___

### \_invalidateInstanceVertexArrayObject

▸ **_invalidateInstanceVertexArrayObject**(): `void`

Invalidate VertexArrayObjects belonging to the mesh (but not to the Geometry of the mesh).

#### Returns

`void`

#### Inherited from

[Mesh](Mesh.md).[_invalidateInstanceVertexArrayObject](Mesh.md#_invalidateinstancevertexarrayobject)

#### Defined in

packages/dev/core/src/Meshes/instancedMesh.ts:570

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

[Mesh](Mesh.md).[addBehavior](Mesh.md#addbehavior)

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

[Mesh](Mesh.md).[addChild](Mesh.md#addchild)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:2141

___

### addLODLevel

▸ **addLODLevel**(`distanceOrScreenCoverage`, `mesh`): [`Mesh`](Mesh.md)

Add a mesh as LOD level triggered at the given distance.

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_lod

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `distanceOrScreenCoverage` | `number` | Either distance from the center of the object to show this level or the screen coverage if `useScreenCoverage` is set to `true`.  If screen coverage, value is a fraction of the screen's total surface, between 0 and 1. |
| `mesh` | [`Nullable`](../modules.md#nullable)[`Mesh`](Mesh.md) | The mesh to be added as LOD level (can be null) |

#### Returns

[`Mesh`](Mesh.md)

This mesh (for chaining)

#### Inherited from

[Mesh](Mesh.md).[addLODLevel](Mesh.md#addlodlevel)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:840

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

[Mesh](Mesh.md).[addRotation](Mesh.md#addrotation)

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

[Mesh](Mesh.md).[alignWithNormal](Mesh.md#alignwithnormal)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:2557

___

### applyDisplacementMap

▸ **applyDisplacementMap**(`url`, `minHeight`, `maxHeight`, `onSuccess?`, `uvOffset?`, `uvScale?`, `forceUpdate?`): [`Mesh`](Mesh.md)

Modifies the mesh geometry according to a displacement map.
A displacement map is a colored image. Each pixel color value (actually a gradient computed from red, green, blue values) will give the displacement to apply to each mesh vertex.
The mesh must be set as updatable. Its internal geometry is directly modified, no new buffer are allocated.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `url` | `string` | `undefined` | is a string, the URL from the image file is to be downloaded. |
| `minHeight` | `number` | `undefined` | is the lower limit of the displacement. |
| `maxHeight` | `number` | `undefined` | is the upper limit of the displacement. |
| `onSuccess?` | (`mesh`: [`Mesh`](Mesh.md)) => `void` | `undefined` | is an optional Javascript function to be called just after the mesh is modified. It is passed the modified mesh and must return nothing. |
| `uvOffset?` | [`Vector2`](Vector2.md) | `undefined` | is an optional vector2 used to offset UV. |
| `uvScale?` | [`Vector2`](Vector2.md) | `undefined` | is an optional vector2 used to scale UV. |
| `forceUpdate` | `boolean` | `false` | defines whether or not to force an update of the generated buffers. This is useful to apply on a deserialized model for instance. |

#### Returns

[`Mesh`](Mesh.md)

the Mesh.

#### Inherited from

[Mesh](Mesh.md).[applyDisplacementMap](Mesh.md#applydisplacementmap)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:2852

___

### applyDisplacementMapFromBuffer

▸ **applyDisplacementMapFromBuffer**(`buffer`, `heightMapWidth`, `heightMapHeight`, `minHeight`, `maxHeight`, `uvOffset?`, `uvScale?`, `forceUpdate?`): [`Mesh`](Mesh.md)

Modifies the mesh geometry according to a displacementMap buffer.
A displacement map is a colored image. Each pixel color value (actually a gradient computed from red, green, blue values) will give the displacement to apply to each mesh vertex.
The mesh must be set as updatable. Its internal geometry is directly modified, no new buffer are allocated.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `buffer` | `Uint8Array` | `undefined` | is a `Uint8Array` buffer containing series of `Uint8` lower than 255, the red, green, blue and alpha values of each successive pixel. |
| `heightMapWidth` | `number` | `undefined` | is the width of the buffer image. |
| `heightMapHeight` | `number` | `undefined` | is the height of the buffer image. |
| `minHeight` | `number` | `undefined` | is the lower limit of the displacement. |
| `maxHeight` | `number` | `undefined` | is the upper limit of the displacement. |
| `uvOffset?` | [`Vector2`](Vector2.md) | `undefined` | is an optional vector2 used to offset UV. |
| `uvScale?` | [`Vector2`](Vector2.md) | `undefined` | is an optional vector2 used to scale UV. |
| `forceUpdate` | `boolean` | `false` | defines whether or not to force an update of the generated buffers. This is useful to apply on a deserialized model for instance. |

#### Returns

[`Mesh`](Mesh.md)

the Mesh.

#### Inherited from

[Mesh](Mesh.md).[applyDisplacementMapFromBuffer](Mesh.md#applydisplacementmapfrombuffer)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:2901

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

[Mesh](Mesh.md).[applyImpulse](Mesh.md#applyimpulse)

#### Defined in

packages/dev/core/src/Physics/physicsEngineComponent.ts:184

___

### applySkeleton

▸ **applySkeleton**(`skeleton`): [`Mesh`](Mesh.md)

Updates the vertex buffer by applying transformation from the bones

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `skeleton` | [`Skeleton`](Skeleton.md) | defines the skeleton to apply to current mesh |

#### Returns

[`Mesh`](Mesh.md)

the current mesh

#### Inherited from

[Mesh](Mesh.md).[applySkeleton](Mesh.md#applyskeleton)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:4248

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

[Mesh](Mesh.md).[attachToBone](Mesh.md#attachtobone)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:822

___

### bakeCurrentTransformIntoVertices

▸ **bakeCurrentTransformIntoVertices**(`bakeIndependenlyOfChildren?`): [`Mesh`](Mesh.md)

Modifies the mesh geometry according to its own current World Matrix.
The mesh World Matrix is then reset.
This method returns nothing but really modifies the mesh even if it's originally not set as updatable.
Note that, under the hood, this method sets a new VertexBuffer each call.

**`See`**

https://doc.babylonjs.com/resources/baking_transformations

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `bakeIndependenlyOfChildren` | `boolean` | `true` | indicates whether to preserve all child nodes' World Matrix during baking |

#### Returns

[`Mesh`](Mesh.md)

the current mesh

#### Inherited from

[Mesh](Mesh.md).[bakeCurrentTransformIntoVertices](Mesh.md#bakecurrenttransformintovertices)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:2701

___

### bakeTransformIntoVertices

▸ **bakeTransformIntoVertices**(`transform`): [`Mesh`](Mesh.md)

Modifies the mesh geometry according to the passed transformation matrix.
This method returns nothing but it really modifies the mesh even if it's originally not set as updatable.
The mesh normals are modified using the same transformation.
Note that, under the hood, this method sets a new VertexBuffer each call.

**`See`**

https://doc.babylonjs.com/resources/baking_transformations

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `transform` | [`Matrix`](Matrix.md) | defines the transform matrix to use |

#### Returns

[`Mesh`](Mesh.md)

the current mesh

#### Inherited from

[Mesh](Mesh.md).[bakeTransformIntoVertices](Mesh.md#baketransformintovertices)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:2651

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

[Mesh](Mesh.md).[beginAnimation](Mesh.md#beginanimation)

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

[Mesh](Mesh.md).[buildBoundingInfo](Mesh.md#buildboundinginfo)

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

[Mesh](Mesh.md).[calcMovePOV](Mesh.md#calcmovepov)

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

[Mesh](Mesh.md).[calcRotatePOV](Mesh.md#calcrotatepov)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1402

___

### cleanMatrixWeights

▸ **cleanMatrixWeights**(): `void`

Renormalize the mesh and patch it up if there are no weights
  Similar to normalization by adding the weights compute the reciprocal and multiply all elements, this wil ensure that everything adds to 1.
  However in the case of zero weights then we set just a single influence to 1.
  We check in the function for extra's present and if so we use the normalizeSkinWeightsWithExtras rather than the FourWeights version.

#### Returns

`void`

#### Inherited from

[Mesh](Mesh.md).[cleanMatrixWeights](Mesh.md#cleanmatrixweights)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:2366

___

### clone

▸ **clone**(`name?`, `newParent?`, `doNotCloneChildren?`, `clonePhysicsImpostor?`): [`Mesh`](Mesh.md)

Returns a new Mesh object generated from the current mesh properties.
This method must not get confused with createInstance()

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `""` | is a string, the name given to the new mesh |
| `newParent` | [`Nullable`](../modules.md#nullable)[`Node`](Node.md) | `null` | can be any Node object (default `null`) |
| `doNotCloneChildren?` | `boolean` | `undefined` | allows/denies the recursive cloning of the original mesh children if any (default `false`) |
| `clonePhysicsImpostor` | `boolean` | `true` | allows/denies the cloning in the same time of the original mesh `body` used by the physics engine, if any (default `true`) |

#### Returns

[`Mesh`](Mesh.md)

a new mesh

#### Inherited from

[Mesh](Mesh.md).[clone](Mesh.md#clone)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:2746

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

[Mesh](Mesh.md).[computeWorldMatrix](Mesh.md#computeworldmatrix)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:1002

___

### convertToFlatShadedMesh

▸ **convertToFlatShadedMesh**(): [`Mesh`](Mesh.md)

Modify the mesh to get a flat shading rendering.
This means each mesh facet will then have its own normals. Usually new vertices are added in the mesh geometry to get this result.
Warning : the mesh is really modified even if not set originally as updatable and, under the hood, a new VertexBuffer is allocated.

#### Returns

[`Mesh`](Mesh.md)

current mesh

#### Inherited from

[Mesh](Mesh.md).[convertToFlatShadedMesh](Mesh.md#converttoflatshadedmesh)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:2968

___

### convertToUnIndexedMesh

▸ **convertToUnIndexedMesh**(): [`Mesh`](Mesh.md)

This method removes all the mesh indices and add new vertices (duplication) in order to unfold facets into buffers.
In other words, more vertices, no more indices and a single bigger VBO.
The mesh is really modified even if not set originally as updatable. Under the hood, a new VertexBuffer is allocated.

#### Returns

[`Mesh`](Mesh.md)

current mesh

#### Inherited from

[Mesh](Mesh.md).[convertToUnIndexedMesh](Mesh.md#converttounindexedmesh)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:3093

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

[Mesh](Mesh.md).[createAnimationRange](Mesh.md#createanimationrange)

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

[Mesh](Mesh.md).[createInstance](Mesh.md#createinstance)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:3462

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

[Mesh](Mesh.md).[createNormals](Mesh.md#createnormals)

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

[Mesh](Mesh.md).[createOrUpdateSubmeshesOctree](Mesh.md#createorupdatesubmeshesoctree)

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

[Mesh](Mesh.md).[deleteAnimationRange](Mesh.md#deleteanimationrange)

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

[Mesh](Mesh.md).[detachFromBone](Mesh.md#detachfrombone)

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

[Mesh](Mesh.md).[disableEdgesRendering](Mesh.md#disableedgesrendering)

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

[Mesh](Mesh.md).[disableFacetData](Mesh.md#disablefacetdata)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:2505

___

### dispose

▸ **dispose**(`doNotRecurse?`, `disposeMaterialAndTextures?`): `void`

Releases resources associated with this mesh.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `doNotRecurse?` | `boolean` | `undefined` | Set to true to not recurse into each children (recurse into each children by default) |
| `disposeMaterialAndTextures` | `boolean` | `false` | Set to true to also dispose referenced materials and textures (false by default) |

#### Returns

`void`

#### Inherited from

[Mesh](Mesh.md).[dispose](Mesh.md#dispose)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:2755

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

[Mesh](Mesh.md).[enableEdgesRendering](Mesh.md#enableedgesrendering)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:2599

___

### flipFaces

▸ **flipFaces**(`flipNormals?`): [`Mesh`](Mesh.md)

Inverses facet orientations.
Warning : the mesh is really modified even if not set originally as updatable. A new VertexBuffer is created under the hood each call.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `flipNormals` | `boolean` | `false` | will also inverts the normals |

#### Returns

[`Mesh`](Mesh.md)

current mesh

#### Inherited from

[Mesh](Mesh.md).[flipFaces](Mesh.md#flipfaces)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:3163

___

### forceSharedVertices

▸ **forceSharedVertices**(): `void`

Force adjacent facets to share vertices and remove any facets that have all vertices in a line
This will undo any application of covertToFlatShadedMesh
Warning : the mesh is really modified even if not set originally as updatable. A new VertexBuffer is created under the hood each call.

#### Returns

`void`

#### Inherited from

[Mesh](Mesh.md).[forceSharedVertices](Mesh.md#forcesharedvertices)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:3350

___

### freezeNormals

▸ **freezeNormals**(): [`Mesh`](Mesh.md)

This function affects parametric shapes on vertex position update only : ribbons, tubes, etc. It has no effect at all on other shapes. It prevents the mesh normals from being recomputed on next `positions` array update.

#### Returns

[`Mesh`](Mesh.md)

the current mesh

#### Inherited from

[Mesh](Mesh.md).[freezeNormals](Mesh.md#freezenormals)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:1248

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

[Mesh](Mesh.md).[freezeWorldMatrix](Mesh.md#freezeworldmatrix)

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

[Mesh](Mesh.md).[getAbsolutePivotPoint](Mesh.md#getabsolutepivotpoint)

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

[Mesh](Mesh.md).[getAbsolutePivotPointToRef](Mesh.md#getabsolutepivotpointtoref)

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

[Mesh](Mesh.md).[getAbsolutePosition](Mesh.md#getabsoluteposition)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:484

___

### getAnimatables

▸ **getAnimatables**(): [`IAnimatable`](../interfaces/IAnimatable.md)[]

Returns as a new array populated with the mesh material and/or skeleton, if any.

#### Returns

[`IAnimatable`](../interfaces/IAnimatable.md)[]

an array of IAnimatable

#### Inherited from

[Mesh](Mesh.md).[getAnimatables](Mesh.md#getanimatables)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:2628

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

[Mesh](Mesh.md).[getAnimationByName](Mesh.md#getanimationbyname)

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

[Mesh](Mesh.md).[getAnimationRange](Mesh.md#getanimationrange)

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

[Mesh](Mesh.md).[getAnimationRanges](Mesh.md#getanimationranges)

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

[Mesh](Mesh.md).[getBehaviorByName](Mesh.md#getbehaviorbyname)

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

[Mesh](Mesh.md).[getBoundingInfo](Mesh.md#getboundinginfo)

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

[Mesh](Mesh.md).[getChildMeshes](Mesh.md#getchildmeshes)

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

[Mesh](Mesh.md).[getChildMeshes](Mesh.md#getchildmeshes)

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

[Mesh](Mesh.md).[getChildTransformNodes](Mesh.md#getchildtransformnodes)

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

[Mesh](Mesh.md).[getChildren](Mesh.md#getchildren)

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

[Mesh](Mesh.md).[getChildren](Mesh.md#getchildren)

#### Defined in

packages/dev/core/src/node.ts:722

___

### getClassName

▸ **getClassName**(): `string`

"GroundMesh"

#### Returns

`string`

"GroundMesh"

#### Overrides

[Mesh](Mesh.md).[getClassName](Mesh.md#getclassname)

#### Defined in

packages/dev/core/src/Meshes/groundMesh.ts:44

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

[Mesh](Mesh.md).[getClosestFacetAtCoordinates](Mesh.md#getclosestfacetatcoordinates)

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

[Mesh](Mesh.md).[getClosestFacetAtLocalCoordinates](Mesh.md#getclosestfacetatlocalcoordinates)

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

[Mesh](Mesh.md).[getConnectedParticleSystems](Mesh.md#getconnectedparticlesystems)

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

[Mesh](Mesh.md).[getDescendants](Mesh.md#getdescendants)

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

[Mesh](Mesh.md).[getDescendants](Mesh.md#getdescendants)

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

[Mesh](Mesh.md).[getDirection](Mesh.md#getdirection)

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

[Mesh](Mesh.md).[getDirectionToRef](Mesh.md#getdirectiontoref)

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

[Mesh](Mesh.md).[getDistanceToCamera](Mesh.md#getdistancetocamera)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:1316

___

### getEmittedParticleSystems

▸ **getEmittedParticleSystems**(): [`IParticleSystem`](../interfaces/IParticleSystem.md)[]

Returns an array populated with IParticleSystem objects whose the mesh is the emitter

#### Returns

[`IParticleSystem`](../interfaces/IParticleSystem.md)[]

an array of IParticleSystem

#### Inherited from

[Mesh](Mesh.md).[getEmittedParticleSystems](Mesh.md#getemittedparticlesystems)

#### Defined in

packages/dev/core/src/Particles/particleSystemComponent.ts:121

___

### getEngine

▸ **getEngine**(): [`Engine`](Engine.md)

Gets the engine of the node

#### Returns

[`Engine`](Engine.md)

a Engine

#### Inherited from

[Mesh](Mesh.md).[getEngine](Mesh.md#getengine)

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

[Mesh](Mesh.md).[getFacetDataParameters](Mesh.md#getfacetdataparameters)

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

[Mesh](Mesh.md).[getFacetLocalNormals](Mesh.md#getfacetlocalnormals)

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

[Mesh](Mesh.md).[getFacetLocalPartitioning](Mesh.md#getfacetlocalpartitioning)

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

[Mesh](Mesh.md).[getFacetLocalPositions](Mesh.md#getfacetlocalpositions)

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

[Mesh](Mesh.md).[getFacetNormal](Mesh.md#getfacetnormal)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:2358

___

### getFacetNormalToRef

▸ **getFacetNormalToRef**(`i`, `ref`): [`GroundMesh`](GroundMesh.md)

Sets the reference Vector3 with the i-th facet normal in the world system

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_facetdata

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `i` | `number` | defines the facet index |
| `ref` | [`Vector3`](Vector3.md) | defines the target vector |

#### Returns

[`GroundMesh`](GroundMesh.md)

the current mesh

#### Inherited from

[Mesh](Mesh.md).[getFacetNormalToRef](Mesh.md#getfacetnormaltoref)

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

[Mesh](Mesh.md).[getFacetPosition](Mesh.md#getfacetposition)

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

[Mesh](Mesh.md).[getFacetPositionToRef](Mesh.md#getfacetpositiontoref)

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

[Mesh](Mesh.md).[getFacetsAtLocalCoordinates](Mesh.md#getfacetsatlocalcoordinates)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:2385

___

### getHeightAtCoordinates

▸ **getHeightAtCoordinates**(`x`, `z`): `number`

Returns a height (y) value in the World system :
the ground altitude at the coordinates (x, z) expressed in the World system.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | x coordinate |
| `z` | `number` | z coordinate |

#### Returns

`number`

the ground y position if (x, z) are outside the ground surface.

#### Defined in

packages/dev/core/src/Meshes/groundMesh.ts:94

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

[Mesh](Mesh.md).[getHierarchyBoundingVectors](Mesh.md#gethierarchyboundingvectors)

#### Defined in

packages/dev/core/src/node.ts:933

___

### getHierarchyEmittedParticleSystems

▸ **getHierarchyEmittedParticleSystems**(): [`IParticleSystem`](../interfaces/IParticleSystem.md)[]

Returns an array populated with IParticleSystem objects whose the mesh or its children are the emitter

#### Returns

[`IParticleSystem`](../interfaces/IParticleSystem.md)[]

an array of IParticleSystem

#### Inherited from

[Mesh](Mesh.md).[getHierarchyEmittedParticleSystems](Mesh.md#gethierarchyemittedparticlesystems)

#### Defined in

packages/dev/core/src/Particles/particleSystemComponent.ts:127

___

### getIndices

▸ **getIndices**(`copyWhenShared?`, `forceCopy?`): [`Nullable`](../modules.md#nullable)[`IndicesArray`](../modules.md#indicesarray)

Returns an array of integers or a typed array (Int32Array, Uint32Array, Uint16Array) populated with the mesh indices.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `copyWhenShared?` | `boolean` | If true (default false) and and if the mesh geometry is shared among some other meshes, the returned array is a copy of the internal one. |
| `forceCopy?` | `boolean` | defines a boolean indicating that the returned array must be cloned upon returning it |

#### Returns

[`Nullable`](../modules.md#nullable)[`IndicesArray`](../modules.md#indicesarray)

the indices array or an empty array if the mesh has no geometry

#### Inherited from

[Mesh](Mesh.md).[getIndices](Mesh.md#getindices)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:1144

___

### getLOD

▸ **getLOD**(`camera`, `boundingSphere?`): [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

Returns the registered LOD mesh distant from the parameter `camera` position if any, else returns the current mesh.

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_lod

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `camera` | [`Camera`](Camera.md) | defines the camera to use to compute distance |
| `boundingSphere?` | [`BoundingSphere`](BoundingSphere.md) | defines a custom bounding sphere to use instead of the one from this mesh |

#### Returns

[`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

This mesh (for chaining)

#### Inherited from

[Mesh](Mesh.md).[getLOD](Mesh.md#getlod)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:904

___

### getLODLevelAtDistance

▸ **getLODLevelAtDistance**(`distance`): [`Nullable`](../modules.md#nullable)[`Mesh`](Mesh.md)

Returns the LOD level mesh at the passed distance or null if not found.

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_lod

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `distance` | `number` | The distance from the center of the object to show this level |

#### Returns

[`Nullable`](../modules.md#nullable)[`Mesh`](Mesh.md)

a Mesh or `null`

#### Inherited from

[Mesh](Mesh.md).[getLODLevelAtDistance](Mesh.md#getlodlevelatdistance)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:864

___

### getLODLevels

▸ **getLODLevels**(): [`MeshLODLevel`](MeshLODLevel.md)[]

Gets the list of MeshLODLevel associated with the current mesh

#### Returns

[`MeshLODLevel`](MeshLODLevel.md)[]

an array of MeshLODLevel

#### Inherited from

[Mesh](Mesh.md).[getLODLevels](Mesh.md#getlodlevels)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:814

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

[Mesh](Mesh.md).[getMaterialForRenderPass](Mesh.md#getmaterialforrenderpass)

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

[Mesh](Mesh.md).[getMeshUniformBuffer](Mesh.md#getmeshuniformbuffer)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:857

___

### getNormalAtCoordinates

▸ **getNormalAtCoordinates**(`x`, `z`): [`Vector3`](Vector3.md)

Returns a normalized vector (Vector3) orthogonal to the ground
at the ground coordinates (x, z) expressed in the World system.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | x coordinate |
| `z` | `number` | z coordinate |

#### Returns

[`Vector3`](Vector3.md)

Vector3(0.0, 1.0, 0.0) if (x, z) are outside the ground surface.

#### Defined in

packages/dev/core/src/Meshes/groundMesh.ts:123

___

### getNormalAtCoordinatesToRef

▸ **getNormalAtCoordinatesToRef**(`x`, `z`, `ref`): [`GroundMesh`](GroundMesh.md)

Updates the Vector3 passed a reference with a normalized vector orthogonal to the ground
at the ground coordinates (x, z) expressed in the World system.
Doesn't update the reference Vector3 if (x, z) are outside the ground surface.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | x coordinate |
| `z` | `number` | z coordinate |
| `ref` | [`Vector3`](Vector3.md) | vector to store the result |

#### Returns

[`GroundMesh`](GroundMesh.md)

the GroundMesh.

#### Defined in

packages/dev/core/src/Meshes/groundMesh.ts:138

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

[Mesh](Mesh.md).[getNormalsData](Mesh.md#getnormalsdata)

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

[Mesh](Mesh.md).[getPhysicsImpostor](Mesh.md#getphysicsimpostor)

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

[Mesh](Mesh.md).[getPivotMatrix](Mesh.md#getpivotmatrix)

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

[Mesh](Mesh.md).[getPivotPoint](Mesh.md#getpivotpoint)

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

[Mesh](Mesh.md).[getPivotPointToRef](Mesh.md#getpivotpointtoref)

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

[Mesh](Mesh.md).[getPoseMatrix](Mesh.md#getposematrix)

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

[Mesh](Mesh.md).[getPositionData](Mesh.md#getpositiondata)

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

[Mesh](Mesh.md).[getPositionExpressedInLocalSpace](Mesh.md#getpositionexpressedinlocalspace)

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

[Mesh](Mesh.md).[getPositionInCameraSpace](Mesh.md#getpositionincameraspace)

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

[Mesh](Mesh.md).[getScene](Mesh.md#getscene)

#### Defined in

packages/dev/core/src/node.ts:344

___

### getTotalIndices

▸ **getTotalIndices**(): `number`

Returns a positive integer : the total number of indices in this mesh geometry.

#### Returns

`number`

the numner of indices or zero if the mesh has no geometry.

#### Inherited from

[Mesh](Mesh.md).[getTotalIndices](Mesh.md#gettotalindices)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:1131

___

### getTotalVertices

▸ **getTotalVertices**(): `number`

Returns the total number of vertices within the mesh geometry or zero if the mesh has no geometry.

#### Returns

`number`

the total number of vertices

#### Inherited from

[Mesh](Mesh.md).[getTotalVertices](Mesh.md#gettotalvertices)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:983

___

### getVertexBuffer

▸ **getVertexBuffer**(`kind`): [`Nullable`](../modules.md#nullable)[`VertexBuffer`](VertexBuffer.md)

Returns the mesh VertexBuffer object from the requested `kind`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `kind` | `string` | defines which buffer to read from (positions, indices, normals, etc). Possible `kind` values :  - VertexBuffer.PositionKind  - VertexBuffer.NormalKind  - VertexBuffer.UVKind  - VertexBuffer.UV2Kind  - VertexBuffer.UV3Kind  - VertexBuffer.UV4Kind  - VertexBuffer.UV5Kind  - VertexBuffer.UV6Kind  - VertexBuffer.ColorKind  - VertexBuffer.MatricesIndicesKind  - VertexBuffer.MatricesIndicesExtraKind  - VertexBuffer.MatricesWeightsKind  - VertexBuffer.MatricesWeightsExtraKind |

#### Returns

[`Nullable`](../modules.md#nullable)[`VertexBuffer`](VertexBuffer.md)

a FloatArray or null if the mesh has no vertex buffer for this kind.

#### Inherited from

[Mesh](Mesh.md).[getVertexBuffer](Mesh.md#getvertexbuffer)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:1041

___

### getVerticesData

▸ **getVerticesData**(`kind`, `copyWhenShared?`, `forceCopy?`): [`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray)

Returns the content of an associated vertex buffer

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `kind` | `string` | defines which buffer to read from (positions, indices, normals, etc). Possible `kind` values :  - VertexBuffer.PositionKind  - VertexBuffer.UVKind  - VertexBuffer.UV2Kind  - VertexBuffer.UV3Kind  - VertexBuffer.UV4Kind  - VertexBuffer.UV5Kind  - VertexBuffer.UV6Kind  - VertexBuffer.ColorKind  - VertexBuffer.MatricesIndicesKind  - VertexBuffer.MatricesIndicesExtraKind  - VertexBuffer.MatricesWeightsKind  - VertexBuffer.MatricesWeightsExtraKind |
| `copyWhenShared?` | `boolean` | defines a boolean indicating that if the mesh geometry is shared among some other meshes, the returned array is a copy of the internal one |
| `forceCopy?` | `boolean` | defines a boolean forcing the copy of the buffer no matter what the value of copyWhenShared is |

#### Returns

[`Nullable`](../modules.md#nullable)[`FloatArray`](../modules.md#floatarray)

a FloatArray or null if the mesh has no geometry or no vertex buffer for this kind.

#### Inherited from

[Mesh](Mesh.md).[getVerticesData](Mesh.md#getverticesdata)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:1009

___

### getVerticesDataKinds

▸ **getVerticesDataKinds**(): `string`[]

Returns a string which contains the list of existing `kinds` of Vertex Data associated with this mesh.

#### Returns

`string`[]

an array of strings

#### Inherited from

[Mesh](Mesh.md).[getVerticesDataKinds](Mesh.md#getverticesdatakinds)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:1108

___

### getWorldMatrix

▸ **getWorldMatrix**(): [`Matrix`](Matrix.md)

Gets the current world matrix

#### Returns

[`Matrix`](Matrix.md)

a Matrix

#### Inherited from

[Mesh](Mesh.md).[getWorldMatrix](Mesh.md#getworldmatrix)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1307

___

### increaseVertices

▸ **increaseVertices**(`numberPerEdge?`): `void`

Increase the number of facets and hence vertices in a mesh
Vertex normals are interpolated from existing vertex normals
Warning : the mesh is really modified even if not set originally as updatable. A new VertexBuffer is created under the hood each call.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `numberPerEdge` | `number` | `1` | the number of new vertices to add to each edge of a facet, optional default 1 |

#### Returns

`void`

#### Inherited from

[Mesh](Mesh.md).[increaseVertices](Mesh.md#increasevertices)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:3192

___

### instantiateHierarchy

▸ **instantiateHierarchy**(`newParent?`, `options?`, `onNewNodeCreated?`): [`Nullable`](../modules.md#nullable)[`TransformNode`](TransformNode.md)

Instantiate (when possible) or clone that node with its hierarchy

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `newParent` | [`Nullable`](../modules.md#nullable)[`TransformNode`](TransformNode.md) | `null` | defines the new parent to use for the instance (or clone) |
| `options?` | `Object` | `undefined` | defines options to configure how copy is done |
| `options.doNotInstantiate` | `boolean` \| (`node`: [`TransformNode`](TransformNode.md)) => `boolean` | `undefined` | - |
| `onNewNodeCreated?` | (`source`: [`TransformNode`](TransformNode.md), `clone`: [`TransformNode`](TransformNode.md)) => `void` | `undefined` | defines an option callback to call when a clone or an instance is created |

#### Returns

[`Nullable`](../modules.md#nullable)[`TransformNode`](TransformNode.md)

an instance (or a clone) of the current node with its hierarchy

#### Inherited from

[Mesh](Mesh.md).[instantiateHierarchy](Mesh.md#instantiatehierarchy)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:720

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

[Mesh](Mesh.md).[intersects](Mesh.md#intersects)

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

[Mesh](Mesh.md).[intersectsMesh](Mesh.md#intersectsmesh)

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

[Mesh](Mesh.md).[intersectsPoint](Mesh.md#intersectspoint)

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

[Mesh](Mesh.md).[isCompletelyInFrustum](Mesh.md#iscompletelyinfrustum)

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

[Mesh](Mesh.md).[isDescendantOf](Mesh.md#isdescendantof)

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

[Mesh](Mesh.md).[isDisposed](Mesh.md#isdisposed)

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

[Mesh](Mesh.md).[isEnabled](Mesh.md#isenabled)

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

[Mesh](Mesh.md).[isInFrustum](Mesh.md#isinfrustum)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:2584

___

### isReady

▸ **isReady**(`completeCheck?`, `forceInstanceSupport?`): `boolean`

Determine if the current mesh is ready to be rendered

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `completeCheck` | `boolean` | `false` | defines if a complete check (including materials and lights) has to be done (false by default) |
| `forceInstanceSupport` | `boolean` | `false` | will check if the mesh will be ready when used with instances (false by default) |

#### Returns

`boolean`

true if all associated assets are ready (material, textures, shaders)

#### Inherited from

[Mesh](Mesh.md).[isReady](Mesh.md#isready)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:1161

___

### isUsingPivotMatrix

▸ **isUsingPivotMatrix**(): `boolean`

return true if a pivot has been set

#### Returns

`boolean`

true if a pivot matrix is used

#### Inherited from

[Mesh](Mesh.md).[isUsingPivotMatrix](Mesh.md#isusingpivotmatrix)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:203

___

### isVertexBufferUpdatable

▸ **isVertexBufferUpdatable**(`kind`): `boolean`

Returns a boolean defining if the vertex data for the requested `kind` is updatable.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `kind` | `string` | defines which buffer to check (positions, indices, normals, etc). Possible `kind` values :  - VertexBuffer.PositionKind  - VertexBuffer.UVKind  - VertexBuffer.UV2Kind  - VertexBuffer.UV3Kind  - VertexBuffer.UV4Kind  - VertexBuffer.UV5Kind  - VertexBuffer.UV6Kind  - VertexBuffer.ColorKind  - VertexBuffer.MatricesIndicesKind  - VertexBuffer.MatricesIndicesExtraKind  - VertexBuffer.MatricesWeightsKind  - VertexBuffer.MatricesWeightsExtraKind |

#### Returns

`boolean`

a boolean

#### Inherited from

[Mesh](Mesh.md).[isVertexBufferUpdatable](Mesh.md#isvertexbufferupdatable)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:1094

___

### isVerticesDataPresent

▸ **isVerticesDataPresent**(`kind`): `boolean`

Tests if a specific vertex buffer is associated with this mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `kind` | `string` | defines which buffer to check (positions, indices, normals, etc). Possible `kind` values :  - VertexBuffer.PositionKind  - VertexBuffer.NormalKind  - VertexBuffer.UVKind  - VertexBuffer.UV2Kind  - VertexBuffer.UV3Kind  - VertexBuffer.UV4Kind  - VertexBuffer.UV5Kind  - VertexBuffer.UV6Kind  - VertexBuffer.ColorKind  - VertexBuffer.MatricesIndicesKind  - VertexBuffer.MatricesIndicesExtraKind  - VertexBuffer.MatricesWeightsKind  - VertexBuffer.MatricesWeightsExtraKind |

#### Returns

`boolean`

a boolean

#### Inherited from

[Mesh](Mesh.md).[isVerticesDataPresent](Mesh.md#isverticesdatapresent)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:1067

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

[Mesh](Mesh.md).[locallyTranslate](Mesh.md#locallytranslate)

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

[Mesh](Mesh.md).[lookAt](Mesh.md#lookat)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:571

___

### makeGeometryUnique

▸ **makeGeometryUnique**(): [`Mesh`](Mesh.md)

Creates a un-shared specific occurence of the geometry for the mesh.

#### Returns

[`Mesh`](Mesh.md)

the current mesh

#### Inherited from

[Mesh](Mesh.md).[makeGeometryUnique](Mesh.md#makegeometryunique)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:1601

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

[Mesh](Mesh.md).[markAsDirty](Mesh.md#markasdirty)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1049

___

### markVerticesDataAsUpdatable

▸ **markVerticesDataAsUpdatable**(`kind`, `updatable?`): `void`

Flags an associated vertex buffer as updatable

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `kind` | `string` | `undefined` | defines which buffer to use (positions, indices, normals, etc). Possible `kind` values :  - VertexBuffer.PositionKind  - VertexBuffer.UVKind  - VertexBuffer.UV2Kind  - VertexBuffer.UV3Kind  - VertexBuffer.UV4Kind  - VertexBuffer.UV5Kind  - VertexBuffer.UV6Kind  - VertexBuffer.ColorKind  - VertexBuffer.MatricesIndicesKind  - VertexBuffer.MatricesIndicesExtraKind  - VertexBuffer.MatricesWeightsKind  - VertexBuffer.MatricesWeightsExtraKind |
| `updatable` | `boolean` | `true` | defines if the updated vertex buffer must be flagged as updatable |

#### Returns

`void`

#### Inherited from

[Mesh](Mesh.md).[markVerticesDataAsUpdatable](Mesh.md#markverticesdataasupdatable)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:1509

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

[Mesh](Mesh.md).[movePOV](Mesh.md#movepov)

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

[Mesh](Mesh.md).[moveWithCollisions](Mesh.md#movewithcollisions)

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

[Mesh](Mesh.md).[normalizeToUnitCube](Mesh.md#normalizetounitcube)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1253

___

### optimize

▸ **optimize**(`chunksCount`, `octreeBlocksSize?`): `void`

This function will update an octree to help to select the right submeshes for rendering, picking and collision computations.
Please note that you must have a decent number of submeshes to get performance improvements when using an octree

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `chunksCount` | `number` | `undefined` | the number of subdivisions for x and y |
| `octreeBlocksSize` | `number` | `32` | (Default: 32) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Meshes/groundMesh.ts:75

___

### optimizeIndices

▸ **optimizeIndices**(`successCallback?`): [`Mesh`](Mesh.md)

Optimization of the mesh's indices, in case a mesh has duplicated vertices.
The function will only reorder the indices and will not remove unused vertices to avoid problems with submeshes.
This should be used together with the simplification to avoid disappearing triangles.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `successCallback?` | (`mesh?`: [`Mesh`](Mesh.md)) => `void` | an optional success callback to be called after the optimization finished. |

#### Returns

[`Mesh`](Mesh.md)

the current mesh

#### Inherited from

[Mesh](Mesh.md).[optimizeIndices](Mesh.md#optimizeindices)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:3486

___

### refreshBoundingInfo

▸ **refreshBoundingInfo**(`applySkeleton?`, `applyMorph?`): [`Mesh`](Mesh.md)

This method recomputes and sets a new BoundingInfo to the mesh unless it is locked.
This means the mesh underlying bounding box and sphere are recomputed.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `applySkeleton` | `boolean` | `false` | defines whether to apply the skeleton before computing the bounding info |
| `applyMorph` | `boolean` | `false` | defines whether to apply the morph target before computing the bounding info |

#### Returns

[`Mesh`](Mesh.md)

the current mesh

#### Inherited from

[Mesh](Mesh.md).[refreshBoundingInfo](Mesh.md#refreshboundinginfo)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:1346

___

### registerAfterRender

▸ **registerAfterRender**(`func`): [`Mesh`](Mesh.md)

Registers for this mesh a javascript function called just after the rendering is complete

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `func` | (`mesh`: [`AbstractMesh`](AbstractMesh.md)) => `void` | defines the function to call after rendering this mesh |

#### Returns

[`Mesh`](Mesh.md)

the current mesh

#### Inherited from

[Mesh](Mesh.md).[registerAfterRender](Mesh.md#registerafterrender)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:1769

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

[Mesh](Mesh.md).[registerAfterWorldMatrixUpdate](Mesh.md#registerafterworldmatrixupdate)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:1283

___

### registerBeforeRender

▸ **registerBeforeRender**(`func`): [`Mesh`](Mesh.md)

Registers for this mesh a javascript function called just before the rendering process

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `func` | (`mesh`: [`AbstractMesh`](AbstractMesh.md)) => `void` | defines the function to call before rendering this mesh |

#### Returns

[`Mesh`](Mesh.md)

the current mesh

#### Inherited from

[Mesh](Mesh.md).[registerBeforeRender](Mesh.md#registerbeforerender)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:1749

___

### registerInstancedBuffer

▸ **registerInstancedBuffer**(`kind`, `stride`): `void`

Register a custom buffer that will be instanced

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_instances#custom-buffers

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `kind` | `string` | defines the buffer kind |
| `stride` | `number` | defines the stride in floats |

#### Returns

`void`

#### Inherited from

[Mesh](Mesh.md).[registerInstancedBuffer](Mesh.md#registerinstancedbuffer)

#### Defined in

packages/dev/core/src/Meshes/instancedMesh.ts:565

___

### releaseSubMeshes

▸ **releaseSubMeshes**(): [`AbstractMesh`](AbstractMesh.md)

Disposes all the submeshes of the current meshnp

#### Returns

[`AbstractMesh`](AbstractMesh.md)

the current mesh

#### Inherited from

[Mesh](Mesh.md).[releaseSubMeshes](Mesh.md#releasesubmeshes)

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

[Mesh](Mesh.md).[removeBehavior](Mesh.md#removebehavior)

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

[Mesh](Mesh.md).[removeChild](Mesh.md#removechild)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:2152

___

### removeLODLevel

▸ **removeLODLevel**(`mesh`): [`Mesh`](Mesh.md)

Remove a mesh from the LOD array

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_lod

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`Mesh`](Mesh.md) | defines the mesh to be removed |

#### Returns

[`Mesh`](Mesh.md)

This mesh (for chaining)

#### Inherited from

[Mesh](Mesh.md).[removeLODLevel](Mesh.md#removelodlevel)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:882

___

### removeVerticesData

▸ **removeVerticesData**(`kind`): `void`

Delete a vertex buffer associated with this mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `kind` | `string` | defines which buffer to delete (positions, indices, normals, etc). Possible `kind` values :  - VertexBuffer.PositionKind  - VertexBuffer.UVKind  - VertexBuffer.UV2Kind  - VertexBuffer.UV3Kind  - VertexBuffer.UV4Kind  - VertexBuffer.UV5Kind  - VertexBuffer.UV6Kind  - VertexBuffer.ColorKind  - VertexBuffer.MatricesIndicesKind  - VertexBuffer.MatricesIndicesExtraKind  - VertexBuffer.MatricesWeightsKind  - VertexBuffer.MatricesWeightsExtraKind |

#### Returns

`void`

#### Inherited from

[Mesh](Mesh.md).[removeVerticesData](Mesh.md#removeverticesdata)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:1484

___

### render

▸ **render**(`subMesh`, `enableAlphaMode`, `effectiveMeshReplacement?`): [`Mesh`](Mesh.md)

Triggers the draw call for the mesh. Usually, you don't need to call this method by your own because the mesh rendering is handled by the scene rendering manager

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `subMesh` | [`SubMesh`](SubMesh.md) | defines the subMesh to render |
| `enableAlphaMode` | `boolean` | defines if alpha mode can be changed |
| `effectiveMeshReplacement?` | [`AbstractMesh`](AbstractMesh.md) | defines an optional mesh used to provide info for the rendering |

#### Returns

[`Mesh`](Mesh.md)

the current mesh

#### Inherited from

[Mesh](Mesh.md).[render](Mesh.md#render)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:2172

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

[Mesh](Mesh.md).[resetDrawCache](Mesh.md#resetdrawcache)

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

[Mesh](Mesh.md).[resetLocalMatrix](Mesh.md#resetlocalmatrix)

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

[Mesh](Mesh.md).[rotate](Mesh.md#rotate)

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

[Mesh](Mesh.md).[rotateAround](Mesh.md#rotatearound)

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

[Mesh](Mesh.md).[rotatePOV](Mesh.md#rotatepov)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:1389

___

### serialize

▸ **serialize**(`serializationObject`): `void`

Serializes this ground mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `serializationObject` | `any` | object to write serialization to |

#### Returns

`void`

#### Overrides

[Mesh](Mesh.md).[serialize](Mesh.md#serialize)

#### Defined in

packages/dev/core/src/Meshes/groundMesh.ts:288

___

### serializeAnimationRanges

▸ **serializeAnimationRanges**(): `any`

Serialize animation ranges into a JSON compatible object

#### Returns

`any`

serialization object

#### Inherited from

[Mesh](Mesh.md).[serializeAnimationRanges](Mesh.md#serializeanimationranges)

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

[Mesh](Mesh.md).[setAbsolutePosition](Mesh.md#setabsoluteposition)

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

[Mesh](Mesh.md).[setBoundingInfo](Mesh.md#setboundinginfo)

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

[Mesh](Mesh.md).[setDirection](Mesh.md#setdirection)

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

[Mesh](Mesh.md).[setEnabled](Mesh.md#setenabled)

#### Defined in

packages/dev/core/src/node.ts:596

___

### setIndices

▸ **setIndices**(`indices`, `totalVertices?`, `updatable?`): [`AbstractMesh`](AbstractMesh.md)

Set the index buffer of this mesh

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `indices` | [`IndicesArray`](../modules.md#indicesarray) | `undefined` | defines the source data |
| `totalVertices` | [`Nullable`](../modules.md#nullable)`number` | `null` | defines the total number of vertices referenced by this index data (can be null) |
| `updatable` | `boolean` | `false` | defines if the updated index buffer must be flagged as updatable (default is false) |

#### Returns

[`AbstractMesh`](AbstractMesh.md)

the current mesh

#### Inherited from

[Mesh](Mesh.md).[setIndices](Mesh.md#setindices)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:1624

___

### setMaterialById

▸ **setMaterialById**(`id`): [`Mesh`](Mesh.md)

Sets the mesh material by the material or multiMaterial `id` property

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | is a string identifying the material or the multiMaterial |

#### Returns

[`Mesh`](Mesh.md)

the current mesh

#### Inherited from

[Mesh](Mesh.md).[setMaterialById](Mesh.md#setmaterialbyid)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:2603

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

[Mesh](Mesh.md).[setMaterialForRenderPass](Mesh.md#setmaterialforrenderpass)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:499

___

### setNormalsForCPUSkinning

▸ **setNormalsForCPUSkinning**(): [`Nullable`](../modules.md#nullable)`Float32Array`

Prepare internal normal array for software CPU skinning

#### Returns

[`Nullable`](../modules.md#nullable)`Float32Array`

original normals used for CPU skinning. Useful for integrating Morphing with skeletons in same mesh.

#### Inherited from

[Mesh](Mesh.md).[setNormalsForCPUSkinning](Mesh.md#setnormalsforcpuskinning)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:4224

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

[Mesh](Mesh.md).[setParent](Mesh.md#setparent)

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

[Mesh](Mesh.md).[setPhysicsLinkWith](Mesh.md#setphysicslinkwith)

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

[Mesh](Mesh.md).[setPivotMatrix](Mesh.md#setpivotmatrix)

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

[Mesh](Mesh.md).[setPivotPoint](Mesh.md#setpivotpoint)

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

[Mesh](Mesh.md).[setPositionWithLocalVector](Mesh.md#setpositionwithlocalvector)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:532

___

### setPositionsForCPUSkinning

▸ **setPositionsForCPUSkinning**(): [`Nullable`](../modules.md#nullable)`Float32Array`

Prepare internal position array for software CPU skinning

#### Returns

[`Nullable`](../modules.md#nullable)`Float32Array`

original positions used for CPU skinning. Useful for integrating Morphing with skeletons in same mesh

#### Inherited from

[Mesh](Mesh.md).[setPositionsForCPUSkinning](Mesh.md#setpositionsforcpuskinning)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:4203

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

[Mesh](Mesh.md).[setPreTransformMatrix](Mesh.md#setpretransformmatrix)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:371

___

### setVerticesBuffer

▸ **setVerticesBuffer**(`buffer`, `disposeExistingBuffer?`): [`Mesh`](Mesh.md)

Sets the mesh global Vertex Buffer

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `buffer` | [`VertexBuffer`](VertexBuffer.md) | `undefined` | defines the buffer to use |
| `disposeExistingBuffer` | `boolean` | `true` | disposes the existing buffer, if any (default: true) |

#### Returns

[`Mesh`](Mesh.md)

the current mesh

#### Inherited from

[Mesh](Mesh.md).[setVerticesBuffer](Mesh.md#setverticesbuffer)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:1525

___

### setVerticesData

▸ **setVerticesData**(`kind`, `data`, `updatable?`, `stride?`): [`AbstractMesh`](AbstractMesh.md)

Copy a FloatArray into a specific associated vertex buffer

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `kind` | `string` | `undefined` | defines which buffer to write to (positions, indices, normals, etc). Possible `kind` values :  - VertexBuffer.PositionKind  - VertexBuffer.UVKind  - VertexBuffer.UV2Kind  - VertexBuffer.UV3Kind  - VertexBuffer.UV4Kind  - VertexBuffer.UV5Kind  - VertexBuffer.UV6Kind  - VertexBuffer.ColorKind  - VertexBuffer.MatricesIndicesKind  - VertexBuffer.MatricesIndicesExtraKind  - VertexBuffer.MatricesWeightsKind  - VertexBuffer.MatricesWeightsExtraKind |
| `data` | [`FloatArray`](../modules.md#floatarray) | `undefined` | defines the data source |
| `updatable` | `boolean` | `false` | defines if the updated vertex buffer must be flagged as updatable |
| `stride?` | `number` | `undefined` | defines the data stride size (can be null) |

#### Returns

[`AbstractMesh`](AbstractMesh.md)

the current mesh

#### Inherited from

[Mesh](Mesh.md).[setVerticesData](Mesh.md#setverticesdata)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:1454

___

### simplify

▸ **simplify**(`settings`, `parallelProcessing?`, `simplificationType?`, `successCallback?`): [`Mesh`](Mesh.md)

Simplify the mesh according to the given array of settings.
Function will return immediately and will simplify async

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `settings` | [`ISimplificationSettings`](../interfaces/ISimplificationSettings.md)[] | a collection of simplification settings |
| `parallelProcessing?` | `boolean` | should all levels calculate parallel or one after the other |
| `simplificationType?` | [`QUADRATIC`](../enums/SimplificationType.md#quadratic) | the type of simplification to run |
| `successCallback?` | (`mesh?`: [`Mesh`](Mesh.md), `submeshIndex?`: `number`) => `void` | optional success callback to be called after the simplification finished processing all settings |

#### Returns

[`Mesh`](Mesh.md)

the current mesh

#### Inherited from

[Mesh](Mesh.md).[simplify](Mesh.md#simplify)

#### Defined in

packages/dev/core/src/Meshes/meshSimplificationSceneComponent.ts:50

___

### subdivide

▸ **subdivide**(`count`): `void`

This function will subdivide the mesh into multiple submeshes

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `count` | `number` | defines the expected number of submeshes |

#### Returns

`void`

#### Inherited from

[Mesh](Mesh.md).[subdivide](Mesh.md#subdivide)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:1406

___

### synchronizeInstances

▸ **synchronizeInstances**(): [`Mesh`](Mesh.md)

Synchronises all the mesh instance submeshes to the current mesh submeshes, if any.
After this call, all the mesh instances have the same submeshes than the current mesh.

#### Returns

[`Mesh`](Mesh.md)

the current mesh

#### Inherited from

[Mesh](Mesh.md).[synchronizeInstances](Mesh.md#synchronizeinstances)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:3471

___

### thinInstanceAdd

▸ **thinInstanceAdd**(`matrix`, `refresh?`): `number`

Creates a new thin instance

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `matrix` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) \| [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md)[] | the matrix or array of matrices (position, rotation, scale) of the thin instance(s) to create |
| `refresh?` | `boolean` | true to refresh the underlying gpu buffer (default: true). If you do multiple calls to this method in a row, set refresh to true only for the last call to save performance |

#### Returns

`number`

the thin instance index number. If you pass an array of matrices, other instance indexes are index+1, index+2, etc

#### Inherited from

[Mesh](Mesh.md).[thinInstanceAdd](Mesh.md#thininstanceadd)

#### Defined in

packages/dev/core/src/Meshes/thinInstanceMesh.ts:19

___

### thinInstanceAddSelf

▸ **thinInstanceAddSelf**(`refresh?`): `number`

Adds the transformation (matrix) of the current mesh as a thin instance

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `refresh?` | `boolean` | true to refresh the underlying gpu buffer (default: true). If you do multiple calls to this method in a row, set refresh to true only for the last call to save performance |

#### Returns

`number`

the thin instance index number

#### Inherited from

[Mesh](Mesh.md).[thinInstanceAddSelf](Mesh.md#thininstanceaddself)

#### Defined in

packages/dev/core/src/Meshes/thinInstanceMesh.ts:26

___

### thinInstanceBufferUpdated

▸ **thinInstanceBufferUpdated**(`kind`): `void`

Synchronize the gpu buffers with a thin instance buffer. Call this method if you update later on the buffers passed to thinInstanceSetBuffer

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `kind` | `string` | name of the attribute to update. Use "matrix" to update the buffer of matrices |

#### Returns

`void`

#### Inherited from

[Mesh](Mesh.md).[thinInstanceBufferUpdated](Mesh.md#thininstancebufferupdated)

#### Defined in

packages/dev/core/src/Meshes/thinInstanceMesh.ts:76

___

### thinInstanceGetWorldMatrices

▸ **thinInstanceGetWorldMatrices**(): [`Matrix`](Matrix.md)[]

Gets the list of world matrices

#### Returns

[`Matrix`](Matrix.md)[]

an array containing all the world matrices from the thin instances

#### Inherited from

[Mesh](Mesh.md).[thinInstanceGetWorldMatrices](Mesh.md#thininstancegetworldmatrices)

#### Defined in

packages/dev/core/src/Meshes/thinInstanceMesh.ts:70

___

### thinInstancePartialBufferUpdate

▸ **thinInstancePartialBufferUpdate**(`kind`, `data`, `offset`): `void`

Applies a partial update to a buffer directly on the GPU
Note that the buffer located on the CPU is NOT updated! It's up to you to update it (or not) with the same data you pass to this method

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `kind` | `string` | name of the attribute to update. Use "matrix" to update the buffer of matrices |
| `data` | `Float32Array` | the data to set in the GPU buffer |
| `offset` | `number` | the offset in the GPU buffer where to update the data |

#### Returns

`void`

#### Inherited from

[Mesh](Mesh.md).[thinInstancePartialBufferUpdate](Mesh.md#thininstancepartialbufferupdate)

#### Defined in

packages/dev/core/src/Meshes/thinInstanceMesh.ts:85

___

### thinInstanceRefreshBoundingInfo

▸ **thinInstanceRefreshBoundingInfo**(`forceRefreshParentInfo?`, `applySkeleton?`, `applyMorph?`): `void`

Refreshes the bounding info, taking into account all the thin instances defined

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `forceRefreshParentInfo?` | `boolean` | true to force recomputing the mesh bounding info and use it to compute the aggregated bounding info |
| `applySkeleton?` | `boolean` | defines whether to apply the skeleton before computing the bounding info |
| `applyMorph?` | `boolean` | defines whether to apply the morph target before computing the bounding info |

#### Returns

`void`

#### Inherited from

[Mesh](Mesh.md).[thinInstanceRefreshBoundingInfo](Mesh.md#thininstancerefreshboundinginfo)

#### Defined in

packages/dev/core/src/Meshes/thinInstanceMesh.ts:93

___

### thinInstanceRegisterAttribute

▸ **thinInstanceRegisterAttribute**(`kind`, `stride`): `void`

Registers a custom attribute to be used with thin instances

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `kind` | `string` | name of the attribute |
| `stride` | `number` | size in floats of the attribute |

#### Returns

`void`

#### Inherited from

[Mesh](Mesh.md).[thinInstanceRegisterAttribute](Mesh.md#thininstanceregisterattribute)

#### Defined in

packages/dev/core/src/Meshes/thinInstanceMesh.ts:33

___

### thinInstanceSetAttributeAt

▸ **thinInstanceSetAttributeAt**(`kind`, `index`, `value`, `refresh?`): `void`

Sets the value of a custom attribute for a thin instance

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `kind` | `string` | name of the attribute |
| `index` | `number` | index of the thin instance |
| `value` | `number`[] | value to set |
| `refresh?` | `boolean` | true to refresh the underlying gpu buffer (default: true). If you do multiple calls to this method in a row, set refresh to true only for the last call to save performance |

#### Returns

`void`

#### Inherited from

[Mesh](Mesh.md).[thinInstanceSetAttributeAt](Mesh.md#thininstancesetattributeat)

#### Defined in

packages/dev/core/src/Meshes/thinInstanceMesh.ts:50

___

### thinInstanceSetBuffer

▸ **thinInstanceSetBuffer**(`kind`, `buffer`, `stride?`, `staticBuffer?`): `void`

Sets a buffer to be used with thin instances. This method is a faster way to setup multiple instances than calling thinInstanceAdd repeatedly

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `kind` | `string` | name of the attribute. Use "matrix" to setup the buffer of matrices |
| `buffer` | [`Nullable`](../modules.md#nullable)`Float32Array` | buffer to set |
| `stride?` | `number` | size in floats of each value of the buffer |
| `staticBuffer?` | `boolean` | indicates that the buffer is static, so that you won't change it after it is set (better performances - false by default) |

#### Returns

`void`

#### Inherited from

[Mesh](Mesh.md).[thinInstanceSetBuffer](Mesh.md#thininstancesetbuffer)

#### Defined in

packages/dev/core/src/Meshes/thinInstanceMesh.ts:64

___

### thinInstanceSetMatrixAt

▸ **thinInstanceSetMatrixAt**(`index`, `matrix`, `refresh?`): `void`

Sets the matrix of a thin instance

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | index of the thin instance |
| `matrix` | [`DeepImmutableObject`](../modules.md#deepimmutableobject)[`Matrix`](Matrix.md) | matrix to set |
| `refresh?` | `boolean` | true to refresh the underlying gpu buffer (default: true). If you do multiple calls to this method in a row, set refresh to true only for the last call to save performance |

#### Returns

`void`

#### Inherited from

[Mesh](Mesh.md).[thinInstanceSetMatrixAt](Mesh.md#thininstancesetmatrixat)

#### Defined in

packages/dev/core/src/Meshes/thinInstanceMesh.ts:41

___

### toLeftHanded

▸ **toLeftHanded**(): [`Mesh`](Mesh.md)

Invert the geometry to move from a right handed system to a left handed one.

#### Returns

[`Mesh`](Mesh.md)

the current mesh

#### Inherited from

[Mesh](Mesh.md).[toLeftHanded](Mesh.md#tolefthanded)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:1658

___

### toString

▸ **toString**(`fullDetails?`): `string`

Returns a description of this mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fullDetails?` | `boolean` | define if full details about this mesh must be used |

#### Returns

`string`

a descriptive string representing this mesh

#### Inherited from

[Mesh](Mesh.md).[toString](Mesh.md#tostring)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:768

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

[Mesh](Mesh.md).[transferToEffect](Mesh.md#transfertoeffect)

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

[Mesh](Mesh.md).[translate](Mesh.md#translate)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:945

___

### unfreezeNormals

▸ **unfreezeNormals**(): [`Mesh`](Mesh.md)

This function affects parametric shapes on vertex position update only : ribbons, tubes, etc. It has no effect at all on other shapes. It reactivates the mesh normals computation if it was previously frozen

#### Returns

[`Mesh`](Mesh.md)

the current mesh

#### Inherited from

[Mesh](Mesh.md).[unfreezeNormals](Mesh.md#unfreezenormals)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:1257

___

### unfreezeWorldMatrix

▸ **unfreezeWorldMatrix**(): [`GroundMesh`](GroundMesh.md)

Allows back the World matrix computation.

#### Returns

[`GroundMesh`](GroundMesh.md)

the TransformNode.

#### Inherited from

[Mesh](Mesh.md).[unfreezeWorldMatrix](Mesh.md#unfreezeworldmatrix)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:467

___

### unregisterAfterRender

▸ **unregisterAfterRender**(`func`): [`Mesh`](Mesh.md)

Disposes a previously registered javascript function called after the rendering.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `func` | (`mesh`: [`AbstractMesh`](AbstractMesh.md)) => `void` | defines the function to remove |

#### Returns

[`Mesh`](Mesh.md)

the current mesh

#### Inherited from

[Mesh](Mesh.md).[unregisterAfterRender](Mesh.md#unregisterafterrender)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:1779

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

[Mesh](Mesh.md).[unregisterAfterWorldMatrixUpdate](Mesh.md#unregisterafterworldmatrixupdate)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:1293

___

### unregisterBeforeRender

▸ **unregisterBeforeRender**(`func`): [`Mesh`](Mesh.md)

Disposes a previously registered javascript function called before the rendering

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `func` | (`mesh`: [`AbstractMesh`](AbstractMesh.md)) => `void` | defines the function to remove |

#### Returns

[`Mesh`](Mesh.md)

the current mesh

#### Inherited from

[Mesh](Mesh.md).[unregisterBeforeRender](Mesh.md#unregisterbeforerender)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:1759

___

### updateCoordinateHeights

▸ **updateCoordinateHeights**(): [`GroundMesh`](GroundMesh.md)

Force the heights to be recomputed for getHeightAtCoordinates() or getNormalAtCoordinates()
if the ground has been updated.
This can be used in the render loop.

#### Returns

[`GroundMesh`](GroundMesh.md)

the GroundMesh.

#### Defined in

packages/dev/core/src/Meshes/groundMesh.ts:164

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

[Mesh](Mesh.md).[updateFacetData](Mesh.md#updatefacetdata)

#### Defined in

packages/dev/core/src/Meshes/abstractMesh.ts:2188

___

### updateIndices

▸ **updateIndices**(`indices`, `offset?`, `gpuMemoryOnly?`): [`AbstractMesh`](AbstractMesh.md)

Update the current index buffer

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `indices` | [`IndicesArray`](../modules.md#indicesarray) | `undefined` | defines the source data |
| `offset?` | `number` | `undefined` | defines the offset in the index buffer where to store the new data (can be null) |
| `gpuMemoryOnly` | `boolean` | `false` | defines a boolean indicating that only the GPU memory must be updated leaving the CPU version of the indices unchanged (false by default) |

#### Returns

[`AbstractMesh`](AbstractMesh.md)

the current mesh

#### Inherited from

[Mesh](Mesh.md).[updateIndices](Mesh.md#updateindices)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:1645

___

### updateMeshPositions

▸ **updateMeshPositions**(`positionFunction`, `computeNormals?`): [`Mesh`](Mesh.md)

This method updates the vertex positions of an updatable mesh according to the `positionFunction` returned values.

**`See`**

https://doc.babylonjs.com/how_to/how_to_dynamically_morph_a_mesh#other-shapes-updatemeshpositions

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `positionFunction` | (`data`: [`FloatArray`](../modules.md#floatarray)) => `void` | `undefined` | is a simple JS function what is passed the mesh `positions` array. It doesn't need to return anything |
| `computeNormals` | `boolean` | `true` | is a boolean (default true) to enable/disable the mesh normal recomputation after the vertex position update |

#### Returns

[`Mesh`](Mesh.md)

the current mesh

#### Inherited from

[Mesh](Mesh.md).[updateMeshPositions](Mesh.md#updatemeshpositions)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:1574

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

[Mesh](Mesh.md).[updatePoseMatrix](Mesh.md#updateposematrix)

#### Defined in

packages/dev/core/src/Meshes/transformNode.ts:279

___

### updateVerticesData

▸ **updateVerticesData**(`kind`, `data`, `updateExtends?`, `makeItUnique?`): [`AbstractMesh`](AbstractMesh.md)

Update a specific associated vertex buffer

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `kind` | `string` | defines which buffer to write to (positions, indices, normals, etc). Possible `kind` values :  - VertexBuffer.PositionKind  - VertexBuffer.UVKind  - VertexBuffer.UV2Kind  - VertexBuffer.UV3Kind  - VertexBuffer.UV4Kind  - VertexBuffer.UV5Kind  - VertexBuffer.UV6Kind  - VertexBuffer.ColorKind  - VertexBuffer.MatricesIndicesKind  - VertexBuffer.MatricesIndicesExtraKind  - VertexBuffer.MatricesWeightsKind  - VertexBuffer.MatricesWeightsExtraKind |
| `data` | [`FloatArray`](../modules.md#floatarray) | defines the data source |
| `updateExtends?` | `boolean` | defines if extends info of the mesh must be updated (can be null). This is mostly useful for "position" kind |
| `makeItUnique?` | `boolean` | defines if the geometry associated with the mesh must be cloned to make the change only for this mesh (and not all meshes associated with the same geometry) |

#### Returns

[`AbstractMesh`](AbstractMesh.md)

the current mesh

#### Inherited from

[Mesh](Mesh.md).[updateVerticesData](Mesh.md#updateverticesdata)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:1554

___

### validateSkinning

▸ **validateSkinning**(): `Object`

ValidateSkinning is used to determine that a mesh has valid skinning data along with skin metrics, if missing weights,
or not normalized it is returned as invalid mesh the string can be used for console logs, or on screen messages to let
the user know there was an issue with importing the mesh

#### Returns

`Object`

a validation object with skinned, valid and report string

| Name | Type |
| :------ | :------ |
| `report` | `string` |
| `skinned` | `boolean` |
| `valid` | `boolean` |

#### Inherited from

[Mesh](Mesh.md).[validateSkinning](Mesh.md#validateskinning)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:2435

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

[Mesh](Mesh.md).[AddNodeConstructor](Mesh.md#addnodeconstructor)

#### Defined in

packages/dev/core/src/node.ts:63

___

### Center

▸ `Static` **Center**(`meshesOrMinMaxVector`): [`Vector3`](Vector3.md)

Returns the center of the `{min:` Vector3`, max:` Vector3`}` or the center of MinMax vector3 computed from a mesh array

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `meshesOrMinMaxVector` | [`AbstractMesh`](AbstractMesh.md)[] \| { `max`: [`Vector3`](Vector3.md) ; `min`: [`Vector3`](Vector3.md)  } | could be an array of meshes or a `{min:` Vector3`, max:` Vector3`}` object |

#### Returns

[`Vector3`](Vector3.md)

a vector3

#### Inherited from

[Mesh](Mesh.md).[Center](Mesh.md#center-1)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:4418

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

[Mesh](Mesh.md).[Construct](Mesh.md#construct)

#### Defined in

packages/dev/core/src/node.ts:75

___

### MergeMeshes

▸ `Static` **MergeMeshes**(`meshes`, `disposeSource?`, `allow32BitsIndices?`, `meshSubclass?`, `subdivideWithSubMeshes?`, `multiMultiMaterials?`): [`Nullable`](../modules.md#nullable)[`Mesh`](Mesh.md)

Merge the array of meshes into a single mesh for performance reasons.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `meshes` | [`Mesh`](Mesh.md)[] | `undefined` | defines he vertices source.  They should all be of the same material.  Entries can empty |
| `disposeSource` | `boolean` | `true` | when true (default), dispose of the vertices from the source meshes |
| `allow32BitsIndices?` | `boolean` | `undefined` | when the sum of the vertices > 64k, this must be set to true |
| `meshSubclass?` | [`Mesh`](Mesh.md) | `undefined` | when set, vertices inserted into this Mesh.  Meshes can then be merged into a Mesh sub-class. |
| `subdivideWithSubMeshes?` | `boolean` | `undefined` | when true (false default), subdivide mesh to his subMesh array with meshes source. |
| `multiMultiMaterials?` | `boolean` | `undefined` | when true (false default), subdivide mesh and accept multiple multi materials, ignores subdivideWithSubMeshes. |

#### Returns

[`Nullable`](../modules.md#nullable)[`Mesh`](Mesh.md)

a new mesh

#### Inherited from

[Mesh](Mesh.md).[MergeMeshes](Mesh.md#mergemeshes)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:4433

___

### MergeMeshesAsync

▸ `Static` **MergeMeshesAsync**(`meshes`, `disposeSource?`, `allow32BitsIndices?`, `meshSubclass?`, `subdivideWithSubMeshes?`, `multiMultiMaterials?`): `Promise``any`

Merge the array of meshes into a single mesh for performance reasons.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `meshes` | [`Mesh`](Mesh.md)[] | `undefined` | defines he vertices source.  They should all be of the same material.  Entries can empty |
| `disposeSource` | `boolean` | `true` | when true (default), dispose of the vertices from the source meshes |
| `allow32BitsIndices?` | `boolean` | `undefined` | when the sum of the vertices > 64k, this must be set to true |
| `meshSubclass?` | [`Mesh`](Mesh.md) | `undefined` | when set, vertices inserted into this Mesh.  Meshes can then be merged into a Mesh sub-class. |
| `subdivideWithSubMeshes?` | `boolean` | `undefined` | when true (false default), subdivide mesh to his subMesh array with meshes source. |
| `multiMultiMaterials?` | `boolean` | `undefined` | when true (false default), subdivide mesh and accept multiple multi materials, ignores subdivideWithSubMeshes. |

#### Returns

`Promise``any`

a new mesh

#### Inherited from

[Mesh](Mesh.md).[MergeMeshesAsync](Mesh.md#mergemeshesasync)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:4454

___

### MinMax

▸ `Static` **MinMax**(`meshes`): `Object`

Returns an object containing a min and max Vector3 which are the minimum and maximum vectors of each mesh bounding box from the passed array, in the world coordinates

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `meshes` | [`AbstractMesh`](AbstractMesh.md)[] | defines the list of meshes to scan |

#### Returns

`Object`

an object `{min:` Vector3`, max:` Vector3`}`

| Name | Type |
| :------ | :------ |
| `max` | [`Vector3`](Vector3.md) |
| `min` | [`Vector3`](Vector3.md) |

#### Inherited from

[Mesh](Mesh.md).[MinMax](Mesh.md#minmax)

#### Defined in

packages/dev/core/src/Meshes/mesh.ts:4383

___

### Parse

▸ `Static` **Parse**(`parsedMesh`, `scene`): [`GroundMesh`](GroundMesh.md)

Parses a serialized ground mesh

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `parsedMesh` | `any` | the serialized mesh |
| `scene` | [`Scene`](Scene.md) | the scene to create the ground mesh in |

#### Returns

[`GroundMesh`](GroundMesh.md)

the created ground mesh

#### Overrides

[Mesh](Mesh.md).[Parse](Mesh.md#parse)

#### Defined in

packages/dev/core/src/Meshes/groundMesh.ts:309

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

[Mesh](Mesh.md).[ParseAnimationRanges](Mesh.md#parseanimationranges)

#### Defined in

packages/dev/core/src/node.ts:919
