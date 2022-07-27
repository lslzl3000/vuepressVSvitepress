[@dev/core](../README.md) / [Exports](../modules.md) / ILoadingScreen

# Interface: ILoadingScreen

Interface used to present a loading screen while loading a scene

**`See`**

https://doc.babylonjs.com/how_to/creating_a_custom_loading_screen

## Implemented by

- [`DefaultLoadingScreen`](../classes/DefaultLoadingScreen.md)

## Table of contents

### Properties

- [displayLoadingUI](ILoadingScreen.md#displayloadingui)
- [hideLoadingUI](ILoadingScreen.md#hideloadingui)
- [loadingUIBackgroundColor](ILoadingScreen.md#loadinguibackgroundcolor)
- [loadingUIText](ILoadingScreen.md#loadinguitext)

## Properties

### displayLoadingUI

• **displayLoadingUI**: () => `void`

#### Type declaration

▸ (): `void`

Function called to display the loading screen

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Loading/loadingScreen.ts:11

___

### hideLoadingUI

• **hideLoadingUI**: () => `void`

#### Type declaration

▸ (): `void`

Function called to hide the loading screen

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Loading/loadingScreen.ts:15

___

### loadingUIBackgroundColor

• **loadingUIBackgroundColor**: `string`

Gets or sets the color to use for the background

#### Defined in

https://github.com/babylon.js/core/src/Loading/loadingScreen.ts:19

___

### loadingUIText

• **loadingUIText**: `string`

Gets or sets the text to display while loading

#### Defined in

https://github.com/babylon.js/core/src/Loading/loadingScreen.ts:23
