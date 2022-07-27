[@dev/core](../README.md) / [Exports](../modules.md) / ITexturePackerOptions

# Interface: ITexturePackerOptions

Defines the basic options interface of a TexturePacker

## Table of contents

### Properties

- [colnum](ITexturePackerOptions.md#colnum)
- [customFillColor](ITexturePackerOptions.md#customfillcolor)
- [disposeSources](ITexturePackerOptions.md#disposesources)
- [fillBlanks](ITexturePackerOptions.md#fillblanks)
- [frameSize](ITexturePackerOptions.md#framesize)
- [layout](ITexturePackerOptions.md#layout)
- [map](ITexturePackerOptions.md#map)
- [paddingColor](ITexturePackerOptions.md#paddingcolor)
- [paddingMode](ITexturePackerOptions.md#paddingmode)
- [paddingRatio](ITexturePackerOptions.md#paddingratio)
- [updateInputMeshes](ITexturePackerOptions.md#updateinputmeshes)
- [uvsIn](ITexturePackerOptions.md#uvsin)
- [uvsOut](ITexturePackerOptions.md#uvsout)

## Properties

### colnum

• `Optional` **colnum**: `number`

number of columns if using custom column count layout(2).  This defaults to 4.

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Packer/packer.ts:42

___

### customFillColor

• `Optional` **customFillColor**: `string`

string value representing the context fill style color.  Defaults to 'black'.

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Packer/packer.ts:62

___

### disposeSources

• `Optional` **disposeSources**: `boolean`

boolean flag to dispose all the source textures.  Defaults to true.

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Packer/packer.ts:52

___

### fillBlanks

• `Optional` **fillBlanks**: `boolean`

Fills the blank cells in a set to the customFillColor.  Defaults to true.

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Packer/packer.ts:57

___

### frameSize

• `Optional` **frameSize**: `number`

Width and Height Value of each Frame in the TexturePacker Sets

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Packer/packer.ts:67

___

### layout

• `Optional` **layout**: `number`

number representing the layout style. Defaults to LAYOUT_STRIP

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Packer/packer.ts:37

___

### map

• `Optional` **map**: `string`[]

Custom targets for the channels of a texture packer.  Default is all the channels of the Standard Material

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Packer/packer.ts:22

___

### paddingColor

• `Optional` **paddingColor**: [`Color3`](../classes/Color3.md) \| [`Color4`](../classes/Color4.md)

If in SUBUV_COLOR padding mode what color to use.

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Packer/packer.ts:82

___

### paddingMode

• `Optional` **paddingMode**: `number`

Number that declares the fill method for the padding gutter.

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Packer/packer.ts:77

___

### paddingRatio

• `Optional` **paddingRatio**: `number`

Ratio of the value to add padding wise to each cell.  Defaults to 0.0115

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Packer/packer.ts:72

___

### updateInputMeshes

• `Optional` **updateInputMeshes**: `boolean`

flag to update the input meshes to the new packed texture after compilation. Defaults to true.

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Packer/packer.ts:47

___

### uvsIn

• `Optional` **uvsIn**: `string`

the UV input targets, as a single value for all meshes. Defaults to VertexBuffer.UVKind

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Packer/packer.ts:27

___

### uvsOut

• `Optional` **uvsOut**: `string`

the UV output targets, as a single value for all meshes.  Defaults to VertexBuffer.UVKind

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/Packer/packer.ts:32
