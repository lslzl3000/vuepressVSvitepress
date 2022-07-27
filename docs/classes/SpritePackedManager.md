[@dev/core](../README.md) / [Exports](../modules.md) / SpritePackedManager

# Class: SpritePackedManager

Class used to manage multiple sprites of different sizes on the same spritesheet

**`See`**

https://doc.babylonjs.com/babylon101/sprites

## Hierarchy

- [`SpriteManager`](SpriteManager.md)

  ↳ **`SpritePackedManager`**

## Table of contents

### Constructors

- [constructor](SpritePackedManager.md#constructor)

### Properties

- [isPickable](SpritePackedManager.md#ispickable)
- [layerMask](SpritePackedManager.md#layermask)
- [name](SpritePackedManager.md#name)
- [onDisposeObservable](SpritePackedManager.md#ondisposeobservable)
- [renderingGroupId](SpritePackedManager.md#renderinggroupid)
- [snippetId](SpritePackedManager.md#snippetid)
- [sprites](SpritePackedManager.md#sprites)
- [uniqueId](SpritePackedManager.md#uniqueid)
- [CreateFromSnippetAsync](SpritePackedManager.md#createfromsnippetasync)
- [SnippetUrl](SpritePackedManager.md#snippeturl)

### Accessors

- [blendMode](SpritePackedManager.md#blendmode)
- [capacity](SpritePackedManager.md#capacity)
- [cellHeight](SpritePackedManager.md#cellheight)
- [cellWidth](SpritePackedManager.md#cellwidth)
- [children](SpritePackedManager.md#children)
- [disableDepthWrite](SpritePackedManager.md#disabledepthwrite)
- [fogEnabled](SpritePackedManager.md#fogenabled)
- [onDispose](SpritePackedManager.md#ondispose)
- [scene](SpritePackedManager.md#scene)
- [texture](SpritePackedManager.md#texture)

### Methods

- [dispose](SpritePackedManager.md#dispose)
- [getClassName](SpritePackedManager.md#getclassname)
- [intersects](SpritePackedManager.md#intersects)
- [multiIntersects](SpritePackedManager.md#multiintersects)
- [rebuild](SpritePackedManager.md#rebuild)
- [render](SpritePackedManager.md#render)
- [serialize](SpritePackedManager.md#serialize)
- [Parse](SpritePackedManager.md#parse)
- [ParseFromFileAsync](SpritePackedManager.md#parsefromfileasync)
- [ParseFromSnippetAsync](SpritePackedManager.md#parsefromsnippetasync)

## Constructors

### constructor

• **new SpritePackedManager**(`name`, `imgUrl`, `capacity`, `scene`, `spriteJSON?`, `epsilon?`, `samplingMode?`)

Creates a new sprite manager from a packed sprite sheet

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | defines the manager's name |
| `imgUrl` | `string` | `undefined` | defines the sprite sheet url |
| `capacity` | `number` | `undefined` | defines the maximum allowed number of sprites |
| `scene` | [`Scene`](Scene.md) | `undefined` | defines the hosting scene |
| `spriteJSON` | ``null`` \| `string` | `null` | null otherwise a JSON object defining sprite sheet data |
| `epsilon` | `number` | `0.01` | defines the epsilon value to align texture (0.01 by default) |
| `samplingMode` | `number` | `Texture.TRILINEAR_SAMPLINGMODE` | defines the sampling mode to use with spritesheet |

#### Overrides

[SpriteManager](SpriteManager.md).[constructor](SpriteManager.md#constructor)

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spritePackedManager.ts:23

## Properties

### isPickable

• **isPickable**: `boolean` = `false`

Gets or sets a boolean indicating if the sprites are pickable

#### Inherited from

[SpriteManager](SpriteManager.md).[isPickable](SpriteManager.md#ispickable)

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:120

___

### layerMask

• **layerMask**: `number` = `0x0fffffff`

Gets or sets camera layer mask

#### Inherited from

[SpriteManager](SpriteManager.md).[layerMask](SpriteManager.md#layermask)

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:118

___

### name

• **name**: `string`

Gets manager's name

#### Inherited from

[SpriteManager](SpriteManager.md).[name](SpriteManager.md#name)

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spritePackedManager.ts:25

___

### onDisposeObservable

• **onDisposeObservable**: [`Observable`](Observable.md)[`SpriteManager`](SpriteManager.md)

An event triggered when the manager is disposed.

#### Inherited from

[SpriteManager](SpriteManager.md).[onDisposeObservable](SpriteManager.md#ondisposeobservable)

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:125

___

### renderingGroupId

• **renderingGroupId**: `number` = `0`

Gets or sets the rendering group id (0 by default)

#### Inherited from

[SpriteManager](SpriteManager.md).[renderingGroupId](SpriteManager.md#renderinggroupid)

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:116

___

### snippetId

• **snippetId**: `string`

Snippet ID if the manager was created from the snippet server

#### Inherited from

[SpriteManager](SpriteManager.md).[snippetId](SpriteManager.md#snippetid)

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:111

___

### sprites

• **sprites**: [`Sprite`](Sprite.md)[]

Gets the list of sprites

#### Inherited from

[SpriteManager](SpriteManager.md).[sprites](SpriteManager.md#sprites)

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:114

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the sprite

#### Inherited from

[SpriteManager](SpriteManager.md).[uniqueId](SpriteManager.md#uniqueid)

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:140

___

### CreateFromSnippetAsync

▪ `Static` **CreateFromSnippetAsync**: (`snippetId`: `string`, `scene`: [`Scene`](Scene.md), `rootUrl`: `string`) => `Promise`[`SpriteManager`](SpriteManager.md) = `SpriteManager.ParseFromSnippetAsync`

#### Type declaration

▸ (`snippetId`, `scene`, `rootUrl?`): `Promise`[`SpriteManager`](SpriteManager.md)

Creates a sprite manager from a snippet saved by the sprite editor

##### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `snippetId` | `string` | `undefined` | defines the snippet to load (can be set to _BLANK to create a default one) |
| `scene` | [`Scene`](Scene.md) | `undefined` | defines the hosting scene |
| `rootUrl` | `string` | `""` | defines the root URL to use to load textures and relative dependencies |

##### Returns

`Promise`[`SpriteManager`](SpriteManager.md)

a promise that will resolve to the new sprite manager

#### Inherited from

[SpriteManager](SpriteManager.md).[CreateFromSnippetAsync](SpriteManager.md#createfromsnippetasync)

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:767

___

### SnippetUrl

▪ `Static` **SnippetUrl**: `string` = `Constants.SnippetUrl`

Define the Url to load snippets

#### Inherited from

[SpriteManager](SpriteManager.md).[SnippetUrl](SpriteManager.md#snippeturl)

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:108

## Accessors

### blendMode

• `get` **blendMode**(): `number`

Blend mode use to render the particle, it can be any of
the static Constants.ALPHA_x properties provided in this class.
Default value is Constants.ALPHA_COMBINE

#### Returns

`number`

#### Inherited from

SpriteManager.blendMode

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:205

• `set` **blendMode**(`blendMode`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `blendMode` | `number` |

#### Returns

`void`

#### Inherited from

SpriteManager.blendMode

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:208

___

### capacity

• `get` **capacity**(): `number`

Gets the capacity of the manager

#### Returns

`number`

#### Inherited from

SpriteManager.capacity

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:159

___

### cellHeight

• `get` **cellHeight**(): `number`

Defines the default height of a cell in the spritesheet

#### Returns

`number`

#### Inherited from

SpriteManager.cellHeight

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:185

• `set` **cellHeight**(`value`): `void`

Defines the default height of a cell in the spritesheet

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

SpriteManager.cellHeight

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:188

___

### cellWidth

• `get` **cellWidth**(): `number`

Defines the default width of a cell in the spritesheet

#### Returns

`number`

#### Inherited from

SpriteManager.cellWidth

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:177

• `set` **cellWidth**(`value`): `void`

Defines the default width of a cell in the spritesheet

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Inherited from

SpriteManager.cellWidth

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:180

___

### children

• `get` **children**(): [`Sprite`](Sprite.md)[]

Gets the array of sprites

#### Returns

[`Sprite`](Sprite.md)[]

#### Inherited from

SpriteManager.children

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:145

___

### disableDepthWrite

• `get` **disableDepthWrite**(): `boolean`

Disables writing to the depth buffer when rendering the sprites.
 It can be handy to disable depth writing when using textures without alpha channel
 and setting some specific blend modes.

#### Returns

`boolean`

#### Inherited from

SpriteManager.disableDepthWrite

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:217

• `set` **disableDepthWrite**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

SpriteManager.disableDepthWrite

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:221

___

### fogEnabled

• `get` **fogEnabled**(): `boolean`

Gets or sets a boolean indicating if the manager must consider scene fog when rendering

#### Returns

`boolean`

#### Inherited from

SpriteManager.fogEnabled

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:193

• `set` **fogEnabled**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

SpriteManager.fogEnabled

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:196

___

### onDispose

• `set` **onDispose**(`callback`): `void`

Callback called when the manager is disposed

#### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | () => `void` |

#### Returns

`void`

#### Inherited from

SpriteManager.onDispose

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:130

___

### scene

• `get` **scene**(): [`Scene`](Scene.md)

Gets the hosting scene

#### Returns

[`Scene`](Scene.md)

#### Inherited from

SpriteManager.scene

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:152

___

### texture

• `get` **texture**(): [`Texture`](Texture.md)

Gets or sets the spritesheet texture

#### Returns

[`Texture`](Texture.md)

#### Inherited from

SpriteManager.texture

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:166

• `set` **texture**(`value`): `void`

Gets or sets the spritesheet texture

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Texture`](Texture.md) |

#### Returns

`void`

#### Inherited from

SpriteManager.texture

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:169

## Methods

### dispose

▸ **dispose**(): `void`

Release associated resources

#### Returns

`void`

#### Inherited from

[SpriteManager](SpriteManager.md).[dispose](SpriteManager.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:611

___

### getClassName

▸ **getClassName**(): `string`

Returns the string "SpriteManager"

#### Returns

`string`

"SpriteManager"

#### Inherited from

[SpriteManager](SpriteManager.md).[getClassName](SpriteManager.md#getclassname)

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:302

___

### intersects

▸ **intersects**(`ray`, `camera`, `predicate?`, `fastCheck?`): [`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md)

Intersects the sprites with a ray

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ray` | [`Ray`](Ray.md) | defines the ray to intersect with |
| `camera` | [`Camera`](Camera.md) | defines the current active camera |
| `predicate?` | (`sprite`: [`Sprite`](Sprite.md)) => `boolean` | defines a predicate used to select candidate sprites |
| `fastCheck?` | `boolean` | defines if a fast check only must be done (the first potential sprite is will be used and not the closer) |

#### Returns

[`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md)

null if no hit or a PickingInfo

#### Inherited from

[SpriteManager](SpriteManager.md).[intersects](SpriteManager.md#intersects)

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:414

___

### multiIntersects

▸ **multiIntersects**(`ray`, `camera`, `predicate?`): [`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md)[]

Intersects the sprites with a ray

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ray` | [`Ray`](Ray.md) | defines the ray to intersect with |
| `camera` | [`Camera`](Camera.md) | defines the current active camera |
| `predicate?` | (`sprite`: [`Sprite`](Sprite.md)) => `boolean` | defines a predicate used to select candidate sprites |

#### Returns

[`Nullable`](../modules.md#nullable)[`PickingInfo`](PickingInfo.md)[]

null if no hit or a PickingInfo array

#### Inherited from

[SpriteManager](SpriteManager.md).[multiIntersects](SpriteManager.md#multiintersects)

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:511

___

### rebuild

▸ **rebuild**(): `void`

Rebuilds the manager (after a context lost, for eg)

#### Returns

`void`

#### Inherited from

[SpriteManager](SpriteManager.md).[rebuild](SpriteManager.md#rebuild)

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:604

___

### render

▸ **render**(): `void`

Render all child sprites

#### Returns

`void`

#### Inherited from

[SpriteManager](SpriteManager.md).[render](SpriteManager.md#render)

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:572

___

### serialize

▸ **serialize**(`serializeTexture?`): `any`

Serializes the sprite manager to a JSON object

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `serializeTexture` | `boolean` | `false` | defines if the texture must be serialized as well |

#### Returns

`any`

the JSON object

#### Inherited from

[SpriteManager](SpriteManager.md).[serialize](SpriteManager.md#serialize)

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:633

___

### Parse

▸ `Static` **Parse**(`parsedManager`, `scene`, `rootUrl`): [`SpriteManager`](SpriteManager.md)

Parses a JSON object to create a new sprite manager.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `parsedManager` | `any` | The JSON object to parse |
| `scene` | [`Scene`](Scene.md) | The scene to create the sprite manager |
| `rootUrl` | `string` | The root url to use to load external dependencies like texture |

#### Returns

[`SpriteManager`](SpriteManager.md)

the new sprite manager

#### Inherited from

[SpriteManager](SpriteManager.md).[Parse](SpriteManager.md#parse)

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:666

___

### ParseFromFileAsync

▸ `Static` **ParseFromFileAsync**(`name`, `url`, `scene`, `rootUrl?`): `Promise`[`SpriteManager`](SpriteManager.md)

Creates a sprite manager from a snippet saved in a remote file

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | [`Nullable`](../modules.md#nullable)`string` | `undefined` | defines the name of the sprite manager to create (can be null or empty to use the one from the json data) |
| `url` | `string` | `undefined` | defines the url to load from |
| `scene` | [`Scene`](Scene.md) | `undefined` | defines the hosting scene |
| `rootUrl` | `string` | `""` | defines the root URL to use to load textures and relative dependencies |

#### Returns

`Promise`[`SpriteManager`](SpriteManager.md)

a promise that will resolve to the new sprite manager

#### Inherited from

[SpriteManager](SpriteManager.md).[ParseFromFileAsync](SpriteManager.md#parsefromfileasync)

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:699

___

### ParseFromSnippetAsync

▸ `Static` **ParseFromSnippetAsync**(`snippetId`, `scene`, `rootUrl?`): `Promise`[`SpriteManager`](SpriteManager.md)

Creates a sprite manager from a snippet saved by the sprite editor

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `snippetId` | `string` | `undefined` | defines the snippet to load (can be set to _BLANK to create a default one) |
| `scene` | [`Scene`](Scene.md) | `undefined` | defines the hosting scene |
| `rootUrl` | `string` | `""` | defines the root URL to use to load textures and relative dependencies |

#### Returns

`Promise`[`SpriteManager`](SpriteManager.md)

a promise that will resolve to the new sprite manager

#### Inherited from

[SpriteManager](SpriteManager.md).[ParseFromSnippetAsync](SpriteManager.md#parsefromsnippetasync)

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteManager.ts:731
