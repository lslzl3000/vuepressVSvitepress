[@dev/core](../README.md) / [Exports](../modules.md) / Viewport

# Class: Viewport

Class used to represent a viewport on screen

## Table of contents

### Constructors

- [constructor](Viewport.md#constructor)

### Properties

- [height](Viewport.md#height)
- [width](Viewport.md#width)
- [x](Viewport.md#x)
- [y](Viewport.md#y)

### Methods

- [clone](Viewport.md#clone)
- [toGlobal](Viewport.md#toglobal)
- [toGlobalToRef](Viewport.md#toglobaltoref)

## Constructors

### constructor

• **new Viewport**(`x`, `y`, `width`, `height`)

Creates a Viewport object located at (x, y) and sized (width, height)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | defines viewport left coordinate |
| `y` | `number` | defines viewport top coordinate |
| `width` | `number` | defines the viewport width |
| `height` | `number` | defines the viewport height |

#### Defined in

packages/dev/core/src/Maths/math.viewport.ts:12

## Properties

### height

• **height**: `number`

#### Defined in

packages/dev/core/src/Maths/math.viewport.ts:20

___

### width

• **width**: `number`

#### Defined in

packages/dev/core/src/Maths/math.viewport.ts:18

___

### x

• **x**: `number`

#### Defined in

packages/dev/core/src/Maths/math.viewport.ts:14

___

### y

• **y**: `number`

#### Defined in

packages/dev/core/src/Maths/math.viewport.ts:16

## Methods

### clone

▸ **clone**(): [`Viewport`](Viewport.md)

Returns a new Viewport copied from the current one

#### Returns

[`Viewport`](Viewport.md)

a new Viewport

#### Defined in

packages/dev/core/src/Maths/math.viewport.ts:52

___

### toGlobal

▸ **toGlobal**(`renderWidth`, `renderHeight`): [`Viewport`](Viewport.md)

Creates a new viewport using absolute sizing (from 0-> width, 0-> height instead of 0->1)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `renderWidth` | `number` | defines the rendering width |
| `renderHeight` | `number` | defines the rendering height |

#### Returns

[`Viewport`](Viewport.md)

a new Viewport

#### Defined in

packages/dev/core/src/Maths/math.viewport.ts:29

___

### toGlobalToRef

▸ **toGlobalToRef**(`renderWidth`, `renderHeight`, `ref`): [`Viewport`](Viewport.md)

Stores absolute viewport value into a target viewport (from 0-> width, 0-> height instead of 0->1)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `renderWidth` | `number` | defines the rendering width |
| `renderHeight` | `number` | defines the rendering height |
| `ref` | [`Viewport`](Viewport.md) | defines the target viewport |

#### Returns

[`Viewport`](Viewport.md)

the current viewport

#### Defined in

packages/dev/core/src/Maths/math.viewport.ts:40
