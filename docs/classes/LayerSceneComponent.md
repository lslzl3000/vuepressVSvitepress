[@dev/core](../README.md) / [Exports](../modules.md) / LayerSceneComponent

# Class: LayerSceneComponent

Defines the layer scene component responsible to manage any layers
in a given scene.

## Implements

- [`ISceneComponent`](../interfaces/ISceneComponent.md)

## Table of contents

### Constructors

- [constructor](LayerSceneComponent.md#constructor)

### Properties

- [\_engine](LayerSceneComponent.md#_engine)
- [name](LayerSceneComponent.md#name)
- [scene](LayerSceneComponent.md#scene)

### Methods

- [\_draw](LayerSceneComponent.md#_draw)
- [\_drawCameraBackground](LayerSceneComponent.md#_drawcamerabackground)
- [\_drawCameraForeground](LayerSceneComponent.md#_drawcameraforeground)
- [\_drawCameraPredicate](LayerSceneComponent.md#_drawcamerapredicate)
- [\_drawRenderTargetBackground](LayerSceneComponent.md#_drawrendertargetbackground)
- [\_drawRenderTargetForeground](LayerSceneComponent.md#_drawrendertargetforeground)
- [\_drawRenderTargetPredicate](LayerSceneComponent.md#_drawrendertargetpredicate)
- [addFromContainer](LayerSceneComponent.md#addfromcontainer)
- [dispose](LayerSceneComponent.md#dispose)
- [rebuild](LayerSceneComponent.md#rebuild)
- [register](LayerSceneComponent.md#register)
- [removeFromContainer](LayerSceneComponent.md#removefromcontainer)

## Constructors

### constructor

• **new LayerSceneComponent**(`scene?`)

Creates a new instance of the component for the given scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene?` | [`Scene`](Scene.md) | Defines the scene to register the component in |

#### Defined in

https://github.com/babylon.js/core/src/Layers/layerSceneComponent.ts:41

## Properties

### \_engine

• `Private` **\_engine**: [`Engine`](Engine.md)

#### Defined in

https://github.com/babylon.js/core/src/Layers/layerSceneComponent.ts:35

___

### name

• `Readonly` **name**: ``"Layer"``

The component name helpful to identify the component in the list of scene components.

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[name](../interfaces/ISceneComponent.md#name)

#### Defined in

https://github.com/babylon.js/core/src/Layers/layerSceneComponent.ts:28

___

### scene

• **scene**: [`Scene`](Scene.md)

The scene the component belongs to.

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[scene](../interfaces/ISceneComponent.md#scene)

#### Defined in

https://github.com/babylon.js/core/src/Layers/layerSceneComponent.ts:33

## Methods

### \_draw

▸ `Private` **_draw**(`predicate`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `predicate` | (`layer`: [`Layer`](Layer.md)) => `boolean` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Layers/layerSceneComponent.ts:84

___

### \_drawCameraBackground

▸ `Private` **_drawCameraBackground**(`camera`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `camera` | [`Camera`](Camera.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Layers/layerSceneComponent.ts:102

___

### \_drawCameraForeground

▸ `Private` **_drawCameraForeground**(`camera`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `camera` | [`Camera`](Camera.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Layers/layerSceneComponent.ts:108

___

### \_drawCameraPredicate

▸ `Private` **_drawCameraPredicate**(`layer`, `isBackground`, `cameraLayerMask`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `layer` | [`Layer`](Layer.md) |
| `isBackground` | `boolean` |
| `cameraLayerMask` | `number` |

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Layers/layerSceneComponent.ts:98

___

### \_drawRenderTargetBackground

▸ `Private` **_drawRenderTargetBackground**(`renderTarget`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `renderTarget` | [`RenderTargetTexture`](RenderTargetTexture.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Layers/layerSceneComponent.ts:123

___

### \_drawRenderTargetForeground

▸ `Private` **_drawRenderTargetForeground**(`renderTarget`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `renderTarget` | [`RenderTargetTexture`](RenderTargetTexture.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Layers/layerSceneComponent.ts:129

___

### \_drawRenderTargetPredicate

▸ `Private` **_drawRenderTargetPredicate**(`layer`, `isBackground`, `cameraLayerMask`, `renderTargetTexture`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `layer` | [`Layer`](Layer.md) |
| `isBackground` | `boolean` |
| `cameraLayerMask` | `number` |
| `renderTargetTexture` | [`RenderTargetTexture`](RenderTargetTexture.md) |

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Layers/layerSceneComponent.ts:114

___

### addFromContainer

▸ **addFromContainer**(`container`): `void`

Adds all the elements from the container to the scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `container` | [`AbstractScene`](AbstractScene.md) | the container holding the elements |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Layers/layerSceneComponent.ts:139

___

### dispose

▸ **dispose**(): `void`

Disposes the component and the associated resources.

#### Returns

`void`

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[dispose](../interfaces/ISceneComponent.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Layers/layerSceneComponent.ts:76

___

### rebuild

▸ **rebuild**(): `void`

Rebuilds the elements related to this component in case of
context lost for instance.

#### Returns

`void`

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[rebuild](../interfaces/ISceneComponent.md#rebuild)

#### Defined in

https://github.com/babylon.js/core/src/Layers/layerSceneComponent.ts:65

___

### register

▸ **register**(): `void`

Registers the component in a given scene

#### Returns

`void`

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[register](../interfaces/ISceneComponent.md#register)

#### Defined in

https://github.com/babylon.js/core/src/Layers/layerSceneComponent.ts:53

___

### removeFromContainer

▸ **removeFromContainer**(`container`, `dispose?`): `void`

Removes all the elements in the container from the scene

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `container` | [`AbstractScene`](AbstractScene.md) | `undefined` | contains the elements to remove |
| `dispose` | `boolean` | `false` | if the removed element should be disposed (default: false) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Layers/layerSceneComponent.ts:153
