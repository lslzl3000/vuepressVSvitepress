[@dev/core](../README.md) / [Exports](../modules.md) / IInspectableOptions

# Interface: IInspectableOptions

Interface used to define custom inspectable options in "Options" mode.
This interface is used by the inspector to display the list of options

## Table of contents

### Properties

- [label](IInspectableOptions.md#label)
- [selected](IInspectableOptions.md#selected)
- [value](IInspectableOptions.md#value)

## Properties

### label

• **label**: `string`

Defines the visible part of the option

#### Defined in

https://github.com/babylon.js/core/src/Misc/iInspectable.ts:51

___

### selected

• `Optional` **selected**: `boolean`

Defines if the option should be selected or not

#### Defined in

https://github.com/babylon.js/core/src/Misc/iInspectable.ts:59

___

### value

• **value**: `string` \| `number`

Defines the value part of the option (returned through the callback)

#### Defined in

https://github.com/babylon.js/core/src/Misc/iInspectable.ts:55
