[@dev/core](../README.md) / [Exports](../modules.md) / SceneInstrumentation

# Class: SceneInstrumentation

This class can be used to get instrumentation data from a Babylon engine

**`See`**

https://doc.babylonjs.com/how_to/optimizing_your_scene#sceneinstrumentation

## Implements

- [`IDisposable`](../interfaces/IDisposable.md)

## Table of contents

### Constructors

- [constructor](SceneInstrumentation.md#constructor)

### Properties

- [\_activeMeshesEvaluationTime](SceneInstrumentation.md#_activemeshesevaluationtime)
- [\_animationsTime](SceneInstrumentation.md#_animationstime)
- [\_cameraRenderTime](SceneInstrumentation.md#_camerarendertime)
- [\_captureActiveMeshesEvaluationTime](SceneInstrumentation.md#_captureactivemeshesevaluationtime)
- [\_captureAnimationsTime](SceneInstrumentation.md#_captureanimationstime)
- [\_captureCameraRenderTime](SceneInstrumentation.md#_capturecamerarendertime)
- [\_captureFrameTime](SceneInstrumentation.md#_captureframetime)
- [\_captureInterFrameTime](SceneInstrumentation.md#_captureinterframetime)
- [\_captureParticlesRenderTime](SceneInstrumentation.md#_captureparticlesrendertime)
- [\_capturePhysicsTime](SceneInstrumentation.md#_capturephysicstime)
- [\_captureRenderTargetsRenderTime](SceneInstrumentation.md#_capturerendertargetsrendertime)
- [\_captureRenderTime](SceneInstrumentation.md#_capturerendertime)
- [\_captureSpritesRenderTime](SceneInstrumentation.md#_capturespritesrendertime)
- [\_frameTime](SceneInstrumentation.md#_frametime)
- [\_interFrameTime](SceneInstrumentation.md#_interframetime)
- [\_onAfterActiveMeshesEvaluationObserver](SceneInstrumentation.md#_onafteractivemeshesevaluationobserver)
- [\_onAfterAnimationsObserver](SceneInstrumentation.md#_onafteranimationsobserver)
- [\_onAfterCameraRenderObserver](SceneInstrumentation.md#_onaftercamerarenderobserver)
- [\_onAfterDrawPhaseObserver](SceneInstrumentation.md#_onafterdrawphaseobserver)
- [\_onAfterParticlesRenderingObserver](SceneInstrumentation.md#_onafterparticlesrenderingobserver)
- [\_onAfterPhysicsObserver](SceneInstrumentation.md#_onafterphysicsobserver)
- [\_onAfterRenderObserver](SceneInstrumentation.md#_onafterrenderobserver)
- [\_onAfterRenderTargetsRenderObserver](SceneInstrumentation.md#_onafterrendertargetsrenderobserver)
- [\_onAfterSpritesRenderingObserver](SceneInstrumentation.md#_onafterspritesrenderingobserver)
- [\_onBeforeActiveMeshesEvaluationObserver](SceneInstrumentation.md#_onbeforeactivemeshesevaluationobserver)
- [\_onBeforeAnimationsObserver](SceneInstrumentation.md#_onbeforeanimationsobserver)
- [\_onBeforeCameraRenderObserver](SceneInstrumentation.md#_onbeforecamerarenderobserver)
- [\_onBeforeDrawPhaseObserver](SceneInstrumentation.md#_onbeforedrawphaseobserver)
- [\_onBeforeParticlesRenderingObserver](SceneInstrumentation.md#_onbeforeparticlesrenderingobserver)
- [\_onBeforePhysicsObserver](SceneInstrumentation.md#_onbeforephysicsobserver)
- [\_onBeforeRenderTargetsRenderObserver](SceneInstrumentation.md#_onbeforerendertargetsrenderobserver)
- [\_onBeforeSpritesRenderingObserver](SceneInstrumentation.md#_onbeforespritesrenderingobserver)
- [\_particlesRenderTime](SceneInstrumentation.md#_particlesrendertime)
- [\_physicsTime](SceneInstrumentation.md#_physicstime)
- [\_renderTargetsRenderTime](SceneInstrumentation.md#_rendertargetsrendertime)
- [\_renderTime](SceneInstrumentation.md#_rendertime)
- [\_spritesRenderTime](SceneInstrumentation.md#_spritesrendertime)
- [scene](SceneInstrumentation.md#scene)

### Accessors

- [activeMeshesEvaluationTimeCounter](SceneInstrumentation.md#activemeshesevaluationtimecounter)
- [animationsTimeCounter](SceneInstrumentation.md#animationstimecounter)
- [cameraRenderTimeCounter](SceneInstrumentation.md#camerarendertimecounter)
- [captureActiveMeshesEvaluationTime](SceneInstrumentation.md#captureactivemeshesevaluationtime)
- [captureAnimationsTime](SceneInstrumentation.md#captureanimationstime)
- [captureCameraRenderTime](SceneInstrumentation.md#capturecamerarendertime)
- [captureFrameTime](SceneInstrumentation.md#captureframetime)
- [captureInterFrameTime](SceneInstrumentation.md#captureinterframetime)
- [captureParticlesRenderTime](SceneInstrumentation.md#captureparticlesrendertime)
- [capturePhysicsTime](SceneInstrumentation.md#capturephysicstime)
- [captureRenderTargetsRenderTime](SceneInstrumentation.md#capturerendertargetsrendertime)
- [captureRenderTime](SceneInstrumentation.md#capturerendertime)
- [captureSpritesRenderTime](SceneInstrumentation.md#capturespritesrendertime)
- [drawCallsCounter](SceneInstrumentation.md#drawcallscounter)
- [frameTimeCounter](SceneInstrumentation.md#frametimecounter)
- [interFrameTimeCounter](SceneInstrumentation.md#interframetimecounter)
- [particlesRenderTimeCounter](SceneInstrumentation.md#particlesrendertimecounter)
- [physicsTimeCounter](SceneInstrumentation.md#physicstimecounter)
- [renderTargetsRenderTimeCounter](SceneInstrumentation.md#rendertargetsrendertimecounter)
- [renderTimeCounter](SceneInstrumentation.md#rendertimecounter)
- [spritesRenderTimeCounter](SceneInstrumentation.md#spritesrendertimecounter)

### Methods

- [dispose](SceneInstrumentation.md#dispose)

## Constructors

### constructor

• **new SceneInstrumentation**(`scene`)

Instantiates a new scene instrumentation.
This class can be used to get instrumentation data from a Babylon engine

**`See`**

https://doc.babylonjs.com/how_to/optimizing_your_scene#sceneinstrumentation

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | Defines the scene to instrument |

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:466

## Properties

### \_activeMeshesEvaluationTime

• `Private` **\_activeMeshesEvaluationTime**: [`PerfCounter`](PerfCounter.md)

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:13

___

### \_animationsTime

• `Private` **\_animationsTime**: [`PerfCounter`](PerfCounter.md)

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:37

___

### \_cameraRenderTime

• `Private` **\_cameraRenderTime**: [`PerfCounter`](PerfCounter.md)

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:40

___

### \_captureActiveMeshesEvaluationTime

• `Private` **\_captureActiveMeshesEvaluationTime**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:12

___

### \_captureAnimationsTime

• `Private` **\_captureAnimationsTime**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:36

___

### \_captureCameraRenderTime

• `Private` **\_captureCameraRenderTime**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:39

___

### \_captureFrameTime

• `Private` **\_captureFrameTime**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:18

___

### \_captureInterFrameTime

• `Private` **\_captureInterFrameTime**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:24

___

### \_captureParticlesRenderTime

• `Private` **\_captureParticlesRenderTime**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:27

___

### \_capturePhysicsTime

• `Private` **\_capturePhysicsTime**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:33

___

### \_captureRenderTargetsRenderTime

• `Private` **\_captureRenderTargetsRenderTime**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:15

___

### \_captureRenderTime

• `Private` **\_captureRenderTime**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:21

___

### \_captureSpritesRenderTime

• `Private` **\_captureSpritesRenderTime**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:30

___

### \_frameTime

• `Private` **\_frameTime**: [`PerfCounter`](PerfCounter.md)

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:19

___

### \_interFrameTime

• `Private` **\_interFrameTime**: [`PerfCounter`](PerfCounter.md)

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:25

___

### \_onAfterActiveMeshesEvaluationObserver

• `Private` **\_onAfterActiveMeshesEvaluationObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Scene`](Scene.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:44

___

### \_onAfterAnimationsObserver

• `Private` **\_onAfterAnimationsObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Scene`](Scene.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:64

___

### \_onAfterCameraRenderObserver

• `Private` **\_onAfterCameraRenderObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Camera`](Camera.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:67

___

### \_onAfterDrawPhaseObserver

• `Private` **\_onAfterDrawPhaseObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Scene`](Scene.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:51

___

### \_onAfterParticlesRenderingObserver

• `Private` **\_onAfterParticlesRenderingObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Scene`](Scene.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:56

___

### \_onAfterPhysicsObserver

• `Private` **\_onAfterPhysicsObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Scene`](Scene.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:62

___

### \_onAfterRenderObserver

• `Private` **\_onAfterRenderObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Scene`](Scene.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:48

___

### \_onAfterRenderTargetsRenderObserver

• `Private` **\_onAfterRenderTargetsRenderObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Scene`](Scene.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:46

___

### \_onAfterSpritesRenderingObserver

• `Private` **\_onAfterSpritesRenderingObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Scene`](Scene.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:59

___

### \_onBeforeActiveMeshesEvaluationObserver

• `Private` **\_onBeforeActiveMeshesEvaluationObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Scene`](Scene.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:43

___

### \_onBeforeAnimationsObserver

• `Private` **\_onBeforeAnimationsObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Scene`](Scene.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:53

___

### \_onBeforeCameraRenderObserver

• `Private` **\_onBeforeCameraRenderObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Camera`](Camera.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:66

___

### \_onBeforeDrawPhaseObserver

• `Private` **\_onBeforeDrawPhaseObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Scene`](Scene.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:50

___

### \_onBeforeParticlesRenderingObserver

• `Private` **\_onBeforeParticlesRenderingObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Scene`](Scene.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:55

___

### \_onBeforePhysicsObserver

• `Private` **\_onBeforePhysicsObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Scene`](Scene.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:61

___

### \_onBeforeRenderTargetsRenderObserver

• `Private` **\_onBeforeRenderTargetsRenderObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Scene`](Scene.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:45

___

### \_onBeforeSpritesRenderingObserver

• `Private` **\_onBeforeSpritesRenderingObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Scene`](Scene.md) = `null`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:58

___

### \_particlesRenderTime

• `Private` **\_particlesRenderTime**: [`PerfCounter`](PerfCounter.md)

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:28

___

### \_physicsTime

• `Private` **\_physicsTime**: [`PerfCounter`](PerfCounter.md)

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:34

___

### \_renderTargetsRenderTime

• `Private` **\_renderTargetsRenderTime**: [`PerfCounter`](PerfCounter.md)

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:16

___

### \_renderTime

• `Private` **\_renderTime**: [`PerfCounter`](PerfCounter.md)

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:22

___

### \_spritesRenderTime

• `Private` **\_spritesRenderTime**: [`PerfCounter`](PerfCounter.md)

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:31

___

### scene

• **scene**: [`Scene`](Scene.md)

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:470

## Accessors

### activeMeshesEvaluationTimeCounter

• `get` **activeMeshesEvaluationTimeCounter**(): [`PerfCounter`](PerfCounter.md)

Gets the perf counter used for active meshes evaluation time

#### Returns

[`PerfCounter`](PerfCounter.md)

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:73

___

### animationsTimeCounter

• `get` **animationsTimeCounter**(): [`PerfCounter`](PerfCounter.md)

Gets the perf counter used for animations time

#### Returns

[`PerfCounter`](PerfCounter.md)

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:296

___

### cameraRenderTimeCounter

• `get` **cameraRenderTimeCounter**(): [`PerfCounter`](PerfCounter.md)

Gets the perf counter used for camera render time capture

#### Returns

[`PerfCounter`](PerfCounter.md)

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:414

___

### captureActiveMeshesEvaluationTime

• `get` **captureActiveMeshesEvaluationTime**(): `boolean`

Gets the active meshes evaluation time capture status

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:80

• `set` **captureActiveMeshesEvaluationTime**(`value`): `void`

Enable or disable the active meshes evaluation time capture

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:87

___

### captureAnimationsTime

• `get` **captureAnimationsTime**(): `boolean`

Gets the animations time capture status

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:303

• `set` **captureAnimationsTime**(`value`): `void`

Enable or disable the animations time capture

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:310

___

### captureCameraRenderTime

• `get` **captureCameraRenderTime**(): `boolean`

Gets the camera render time capture status

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:421

• `set` **captureCameraRenderTime**(`value`): `void`

Enable or disable the camera render time capture

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:428

___

### captureFrameTime

• `get` **captureFrameTime**(): `boolean`

Gets the frame time capture status

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:337

• `set` **captureFrameTime**(`value`): `void`

Enable or disable the frame time capture

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:344

___

### captureInterFrameTime

• `get` **captureInterFrameTime**(): `boolean`

Gets the inter-frames time capture status

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:358

• `set` **captureInterFrameTime**(`value`): `void`

Enable or disable the inter-frames time capture

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:365

___

### captureParticlesRenderTime

• `get` **captureParticlesRenderTime**(): `boolean`

Gets the particles render time capture status

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:166

• `set` **captureParticlesRenderTime**(`value`): `void`

Enable or disable the particles render time capture

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:173

___

### capturePhysicsTime

• `get` **capturePhysicsTime**(): `boolean`

Gets the physics time capture status

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:256

• `set` **capturePhysicsTime**(`value`): `void`

Enable or disable the physics time capture

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:263

___

### captureRenderTargetsRenderTime

• `get` **captureRenderTargetsRenderTime**(): `boolean`

Gets the render targets render time capture status

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:123

• `set` **captureRenderTargetsRenderTime**(`value`): `void`

Enable or disable the render targets render time capture

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:130

___

### captureRenderTime

• `get` **captureRenderTime**(): `boolean`

Gets the render time capture status

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:379

• `set` **captureRenderTime**(`value`): `void`

Enable or disable the render time capture

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:386

___

### captureSpritesRenderTime

• `get` **captureSpritesRenderTime**(): `boolean`

Gets the sprites render time capture status

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:209

• `set` **captureSpritesRenderTime**(`value`): `void`

Enable or disable the sprites render time capture

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:216

___

### drawCallsCounter

• `get` **drawCallsCounter**(): [`PerfCounter`](PerfCounter.md)

Gets the perf counter used for draw calls

#### Returns

[`PerfCounter`](PerfCounter.md)

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:456

___

### frameTimeCounter

• `get` **frameTimeCounter**(): [`PerfCounter`](PerfCounter.md)

Gets the perf counter used for frame time capture

#### Returns

[`PerfCounter`](PerfCounter.md)

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:330

___

### interFrameTimeCounter

• `get` **interFrameTimeCounter**(): [`PerfCounter`](PerfCounter.md)

Gets the perf counter used for inter-frames time capture

#### Returns

[`PerfCounter`](PerfCounter.md)

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:351

___

### particlesRenderTimeCounter

• `get` **particlesRenderTimeCounter**(): [`PerfCounter`](PerfCounter.md)

Gets the perf counter used for particles render time

#### Returns

[`PerfCounter`](PerfCounter.md)

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:159

___

### physicsTimeCounter

• `get` **physicsTimeCounter**(): [`PerfCounter`](PerfCounter.md)

Gets the perf counter used for physics time

#### Returns

[`PerfCounter`](PerfCounter.md)

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:249

___

### renderTargetsRenderTimeCounter

• `get` **renderTargetsRenderTimeCounter**(): [`PerfCounter`](PerfCounter.md)

Gets the perf counter used for render targets render time

#### Returns

[`PerfCounter`](PerfCounter.md)

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:116

___

### renderTimeCounter

• `get` **renderTimeCounter**(): [`PerfCounter`](PerfCounter.md)

Gets the perf counter used for render time capture

#### Returns

[`PerfCounter`](PerfCounter.md)

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:372

___

### spritesRenderTimeCounter

• `get` **spritesRenderTimeCounter**(): [`PerfCounter`](PerfCounter.md)

Gets the perf counter used for sprites render time

#### Returns

[`PerfCounter`](PerfCounter.md)

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:202

## Methods

### dispose

▸ **dispose**(): `void`

Dispose and release associated resources.

#### Returns

`void`

#### Implementation of

[IDisposable](../interfaces/IDisposable.md).[dispose](../interfaces/IDisposable.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Instrumentation/sceneInstrumentation.ts:526
