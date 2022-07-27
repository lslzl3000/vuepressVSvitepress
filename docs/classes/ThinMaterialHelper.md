[@dev/core](../README.md) / [Exports](../modules.md) / ThinMaterialHelper

# Class: ThinMaterialHelper

"Static Class" containing a few commonly used helper while dealing with material for rendering purpose.

It is complementary with MaterialHelper but provides completely independent functions (for tree shaking sake)

This works by convention in BabylonJS but is meant to be use only with shader following the in place naming rules and conventions.

## Table of contents

### Constructors

- [constructor](ThinMaterialHelper.md#constructor)

### Methods

- [BindClipPlane](ThinMaterialHelper.md#bindclipplane)

## Constructors

### constructor

• **new ThinMaterialHelper**()

## Methods

### BindClipPlane

▸ `Static` **BindClipPlane**(`effect`, `holder`): `void`

Binds the clip plane information from the holder to the effect.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `effect` | [`Effect`](Effect.md) | The effect we are binding the data to |
| `holder` | `IClipPlanesHolder` | The entity containing the clip plane information |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Materials/thinMaterialHelper.ts:17
