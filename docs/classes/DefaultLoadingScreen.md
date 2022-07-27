[@dev/core](../README.md) / [Exports](../modules.md) / DefaultLoadingScreen

# Class: DefaultLoadingScreen

Class used for the default loading screen

**`See`**

https://doc.babylonjs.com/how_to/creating_a_custom_loading_screen

## Implements

- [`ILoadingScreen`](../interfaces/ILoadingScreen.md)

## Table of contents

### Constructors

- [constructor](DefaultLoadingScreen.md#constructor)

### Properties

- [\_loadingDiv](DefaultLoadingScreen.md#_loadingdiv)
- [\_loadingTextDiv](DefaultLoadingScreen.md#_loadingtextdiv)
- [\_style](DefaultLoadingScreen.md#_style)
- [DefaultLogoUrl](DefaultLoadingScreen.md#defaultlogourl)
- [DefaultSpinnerUrl](DefaultLoadingScreen.md#defaultspinnerurl)

### Accessors

- [loadingUIBackgroundColor](DefaultLoadingScreen.md#loadinguibackgroundcolor)
- [loadingUIText](DefaultLoadingScreen.md#loadinguitext)

### Methods

- [\_resizeLoadingUI](DefaultLoadingScreen.md#_resizeloadingui)
- [displayLoadingUI](DefaultLoadingScreen.md#displayloadingui)
- [hideLoadingUI](DefaultLoadingScreen.md#hideloadingui)

## Constructors

### constructor

• **new DefaultLoadingScreen**(`_renderingCanvas`, `_loadingText?`, `_loadingDivBackgroundColor?`)

Creates a new default loading screen

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `_renderingCanvas` | `HTMLCanvasElement` | `undefined` | defines the canvas used to render the scene |
| `_loadingText` | `string` | `""` | defines the default text to display |
| `_loadingDivBackgroundColor` | `string` | `"black"` | defines the default background color |

#### Defined in

packages/dev/core/src/Loading/loadingScreen.ts:47

## Properties

### \_loadingDiv

• `Private` **\_loadingDiv**: [`Nullable`](../modules.md#nullable)`HTMLDivElement`

#### Defined in

packages/dev/core/src/Loading/loadingScreen.ts:31

___

### \_loadingTextDiv

• `Private` **\_loadingTextDiv**: `HTMLDivElement`

#### Defined in

packages/dev/core/src/Loading/loadingScreen.ts:32

___

### \_style

• `Private` **\_style**: [`Nullable`](../modules.md#nullable)`HTMLStyleElement`

#### Defined in

packages/dev/core/src/Loading/loadingScreen.ts:33

___

### DefaultLogoUrl

▪ `Static` **DefaultLogoUrl**: `string` = `""`

Gets or sets the logo url to use for the default loading screen

#### Defined in

packages/dev/core/src/Loading/loadingScreen.ts:36

___

### DefaultSpinnerUrl

▪ `Static` **DefaultSpinnerUrl**: `string` = `""`

Gets or sets the spinner url to use for the default loading screen

#### Defined in

packages/dev/core/src/Loading/loadingScreen.ts:39

## Accessors

### loadingUIBackgroundColor

• `get` **loadingUIBackgroundColor**(): `string`

Gets or sets the color to use for the background

#### Returns

`string`

#### Implementation of

[ILoadingScreen](../interfaces/ILoadingScreen.md).[loadingUIBackgroundColor](../interfaces/ILoadingScreen.md#loadinguibackgroundcolor)

#### Defined in

packages/dev/core/src/Loading/loadingScreen.ts:224

• `set` **loadingUIBackgroundColor**(`color`): `void`

Gets or sets the color to use for the background

#### Parameters

| Name | Type |
| :------ | :------ |
| `color` | `string` |

#### Returns

`void`

#### Implementation of

[ILoadingScreen](../interfaces/ILoadingScreen.md).[loadingUIBackgroundColor](../interfaces/ILoadingScreen.md#loadinguibackgroundcolor)

#### Defined in

packages/dev/core/src/Loading/loadingScreen.ts:228

___

### loadingUIText

• `get` **loadingUIText**(): `string`

Gets or sets the text to display while loading

#### Returns

`string`

#### Implementation of

[ILoadingScreen](../interfaces/ILoadingScreen.md).[loadingUIText](../interfaces/ILoadingScreen.md#loadinguitext)

#### Defined in

packages/dev/core/src/Loading/loadingScreen.ts:217

• `set` **loadingUIText**(`text`): `void`

Gets or sets the text to display while loading

#### Parameters

| Name | Type |
| :------ | :------ |
| `text` | `string` |

#### Returns

`void`

#### Implementation of

[ILoadingScreen](../interfaces/ILoadingScreen.md).[loadingUIText](../interfaces/ILoadingScreen.md#loadinguitext)

#### Defined in

packages/dev/core/src/Loading/loadingScreen.ts:209

## Methods

### \_resizeLoadingUI

▸ `Private` **_resizeLoadingUI**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Loading/loadingScreen.ts:239

___

### displayLoadingUI

▸ **displayLoadingUI**(): `void`

Function called to display the loading screen

#### Returns

`void`

#### Implementation of

ILoadingScreen.displayLoadingUI

#### Defined in

packages/dev/core/src/Loading/loadingScreen.ts:52

___

### hideLoadingUI

▸ **hideLoadingUI**(): `void`

Function called to hide the loading screen

#### Returns

`void`

#### Implementation of

ILoadingScreen.hideLoadingUI

#### Defined in

packages/dev/core/src/Loading/loadingScreen.ts:181
