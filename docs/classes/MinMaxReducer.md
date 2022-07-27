[@dev/core](../README.md) / [Exports](../modules.md) / MinMaxReducer

# Class: MinMaxReducer

This class computes a min/max reduction from a texture: it means it computes the minimum
and maximum values from all values of the texture.
It is performed on the GPU for better performances, thanks to a succession of post processes.
The source values are read from the red channel of the texture.

## Hierarchy

- **`MinMaxReducer`**

  ↳ [`DepthReducer`](DepthReducer.md)

## Table of contents

### Constructors

- [constructor](MinMaxReducer.md#constructor)

### Properties

- [\_activated](MinMaxReducer.md#_activated)
- [\_camera](MinMaxReducer.md#_camera)
- [\_forceFullscreenViewport](MinMaxReducer.md#_forcefullscreenviewport)
- [\_onAfterUnbindObserver](MinMaxReducer.md#_onafterunbindobserver)
- [\_onContextRestoredObserver](MinMaxReducer.md#_oncontextrestoredobserver)
- [\_postProcessManager](MinMaxReducer.md#_postprocessmanager)
- [\_reductionSteps](MinMaxReducer.md#_reductionsteps)
- [\_sourceTexture](MinMaxReducer.md#_sourcetexture)
- [onAfterReductionPerformed](MinMaxReducer.md#onafterreductionperformed)

### Accessors

- [activated](MinMaxReducer.md#activated)
- [refreshRate](MinMaxReducer.md#refreshrate)
- [sourceTexture](MinMaxReducer.md#sourcetexture)

### Methods

- [activate](MinMaxReducer.md#activate)
- [deactivate](MinMaxReducer.md#deactivate)
- [dispose](MinMaxReducer.md#dispose)
- [setSourceTexture](MinMaxReducer.md#setsourcetexture)

## Constructors

### constructor

• **new MinMaxReducer**(`camera`)

Creates a min/max reducer

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `camera` | [`Camera`](Camera.md) | The camera to use for the post processes |

#### Defined in

https://github.com/babylon.js/core/src/Misc/minMaxReducer.ts:39

## Properties

### \_activated

• `Protected` **\_activated**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Misc/minMaxReducer.ts:185

___

### \_camera

• `Protected` **\_camera**: [`Camera`](Camera.md)

#### Defined in

https://github.com/babylon.js/core/src/Misc/minMaxReducer.ts:27

___

### \_forceFullscreenViewport

• `Protected` **\_forceFullscreenViewport**: `boolean` = `true`

#### Defined in

https://github.com/babylon.js/core/src/Misc/minMaxReducer.ts:32

___

### \_onAfterUnbindObserver

• `Protected` **\_onAfterUnbindObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`RenderTargetTexture`](RenderTargetTexture.md)

#### Defined in

https://github.com/babylon.js/core/src/Misc/minMaxReducer.ts:31

___

### \_onContextRestoredObserver

• `Protected` **\_onContextRestoredObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`ThinEngine`](ThinEngine.md)

#### Defined in

https://github.com/babylon.js/core/src/Misc/minMaxReducer.ts:33

___

### \_postProcessManager

• `Protected` **\_postProcessManager**: [`PostProcessManager`](PostProcessManager.md)

#### Defined in

https://github.com/babylon.js/core/src/Misc/minMaxReducer.ts:30

___

### \_reductionSteps

• `Protected` **\_reductionSteps**: [`Nullable`](../modules.md#nullable)[`PostProcess`](PostProcess.md)[]

#### Defined in

https://github.com/babylon.js/core/src/Misc/minMaxReducer.ts:29

___

### \_sourceTexture

• `Protected` **\_sourceTexture**: [`Nullable`](../modules.md#nullable)[`RenderTargetTexture`](RenderTargetTexture.md)

#### Defined in

https://github.com/babylon.js/core/src/Misc/minMaxReducer.ts:28

___

### onAfterReductionPerformed

• **onAfterReductionPerformed**: [`Observable`](Observable.md){ `max`: `number` ; `min`: `number`  }

Observable triggered when the computation has been performed

#### Defined in

https://github.com/babylon.js/core/src/Misc/minMaxReducer.ts:25

## Accessors

### activated

• `get` **activated**(): `boolean`

Gets the activation status of the reducer

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Misc/minMaxReducer.ts:190

___

### refreshRate

• `get` **refreshRate**(): `number`

Defines the refresh rate of the computation.
Use 0 to compute just once, 1 to compute on every frame, 2 to compute every two frames and so on...

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Misc/minMaxReducer.ts:175

• `set` **refreshRate**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/minMaxReducer.ts:179

___

### sourceTexture

• `get` **sourceTexture**(): [`Nullable`](../modules.md#nullable)[`RenderTargetTexture`](RenderTargetTexture.md)

Gets the texture used to read the values from.

#### Returns

[`Nullable`](../modules.md#nullable)[`RenderTargetTexture`](RenderTargetTexture.md)

#### Defined in

https://github.com/babylon.js/core/src/Misc/minMaxReducer.ts:51

## Methods

### activate

▸ **activate**(): `void`

Activates the reduction computation.
When activated, the observers registered in onAfterReductionPerformed are
called after the computation is performed

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/minMaxReducer.ts:199

___

### deactivate

▸ **deactivate**(): `void`

Deactivates the reduction computation.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/minMaxReducer.ts:219

___

### dispose

▸ **dispose**(`disposeAll?`): `void`

Disposes the min/max reducer

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `disposeAll` | `boolean` | `true` | true to dispose all the resources. You should always call this function with true as the parameter (or without any parameter as it is the default one). This flag is meant to be used internally. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/minMaxReducer.ts:233

___

### setSourceTexture

▸ **setSourceTexture**(`sourceTexture`, `depthRedux`, `type?`, `forceFullscreenViewport?`): `void`

Sets the source texture to read the values from.
One must indicate if the texture is a depth texture or not through the depthRedux parameter
because in such textures '1' value must not be taken into account to compute the maximum
as this value is used to clear the texture.
Note that the computation is not activated by calling this function, you must call activate() for that!

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `sourceTexture` | [`RenderTargetTexture`](RenderTargetTexture.md) | `undefined` | The texture to read the values from. The values should be in the red channel. |
| `depthRedux` | `boolean` | `undefined` | Indicates if the texture is a depth texture or not |
| `type` | `number` | `Constants.TEXTURETYPE_HALF_FLOAT` | The type of the textures created for the reduction (defaults to TEXTURETYPE_HALF_FLOAT) |
| `forceFullscreenViewport` | `boolean` | `true` | Forces the post processes used for the reduction to be applied without taking into account viewport (defaults to true) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/minMaxReducer.ts:66
