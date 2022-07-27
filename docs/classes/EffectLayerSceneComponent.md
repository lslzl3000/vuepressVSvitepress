[@dev/core](../README.md) / [Exports](../modules.md) / EffectLayerSceneComponent

# Class: EffectLayerSceneComponent

Defines the layer scene component responsible to manage any effect layers
in a given scene.

## Implements

- [`ISceneSerializableComponent`](../interfaces/ISceneSerializableComponent.md)

## Table of contents

### Constructors

- [constructor](EffectLayerSceneComponent.md#constructor)

### Properties

- [\_engine](EffectLayerSceneComponent.md#_engine)
- [\_needStencil](EffectLayerSceneComponent.md#_needstencil)
- [\_previousStencilState](EffectLayerSceneComponent.md#_previousstencilstate)
- [\_renderEffects](EffectLayerSceneComponent.md#_rendereffects)
- [name](EffectLayerSceneComponent.md#name)
- [scene](EffectLayerSceneComponent.md#scene)

### Methods

- [\_draw](EffectLayerSceneComponent.md#_draw)
- [\_drawCamera](EffectLayerSceneComponent.md#_drawcamera)
- [\_drawRenderingGroup](EffectLayerSceneComponent.md#_drawrenderinggroup)
- [\_isReadyForMesh](EffectLayerSceneComponent.md#_isreadyformesh)
- [\_renderMainTexture](EffectLayerSceneComponent.md#_rendermaintexture)
- [\_setStencil](EffectLayerSceneComponent.md#_setstencil)
- [\_setStencilBack](EffectLayerSceneComponent.md#_setstencilback)
- [addFromContainer](EffectLayerSceneComponent.md#addfromcontainer)
- [dispose](EffectLayerSceneComponent.md#dispose)
- [rebuild](EffectLayerSceneComponent.md#rebuild)
- [register](EffectLayerSceneComponent.md#register)
- [removeFromContainer](EffectLayerSceneComponent.md#removefromcontainer)
- [serialize](EffectLayerSceneComponent.md#serialize)

## Constructors

### constructor

• **new EffectLayerSceneComponent**(`scene?`)

Creates a new instance of the component for the given scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene?` | [`Scene`](Scene.md) | Defines the scene to register the component in |

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayerSceneComponent.ts:87

## Properties

### \_engine

• `Private` **\_engine**: [`Engine`](Engine.md)

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayerSceneComponent.ts:78

___

### \_needStencil

• `Private` **\_needStencil**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayerSceneComponent.ts:80

___

### \_previousStencilState

• `Private` **\_previousStencilState**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayerSceneComponent.ts:81

___

### \_renderEffects

• `Private` **\_renderEffects**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayerSceneComponent.ts:79

___

### name

• `Readonly` **name**: ``"EffectLayer"``

The component name helpful to identify the component in the list of scene components.

#### Implementation of

[ISceneSerializableComponent](../interfaces/ISceneSerializableComponent.md).[name](../interfaces/ISceneSerializableComponent.md#name)

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayerSceneComponent.ts:71

___

### scene

• **scene**: [`Scene`](Scene.md)

The scene the component belongs to.

#### Implementation of

[ISceneSerializableComponent](../interfaces/ISceneSerializableComponent.md).[scene](../interfaces/ISceneSerializableComponent.md#scene)

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayerSceneComponent.ts:76

## Methods

### \_draw

▸ `Private` **_draw**(`renderingGroupId`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `renderingGroupId` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayerSceneComponent.ts:249

___

### \_drawCamera

▸ `Private` **_drawCamera**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayerSceneComponent.ts:266

___

### \_drawRenderingGroup

▸ `Private` **_drawRenderingGroup**(`index`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `index` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayerSceneComponent.ts:271

___

### \_isReadyForMesh

▸ `Private` **_isReadyForMesh**(`mesh`, `hardwareInstancedRendering`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `mesh` | [`AbstractMesh`](AbstractMesh.md) |
| `hardwareInstancedRendering` | `boolean` |

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayerSceneComponent.ts:179

___

### \_renderMainTexture

▸ `Private` **_renderMainTexture**(`camera`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `camera` | [`Camera`](Camera.md) |

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayerSceneComponent.ts:201

___

### \_setStencil

▸ `Private` **_setStencil**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayerSceneComponent.ts:235

___

### \_setStencilBack

▸ `Private` **_setStencilBack**(): `void`

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayerSceneComponent.ts:242

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

#### Implementation of

[ISceneSerializableComponent](../interfaces/ISceneSerializableComponent.md).[addFromContainer](../interfaces/ISceneSerializableComponent.md#addfromcontainer)

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayerSceneComponent.ts:143

___

### dispose

▸ **dispose**(): `void`

Disposes the component and the associated resources.

#### Returns

`void`

#### Implementation of

[ISceneSerializableComponent](../interfaces/ISceneSerializableComponent.md).[dispose](../interfaces/ISceneSerializableComponent.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayerSceneComponent.ts:172

___

### rebuild

▸ **rebuild**(): `void`

Rebuilds the elements related to this component in case of
context lost for instance.

#### Returns

`void`

#### Implementation of

[ISceneSerializableComponent](../interfaces/ISceneSerializableComponent.md).[rebuild](../interfaces/ISceneSerializableComponent.md#rebuild)

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayerSceneComponent.ts:116

___

### register

▸ **register**(): `void`

Registers the component in a given scene

#### Returns

`void`

#### Implementation of

[ISceneSerializableComponent](../interfaces/ISceneSerializableComponent.md).[register](../interfaces/ISceneSerializableComponent.md#register)

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayerSceneComponent.ts:99

___

### removeFromContainer

▸ **removeFromContainer**(`container`, `dispose?`): `void`

Removes all the elements in the container from the scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `container` | [`AbstractScene`](AbstractScene.md) | contains the elements to remove |
| `dispose?` | `boolean` | if the removed element should be disposed (default: false) |

#### Returns

`void`

#### Implementation of

[ISceneSerializableComponent](../interfaces/ISceneSerializableComponent.md).[removeFromContainer](../interfaces/ISceneSerializableComponent.md#removefromcontainer)

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayerSceneComponent.ts:157

___

### serialize

▸ **serialize**(`serializationObject`): `void`

Serializes the component data to the specified json object

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `serializationObject` | `any` | The object to serialize to |

#### Returns

`void`

#### Implementation of

[ISceneSerializableComponent](../interfaces/ISceneSerializableComponent.md).[serialize](../interfaces/ISceneSerializableComponent.md#serialize)

#### Defined in

https://github.com/babylon.js/core/src/Layers/effectLayerSceneComponent.ts:127
