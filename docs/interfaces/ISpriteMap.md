[@dev/core](../README.md) / [Exports](../modules.md) / ISpriteMap

# Interface: ISpriteMap

Defines the IDisposable interface in order to be cleanable from resources.

## Hierarchy

- [`IDisposable`](IDisposable.md)

  ↳ **`ISpriteMap`**

## Implemented by

- [`SpriteMap`](../classes/SpriteMap.md)

## Table of contents

### Properties

- [atlasJSON](ISpriteMap.md#atlasjson)
- [name](ISpriteMap.md#name)
- [options](ISpriteMap.md#options)
- [spriteSheet](ISpriteMap.md#spritesheet)

### Methods

- [dispose](ISpriteMap.md#dispose)

## Properties

### atlasJSON

• **atlasJSON**: [`ISpriteJSONAtlas`](ISpriteJSONAtlas.md)

The JSON Array file from a https://www.codeandweb.com/texturepacker export.  Or similar structure.

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteMap.ts:79

___

### name

• **name**: `string`

String name of the SpriteMap.

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteMap.ts:74

___

### options

• **options**: [`ISpriteMapOptions`](ISpriteMapOptions.md)

The parameters to initialize the SpriteMap with.

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteMap.ts:89

___

### spriteSheet

• **spriteSheet**: [`Texture`](../classes/Texture.md)

Texture of the SpriteMap.

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteMap.ts:84

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
