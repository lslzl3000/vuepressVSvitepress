[@dev/core](../README.md) / [Exports](../modules.md) / ISpriteMapOptions

# Interface: ISpriteMapOptions

Defines the basic options interface of a SpriteMap

## Table of contents

### Properties

- [baseTile](ISpriteMapOptions.md#basetile)
- [colorMultiply](ISpriteMapOptions.md#colormultiply)
- [flipU](ISpriteMapOptions.md#flipu)
- [layerCount](ISpriteMapOptions.md#layercount)
- [maxAnimationFrames](ISpriteMapOptions.md#maxanimationframes)
- [outputPosition](ISpriteMapOptions.md#outputposition)
- [outputRotation](ISpriteMapOptions.md#outputrotation)
- [outputSize](ISpriteMapOptions.md#outputsize)
- [stageSize](ISpriteMapOptions.md#stagesize)

## Properties

### baseTile

• `Optional` **baseTile**: `number`

number cell index of the base tile when the system compiles.

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteMap.ts:54

___

### colorMultiply

• `Optional` **colorMultiply**: [`Vector3`](../classes/Vector3.md)

Vector3 scalar of the global RGB values of the SpriteMap.

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteMap.ts:64

___

### flipU

• `Optional` **flipU**: `boolean`

boolean flip the sprite after its been repositioned by the framing data.

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteMap.ts:59

___

### layerCount

• `Optional` **layerCount**: `number`

number of layers that the system will reserve in resources.

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteMap.ts:44

___

### maxAnimationFrames

• `Optional` **maxAnimationFrames**: `number`

number of max animation frames a single cell will reserve in resources.

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteMap.ts:49

___

### outputPosition

• `Optional` **outputPosition**: [`Vector3`](../classes/Vector3.md)

Vector3 of the position of the output plane in World Units.

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteMap.ts:34

___

### outputRotation

• `Optional` **outputRotation**: [`Vector3`](../classes/Vector3.md)

Vector3 of the rotation of the output plane.

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteMap.ts:39

___

### outputSize

• `Optional` **outputSize**: [`Vector2`](../classes/Vector2.md)

Vector2 of the size of the output plane in World Units.

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteMap.ts:29

___

### stageSize

• `Optional` **stageSize**: [`Vector2`](../classes/Vector2.md)

Vector2 of the number of cells in the grid.

#### Defined in

https://github.com/babylon.js/core/src/Sprites/spriteMap.ts:24
