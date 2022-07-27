[@dev/core](../README.md) / [Exports](../modules.md) / Scene

# Class: Scene

Represents a scene to be rendered by the engine.

**`See`**

https://doc.babylonjs.com/features/scene

## Hierarchy

- [`AbstractScene`](AbstractScene.md)

  ↳ **`Scene`**

## Implements

- [`IAnimatable`](../interfaces/IAnimatable.md)
- `IClipPlanesHolder`

## Table of contents

### Constructors

- [constructor](Scene.md#constructor)

### Properties

- [\_activeMeshes](Scene.md#_activemeshes)
- [\_activeMeshesFrozenButKeepClipping](Scene.md#_activemeshesfrozenbutkeepclipping)
- [\_activeRequests](Scene.md#_activerequests)
- [\_activeSkeletons](Scene.md#_activeskeletons)
- [\_animationPropertiesOverride](Scene.md#_animationpropertiesoverride)
- [\_animationRatio](Scene.md#_animationratio)
- [\_blockMaterialDirtyMechanism](Scene.md#_blockmaterialdirtymechanism)
- [\_collisionCoordinator](Scene.md#_collisioncoordinator)
- [\_computePressureObserver](Scene.md#_computepressureobserver)
- [\_currentInternalStep](Scene.md#_currentinternalstep)
- [\_currentStepId](Scene.md#_currentstepid)
- [\_defaultFrameBufferCleared](Scene.md#_defaultframebuffercleared)
- [\_defaultMaterial](Scene.md#_defaultmaterial)
- [\_defaultMeshCandidates](Scene.md#_defaultmeshcandidates)
- [\_defaultSubMeshCandidates](Scene.md#_defaultsubmeshcandidates)
- [\_engine](Scene.md#_engine)
- [\_executeWhenReadyTimeoutId](Scene.md#_executewhenreadytimeoutid)
- [\_externalData](Scene.md#_externaldata)
- [\_fogEnabled](Scene.md#_fogenabled)
- [\_fogMode](Scene.md#_fogmode)
- [\_forcePointsCloud](Scene.md#_forcepointscloud)
- [\_forceWireframe](Scene.md#_forcewireframe)
- [\_frameId](Scene.md#_frameid)
- [\_geometriesByUniqueId](Scene.md#_geometriesbyuniqueid)
- [\_intermediateRendering](Scene.md#_intermediaterendering)
- [\_isDisposed](Scene.md#_isdisposed)
- [\_lightsEnabled](Scene.md#_lightsenabled)
- [\_materialsRenderTargets](Scene.md#_materialsrendertargets)
- [\_meshesForIntersections](Scene.md#_meshesforintersections)
- [\_onAfterCameraRenderObserver](Scene.md#_onaftercamerarenderobserver)
- [\_onAfterRenderObserver](Scene.md#_onafterrenderobserver)
- [\_onBeforeCameraRenderObserver](Scene.md#_onbeforecamerarenderobserver)
- [\_onBeforeRenderObserver](Scene.md#_onbeforerenderobserver)
- [\_onDisposeObserver](Scene.md#_ondisposeobserver)
- [\_perfCollector](Scene.md#_perfcollector)
- [\_preventFreeActiveMeshesAndRenderingGroups](Scene.md#_preventfreeactivemeshesandrenderinggroups)
- [\_processedMaterials](Scene.md#_processedmaterials)
- [\_projectionUpdateFlag](Scene.md#_projectionupdateflag)
- [\_renderId](Scene.md#_renderid)
- [\_renderTargets](Scene.md#_rendertargets)
- [\_renderingManager](Scene.md#_renderingmanager)
- [\_sceneUbo](Scene.md#_sceneubo)
- [\_shadowsEnabled](Scene.md#_shadowsenabled)
- [\_skeletonsEnabled](Scene.md#_skeletonsenabled)
- [\_skipEvaluateActiveMeshesCompletely](Scene.md#_skipevaluateactivemeshescompletely)
- [\_skipFrustumClipping](Scene.md#_skipfrustumclipping)
- [\_softwareSkinnedMeshes](Scene.md#_softwareskinnedmeshes)
- [\_texturesEnabled](Scene.md#_texturesenabled)
- [\_timeAccumulator](Scene.md#_timeaccumulator)
- [\_totalVertices](Scene.md#_totalvertices)
- [\_transformMatrix](Scene.md#_transformmatrix)
- [\_transientComponents](Scene.md#_transientcomponents)
- [\_uid](Scene.md#_uid)
- [\_useRightHandedSystem](Scene.md#_userighthandedsystem)
- [\_viewUpdateFlag](Scene.md#_viewupdateflag)
- [actionManager](Scene.md#actionmanager)
- [actionManagers](Scene.md#actionmanagers)
- [activeCameras](Scene.md#activecameras)
- [ambientColor](Scene.md#ambientcolor)
- [animationGroups](Scene.md#animationgroups)
- [animationTimeScale](Scene.md#animationtimescale)
- [animations](Scene.md#animations)
- [animationsEnabled](Scene.md#animationsenabled)
- [audioEnabled](Scene.md#audioenabled)
- [audioListenerPositionProvider](Scene.md#audiolistenerpositionprovider)
- [audioPositioningRefreshRate](Scene.md#audiopositioningrefreshrate)
- [autoClear](Scene.md#autoclear)
- [autoClearDepthAndStencil](Scene.md#autocleardepthandstencil)
- [cameraToUseForPointers](Scene.md#cameratouseforpointers)
- [cameras](Scene.md#cameras)
- [clearColor](Scene.md#clearcolor)
- [clipPlane](Scene.md#clipplane)
- [clipPlane2](Scene.md#clipplane2)
- [clipPlane3](Scene.md#clipplane3)
- [clipPlane4](Scene.md#clipplane4)
- [clipPlane5](Scene.md#clipplane5)
- [clipPlane6](Scene.md#clipplane6)
- [collisionsEnabled](Scene.md#collisionsenabled)
- [constantlyUpdateMeshUnderPointer](Scene.md#constantlyupdatemeshunderpointer)
- [customLODSelector](Scene.md#customlodselector)
- [customRenderTargets](Scene.md#customrendertargets)
- [debugLayer](Scene.md#debuglayer)
- [defaultCursor](Scene.md#defaultcursor)
- [deltaTime](Scene.md#deltatime)
- [depthPeelingRenderer](Scene.md#depthpeelingrenderer)
- [disableOfflineSupportExceptionRules](Scene.md#disableofflinesupportexceptionrules)
- [dispatchAllSubMeshesOfActiveMeshes](Scene.md#dispatchallsubmeshesofactivemeshes)
- [doNotHandleCursors](Scene.md#donothandlecursors)
- [dumpNextRenderTargets](Scene.md#dumpnextrendertargets)
- [effectLayers](Scene.md#effectlayers)
- [environmentBRDFTexture](Scene.md#environmentbrdftexture)
- [environmentIntensity](Scene.md#environmentintensity)
- [fogColor](Scene.md#fogcolor)
- [fogDensity](Scene.md#fogdensity)
- [fogEnd](Scene.md#fogend)
- [fogStart](Scene.md#fogstart)
- [forceShowBoundingBoxes](Scene.md#forceshowboundingboxes)
- [gamepadManager](Scene.md#gamepadmanager)
- [geometries](Scene.md#geometries)
- [geometryBufferRenderer](Scene.md#geometrybufferrenderer)
- [getActiveMeshCandidates](Scene.md#getactivemeshcandidates)
- [getActiveSubMeshCandidates](Scene.md#getactivesubmeshcandidates)
- [getCollidingSubMeshCandidates](Scene.md#getcollidingsubmeshcandidates)
- [getDeterministicFrameTime](Scene.md#getdeterministicframetime)
- [getIntersectingSubMeshCandidates](Scene.md#getintersectingsubmeshcandidates)
- [gravity](Scene.md#gravity)
- [headphone](Scene.md#headphone)
- [hoverCursor](Scene.md#hovercursor)
- [importedMeshesFiles](Scene.md#importedmeshesfiles)
- [layers](Scene.md#layers)
- [lensFlareSystems](Scene.md#lensflaresystems)
- [lensFlaresEnabled](Scene.md#lensflaresenabled)
- [lights](Scene.md#lights)
- [loadingPluginName](Scene.md#loadingpluginname)
- [mainSoundTrack](Scene.md#mainsoundtrack)
- [materials](Scene.md#materials)
- [meshes](Scene.md#meshes)
- [metadata](Scene.md#metadata)
- [morphTargetManagers](Scene.md#morphtargetmanagers)
- [multiMaterials](Scene.md#multimaterials)
- [needsPreviousWorldMatrices](Scene.md#needspreviousworldmatrices)
- [offlineProvider](Scene.md#offlineprovider)
- [onActiveCameraChanged](Scene.md#onactivecamerachanged)
- [onAfterActiveMeshesEvaluationObservable](Scene.md#onafteractivemeshesevaluationobservable)
- [onAfterAnimationsObservable](Scene.md#onafteranimationsobservable)
- [onAfterCameraRenderObservable](Scene.md#onaftercamerarenderobservable)
- [onAfterDrawPhaseObservable](Scene.md#onafterdrawphaseobservable)
- [onAfterParticlesRenderingObservable](Scene.md#onafterparticlesrenderingobservable)
- [onAfterPhysicsObservable](Scene.md#onafterphysicsobservable)
- [onAfterRenderCameraObservable](Scene.md#onafterrendercameraobservable)
- [onAfterRenderObservable](Scene.md#onafterrenderobservable)
- [onAfterRenderTargetsRenderObservable](Scene.md#onafterrendertargetsrenderobservable)
- [onAfterRenderingGroupObservable](Scene.md#onafterrenderinggroupobservable)
- [onAfterSpritesRenderingObservable](Scene.md#onafterspritesrenderingobservable)
- [onAfterStepObservable](Scene.md#onafterstepobservable)
- [onAnimationFileImportedObservable](Scene.md#onanimationfileimportedobservable)
- [onBeforeActiveMeshesEvaluationObservable](Scene.md#onbeforeactivemeshesevaluationobservable)
- [onBeforeAnimationsObservable](Scene.md#onbeforeanimationsobservable)
- [onBeforeCameraRenderObservable](Scene.md#onbeforecamerarenderobservable)
- [onBeforeDrawPhaseObservable](Scene.md#onbeforedrawphaseobservable)
- [onBeforeParticlesRenderingObservable](Scene.md#onbeforeparticlesrenderingobservable)
- [onBeforePhysicsObservable](Scene.md#onbeforephysicsobservable)
- [onBeforeRenderObservable](Scene.md#onbeforerenderobservable)
- [onBeforeRenderTargetsRenderObservable](Scene.md#onbeforerendertargetsrenderobservable)
- [onBeforeRenderingGroupObservable](Scene.md#onbeforerenderinggroupobservable)
- [onBeforeSpritesRenderingObservable](Scene.md#onbeforespritesrenderingobservable)
- [onBeforeStepObservable](Scene.md#onbeforestepobservable)
- [onCameraRemovedObservable](Scene.md#oncameraremovedobservable)
- [onComputePressureChanged](Scene.md#oncomputepressurechanged)
- [onDataLoadedObservable](Scene.md#ondataloadedobservable)
- [onDisposeObservable](Scene.md#ondisposeobservable)
- [onGeometryRemovedObservable](Scene.md#ongeometryremovedobservable)
- [onKeyboardObservable](Scene.md#onkeyboardobservable)
- [onLightRemovedObservable](Scene.md#onlightremovedobservable)
- [onMaterialRemovedObservable](Scene.md#onmaterialremovedobservable)
- [onMeshImportedObservable](Scene.md#onmeshimportedobservable)
- [onMeshRemovedObservable](Scene.md#onmeshremovedobservable)
- [onMultiMaterialRemovedObservable](Scene.md#onmultimaterialremovedobservable)
- [onNewCameraAddedObservable](Scene.md#onnewcameraaddedobservable)
- [onNewGeometryAddedObservable](Scene.md#onnewgeometryaddedobservable)
- [onNewLightAddedObservable](Scene.md#onnewlightaddedobservable)
- [onNewMaterialAddedObservable](Scene.md#onnewmaterialaddedobservable)
- [onNewMeshAddedObservable](Scene.md#onnewmeshaddedobservable)
- [onNewMultiMaterialAddedObservable](Scene.md#onnewmultimaterialaddedobservable)
- [onNewSkeletonAddedObservable](Scene.md#onnewskeletonaddedobservable)
- [onNewTextureAddedObservable](Scene.md#onnewtextureaddedobservable)
- [onNewTransformNodeAddedObservable](Scene.md#onnewtransformnodeaddedobservable)
- [onPointerDown](Scene.md#onpointerdown)
- [onPointerMove](Scene.md#onpointermove)
- [onPointerObservable](Scene.md#onpointerobservable)
- [onPointerPick](Scene.md#onpointerpick)
- [onPointerUp](Scene.md#onpointerup)
- [onPreKeyboardObservable](Scene.md#onprekeyboardobservable)
- [onPrePointerObservable](Scene.md#onprepointerobservable)
- [onReadyObservable](Scene.md#onreadyobservable)
- [onSkeletonRemovedObservable](Scene.md#onskeletonremovedobservable)
- [onTextureRemovedObservable](Scene.md#ontextureremovedobservable)
- [onTransformNodeRemovedObservable](Scene.md#ontransformnoderemovedobservable)
- [particleSystems](Scene.md#particlesystems)
- [particlesEnabled](Scene.md#particlesenabled)
- [physicsEnabled](Scene.md#physicsenabled)
- [pointerDownPredicate](Scene.md#pointerdownpredicate)
- [pointerMovePredicate](Scene.md#pointermovepredicate)
- [pointerMoveTrianglePredicate](Scene.md#pointermovetrianglepredicate)
- [pointerUpPredicate](Scene.md#pointeruppredicate)
- [postProcessManager](Scene.md#postprocessmanager)
- [postProcessRenderPipelineManager](Scene.md#postprocessrenderpipelinemanager)
- [postProcesses](Scene.md#postprocesses)
- [postProcessesEnabled](Scene.md#postprocessesenabled)
- [prePassRenderer](Scene.md#prepassrenderer)
- [preventDefaultOnPointerDown](Scene.md#preventdefaultonpointerdown)
- [preventDefaultOnPointerUp](Scene.md#preventdefaultonpointerup)
- [probesEnabled](Scene.md#probesenabled)
- [proceduralTextures](Scene.md#proceduraltextures)
- [proceduralTexturesEnabled](Scene.md#proceduraltexturesenabled)
- [reflectionProbes](Scene.md#reflectionprobes)
- [renderTargetsEnabled](Scene.md#rendertargetsenabled)
- [requireLightSorting](Scene.md#requirelightsorting)
- [reservedDataStore](Scene.md#reserveddatastore)
- [rootNodes](Scene.md#rootnodes)
- [selectionOctree](Scene.md#selectionoctree)
- [simplificationQueue](Scene.md#simplificationqueue)
- [skeletons](Scene.md#skeletons)
- [skipPointerDownPicking](Scene.md#skippointerdownpicking)
- [skipPointerMovePicking](Scene.md#skippointermovepicking)
- [skipPointerUpPicking](Scene.md#skippointeruppicking)
- [soundTracks](Scene.md#soundtracks)
- [sounds](Scene.md#sounds)
- [spriteManagers](Scene.md#spritemanagers)
- [spritesEnabled](Scene.md#spritesenabled)
- [subSurfaceConfiguration](Scene.md#subsurfaceconfiguration)
- [textures](Scene.md#textures)
- [transformNodes](Scene.md#transformnodes)
- [useConstantAnimationDeltaTime](Scene.md#useconstantanimationdeltatime)
- [useDelayedTextureLoading](Scene.md#usedelayedtextureloading)
- [useOrderIndependentTransparency](Scene.md#useorderindependenttransparency)
- [FOGMODE\_EXP](Scene.md#fogmode_exp)
- [FOGMODE\_EXP2](Scene.md#fogmode_exp2)
- [FOGMODE\_LINEAR](Scene.md#fogmode_linear)
- [FOGMODE\_NONE](Scene.md#fogmode_none)
- [MaxDeltaTime](Scene.md#maxdeltatime)
- [MinDeltaTime](Scene.md#mindeltatime)

### Accessors

- [activeBonesPerfCounter](Scene.md#activebonesperfcounter)
- [activeCamera](Scene.md#activecamera)
- [activeParticlesPerfCounter](Scene.md#activeparticlesperfcounter)
- [afterCameraRender](Scene.md#aftercamerarender)
- [afterRender](Scene.md#afterrender)
- [animatables](Scene.md#animatables)
- [animationPropertiesOverride](Scene.md#animationpropertiesoverride)
- [beforeCameraRender](Scene.md#beforecamerarender)
- [beforeRender](Scene.md#beforerender)
- [blockMaterialDirtyMechanism](Scene.md#blockmaterialdirtymechanism)
- [blockfreeActiveMeshesAndRenderingGroups](Scene.md#blockfreeactivemeshesandrenderinggroups)
- [defaultMaterial](Scene.md#defaultmaterial)
- [environmentTexture](Scene.md#environmenttexture)
- [fogEnabled](Scene.md#fogenabled)
- [fogMode](Scene.md#fogmode)
- [forcePointsCloud](Scene.md#forcepointscloud)
- [forceWireframe](Scene.md#forcewireframe)
- [frustumPlanes](Scene.md#frustumplanes)
- [imageProcessingConfiguration](Scene.md#imageprocessingconfiguration)
- [isDisposed](Scene.md#isdisposed)
- [isLoading](Scene.md#isloading)
- [lightsEnabled](Scene.md#lightsenabled)
- [meshUnderPointer](Scene.md#meshunderpointer)
- [onDispose](Scene.md#ondispose)
- [pointerX](Scene.md#pointerx)
- [pointerY](Scene.md#pointery)
- [prePass](Scene.md#prepass)
- [shadowsEnabled](Scene.md#shadowsenabled)
- [skeletonsEnabled](Scene.md#skeletonsenabled)
- [skipFrustumClipping](Scene.md#skipfrustumclipping)
- [texturesEnabled](Scene.md#texturesenabled)
- [totalActiveIndicesPerfCounter](Scene.md#totalactiveindicesperfcounter)
- [totalVerticesPerfCounter](Scene.md#totalverticesperfcounter)
- [uid](Scene.md#uid)
- [unTranslatedPointer](Scene.md#untranslatedpointer)
- [useRightHandedSystem](Scene.md#userighthandedsystem)
- [DoubleClickDelay](Scene.md#doubleclickdelay)
- [DragMovementThreshold](Scene.md#dragmovementthreshold)
- [ExclusiveDoubleClickMode](Scene.md#exclusivedoubleclickmode)
- [LongPressDelay](Scene.md#longpressdelay)

### Methods

- [\_activeMesh](Scene.md#_activemesh)
- [\_bindFrameBuffer](Scene.md#_bindframebuffer)
- [\_checkCameraRenderTarget](Scene.md#_checkcamerarendertarget)
- [\_checkIntersections](Scene.md#_checkintersections)
- [\_clear](Scene.md#_clear)
- [\_clearFrameBuffer](Scene.md#_clearframebuffer)
- [\_createUbo](Scene.md#_createubo)
- [\_disposeList](Scene.md#_disposelist)
- [\_evaluateActiveMeshes](Scene.md#_evaluateactivemeshes)
- [\_evaluateSubMesh](Scene.md#_evaluatesubmesh)
- [\_executeActiveContainerCleanup](Scene.md#_executeactivecontainercleanup)
- [\_executeOnceBeforeRender](Scene.md#_executeoncebeforerender)
- [\_getByTags](Scene.md#_getbytags)
- [\_getGeometryByUniqueId](Scene.md#_getgeometrybyuniqueid)
- [\_processSubCameras](Scene.md#_processsubcameras)
- [\_registerTransientComponents](Scene.md#_registertransientcomponents)
- [addActionManager](Scene.md#addactionmanager)
- [addAnimation](Scene.md#addanimation)
- [addAnimationGroup](Scene.md#addanimationgroup)
- [addCamera](Scene.md#addcamera)
- [addEffectLayer](Scene.md#addeffectlayer)
- [addExternalData](Scene.md#addexternaldata)
- [addGeometry](Scene.md#addgeometry)
- [addLensFlareSystem](Scene.md#addlensflaresystem)
- [addLight](Scene.md#addlight)
- [addMaterial](Scene.md#addmaterial)
- [addMesh](Scene.md#addmesh)
- [addMorphTargetManager](Scene.md#addmorphtargetmanager)
- [addMultiMaterial](Scene.md#addmultimaterial)
- [addParticleSystem](Scene.md#addparticlesystem)
- [addPendingData](Scene.md#addpendingdata)
- [addReflectionProbe](Scene.md#addreflectionprobe)
- [addSkeleton](Scene.md#addskeleton)
- [addTexture](Scene.md#addtexture)
- [addTransformNode](Scene.md#addtransformnode)
- [animate](Scene.md#animate)
- [attachControl](Scene.md#attachcontrol)
- [beginAnimation](Scene.md#beginanimation)
- [beginDirectAnimation](Scene.md#begindirectanimation)
- [beginDirectHierarchyAnimation](Scene.md#begindirecthierarchyanimation)
- [beginHierarchyAnimation](Scene.md#beginhierarchyanimation)
- [beginWeightedAnimation](Scene.md#beginweightedanimation)
- [bindEyePosition](Scene.md#bindeyeposition)
- [cleanCachedTextureBuffer](Scene.md#cleancachedtexturebuffer)
- [clearCachedVertexData](Scene.md#clearcachedvertexdata)
- [createDefaultCamera](Scene.md#createdefaultcamera)
- [createDefaultCameraOrLight](Scene.md#createdefaultcameraorlight)
- [createDefaultEnvironment](Scene.md#createdefaultenvironment)
- [createDefaultLight](Scene.md#createdefaultlight)
- [createDefaultSkybox](Scene.md#createdefaultskybox)
- [createDefaultVRExperience](Scene.md#createdefaultvrexperience)
- [createDefaultXRExperienceAsync](Scene.md#createdefaultxrexperienceasync)
- [createOrUpdateSelectionOctree](Scene.md#createorupdateselectionoctree)
- [createPickingRay](Scene.md#createpickingray)
- [createPickingRayInCameraSpace](Scene.md#createpickingrayincameraspace)
- [createPickingRayInCameraSpaceToRef](Scene.md#createpickingrayincameraspacetoref)
- [createPickingRayToRef](Scene.md#createpickingraytoref)
- [createSceneUniformBuffer](Scene.md#createsceneuniformbuffer)
- [deleteCompoundImpostor](Scene.md#deletecompoundimpostor)
- [detachControl](Scene.md#detachcontrol)
- [disableDepthRenderer](Scene.md#disabledepthrenderer)
- [disableGeometryBufferRenderer](Scene.md#disablegeometrybufferrenderer)
- [disablePhysicsEngine](Scene.md#disablephysicsengine)
- [disablePrePassRenderer](Scene.md#disableprepassrenderer)
- [disableSubSurfaceForPrePass](Scene.md#disablesubsurfaceforprepass)
- [dispose](Scene.md#dispose)
- [enableDepthRenderer](Scene.md#enabledepthrenderer)
- [enableGeometryBufferRenderer](Scene.md#enablegeometrybufferrenderer)
- [enablePhysics](Scene.md#enablephysics)
- [enablePrePassRenderer](Scene.md#enableprepassrenderer)
- [enableSubSurfaceForPrePass](Scene.md#enablesubsurfaceforprepass)
- [executeOnceBeforeRender](Scene.md#executeoncebeforerender)
- [executeWhenReady](Scene.md#executewhenready)
- [finalizeSceneUbo](Scene.md#finalizesceneubo)
- [freeActiveMeshes](Scene.md#freeactivemeshes)
- [freeProcessedMaterials](Scene.md#freeprocessedmaterials)
- [freeRenderingGroups](Scene.md#freerenderinggroups)
- [freezeActiveMeshes](Scene.md#freezeactivemeshes)
- [freezeMaterials](Scene.md#freezematerials)
- [getActiveBones](Scene.md#getactivebones)
- [getActiveIndices](Scene.md#getactiveindices)
- [getActiveMeshes](Scene.md#getactivemeshes)
- [getActiveParticles](Scene.md#getactiveparticles)
- [getAllAnimatablesByTarget](Scene.md#getallanimatablesbytarget)
- [getAnimatableByTarget](Scene.md#getanimatablebytarget)
- [getAnimationGroupByName](Scene.md#getanimationgroupbyname)
- [getAnimationRatio](Scene.md#getanimationratio)
- [getAutoClearDepthStencilSetup](Scene.md#getautocleardepthstencilsetup)
- [getBoneById](Scene.md#getbonebyid)
- [getBoneByName](Scene.md#getbonebyname)
- [getBoundingBoxRenderer](Scene.md#getboundingboxrenderer)
- [getCachedEffect](Scene.md#getcachedeffect)
- [getCachedMaterial](Scene.md#getcachedmaterial)
- [getCachedVisibility](Scene.md#getcachedvisibility)
- [getCameraById](Scene.md#getcamerabyid)
- [getCameraByName](Scene.md#getcamerabyname)
- [getCameraByUniqueId](Scene.md#getcamerabyuniqueid)
- [getCamerasByTags](Scene.md#getcamerasbytags)
- [getClassName](Scene.md#getclassname)
- [getEngine](Scene.md#getengine)
- [getExternalData](Scene.md#getexternaldata)
- [getFrameId](Scene.md#getframeid)
- [getGeometries](Scene.md#getgeometries)
- [getGeometryById](Scene.md#getgeometrybyid)
- [getGlowLayerByName](Scene.md#getglowlayerbyname)
- [getHighlightLayerByName](Scene.md#gethighlightlayerbyname)
- [getInternalStep](Scene.md#getinternalstep)
- [getLastEntryById](Scene.md#getlastentrybyid)
- [getLastMaterialById](Scene.md#getlastmaterialbyid)
- [getLastMeshById](Scene.md#getlastmeshbyid)
- [getLastSkeletonById](Scene.md#getlastskeletonbyid)
- [getLensFlareSystemByID](Scene.md#getlensflaresystembyid)
- [getLensFlareSystemById](Scene.md#getlensflaresystembyid-1)
- [getLensFlareSystemByName](Scene.md#getlensflaresystembyname)
- [getLightById](Scene.md#getlightbyid)
- [getLightByName](Scene.md#getlightbyname)
- [getLightByUniqueId](Scene.md#getlightbyuniqueid)
- [getLightsByTags](Scene.md#getlightsbytags)
- [getMaterialById](Scene.md#getmaterialbyid)
- [getMaterialByName](Scene.md#getmaterialbyname)
- [getMaterialByTags](Scene.md#getmaterialbytags)
- [getMaterialByUniqueID](Scene.md#getmaterialbyuniqueid)
- [getMeshById](Scene.md#getmeshbyid)
- [getMeshByName](Scene.md#getmeshbyname)
- [getMeshByUniqueId](Scene.md#getmeshbyuniqueid)
- [getMeshesById](Scene.md#getmeshesbyid)
- [getMeshesByTags](Scene.md#getmeshesbytags)
- [getMorphTargetById](Scene.md#getmorphtargetbyid)
- [getMorphTargetByName](Scene.md#getmorphtargetbyname)
- [getMorphTargetManagerById](Scene.md#getmorphtargetmanagerbyid)
- [getNodeById](Scene.md#getnodebyid)
- [getNodeByName](Scene.md#getnodebyname)
- [getNodes](Scene.md#getnodes)
- [getOrAddExternalDataWithFactory](Scene.md#getoraddexternaldatawithfactory)
- [getOutlineRenderer](Scene.md#getoutlinerenderer)
- [getParticleSystemById](Scene.md#getparticlesystembyid)
- [getPerfCollector](Scene.md#getperfcollector)
- [getPhysicsEngine](Scene.md#getphysicsengine)
- [getPointerOverMesh](Scene.md#getpointerovermesh)
- [getPointerOverSprite](Scene.md#getpointeroversprite)
- [getPostProcessByName](Scene.md#getpostprocessbyname)
- [getProjectionMatrix](Scene.md#getprojectionmatrix)
- [getRenderId](Scene.md#getrenderid)
- [getSceneUniformBuffer](Scene.md#getsceneuniformbuffer)
- [getSkeletonById](Scene.md#getskeletonbyid)
- [getSkeletonByName](Scene.md#getskeletonbyname)
- [getSkeletonByUniqueId](Scene.md#getskeletonbyuniqueid)
- [getSoundByName](Scene.md#getsoundbyname)
- [getStepId](Scene.md#getstepid)
- [getTextureByName](Scene.md#gettexturebyname)
- [getTextureByUniqueId](Scene.md#gettexturebyuniqueid)
- [getTotalVertices](Scene.md#gettotalvertices)
- [getTransformMatrix](Scene.md#gettransformmatrix)
- [getTransformNodeById](Scene.md#gettransformnodebyid)
- [getTransformNodeByName](Scene.md#gettransformnodebyname)
- [getTransformNodeByUniqueId](Scene.md#gettransformnodebyuniqueid)
- [getTransformNodesById](Scene.md#gettransformnodesbyid)
- [getTransformNodesByTags](Scene.md#gettransformnodesbytags)
- [getUniqueId](Scene.md#getuniqueid)
- [getViewMatrix](Scene.md#getviewmatrix)
- [getWaitingItemsCount](Scene.md#getwaitingitemscount)
- [getWorldExtends](Scene.md#getworldextends)
- [incrementRenderId](Scene.md#incrementrenderid)
- [isActiveMesh](Scene.md#isactivemesh)
- [isCachedMaterialInvalid](Scene.md#iscachedmaterialinvalid)
- [isPhysicsEnabled](Scene.md#isphysicsenabled)
- [isPointerCaptured](Scene.md#ispointercaptured)
- [isReady](Scene.md#isready)
- [markAllMaterialsAsDirty](Scene.md#markallmaterialsasdirty)
- [multiPick](Scene.md#multipick)
- [multiPickSprite](Scene.md#multipicksprite)
- [multiPickSpriteWithRay](Scene.md#multipickspritewithray)
- [multiPickWithRay](Scene.md#multipickwithray)
- [pick](Scene.md#pick)
- [pickSprite](Scene.md#picksprite)
- [pickSpriteWithRay](Scene.md#pickspritewithray)
- [pickWithBoundingInfo](Scene.md#pickwithboundinginfo)
- [pickWithRay](Scene.md#pickwithray)
- [pushGeometry](Scene.md#pushgeometry)
- [registerAfterRender](Scene.md#registerafterrender)
- [registerBeforeRender](Scene.md#registerbeforerender)
- [removeActionManager](Scene.md#removeactionmanager)
- [removeAnimation](Scene.md#removeanimation)
- [removeAnimationGroup](Scene.md#removeanimationgroup)
- [removeCamera](Scene.md#removecamera)
- [removeEffectLayer](Scene.md#removeeffectlayer)
- [removeExternalData](Scene.md#removeexternaldata)
- [removeGeometry](Scene.md#removegeometry)
- [removeLensFlareSystem](Scene.md#removelensflaresystem)
- [removeLight](Scene.md#removelight)
- [removeMaterial](Scene.md#removematerial)
- [removeMesh](Scene.md#removemesh)
- [removeMorphTargetManager](Scene.md#removemorphtargetmanager)
- [removeMultiMaterial](Scene.md#removemultimaterial)
- [removeParticleSystem](Scene.md#removeparticlesystem)
- [removePendingData](Scene.md#removependingdata)
- [removeReflectionProbe](Scene.md#removereflectionprobe)
- [removeSkeleton](Scene.md#removeskeleton)
- [removeTexture](Scene.md#removetexture)
- [removeTransformNode](Scene.md#removetransformnode)
- [render](Scene.md#render)
- [resetCachedMaterial](Scene.md#resetcachedmaterial)
- [resetDrawCache](Scene.md#resetdrawcache)
- [resetLastAnimationTimeFrame](Scene.md#resetlastanimationtimeframe)
- [setActiveCameraById](Scene.md#setactivecamerabyid)
- [setActiveCameraByName](Scene.md#setactivecamerabyname)
- [setDefaultCandidateProviders](Scene.md#setdefaultcandidateproviders)
- [setPointerOverMesh](Scene.md#setpointerovermesh)
- [setPointerOverSprite](Scene.md#setpointeroversprite)
- [setRenderingAutoClearDepthStencil](Scene.md#setrenderingautocleardepthstencil)
- [setRenderingOrder](Scene.md#setrenderingorder)
- [setSceneUniformBuffer](Scene.md#setsceneuniformbuffer)
- [setStepId](Scene.md#setstepid)
- [setTransformMatrix](Scene.md#settransformmatrix)
- [simulatePointerDown](Scene.md#simulatepointerdown)
- [simulatePointerMove](Scene.md#simulatepointermove)
- [simulatePointerUp](Scene.md#simulatepointerup)
- [sortLightsByPriority](Scene.md#sortlightsbypriority)
- [stopAllAnimations](Scene.md#stopallanimations)
- [stopAnimation](Scene.md#stopanimation)
- [switchActiveCamera](Scene.md#switchactivecamera)
- [unfreezeActiveMeshes](Scene.md#unfreezeactivemeshes)
- [unfreezeMaterials](Scene.md#unfreezematerials)
- [unregisterAfterRender](Scene.md#unregisterafterrender)
- [unregisterBeforeRender](Scene.md#unregisterbeforerender)
- [updateTransformMatrix](Scene.md#updatetransformmatrix)
- [whenReadyAsync](Scene.md#whenreadyasync)
- [AddIndividualParser](Scene.md#addindividualparser)
- [AddParser](Scene.md#addparser)
- [CollisionCoordinatorFactory](Scene.md#collisioncoordinatorfactory)
- [DefaultMaterialFactory](Scene.md#defaultmaterialfactory)
- [GetIndividualParser](Scene.md#getindividualparser)
- [GetParser](Scene.md#getparser)
- [Parse](Scene.md#parse)

## Constructors

### constructor

• **new Scene**(`engine`, `options?`)

Creates a new Scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `engine` | [`Engine`](Engine.md) | defines the engine to use to render this scene |
| `options?` | [`SceneOptions`](../interfaces/SceneOptions.md) | defines the scene options |

#### Overrides

[AbstractScene](AbstractScene.md).[constructor](AbstractScene.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1481

## Properties

### \_activeMeshes

• `Private` **\_activeMeshes**: [`SmartArray`](SmartArray.md)[`AbstractMesh`](AbstractMesh.md)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1251

___

### \_activeMeshesFrozenButKeepClipping

• **\_activeMeshesFrozenButKeepClipping**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3702

___

### \_activeRequests

• `Private` **\_activeRequests**: [`IFileRequest`](../interfaces/IFileRequest.md)[]

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1240

___

### \_activeSkeletons

• `Private` **\_activeSkeletons**: [`SmartArrayNoDuplicate`](SmartArrayNoDuplicate.md)[`Skeleton`](Skeleton.md)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1257

___

### \_animationPropertiesOverride

• `Private` **\_animationPropertiesOverride**: [`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:336

___

### \_animationRatio

• `Private` **\_animationRatio**: `number`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1208

___

### \_blockMaterialDirtyMechanism

• `Private` **\_blockMaterialDirtyMechanism**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:5126

___

### \_collisionCoordinator

• `Private` **\_collisionCoordinator**: `ICollisionCoordinator`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1115

___

### \_computePressureObserver

• `Private` **\_computePressureObserver**: `undefined` \| [`ComputePressureObserverWrapper`](ComputePressureObserverWrapper.md)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:5341

___

### \_currentInternalStep

• `Private` **\_currentInternalStep**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:876

___

### \_currentStepId

• `Private` **\_currentStepId**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:875

___

### \_defaultFrameBufferCleared

• `Private` **\_defaultFrameBufferCleared**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1233

___

### \_defaultMaterial

• `Private` **\_defaultMaterial**: [`Material`](Material.md)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1034

___

### \_defaultMeshCandidates

• `Private` **\_defaultMeshCandidates**: [`ISmartArrayLike`](../interfaces/ISmartArrayLike.md)[`AbstractMesh`](AbstractMesh.md)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1556

___

### \_defaultSubMeshCandidates

• `Private` **\_defaultSubMeshCandidates**: [`ISmartArrayLike`](../interfaces/ISmartArrayLike.md)[`SubMesh`](SubMesh.md)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1570

___

### \_engine

• `Private` **\_engine**: [`Engine`](Engine.md)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1197

___

### \_executeWhenReadyTimeoutId

• `Private` **\_executeWhenReadyTimeoutId**: [`Nullable`](../modules.md#nullable)`Timeout` = `null`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1231

___

### \_externalData

• `Private` **\_externalData**: [`StringDictionary`](StringDictionary.md)`Object`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1295

___

### \_fogEnabled

• `Private` **\_fogEnabled**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:907

___

### \_fogMode

• `Private` **\_fogMode**: `number` = `Scene.FOGMODE_NONE`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:924

___

### \_forcePointsCloud

• `Private` **\_forcePointsCloud**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:286

___

### \_forceWireframe

• `Private` **\_forceWireframe**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:257

___

### \_frameId

• `Private` **\_frameId**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1230

___

### \_geometriesByUniqueId

• `Private` **\_geometriesByUniqueId**: [`Nullable`](../modules.md#nullable){ `[uniqueId: string]`: `number` \| `undefined`;  } = `null`

an optional map from Geometry Id to Geometry index in the 'geometries' array

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1474

___

### \_intermediateRendering

• `Private` **\_intermediateRendering**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1232

___

### \_isDisposed

• `Private` **\_isDisposed**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1244

___

### \_lightsEnabled

• `Private` **\_lightsEnabled**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:999

___

### \_materialsRenderTargets

• `Private` **\_materialsRenderTargets**: [`SmartArrayNoDuplicate`](SmartArrayNoDuplicate.md)[`RenderTargetTexture`](RenderTargetTexture.md)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1254

___

### \_meshesForIntersections

• `Private` **\_meshesForIntersections**: [`SmartArrayNoDuplicate`](SmartArrayNoDuplicate.md)[`AbstractMesh`](AbstractMesh.md)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1188

___

### \_onAfterCameraRenderObserver

• `Private` **\_onAfterCameraRenderObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Camera`](Camera.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:504

___

### \_onAfterRenderObserver

• `Private` **\_onAfterRenderObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Scene`](Scene.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:446

___

### \_onBeforeCameraRenderObserver

• `Private` **\_onBeforeCameraRenderObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Camera`](Camera.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:488

___

### \_onBeforeRenderObserver

• `Private` **\_onBeforeRenderObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Scene`](Scene.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:424

___

### \_onDisposeObserver

• `Private` **\_onDisposeObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Scene`](Scene.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:410

___

### \_perfCollector

• `Protected` **\_perfCollector**: [`Nullable`](../modules.md#nullable)[`PerformanceViewerCollector`](PerformanceViewerCollector.md) = `null`

Internal perfCollector instance used for sharing between inspector and playground.
Marked as protected to allow sharing between prototype extensions, but disallow access at toplevel.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:5331

___

### \_preventFreeActiveMeshesAndRenderingGroups

• `Private` **\_preventFreeActiveMeshesAndRenderingGroups**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3608

___

### \_processedMaterials

• `Private` **\_processedMaterials**: [`SmartArray`](SmartArray.md)[`Material`](Material.md)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1252

___

### \_projectionUpdateFlag

• `Private` **\_projectionUpdateFlag**: `number` = `-1`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1236

___

### \_renderId

• `Private` **\_renderId**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1229

___

### \_renderTargets

• `Private` **\_renderTargets**: [`SmartArrayNoDuplicate`](SmartArrayNoDuplicate.md)[`RenderTargetTexture`](RenderTargetTexture.md)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1253

___

### \_renderingManager

• `Private` **\_renderingManager**: [`RenderingManager`](RenderingManager.md)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1260

___

### \_sceneUbo

• `Private` **\_sceneUbo**: [`UniformBuffer`](UniformBuffer.md)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1266

___

### \_shadowsEnabled

• `Private` **\_shadowsEnabled**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:984

___

### \_skeletonsEnabled

• `Private` **\_skeletonsEnabled**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1086

___

### \_skipEvaluateActiveMeshesCompletely

• `Private` **\_skipEvaluateActiveMeshesCompletely**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3703

___

### \_skipFrustumClipping

• `Private` **\_skipFrustumClipping**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:272

___

### \_softwareSkinnedMeshes

• `Private` **\_softwareSkinnedMeshes**: [`SmartArrayNoDuplicate`](SmartArrayNoDuplicate.md)[`Mesh`](Mesh.md)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1258

___

### \_texturesEnabled

• `Private` **\_texturesEnabled**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1051

___

### \_timeAccumulator

• `Private` **\_timeAccumulator**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:874

___

### \_totalVertices

• `Private` **\_totalVertices**: [`PerfCounter`](PerfCounter.md)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1200

___

### \_transformMatrix

• `Private` **\_transformMatrix**: [`Matrix`](Matrix.md)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1265

___

### \_transientComponents

• `Private` **\_transientComponents**: [`ISceneComponent`](../interfaces/ISceneComponent.md)[] = `[]`

List of components to register on the next registration step.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1313

___

### \_uid

• `Private` **\_uid**: [`Nullable`](../modules.md#nullable)`string`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1296

___

### \_useRightHandedSystem

• `Private` **\_useRightHandedSystem**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:858

___

### \_viewUpdateFlag

• `Private` **\_viewUpdateFlag**: `number` = `-1`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1235

___

### actionManager

• **actionManager**: [`AbstractActionManager`](AbstractActionManager.md)

Gets or sets the action manager associated with the scene

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1186

___

### actionManagers

• **actionManagers**: [`AbstractActionManager`](AbstractActionManager.md)[]

ActionManagers available on the scene.

**`Deprecated`**

#### Inherited from

[AbstractScene](AbstractScene.md).[actionManagers](AbstractScene.md#actionmanagers)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:192

___

### activeCameras

• **activeCameras**: [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md)[]

All of the active cameras added to this scene.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1016

___

### ambientColor

• **ambientColor**: [`Color3`](Color3.md)

Defines the color used to simulate the ambient color (Default is (0, 0, 0))

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:201

___

### animationGroups

• **animationGroups**: [`AnimationGroup`](AnimationGroup.md)[]

All of the animation groups added to this scene

**`See`**

https://doc.babylonjs.com/divingDeeper/animation/groupAnimations

#### Inherited from

[AbstractScene](AbstractScene.md).[animationGroups](AbstractScene.md#animationgroups)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:151

___

### animationTimeScale

• **animationTimeScale**: `number` = `1`

Gets or sets a general scale for animation speed

**`See`**

https://www.babylonjs-playground.com/#IBU2W7#3

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1220

___

### animations

• **animations**: [`Animation`](Animation.md)[] = `[]`

Gets a list of Animations associated with the scene

#### Implementation of

[IAnimatable](../interfaces/IAnimatable.md).[animations](../interfaces/IAnimatable.md#animations)

#### Inherited from

[AbstractScene](AbstractScene.md).[animations](AbstractScene.md#animations)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:145

___

### animationsEnabled

• **animationsEnabled**: `boolean` = `true`

Gets or sets a boolean indicating if animations are enabled

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:334

___

### audioEnabled

• **audioEnabled**: `boolean`

Gets or sets if audio support is enabled

**`See`**

https://doc.babylonjs.com/how_to/playing_sounds_and_music

#### Defined in

https://github.com/babylon.js/core/src/Audio/audioSceneComponent.ts:84

___

### audioListenerPositionProvider

• **audioListenerPositionProvider**: [`Nullable`](../modules.md#nullable)() => [`Vector3`](Vector3.md)

Gets or sets custom audio listener position provider

**`See`**

https://doc.babylonjs.com/how_to/playing_sounds_and_music

#### Defined in

https://github.com/babylon.js/core/src/Audio/audioSceneComponent.ts:96

___

### audioPositioningRefreshRate

• **audioPositioningRefreshRate**: `number`

Gets or sets a refresh rate when using 3D audio positioning

#### Defined in

https://github.com/babylon.js/core/src/Audio/audioSceneComponent.ts:101

___

### autoClear

• **autoClear**: `boolean` = `true`

Gets or sets a boolean that indicates if the scene must clear the render buffer before rendering a frame

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:189

___

### autoClearDepthAndStencil

• **autoClearDepthAndStencil**: `boolean` = `true`

Gets or sets a boolean that indicates if the scene must clear the depth and stencil buffers before rendering a frame

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:193

___

### cameraToUseForPointers

• **cameraToUseForPointers**: [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md) = `null`

Define this parameter if you are using multiple cameras and you want to specify which one should be used for pointer position

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:178

___

### cameras

• **cameras**: [`Camera`](Camera.md)[]

All of the cameras added to this scene

**`See`**

https://doc.babylonjs.com/babylon101/cameras

#### Inherited from

[AbstractScene](AbstractScene.md).[cameras](AbstractScene.md#cameras)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:117

___

### clearColor

• **clearColor**: [`Color4`](Color4.md)

Defines the color used to clear the render buffer (Default is (0.2, 0.2, 0.3, 1.0))

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:197

___

### clipPlane

• **clipPlane**: [`Nullable`](../modules.md#nullable)[`Plane`](Plane.md)

Gets or sets the active clipplane 1

#### Implementation of

IClipPlanesHolder.clipPlane

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:304

___

### clipPlane2

• **clipPlane2**: [`Nullable`](../modules.md#nullable)[`Plane`](Plane.md)

Gets or sets the active clipplane 2

#### Implementation of

IClipPlanesHolder.clipPlane2

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:309

___

### clipPlane3

• **clipPlane3**: [`Nullable`](../modules.md#nullable)[`Plane`](Plane.md)

Gets or sets the active clipplane 3

#### Implementation of

IClipPlanesHolder.clipPlane3

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:314

___

### clipPlane4

• **clipPlane4**: [`Nullable`](../modules.md#nullable)[`Plane`](Plane.md)

Gets or sets the active clipplane 4

#### Implementation of

IClipPlanesHolder.clipPlane4

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:319

___

### clipPlane5

• **clipPlane5**: [`Nullable`](../modules.md#nullable)[`Plane`](Plane.md)

Gets or sets the active clipplane 5

#### Implementation of

IClipPlanesHolder.clipPlane5

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:324

___

### clipPlane6

• **clipPlane6**: [`Nullable`](../modules.md#nullable)[`Plane`](Plane.md)

Gets or sets the active clipplane 6

#### Implementation of

IClipPlanesHolder.clipPlane6

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:329

___

### collisionsEnabled

• **collisionsEnabled**: `boolean` = `true`

Gets or sets a boolean indicating if collisions are enabled on this scene

**`See`**

https://doc.babylonjs.com/babylon101/cameras,_mesh_collisions_and_gravity

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1113

___

### constantlyUpdateMeshUnderPointer

• **constantlyUpdateMeshUnderPointer**: `boolean` = `false`

Gets or sets a boolean indicating if the scene must keep the meshUnderPointer property updated
Please note that it requires to run a ray cast through the scene on every frame

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:358

___

### customLODSelector

• **customLODSelector**: (`mesh`: [`AbstractMesh`](AbstractMesh.md), `camera`: [`Camera`](Camera.md)) => [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

#### Type declaration

▸ (`mesh`, `camera`): [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

Gets or sets a user defined funtion to select LOD from a mesh and a camera.
By default this function is undefined and Babylon.js will select LOD based on distance to camera

##### Parameters

| Name | Type |
| :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) |
| `camera` | [`Camera`](Camera.md) |

##### Returns

[`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:685

___

### customRenderTargets

• **customRenderTargets**: [`RenderTargetTexture`](RenderTargetTexture.md)[]

The list of user defined render targets added to the scene

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1156

___

### debugLayer

• **debugLayer**: [`DebugLayer`](DebugLayer.md)

Gets the debug layer (aka Inspector) associated with the scene

**`See`**

https://doc.babylonjs.com/features/playground_debuglayer

#### Defined in

https://github.com/babylon.js/core/src/Debug/debugLayer.ts:102

___

### defaultCursor

• **defaultCursor**: `string` = `""`

Defines the HTML default cursor to use (empty by default)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:367

___

### deltaTime

• **deltaTime**: `number`

Gets the current delta time used by animation engine

#### Defined in

https://github.com/babylon.js/core/src/Animations/animatable.ts:638

___

### depthPeelingRenderer

• **depthPeelingRenderer**: [`Nullable`](../modules.md#nullable)[`DepthPeelingRenderer`](DepthPeelingRenderer.md)

The depth peeling renderer

#### Defined in

https://github.com/babylon.js/core/src/Rendering/depthPeelingSceneComponent.ts:13

___

### disableOfflineSupportExceptionRules

• **disableOfflineSupportExceptionRules**: `RegExp`[]

Use this array to add regular expressions used to disable offline support for specific urls

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:403

___

### dispatchAllSubMeshesOfActiveMeshes

• **dispatchAllSubMeshesOfActiveMeshes**: `boolean` = `false`

Gets or sets a boolean indicating that all submeshes of active meshes must be rendered
Use this boolean to avoid computing frustum clipping on submeshes (This could help when you are CPU bound)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1250

___

### doNotHandleCursors

• **doNotHandleCursors**: `boolean` = `false`

Defines whether cursors are handled by the scene.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:371

___

### dumpNextRenderTargets

• **dumpNextRenderTargets**: `boolean` = `false`

Gets or sets a boolean indicating if next render targets must be dumped as image for debugging purposes
We recommend not using it and instead rely on Spector.js: http://spector.babylonjs.com

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1152

___

### effectLayers

• **effectLayers**: [`EffectLayer`](EffectLayer.md)[]

The list of effect layers (highlights/glow) added to the scene

**`See`**

 - https://doc.babylonjs.com/how_to/highlight_layer
 - https://doc.babylonjs.com/how_to/glow_layer

#### Inherited from

[AbstractScene](AbstractScene.md).[effectLayers](AbstractScene.md#effectlayers)

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayerSceneComponent.ts:33

___

### environmentBRDFTexture

• **environmentBRDFTexture**: [`BaseTexture`](BaseTexture.md)

This is use to store the default BRDF lookup for PBR materials in your scene.
It should only be one of the following (if not the default embedded one):
* For uncorrelated BRDF (pbr.brdf.useEnergyConservation = false and pbr.brdf.useSmithVisibilityHeightCorrelated = false) : https://assets.babylonjs.com/environments/uncorrelatedBRDF.dds
* For correlated BRDF (pbr.brdf.useEnergyConservation = false and pbr.brdf.useSmithVisibilityHeightCorrelated = true) : https://assets.babylonjs.com/environments/correlatedBRDF.dds
* For correlated multi scattering BRDF (pbr.brdf.useEnergyConservation = true and pbr.brdf.useSmithVisibilityHeightCorrelated = true) : https://assets.babylonjs.com/environments/correlatedMSBRDF.dds
The material properties need to be setup according to the type of texture in use.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:211

___

### environmentIntensity

• **environmentIntensity**: `number` = `1`

Intensity of the environment in all pbr material.
This dims or reinforces the IBL lighting overall (reflection and diffuse).
As in the majority of the scene they are the same (exception for multi room and so on),
this is easier to reference from here than from all the materials.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:241

___

### fogColor

• **fogColor**: [`Color3`](Color3.md)

Gets or sets the fog color to use

**`See`**

https://doc.babylonjs.com/babylon101/environment#fog
(Default is Color3(0.2, 0.2, 0.3))

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:951

___

### fogDensity

• **fogDensity**: `number` = `0.1`

Gets or sets the fog density to use

**`See`**

https://doc.babylonjs.com/babylon101/environment#fog
(Default is 0.1)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:957

___

### fogEnd

• **fogEnd**: `number` = `1000.0`

Gets or sets the fog end distance to use

**`See`**

https://doc.babylonjs.com/babylon101/environment#fog
(Default is 1000)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:969

___

### fogStart

• **fogStart**: `number` = `0`

Gets or sets the fog start distance to use

**`See`**

https://doc.babylonjs.com/babylon101/environment#fog
(Default is 0)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:963

___

### forceShowBoundingBoxes

• **forceShowBoundingBoxes**: `boolean`

Gets or sets a boolean indicating if all bounding boxes must be rendered

#### Defined in

https://github.com/babylon.js/core/src/Rendering/boundingBoxRenderer.ts:35

___

### gamepadManager

• **gamepadManager**: [`GamepadManager`](GamepadManager.md)

Gets the gamepad manager associated with the scene

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_gamepads

#### Defined in

https://github.com/babylon.js/core/src/Gamepads/gamepadSceneComponent.ts:21

___

### geometries

• **geometries**: [`Geometry`](Geometry.md)[]

The list of geometries used in the scene.

#### Inherited from

[AbstractScene](AbstractScene.md).[geometries](AbstractScene.md#geometries)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:177

___

### geometryBufferRenderer

• **geometryBufferRenderer**: [`Nullable`](../modules.md#nullable)[`GeometryBufferRenderer`](GeometryBufferRenderer.md)

Gets or Sets the current geometry buffer associated to the scene.

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRendererSceneComponent.ts:17

___

### getActiveMeshCandidates

• **getActiveMeshCandidates**: () => [`ISmartArrayLike`](../interfaces/ISmartArrayLike.md)[`AbstractMesh`](AbstractMesh.md)

#### Type declaration

▸ (): [`ISmartArrayLike`](../interfaces/ISmartArrayLike.md)[`AbstractMesh`](AbstractMesh.md)

Lambda returning the list of potentially active meshes.

##### Returns

[`ISmartArrayLike`](../interfaces/ISmartArrayLike.md)[`AbstractMesh`](AbstractMesh.md)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3683

___

### getActiveSubMeshCandidates

• **getActiveSubMeshCandidates**: (`mesh`: [`AbstractMesh`](AbstractMesh.md)) => [`ISmartArrayLike`](../interfaces/ISmartArrayLike.md)[`SubMesh`](SubMesh.md)

#### Type declaration

▸ (`mesh`): [`ISmartArrayLike`](../interfaces/ISmartArrayLike.md)[`SubMesh`](SubMesh.md)

Lambda returning the list of potentially active sub meshes.

##### Parameters

| Name | Type |
| :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) |

##### Returns

[`ISmartArrayLike`](../interfaces/ISmartArrayLike.md)[`SubMesh`](SubMesh.md)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3688

___

### getCollidingSubMeshCandidates

• **getCollidingSubMeshCandidates**: (`mesh`: [`AbstractMesh`](AbstractMesh.md), `collider`: `Collider`) => [`ISmartArrayLike`](../interfaces/ISmartArrayLike.md)[`SubMesh`](SubMesh.md)

#### Type declaration

▸ (`mesh`, `collider`): [`ISmartArrayLike`](../interfaces/ISmartArrayLike.md)[`SubMesh`](SubMesh.md)

Lambda returning the list of potentially colliding sub meshes.

##### Parameters

| Name | Type |
| :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) |
| `collider` | `Collider` |

##### Returns

[`ISmartArrayLike`](../interfaces/ISmartArrayLike.md)[`SubMesh`](SubMesh.md)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3698

___

### getDeterministicFrameTime

• **getDeterministicFrameTime**: () => `number`

#### Type declaration

▸ (): `number`

User updatable function that will return a deterministic frame time when engine is in deterministic lock step mode

##### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:4242

___

### getIntersectingSubMeshCandidates

• **getIntersectingSubMeshCandidates**: (`mesh`: [`AbstractMesh`](AbstractMesh.md), `localRay`: [`Ray`](Ray.md)) => [`ISmartArrayLike`](../interfaces/ISmartArrayLike.md)[`SubMesh`](SubMesh.md)

#### Type declaration

▸ (`mesh`, `localRay`): [`ISmartArrayLike`](../interfaces/ISmartArrayLike.md)[`SubMesh`](SubMesh.md)

Lambda returning the list of potentially intersecting sub meshes.

##### Parameters

| Name | Type |
| :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) |
| `localRay` | [`Ray`](Ray.md) |

##### Returns

[`ISmartArrayLike`](../interfaces/ISmartArrayLike.md)[`SubMesh`](SubMesh.md)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3693

___

### gravity

• **gravity**: [`Vector3`](Vector3.md)

Defines the gravity applied to this scene (used only for collisions)

**`See`**

https://doc.babylonjs.com/babylon101/cameras,_mesh_collisions_and_gravity

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1131

___

### headphone

• **headphone**: `boolean`

Gets or sets if audio will be output to headphones

**`See`**

https://doc.babylonjs.com/how_to/playing_sounds_and_music

#### Defined in

https://github.com/babylon.js/core/src/Audio/audioSceneComponent.ts:90

___

### hoverCursor

• **hoverCursor**: `string` = `"pointer"`

Defines the HTML cursor to use when hovering over interactive elements

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:363

___

### importedMeshesFiles

• **importedMeshesFiles**: `string`[]

Gets the list of meshes imported to the scene through SceneLoader

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1167

___

### layers

• **layers**: [`Layer`](Layer.md)[]

The list of layers (background and foreground) of the scene

#### Inherited from

[AbstractScene](AbstractScene.md).[layers](AbstractScene.md#layers)

#### Defined in

https://github.com/babylon.js/core/src/Layers/layerSceneComponent.ts:16

___

### lensFlareSystems

• **lensFlareSystems**: [`LensFlareSystem`](LensFlareSystem.md)[]

The list of lens flare system added to the scene

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_lens_flares

#### Inherited from

[AbstractScene](AbstractScene.md).[lensFlareSystems](AbstractScene.md#lensflaresystems)

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlareSystemSceneComponent.ts:32

___

### lensFlaresEnabled

• **lensFlaresEnabled**: `boolean` = `true`

Gets or sets a boolean indicating if lens flares are enabled on this scene

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1106

___

### lights

• **lights**: [`Light`](Light.md)[]

All of the lights added to this scene

**`See`**

https://doc.babylonjs.com/babylon101/lights

#### Inherited from

[AbstractScene](AbstractScene.md).[lights](AbstractScene.md#lights)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:123

___

### loadingPluginName

• **loadingPluginName**: `string`

Gets the name of the plugin used to load this scene (null by default)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:398

___

### mainSoundTrack

• **mainSoundTrack**: [`SoundTrack`](SoundTrack.md)

The main sound track played by the scene.
It contains your primary collection of sounds.

#### Defined in

https://github.com/babylon.js/core/src/Audio/audioSceneComponent.ts:66

___

### materials

• **materials**: [`Material`](Material.md)[]

All of the materials added to this scene
In the context of a Scene, it is not supposed to be modified manually.
Any addition or removal should be done using the addMaterial and removeMaterial Scene methods.
Note also that the order of the Material within the array is not significant and might change.

**`See`**

https://doc.babylonjs.com/babylon101/materials

#### Inherited from

[AbstractScene](AbstractScene.md).[materials](AbstractScene.md#materials)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:166

___

### meshes

• **meshes**: [`AbstractMesh`](AbstractMesh.md)[]

All of the (abstract) meshes added to this scene

#### Inherited from

[AbstractScene](AbstractScene.md).[meshes](AbstractScene.md#meshes)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:128

___

### metadata

• **metadata**: `any` = `null`

Gets or sets user defined metadata

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:388

___

### morphTargetManagers

• **morphTargetManagers**: [`MorphTargetManager`](MorphTargetManager.md)[]

The list of morph target managers added to the scene

**`See`**

https://doc.babylonjs.com/how_to/how_to_dynamically_morph_a_mesh

#### Inherited from

[AbstractScene](AbstractScene.md).[morphTargetManagers](AbstractScene.md#morphtargetmanagers)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:172

___

### multiMaterials

• **multiMaterials**: [`MultiMaterial`](MultiMaterial.md)[]

All of the multi-materials added to this scene

**`See`**

https://doc.babylonjs.com/how_to/multi_materials

#### Inherited from

[AbstractScene](AbstractScene.md).[multiMaterials](AbstractScene.md#multimaterials)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:157

___

### needsPreviousWorldMatrices

• **needsPreviousWorldMatrices**: `boolean` = `false`

Flag indicating if we need to store previous matrices when rendering

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:981

___

### offlineProvider

• **offlineProvider**: [`IOfflineProvider`](../interfaces/IOfflineProvider.md)

Gets or sets the current offline provider to use to store scene data

**`See`**

https://doc.babylonjs.com/how_to/caching_resources_in_indexeddb

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1180

___

### onActiveCameraChanged

• **onActiveCameraChanged**: [`Observable`](Observable.md)[`Scene`](Scene.md)

An event triggered when the activeCamera property is updated

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:655

___

### onAfterActiveMeshesEvaluationObservable

• **onAfterActiveMeshesEvaluationObservable**: [`Observable`](Observable.md)[`Scene`](Scene.md)

An event triggered when active meshes evaluation is done

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:521

___

### onAfterAnimationsObservable

• **onAfterAnimationsObservable**: [`Observable`](Observable.md)[`Scene`](Scene.md)

An event triggered after animations processing

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:466

___

### onAfterCameraRenderObservable

• **onAfterCameraRenderObservable**: [`Observable`](Observable.md)[`Camera`](Camera.md)

An event triggered after rendering a camera
This is triggered for the full rig Camera only unlike onAfterRenderCameraObservable

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:502

___

### onAfterDrawPhaseObservable

• **onAfterDrawPhaseObservable**: [`Observable`](Observable.md)[`Scene`](Scene.md)

An event triggered after draw calls have been sent

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:476

___

### onAfterParticlesRenderingObservable

• **onAfterParticlesRenderingObservable**: [`Observable`](Observable.md)[`Scene`](Scene.md)

An event triggered when particles rendering is done
Note: This event can be trigger more than once per frame (because particles can be rendered by render target textures as well)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:533

___

### onAfterPhysicsObservable

• **onAfterPhysicsObservable**: [`Observable`](Observable.md)[`Scene`](Scene.md)

An event triggered when physic simulation has been done

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsEngineComponent.ts:64

___

### onAfterRenderCameraObservable

• **onAfterRenderCameraObservable**: [`Observable`](Observable.md)[`Camera`](Camera.md)

An event triggered after rendering the scene for an active camera (When scene.render is called this will be called after each camera)
This is triggered for each "sub" camera in a Camera Rig unlike onAfterCameraRenderObservable

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:444

___

### onAfterRenderObservable

• **onAfterRenderObservable**: [`Observable`](Observable.md)[`Scene`](Scene.md)

An event triggered after rendering the scene

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:438

___

### onAfterRenderTargetsRenderObservable

• **onAfterRenderTargetsRenderObservable**: [`Observable`](Observable.md)[`Scene`](Scene.md)

An event triggered when render targets were rendered.
Can happen multiple times per frame.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:640

___

### onAfterRenderingGroupObservable

• **onAfterRenderingGroupObservable**: [`Observable`](Observable.md)[`RenderingGroupInfo`](RenderingGroupInfo.md)

This Observable will be triggered after rendering each renderingGroup of each rendered camera.
The RenderingGroupInfo class contains all the information about the context in which the observable is called
If you wish to register an Observer only for a given set of renderingGroup, use the mask with a combination of the renderingGroup index elevated to the power of two (1 for renderingGroup 0, 2 for renderingrOup1, 4 for 2 and 8 for 3)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:669

___

### onAfterSpritesRenderingObservable

• **onAfterSpritesRenderingObservable**: [`Observable`](Observable.md)[`Scene`](Scene.md)

An event triggered when sprites rendering is done
Note: This event can be trigger more than once per frame (because sprites can be rendered by render target textures as well)

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteSceneComponent.ts:42

___

### onAfterStepObservable

• **onAfterStepObservable**: [`Observable`](Observable.md)[`Scene`](Scene.md)

An event triggered after calculating deterministic simulation step

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:650

___

### onAnimationFileImportedObservable

• **onAnimationFileImportedObservable**: [`Observable`](Observable.md)[`Scene`](Scene.md)

This Observable will when an animation file has been imported into the scene.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:679

___

### onBeforeActiveMeshesEvaluationObservable

• **onBeforeActiveMeshesEvaluationObservable**: [`Observable`](Observable.md)[`Scene`](Scene.md)

An event triggered when active meshes evaluation is about to start

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:516

___

### onBeforeAnimationsObservable

• **onBeforeAnimationsObservable**: [`Observable`](Observable.md)[`Scene`](Scene.md)

An event triggered before animating the scene

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:461

___

### onBeforeCameraRenderObservable

• **onBeforeCameraRenderObservable**: [`Observable`](Observable.md)[`Camera`](Camera.md)

An event triggered before rendering a camera

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:486

___

### onBeforeDrawPhaseObservable

• **onBeforeDrawPhaseObservable**: [`Observable`](Observable.md)[`Scene`](Scene.md)

An event triggered before draw calls are ready to be sent

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:471

___

### onBeforeParticlesRenderingObservable

• **onBeforeParticlesRenderingObservable**: [`Observable`](Observable.md)[`Scene`](Scene.md)

An event triggered when particles rendering is about to start
Note: This event can be trigger more than once per frame (because particles can be rendered by render target textures as well)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:527

___

### onBeforePhysicsObservable

• **onBeforePhysicsObservable**: [`Observable`](Observable.md)[`Scene`](Scene.md)

An event triggered when physic simulation is about to be run

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsEngineComponent.ts:59

___

### onBeforeRenderObservable

• **onBeforeRenderObservable**: [`Observable`](Observable.md)[`Scene`](Scene.md)

An event triggered before rendering the scene (right after animations and physics)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:422

___

### onBeforeRenderTargetsRenderObservable

• **onBeforeRenderTargetsRenderObservable**: [`Observable`](Observable.md)[`Scene`](Scene.md)

An event triggered when render targets are about to be rendered
Can happen multiple times per frame.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:634

___

### onBeforeRenderingGroupObservable

• **onBeforeRenderingGroupObservable**: [`Observable`](Observable.md)[`RenderingGroupInfo`](RenderingGroupInfo.md)

This Observable will be triggered before rendering each renderingGroup of each rendered camera.
The RenderingGroupInfo class contains all the information about the context in which the observable is called
If you wish to register an Observer only for a given set of renderingGroup, use the mask with a combination of the renderingGroup index elevated to the power of two (1 for renderingGroup 0, 2 for renderingrOup1, 4 for 2 and 8 for 3)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:662

___

### onBeforeSpritesRenderingObservable

• **onBeforeSpritesRenderingObservable**: [`Observable`](Observable.md)[`Scene`](Scene.md)

An event triggered when sprites rendering is about to start
Note: This event can be trigger more than once per frame (because sprites can be rendered by render target textures as well)

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteSceneComponent.ts:36

___

### onBeforeStepObservable

• **onBeforeStepObservable**: [`Observable`](Observable.md)[`Scene`](Scene.md)

An event triggered before calculating deterministic simulation step

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:645

___

### onCameraRemovedObservable

• **onCameraRemovedObservable**: [`Observable`](Observable.md)[`Camera`](Camera.md)

An event triggered when a camera is removed

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:548

___

### onComputePressureChanged

• **onComputePressureChanged**: [`Observable`](Observable.md)[`IComputePressureData`](../interfaces/IComputePressureData.md)

An event triggered when the cpu usage/speed meets certain thresholds.
Note: Compute pressure is an experimental API.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:5347

___

### onDataLoadedObservable

• **onDataLoadedObservable**: [`Observable`](Observable.md)[`Scene`](Scene.md)

An event triggered when SceneLoader.Append or SceneLoader.Load or SceneLoader.ImportMesh were successfully executed

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:538

___

### onDisposeObservable

• **onDisposeObservable**: [`Observable`](Observable.md)[`Scene`](Scene.md)

An event triggered when the scene is disposed.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:408

___

### onGeometryRemovedObservable

• **onGeometryRemovedObservable**: [`Observable`](Observable.md)[`Geometry`](Geometry.md)

An event triggered when a geometry is removed

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:568

___

### onKeyboardObservable

• **onKeyboardObservable**: [`Observable`](Observable.md)[`KeyboardInfo`](KeyboardInfo.md)

Observable event triggered each time an keyboard event is received from the hosting window

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:854

___

### onLightRemovedObservable

• **onLightRemovedObservable**: [`Observable`](Observable.md)[`Light`](Light.md)

An event triggered when a light is removed

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:558

___

### onMaterialRemovedObservable

• **onMaterialRemovedObservable**: [`Observable`](Observable.md)[`Material`](Material.md)

An event triggered when a material is removed

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:613

___

### onMeshImportedObservable

• **onMeshImportedObservable**: [`Observable`](Observable.md)[`AbstractMesh`](AbstractMesh.md)

This Observable will when a mesh has been imported into the scene.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:674

___

### onMeshRemovedObservable

• **onMeshRemovedObservable**: [`Observable`](Observable.md)[`AbstractMesh`](AbstractMesh.md)

An event triggered when a mesh is removed

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:588

___

### onMultiMaterialRemovedObservable

• **onMultiMaterialRemovedObservable**: [`Observable`](Observable.md)[`MultiMaterial`](MultiMaterial.md)

An event triggered when a multi material is removed

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:618

___

### onNewCameraAddedObservable

• **onNewCameraAddedObservable**: [`Observable`](Observable.md)[`Camera`](Camera.md)

An event triggered when a camera is created

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:543

___

### onNewGeometryAddedObservable

• **onNewGeometryAddedObservable**: [`Observable`](Observable.md)[`Geometry`](Geometry.md)

An event triggered when a geometry is created

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:563

___

### onNewLightAddedObservable

• **onNewLightAddedObservable**: [`Observable`](Observable.md)[`Light`](Light.md)

An event triggered when a light is created

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:553

___

### onNewMaterialAddedObservable

• **onNewMaterialAddedObservable**: [`Observable`](Observable.md)[`Material`](Material.md)

An event triggered when a material is created

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:603

___

### onNewMeshAddedObservable

• **onNewMeshAddedObservable**: [`Observable`](Observable.md)[`AbstractMesh`](AbstractMesh.md)

An event triggered when a mesh is created

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:583

___

### onNewMultiMaterialAddedObservable

• **onNewMultiMaterialAddedObservable**: [`Observable`](Observable.md)[`MultiMaterial`](MultiMaterial.md)

An event triggered when a multi material is created

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:608

___

### onNewSkeletonAddedObservable

• **onNewSkeletonAddedObservable**: [`Observable`](Observable.md)[`Skeleton`](Skeleton.md)

An event triggered when a skeleton is created

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:593

___

### onNewTextureAddedObservable

• **onNewTextureAddedObservable**: [`Observable`](Observable.md)[`BaseTexture`](BaseTexture.md)

An event triggered when a texture is created

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:623

___

### onNewTransformNodeAddedObservable

• **onNewTransformNodeAddedObservable**: [`Observable`](Observable.md)[`TransformNode`](TransformNode.md)

An event triggered when a transform node is created

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:573

___

### onPointerDown

• **onPointerDown**: (`evt`: [`IPointerEvent`](../interfaces/IPointerEvent.md), `pickInfo`: [`PickingInfo`](PickingInfo.md), `type`: [`PointerEventTypes`](PointerEventTypes.md)) => `void`

#### Type declaration

▸ (`evt`, `pickInfo`, `type`): `void`

Callback called when a pointer down is detected

##### Parameters

| Name | Type |
| :------ | :------ |
| `evt` | [`IPointerEvent`](../interfaces/IPointerEvent.md) |
| `pickInfo` | [`PickingInfo`](PickingInfo.md) |
| `type` | [`PointerEventTypes`](PointerEventTypes.md) |

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:725

___

### onPointerMove

• **onPointerMove**: (`evt`: [`IPointerEvent`](../interfaces/IPointerEvent.md), `pickInfo`: [`PickingInfo`](PickingInfo.md), `type`: [`PointerEventTypes`](PointerEventTypes.md)) => `void`

#### Type declaration

▸ (`evt`, `pickInfo`, `type`): `void`

Callback called when a pointer move is detected

##### Parameters

| Name | Type |
| :------ | :------ |
| `evt` | [`IPointerEvent`](../interfaces/IPointerEvent.md) |
| `pickInfo` | [`PickingInfo`](PickingInfo.md) |
| `type` | [`PointerEventTypes`](PointerEventTypes.md) |

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:723

___

### onPointerObservable

• **onPointerObservable**: [`Observable`](Observable.md)[`PointerInfo`](PointerInfo.md)

Observable event triggered each time an input event is received from the rendering canvas

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:745

___

### onPointerPick

• **onPointerPick**: (`evt`: [`IPointerEvent`](../interfaces/IPointerEvent.md), `pickInfo`: [`PickingInfo`](PickingInfo.md)) => `void`

#### Type declaration

▸ (`evt`, `pickInfo`): `void`

Callback called when a pointer pick is detected

##### Parameters

| Name | Type |
| :------ | :------ |
| `evt` | [`IPointerEvent`](../interfaces/IPointerEvent.md) |
| `pickInfo` | [`PickingInfo`](PickingInfo.md) |

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:729

___

### onPointerUp

• **onPointerUp**: (`evt`: [`IPointerEvent`](../interfaces/IPointerEvent.md), `pickInfo`: [`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md), `type`: [`PointerEventTypes`](PointerEventTypes.md)) => `void`

#### Type declaration

▸ (`evt`, `pickInfo`, `type`): `void`

Callback called when a pointer up is detected

##### Parameters

| Name | Type |
| :------ | :------ |
| `evt` | [`IPointerEvent`](../interfaces/IPointerEvent.md) |
| `pickInfo` | [`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md) |
| `type` | [`PointerEventTypes`](PointerEventTypes.md) |

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:727

___

### onPreKeyboardObservable

• **onPreKeyboardObservable**: [`Observable`](Observable.md)[`KeyboardInfoPre`](KeyboardInfoPre.md)

This observable event is triggered when any keyboard event si raised and registered during Scene.attachControl()
You have the possibility to skip the process and the call to onKeyboardObservable by setting KeyboardInfoPre.skipOnPointerObservable to true

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:849

___

### onPrePointerObservable

• **onPrePointerObservable**: [`Observable`](Observable.md)[`PointerInfoPre`](PointerInfoPre.md)

This observable event is triggered when any ponter event is triggered. It is registered during Scene.attachControl() and it is called BEFORE the 3D engine process anything (mesh/sprite picking for instance).
You have the possibility to skip the process and the call to onPointerObservable by setting PointerInfoPre.skipOnPointerObservable to true

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:740

___

### onReadyObservable

• **onReadyObservable**: [`Observable`](Observable.md)[`Scene`](Scene.md)

An event triggered when the scene is ready

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:481

___

### onSkeletonRemovedObservable

• **onSkeletonRemovedObservable**: [`Observable`](Observable.md)[`Skeleton`](Skeleton.md)

An event triggered when a skeleton is removed

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:598

___

### onTextureRemovedObservable

• **onTextureRemovedObservable**: [`Observable`](Observable.md)[`BaseTexture`](BaseTexture.md)

An event triggered when a texture is removed

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:628

___

### onTransformNodeRemovedObservable

• **onTransformNodeRemovedObservable**: [`Observable`](Observable.md)[`TransformNode`](TransformNode.md)

An event triggered when a transform node is removed

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:578

___

### particleSystems

• **particleSystems**: [`IParticleSystem`](../interfaces/IParticleSystem.md)[]

All of the particle systems added to this scene

**`See`**

https://doc.babylonjs.com/babylon101/particles

#### Inherited from

[AbstractScene](AbstractScene.md).[particleSystems](AbstractScene.md#particlesystems)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:140

___

### particlesEnabled

• **particlesEnabled**: `boolean` = `true`

Gets or sets a boolean indicating if particles are enabled on this scene

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1077

___

### physicsEnabled

• **physicsEnabled**: `boolean` = `true`

Gets or sets a boolean indicating if physic engines are enabled on this scene

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1071

___

### pointerDownPredicate

• **pointerDownPredicate**: (`Mesh`: [`AbstractMesh`](AbstractMesh.md)) => `boolean`

#### Type declaration

▸ (`Mesh`): `boolean`

Gets or sets a predicate used to select candidate meshes for a pointer down event

##### Parameters

| Name | Type |
| :------ | :------ |
| `Mesh` | [`AbstractMesh`](AbstractMesh.md) |

##### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:696

___

### pointerMovePredicate

• **pointerMovePredicate**: (`Mesh`: [`AbstractMesh`](AbstractMesh.md)) => `boolean`

#### Type declaration

▸ (`Mesh`): `boolean`

Gets or sets a predicate used to select candidate meshes for a pointer move event

##### Parameters

| Name | Type |
| :------ | :------ |
| `Mesh` | [`AbstractMesh`](AbstractMesh.md) |

##### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:705

___

### pointerMoveTrianglePredicate

• **pointerMoveTrianglePredicate**: `undefined` \| (`p0`: [`Vector3`](Vector3.md), `p1`: [`Vector3`](Vector3.md), `p2`: [`Vector3`](Vector3.md), `ray`: [`Ray`](Ray.md)) => `boolean`

Gets or sets a predicate used to select candidate faces for a pointer move event

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:734

___

### pointerUpPredicate

• **pointerUpPredicate**: (`Mesh`: [`AbstractMesh`](AbstractMesh.md)) => `boolean`

#### Type declaration

▸ (`Mesh`): `boolean`

Gets or sets a predicate used to select candidate meshes for a pointer up event

##### Parameters

| Name | Type |
| :------ | :------ |
| `Mesh` | [`AbstractMesh`](AbstractMesh.md) |

##### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:700

___

### postProcessManager

• **postProcessManager**: [`PostProcessManager`](PostProcessManager.md)

Gets the current postprocess manager

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1141

___

### postProcessRenderPipelineManager

• `Readonly` **postProcessRenderPipelineManager**: [`PostProcessRenderPipelineManager`](PostProcessRenderPipelineManager.md)

Gets the postprocess render pipeline manager

**`See`**

 - https://doc.babylonjs.com/how_to/how_to_use_postprocessrenderpipeline
 - https://doc.babylonjs.com/how_to/using_default_rendering_pipeline

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/RenderPipeline/postProcessRenderPipelineManagerSceneComponent.ts:16

___

### postProcesses

• **postProcesses**: [`PostProcess`](PostProcess.md)[]

The list of postprocesses added to the scene

#### Inherited from

[AbstractScene](AbstractScene.md).[postProcesses](AbstractScene.md#postprocesses)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:217

___

### postProcessesEnabled

• **postProcessesEnabled**: `boolean` = `true`

Gets or sets a boolean indicating if postprocesses are enabled on this scene

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1137

___

### prePassRenderer

• **prePassRenderer**: [`Nullable`](../modules.md#nullable)[`PrePassRenderer`](PrePassRenderer.md)

Gets or Sets the current prepass renderer associated to the scene.

#### Inherited from

[AbstractScene](AbstractScene.md).[prePassRenderer](AbstractScene.md#prepassrenderer)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRendererSceneComponent.ts:23

___

### preventDefaultOnPointerDown

• **preventDefaultOnPointerDown**: `boolean` = `true`

This is used to call preventDefault() on pointer down
in order to block unwanted artifacts like system double clicks

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:376

___

### preventDefaultOnPointerUp

• **preventDefaultOnPointerUp**: `boolean` = `true`

This is used to call preventDefault() on pointer up
in order to block unwanted artifacts like system double clicks

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:382

___

### probesEnabled

• **probesEnabled**: `boolean` = `true`

Gets or sets a boolean indicating if probes are enabled on this scene

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1173

___

### proceduralTextures

• **proceduralTextures**: [`ProceduralTexture`](ProceduralTexture.md)[]

The list of procedural textures added to the scene

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_procedural_textures

#### Inherited from

[AbstractScene](AbstractScene.md).[proceduralTextures](AbstractScene.md#proceduraltextures)

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Procedurals/proceduralTextureSceneComponent.ts:14

___

### proceduralTexturesEnabled

• **proceduralTexturesEnabled**: `boolean` = `true`

Gets or sets a boolean indicating if procedural textures are enabled on this scene

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1194

___

### reflectionProbes

• **reflectionProbes**: [`ReflectionProbe`](ReflectionProbe.md)[]

The list of reflection probes added to the scene

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_reflection_probes

#### Inherited from

[AbstractScene](AbstractScene.md).[reflectionProbes](AbstractScene.md#reflectionprobes)

#### Defined in

https://github.com/babylon.js/core/src/Probes/reflectionProbe.ts:17

___

### renderTargetsEnabled

• **renderTargetsEnabled**: `boolean` = `true`

Gets or sets a boolean indicating if render targets are enabled on this scene

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1147

___

### requireLightSorting

• **requireLightSorting**: `boolean` = `false`

Gets or sets a boolean indicating if lights must be sorted by priority (off by default)
This is useful if there are more lights that the maximum simulteanous authorized

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1288

___

### reservedDataStore

• **reservedDataStore**: `any` = `null`

For internal use only. Please do not use.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:393

___

### rootNodes

• **rootNodes**: [`Node`](Node.md)[]

Gets the list of root nodes (ie. nodes with no parent)

#### Inherited from

[AbstractScene](AbstractScene.md).[rootNodes](AbstractScene.md#rootnodes)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:112

___

### selectionOctree

• **selectionOctree**: [`Octree`](Octree.md)[`AbstractMesh`](AbstractMesh.md)

Gets the octree used to boost mesh selection (picking)

**`See`**

https://doc.babylonjs.com/how_to/optimizing_your_scene_with_octrees

#### Defined in

https://github.com/babylon.js/core/src/Culling/Octrees/octreeSceneComponent.ts:26

___

### simplificationQueue

• **simplificationQueue**: [`SimplificationQueue`](SimplificationQueue.md)

Gets or sets the simplification queue attached to the scene

**`See`**

https://doc.babylonjs.com/how_to/in-browser_mesh_simplification

#### Defined in

https://github.com/babylon.js/core/src/Meshes/meshSimplificationSceneComponent.ts:17

___

### skeletons

• **skeletons**: [`Skeleton`](Skeleton.md)[]

The list of skeletons added to the scene

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_bones_and_skeletons

#### Inherited from

[AbstractScene](AbstractScene.md).[skeletons](AbstractScene.md#skeletons)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:134

___

### skipPointerDownPicking

• **skipPointerDownPicking**: `boolean` = `false`

Gets or sets a boolean indicating if the user want to entirely skip the picking phase when a pointer down event occurs.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:715

___

### skipPointerMovePicking

• **skipPointerMovePicking**: `boolean` = `false`

Gets or sets a boolean indicating if the user want to entirely skip the picking phase when a pointer move event occurs.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:710

___

### skipPointerUpPicking

• **skipPointerUpPicking**: `boolean` = `false`

Gets or sets a boolean indicating if the user want to entirely skip the picking phase when a pointer up event occurs.  Off by default.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:720

___

### soundTracks

• **soundTracks**: [`Nullable`](../modules.md#nullable)[`SoundTrack`](SoundTrack.md)[]

The list of sound tracks added to the scene

**`See`**

https://doc.babylonjs.com/how_to/playing_sounds_and_music

#### Defined in

https://github.com/babylon.js/core/src/Audio/audioSceneComponent.ts:71

___

### sounds

• **sounds**: [`Nullable`](../modules.md#nullable)[`Sound`](Sound.md)[]

The list of sounds used in the scene.

#### Inherited from

[AbstractScene](AbstractScene.md).[sounds](AbstractScene.md#sounds)

#### Defined in

https://github.com/babylon.js/core/src/Audio/audioSceneComponent.ts:51

___

### spriteManagers

• **spriteManagers**: [`ISpriteManager`](../interfaces/ISpriteManager.md)[]

All of the sprite managers added to this scene

**`See`**

https://doc.babylonjs.com/babylon101/sprites

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteSceneComponent.ts:30

___

### spritesEnabled

• **spritesEnabled**: `boolean` = `true`

Gets or sets a boolean indicating if sprites are enabled on this scene

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1083

___

### subSurfaceConfiguration

• **subSurfaceConfiguration**: [`Nullable`](../modules.md#nullable)`SubSurfaceConfiguration`

Gets or Sets the current prepass renderer associated to the scene.

#### Inherited from

[AbstractScene](AbstractScene.md).[subSurfaceConfiguration](AbstractScene.md#subsurfaceconfiguration)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/subSurfaceSceneComponent.ts:31

___

### textures

• **textures**: [`BaseTexture`](BaseTexture.md)[]

Textures to keep.

#### Inherited from

[AbstractScene](AbstractScene.md).[textures](AbstractScene.md#textures)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:197

___

### transformNodes

• **transformNodes**: [`TransformNode`](TransformNode.md)[]

All of the transform nodes added to this scene
In the context of a Scene, it is not supposed to be modified manually.
Any addition or removal should be done using the addTransformNode and removeTransformNode Scene methods.
Note also that the order of the TransformNode within the array is not significant and might change.

**`See`**

https://doc.babylonjs.com/how_to/transformnode

#### Inherited from

[AbstractScene](AbstractScene.md).[transformNodes](AbstractScene.md#transformnodes)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:186

___

### useConstantAnimationDeltaTime

• **useConstantAnimationDeltaTime**: `boolean` = `false`

Gets or sets a boolean indicating if a constant deltatime has to be used
This is mostly useful for testing purposes when you do not want the animations to scale with the framerate

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:353

___

### useDelayedTextureLoading

• **useDelayedTextureLoading**: `boolean`

Defines if texture loading must be delayed
If true, textures will only be loaded when they need to be rendered

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1162

___

### useOrderIndependentTransparency

• **useOrderIndependentTransparency**: `boolean`

Flag to indicate if we want to use order independent transparency, despite the performance hit

#### Defined in

https://github.com/babylon.js/core/src/Rendering/depthPeelingSceneComponent.ts:20

___

### FOGMODE\_EXP

▪ `Static` `Readonly` **FOGMODE\_EXP**: ``1``

The fog density is following an exponential function

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:138

___

### FOGMODE\_EXP2

▪ `Static` `Readonly` **FOGMODE\_EXP2**: ``2``

The fog density is following an exponential function faster than FOGMODE_EXP

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:140

___

### FOGMODE\_LINEAR

▪ `Static` `Readonly` **FOGMODE\_LINEAR**: ``3``

The fog density is following a linear function.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:142

___

### FOGMODE\_NONE

▪ `Static` `Readonly` **FOGMODE\_NONE**: ``0``

The fog is deactivated

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:136

___

### MaxDeltaTime

▪ `Static` **MaxDeltaTime**: `number` = `1000.0`

Gets or sets the maximum deltatime when deterministic lock step is enabled

**`See`**

https://doc.babylonjs.com/babylon101/animations#deterministic-lockstep

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:153

___

### MinDeltaTime

▪ `Static` **MinDeltaTime**: `number` = `1.0`

Gets or sets the minimum deltatime when deterministic lock step is enabled

**`See`**

https://doc.babylonjs.com/babylon101/animations#deterministic-lockstep

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:148

## Accessors

### activeBonesPerfCounter

• `get` **activeBonesPerfCounter**(): [`PerfCounter`](PerfCounter.md)

Gets the performance counter for active bones

**`See`**

https://doc.babylonjs.com/how_to/optimizing_your_scene#instrumentation

#### Returns

[`PerfCounter`](PerfCounter.md)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1730

___

### activeCamera

• `get` **activeCamera**(): [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md)

Gets or sets the current active camera

#### Returns

[`Nullable`](../modules.md#nullable)[`Camera`](Camera.md)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1021

• `set` **activeCamera**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1025

___

### activeParticlesPerfCounter

• `get` **activeParticlesPerfCounter**(): [`PerfCounter`](PerfCounter.md)

Gets the performance counter for active particles

**`See`**

https://doc.babylonjs.com/how_to/optimizing_your_scene#instrumentation

#### Returns

[`PerfCounter`](PerfCounter.md)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1714

___

### afterCameraRender

• `set` **afterCameraRender**(`callback`): `void`

Sets a function to be executed after rendering a camera

#### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | () => `void` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:506

___

### afterRender

• `set` **afterRender**(`callback`): `void`

Sets a function to be executed after rendering this scene

#### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | [`Nullable`](../modules.md#nullable)() => `void` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:448

___

### animatables

• `get` **animatables**(): [`Animatable`](Animatable.md)[]

Gets all animatable attached to the scene

#### Returns

[`Animatable`](Animatable.md)[]

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2132

___

### animationPropertiesOverride

• `get` **animationPropertiesOverride**(): [`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md)

Gets or sets the animation properties override

#### Returns

[`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:341

• `set` **animationPropertiesOverride**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`AnimationPropertiesOverride`](AnimationPropertiesOverride.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:345

___

### beforeCameraRender

• `set` **beforeCameraRender**(`callback`): `void`

Sets a function to be executed before rendering a camera

#### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | () => `void` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:490

___

### beforeRender

• `set` **beforeRender**(`callback`): `void`

Sets a function to be executed before rendering this scene

#### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | [`Nullable`](../modules.md#nullable)() => `void` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:426

___

### blockMaterialDirtyMechanism

• `get` **blockMaterialDirtyMechanism**(): `boolean`

Gets or sets a boolean blocking all the calls to markAllMaterialsAsDirty (ie. the materials won't be updated if they are out of sync)

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:5129

• `set` **blockMaterialDirtyMechanism**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:5133

___

### blockfreeActiveMeshesAndRenderingGroups

• `get` **blockfreeActiveMeshesAndRenderingGroups**(): `boolean`

Gets or sets a boolean blocking all the calls to freeActiveMeshes and freeRenderingGroups
It can be used in order to prevent going through methods freeRenderingGroups and freeActiveMeshes several times to improve performance
when disposing several meshes in a row or a hierarchy of meshes.
When used, it is the responsibility of the user to blockfreeActiveMeshesAndRenderingGroups back to false.

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3615

• `set` **blockfreeActiveMeshesAndRenderingGroups**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3619

___

### defaultMaterial

• `get` **defaultMaterial**(): [`Material`](Material.md)

The default material used on meshes when no material is affected

#### Returns

[`Material`](Material.md)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1037

• `set` **defaultMaterial**(`value`): `void`

The default material used on meshes when no material is affected

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Material`](Material.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1046

___

### environmentTexture

• `get` **environmentTexture**(): [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Texture used in all pbr material as the reflection texture.
As in the majority of the scene they are the same (exception for multi room and so on),
this is easier to reference from here than from all the materials.

#### Returns

[`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

#### Overrides

AbstractScene.environmentTexture

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:218

• `set` **environmentTexture**(`value`): `void`

Texture used in all pbr material as the reflection texture.
As in the majority of the scene they are the same (exception for multi room and so on),
this is easier to set here than in all the materials.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md) |

#### Returns

`void`

#### Overrides

AbstractScene.environmentTexture

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:226

___

### fogEnabled

• `get` **fogEnabled**(): `boolean`

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:920

• `set` **fogEnabled**(`value`): `void`

Gets or sets a boolean indicating if fog is enabled on this scene

**`See`**

https://doc.babylonjs.com/babylon101/environment#fog
(Default is true)

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:913

___

### fogMode

• `get` **fogMode**(): `number`

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:942

• `set` **fogMode**(`value`): `void`

Gets or sets the fog mode to use

**`See`**

https://doc.babylonjs.com/babylon101/environment#fog
| mode | value |
| --- | --- |
| FOGMODE_NONE | 0 |
| FOGMODE_EXP | 1 |
| FOGMODE_EXP2 | 2 |
| FOGMODE_LINEAR | 3 |

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:935

___

### forcePointsCloud

• `get` **forcePointsCloud**(): `boolean`

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:297

• `set` **forcePointsCloud**(`value`): `void`

Gets or sets a boolean indicating if all rendering must be done in point cloud

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:290

___

### forceWireframe

• `get` **forceWireframe**(): `boolean`

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:268

• `set` **forceWireframe**(`value`): `void`

Gets or sets a boolean indicating if all rendering must be done in wireframe

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:261

___

### frustumPlanes

• `get` **frustumPlanes**(): [`Plane`](Plane.md)[]

Gets the list of frustum planes (built from the active camera)

#### Returns

[`Plane`](Plane.md)[]

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1280

___

### imageProcessingConfiguration

• `get` **imageProcessingConfiguration**(): [`ImageProcessingConfiguration`](ImageProcessingConfiguration.md)

Default image processing configuration used either in the rendering
Forward main pass or through the imageProcessingPostProcess if present.
As in the majority of the scene they are the same (exception for multi camera),
this is easier to reference from here than from all the materials and post process.

No setter as we it is a shared configuration, you can set the values instead.

#### Returns

[`ImageProcessingConfiguration`](ImageProcessingConfiguration.md)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:253

___

### isDisposed

• `get` **isDisposed**(): `boolean`

Gets if the scene is already disposed

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:4754

___

### isLoading

• `get` **isLoading**(): `boolean`

Returns a boolean indicating if the scene is still loading data

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2071

___

### lightsEnabled

• `get` **lightsEnabled**(): `boolean`

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1011

• `set` **lightsEnabled**(`value`): `void`

Gets or sets a boolean indicating if lights are enabled on this scene

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1003

___

### meshUnderPointer

• `get` **meshUnderPointer**(): [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

Gets the mesh that is currently under the pointer

#### Returns

[`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1601

___

### onDispose

• `set` **onDispose**(`callback`): `void`

Sets a function to be executed when this scene is disposed.

#### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | () => `void` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:412

___

### pointerX

• `get` **pointerX**(): `number`

Gets or sets the current on-screen X position of the pointer

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1608

• `set` **pointerX**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1612

___

### pointerY

• `get` **pointerY**(): `number`

Gets or sets the current on-screen Y position of the pointer

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1619

• `set` **pointerY**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1623

___

### prePass

• `get` **prePass**(): `boolean`

Flag indicating that the frame buffer binding is handled by another component

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:974

___

### shadowsEnabled

• `get` **shadowsEnabled**(): `boolean`

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:995

• `set` **shadowsEnabled**(`value`): `void`

Gets or sets a boolean indicating if shadows are enabled on this scene

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:988

___

### skeletonsEnabled

• `get` **skeletonsEnabled**(): `boolean`

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1098

• `set` **skeletonsEnabled**(`value`): `void`

Gets or sets a boolean indicating if skeletons are enabled on this scene

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1090

___

### skipFrustumClipping

• `get` **skipFrustumClipping**(): `boolean`

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:282

• `set` **skipFrustumClipping**(`value`): `void`

Gets or sets a boolean indicating if we should skip the frustum clipping part of the active meshes selection

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:276

___

### texturesEnabled

• `get` **texturesEnabled**(): `boolean`

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1063

• `set` **texturesEnabled**(`value`): `void`

Gets or sets a boolean indicating if textures are enabled on this scene

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1055

___

### totalActiveIndicesPerfCounter

• `get` **totalActiveIndicesPerfCounter**(): [`PerfCounter`](PerfCounter.md)

Gets the performance counter for active indices

**`See`**

https://doc.babylonjs.com/how_to/optimizing_your_scene#instrumentation

#### Returns

[`PerfCounter`](PerfCounter.md)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1698

___

### totalVerticesPerfCounter

• `get` **totalVerticesPerfCounter**(): [`PerfCounter`](PerfCounter.md)

Gets the performance counter for total vertices

**`See`**

https://doc.babylonjs.com/how_to/optimizing_your_scene#instrumentation

#### Returns

[`PerfCounter`](PerfCounter.md)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1682

___

### uid

• `get` **uid**(): `string`

Return a unique id as a string which can serve as an identifier for the scene

#### Returns

`string`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3514

___

### unTranslatedPointer

• `get` **unTranslatedPointer**(): [`Vector2`](Vector2.md)

Gets the pointer coordinates without any translation (ie. straight out of the pointer event)

#### Returns

[`Vector2`](Vector2.md)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:750

___

### useRightHandedSystem

• `get` **useRightHandedSystem**(): `boolean`

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:869

• `set` **useRightHandedSystem**(`value`): `void`

Gets or sets a boolean indicating if the scene must use right-handed coordinates system

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:862

___

### DoubleClickDelay

• `Static` `get` **DoubleClickDelay**(): `number`

Time in milliseconds to wait to raise long press events if button is still pressed. Default is 300 ms

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:779

• `Static` `set` **DoubleClickDelay**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:783

___

### DragMovementThreshold

• `Static` `get` **DragMovementThreshold**(): `number`

Gets or sets the distance in pixel that you have to move to prevent some events. Default is 10 pixels

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:757

• `Static` `set` **DragMovementThreshold**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:761

___

### ExclusiveDoubleClickMode

• `Static` `get` **ExclusiveDoubleClickMode**(): `boolean`

If you need to check double click without raising a single click at first click, enable this flag

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:788

• `Static` `set` **ExclusiveDoubleClickMode**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:792

___

### LongPressDelay

• `Static` `get` **LongPressDelay**(): `number`

Time in milliseconds to wait to raise long press events if button is still pressed. Default is 500 ms

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:768

• `Static` `set` **LongPressDelay**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:772

## Methods

### \_activeMesh

▸ `Private` **_activeMesh**(`sourceMesh`, `mesh`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `sourceMesh` | [`AbstractMesh`](AbstractMesh.md) |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3925

___

### \_bindFrameBuffer

▸ `Private` **_bindFrameBuffer**(`camera`, `clear?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `camera` | [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md) | `undefined` |
| `clear` | `boolean` | `true` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3965

___

### \_checkCameraRenderTarget

▸ `Private` **_checkCameraRenderTarget**(`camera`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `camera` | [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:4307

___

### \_checkIntersections

▸ `Private` **_checkIntersections**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:4182

___

### \_clear

▸ `Private` **_clear**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:4301

___

### \_clearFrameBuffer

▸ `Private` **_clearFrameBuffer**(`camera`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `camera` | [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3980

___

### \_createUbo

▸ `Private` **_createUbo**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1771

___

### \_disposeList

▸ `Private` **_disposeList**`T`(`items`, `callback?`): `void`

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`IDisposable`](../interfaces/IDisposable.md) |

#### Parameters

| Name | Type |
| :------ | :------ |
| `items` | `T`[] |
| `callback?` | (`item`: `T`) => `void` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:4742

___

### \_evaluateActiveMeshes

▸ `Private` **_evaluateActiveMeshes**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3777

___

### \_evaluateSubMesh

▸ `Private` **_evaluateSubMesh**(`subMesh`, `mesh`, `initialMesh`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `subMesh` | [`SubMesh`](SubMesh.md) |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) |
| `initialMesh` | [`AbstractMesh`](AbstractMesh.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3570

___

### \_executeActiveContainerCleanup

▸ `Private` **_executeActiveContainerCleanup**(`container`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `container` | [`SmartArray`](SmartArray.md)`any` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3766

___

### \_executeOnceBeforeRender

▸ `Private` **_executeOnceBeforeRender**(`func`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `func` | () => `void` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2008

___

### \_getByTags

▸ `Private` **_getByTags**(`list`, `tagsQuery`, `forEach?`): `any`[]

#### Parameters

| Name | Type |
| :------ | :------ |
| `list` | `any`[] |
| `tagsQuery` | `string` |
| `forEach?` | (`item`: `any`) => `void` |

#### Returns

`any`[]

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:5011

___

### \_getGeometryByUniqueId

▸ `Private` **_getGeometryByUniqueId**(`uniqueId`): [`Nullable`](../modules.md#nullable)[`Geometry`](Geometry.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `uniqueId` | `number` |

#### Returns

[`Nullable`](../modules.md#nullable)[`Geometry`](Geometry.md)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3068

___

### \_processSubCameras

▸ `Private` **_processSubCameras**(`camera`, `bindFrameBuffer?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `camera` | [`Camera`](Camera.md) | `undefined` |
| `bindFrameBuffer` | `boolean` | `true` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:4156

___

### \_registerTransientComponents

▸ `Private` **_registerTransientComponents**(): `void`

Registers the transient components if needed.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1318

___

### addActionManager

▸ **addActionManager**(`newActionManager`): `void`

Adds the given action manager to this scene

**`Deprecated`**

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newActionManager` | [`AbstractActionManager`](AbstractActionManager.md) | The action manager to add |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2730

___

### addAnimation

▸ **addAnimation**(`newAnimation`): `void`

Adds the given animation to this scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newAnimation` | [`Animation`](Animation.md) | The animation to add |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2649

___

### addAnimationGroup

▸ **addAnimationGroup**(`newAnimationGroup`): `void`

Adds the given animation group to this scene.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newAnimationGroup` | [`AnimationGroup`](AnimationGroup.md) | The animation group to add |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2660

___

### addCamera

▸ **addCamera**(`newCamera`): `void`

Adds the given camera to this scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newCamera` | [`Camera`](Camera.md) | The camera to add |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2609

___

### addEffectLayer

▸ **addEffectLayer**(`newEffectLayer`): `void`

Adds the given effect layer to this scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newEffectLayer` | [`EffectLayer`](EffectLayer.md) | defines the effect layer to add |

#### Returns

`void`

#### Inherited from

[AbstractScene](AbstractScene.md).[addEffectLayer](AbstractScene.md#addeffectlayer)

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayerSceneComponent.ts:46

___

### addExternalData

▸ **addExternalData**`T`(`key`, `data`): `boolean`

Add an externally attached data from its key.
This method call will fail and return false, if such key already exists.
If you don't care and just want to get the data no matter what, use the more convenient getOrAddExternalDataWithFactory() method.

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | `string` | the unique key that identifies the data |
| `data` | `T` | the data object to associate to the key for this Engine instance |

#### Returns

`boolean`

true if no such key were already present and the data was added successfully, false otherwise

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3529

___

### addGeometry

▸ **addGeometry**(`newGeometry`): `void`

Adds the given geometry to this scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newGeometry` | [`Geometry`](Geometry.md) | The geometry to add |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2713

___

### addLensFlareSystem

▸ **addLensFlareSystem**(`newLensFlareSystem`): `void`

Adds the given lens flare system to this scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newLensFlareSystem` | [`LensFlareSystem`](LensFlareSystem.md) | The lens flare system to add |

#### Returns

`void`

#### Inherited from

[AbstractScene](AbstractScene.md).[addLensFlareSystem](AbstractScene.md#addlensflaresystem)

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlareSystemSceneComponent.ts:45

___

### addLight

▸ **addLight**(`newLight`): `void`

Adds the given light to this scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newLight` | [`Light`](Light.md) | The light to add |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2574

___

### addMaterial

▸ **addMaterial**(`newMaterial`): `void`

Adds the given material to this scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newMaterial` | [`Material`](Material.md) | The material to add |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2683

___

### addMesh

▸ **addMesh**(`newMesh`, `recursive?`): `void`

Add a mesh to the list of scene's meshes

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `newMesh` | [`AbstractMesh`](AbstractMesh.md) | `undefined` | defines the mesh to add |
| `recursive` | `boolean` | `false` | if all child meshes should also be added to the scene |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2256

___

### addMorphTargetManager

▸ **addMorphTargetManager**(`newMorphTargetManager`): `void`

Adds the given morph target to this scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newMorphTargetManager` | [`MorphTargetManager`](MorphTargetManager.md) | The morph target to add |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2702

___

### addMultiMaterial

▸ **addMultiMaterial**(`newMultiMaterial`): `void`

Adds the given multi-material to this scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newMultiMaterial` | [`MultiMaterial`](MultiMaterial.md) | The multi-material to add |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2671

___

### addParticleSystem

▸ **addParticleSystem**(`newParticleSystem`): `void`

Adds the given particle system to this scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newParticleSystem` | [`IParticleSystem`](../interfaces/IParticleSystem.md) | The particle system to add |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2638

___

### addPendingData

▸ **addPendingData**(`data`): `void`

This function can help adding any object to the list of data awaited to be ready in order to check for a complete scene loading.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `any` | defines the object to wait for |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2039

___

### addReflectionProbe

▸ **addReflectionProbe**(`newReflectionProbe`): `void`

Adds the given reflection probe to this scene.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newReflectionProbe` | [`ReflectionProbe`](ReflectionProbe.md) | The reflection probe to add |

#### Returns

`void`

#### Inherited from

[AbstractScene](AbstractScene.md).[addReflectionProbe](AbstractScene.md#addreflectionprobe)

#### Defined in

https://github.com/babylon.js/core/src/Probes/reflectionProbe.ts:30

___

### addSkeleton

▸ **addSkeleton**(`newSkeleton`): `void`

Adds the given skeleton to this scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newSkeleton` | [`Skeleton`](Skeleton.md) | The skeleton to add |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2626

___

### addTexture

▸ **addTexture**(`newTexture`): `void`

Adds the given texture to this scene.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newTexture` | [`BaseTexture`](BaseTexture.md) | The texture to add |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2738

___

### addTransformNode

▸ **addTransformNode**(`newTransformNode`): `void`

Add a transform node to the list of scene's transform nodes

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newTransformNode` | [`TransformNode`](TransformNode.md) | defines the transform node to add |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2311

___

### animate

▸ **animate**(): `void`

Execute all animations (for a frame)

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:4252

___

### attachControl

▸ **attachControl**(`attachUp?`, `attachDown?`, `attachMove?`): `void`

Attach events to the canvas (To handle actionManagers triggers and raise onPointerMove, onPointerDown and onPointerUp

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `attachUp` | `boolean` | `true` | defines if you want to attach events to pointerup |
| `attachDown` | `boolean` | `true` | defines if you want to attach events to pointerdown |
| `attachMove` | `boolean` | `true` | defines if you want to attach events to pointermove |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1827

___

### beginAnimation

▸ **beginAnimation**(`target`, `from`, `to`, `loop?`, `speedRatio?`, `onAnimationEnd?`, `animatable?`, `stopCurrent?`, `targetMask?`, `onAnimationLoop?`, `isAdditive?`): [`Animatable`](Animatable.md)

Will start the animation sequence of a given target

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `target` | `any` | defines the target |
| `from` | `number` | defines from which frame should animation start |
| `to` | `number` | defines until which frame should animation run. |
| `loop?` | `boolean` | defines if the animation loops |
| `speedRatio?` | `number` | defines the speed in which to run the animation (1.0 by default) |
| `onAnimationEnd?` | () => `void` | defines the function to be executed when the animation ends |
| `animatable?` | [`Animatable`](Animatable.md) | defines an animatable object. If not provided a new one will be created from the given params |
| `stopCurrent?` | `boolean` | defines if the current animations must be stopped first (true by default) |
| `targetMask?` | (`target`: `any`) => `boolean` | defines if the target should be animate if animations are present (this is called recursively on descendant animatables regardless of return value) |
| `onAnimationLoop?` | () => `void` | defines the callback to call when an animation loops |
| `isAdditive?` | `boolean` | defines whether the animation should be evaluated additively (false by default) |

#### Returns

[`Animatable`](Animatable.md)

the animatable object created for this animation

#### Defined in

https://github.com/babylon.js/core/src/Animations/animatable.ts:519

___

### beginDirectAnimation

▸ **beginDirectAnimation**(`target`, `animations`, `from`, `to`, `loop?`, `speedRatio?`, `onAnimationEnd?`, `onAnimationLoop?`, `isAdditive?`): [`Animatable`](Animatable.md)

Begin a new animation on a given node

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `target` | `any` | defines the target where the animation will take place |
| `animations` | [`Animation`](Animation.md)[] | defines the list of animations to start |
| `from` | `number` | defines the initial value |
| `to` | `number` | defines the final value |
| `loop?` | `boolean` | defines if you want animation to loop (off by default) |
| `speedRatio?` | `number` | defines the speed ratio to apply to all animations |
| `onAnimationEnd?` | () => `void` | defines the callback to call when an animation ends (will be called once per node) |
| `onAnimationLoop?` | () => `void` | defines the callback to call when an animation loops |
| `isAdditive?` | `boolean` | defines whether the animation should be evaluated additively (false by default) |

#### Returns

[`Animatable`](Animatable.md)

the list of created animatables

#### Defined in

https://github.com/babylon.js/core/src/Animations/animatable.ts:577

___

### beginDirectHierarchyAnimation

▸ **beginDirectHierarchyAnimation**(`target`, `directDescendantsOnly`, `animations`, `from`, `to`, `loop?`, `speedRatio?`, `onAnimationEnd?`, `onAnimationLoop?`, `isAdditive?`): [`Animatable`](Animatable.md)[]

Begin a new animation on a given node and its hierarchy

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `target` | [`Node`](Node.md) | defines the root node where the animation will take place |
| `directDescendantsOnly` | `boolean` | if true only direct descendants will be used, if false direct and also indirect (children of children, an so on in a recursive manner) descendants will be used. |
| `animations` | [`Animation`](Animation.md)[] | defines the list of animations to start |
| `from` | `number` | defines the initial value |
| `to` | `number` | defines the final value |
| `loop?` | `boolean` | defines if you want animation to loop (off by default) |
| `speedRatio?` | `number` | defines the speed ratio to apply to all animations |
| `onAnimationEnd?` | () => `void` | defines the callback to call when an animation ends (will be called once per node) |
| `onAnimationLoop?` | () => `void` | defines the callback to call when an animation loops |
| `isAdditive?` | `boolean` | defines whether the animation should be evaluated additively (false by default) |

#### Returns

[`Animatable`](Animatable.md)[]

the list of animatables created for all nodes

#### Defined in

https://github.com/babylon.js/core/src/Animations/animatable.ts:603

___

### beginHierarchyAnimation

▸ **beginHierarchyAnimation**(`target`, `directDescendantsOnly`, `from`, `to`, `loop?`, `speedRatio?`, `onAnimationEnd?`, `animatable?`, `stopCurrent?`, `targetMask?`, `onAnimationLoop?`, `isAdditive?`): [`Animatable`](Animatable.md)[]

Will start the animation sequence of a given target and its hierarchy

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `target` | `any` | defines the target |
| `directDescendantsOnly` | `boolean` | if true only direct descendants will be used, if false direct and also indirect (children of children, an so on in a recursive manner) descendants will be used. |
| `from` | `number` | defines from which frame should animation start |
| `to` | `number` | defines until which frame should animation run. |
| `loop?` | `boolean` | defines if the animation loops |
| `speedRatio?` | `number` | defines the speed in which to run the animation (1.0 by default) |
| `onAnimationEnd?` | () => `void` | defines the function to be executed when the animation ends |
| `animatable?` | [`Animatable`](Animatable.md) | defines an animatable object. If not provided a new one will be created from the given params |
| `stopCurrent?` | `boolean` | defines if the current animations must be stopped first (true by default) |
| `targetMask?` | (`target`: `any`) => `boolean` | defines if the target should be animated if animations are present (this is called recursively on descendant animatables regardless of return value) |
| `onAnimationLoop?` | () => `void` | defines the callback to call when an animation loops |
| `isAdditive?` | `boolean` | defines whether the animation should be evaluated additively (false by default) |

#### Returns

[`Animatable`](Animatable.md)[]

the list of created animatables

#### Defined in

https://github.com/babylon.js/core/src/Animations/animatable.ts:549

___

### beginWeightedAnimation

▸ **beginWeightedAnimation**(`target`, `from`, `to`, `weight`, `loop?`, `speedRatio?`, `onAnimationEnd?`, `animatable?`, `targetMask?`, `onAnimationLoop?`, `isAdditive?`): [`Animatable`](Animatable.md)

Will start the animation sequence of a given target

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `target` | `any` | defines the target |
| `from` | `number` | defines from which frame should animation start |
| `to` | `number` | defines until which frame should animation run. |
| `weight` | `number` | defines the weight to apply to the animation (1.0 by default) |
| `loop?` | `boolean` | defines if the animation loops |
| `speedRatio?` | `number` | defines the speed in which to run the animation (1.0 by default) |
| `onAnimationEnd?` | () => `void` | defines the function to be executed when the animation ends |
| `animatable?` | [`Animatable`](Animatable.md) | defines an animatable object. If not provided a new one will be created from the given params |
| `targetMask?` | (`target`: `any`) => `boolean` | defines if the target should be animated if animations are present (this is called recursively on descendant animatables regardless of return value) |
| `onAnimationLoop?` | () => `void` | defines the callback to call when an animation loops |
| `isAdditive?` | `boolean` | defines whether the animation should be evaluated additively (false by default) |

#### Returns

[`Animatable`](Animatable.md)

the animatable object created for this animation

#### Defined in

https://github.com/babylon.js/core/src/Animations/animatable.ts:490

___

### bindEyePosition

▸ **bindEyePosition**(`effect`, `variableName?`, `isVector3?`): [`Vector4`](Vector4.md)

Bind the current view position to an effect.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `effect` | [`Nullable`](../modules.md#nullable)[`Effect`](Effect.md) | `undefined` | The effect to be bound |
| `variableName` | `string` | `"vEyePosition"` | name of the shader variable that will hold the eye position |
| `isVector3` | `boolean` | `false` | true to indicates that variableName is a Vector3 and not a Vector4 |

#### Returns

[`Vector4`](Vector4.md)

the computed eye position

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:803

___

### cleanCachedTextureBuffer

▸ **cleanCachedTextureBuffer**(): `void`

This function will remove the local cached buffer data from texture.
It will save memory but will prevent the texture from being rebuilt

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:4777

___

### clearCachedVertexData

▸ **clearCachedVertexData**(): `void`

Call this function to reduce memory footprint of the scene.
Vertex buffers will not store CPU data anymore (this will prevent picking, collisions or physics to work correctly)

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:4762

___

### createDefaultCamera

▸ **createDefaultCamera**(`createArcRotateCamera?`, `replace?`, `attachCameraControls?`): `void`

Creates a default camera for the scene.

**`See`**

https://doc.babylonjs.com/How_To/Fast_Build#create-default-camera

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `createArcRotateCamera?` | `boolean` | has the default false which creates a free camera, when true creates an arc rotate camera |
| `replace?` | `boolean` | has default false, when true replaces the active camera in the scene |
| `attachCameraControls?` | `boolean` | has default false, when true attaches camera controls to the canvas. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Helpers/sceneHelpers.ts:46

___

### createDefaultCameraOrLight

▸ **createDefaultCameraOrLight**(`createArcRotateCamera?`, `replace?`, `attachCameraControls?`): `void`

Creates a default camera and a default light.

**`See`**

https://doc.babylonjs.com/divingDeeper/scene/fastBuildWorld#create-default-camera-or-light

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `createArcRotateCamera?` | `boolean` | has the default false which creates a free camera, when true creates an arc rotate camera |
| `replace?` | `boolean` | has the default false, when true replaces the active camera/light in the scene |
| `attachCameraControls?` | `boolean` | has the default false, when true attaches camera controls to the canvas. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Helpers/sceneHelpers.ts:55

___

### createDefaultEnvironment

▸ **createDefaultEnvironment**(`options?`): [`Nullable`](../modules.md#nullable)[`EnvironmentHelper`](EnvironmentHelper.md)

Creates a new environment

**`See`**

https://doc.babylonjs.com/How_To/Fast_Build#create-default-environment

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options?` | `Partial`[`IEnvironmentHelperOptions`](../interfaces/IEnvironmentHelperOptions.md) | defines the options you can use to configure the environment |

#### Returns

[`Nullable`](../modules.md#nullable)[`EnvironmentHelper`](EnvironmentHelper.md)

the new EnvironmentHelper

#### Defined in

https://github.com/babylon.js/core/src/Helpers/sceneHelpers.ts:75

___

### createDefaultLight

▸ **createDefaultLight**(`replace?`): `void`

Creates a default light for the scene.

**`See`**

https://doc.babylonjs.com/How_To/Fast_Build#create-default-light

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `replace?` | `boolean` | has the default false, when true replaces the existing lights in the scene with a hemispheric light |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Helpers/sceneHelpers.ts:37

___

### createDefaultSkybox

▸ **createDefaultSkybox**(`environmentTexture?`, `pbr?`, `scale?`, `blur?`, `setGlobalEnvTexture?`): [`Nullable`](../modules.md#nullable)[`Mesh`](Mesh.md)

Creates a new sky box

**`See`**

https://doc.babylonjs.com/divingDeeper/scene/fastBuildWorld#create-default-skybox

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `environmentTexture?` | [`BaseTexture`](BaseTexture.md) | defines the texture to use as environment texture |
| `pbr?` | `boolean` | has default false which requires the StandardMaterial to be used, when true PBRMaterial must be used |
| `scale?` | `number` | defines the overall scale of the skybox |
| `blur?` | `number` | is only available when pbr is true, default is 0, no blur, maximum value is 1 |
| `setGlobalEnvTexture?` | `boolean` | has default true indicating that scene.environmentTexture must match the current skybox texture |

#### Returns

[`Nullable`](../modules.md#nullable)[`Mesh`](Mesh.md)

a new mesh holding the sky box

#### Defined in

https://github.com/babylon.js/core/src/Helpers/sceneHelpers.ts:67

___

### createDefaultVRExperience

▸ **createDefaultVRExperience**(`webVROptions?`): [`VRExperienceHelper`](VRExperienceHelper.md)

Creates a new VREXperienceHelper

**`See`**

https://doc.babylonjs.com/divingDeeper/cameras/webVRHelper

**`Deprecated`**

Please use createDefaultXRExperienceAsync instead

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `webVROptions?` | [`VRExperienceHelperOptions`](../interfaces/VRExperienceHelperOptions.md) | defines the options used to create the new VREXperienceHelper |

#### Returns

[`VRExperienceHelper`](VRExperienceHelper.md)

a new VREXperienceHelper

#### Defined in

https://github.com/babylon.js/core/src/Helpers/sceneHelpers.ts:84

___

### createDefaultXRExperienceAsync

▸ **createDefaultXRExperienceAsync**(`options?`): `Promise`[`WebXRDefaultExperience`](WebXRDefaultExperience.md)

Creates a new WebXRDefaultExperience

**`See`**

https://doc.babylonjs.com/how_to/introduction_to_webxr

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options?` | [`WebXRDefaultExperienceOptions`](WebXRDefaultExperienceOptions.md) | experience options |

#### Returns

`Promise`[`WebXRDefaultExperience`](WebXRDefaultExperience.md)

a promise for a new WebXRDefaultExperience

#### Defined in

https://github.com/babylon.js/core/src/Helpers/sceneHelpers.ts:92

___

### createOrUpdateSelectionOctree

▸ **createOrUpdateSelectionOctree**(`maxCapacity?`, `maxDepth?`): [`Octree`](Octree.md)[`AbstractMesh`](AbstractMesh.md)

Creates or updates the octree used to boost selection (picking)

**`See`**

https://doc.babylonjs.com/how_to/optimizing_your_scene_with_octrees

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `maxCapacity?` | `number` | defines the maximum capacity per leaf |
| `maxDepth?` | `number` | defines the maximum depth of the octree |

#### Returns

[`Octree`](Octree.md)[`AbstractMesh`](AbstractMesh.md)

an octree of AbstractMesh

#### Defined in

https://github.com/babylon.js/core/src/Culling/Octrees/octreeSceneComponent.ts:35

___

### createPickingRay

▸ **createPickingRay**(`x`, `y`, `world`, `camera`, `cameraViewSpace?`): [`Ray`](Ray.md)

Creates a ray that can be used to pick in the scene

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `x` | `number` | `undefined` | defines the x coordinate of the origin (on-screen) |
| `y` | `number` | `undefined` | defines the y coordinate of the origin (on-screen) |
| `world` | [`Nullable`](../modules.md#nullable)[`Matrix`](Matrix.md) | `undefined` | defines the world matrix to use if you want to pick in object space (instead of world space) |
| `camera` | [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md) | `undefined` | defines the camera to use for the picking |
| `cameraViewSpace` | `boolean` | `false` | defines if picking will be done in view space (false by default) |

#### Returns

[`Ray`](Ray.md)

a Ray

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:4830

___

### createPickingRayInCameraSpace

▸ **createPickingRayInCameraSpace**(`x`, `y`, `camera?`): [`Ray`](Ray.md)

Creates a ray that can be used to pick in the scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | defines the x coordinate of the origin (on-screen) |
| `y` | `number` | defines the y coordinate of the origin (on-screen) |
| `camera?` | [`Camera`](Camera.md) | defines the camera to use for the picking |

#### Returns

[`Ray`](Ray.md)

a Ray

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:4864

___

### createPickingRayInCameraSpaceToRef

▸ **createPickingRayInCameraSpaceToRef**(`x`, `y`, `result`, `camera?`): [`Scene`](Scene.md)

Creates a ray that can be used to pick in the scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | defines the x coordinate of the origin (on-screen) |
| `y` | `number` | defines the y coordinate of the origin (on-screen) |
| `result` | [`Ray`](Ray.md) | defines the ray where to store the picking ray |
| `camera?` | [`Camera`](Camera.md) | defines the camera to use for the picking |

#### Returns

[`Scene`](Scene.md)

the current scene

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:4876

___

### createPickingRayToRef

▸ **createPickingRayToRef**(`x`, `y`, `world`, `result`, `camera`, `cameraViewSpace?`, `enableDistantPicking?`): [`Scene`](Scene.md)

Creates a ray that can be used to pick in the scene

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `x` | `number` | `undefined` | defines the x coordinate of the origin (on-screen) |
| `y` | `number` | `undefined` | defines the y coordinate of the origin (on-screen) |
| `world` | [`Nullable`](../modules.md#nullable)[`Matrix`](Matrix.md) | `undefined` | defines the world matrix to use if you want to pick in object space (instead of world space) |
| `result` | [`Ray`](Ray.md) | `undefined` | defines the ray where to store the picking ray |
| `camera` | [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md) | `undefined` | defines the camera to use for the picking |
| `cameraViewSpace` | `boolean` | `false` | defines if picking will be done in view space (false by default) |
| `enableDistantPicking` | `boolean` | `false` | defines if picking should handle large values for mesh position/scaling (false by default) |

#### Returns

[`Scene`](Scene.md)

the current scene

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:4845

___

### createSceneUniformBuffer

▸ **createSceneUniformBuffer**(`name?`): [`UniformBuffer`](UniformBuffer.md)

Creates a scene UBO

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name?` | `string` | name of the uniform buffer (optional, for debugging purpose only) |

#### Returns

[`UniformBuffer`](UniformBuffer.md)

a new ubo

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2223

___

### deleteCompoundImpostor

▸ **deleteCompoundImpostor**(`compound`): `void`

Deletes a physics compound impostor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `compound` | `any` | defines the compound to delete |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsEngineComponent.ts:54

___

### detachControl

▸ **detachControl**(): `void`

Detaches all event handlers

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1832

___

### disableDepthRenderer

▸ **disableDepthRenderer**(`camera?`): `void`

Disables a depth renderer for a given camera

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `camera?` | [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md) | The camera to disable the depth renderer on (default: scene's active camera) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/depthRendererSceneComponent.ts:29

___

### disableGeometryBufferRenderer

▸ **disableGeometryBufferRenderer**(): `void`

Disables the GeometryBufferRender associated with the scene

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRendererSceneComponent.ts:29

___

### disablePhysicsEngine

▸ **disablePhysicsEngine**(): `void`

Disables and disposes the physics engine associated with the scene

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsEngineComponent.ts:42

___

### disablePrePassRenderer

▸ **disablePrePassRenderer**(): `void`

Disables the prepass associated with the scene

#### Returns

`void`

#### Inherited from

[AbstractScene](AbstractScene.md).[disablePrePassRenderer](AbstractScene.md#disableprepassrenderer)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRendererSceneComponent.ts:34

___

### disableSubSurfaceForPrePass

▸ **disableSubSurfaceForPrePass**(): `void`

Disables the subsurface effect for prepass

#### Returns

`void`

#### Inherited from

[AbstractScene](AbstractScene.md).[disableSubSurfaceForPrePass](AbstractScene.md#disablesubsurfaceforprepass)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/subSurfaceSceneComponent.ts:42

___

### dispose

▸ **dispose**(): `void`

Releases all held resources

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:4542

___

### enableDepthRenderer

▸ **enableDepthRenderer**(`camera?`, `storeNonLinearDepth?`, `force32bitsFloat?`): [`DepthRenderer`](DepthRenderer.md)

Creates a depth renderer a given camera which contains a depth map which can be used for post processing.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `camera?` | [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md) | The camera to create the depth renderer on (default: scene's active camera) |
| `storeNonLinearDepth?` | `boolean` | Defines whether the depth is stored linearly like in Babylon Shadows or directly like glFragCoord.z |
| `force32bitsFloat?` | `boolean` | Forces 32 bits float when supported (else 16 bits float is prioritized over 32 bits float if supported) |

#### Returns

[`DepthRenderer`](DepthRenderer.md)

the created depth renderer

#### Defined in

https://github.com/babylon.js/core/src/Rendering/depthRendererSceneComponent.ts:23

___

### enableGeometryBufferRenderer

▸ **enableGeometryBufferRenderer**(`ratio?`): [`Nullable`](../modules.md#nullable)[`GeometryBufferRenderer`](GeometryBufferRenderer.md)

Enables a GeometryBufferRender and associates it with the scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ratio?` | `number` | defines the scaling ratio to apply to the renderer (1 by default which means same resolution) |

#### Returns

[`Nullable`](../modules.md#nullable)[`GeometryBufferRenderer`](GeometryBufferRenderer.md)

the GeometryBufferRenderer

#### Defined in

https://github.com/babylon.js/core/src/Rendering/geometryBufferRendererSceneComponent.ts:24

___

### enablePhysics

▸ **enablePhysics**(`gravity?`, `plugin?`): `boolean`

Enables physics to the current scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `gravity?` | [`Nullable`](../modules.md#nullable)[`Vector3`](Vector3.md) | defines the scene's gravity for the physics engine. defaults to real earth gravity : (0, -9.81, 0) |
| `plugin?` | `IPhysicsEnginePlugin` | defines the physics engine to be used. defaults to CannonJS. |

#### Returns

`boolean`

a boolean indicating if the physics engine was initialized

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsEngineComponent.ts:37

___

### enablePrePassRenderer

▸ **enablePrePassRenderer**(): [`Nullable`](../modules.md#nullable)[`PrePassRenderer`](PrePassRenderer.md)

Enables the prepass and associates it with the scene

#### Returns

[`Nullable`](../modules.md#nullable)[`PrePassRenderer`](PrePassRenderer.md)

the PrePassRenderer

#### Inherited from

[AbstractScene](AbstractScene.md).[enablePrePassRenderer](AbstractScene.md#enableprepassrenderer)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/prePassRendererSceneComponent.ts:29

___

### enableSubSurfaceForPrePass

▸ **enableSubSurfaceForPrePass**(): [`Nullable`](../modules.md#nullable)`SubSurfaceConfiguration`

Enables the subsurface effect for prepass

#### Returns

[`Nullable`](../modules.md#nullable)`SubSurfaceConfiguration`

the SubSurfaceConfiguration

#### Inherited from

[AbstractScene](AbstractScene.md).[enableSubSurfaceForPrePass](AbstractScene.md#enablesubsurfaceforprepass)

#### Defined in

https://github.com/babylon.js/core/src/Rendering/subSurfaceSceneComponent.ts:37

___

### executeOnceBeforeRender

▸ **executeOnceBeforeRender**(`func`, `timeout?`): `void`

The provided function will run before render once and will be disposed afterwards.
A timeout delay can be provided so that the function will be executed in N ms.
The timeout is using the browser's native setTimeout so time percision cannot be guaranteed.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `func` | () => `void` | The function to be executed. |
| `timeout?` | `number` | optional delay in ms |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2025

___

### executeWhenReady

▸ **executeWhenReady**(`func`, `checkRenderTargets?`): `void`

Registers a function to be executed when the scene is ready

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `func` | () => `void` | `undefined` | the function to be executed |
| `checkRenderTargets` | `boolean` | `false` | true to also check that the meshes rendered as part of a render target are ready (default: false) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2080

___

### finalizeSceneUbo

▸ **finalizeSceneUbo**(): [`UniformBuffer`](UniformBuffer.md)

Update the scene ubo before it can be used in rendering processing

#### Returns

[`UniformBuffer`](UniformBuffer.md)

the scene UniformBuffer

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:829

___

### freeActiveMeshes

▸ **freeActiveMeshes**(): `void`

Clear the active meshes smart array preventing retention point in mesh dispose.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3635

___

### freeProcessedMaterials

▸ **freeProcessedMaterials**(): `void`

Clear the processed materials smart array preventing retention point in material dispose.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3604

___

### freeRenderingGroups

▸ **freeRenderingGroups**(): `void`

Clear the info related to rendering groups preventing retention points during dispose.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3657

___

### freezeActiveMeshes

▸ **freezeActiveMeshes**(`skipEvaluateActiveMeshes?`, `onSuccess?`, `onError?`, `freezeMeshes?`, `keepFrustumCulling?`): [`Scene`](Scene.md)

Use this function to stop evaluating active meshes. The current list will be keep alive between frames

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `skipEvaluateActiveMeshes` | `boolean` | `false` | defines an optional boolean indicating that the evaluate active meshes step must be completely skipped |
| `onSuccess?` | () => `void` | `undefined` | optional success callback |
| `onError?` | (`message`: `string`) => `void` | `undefined` | optional error callback |
| `freezeMeshes` | `boolean` | `true` | defines if meshes should be frozen (true by default) |
| `keepFrustumCulling` | `boolean` | `false` | defines if you want to keep running the frustum clipping (false by default) |

#### Returns

[`Scene`](Scene.md)

the current scene

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3714

___

### freezeMaterials

▸ **freezeMaterials**(): `void`

Freeze all materials
A frozen material will not be updatable but should be faster to render

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:4523

___

### getActiveBones

▸ **getActiveBones**(): `number`

Gets the total number of active bones rendered per frame

#### Returns

`number`

the total number of active bones rendered per frame

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1722

___

### getActiveIndices

▸ **getActiveIndices**(): `number`

Gets the total number of active indices rendered per frame (You can deduce the number of rendered triangles by dividing this number by 3)

#### Returns

`number`

the total number of active indices rendered per frame

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1690

___

### getActiveMeshes

▸ **getActiveMeshes**(): [`SmartArray`](SmartArray.md)[`AbstractMesh`](AbstractMesh.md)

Gets the array of active meshes

#### Returns

[`SmartArray`](SmartArray.md)[`AbstractMesh`](AbstractMesh.md)

an array of AbstractMesh

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1738

___

### getActiveParticles

▸ **getActiveParticles**(): `number`

Gets the total number of active particles rendered per frame

#### Returns

`number`

the total number of active particles rendered per frame

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1706

___

### getAllAnimatablesByTarget

▸ **getAllAnimatablesByTarget**(`target`): [`Animatable`](Animatable.md)[]

Gets all animatables associated with a given target

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `target` | `any` | defines the target to look animatables for |

#### Returns

[`Animatable`](Animatable.md)[]

an array of Animatables

#### Defined in

https://github.com/babylon.js/core/src/Animations/animatable.ts:628

___

### getAnimatableByTarget

▸ **getAnimatableByTarget**(`target`): [`Nullable`](../modules.md#nullable)[`Animatable`](Animatable.md)

Gets the animatable associated with a specific target

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `target` | `any` | defines the target of the animatable |

#### Returns

[`Nullable`](../modules.md#nullable)[`Animatable`](Animatable.md)

the required animatable if found

#### Defined in

https://github.com/babylon.js/core/src/Animations/animatable.ts:621

___

### getAnimationGroupByName

▸ **getAnimationGroupByName**(`name`): [`Nullable`](../modules.md#nullable)[`AnimationGroup`](AnimationGroup.md)

get an animation group using its name

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the material's name |

#### Returns

[`Nullable`](../modules.md#nullable)[`AnimationGroup`](AnimationGroup.md)

the animation group or null if none found.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2804

___

### getAnimationRatio

▸ **getAnimationRatio**(): `number`

Gets the animation ratio (which is 1.0 is the scene renders at 60fps and 2 if the scene renders at 30fps, etc.)

#### Returns

`number`

a number

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1746

___

### getAutoClearDepthStencilSetup

▸ **getAutoClearDepthStencilSetup**(`index`): [`IRenderingManagerAutoClearSetup`](../interfaces/IRenderingManagerAutoClearSetup.md)

Gets the current auto clear configuration for one rendering group of the rendering
manager.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | the rendering group index to get the information for |

#### Returns

[`IRenderingManagerAutoClearSetup`](../interfaces/IRenderingManagerAutoClearSetup.md)

The auto clear setup for the requested rendering group

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:5122

___

### getBoneById

▸ **getBoneById**(`id`): [`Nullable`](../modules.md#nullable)[`Bone`](Bone.md)

Gets a bone using its Id

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | defines the bone's Id |

#### Returns

[`Nullable`](../modules.md#nullable)[`Bone`](Bone.md)

the bone or null if not found

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2962

___

### getBoneByName

▸ **getBoneByName**(`name`): [`Nullable`](../modules.md#nullable)[`Bone`](Bone.md)

Gets a bone using its id

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the bone's name |

#### Returns

[`Nullable`](../modules.md#nullable)[`Bone`](Bone.md)

the bone or null if not found

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2980

___

### getBoundingBoxRenderer

▸ **getBoundingBoxRenderer**(): [`BoundingBoxRenderer`](BoundingBoxRenderer.md)

Gets the bounding box renderer associated with the scene

#### Returns

[`BoundingBoxRenderer`](BoundingBoxRenderer.md)

a BoundingBoxRenderer

#### Defined in

https://github.com/babylon.js/core/src/Rendering/boundingBoxRenderer.ts:41

___

### getCachedEffect

▸ **getCachedEffect**(): [`Nullable`](../modules.md#nullable)[`Effect`](Effect.md)

Gets the cached effect (ie. the latest rendered one)

#### Returns

[`Nullable`](../modules.md#nullable)[`Effect`](Effect.md)

the cached effect

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1639

___

### getCachedMaterial

▸ **getCachedMaterial**(): [`Nullable`](../modules.md#nullable)[`Material`](Material.md)

Gets the cached material (ie. the latest rendered one)

#### Returns

[`Nullable`](../modules.md#nullable)[`Material`](Material.md)

the cached material

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1631

___

### getCachedVisibility

▸ **getCachedVisibility**(): [`Nullable`](../modules.md#nullable)`number`

Gets the cached visibility state (ie. the latest rendered one)

#### Returns

[`Nullable`](../modules.md#nullable)`number`

the cached visibility state

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1647

___

### getCameraById

▸ **getCameraById**(`id`): [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md)

Gets a camera using its Id

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | defines the Id to look for |

#### Returns

[`Nullable`](../modules.md#nullable)[`Camera`](Camera.md)

the camera or null if not found

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2917

___

### getCameraByName

▸ **getCameraByName**(`name`): [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md)

Gets a camera using its name

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the camera's name |

#### Returns

[`Nullable`](../modules.md#nullable)[`Camera`](Camera.md)

the camera or null if none found.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2947

___

### getCameraByUniqueId

▸ **getCameraByUniqueId**(`uniqueId`): [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md)

Gets a camera using its unique Id

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniqueId` | `number` | defines the unique Id to look for |

#### Returns

[`Nullable`](../modules.md#nullable)[`Camera`](Camera.md)

the camera or null if not found

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2932

___

### getCamerasByTags

▸ **getCamerasByTags**(`tagsQuery`, `forEach?`): [`Camera`](Camera.md)[]

Get a list of cameras by tags

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `tagsQuery` | `string` | defines the tags query to use |
| `forEach?` | (`camera`: [`Camera`](Camera.md)) => `void` | defines a predicate used to filter results |

#### Returns

[`Camera`](Camera.md)[]

an array of Camera

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:5052

___

### getClassName

▸ **getClassName**(): `string`

Gets a string identifying the name of the class

#### Returns

`string`

"Scene" string

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1552

___

### getEngine

▸ **getEngine**(): [`Engine`](Engine.md)

Gets the engine associated with the scene

#### Returns

[`Engine`](Engine.md)

an Engine

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1666

___

### getExternalData

▸ **getExternalData**`T`(`key`): [`Nullable`](../modules.md#nullable)`T`

Get an externally attached data from its key

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | `string` | the unique key that identifies the data |

#### Returns

[`Nullable`](../modules.md#nullable)`T`

the associated data, if present (can be null), or undefined if not present

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3541

___

### getFrameId

▸ **getFrameId**(): `number`

Gets an unique Id for the current frame

#### Returns

`number`

a number

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1762

___

### getGeometries

▸ **getGeometries**(): [`Geometry`](Geometry.md)[]

Gets the list of geometries attached to the scene

#### Returns

[`Geometry`](Geometry.md)[]

an array of Geometry

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3143

___

### getGeometryById

▸ **getGeometryById**(`id`): [`Nullable`](../modules.md#nullable)[`Geometry`](Geometry.md)

Gets a geometry using its Id

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | defines the geometry's Id |

#### Returns

[`Nullable`](../modules.md#nullable)[`Geometry`](Geometry.md)

the geometry or null if none found.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3058

___

### getGlowLayerByName

▸ **getGlowLayerByName**(`name`): [`Nullable`](../modules.md#nullable)[`GlowLayer`](GlowLayer.md)

Return a the first highlight layer of the scene with a given name.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | The name of the highlight layer to look for. |

#### Returns

[`Nullable`](../modules.md#nullable)[`GlowLayer`](GlowLayer.md)

The highlight layer if found otherwise null.

#### Inherited from

[AbstractScene](AbstractScene.md).[getGlowLayerByName](AbstractScene.md#getglowlayerbyname)

#### Defined in

https://github.com/babylon.js/core/src/Layers/glowLayer.ts:36

___

### getHighlightLayerByName

▸ **getHighlightLayerByName**(`name`): [`Nullable`](../modules.md#nullable)[`HighlightLayer`](HighlightLayer.md)

Return a the first highlight layer of the scene with a given name.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | The name of the highlight layer to look for. |

#### Returns

[`Nullable`](../modules.md#nullable)[`HighlightLayer`](HighlightLayer.md)

The highlight layer if found otherwise null.

#### Inherited from

[AbstractScene](AbstractScene.md).[getHighlightLayerByName](AbstractScene.md#gethighlightlayerbyname)

#### Defined in

https://github.com/babylon.js/core/src/Layers/highlightLayer.ts:41

___

### getInternalStep

▸ **getInternalStep**(): `number`

Gets the internal step used by deterministic lock step

**`See`**

https://doc.babylonjs.com/babylon101/animations#deterministic-lockstep

#### Returns

`number`

the internal step

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:901

___

### getLastEntryById

▸ **getLastEntryById**(`id`): [`Nullable`](../modules.md#nullable)[`Node`](Node.md)

Gets a the last added node (Mesh, Camera, Light) using a given Id

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | defines the Id to search for |

#### Returns

[`Nullable`](../modules.md#nullable)[`Node`](Node.md)

the found node or null if not found at all

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3249

___

### getLastMaterialById

▸ **getLastMaterialById**(`id`, `allowMultiMaterials?`): [`Nullable`](../modules.md#nullable)[`Material`](Material.md)

Gets a the last added material using a given id

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `id` | `string` | `undefined` | defines the material's Id |
| `allowMultiMaterials` | `boolean` | `false` | determines whether multimaterials should be considered |

#### Returns

[`Nullable`](../modules.md#nullable)[`Material`](Material.md)

the last material with the given id or null if none found.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2850

___

### getLastMeshById

▸ **getLastMeshById**(`id`): [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

Gets a the last added mesh using a given Id

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | defines the Id to search for |

#### Returns

[`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

the found mesh or null if not found at all.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3234

___

### getLastSkeletonById

▸ **getLastSkeletonById**(`id`): [`Nullable`](../modules.md#nullable)[`Skeleton`](Skeleton.md)

Gets a skeleton using a given Id (if many are found, this function will pick the last one)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | defines the Id to search for |

#### Returns

[`Nullable`](../modules.md#nullable)[`Skeleton`](Skeleton.md)

the found skeleton or null if not found at all.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3381

___

### getLensFlareSystemByID

▸ **getLensFlareSystemByID**(`id`): [`Nullable`](../modules.md#nullable)[`LensFlareSystem`](LensFlareSystem.md)

Gets a lens flare system using its Id

**`Deprecated`**

Please use getLensFlareSystemById instead

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | defines the Id to look for |

#### Returns

[`Nullable`](../modules.md#nullable)[`LensFlareSystem`](LensFlareSystem.md)

the lens flare system or null if not found

#### Inherited from

[AbstractScene](AbstractScene.md).[getLensFlareSystemByID](AbstractScene.md#getlensflaresystembyid)

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlareSystemSceneComponent.ts:60

___

### getLensFlareSystemById

▸ **getLensFlareSystemById**(`id`): [`Nullable`](../modules.md#nullable)[`LensFlareSystem`](LensFlareSystem.md)

Gets a lens flare system using its Id

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | defines the Id to look for |

#### Returns

[`Nullable`](../modules.md#nullable)[`LensFlareSystem`](LensFlareSystem.md)

the lens flare system or null if not found

#### Inherited from

[AbstractScene](AbstractScene.md).[getLensFlareSystemById](AbstractScene.md#getlensflaresystembyid-1)

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlareSystemSceneComponent.ts:67

___

### getLensFlareSystemByName

▸ **getLensFlareSystemByName**(`name`): [`Nullable`](../modules.md#nullable)[`LensFlareSystem`](LensFlareSystem.md)

Gets a lens flare system using its name

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the name to look for |

#### Returns

[`Nullable`](../modules.md#nullable)[`LensFlareSystem`](LensFlareSystem.md)

the lens flare system or null if not found

#### Inherited from

[AbstractScene](AbstractScene.md).[getLensFlareSystemByName](AbstractScene.md#getlensflaresystembyname)

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlareSystemSceneComponent.ts:52

___

### getLightById

▸ **getLightById**(`id`): [`Nullable`](../modules.md#nullable)[`Light`](Light.md)

Gets a light node using its Id

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | defines the light's Id |

#### Returns

[`Nullable`](../modules.md#nullable)[`Light`](Light.md)

the light or null if none found.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3013

___

### getLightByName

▸ **getLightByName**(`name`): [`Nullable`](../modules.md#nullable)[`Light`](Light.md)

Gets a light node using its name

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the the light's name |

#### Returns

[`Nullable`](../modules.md#nullable)[`Light`](Light.md)

the light or null if none found.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2998

___

### getLightByUniqueId

▸ **getLightByUniqueId**(`uniqueId`): [`Nullable`](../modules.md#nullable)[`Light`](Light.md)

Gets a light node using its scene-generated unique Id

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniqueId` | `number` | defines the light's unique Id |

#### Returns

[`Nullable`](../modules.md#nullable)[`Light`](Light.md)

the light or null if none found.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3028

___

### getLightsByTags

▸ **getLightsByTags**(`tagsQuery`, `forEach?`): [`Light`](Light.md)[]

Get a list of lights by tags

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `tagsQuery` | `string` | defines the tags query to use |
| `forEach?` | (`light`: [`Light`](Light.md)) => `void` | defines a predicate used to filter results |

#### Returns

[`Light`](Light.md)[]

an array of Light

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:5062

___

### getMaterialById

▸ **getMaterialById**(`id`): [`Nullable`](../modules.md#nullable)[`Material`](Material.md)

get a material using its id

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | defines the material's Id |

#### Returns

[`Nullable`](../modules.md#nullable)[`Material`](Material.md)

the material or null if none found.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2834

___

### getMaterialByName

▸ **getMaterialByName**(`name`): [`Nullable`](../modules.md#nullable)[`Material`](Material.md)

Gets a material using its name

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the material's name |

#### Returns

[`Nullable`](../modules.md#nullable)[`Material`](Material.md)

the material or null if none found.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2872

___

### getMaterialByTags

▸ **getMaterialByTags**(`tagsQuery`, `forEach?`): [`Material`](Material.md)[]

Get a list of materials by tags

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `tagsQuery` | `string` | defines the tags query to use |
| `forEach?` | (`material`: [`Material`](Material.md)) => `void` | defines a predicate used to filter results |

#### Returns

[`Material`](Material.md)[]

an array of Material

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:5072

___

### getMaterialByUniqueID

▸ **getMaterialByUniqueID**(`uniqueId`): [`Nullable`](../modules.md#nullable)[`Material`](Material.md)

Get a material using its unique id

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniqueId` | `number` | defines the material's unique id |

#### Returns

[`Nullable`](../modules.md#nullable)[`Material`](Material.md)

the material or null if none found.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2819

___

### getMeshById

▸ **getMeshById**(`id`): [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

Gets the first added mesh found of a given Id

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | defines the Id to search for |

#### Returns

[`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

the mesh found or null if not found at all

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3152

___

### getMeshByName

▸ **getMeshByName**(`name`): [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

Gets a mesh using a given name

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the name to search for |

#### Returns

[`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

the found mesh or null if not found at all.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3351

___

### getMeshByUniqueId

▸ **getMeshByUniqueId**(`uniqueId`): [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

Gets a mesh with its auto-generated unique Id

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniqueId` | `number` | defines the unique Id to search for |

#### Returns

[`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

the found mesh or null if not found at all.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3219

___

### getMeshesById

▸ **getMeshesById**(`id`): [`AbstractMesh`](AbstractMesh.md)[]

Gets a list of meshes using their Id

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | defines the Id to search for |

#### Returns

[`AbstractMesh`](AbstractMesh.md)[]

a list of meshes

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3167

___

### getMeshesByTags

▸ **getMeshesByTags**(`tagsQuery`, `forEach?`): [`Mesh`](Mesh.md)[]

Get a list of meshes by tags

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `tagsQuery` | `string` | defines the tags query to use |
| `forEach?` | (`mesh`: [`AbstractMesh`](AbstractMesh.md)) => `void` | defines a predicate used to filter results |

#### Returns

[`Mesh`](Mesh.md)[]

an array of Mesh

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:5042

___

### getMorphTargetById

▸ **getMorphTargetById**(`id`): [`Nullable`](../modules.md#nullable)[`MorphTarget`](MorphTarget.md)

Gets a morph target using a given id (if many are found, this function will pick the first one)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | defines the id to search for |

#### Returns

[`Nullable`](../modules.md#nullable)[`MorphTarget`](MorphTarget.md)

the found morph target or null if not found at all.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3456

___

### getMorphTargetByName

▸ **getMorphTargetByName**(`name`): [`Nullable`](../modules.md#nullable)[`MorphTarget`](MorphTarget.md)

Gets a morph target using a given name (if many are found, this function will pick the first one)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the name to search for |

#### Returns

[`Nullable`](../modules.md#nullable)[`MorphTarget`](MorphTarget.md)

the found morph target or null if not found at all.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3474

___

### getMorphTargetManagerById

▸ **getMorphTargetManagerById**(`id`): [`Nullable`](../modules.md#nullable)[`MorphTargetManager`](MorphTargetManager.md)

Gets a morph target manager  using a given id (if many are found, this function will pick the last one)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `number` | defines the id to search for |

#### Returns

[`Nullable`](../modules.md#nullable)[`MorphTargetManager`](MorphTargetManager.md)

the found morph target manager or null if not found at all.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3441

___

### getNodeById

▸ **getNodeById**(`id`): [`Nullable`](../modules.md#nullable)[`Node`](Node.md)

Gets a node (Mesh, Camera, Light) using a given Id

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | defines the Id to search for |

#### Returns

[`Nullable`](../modules.md#nullable)[`Node`](Node.md)

the found node or null if not found at all

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3283

___

### getNodeByName

▸ **getNodeByName**(`name`): [`Nullable`](../modules.md#nullable)[`Node`](Node.md)

Gets a node (Mesh, Camera, Light) using a given name

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the name to search for |

#### Returns

[`Nullable`](../modules.md#nullable)[`Node`](Node.md)

the found node or null if not found at all.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3317

___

### getNodes

▸ **getNodes**(): [`Node`](Node.md)[]

#### Returns

[`Node`](Node.md)[]

all meshes, lights, cameras, transformNodes and bones

#### Inherited from

[AbstractScene](AbstractScene.md).[getNodes](AbstractScene.md#getnodes)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:222

___

### getOrAddExternalDataWithFactory

▸ **getOrAddExternalDataWithFactory**`T`(`key`, `factory`): `T`

Get an externally attached data from its key, create it using a factory if it's not already present

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | `string` | the unique key that identifies the data |
| `factory` | (`k`: `string`) => `T` | the factory that will be called to create the instance if and only if it doesn't exists |

#### Returns

`T`

the associated data, can be null if the factory returned null.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3554

___

### getOutlineRenderer

▸ **getOutlineRenderer**(): [`OutlineRenderer`](OutlineRenderer.md)

Gets the outline renderer associated with the scene

#### Returns

[`OutlineRenderer`](OutlineRenderer.md)

a OutlineRenderer

#### Defined in

https://github.com/babylon.js/core/src/Rendering/outlineRenderer.ts:25

___

### getParticleSystemById

▸ **getParticleSystemById**(`id`): [`Nullable`](../modules.md#nullable)[`IParticleSystem`](../interfaces/IParticleSystem.md)

Gets a particle system by Id

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | defines the particle system Id |

#### Returns

[`Nullable`](../modules.md#nullable)[`IParticleSystem`](../interfaces/IParticleSystem.md)

the corresponding system or null if none found

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3043

___

### getPerfCollector

▸ **getPerfCollector**(): [`PerformanceViewerCollector`](PerformanceViewerCollector.md)

This method gets the performance collector belonging to the scene, which is generally shared with the inspector.

#### Returns

[`PerformanceViewerCollector`](PerformanceViewerCollector.md)

the perf collector belonging to the scene.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:5337

___

### getPhysicsEngine

▸ **getPhysicsEngine**(): [`Nullable`](../modules.md#nullable)[`IPhysicsEngine`](../interfaces/IPhysicsEngine.md)

Gets the current physics engine

#### Returns

[`Nullable`](../modules.md#nullable)[`IPhysicsEngine`](../interfaces/IPhysicsEngine.md)

a IPhysicsEngine or null if none attached

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsEngineComponent.ts:29

___

### getPointerOverMesh

▸ **getPointerOverMesh**(): [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

Gets the mesh under the pointer

#### Returns

[`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)

a Mesh or null if no mesh is under the pointer

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:4967

___

### getPointerOverSprite

▸ **getPointerOverSprite**(): [`Nullable`](../modules.md#nullable)[`Sprite`](Sprite.md)

Gets the sprite under the pointer

#### Returns

[`Nullable`](../modules.md#nullable)[`Sprite`](Sprite.md)

a Sprite or null if no sprite is under the pointer

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteSceneComponent.ts:96

___

### getPostProcessByName

▸ **getPostProcessByName**(`name`): [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)

Gets a post process using a given name (if many are found, this function will pick the first one)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the name to search for |

#### Returns

[`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)

the found post process or null if not found at all.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3492

___

### getProjectionMatrix

▸ **getProjectionMatrix**(): [`Matrix`](Matrix.md)

Gets the current projection matrix

#### Returns

[`Matrix`](Matrix.md)

a Matrix

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2158

___

### getRenderId

▸ **getRenderId**(): `number`

Gets an unique Id for the current render phase

#### Returns

`number`

a number

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1754

___

### getSceneUniformBuffer

▸ **getSceneUniformBuffer**(): [`UniformBuffer`](UniformBuffer.md)

Gets the uniform buffer used to store scene data

#### Returns

[`UniformBuffer`](UniformBuffer.md)

a UniformBuffer

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2214

___

### getSkeletonById

▸ **getSkeletonById**(`id`): [`Nullable`](../modules.md#nullable)[`Skeleton`](Skeleton.md)

Gets a skeleton using a given id (if many are found, this function will pick the first one)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | defines the id to search for |

#### Returns

[`Nullable`](../modules.md#nullable)[`Skeleton`](Skeleton.md)

the found skeleton or null if not found at all.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3411

___

### getSkeletonByName

▸ **getSkeletonByName**(`name`): [`Nullable`](../modules.md#nullable)[`Skeleton`](Skeleton.md)

Gets a skeleton using a given name

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the name to search for |

#### Returns

[`Nullable`](../modules.md#nullable)[`Skeleton`](Skeleton.md)

the found skeleton or null if not found at all.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3426

___

### getSkeletonByUniqueId

▸ **getSkeletonByUniqueId**(`uniqueId`): [`Nullable`](../modules.md#nullable)[`Skeleton`](Skeleton.md)

Gets a skeleton using a given auto generated unique id

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniqueId` | `number` | defines the unique id to search for |

#### Returns

[`Nullable`](../modules.md#nullable)[`Skeleton`](Skeleton.md)

the found skeleton or null if not found at all.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3396

___

### getSoundByName

▸ **getSoundByName**(`name`): [`Nullable`](../modules.md#nullable)[`Sound`](Sound.md)

Gets a sound using a given name

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the name to search for |

#### Returns

[`Nullable`](../modules.md#nullable)[`Sound`](Sound.md)

the found sound or null if not found at all.

#### Defined in

https://github.com/babylon.js/core/src/Audio/audioSceneComponent.ts:78

___

### getStepId

▸ **getStepId**(): `number`

Gets the step Id used by deterministic lock step

**`See`**

https://doc.babylonjs.com/babylon101/animations#deterministic-lockstep

#### Returns

`number`

the step Id

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:892

___

### getTextureByName

▸ **getTextureByName**(`name`): [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Gets a texture using its name

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the texture's name |

#### Returns

[`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

the texture or null if none found.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2902

___

### getTextureByUniqueId

▸ **getTextureByUniqueId**(`uniqueId`): [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Get a texture using its unique id

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniqueId` | `number` | defines the texture's unique id |

#### Returns

[`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

the texture or null if none found.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2887

___

### getTotalVertices

▸ **getTotalVertices**(): `number`

Gets the total number of vertices rendered per frame

#### Returns

`number`

the total number of vertices rendered per frame

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1674

___

### getTransformMatrix

▸ **getTransformMatrix**(): [`Matrix`](Matrix.md)

Gets the current transform matrix

#### Returns

[`Matrix`](Matrix.md)

a Matrix made of View * Projection

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2166

___

### getTransformNodeById

▸ **getTransformNodeById**(`id`): [`Nullable`](../modules.md#nullable)[`TransformNode`](TransformNode.md)

Gets the first added transform node found of a given Id

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | defines the Id to search for |

#### Returns

[`Nullable`](../modules.md#nullable)[`TransformNode`](TransformNode.md)

the found transform node or null if not found at all.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3178

___

### getTransformNodeByName

▸ **getTransformNodeByName**(`name`): [`Nullable`](../modules.md#nullable)[`TransformNode`](TransformNode.md)

Gets a transform node using a given name

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the name to search for |

#### Returns

[`Nullable`](../modules.md#nullable)[`TransformNode`](TransformNode.md)

the found transform node or null if not found at all.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3366

___

### getTransformNodeByUniqueId

▸ **getTransformNodeByUniqueId**(`uniqueId`): [`Nullable`](../modules.md#nullable)[`TransformNode`](TransformNode.md)

Gets a transform node with its auto-generated unique Id

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `uniqueId` | `number` | defines the unique Id to search for |

#### Returns

[`Nullable`](../modules.md#nullable)[`TransformNode`](TransformNode.md)

the found transform node or null if not found at all.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3193

___

### getTransformNodesById

▸ **getTransformNodesById**(`id`): [`TransformNode`](TransformNode.md)[]

Gets a list of transform nodes using their Id

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | defines the Id to search for |

#### Returns

[`TransformNode`](TransformNode.md)[]

a list of transform nodes

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3208

___

### getTransformNodesByTags

▸ **getTransformNodesByTags**(`tagsQuery`, `forEach?`): [`TransformNode`](TransformNode.md)[]

Get a list of transform nodes by tags

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `tagsQuery` | `string` | defines the tags query to use |
| `forEach?` | (`transform`: [`TransformNode`](TransformNode.md)) => `void` | defines a predicate used to filter results |

#### Returns

[`TransformNode`](TransformNode.md)[]

an array of TransformNode

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:5082

___

### getUniqueId

▸ **getUniqueId**(): `number`

Gets an unique (relatively to the current scene) Id

#### Returns

`number`

an unique number for the scene

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2247

___

### getViewMatrix

▸ **getViewMatrix**(): [`Matrix`](Matrix.md)

Gets the current view matrix

#### Returns

[`Matrix`](Matrix.md)

a Matrix

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2150

___

### getWaitingItemsCount

▸ **getWaitingItemsCount**(): `number`

Returns the number of items waiting to be loaded

#### Returns

`number`

the number of items waiting to be loaded

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2064

___

### getWorldExtends

▸ **getWorldExtends**(`filterPredicate?`): `Object`

Get the world extend vectors with an optional filter

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `filterPredicate?` | (`mesh`: [`AbstractMesh`](AbstractMesh.md)) => `boolean` | the predicate - which meshes should be included when calculating the world size |

#### Returns

`Object`

min and max vectors

| Name | Type |
| :------ | :------ |
| `max` | [`Vector3`](Vector3.md) |
| `min` | [`Vector3`](Vector3.md) |

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:4793

___

### incrementRenderId

▸ **incrementRenderId**(): `void`

Call this function if you want to manually increment the render Id

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1767

___

### isActiveMesh

▸ **isActiveMesh**(`mesh`): `boolean`

Gets a boolean indicating if the given mesh is active

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) | defines the mesh to look for |

#### Returns

`boolean`

true if the mesh is in the active list

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3507

___

### isCachedMaterialInvalid

▸ **isCachedMaterialInvalid**(`material`, `effect`, `visibility?`): `boolean`

Gets a boolean indicating if the current material / effect / visibility must be bind again

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `material` | [`Material`](Material.md) | `undefined` | defines the current material |
| `effect` | [`Effect`](Effect.md) | `undefined` | defines the current effect |
| `visibility` | `number` | `1` | defines the current visibility state |

#### Returns

`boolean`

true if one parameter is not cached

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1658

___

### isPhysicsEnabled

▸ **isPhysicsEnabled**(): `boolean`

Gets a boolean indicating if there is an active physics engine

#### Returns

`boolean`

a boolean indicating if there is an active physics engine

#### Defined in

https://github.com/babylon.js/core/src/Physics/physicsEngineComponent.ts:48

___

### isPointerCaptured

▸ **isPointerCaptured**(`pointerId?`): `boolean`

Gets a boolean indicating if the current pointer event is captured (meaning that the scene has already handled the pointer down)

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `pointerId` | `number` | `0` | defines the pointer id to use in a multi-touch scenario (0 by default) |

#### Returns

`boolean`

true if the pointer was captured

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1817

___

### isReady

▸ **isReady**(`checkRenderTargets?`): `boolean`

This function will check if the scene can be rendered (textures are loaded, shaders are compiled)
Delay loaded resources are not taking in account

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `checkRenderTargets` | `boolean` | `true` | true to also check that the meshes rendered as part of a render target are ready (default: true) |

#### Returns

`boolean`

true if all required resources are ready

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1842

___

### markAllMaterialsAsDirty

▸ **markAllMaterialsAsDirty**(`flag`, `predicate?`): `void`

Will flag all materials as dirty to trigger new shader compilation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `flag` | `number` | defines the flag used to specify which material part must be marked as dirty |
| `predicate?` | (`mat`: [`Material`](Material.md)) => `boolean` | If not null, it will be used to specify if a material has to be marked as dirty |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:5151

___

### multiPick

▸ **multiPick**(`x`, `y`, `predicate?`, `camera?`, `trianglePredicate?`): [`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md)[]

Launch a ray to try to pick a mesh in the scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | X position on screen |
| `y` | `number` | Y position on screen |
| `predicate?` | (`mesh`: [`AbstractMesh`](AbstractMesh.md)) => `boolean` | Predicate function used to determine eligible meshes. Can be set to null. In this case, a mesh must be enabled, visible and with isPickable set to true |
| `camera?` | [`Camera`](Camera.md) | camera to use for computing the picking ray. Can be set to null. In this case, the scene.activeCamera will be used |
| `trianglePredicate?` | [`TrianglePickingPredicate`](../modules.md#trianglepickingpredicate) | defines an optional predicate used to select faces when a mesh intersection is detected |

#### Returns

[`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md)[]

an array of PickingInfo

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:4938

___

### multiPickSprite

▸ **multiPickSprite**(`x`, `y`, `predicate?`, `camera?`): [`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md)[]

Launch a ray to try to pick sprites in the scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | position on screen |
| `y` | `number` | position on screen |
| `predicate?` | (`sprite`: [`Sprite`](Sprite.md)) => `boolean` | Predicate function used to determine eligible sprites. Can be set to null. In this case, a sprite must have isPickable set to true |
| `camera?` | [`Camera`](Camera.md) | camera to use for computing the picking ray. Can be set to null. In this case, the scene.activeCamera will be used |

#### Returns

[`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md)[]

a PickingInfo array

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteSceneComponent.ts:76

___

### multiPickSpriteWithRay

▸ **multiPickSpriteWithRay**(`ray`, `predicate?`, `camera?`): [`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md)[]

Use the given ray to pick sprites in the scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ray` | [`Ray`](Ray.md) | The ray (in world space) to use to pick meshes |
| `predicate?` | (`sprite`: [`Sprite`](Sprite.md)) => `boolean` | Predicate function used to determine eligible sprites. Can be set to null. In this case, a sprite must have isPickable set to true |
| `camera?` | [`Camera`](Camera.md) | camera to use. Can be set to null. In this case, the scene.activeCamera will be used |

#### Returns

[`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md)[]

a PickingInfo array

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteSceneComponent.ts:84

___

### multiPickWithRay

▸ **multiPickWithRay**(`ray`, `predicate`, `trianglePredicate?`): [`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md)[]

Launch a ray to try to pick a mesh in the scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ray` | [`Ray`](Ray.md) | Ray to use |
| `predicate` | (`mesh`: [`AbstractMesh`](AbstractMesh.md)) => `boolean` | Predicate function used to determine eligible meshes. Can be set to null. In this case, a mesh must be enabled, visible and with isPickable set to true |
| `trianglePredicate?` | [`TrianglePickingPredicate`](../modules.md#trianglepickingpredicate) | defines an optional predicate used to select faces when a mesh intersection is detected |

#### Returns

[`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md)[]

an array of PickingInfo

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:4949

___

### pick

▸ **pick**(`x`, `y`, `predicate?`, `fastCheck?`, `camera?`, `trianglePredicate?`): [`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md)

Launch a ray to try to pick a mesh in the scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | position on screen |
| `y` | `number` | position on screen |
| `predicate?` | (`mesh`: [`AbstractMesh`](AbstractMesh.md)) => `boolean` | Predicate function used to determine eligible meshes. Can be set to null. In this case, a mesh must be enabled, visible and with isPickable set to true |
| `fastCheck?` | `boolean` | defines if the first intersection will be used (and not the closest) |
| `camera?` | [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md) | to use for computing the picking ray. Can be set to null. In this case, the scene.activeCamera will be used |
| `trianglePredicate?` | [`TrianglePickingPredicate`](../modules.md#trianglepickingpredicate) | defines an optional predicate used to select faces when a mesh intersection is detected |

#### Returns

[`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md)

a PickingInfo

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:4889

___

### pickSprite

▸ **pickSprite**(`x`, `y`, `predicate?`, `fastCheck?`, `camera?`): [`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md)

Launch a ray to try to pick a sprite in the scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | position on screen |
| `y` | `number` | position on screen |
| `predicate?` | (`sprite`: [`Sprite`](Sprite.md)) => `boolean` | Predicate function used to determine eligible sprites. Can be set to null. In this case, a sprite must have isPickable set to true |
| `fastCheck?` | `boolean` | defines if the first intersection will be used (and not the closest) |
| `camera?` | [`Camera`](Camera.md) | camera to use for computing the picking ray. Can be set to null. In this case, the scene.activeCamera will be used |

#### Returns

[`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md)

a PickingInfo

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteSceneComponent.ts:55

___

### pickSpriteWithRay

▸ **pickSpriteWithRay**(`ray`, `predicate?`, `fastCheck?`, `camera?`): [`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md)

Use the given ray to pick a sprite in the scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ray` | [`Ray`](Ray.md) | The ray (in world space) to use to pick meshes |
| `predicate?` | (`sprite`: [`Sprite`](Sprite.md)) => `boolean` | Predicate function used to determine eligible sprites. Can be set to null. In this case, a sprite must have isPickable set to true |
| `fastCheck?` | `boolean` | defines if the first intersection will be used (and not the closest) |
| `camera?` | [`Camera`](Camera.md) | camera to use. Can be set to null. In this case, the scene.activeCamera will be used |

#### Returns

[`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md)

a PickingInfo

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteSceneComponent.ts:64

___

### pickWithBoundingInfo

▸ **pickWithBoundingInfo**(`x`, `y`, `predicate?`, `fastCheck?`, `camera?`): [`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md)

Launch a ray to try to pick a mesh in the scene using only bounding information of the main mesh (not using submeshes)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | position on screen |
| `y` | `number` | position on screen |
| `predicate?` | (`mesh`: [`AbstractMesh`](AbstractMesh.md)) => `boolean` | Predicate function used to determine eligible meshes. Can be set to null. In this case, a mesh must be enabled, visible and with isPickable set to true |
| `fastCheck?` | `boolean` | defines if the first intersection will be used (and not the closest) |
| `camera?` | [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md) | to use for computing the picking ray. Can be set to null. In this case, the scene.activeCamera will be used |

#### Returns

[`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md)

a PickingInfo (Please note that some info will not be set like distance, bv, bu and everything that cannot be capture by only using bounding infos)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:4911

___

### pickWithRay

▸ **pickWithRay**(`ray`, `predicate?`, `fastCheck?`, `trianglePredicate?`): [`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md)

Use the given ray to pick a mesh in the scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ray` | [`Ray`](Ray.md) | The ray to use to pick meshes |
| `predicate?` | (`mesh`: [`AbstractMesh`](AbstractMesh.md)) => `boolean` | Predicate function used to determine eligible meshes. Can be set to null. In this case, a mesh must have isPickable set to true |
| `fastCheck?` | `boolean` | defines if the first intersection will be used (and not the closest) |
| `trianglePredicate?` | [`TrianglePickingPredicate`](../modules.md#trianglepickingpredicate) | defines an optional predicate used to select faces when a mesh intersection is detected |

#### Returns

[`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md)

a PickingInfo

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:4925

___

### pushGeometry

▸ **pushGeometry**(`geometry`, `force?`): `boolean`

Add a new geometry to this scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `geometry` | [`Geometry`](Geometry.md) | defines the geometry to be added to the scene. |
| `force?` | `boolean` | defines if the geometry must be pushed even if a geometry with this id already exists |

#### Returns

`boolean`

a boolean defining if the geometry was added or not

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3091

___

### registerAfterRender

▸ **registerAfterRender**(`func`): `void`

Registers a function to be called after every frame render

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `func` | () => `void` | defines the function to register |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1996

___

### registerBeforeRender

▸ **registerBeforeRender**(`func`): `void`

Registers a function to be called before every frame render

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `func` | () => `void` | defines the function to register |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1980

___

### removeActionManager

▸ **removeActionManager**(`toRemove`): `number`

Removes the given action manager from this scene.

**`Deprecated`**

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `toRemove` | [`AbstractActionManager`](AbstractActionManager.md) | The action manager to remove |

#### Returns

`number`

The index of the removed action manager

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2547

___

### removeAnimation

▸ **removeAnimation**(`toRemove`): `number`

Remove a animation for the list of scene's animations

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `toRemove` | [`Animation`](Animation.md) | defines the animation to remove |

#### Returns

`number`

the index where the animation was in the animation list

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2471

___

### removeAnimationGroup

▸ **removeAnimationGroup**(`toRemove`): `number`

Removes the given animation group from this scene.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `toRemove` | [`AnimationGroup`](AnimationGroup.md) | The animation group to remove |

#### Returns

`number`

The index of the removed animation group

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2494

___

### removeCamera

▸ **removeCamera**(`toRemove`): `number`

Remove a camera for the list of scene's cameras

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `toRemove` | [`Camera`](Camera.md) | defines the camera to remove |

#### Returns

`number`

the index where the camera was in the camera list

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2421

___

### removeEffectLayer

▸ **removeEffectLayer**(`toRemove`): `number`

Removes the given effect layer from this scene.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `toRemove` | [`EffectLayer`](EffectLayer.md) | defines the effect layer to remove |

#### Returns

`number`

the index of the removed effect layer

#### Inherited from

[AbstractScene](AbstractScene.md).[removeEffectLayer](AbstractScene.md#removeeffectlayer)

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayerSceneComponent.ts:40

___

### removeExternalData

▸ **removeExternalData**(`key`): `boolean`

Remove an externally attached data from the Engine instance

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | `string` | the unique key that identifies the data |

#### Returns

`boolean`

true if the data was successfully removed, false if it doesn't exist

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3566

___

### removeGeometry

▸ **removeGeometry**(`geometry`): `boolean`

Removes an existing geometry

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `geometry` | [`Geometry`](Geometry.md) | defines the geometry to be removed from the scene |

#### Returns

`boolean`

a boolean defining if the geometry was removed or not

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3108

___

### removeLensFlareSystem

▸ **removeLensFlareSystem**(`toRemove`): `number`

Removes the given lens flare system from this scene.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `toRemove` | [`LensFlareSystem`](LensFlareSystem.md) | The lens flare system to remove |

#### Returns

`number`

The index of the removed lens flare system

#### Inherited from

[AbstractScene](AbstractScene.md).[removeLensFlareSystem](AbstractScene.md#removelensflaresystem)

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlareSystemSceneComponent.ts:39

___

### removeLight

▸ **removeLight**(`toRemove`): `number`

Remove a light for the list of scene's lights

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `toRemove` | [`Light`](Light.md) | defines the light to remove |

#### Returns

`number`

the index where the light was in the light list

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2396

___

### removeMaterial

▸ **removeMaterial**(`toRemove`): `number`

Removes the given material from this scene.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `toRemove` | [`Material`](Material.md) | The material to remove |

#### Returns

`number`

The index of the removed material

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2523

___

### removeMesh

▸ **removeMesh**(`toRemove`, `recursive?`): `number`

Remove a mesh for the list of scene's meshes

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `toRemove` | [`AbstractMesh`](AbstractMesh.md) | `undefined` | defines the mesh to remove |
| `recursive` | `boolean` | `false` | if all child meshes should also be removed from the scene |

#### Returns

`number`

the index where the mesh was in the mesh list

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2284

___

### removeMorphTargetManager

▸ **removeMorphTargetManager**(`toRemove`): `number`

Remove a morph target for the list of scene's morph targets

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `toRemove` | [`MorphTargetManager`](MorphTargetManager.md) | defines the morph target to remove |

#### Returns

`number`

the index where the morph target was in the morph target list

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2381

___

### removeMultiMaterial

▸ **removeMultiMaterial**(`toRemove`): `number`

Removes the given multi-material from this scene.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `toRemove` | [`MultiMaterial`](MultiMaterial.md) | The multi-material to remove |

#### Returns

`number`

The index of the removed multi-material

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2507

___

### removeParticleSystem

▸ **removeParticleSystem**(`toRemove`): `number`

Remove a particle system for the list of scene's particle systems

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `toRemove` | [`IParticleSystem`](../interfaces/IParticleSystem.md) | defines the particle system to remove |

#### Returns

`number`

the index where the particle system was in the particle system list

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2455

___

### removePendingData

▸ **removePendingData**(`data`): `void`

Remove a pending data from the loading list which has previously been added with addPendingData.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `any` | defines the object to remove from the pending list |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2047

___

### removeReflectionProbe

▸ **removeReflectionProbe**(`toRemove`): `number`

Removes the given reflection probe from this scene.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `toRemove` | [`ReflectionProbe`](ReflectionProbe.md) | The reflection probe to remove |

#### Returns

`number`

The index of the removed reflection probe

#### Inherited from

[AbstractScene](AbstractScene.md).[removeReflectionProbe](AbstractScene.md#removereflectionprobe)

#### Defined in

https://github.com/babylon.js/core/src/Probes/reflectionProbe.ts:24

___

### removeSkeleton

▸ **removeSkeleton**(`toRemove`): `number`

Remove a skeleton for the list of scene's skeletons

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `toRemove` | [`Skeleton`](Skeleton.md) | defines the skeleton to remove |

#### Returns

`number`

the index where the skeleton was in the skeleton list

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2362

___

### removeTexture

▸ **removeTexture**(`toRemove`): `number`

Removes the given texture from this scene.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `toRemove` | [`BaseTexture`](BaseTexture.md) | The texture to remove |

#### Returns

`number`

The index of the removed texture

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2560

___

### removeTransformNode

▸ **removeTransformNode**(`toRemove`): `number`

Remove a transform node for the list of scene's transform nodes

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `toRemove` | [`TransformNode`](TransformNode.md) | defines the transform node to remove |

#### Returns

`number`

the index where the transform node was in the transform node list

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2336

___

### render

▸ **render**(`updateCameras?`, `ignoreAnimations?`): `void`

Render the scene

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `updateCameras` | `boolean` | `true` | defines a boolean indicating if cameras must update according to their inputs (true by default) |
| `ignoreAnimations` | `boolean` | `false` | defines a boolean indicating if animations should not be executed (false by default) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:4340

___

### resetCachedMaterial

▸ **resetCachedMaterial**(): `void`

Resets all cached information relative to material (including effect and visibility)

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1970

___

### resetDrawCache

▸ **resetDrawCache**(`passId?`): `void`

Resets the draw wrappers cache of all meshes

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `passId?` | `number` | If provided, releases only the draw wrapper corresponding to this render pass id |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:4325

___

### resetLastAnimationTimeFrame

▸ **resetLastAnimationTimeFrame**(): `void`

Resets the last animation time frame.
Useful to override when animations start running when loading a scene for the first time.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2140

___

### setActiveCameraById

▸ **setActiveCameraById**(`id`): [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md)

sets the active camera of the scene using its Id

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | defines the camera's Id |

#### Returns

[`Nullable`](../modules.md#nullable)[`Camera`](Camera.md)

the new active camera or null if none found.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2772

___

### setActiveCameraByName

▸ **setActiveCameraByName**(`name`): [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md)

sets the active camera of the scene using its name

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the camera's name |

#### Returns

[`Nullable`](../modules.md#nullable)[`Camera`](Camera.md)

the new active camera or null if none found.

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2788

___

### setDefaultCandidateProviders

▸ **setDefaultCandidateProviders**(): `void`

Sets the default candidate providers for the scene.
This sets the getActiveMeshCandidates, getActiveSubMeshCandidates, getIntersectingSubMeshCandidates
and getCollidingSubMeshCandidates to their default function

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1590

___

### setPointerOverMesh

▸ **setPointerOverMesh**(`mesh`, `pointerId?`, `pickResult?`): `void`

Force the value of meshUnderPointer

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mesh` | [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md) | defines the mesh to use |
| `pointerId?` | `number` | optional pointer id when using more than one pointer |
| `pickResult?` | [`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md) | optional pickingInfo data used to find mesh |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:4959

___

### setPointerOverSprite

▸ **setPointerOverSprite**(`sprite`): `void`

Force the sprite under the pointer

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sprite` | [`Nullable`](../modules.md#nullable)[`Sprite`](Sprite.md) | defines the sprite to use |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteSceneComponent.ts:90

___

### setRenderingAutoClearDepthStencil

▸ **setRenderingAutoClearDepthStencil**(`renderingGroupId`, `autoClearDepthStencil`, `depth?`, `stencil?`): `void`

Specifies whether or not the stencil and depth buffer are cleared between two rendering groups.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `renderingGroupId` | `number` | `undefined` | The rendering group id corresponding to its index |
| `autoClearDepthStencil` | `boolean` | `undefined` | Automatically clears depth and stencil between groups if true. |
| `depth` | `boolean` | `true` | Automatically clears depth between groups if true and autoClear is true. |
| `stencil` | `boolean` | `true` | Automatically clears stencil between groups if true and autoClear is true. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:5112

___

### setRenderingOrder

▸ **setRenderingOrder**(`renderingGroupId`, `opaqueSortCompareFn?`, `alphaTestSortCompareFn?`, `transparentSortCompareFn?`): `void`

Overrides the default sort function applied in the rendering group to prepare the meshes.
This allowed control for front to back rendering or reversly depending of the special needs.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `renderingGroupId` | `number` | `undefined` | The rendering group id corresponding to its index |
| `opaqueSortCompareFn` | [`Nullable`](../modules.md#nullable)(`a`: [`SubMesh`](SubMesh.md), `b`: [`SubMesh`](SubMesh.md)) => `number` | `null` | The opaque queue comparison function use to sort. |
| `alphaTestSortCompareFn` | [`Nullable`](../modules.md#nullable)(`a`: [`SubMesh`](SubMesh.md), `b`: [`SubMesh`](SubMesh.md)) => `number` | `null` | The alpha test queue comparison function use to sort. |
| `transparentSortCompareFn` | [`Nullable`](../modules.md#nullable)(`a`: [`SubMesh`](SubMesh.md), `b`: [`SubMesh`](SubMesh.md)) => `number` | `null` | The transparent queue comparison function use to sort. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:5095

___

### setSceneUniformBuffer

▸ **setSceneUniformBuffer**(`ubo`): `void`

Sets the scene ubo

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ubo` | [`UniformBuffer`](UniformBuffer.md) | the ubo to set for the scene |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2237

___

### setStepId

▸ **setStepId**(`newStepId`): `void`

Sets the step Id used by deterministic lock step

**`See`**

https://doc.babylonjs.com/babylon101/animations#deterministic-lockstep

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newStepId` | `number` | defines the step Id |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:883

___

### setTransformMatrix

▸ **setTransformMatrix**(`viewL`, `projectionL`, `viewR?`, `projectionR?`): `void`

Sets the current transform matrix

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `viewL` | [`Matrix`](Matrix.md) | defines the View matrix to use |
| `projectionL` | [`Matrix`](Matrix.md) | defines the Projection matrix to use |
| `viewR?` | [`Matrix`](Matrix.md) | defines the right View matrix to use (if provided) |
| `projectionR?` | [`Matrix`](Matrix.md) | defines the right Projection matrix to use (if provided) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2177

___

### simulatePointerDown

▸ **simulatePointerDown**(`pickResult`, `pointerEventInit?`): [`Scene`](Scene.md)

Use this method to simulate a pointer down on a mesh
The pickResult parameter can be obtained from a scene.pick or scene.pickWithRay

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `pickResult` | [`PickingInfo`](PickingInfo.md) | pickingInfo of the object wished to simulate pointer event on |
| `pointerEventInit?` | `PointerEventInit` | pointer event state to be used when simulating the pointer event (eg. pointer id for multitouch) |

#### Returns

[`Scene`](Scene.md)

the current scene

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1794

___

### simulatePointerMove

▸ **simulatePointerMove**(`pickResult`, `pointerEventInit?`): [`Scene`](Scene.md)

Use this method to simulate a pointer move on a mesh
The pickResult parameter can be obtained from a scene.pick or scene.pickWithRay

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `pickResult` | [`PickingInfo`](PickingInfo.md) | pickingInfo of the object wished to simulate pointer event on |
| `pointerEventInit?` | `PointerEventInit` | pointer event state to be used when simulating the pointer event (eg. pointer id for multitouch) |

#### Returns

[`Scene`](Scene.md)

the current scene

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1782

___

### simulatePointerUp

▸ **simulatePointerUp**(`pickResult`, `pointerEventInit?`, `doubleTap?`): [`Scene`](Scene.md)

Use this method to simulate a pointer up on a mesh
The pickResult parameter can be obtained from a scene.pick or scene.pickWithRay

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `pickResult` | [`PickingInfo`](PickingInfo.md) | pickingInfo of the object wished to simulate pointer event on |
| `pointerEventInit?` | `PointerEventInit` | pointer event state to be used when simulating the pointer event (eg. pointer id for multitouch) |
| `doubleTap?` | `boolean` | indicates that the pointer up event should be considered as part of a double click (false by default) |

#### Returns

[`Scene`](Scene.md)

the current scene

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1807

___

### sortLightsByPriority

▸ **sortLightsByPriority**(): `void`

Sorts the list list based on light priorities

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2599

___

### stopAllAnimations

▸ **stopAllAnimations**(): `void`

Stops and removes all animations that have been applied to the scene

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Animations/animatable.ts:633

___

### stopAnimation

▸ **stopAnimation**(`target`, `animationName?`, `targetMask?`): `void`

Will stop the animation of the given target

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `target` | `any` | the target |
| `animationName?` | `string` | the name of the animation to stop (all animations will be stopped if both this and targetMask are empty) |
| `targetMask?` | (`target`: `any`) => `boolean` | a function that determines if the animation should be stopped based on its target (all animations will be stopped if both this and animationName are empty) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2485

___

### switchActiveCamera

▸ **switchActiveCamera**(`newCamera`, `attachControl?`): `void`

Switch active camera

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `newCamera` | [`Camera`](Camera.md) | `undefined` | defines the new active camera |
| `attachControl` | `boolean` | `true` | defines if attachControl must be called for the new active camera (default: true) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2751

___

### unfreezeActiveMeshes

▸ **unfreezeActiveMeshes**(): [`Scene`](Scene.md)

Use this function to restart evaluating active meshes on every frame

#### Returns

[`Scene`](Scene.md)

the current scene

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3750

___

### unfreezeMaterials

▸ **unfreezeMaterials**(): `void`

Unfreeze all materials
A frozen material will not be updatable but should be faster to render

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:4533

___

### unregisterAfterRender

▸ **unregisterAfterRender**(`func`): `void`

Unregisters a function called after every frame render

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `func` | () => `void` | defines the function to unregister |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2004

___

### unregisterBeforeRender

▸ **unregisterBeforeRender**(`func`): `void`

Unregisters a function called before every frame render

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `func` | () => `void` | defines the function to unregister |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:1988

___

### updateTransformMatrix

▸ **updateTransformMatrix**(`force?`): `void`

Update the transform matrix to update from the current active camera

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `force?` | `boolean` | defines a boolean used to force the update even if cache is up to date |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:3951

___

### whenReadyAsync

▸ **whenReadyAsync**(`checkRenderTargets?`): `Promise``void`

Returns a promise that resolves when the scene is ready

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `checkRenderTargets` | `boolean` | `false` | true to also check that the meshes rendered as part of a render target are ready (default: false) |

#### Returns

`Promise``void`

A promise that resolves when the scene is ready

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:2095

___

### AddIndividualParser

▸ `Static` **AddIndividualParser**(`name`, `parser`): `void`

Adds n individual parser in the list of available ones

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Defines the name of the parser |
| `parser` | [`IndividualBabylonFileParser`](../modules.md#individualbabylonfileparser) | Defines the parser to add |

#### Returns

`void`

#### Inherited from

[AbstractScene](AbstractScene.md).[AddIndividualParser](AbstractScene.md#addindividualparser)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:77

___

### AddParser

▸ `Static` **AddParser**(`name`, `parser`): `void`

Adds a parser in the list of available ones

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Defines the name of the parser |
| `parser` | [`BabylonFileParser`](../modules.md#babylonfileparser) | Defines the parser to add |

#### Returns

`void`

#### Inherited from

[AbstractScene](AbstractScene.md).[AddParser](AbstractScene.md#addparser)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:55

___

### CollisionCoordinatorFactory

▸ `Static` **CollisionCoordinatorFactory**(): `ICollisionCoordinator`

Factory used to create the a collision coordinator.

#### Returns

`ICollisionCoordinator`

The collision coordinator

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:168

___

### DefaultMaterialFactory

▸ `Static` **DefaultMaterialFactory**(`scene`): [`Material`](Material.md)

Factory used to create the default material.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | The scene to create the material for |

#### Returns

[`Material`](Material.md)

The default material

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:160

___

### GetIndividualParser

▸ `Static` **GetIndividualParser**(`name`): [`Nullable`](../modules.md#nullable)[`IndividualBabylonFileParser`](../modules.md#individualbabylonfileparser)

Gets an individual parser from the list of available ones

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Defines the name of the parser |

#### Returns

[`Nullable`](../modules.md#nullable)[`IndividualBabylonFileParser`](../modules.md#individualbabylonfileparser)

the requested parser or null

#### Inherited from

[AbstractScene](AbstractScene.md).[GetIndividualParser](AbstractScene.md#getindividualparser)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:86

___

### GetParser

▸ `Static` **GetParser**(`name`): [`Nullable`](../modules.md#nullable)[`BabylonFileParser`](../modules.md#babylonfileparser)

Gets a general parser from the list of available ones

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | Defines the name of the parser |

#### Returns

[`Nullable`](../modules.md#nullable)[`BabylonFileParser`](../modules.md#babylonfileparser)

the requested parser or null

#### Inherited from

[AbstractScene](AbstractScene.md).[GetParser](AbstractScene.md#getparser)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:64

___

### Parse

▸ `Static` **Parse**(`jsonData`, `scene`, `container`, `rootUrl`): `void`

Parser json data and populate both a scene and its associated container object

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `jsonData` | `any` | Defines the data to parse |
| `scene` | [`Scene`](Scene.md) | Defines the scene to parse the data for |
| `container` | [`AssetContainer`](AssetContainer.md) | Defines the container attached to the parsing sequence |
| `rootUrl` | `string` | Defines the root url of the data |

#### Returns

`void`

#### Inherited from

[AbstractScene](AbstractScene.md).[Parse](AbstractScene.md#parse)

#### Defined in

https://github.com/babylon.js/core/src/abstractScene.ts:101
