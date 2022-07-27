[@dev/core](../README.md) / [Exports](../modules.md) / DepthReducer

# Class: DepthReducer

This class is a small wrapper around the MinMaxReducer class to compute the min/max values of a depth texture

## Hierarchy

- [`MinMaxReducer`](MinMaxReducer.md)

  ↳ **`DepthReducer`**

## Table of contents

### Constructors

- [constructor](DepthReducer.md#constructor)

### Properties

- [\_activated](DepthReducer.md#_activated)
- [\_camera](DepthReducer.md#_camera)
- [\_depthRenderer](DepthReducer.md#_depthrenderer)
- [\_depthRendererId](DepthReducer.md#_depthrendererid)
- [\_forceFullscreenViewport](DepthReducer.md#_forcefullscreenviewport)
- [\_onAfterUnbindObserver](DepthReducer.md#_onafterunbindobserver)
- [\_onContextRestoredObserver](DepthReducer.md#_oncontextrestoredobserver)
- [\_postProcessManager](DepthReducer.md#_postprocessmanager)
- [\_reductionSteps](DepthReducer.md#_reductionsteps)
- [\_sourceTexture](DepthReducer.md#_sourcetexture)
- [onAfterReductionPerformed](DepthReducer.md#onafterreductionperformed)

### Accessors

- [activated](DepthReducer.md#activated)
- [depthRenderer](DepthReducer.md#depthrenderer)
- [refreshRate](DepthReducer.md#refreshrate)
- [sourceTexture](DepthReducer.md#sourcetexture)

### Methods

- [activate](DepthReducer.md#activate)
- [deactivate](DepthReducer.md#deactivate)
- [dispose](DepthReducer.md#dispose)
- [setDepthRenderer](DepthReducer.md#setdepthrenderer)

## Constructors

### constructor

• **new DepthReducer**(`camera`)

Creates a depth reducer

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `camera` | [`Camera`](Camera.md) | The camera used to render the depth texture |

#### Overrides

[MinMaxReducer](MinMaxReducer.md).[constructor](MinMaxReducer.md#constructor)

#### Defined in

packages/dev/core/src/Misc/depthReducer.ts:28

## Properties

### \_activated

• `Protected` **\_activated**: `boolean` = `false`

#### Inherited from

[MinMaxReducer](MinMaxReducer.md).[_activated](MinMaxReducer.md#_activated)

#### Defined in

packages/dev/core/src/Misc/minMaxReducer.ts:185

___

### \_camera

• `Protected` **\_camera**: [`Camera`](Camera.md)

#### Inherited from

[MinMaxReducer](MinMaxReducer.md).[_camera](MinMaxReducer.md#_camera)

#### Defined in

packages/dev/core/src/Misc/minMaxReducer.ts:27

___

### \_depthRenderer

• `Private` **\_depthRenderer**: [`Nullable`](../modules.md#nullable)[`DepthRenderer`](DepthRenderer.md)

#### Defined in

packages/dev/core/src/Misc/depthReducer.ts:13

___

### \_depthRendererId

• `Private` **\_depthRendererId**: `string`

#### Defined in

packages/dev/core/src/Misc/depthReducer.ts:14

___

### \_forceFullscreenViewport

• `Protected` **\_forceFullscreenViewport**: `boolean` = `true`

#### Inherited from

[MinMaxReducer](MinMaxReducer.md).[_forceFullscreenViewport](MinMaxReducer.md#_forcefullscreenviewport)

#### Defined in

packages/dev/core/src/Misc/minMaxReducer.ts:32

___

### \_onAfterUnbindObserver

• `Protected` **\_onAfterUnbindObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`RenderTargetTexture`](RenderTargetTexture.md)

#### Inherited from

[MinMaxReducer](MinMaxReducer.md).[_onAfterUnbindObserver](MinMaxReducer.md#_onafterunbindobserver)

#### Defined in

packages/dev/core/src/Misc/minMaxReducer.ts:31

___

### \_onContextRestoredObserver

• `Protected` **\_onContextRestoredObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`ThinEngine`](ThinEngine.md)

#### Inherited from

[MinMaxReducer](MinMaxReducer.md).[_onContextRestoredObserver](MinMaxReducer.md#_oncontextrestoredobserver)

#### Defined in

packages/dev/core/src/Misc/minMaxReducer.ts:33

___

### \_postProcessManager

• `Protected` **\_postProcessManager**: [`PostProcessManager`](PostProcessManager.md)

#### Inherited from

[MinMaxReducer](MinMaxReducer.md).[_postProcessManager](MinMaxReducer.md#_postprocessmanager)

#### Defined in

packages/dev/core/src/Misc/minMaxReducer.ts:30

___

### \_reductionSteps

• `Protected` **\_reductionSteps**: [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)[]

#### Inherited from

[MinMaxReducer](MinMaxReducer.md).[_reductionSteps](MinMaxReducer.md#_reductionsteps)

#### Defined in

packages/dev/core/src/Misc/minMaxReducer.ts:29

___

### \_sourceTexture

• `Protected` **\_sourceTexture**: [`Nullable`](../modules.md#nullable)[`RenderTargetTexture`](RenderTargetTexture.md)

#### Inherited from

[MinMaxReducer](MinMaxReducer.md).[_sourceTexture](MinMaxReducer.md#_sourcetexture)

#### Defined in

packages/dev/core/src/Misc/minMaxReducer.ts:28

___

### onAfterReductionPerformed

• **onAfterReductionPerformed**: [`Observable`](Observable.md){ `max`: `number` ; `min`: `number`  }

Observable triggered when the computation has been performed

#### Inherited from

[MinMaxReducer](MinMaxReducer.md).[onAfterReductionPerformed](MinMaxReducer.md#onafterreductionperformed)

#### Defined in

packages/dev/core/src/Misc/minMaxReducer.ts:25

## Accessors

### activated

• `get` **activated**(): `boolean`

Gets the activation status of the reducer

#### Returns

`boolean`

#### Inherited from

MinMaxReducer.activated

#### Defined in

packages/dev/core/src/Misc/minMaxReducer.ts:190

___

### depthRenderer

• `get` **depthRenderer**(): [`Nullable`](../modules.md#nullable)[`DepthRenderer`](DepthRenderer.md)

Gets the depth renderer used for the computation.
Note that the result is null if you provide your own renderer when calling setDepthRenderer.

#### Returns

[`Nullable`](../modules.md#nullable)[`DepthRenderer`](DepthRenderer.md)

#### Defined in

packages/dev/core/src/Misc/depthReducer.ts:20

___

### refreshRate

• `get` **refreshRate**(): `number`

Defines the refresh rate of the computation.
Use 0 to compute just once, 1 to compute on every frame, 2 to compute every two frames and so on...

#### Returns

`number`

#### Inherited from

MinMaxReducer.refreshRate

#### Defined in

packages/dev/core/src/Misc/minMaxReducer.ts:175

• `set` **refreshRate**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

MinMaxReducer.refreshRate

#### Defined in

packages/dev/core/src/Misc/minMaxReducer.ts:179

___

### sourceTexture

• `get` **sourceTexture**(): [`Nullable`](../modules.md#nullable)[`RenderTargetTexture`](RenderTargetTexture.md)

Gets the texture used to read the values from.

#### Returns

[`Nullable`](../modules.md#nullable)[`RenderTargetTexture`](RenderTargetTexture.md)

#### Inherited from

MinMaxReducer.sourceTexture

#### Defined in

packages/dev/core/src/Misc/minMaxReducer.ts:51

## Methods

### activate

▸ **activate**(): `void`

Activates the reduction computation.
When activated, the observers registered in onAfterReductionPerformed are
called after the computation is performed

#### Returns

`void`

#### Overrides

[MinMaxReducer](MinMaxReducer.md).[activate](MinMaxReducer.md#activate)

#### Defined in

packages/dev/core/src/Misc/depthReducer.ts:79

___

### deactivate

▸ **deactivate**(): `void`

Deactivates the reduction computation.

#### Returns

`void`

#### Overrides

[MinMaxReducer](MinMaxReducer.md).[deactivate](MinMaxReducer.md#deactivate)

#### Defined in

packages/dev/core/src/Misc/depthReducer.ts:90

___

### dispose

▸ **dispose**(`disposeAll?`): `void`

Disposes the depth reducer

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `disposeAll` | `boolean` | `true` | true to dispose all the resources. You should always call this function with true as the parameter (or without any parameter as it is the default one). This flag is meant to be used internally. |

#### Returns

`void`

#### Overrides

[MinMaxReducer](MinMaxReducer.md).[dispose](MinMaxReducer.md#dispose)

#### Defined in

packages/dev/core/src/Misc/depthReducer.ts:102

___

### setDepthRenderer

▸ **setDepthRenderer**(`depthRenderer?`, `type?`, `forceFullscreenViewport?`): `void`

Sets the depth renderer to use to generate the depth map

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `depthRenderer` | [`Nullable`](../modules.md#nullable)[`DepthRenderer`](DepthRenderer.md) | `null` | The depth renderer to use. If not provided, a new one will be created automatically |
| `type` | `number` | `Constants.TEXTURETYPE_HALF_FLOAT` | The texture type of the depth map (default: TEXTURETYPE_HALF_FLOAT) |
| `forceFullscreenViewport` | `boolean` | `true` | Forces the post processes used for the reduction to be applied without taking into account viewport (defaults to true) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/depthReducer.ts:38
