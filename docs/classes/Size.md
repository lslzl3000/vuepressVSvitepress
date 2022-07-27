[@dev/core](../README.md) / [Exports](../modules.md) / Size

# Class: Size

Size containing width and height

## Implements

- [`ISize`](../interfaces/ISize.md)

## Table of contents

### Constructors

- [constructor](Size.md#constructor)

### Properties

- [height](Size.md#height)
- [width](Size.md#width)

### Accessors

- [surface](Size.md#surface)

### Methods

- [add](Size.md#add)
- [clone](Size.md#clone)
- [copyFrom](Size.md#copyfrom)
- [copyFromFloats](Size.md#copyfromfloats)
- [equals](Size.md#equals)
- [getClassName](Size.md#getclassname)
- [getHashCode](Size.md#gethashcode)
- [multiplyByFloats](Size.md#multiplybyfloats)
- [set](Size.md#set)
- [subtract](Size.md#subtract)
- [toString](Size.md#tostring)
- [Lerp](Size.md#lerp)
- [Zero](Size.md#zero)

## Constructors

### constructor

• **new Size**(`width`, `height`)

Creates a Size object from the given width and height (floats).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `width` | `number` | width of the new size |
| `height` | `number` | height of the new size |

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.size.ts:33

## Properties

### height

• **height**: `number`

Height

#### Implementation of

[ISize](../interfaces/ISize.md).[height](../interfaces/ISize.md#height)

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.size.ts:26

___

### width

• **width**: `number`

Width

#### Implementation of

[ISize](../interfaces/ISize.md).[width](../interfaces/ISize.md#width)

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.size.ts:22

## Accessors

### surface

• `get` **surface**(): `number`

The surface of the Size : width * height (float).

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.size.ts:119

## Methods

### add

▸ **add**(`otherSize`): [`Size`](Size.md)

Sums the width and height of two sizes

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherSize` | [`Size`](Size.md) | size to add to this size |

#### Returns

[`Size`](Size.md)

a new Size set as the addition result of the current Size and the given one.

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.size.ts:134

___

### clone

▸ **clone**(): [`Size`](Size.md)

Clones the size

#### Returns

[`Size`](Size.md)

a new Size copied from the given one.

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.size.ts:102

___

### copyFrom

▸ **copyFrom**(`src`): `void`

Updates the current size from the given one.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `src` | [`Size`](Size.md) | the given size |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.size.ts:65

___

### copyFromFloats

▸ **copyFromFloats**(`width`, `height`): [`Size`](Size.md)

Updates in place the current Size from the given floats.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `width` | `number` | width of the new size |
| `height` | `number` | height of the new size |

#### Returns

[`Size`](Size.md)

the updated Size.

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.size.ts:75

___

### equals

▸ **equals**(`other`): `boolean`

True if the current Size and the given one width and height are strictly equal.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `other` | [`Size`](Size.md) | the other size to compare against |

#### Returns

`boolean`

True if the current Size and the given one width and height are strictly equal.

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.size.ts:110

___

### getClassName

▸ **getClassName**(): `string`

"Size"

#### Returns

`string`

the string "Size"

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.size.ts:49

___

### getHashCode

▸ **getHashCode**(): `number`

Returns the Size hash code.

#### Returns

`number`

a hash code for a unique width and height

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.size.ts:56

___

### multiplyByFloats

▸ **multiplyByFloats**(`w`, `h`): [`Size`](Size.md)

Multiplies the width and height by numbers

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `w` | `number` | factor to multiple the width by |
| `h` | `number` | factor to multiple the height by |

#### Returns

[`Size`](Size.md)

a new Size set with the multiplication result of the current Size and the given floats.

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.size.ts:95

___

### set

▸ **set**(`width`, `height`): [`Size`](Size.md)

Updates in place the current Size from the given floats.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `width` | `number` | width to set |
| `height` | `number` | height to set |

#### Returns

[`Size`](Size.md)

the updated Size.

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.size.ts:86

___

### subtract

▸ **subtract**(`otherSize`): [`Size`](Size.md)

Subtracts the width and height of two

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `otherSize` | [`Size`](Size.md) | size to subtract to this size |

#### Returns

[`Size`](Size.md)

a new Size set as the subtraction result of  the given one from the current Size.

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.size.ts:143

___

### toString

▸ **toString**(): `string`

Returns a string with the Size width and height

#### Returns

`string`

a string with the Size width and height

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.size.ts:42

___

### Lerp

▸ `Static` **Lerp**(`start`, `end`, `amount`): [`Size`](Size.md)

Creates a new Size set at the linear interpolation "amount" between "start" and "end"

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `start` | [`Size`](Size.md) | starting size to lerp between |
| `end` | [`Size`](Size.md) | end size to lerp between |
| `amount` | `number` | amount to lerp between the start and end values |

#### Returns

[`Size`](Size.md)

a new Size set at the linear interpolation "amount" between "start" and "end"

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.size.ts:154

___

### Zero

▸ `Static` **Zero**(): [`Size`](Size.md)

Create a new size of zero

#### Returns

[`Size`](Size.md)

a new Size set to (0.0, 0.0)

#### Defined in

https://github.com/babylon.js/core/src/Maths/math.size.ts:126
