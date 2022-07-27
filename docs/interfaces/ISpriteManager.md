[@dev/core](../README.md) / [Exports](../modules.md) / ISpriteManager

# Interface: ISpriteManager

Defines the minimum interface to fulfill in order to be a sprite manager.

## Hierarchy

- [`IDisposable`](IDisposable.md)

  ↳ **`ISpriteManager`**

## Implemented by

- [`SpriteManager`](../classes/SpriteManager.md)

## Table of contents

### Properties

- [cellHeight](ISpriteManager.md#cellheight)
- [cellWidth](ISpriteManager.md#cellwidth)
- [isPickable](ISpriteManager.md#ispickable)
- [layerMask](ISpriteManager.md#layermask)
- [name](ISpriteManager.md#name)
- [renderingGroupId](ISpriteManager.md#renderinggroupid)
- [scene](ISpriteManager.md#scene)
- [sprites](ISpriteManager.md#sprites)
- [texture](ISpriteManager.md#texture)

### Methods

- [dispose](ISpriteManager.md#dispose)
- [intersects](ISpriteManager.md#intersects)
- [multiIntersects](ISpriteManager.md#multiintersects)
- [rebuild](ISpriteManager.md#rebuild)
- [render](ISpriteManager.md#render)

## Properties

### cellHeight

• **cellHeight**: `number`

Defines the default height of a cell in the spritesheet

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:70

___

### cellWidth

• **cellWidth**: `number`

Defines the default width of a cell in the spritesheet

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:68

___

### isPickable

• **isPickable**: `boolean`

Gets or sets a boolean indicating if the mesh can be picked (by scene.pick for instance or through actions). Default is true

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:44

___

### layerMask

• **layerMask**: `number`

Restricts the camera to viewing objects with the same layerMask.
A camera with a layerMask of 1 will render spriteManager.layerMask & camera.layerMask!== 0

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:39

___

### name

• **name**: `string`

Gets manager's name

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:33

___

### renderingGroupId

• **renderingGroupId**: `number`

Specifies the rendering group id for this mesh (0 by default)

**`See`**

https://doc.babylonjs.com/resources/transparency_and_how_meshes_are_rendered#rendering-groups

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:55

___

### scene

• **scene**: [`Scene`](../classes/Scene.md)

Gets the hosting scene

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:49

___

### sprites

• **sprites**: [`Sprite`](../classes/Sprite.md)[]

Defines the list of sprites managed by the manager.

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:60

___

### texture

• **texture**: [`Texture`](../classes/Texture.md)

Gets or sets the spritesheet texture

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:65

## Methods

### dispose

▸ **dispose**(): `void`

Releases all held resources

#### Returns

`void`

#### Inherited from

[IDisposable](IDisposable.md).[dispose](IDisposable.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:103

___

### intersects

▸ **intersects**(`ray`, `camera`, `predicate?`, `fastCheck?`): [`Nullable`](../modules.md#nullable)[`PickingInfo`](../classes/PickingInfo.md)

Tests the intersection of a sprite with a specific ray.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ray` | [`Ray`](../classes/Ray.md) | The ray we are sending to test the collision |
| `camera` | [`Camera`](../classes/Camera.md) | The camera space we are sending rays in |
| `predicate?` | (`sprite`: [`Sprite`](../classes/Sprite.md)) => `boolean` | A predicate allowing excluding sprites from the list of object to test |
| `fastCheck?` | `boolean` | defines if the first intersection will be used (and not the closest) |

#### Returns

[`Nullable`](../modules.md#nullable)[`PickingInfo`](../classes/PickingInfo.md)

picking info or null.

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:80

___

### multiIntersects

▸ **multiIntersects**(`ray`, `camera`, `predicate?`): [`Nullable`](../modules.md#nullable)[`PickingInfo`](../classes/PickingInfo.md)[]

Intersects the sprites with a ray

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ray` | [`Ray`](../classes/Ray.md) | defines the ray to intersect with |
| `camera` | [`Camera`](../classes/Camera.md) | defines the current active camera |
| `predicate?` | (`sprite`: [`Sprite`](../classes/Sprite.md)) => `boolean` | defines a predicate used to select candidate sprites |

#### Returns

[`Nullable`](../modules.md#nullable)[`PickingInfo`](../classes/PickingInfo.md)[]

null if no hit or a PickingInfo array

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:89

___

### rebuild

▸ **rebuild**(): `void`

Rebuilds the manager (after a context lost, for eg)

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:99

___

### render

▸ **render**(): `void`

Renders the list of sprites on screen.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:94
