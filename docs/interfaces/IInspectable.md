[@dev/core](../README.md) / [Exports](../modules.md) / IInspectable

# Interface: IInspectable

Interface used to define custom inspectable properties.
This interface is used by the inspector to display custom property grids

**`See`**

https://doc.babylonjs.com/how_to/debug_layer#extensibility

## Table of contents

### Properties

- [callback](IInspectable.md#callback)
- [label](IInspectable.md#label)
- [max](IInspectable.md#max)
- [min](IInspectable.md#min)
- [options](IInspectable.md#options)
- [propertyName](IInspectable.md#propertyname)
- [step](IInspectable.md#step)
- [type](IInspectable.md#type)

## Properties

### callback

• `Optional` **callback**: () => `void`

#### Type declaration

▸ (): `void`

Gets the callback function when using "Button" mode

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/iInspectable.ts:95

___

### label

• **label**: `string`

Gets the label to display

#### Defined in

https://github.com/babylon.js/core/src/Misc/iInspectable.ts:71

___

### max

• `Optional` **max**: `number`

Gets the maximum value of the property when using in "slider" mode

#### Defined in

https://github.com/babylon.js/core/src/Misc/iInspectable.ts:87

___

### min

• `Optional` **min**: `number`

Gets the minimum value of the property when using in "slider" mode

#### Defined in

https://github.com/babylon.js/core/src/Misc/iInspectable.ts:83

___

### options

• `Optional` **options**: [`IInspectableOptions`](IInspectableOptions.md)[]

Gets the list of options when using "Option" mode

#### Defined in

https://github.com/babylon.js/core/src/Misc/iInspectable.ts:99

___

### propertyName

• **propertyName**: `string`

Gets the name of the property to edit

#### Defined in

https://github.com/babylon.js/core/src/Misc/iInspectable.ts:75

___

### step

• `Optional` **step**: `number`

Gets the setp to use when using in "slider" mode

#### Defined in

https://github.com/babylon.js/core/src/Misc/iInspectable.ts:91

___

### type

• **type**: [`InspectableType`](../enums/InspectableType.md)

Gets the type of the editor to use

#### Defined in

https://github.com/babylon.js/core/src/Misc/iInspectable.ts:79
