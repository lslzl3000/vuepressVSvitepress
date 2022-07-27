[@dev/core](../README.md) / [Exports](../modules.md) / TexturePackerFrame

# Class: TexturePackerFrame

This is a support class for frame Data on texture packer sets.

## Implements

- [`ITexturePackerFrame`](../interfaces/ITexturePackerFrame.md)

## Table of contents

### Constructors

- [constructor](TexturePackerFrame.md#constructor)

### Properties

- [id](TexturePackerFrame.md#id)
- [offset](TexturePackerFrame.md#offset)
- [scale](TexturePackerFrame.md#scale)

## Constructors

### constructor

• **new TexturePackerFrame**(`id`, `scale`, `offset`)

Initializes a texture package frame.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `number` | The numerical frame identifier |
| `scale` | [`Vector2`](Vector2.md) | Scalar Vector2 for UV frame |
| `offset` | [`Vector2`](Vector2.md) | Vector2 for the frame position in UV units. |

#### Defined in

packages/dev/core/src/Materials/Textures/Packer/frame.ts:49

## Properties

### id

• **id**: `number`

The frame ID

#### Implementation of

[ITexturePackerFrame](../interfaces/ITexturePackerFrame.md).[id](../interfaces/ITexturePackerFrame.md#id)

#### Defined in

packages/dev/core/src/Materials/Textures/Packer/frame.ts:30

___

### offset

• **offset**: [`Vector2`](Vector2.md)

The Frames offset

#### Implementation of

[ITexturePackerFrame](../interfaces/ITexturePackerFrame.md).[offset](../interfaces/ITexturePackerFrame.md#offset)

#### Defined in

packages/dev/core/src/Materials/Textures/Packer/frame.ts:40

___

### scale

• **scale**: [`Vector2`](Vector2.md)

The frames Scale

#### Implementation of

[ITexturePackerFrame](../interfaces/ITexturePackerFrame.md).[scale](../interfaces/ITexturePackerFrame.md#scale)

#### Defined in

packages/dev/core/src/Materials/Textures/Packer/frame.ts:35
