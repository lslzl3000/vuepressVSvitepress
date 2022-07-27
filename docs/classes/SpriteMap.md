[@dev/core](../README.md) / [Exports](../modules.md) / SpriteMap

# Class: SpriteMap

Class used to manage a grid restricted sprite deployment on an Output plane.

## Implements

- [`ISpriteMap`](../interfaces/ISpriteMap.md)

## Table of contents

### Constructors

- [constructor](SpriteMap.md#constructor)

### Properties

- [\_animationMap](SpriteMap.md#_animationmap)
- [\_frameMap](SpriteMap.md#_framemap)
- [\_material](SpriteMap.md#_material)
- [\_output](SpriteMap.md#_output)
- [\_scene](SpriteMap.md#_scene)
- [\_tileMaps](SpriteMap.md#_tilemaps)
- [\_time](SpriteMap.md#_time)
- [atlasJSON](SpriteMap.md#atlasjson)
- [name](SpriteMap.md#name)
- [options](SpriteMap.md#options)
- [spriteSheet](SpriteMap.md#spritesheet)
- [sprites](SpriteMap.md#sprites)

### Accessors

- [animationMap](SpriteMap.md#animationmap)
- [position](SpriteMap.md#position)
- [rotation](SpriteMap.md#rotation)
- [spriteCount](SpriteMap.md#spritecount)

### Methods

- [\_createFrameBuffer](SpriteMap.md#_createframebuffer)
- [\_createTileAnimationBuffer](SpriteMap.md#_createtileanimationbuffer)
- [\_createTileBuffer](SpriteMap.md#_createtilebuffer)
- [addAnimationToTile](SpriteMap.md#addanimationtotile)
- [changeTiles](SpriteMap.md#changetiles)
- [dispose](SpriteMap.md#dispose)
- [getMousePosition](SpriteMap.md#getmouseposition)
- [getTileID](SpriteMap.md#gettileid)
- [loadTileMaps](SpriteMap.md#loadtilemaps)
- [saveTileMaps](SpriteMap.md#savetilemaps)

## Constructors

### constructor

• **new SpriteMap**(`name`, `atlasJSON`, `spriteSheet`, `options`, `scene`)

Creates a new SpriteMap

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the SpriteMaps Name |
| `atlasJSON` | [`ISpriteJSONAtlas`](../interfaces/ISpriteJSONAtlas.md) | is the JSON file that controls the Sprites Frames and Meta |
| `spriteSheet` | [`Texture`](Texture.md) | is the Texture that the Sprites are on. |
| `options` | [`ISpriteMapOptions`](../interfaces/ISpriteMapOptions.md) | a basic deployment configuration |
| `scene` | [`Scene`](Scene.md) | The Scene that the map is deployed on |

#### Defined in

packages/dev/core/src/Sprites/spriteMap.ts:179

## Properties

### \_animationMap

• `Private` **\_animationMap**: [`RawTexture`](RawTexture.md)

Texture Buffer of Float32 that holds Animation Data

#### Defined in

packages/dev/core/src/Sprites/spriteMap.ts:160

___

### \_frameMap

• `Private` **\_frameMap**: [`RawTexture`](RawTexture.md)

Texture Buffer of Float32 that holds tile frame data

#### Defined in

packages/dev/core/src/Sprites/spriteMap.ts:154

___

### \_material

• `Private` **\_material**: [`ShaderMaterial`](ShaderMaterial.md)

Custom ShaderMaterial Central to the System

#### Defined in

packages/dev/core/src/Sprites/spriteMap.ts:163

___

### \_output

• `Private` **\_output**: [`Mesh`](Mesh.md)

Custom ShaderMaterial Central to the System

#### Defined in

packages/dev/core/src/Sprites/spriteMap.ts:166

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

Scene that the SpriteMap was created in

#### Defined in

packages/dev/core/src/Sprites/spriteMap.ts:151

___

### \_tileMaps

• `Private` **\_tileMaps**: [`RawTexture`](RawTexture.md)[]

Texture Buffers of Float32 that holds tileMap data

#### Defined in

packages/dev/core/src/Sprites/spriteMap.ts:157

___

### \_time

• `Private` **\_time**: `number`

Systems Time Ticker

#### Defined in

packages/dev/core/src/Sprites/spriteMap.ts:169

___

### atlasJSON

• **atlasJSON**: [`ISpriteJSONAtlas`](../interfaces/ISpriteJSONAtlas.md)

The JSON file with the frame and meta data

#### Implementation of

[ISpriteMap](../interfaces/ISpriteMap.md).[atlasJSON](../interfaces/ISpriteMap.md#atlasjson)

#### Defined in

packages/dev/core/src/Sprites/spriteMap.ts:100

___

### name

• **name**: `string`

The Name of the spriteMap

#### Implementation of

[ISpriteMap](../interfaces/ISpriteMap.md).[name](../interfaces/ISpriteMap.md#name)

#### Defined in

packages/dev/core/src/Sprites/spriteMap.ts:97

___

### options

• **options**: [`ISpriteMapOptions`](../interfaces/ISpriteMapOptions.md)

Arguments passed with the Constructor

#### Implementation of

[ISpriteMap](../interfaces/ISpriteMap.md).[options](../interfaces/ISpriteMap.md#options)

#### Defined in

packages/dev/core/src/Sprites/spriteMap.ts:106

___

### spriteSheet

• **spriteSheet**: [`Texture`](Texture.md)

The systems Sprite Sheet Texture

#### Implementation of

[ISpriteMap](../interfaces/ISpriteMap.md).[spriteSheet](../interfaces/ISpriteMap.md#spritesheet)

#### Defined in

packages/dev/core/src/Sprites/spriteMap.ts:103

___

### sprites

• **sprites**: [`ISpriteJSONSprite`](../interfaces/ISpriteJSONSprite.md)[]

Public Sprite Storage array, parsed from atlasJSON

#### Defined in

packages/dev/core/src/Sprites/spriteMap.ts:109

## Accessors

### animationMap

• `get` **animationMap**(): [`RawTexture`](RawTexture.md)

Sets the AnimationMap

#### Returns

[`RawTexture`](RawTexture.md)

#### Defined in

packages/dev/core/src/Sprites/spriteMap.ts:137

• `set` **animationMap**(`v`): `void`

Sets the AnimationMap

#### Parameters

| Name | Type |
| :------ | :------ |
| `v` | [`RawTexture`](RawTexture.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Sprites/spriteMap.ts:142

___

### position

• `get` **position**(): [`Vector3`](Vector3.md)

Returns the Position of Output Plane

#### Returns

[`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Sprites/spriteMap.ts:117

• `set` **position**(`v`): `void`

Returns the Position of Output Plane

#### Parameters

| Name | Type |
| :------ | :------ |
| `v` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Sprites/spriteMap.ts:122

___

### rotation

• `get` **rotation**(): [`Vector3`](Vector3.md)

Returns the Rotation of Output Plane

#### Returns

[`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Sprites/spriteMap.ts:127

• `set` **rotation**(`v`): `void`

Returns the Rotation of Output Plane

#### Parameters

| Name | Type |
| :------ | :------ |
| `v` | [`Vector3`](Vector3.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Sprites/spriteMap.ts:132

___

### spriteCount

• `get` **spriteCount**(): `number`

Returns the Number of Sprites in the System

#### Returns

`number`

#### Defined in

packages/dev/core/src/Sprites/spriteMap.ts:112

## Methods

### \_createFrameBuffer

▸ `Private` **_createFrameBuffer**(): [`RawTexture`](RawTexture.md)

Creates the "frame" texture Buffer
-------------------------------------
Structure of frames
 "filename": "Falling-Water-2.png",
"frame": {"x":69,"y":103,"w":24,"h":32},
"rotated": true,
"trimmed": true,
"spriteSourceSize": {"x":4,"y":0,"w":24,"h":32},
"sourceSize": {"w":32,"h":32}

#### Returns

[`RawTexture`](RawTexture.md)

RawTexture of the frameMap

#### Defined in

packages/dev/core/src/Sprites/spriteMap.ts:353

___

### \_createTileAnimationBuffer

▸ `Private` **_createTileAnimationBuffer**(`buffer`): [`RawTexture`](RawTexture.md)

Creates the animationMap texture Buffer

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `buffer` | [`Nullable`](../modules.md#nullable)`ArrayBufferView` | normally and array of numbers, or a false to generate from scratch |

#### Returns

[`RawTexture`](RawTexture.md)

RawTexture of the animationMap

#### Defined in

packages/dev/core/src/Sprites/spriteMap.ts:465

___

### \_createTileBuffer

▸ `Private` **_createTileBuffer**(`buffer`, `_layer?`): [`RawTexture`](RawTexture.md)

Creates the tileMap texture Buffer

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `buffer` | `any` | `undefined` | normally and array of numbers, or a false to generate from scratch |
| `_layer` | `number` | `0` | indicates what layer for a logic trigger dealing with the baseTile.  The system uses this |

#### Returns

[`RawTexture`](RawTexture.md)

RawTexture of the tileMap

#### Defined in

packages/dev/core/src/Sprites/spriteMap.ts:399

___

### addAnimationToTile

▸ **addAnimationToTile**(`cellID?`, `_frame?`, `toCell?`, `time?`, `speed?`): `void`

Modifies the data of the animationMap

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `cellID` | `number` | `0` | is the Index of the Sprite |
| `_frame` | `number` | `0` | is the target Animation frame |
| `toCell` | `number` | `0` | is the Target Index of the next frame of the animation |
| `time` | `number` | `0` | is a value between 0-1 that is the trigger for when the frame should change tiles |
| `speed` | `number` | `1` | is a global scalar of the time variable on the map. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Sprites/spriteMap.ts:504

___

### changeTiles

▸ **changeTiles**(`_layer?`, `pos`, `tile?`): `void`

Modifies the data of the tileMaps

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `_layer` | `number` | `0` | is the ID of the layer you want to edit on the SpriteMap |
| `pos` | [`Vector2`](Vector2.md) \| [`Vector2`](Vector2.md)[] | `undefined` | is the iVector2 Coordinates of the Tile |
| `tile` | `number` | `0` | The SpriteIndex of the new Tile |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Sprites/spriteMap.ts:431

___

### dispose

▸ **dispose**(): `void`

Release associated resources

#### Returns

`void`

#### Implementation of

[ISpriteMap](../interfaces/ISpriteMap.md).[dispose](../interfaces/ISpriteMap.md#dispose)

#### Defined in

packages/dev/core/src/Sprites/spriteMap.ts:565

___

### getMousePosition

▸ **getMousePosition**(): [`Vector2`](Vector2.md)

Gets the UV location of the mouse over the SpriteMap.

#### Returns

[`Vector2`](Vector2.md)

Vector2 the UV position of the mouse interaction

#### Defined in

packages/dev/core/src/Sprites/spriteMap.ts:320

___

### getTileID

▸ **getTileID**(): [`Vector2`](Vector2.md)

Returns tileID location

#### Returns

[`Vector2`](Vector2.md)

Vector2 the cell position ID

#### Defined in

packages/dev/core/src/Sprites/spriteMap.ts:308

___

### loadTileMaps

▸ **loadTileMaps**(`url`): `void`

Imports the .tilemaps file

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `url` | `string` | of the .tilemaps file |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Sprites/spriteMap.ts:543

___

### saveTileMaps

▸ **saveTileMaps**(): `void`

Exports the .tilemaps file

#### Returns

`void`

#### Defined in

packages/dev/core/src/Sprites/spriteMap.ts:522
