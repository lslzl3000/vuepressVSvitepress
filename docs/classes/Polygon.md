[@dev/core](../README.md) / [Exports](../modules.md) / Polygon

# Class: Polygon

Polygon

**`See`**

https://doc.babylonjs.com/how_to/parametric_shapes#non-regular-polygon

## Table of contents

### Constructors

- [constructor](Polygon.md#constructor)

### Methods

- [Circle](Polygon.md#circle)
- [Parse](Polygon.md#parse)
- [Rectangle](Polygon.md#rectangle)
- [StartingAt](Polygon.md#startingat)

## Constructors

### constructor

• **new Polygon**()

## Methods

### Circle

▸ `Static` **Circle**(`radius`, `cx?`, `cy?`, `numberOfSides?`): [`Vector2`](Vector2.md)[]

Creates a circle

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `radius` | `number` | `undefined` | radius of circle |
| `cx` | `number` | `0` | scale in x |
| `cy` | `number` | `0` | scale in y |
| `numberOfSides` | `number` | `32` | number of sides that make up the circle |

#### Returns

[`Vector2`](Vector2.md)[]

points that make the resulting circle

#### Defined in

https://github.com/babylon.js/core/src/Meshes/polygonMesh.ts:97

___

### Parse

▸ `Static` **Parse**(`input`): [`Vector2`](Vector2.md)[]

Creates a polygon from input string

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `input` | `string` | Input polygon data |

#### Returns

[`Vector2`](Vector2.md)[]

the parsed points

#### Defined in

https://github.com/babylon.js/core/src/Meshes/polygonMesh.ts:116

___

### Rectangle

▸ `Static` **Rectangle**(`xmin`, `ymin`, `xmax`, `ymax`): [`Vector2`](Vector2.md)[]

Creates a rectangle

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `xmin` | `number` | bottom X coord |
| `ymin` | `number` | bottom Y coord |
| `xmax` | `number` | top X coord |
| `ymax` | `number` | top Y coord |

#### Returns

[`Vector2`](Vector2.md)[]

points that make the resulting rectangle

#### Defined in

https://github.com/babylon.js/core/src/Meshes/polygonMesh.ts:85

___

### StartingAt

▸ `Static` **StartingAt**(`x`, `y`): [`Path2`](Path2.md)

Starts building a polygon from x and y coordinates

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | x coordinate |
| `y` | `number` | y coordinate |

#### Returns

[`Path2`](Path2.md)

the started path2

#### Defined in

https://github.com/babylon.js/core/src/Meshes/polygonMesh.ts:135
