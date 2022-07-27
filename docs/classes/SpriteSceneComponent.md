[@dev/core](../README.md) / [Exports](../modules.md) / SpriteSceneComponent

# Class: SpriteSceneComponent

Defines the sprite scene component responsible to manage sprites
in a given scene.

## Implements

- [`ISceneComponent`](../interfaces/ISceneComponent.md)

## Table of contents

### Constructors

- [constructor](SpriteSceneComponent.md#constructor)

### Properties

- [name](SpriteSceneComponent.md#name)
- [scene](SpriteSceneComponent.md#scene)

### Methods

- [\_pickSpriteButKeepRay](SpriteSceneComponent.md#_pickspritebutkeepray)
- [\_pointerDown](SpriteSceneComponent.md#_pointerdown)
- [\_pointerMove](SpriteSceneComponent.md#_pointermove)
- [\_pointerUp](SpriteSceneComponent.md#_pointerup)
- [dispose](SpriteSceneComponent.md#dispose)
- [rebuild](SpriteSceneComponent.md#rebuild)
- [register](SpriteSceneComponent.md#register)

## Constructors

### constructor

• **new SpriteSceneComponent**(`scene`)

Creates a new instance of the component for the given scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | Defines the scene to register the component in |

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteSceneComponent.ts:276

## Properties

### name

• `Readonly` **name**: ``"Sprite"``

The component name helpfull to identify the component in the list of scene components.

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[name](../interfaces/ISceneComponent.md#name)

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteSceneComponent.ts:262

___

### scene

• **scene**: [`Scene`](Scene.md)

The scene the component belongs to.

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[scene](../interfaces/ISceneComponent.md#scene)

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteSceneComponent.ts:267

## Methods

### \_pickSpriteButKeepRay

▸ `Private` **_pickSpriteButKeepRay**(`originalPointerInfo`, `x`, `y`, `fastCheck?`, `camera?`): [`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `originalPointerInfo` | [`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md) |
| `x` | `number` |
| `y` | `number` |
| `fastCheck?` | `boolean` |
| `camera?` | [`Camera`](Camera.md) |

#### Returns

[`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md)

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteSceneComponent.ts:320

___

### \_pointerDown

▸ `Private` **_pointerDown**(`unTranslatedPointerX`, `unTranslatedPointerY`, `pickResult`, `evt`): [`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `unTranslatedPointerX` | `number` |
| `unTranslatedPointerY` | `number` |
| `pickResult` | [`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md) |
| `evt` | [`IPointerEvent`](../interfaces/IPointerEvent.md) |

#### Returns

[`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md)

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteSceneComponent.ts:358

___

### \_pointerMove

▸ `Private` **_pointerMove**(`unTranslatedPointerX`, `unTranslatedPointerY`, `pickResult`, `isMeshPicked`, `element`): [`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `unTranslatedPointerX` | `number` |
| `unTranslatedPointerY` | `number` |
| `pickResult` | [`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md) |
| `isMeshPicked` | `boolean` |
| `element` | [`Nullable`](../modules.md#nullable)`HTMLElement` |

#### Returns

[`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md)

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteSceneComponent.ts:328

___

### \_pointerUp

▸ `Private` **_pointerUp**(`unTranslatedPointerX`, `unTranslatedPointerY`, `pickResult`, `evt`): [`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `unTranslatedPointerX` | `number` |
| `unTranslatedPointerY` | `number` |
| `pickResult` | [`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md) |
| `evt` | [`IPointerEvent`](../interfaces/IPointerEvent.md) |

#### Returns

[`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md)

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteSceneComponent.ts:400

___

### dispose

▸ **dispose**(): `void`

Disposes the component and the associated resources.

#### Returns

`void`

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[dispose](../interfaces/ISceneComponent.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteSceneComponent.ts:310

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

https://github.com/babylon.js/core/src/Sprites/spriteSceneComponent.ts:303

___

### register

▸ **register**(): `void`

Registers the component in a given scene

#### Returns

`void`

#### Implementation of

[ISceneComponent](../interfaces/ISceneComponent.md).[register](../interfaces/ISceneComponent.md#register)

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteSceneComponent.ts:293
