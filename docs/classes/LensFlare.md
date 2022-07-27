[@dev/core](../README.md) / [Exports](../modules.md) / LensFlare

# Class: LensFlare

This represents one of the lens effect in a `lensFlareSystem`.
It controls one of the individual texture used in the effect.

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_lens_flares

## Table of contents

### Constructors

- [constructor](LensFlare.md#constructor)

### Properties

- [\_system](LensFlare.md#_system)
- [alphaMode](LensFlare.md#alphamode)
- [color](LensFlare.md#color)
- [position](LensFlare.md#position)
- [size](LensFlare.md#size)
- [texture](LensFlare.md#texture)

### Methods

- [dispose](LensFlare.md#dispose)
- [AddFlare](LensFlare.md#addflare)

## Constructors

### constructor

• **new LensFlare**(`size`, `position`, `color`, `imgUrl`, `system`)

Instantiates a new Lens Flare.
This represents one of the lens effect in a `lensFlareSystem`.
It controls one of the individual texture used in the effect.

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_lens_flares

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `size` | `number` | Define the size of the lens flare in the system (a floating value between 0 and 1) |
| `position` | `number` | Define the position of the lens flare in the system. (a floating value between -1 and 1). A value of 0 is located on the emitter. A value greater than 0 is beyond the emitter and a value lesser than 0 is behind. |
| `color` | [`Color3`](Color3.md) | Define the lens color |
| `imgUrl` | `string` | Define the lens texture url |
| `system` | [`LensFlareSystem`](LensFlareSystem.md) | Define the `lensFlareSystem` this flare is part of |

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlare.ts:61

## Properties

### \_system

• `Private` **\_system**: [`LensFlareSystem`](LensFlareSystem.md)

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlare.ts:32

___

### alphaMode

• **alphaMode**: `number` = `Constants.ALPHA_ONEONE`

Define the alpha mode to render this particular lens.

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlare.ts:27

___

### color

• **color**: [`Color3`](Color3.md)

Define the lens color.

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlare.ts:17

___

### position

• **position**: `number`

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlare.ts:69

___

### size

• **size**: `number`

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlare.ts:65

___

### texture

• **texture**: [`Nullable`](../modules.md#nullable)[`Texture`](Texture.md)

Define the lens texture.

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlare.ts:22

## Methods

### dispose

▸ **dispose**(): `void`

Dispose and release the lens flare with its associated resources.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlare.ts:90

___

### AddFlare

▸ `Static` **AddFlare**(`size`, `position`, `color`, `imgUrl`, `system`): [`LensFlare`](LensFlare.md)

Creates a new Lens Flare.
This represents one of the lens effect in a `lensFlareSystem`.
It controls one of the individual texture used in the effect.

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_lens_flares

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `size` | `number` | Define the size of the lens flare (a floating value between 0 and 1) |
| `position` | `number` | Define the position of the lens flare in the system. (a floating value between -1 and 1). A value of 0 is located on the emitter. A value greater than 0 is beyond the emitter and a value lesser than 0 is behind. |
| `color` | [`Color3`](Color3.md) | Define the lens color |
| `imgUrl` | `string` | Define the lens texture url |
| `system` | [`LensFlareSystem`](LensFlareSystem.md) | Define the `lensFlareSystem` this flare is part of |

#### Returns

[`LensFlare`](LensFlare.md)

The newly created Lens Flare

#### Defined in

https://github.com/babylon.js/core/src/LensFlares/lensFlare.ts:46
