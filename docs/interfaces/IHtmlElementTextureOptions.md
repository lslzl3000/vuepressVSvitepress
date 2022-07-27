[@dev/core](../README.md) / [Exports](../modules.md) / IHtmlElementTextureOptions

# Interface: IHtmlElementTextureOptions

Defines the options related to the creation of an HtmlElementTexture

## Table of contents

### Properties

- [engine](IHtmlElementTextureOptions.md#engine)
- [generateMipMaps](IHtmlElementTextureOptions.md#generatemipmaps)
- [samplingMode](IHtmlElementTextureOptions.md#samplingmode)
- [scene](IHtmlElementTextureOptions.md#scene)

## Properties

### engine

• **engine**: [`Nullable`](../modules.md#nullable)[`ThinEngine`](../classes/ThinEngine.md)

Defines the engine instance to use the texture with. It is not mandatory if you define a scene.

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/htmlElementTexture.ts:28

___

### generateMipMaps

• `Optional` **generateMipMaps**: `boolean`

Defines whether mip maps should be created or not.

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/htmlElementTexture.ts:20

___

### samplingMode

• `Optional` **samplingMode**: `number`

Defines the sampling mode of the texture.

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/htmlElementTexture.ts:24

___

### scene

• **scene**: [`Nullable`](../modules.md#nullable)[`Scene`](../classes/Scene.md)

Defines the scene the texture belongs to. It is not mandatory if you define an engine.

#### Defined in

https://github.com/babylon.js/core/src/Materials/Textures/htmlElementTexture.ts:32
