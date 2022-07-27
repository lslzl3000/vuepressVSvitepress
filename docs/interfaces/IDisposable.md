[@dev/core](../README.md) / [Exports](../modules.md) / IDisposable

# Interface: IDisposable

Define an interface for all classes that will hold resources

## Hierarchy

- **`IDisposable`**

  ↳ [`IAudioEngine`](IAudioEngine.md)

  ↳ [`IEdgesRenderer`](IEdgesRenderer.md)

  ↳ [`ISpriteManager`](ISpriteManager.md)

  ↳ [`ISpriteMap`](ISpriteMap.md)

  ↳ [`WebXRRenderTarget`](WebXRRenderTarget.md)

  ↳ [`IWebXRFeature`](IWebXRFeature.md)

## Implemented by

- [`AbstractActionManager`](../classes/AbstractActionManager.md)
- [`AbstractMesh`](../classes/AbstractMesh.md)
- [`AdvancedTimer`](../classes/AdvancedTimer.md)
- [`AnimationGroup`](../classes/AnimationGroup.md)
- [`DefaultRenderingPipeline`](../classes/DefaultRenderingPipeline.md)
- [`DeviceSourceManager`](../classes/DeviceSourceManager.md)
- [`DracoCompression`](../classes/DracoCompression.md)
- [`Effect`](../classes/Effect.md)
- [`EngineInstrumentation`](../classes/EngineInstrumentation.md)
- [`GPUParticleSystem`](../classes/GPUParticleSystem.md)
- [`Gizmo`](../classes/Gizmo.md)
- [`GizmoManager`](../classes/GizmoManager.md)
- [`MeshoptCompression`](../classes/MeshoptCompression.md)
- [`MorphTargetManager`](../classes/MorphTargetManager.md)
- [`ParticleSystem`](../classes/ParticleSystem.md)
- [`ParticleSystemSet`](../classes/ParticleSystemSet.md)
- [`PointsCloudSystem`](../classes/PointsCloudSystem.md)
- [`SceneInstrumentation`](../classes/SceneInstrumentation.md)
- [`SceneOptimizer`](../classes/SceneOptimizer.md)
- [`SolidParticleSystem`](../classes/SolidParticleSystem.md)
- [`StandardRenderingPipeline`](../classes/StandardRenderingPipeline.md)
- [`UtilityLayerRenderer`](../classes/UtilityLayerRenderer.md)
- [`WebXRAbstractMotionController`](../classes/WebXRAbstractMotionController.md)
- [`WebXRControllerComponent`](../classes/WebXRControllerComponent.md)
- [`WebXREnterExitUI`](../classes/WebXREnterExitUI.md)
- [`WebXRExperienceHelper`](../classes/WebXRExperienceHelper.md)
- [`WebXRFeaturesManager`](../classes/WebXRFeaturesManager.md)
- [`WebXRHand`](../classes/WebXRHand.md)
- [`WebXRInput`](../classes/WebXRInput.md)
- [`WebXRSessionManager`](../classes/WebXRSessionManager.md)
- [`WorkerPool`](../classes/WorkerPool.md)

## Table of contents

### Methods

- [dispose](IDisposable.md#dispose)

## Methods

### dispose

▸ **dispose**(): `void`

Releases all held resources

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:103
