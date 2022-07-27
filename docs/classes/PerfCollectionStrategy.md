[@dev/core](../README.md) / [Exports](../modules.md) / PerfCollectionStrategy

# Class: PerfCollectionStrategy

Defines the predefined strategies used in the performance viewer.

## Table of contents

### Constructors

- [constructor](PerfCollectionStrategy.md#constructor)

### Methods

- [AbsoluteFpsStrategy](PerfCollectionStrategy.md#absolutefpsstrategy)
- [ActiveBonesStrategy](PerfCollectionStrategy.md#activebonesstrategy)
- [ActiveFacesStrategy](PerfCollectionStrategy.md#activefacesstrategy)
- [ActiveIndicesStrategy](PerfCollectionStrategy.md#activeindicesstrategy)
- [ActiveMeshesStrategy](PerfCollectionStrategy.md#activemeshesstrategy)
- [ActiveParticlesStrategy](PerfCollectionStrategy.md#activeparticlesstrategy)
- [AnimationsStrategy](PerfCollectionStrategy.md#animationsstrategy)
- [CpuStrategy](PerfCollectionStrategy.md#cpustrategy)
- [DrawCallsStrategy](PerfCollectionStrategy.md#drawcallsstrategy)
- [FpsStrategy](PerfCollectionStrategy.md#fpsstrategy)
- [FrameTotalStrategy](PerfCollectionStrategy.md#frametotalstrategy)
- [GpuFrameTimeStrategy](PerfCollectionStrategy.md#gpuframetimestrategy)
- [InterFrameStrategy](PerfCollectionStrategy.md#interframestrategy)
- [MeshesSelectionStrategy](PerfCollectionStrategy.md#meshesselectionstrategy)
- [ParticlesStrategy](PerfCollectionStrategy.md#particlesstrategy)
- [PhysicsStrategy](PerfCollectionStrategy.md#physicsstrategy)
- [RenderStrategy](PerfCollectionStrategy.md#renderstrategy)
- [RenderTargetsStrategy](PerfCollectionStrategy.md#rendertargetsstrategy)
- [SpritesStrategy](PerfCollectionStrategy.md#spritesstrategy)
- [TotalLightsStrategy](PerfCollectionStrategy.md#totallightsstrategy)
- [TotalMaterialsStrategy](PerfCollectionStrategy.md#totalmaterialsstrategy)
- [TotalMeshesStrategy](PerfCollectionStrategy.md#totalmeshesstrategy)
- [TotalTexturesStrategy](PerfCollectionStrategy.md#totaltexturesstrategy)
- [TotalVerticesStrategy](PerfCollectionStrategy.md#totalverticesstrategy)

## Constructors

### constructor

• **new PerfCollectionStrategy**()

## Methods

### AbsoluteFpsStrategy

▸ `Static` **AbsoluteFpsStrategy**(): [`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

Gets the initializer for the strategy used for collection of absolute fps metrics.

#### Returns

[`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

the initializer for the absolute fps strategy

#### Defined in

https://github.com/babylon.js/core/src/Misc/PerformanceViewer/performanceViewerCollectionStrategies.ts:238

___

### ActiveBonesStrategy

▸ `Static` **ActiveBonesStrategy**(): [`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

Gets the initializer for the strategy used for collection of active bones metrics.

#### Returns

[`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

the initializer for the active bones strategy

#### Defined in

https://github.com/babylon.js/core/src/Misc/PerformanceViewer/performanceViewerCollectionStrategies.ts:128

___

### ActiveFacesStrategy

▸ `Static` **ActiveFacesStrategy**(): [`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

Gets the initializer for the strategy used for collection of active faces metrics.

#### Returns

[`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

the initializer for the active faces strategy

#### Defined in

https://github.com/babylon.js/core/src/Misc/PerformanceViewer/performanceViewerCollectionStrategies.ts:114

___

### ActiveIndicesStrategy

▸ `Static` **ActiveIndicesStrategy**(): [`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

Gets the initializer for the strategy used for collection of active indices metrics.

#### Returns

[`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

the initializer for the active indices strategy

#### Defined in

https://github.com/babylon.js/core/src/Misc/PerformanceViewer/performanceViewerCollectionStrategies.ts:100

___

### ActiveMeshesStrategy

▸ `Static` **ActiveMeshesStrategy**(): [`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

Gets the initializer for the strategy used for collection of active meshes metrics.

#### Returns

[`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

the initializer for the active meshes strategy

#### Defined in

https://github.com/babylon.js/core/src/Misc/PerformanceViewer/performanceViewerCollectionStrategies.ts:86

___

### ActiveParticlesStrategy

▸ `Static` **ActiveParticlesStrategy**(): [`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

Gets the initializer for the strategy used for collection of active particles metrics.

#### Returns

[`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

the initializer for the active particles strategy

#### Defined in

https://github.com/babylon.js/core/src/Misc/PerformanceViewer/performanceViewerCollectionStrategies.ts:142

___

### AnimationsStrategy

▸ `Static` **AnimationsStrategy**(): [`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

Gets the initializer for the strategy used for collection of animations time metrics.

#### Returns

[`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

the initializer for the animations time strategy

#### Defined in

https://github.com/babylon.js/core/src/Misc/PerformanceViewer/performanceViewerCollectionStrategies.ts:365

___

### CpuStrategy

▸ `Static` **CpuStrategy**(): [`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

Gets the initializer for the strategy used for collection of cpu utilization metrics.
Needs the experimental compute pressure API.

#### Returns

[`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

the initializer for the cpu utilization strategy

#### Defined in

https://github.com/babylon.js/core/src/Misc/PerformanceViewer/performanceViewerCollectionStrategies.ts:54

___

### DrawCallsStrategy

▸ `Static` **DrawCallsStrategy**(): [`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

Gets the initializer for the strategy used for collection of draw calls metrics.

#### Returns

[`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

the initializer for the draw calls strategy

#### Defined in

https://github.com/babylon.js/core/src/Misc/PerformanceViewer/performanceViewerCollectionStrategies.ts:156

___

### FpsStrategy

▸ `Static` **FpsStrategy**(): [`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

Gets the initializer for the strategy used for collection of fps metrics

#### Returns

[`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

the initializer for the fps strategy

#### Defined in

https://github.com/babylon.js/core/src/Misc/PerformanceViewer/performanceViewerCollectionStrategies.ts:38

___

### FrameTotalStrategy

▸ `Static` **FrameTotalStrategy**(): [`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

Gets the initializer for the strategy used for collection of total frame time metrics.

#### Returns

[`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

the initializer for the total frame time strategy

#### Defined in

https://github.com/babylon.js/core/src/Misc/PerformanceViewer/performanceViewerCollectionStrategies.ts:446

___

### GpuFrameTimeStrategy

▸ `Static` **GpuFrameTimeStrategy**(): [`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

Gets the initializer for the strategy used for collection of gpu frame time metrics.

#### Returns

[`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

the initializer for the gpu frame time strategy

#### Defined in

https://github.com/babylon.js/core/src/Misc/PerformanceViewer/performanceViewerCollectionStrategies.ts:501

___

### InterFrameStrategy

▸ `Static` **InterFrameStrategy**(): [`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

Gets the initializer for the strategy used for collection of inter-frame time metrics.

#### Returns

[`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

the initializer for the inter-frame time strategy

#### Defined in

https://github.com/babylon.js/core/src/Misc/PerformanceViewer/performanceViewerCollectionStrategies.ts:473

___

### MeshesSelectionStrategy

▸ `Static` **MeshesSelectionStrategy**(): [`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

Gets the initializer for the strategy used for collection of meshes selection time metrics.

#### Returns

[`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

the initializer for the meshes selection time strategy

#### Defined in

https://github.com/babylon.js/core/src/Misc/PerformanceViewer/performanceViewerCollectionStrategies.ts:257

___

### ParticlesStrategy

▸ `Static` **ParticlesStrategy**(): [`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

Gets the initializer for the strategy used for collection of particles time metrics.

#### Returns

[`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

the initializer for the particles time strategy

#### Defined in

https://github.com/babylon.js/core/src/Misc/PerformanceViewer/performanceViewerCollectionStrategies.ts:311

___

### PhysicsStrategy

▸ `Static` **PhysicsStrategy**(): [`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

Gets the initializer for the strategy used for collection of physics time metrics.

#### Returns

[`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

the initializer for the physics time strategy

#### Defined in

https://github.com/babylon.js/core/src/Misc/PerformanceViewer/performanceViewerCollectionStrategies.ts:392

___

### RenderStrategy

▸ `Static` **RenderStrategy**(): [`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

Gets the initializer for the strategy used for collection of render time metrics.

#### Returns

[`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

the initializer for the render time strategy

#### Defined in

https://github.com/babylon.js/core/src/Misc/PerformanceViewer/performanceViewerCollectionStrategies.ts:419

___

### RenderTargetsStrategy

▸ `Static` **RenderTargetsStrategy**(): [`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

Gets the initializer for the strategy used for collection of render targets time metrics.

#### Returns

[`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

the initializer for the render targets time strategy

#### Defined in

https://github.com/babylon.js/core/src/Misc/PerformanceViewer/performanceViewerCollectionStrategies.ts:284

___

### SpritesStrategy

▸ `Static` **SpritesStrategy**(): [`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

Gets the initializer for the strategy used for collection of sprites time metrics.

#### Returns

[`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

the initializer for the sprites time strategy

#### Defined in

https://github.com/babylon.js/core/src/Misc/PerformanceViewer/performanceViewerCollectionStrategies.ts:338

___

### TotalLightsStrategy

▸ `Static` **TotalLightsStrategy**(): [`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

Gets the initializer for the strategy used for collection of total lights metrics.

#### Returns

[`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

the initializer for the total lights strategy

#### Defined in

https://github.com/babylon.js/core/src/Misc/PerformanceViewer/performanceViewerCollectionStrategies.ts:182

___

### TotalMaterialsStrategy

▸ `Static` **TotalMaterialsStrategy**(): [`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

Gets the initializer for the strategy used for collection of total materials metrics.

#### Returns

[`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

the initializer for the total materials strategy

#### Defined in

https://github.com/babylon.js/core/src/Misc/PerformanceViewer/performanceViewerCollectionStrategies.ts:210

___

### TotalMeshesStrategy

▸ `Static` **TotalMeshesStrategy**(): [`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

Gets the initializer for the strategy used for collection of total meshes metrics.

#### Returns

[`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

the initializer for the total meshes strategy

#### Defined in

https://github.com/babylon.js/core/src/Misc/PerformanceViewer/performanceViewerCollectionStrategies.ts:72

___

### TotalTexturesStrategy

▸ `Static` **TotalTexturesStrategy**(): [`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

Gets the initializer for the strategy used for collection of total textures metrics.

#### Returns

[`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

the initializer for the total textures strategy

#### Defined in

https://github.com/babylon.js/core/src/Misc/PerformanceViewer/performanceViewerCollectionStrategies.ts:224

___

### TotalVerticesStrategy

▸ `Static` **TotalVerticesStrategy**(): [`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

Gets the initializer for the strategy used for collection of total vertices metrics.

#### Returns

[`PerfStrategyInitialization`](../modules.md#perfstrategyinitialization)

the initializer for the total vertices strategy

#### Defined in

https://github.com/babylon.js/core/src/Misc/PerformanceViewer/performanceViewerCollectionStrategies.ts:196
