[@dev/core](../README.md) / [Exports](../modules.md) / SpriteManager

# Class: SpriteManager

Class used to manage multiple sprites on the same spritesheet

**`See`**

https://doc.babylonjs.com/babylon101/sprites

## Hierarchy

- **`SpriteManager`**

  ↳ [`SpritePackedManager`](SpritePackedManager.md)

## Implements

- [`ISpriteManager`](../interfaces/ISpriteManager.md)

## Table of contents

### Constructors

- [constructor](SpriteManager.md#constructor)

### Properties

- [\_cellData](SpriteManager.md#_celldata)
- [\_disableDepthWrite](SpriteManager.md#_disabledepthwrite)
- [\_fromPacked](SpriteManager.md#_frompacked)
- [\_onDisposeObserver](SpriteManager.md#_ondisposeobserver)
- [\_packedAndReady](SpriteManager.md#_packedandready)
- [\_scene](SpriteManager.md#_scene)
- [\_spriteMap](SpriteManager.md#_spritemap)
- [\_spriteRenderer](SpriteManager.md#_spriterenderer)
- [\_textureContent](SpriteManager.md#_texturecontent)
- [isPickable](SpriteManager.md#ispickable)
- [layerMask](SpriteManager.md#layermask)
- [name](SpriteManager.md#name)
- [onDisposeObservable](SpriteManager.md#ondisposeobservable)
- [renderingGroupId](SpriteManager.md#renderinggroupid)
- [snippetId](SpriteManager.md#snippetid)
- [sprites](SpriteManager.md#sprites)
- [uniqueId](SpriteManager.md#uniqueid)
- [CreateFromSnippetAsync](SpriteManager.md#createfromsnippetasync)
- [SnippetUrl](SpriteManager.md#snippeturl)

### Accessors

- [blendMode](SpriteManager.md#blendmode)
- [capacity](SpriteManager.md#capacity)
- [cellHeight](SpriteManager.md#cellheight)
- [cellWidth](SpriteManager.md#cellwidth)
- [children](SpriteManager.md#children)
- [disableDepthWrite](SpriteManager.md#disabledepthwrite)
- [fogEnabled](SpriteManager.md#fogenabled)
- [onDispose](SpriteManager.md#ondispose)
- [scene](SpriteManager.md#scene)
- [texture](SpriteManager.md#texture)

### Methods

- [\_checkTextureAlpha](SpriteManager.md#_checktexturealpha)
- [\_customUpdate](SpriteManager.md#_customupdate)
- [\_makePacked](SpriteManager.md#_makepacked)
- [dispose](SpriteManager.md#dispose)
- [getClassName](SpriteManager.md#getclassname)
- [intersects](SpriteManager.md#intersects)
- [multiIntersects](SpriteManager.md#multiintersects)
- [rebuild](SpriteManager.md#rebuild)
- [render](SpriteManager.md#render)
- [serialize](SpriteManager.md#serialize)
- [Parse](SpriteManager.md#parse)
- [ParseFromFileAsync](SpriteManager.md#parsefromfileasync)
- [ParseFromSnippetAsync](SpriteManager.md#parsefromsnippetasync)

## Constructors

### constructor

• **new SpriteManager**(`name`, `imgUrl`, `capacity`, `cellSize`, `scene`, `epsilon?`, `samplingMode?`, `fromPacked?`, `spriteJSON?`)

Creates a new sprite manager

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `name` | `string` | `undefined` | defines the manager's name |
| `imgUrl` | `string` | `undefined` | defines the sprite sheet url |
| `capacity` | `number` | `undefined` | defines the maximum allowed number of sprites |
| `cellSize` | `any` | `undefined` | defines the size of a sprite cell |
| `scene` | [`Scene`](Scene.md) | `undefined` | defines the hosting scene |
| `epsilon` | `number` | `0.01` | defines the epsilon value to align texture (0.01 by default) |
| `samplingMode` | `number` | `Texture.TRILINEAR_SAMPLINGMODE` | defines the sampling mode to use with spritesheet |
| `fromPacked` | `boolean` | `false` | set to false; do not alter |
| `spriteJSON` | `any` | `null` | null otherwise a JSON object defining sprite sheet data; do not alter |

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:250

## Properties

### \_cellData

• `Private` **\_cellData**: `any`

Associative array from JSON sprite data file

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:228

___

### \_disableDepthWrite

• `Private` **\_disableDepthWrite**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:212

___

### \_fromPacked

• `Private` **\_fromPacked**: `boolean`

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:235

___

### \_onDisposeObserver

• `Private` **\_onDisposeObserver**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)[`SpriteManager`](SpriteManager.md)

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:234

___

### \_packedAndReady

• `Private` **\_packedAndReady**: `boolean` = `false`

True when packed cell data from JSON file is ready

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:232

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:236

___

### \_spriteMap

• `Private` **\_spriteMap**: `string`[]

Array of sprite names from JSON sprite data file

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:230

___

### \_spriteRenderer

• `Private` **\_spriteRenderer**: `SpriteRenderer`

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:226

___

### \_textureContent

• `Private` **\_textureContent**: [`Nullable`](../modules.md#nullable)`Uint8Array`

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:233

___

### isPickable

• **isPickable**: `boolean` = `false`

Gets or sets a boolean indicating if the sprites are pickable

#### Implementation of

[ISpriteManager](../interfaces/ISpriteManager.md).[isPickable](../interfaces/ISpriteManager.md#ispickable)

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:120

___

### layerMask

• **layerMask**: `number` = `0x0fffffff`

Gets or sets camera layer mask

#### Implementation of

[ISpriteManager](../interfaces/ISpriteManager.md).[layerMask](../interfaces/ISpriteManager.md#layermask)

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:118

___

### name

• **name**: `string`

Gets manager's name

#### Implementation of

[ISpriteManager](../interfaces/ISpriteManager.md).[name](../interfaces/ISpriteManager.md#name)

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:252

___

### onDisposeObservable

• **onDisposeObservable**: [`Observable`](Observable.md)[`SpriteManager`](SpriteManager.md)

An event triggered when the manager is disposed.

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:125

___

### renderingGroupId

• **renderingGroupId**: `number` = `0`

Gets or sets the rendering group id (0 by default)

#### Implementation of

[ISpriteManager](../interfaces/ISpriteManager.md).[renderingGroupId](../interfaces/ISpriteManager.md#renderinggroupid)

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:116

___

### snippetId

• **snippetId**: `string`

Snippet ID if the manager was created from the snippet server

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:111

___

### sprites

• **sprites**: [`Sprite`](Sprite.md)[]

Gets the list of sprites

#### Implementation of

[ISpriteManager](../interfaces/ISpriteManager.md).[sprites](../interfaces/ISpriteManager.md#sprites)

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:114

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the sprite

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:140

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

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:767

___

### SnippetUrl

▪ `Static` **SnippetUrl**: `string` = `Constants.SnippetUrl`

Define the Url to load snippets

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:108

## Accessors

### blendMode

• `get` **blendMode**(): `number`

Blend mode use to render the particle, it can be any of
the static Constants.ALPHA_x properties provided in this class.
Default value is Constants.ALPHA_COMBINE

#### Returns

`number`

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:205

• `set` **blendMode**(`blendMode`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `blendMode` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:208

___

### capacity

• `get` **capacity**(): `number`

Gets the capacity of the manager

#### Returns

`number`

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:159

___

### cellHeight

• `get` **cellHeight**(): `number`

Defines the default height of a cell in the spritesheet

#### Returns

`number`

#### Implementation of

[ISpriteManager](../interfaces/ISpriteManager.md).[cellHeight](../interfaces/ISpriteManager.md#cellheight)

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:185

• `set` **cellHeight**(`value`): `void`

Defines the default height of a cell in the spritesheet

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Implementation of

[ISpriteManager](../interfaces/ISpriteManager.md).[cellHeight](../interfaces/ISpriteManager.md#cellheight)

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:188

___

### cellWidth

• `get` **cellWidth**(): `number`

Defines the default width of a cell in the spritesheet

#### Returns

`number`

#### Implementation of

[ISpriteManager](../interfaces/ISpriteManager.md).[cellWidth](../interfaces/ISpriteManager.md#cellwidth)

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:177

• `set` **cellWidth**(`value`): `void`

Defines the default width of a cell in the spritesheet

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Implementation of

[ISpriteManager](../interfaces/ISpriteManager.md).[cellWidth](../interfaces/ISpriteManager.md#cellwidth)

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:180

___

### children

• `get` **children**(): [`Sprite`](Sprite.md)[]

Gets the array of sprites

#### Returns

[`Sprite`](Sprite.md)[]

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:145

___

### disableDepthWrite

• `get` **disableDepthWrite**(): `boolean`

Disables writing to the depth buffer when rendering the sprites.
 It can be handy to disable depth writing when using textures without alpha channel
 and setting some specific blend modes.

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:217

• `set` **disableDepthWrite**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:221

___

### fogEnabled

• `get` **fogEnabled**(): `boolean`

Gets or sets a boolean indicating if the manager must consider scene fog when rendering

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:193

• `set` **fogEnabled**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:196

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

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:130

___

### scene

• `get` **scene**(): [`Scene`](Scene.md)

Gets the hosting scene

#### Returns

[`Scene`](Scene.md)

#### Implementation of

[ISpriteManager](../interfaces/ISpriteManager.md).[scene](../interfaces/ISpriteManager.md#scene)

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:152

___

### texture

• `get` **texture**(): [`Texture`](Texture.md)

Gets or sets the spritesheet texture

#### Returns

[`Texture`](Texture.md)

#### Implementation of

[ISpriteManager](../interfaces/ISpriteManager.md).[texture](../interfaces/ISpriteManager.md#texture)

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:166

• `set` **texture**(`value`): `void`

Gets or sets the spritesheet texture

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`Texture`](Texture.md) |

#### Returns

`void`

#### Implementation of

[ISpriteManager](../interfaces/ISpriteManager.md).[texture](../interfaces/ISpriteManager.md#texture)

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:169

## Methods

### \_checkTextureAlpha

▸ `Private` **_checkTextureAlpha**(`sprite`, `ray`, `distance`, `min`, `max`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `sprite` | [`Sprite`](Sprite.md) |
| `ray` | [`Ray`](Ray.md) |
| `distance` | `number` |
| `min` | [`Vector3`](Vector3.md) |
| `max` | [`Vector3`](Vector3.md) |

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:371

___

### \_customUpdate

▸ `Private` **_customUpdate**(`sprite`, `baseSize`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `sprite` | `ThinSprite` |
| `baseSize` | [`ISize`](../interfaces/ISize.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:587

___

### \_makePacked

▸ `Private` **_makePacked**(`imgUrl`, `spriteJSON`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `imgUrl` | `string` |
| `spriteJSON` | `any` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:306

___

### dispose

▸ **dispose**(): `void`

Release associated resources

#### Returns

`void`

#### Implementation of

[ISpriteManager](../interfaces/ISpriteManager.md).[dispose](../interfaces/ISpriteManager.md#dispose)

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:611

___

### getClassName

▸ **getClassName**(): `string`

Returns the string "SpriteManager"

#### Returns

`string`

"SpriteManager"

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:302

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

#### Implementation of

[ISpriteManager](../interfaces/ISpriteManager.md).[intersects](../interfaces/ISpriteManager.md#intersects)

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:414

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

#### Implementation of

[ISpriteManager](../interfaces/ISpriteManager.md).[multiIntersects](../interfaces/ISpriteManager.md#multiintersects)

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:511

___

### rebuild

▸ **rebuild**(): `void`

Rebuilds the manager (after a context lost, for eg)

#### Returns

`void`

#### Implementation of

[ISpriteManager](../interfaces/ISpriteManager.md).[rebuild](../interfaces/ISpriteManager.md#rebuild)

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:604

___

### render

▸ **render**(): `void`

Render all child sprites

#### Returns

`void`

#### Implementation of

[ISpriteManager](../interfaces/ISpriteManager.md).[render](../interfaces/ISpriteManager.md#render)

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:572

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

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:633

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

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:666

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

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:699

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

#### Defined in

packages/dev/core/src/Sprites/spriteManager.ts:731
