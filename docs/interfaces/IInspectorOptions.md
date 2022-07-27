[@dev/core](../README.md) / [Exports](../modules.md) / IInspectorOptions

# Interface: IInspectorOptions

Interface used to define the options to use to create the Inspector

## Table of contents

### Properties

- [embedMode](IInspectorOptions.md#embedmode)
- [enableClose](IInspectorOptions.md#enableclose)
- [enablePopup](IInspectorOptions.md#enablepopup)
- [explorerExtensibility](IInspectorOptions.md#explorerextensibility)
- [globalRoot](IInspectorOptions.md#globalroot)
- [handleResize](IInspectorOptions.md#handleresize)
- [initialTab](IInspectorOptions.md#initialtab)
- [inspectorURL](IInspectorOptions.md#inspectorurl)
- [overlay](IInspectorOptions.md#overlay)
- [showExplorer](IInspectorOptions.md#showexplorer)
- [showInspector](IInspectorOptions.md#showinspector)

## Properties

### embedMode

• `Optional` **embedMode**: `boolean`

Display in embed mode (both panes on the right)

#### Defined in

https://github.com/babylon.js/core/src/Debug/debugLayer.ts:63

___

### enableClose

• `Optional` **enableClose**: `boolean`

Allow the panes to be closed by users (default: true)

#### Defined in

https://github.com/babylon.js/core/src/Debug/debugLayer.ts:75

___

### enablePopup

• `Optional` **enablePopup**: `boolean`

Allow the panes to popup (default: true)

#### Defined in

https://github.com/babylon.js/core/src/Debug/debugLayer.ts:71

___

### explorerExtensibility

• `Optional` **explorerExtensibility**: [`IExplorerExtensibilityGroup`](IExplorerExtensibilityGroup.md)[]

Optional list of extensibility entries

#### Defined in

https://github.com/babylon.js/core/src/Debug/debugLayer.ts:79

___

### globalRoot

• `Optional` **globalRoot**: `HTMLElement`

HTML element to use as root (the parent of the rendering canvas will be used as default value)

#### Defined in

https://github.com/babylon.js/core/src/Debug/debugLayer.ts:51

___

### handleResize

• `Optional` **handleResize**: `boolean`

let the Inspector handles resize of the canvas when panes are resized (default to true)

#### Defined in

https://github.com/babylon.js/core/src/Debug/debugLayer.ts:67

___

### initialTab

• `Optional` **initialTab**: [`DebugLayerTab`](../enums/DebugLayerTab.md)

Optional initial tab (default to DebugLayerTab.Properties)

#### Defined in

https://github.com/babylon.js/core/src/Debug/debugLayer.ts:87

___

### inspectorURL

• `Optional` **inspectorURL**: `string`

Optional URL to get the inspector script from (by default it uses the babylonjs CDN).

#### Defined in

https://github.com/babylon.js/core/src/Debug/debugLayer.ts:83

___

### overlay

• `Optional` **overlay**: `boolean`

Display in overlay mode (default: false)

#### Defined in

https://github.com/babylon.js/core/src/Debug/debugLayer.ts:47

___

### showExplorer

• `Optional` **showExplorer**: `boolean`

Display the Scene explorer

#### Defined in

https://github.com/babylon.js/core/src/Debug/debugLayer.ts:55

___

### showInspector

• `Optional` **showInspector**: `boolean`

Display the property inspector

#### Defined in

https://github.com/babylon.js/core/src/Debug/debugLayer.ts:59
