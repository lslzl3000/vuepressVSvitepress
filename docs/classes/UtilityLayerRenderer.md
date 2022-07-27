[@dev/core](../README.md) / [Exports](../modules.md) / UtilityLayerRenderer

# Class: UtilityLayerRenderer

Renders a layer on top of an existing scene

## Implements

- [`IDisposable`](../interfaces/IDisposable.md)

## Table of contents

### Constructors

- [constructor](UtilityLayerRenderer.md#constructor)

### Properties

- [\_afterRenderObserver](UtilityLayerRenderer.md#_afterrenderobserver)
- [\_lastPointerEvents](UtilityLayerRenderer.md#_lastpointerevents)
- [\_originalPointerObserver](UtilityLayerRenderer.md#_originalpointerobserver)
- [\_pointerCaptures](UtilityLayerRenderer.md#_pointercaptures)
- [\_renderCamera](UtilityLayerRenderer.md#_rendercamera)
- [\_sceneDisposeObserver](UtilityLayerRenderer.md#_scenedisposeobserver)
- [\_sharedGizmoLight](UtilityLayerRenderer.md#_sharedgizmolight)
- [mainSceneTrackerPredicate](UtilityLayerRenderer.md#mainscenetrackerpredicate)
- [onPointerOutObservable](UtilityLayerRenderer.md#onpointeroutobservable)
- [onlyCheckPointerDownEvents](UtilityLayerRenderer.md#onlycheckpointerdownevents)
- [originalScene](UtilityLayerRenderer.md#originalscene)
- [pickUtilitySceneFirst](UtilityLayerRenderer.md#pickutilityscenefirst)
- [pickingEnabled](UtilityLayerRenderer.md#pickingenabled)
- [processAllEvents](UtilityLayerRenderer.md#processallevents)
- [shouldRender](UtilityLayerRenderer.md#shouldrender)
- [utilityLayerScene](UtilityLayerRenderer.md#utilitylayerscene)

### Accessors

- [DefaultKeepDepthUtilityLayer](UtilityLayerRenderer.md#defaultkeepdepthutilitylayer)
- [DefaultUtilityLayer](UtilityLayerRenderer.md#defaultutilitylayer)

### Methods

- [\_notifyObservers](UtilityLayerRenderer.md#_notifyobservers)
- [\_updateCamera](UtilityLayerRenderer.md#_updatecamera)
- [dispose](UtilityLayerRenderer.md#dispose)
- [getRenderCamera](UtilityLayerRenderer.md#getrendercamera)
- [render](UtilityLayerRenderer.md#render)
- [setRenderCamera](UtilityLayerRenderer.md#setrendercamera)

## Constructors

### constructor

• **new UtilityLayerRenderer**(`originalScene`, `handleEvents?`)

Instantiates a UtilityLayerRenderer

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `originalScene` | [`Scene`](Scene.md) | `undefined` | the original scene that will be rendered on top of |
| `handleEvents` | `boolean` | `true` | boolean indicating if the utility layer should handle events |

#### Defined in

packages/dev/core/src/Rendering/utilityLayerRenderer.ts:156

## Properties

### \_afterRenderObserver

• `Private` **\_afterRenderObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Camera`](Camera.md)

#### Defined in

packages/dev/core/src/Rendering/utilityLayerRenderer.ts:148

___

### \_lastPointerEvents

• `Private` **\_lastPointerEvents**: `Object` = `{}`

#### Index signature

▪ [pointerId: `number`]: `boolean`

#### Defined in

packages/dev/core/src/Rendering/utilityLayerRenderer.ts:22

___

### \_originalPointerObserver

• `Private` **\_originalPointerObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`PointerInfoPre`](PointerInfoPre.md)

#### Defined in

packages/dev/core/src/Rendering/utilityLayerRenderer.ts:150

___

### \_pointerCaptures

• `Private` **\_pointerCaptures**: `Object` = `{}`

#### Index signature

▪ [pointerId: `number`]: `boolean`

#### Defined in

packages/dev/core/src/Rendering/utilityLayerRenderer.ts:21

___

### \_renderCamera

• `Private` **\_renderCamera**: [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md) = `null`

#### Defined in

packages/dev/core/src/Rendering/utilityLayerRenderer.ts:29

___

### \_sceneDisposeObserver

• `Private` **\_sceneDisposeObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/Rendering/utilityLayerRenderer.ts:149

___

### \_sharedGizmoLight

• `Private` **\_sharedGizmoLight**: [`Nullable`](../modules.md#nullable)[`HemisphericLight`](HemisphericLight.md) = `null`

#### Defined in

packages/dev/core/src/Rendering/utilityLayerRenderer.ts:27

___

### mainSceneTrackerPredicate

• **mainSceneTrackerPredicate**: (`mesh`: [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)) => `boolean`

#### Type declaration

▸ (`mesh`): `boolean`

Gets or sets a predicate that will be used to indicate utility meshes present in the main scene

##### Parameters

| Name | Type |
| :------ | :------ |
| `mesh` | [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md) |

##### Returns

`boolean`

#### Defined in

packages/dev/core/src/Rendering/utilityLayerRenderer.ts:146

___

### onPointerOutObservable

• **onPointerOutObservable**: [`Observable`](Observable.md)`number`

Observable raised when the pointer moves from the utility layer scene to the main scene

#### Defined in

packages/dev/core/src/Rendering/utilityLayerRenderer.ts:143

___

### onlyCheckPointerDownEvents

• **onlyCheckPointerDownEvents**: `boolean` = `true`

If set to true, only pointer down onPointerObservable events will be blocked when picking is occluded by original scene

#### Defined in

packages/dev/core/src/Rendering/utilityLayerRenderer.ts:128

___

### originalScene

• **originalScene**: [`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/Rendering/utilityLayerRenderer.ts:158

___

### pickUtilitySceneFirst

• **pickUtilitySceneFirst**: `boolean` = `true`

If the picking should be done on the utility layer prior to the actual scene (Default: true)

#### Defined in

packages/dev/core/src/Rendering/utilityLayerRenderer.ts:77

___

### pickingEnabled

• **pickingEnabled**: `boolean` = `true`

Set to false to disable picking

#### Defined in

packages/dev/core/src/Rendering/utilityLayerRenderer.ts:138

___

### processAllEvents

• **processAllEvents**: `boolean` = `false`

If set to false, only pointerUp, pointerDown and pointerMove will be sent to the utilityLayerScene (false by default)

#### Defined in

packages/dev/core/src/Rendering/utilityLayerRenderer.ts:133

___

### shouldRender

• **shouldRender**: `boolean` = `true`

If the utility layer should automatically be rendered on top of existing scene

#### Defined in

packages/dev/core/src/Rendering/utilityLayerRenderer.ts:124

___

### utilityLayerScene

• **utilityLayerScene**: [`Scene`](Scene.md)

The scene that is rendered on top of the original scene

#### Defined in

packages/dev/core/src/Rendering/utilityLayerRenderer.ts:119

## Accessors

### DefaultKeepDepthUtilityLayer

• `Static` `get` **DefaultKeepDepthUtilityLayer**(): [`UtilityLayerRenderer`](UtilityLayerRenderer.md)

A shared utility layer that can be used to embed objects into a scene (Depth map of the previous scene is not cleared before drawing on top of it)

#### Returns

[`UtilityLayerRenderer`](UtilityLayerRenderer.md)

#### Defined in

packages/dev/core/src/Rendering/utilityLayerRenderer.ts:105

___

### DefaultUtilityLayer

• `Static` `get` **DefaultUtilityLayer**(): [`UtilityLayerRenderer`](UtilityLayerRenderer.md)

A shared utility layer that can be used to overlay objects into a scene (Depth map of the previous scene is cleared before drawing on top of it)

#### Returns

[`UtilityLayerRenderer`](UtilityLayerRenderer.md)

#### Defined in

packages/dev/core/src/Rendering/utilityLayerRenderer.ts:81

## Methods

### \_notifyObservers

▸ `Private` **_notifyObservers**(`prePointerInfo`, `pickInfo`, `pointerEvent`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `prePointerInfo` | [`PointerInfoPre`](PointerInfoPre.md) |
| `pickInfo` | [`PickingInfo`](PickingInfo.md) |
| `pointerEvent` | [`IPointerEvent`](../interfaces/IPointerEvent.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Rendering/utilityLayerRenderer.ts:340

___

### \_updateCamera

▸ `Private` **_updateCamera**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Rendering/utilityLayerRenderer.ts:395

___

### dispose

▸ **dispose**(): `void`

Disposes of the renderer

#### Returns

`void`

#### Implementation of

[IDisposable](../interfaces/IDisposable.md).[dispose](../interfaces/IDisposable.md#dispose)

#### Defined in

packages/dev/core/src/Rendering/utilityLayerRenderer.ts:380

___

### getRenderCamera

▸ **getRenderCamera**(`getRigParentIfPossible?`): [`Camera`](Camera.md)

Gets the camera that is used to render the utility layer (when not set, this will be the last active camera)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `getRigParentIfPossible?` | `boolean` | if the current active camera is a rig camera, should its parent camera be returned |

#### Returns

[`Camera`](Camera.md)

the camera that is used when rendering the utility layer

#### Defined in

packages/dev/core/src/Rendering/utilityLayerRenderer.ts:36

___

### render

▸ **render**(): `void`

Renders the utility layers scene on top of the original scene

#### Returns

`void`

#### Defined in

packages/dev/core/src/Rendering/utilityLayerRenderer.ts:350

___

### setRenderCamera

▸ **setRenderCamera**(`cam`): `void`

Sets the camera that should be used when rendering the utility layer (If set to null the last active camera will be used)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `cam` | [`Nullable`](../modules.md#nullable)[`Camera`](Camera.md) | the camera that should be used when rendering the utility layer |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Rendering/utilityLayerRenderer.ts:57
