[@dev/core](../README.md) / [Exports](../modules.md) / ICanvasRenderingContext

# Interface: ICanvasRenderingContext

Class used to abstract canvas rendering

## Table of contents

### Properties

- [canvas](ICanvasRenderingContext.md#canvas)
- [fillStyle](ICanvasRenderingContext.md#fillstyle)
- [font](ICanvasRenderingContext.md#font)
- [globalAlpha](ICanvasRenderingContext.md#globalalpha)
- [lineJoin](ICanvasRenderingContext.md#linejoin)
- [lineWidth](ICanvasRenderingContext.md#linewidth)
- [miterLimit](ICanvasRenderingContext.md#miterlimit)
- [shadowBlur](ICanvasRenderingContext.md#shadowblur)
- [shadowColor](ICanvasRenderingContext.md#shadowcolor)
- [shadowOffsetX](ICanvasRenderingContext.md#shadowoffsetx)
- [shadowOffsetY](ICanvasRenderingContext.md#shadowoffsety)
- [strokeStyle](ICanvasRenderingContext.md#strokestyle)

### Methods

- [arc](ICanvasRenderingContext.md#arc)
- [beginPath](ICanvasRenderingContext.md#beginpath)
- [clearRect](ICanvasRenderingContext.md#clearrect)
- [clip](ICanvasRenderingContext.md#clip)
- [closePath](ICanvasRenderingContext.md#closepath)
- [createLinearGradient](ICanvasRenderingContext.md#createlineargradient)
- [drawImage](ICanvasRenderingContext.md#drawimage)
- [fill](ICanvasRenderingContext.md#fill)
- [fillRect](ICanvasRenderingContext.md#fillrect)
- [fillText](ICanvasRenderingContext.md#filltext)
- [getImageData](ICanvasRenderingContext.md#getimagedata)
- [lineTo](ICanvasRenderingContext.md#lineto)
- [measureText](ICanvasRenderingContext.md#measuretext)
- [moveTo](ICanvasRenderingContext.md#moveto)
- [putImageData](ICanvasRenderingContext.md#putimagedata)
- [quadraticCurveTo](ICanvasRenderingContext.md#quadraticcurveto)
- [rect](ICanvasRenderingContext.md#rect)
- [restore](ICanvasRenderingContext.md#restore)
- [rotate](ICanvasRenderingContext.md#rotate)
- [save](ICanvasRenderingContext.md#save)
- [scale](ICanvasRenderingContext.md#scale)
- [setLineDash](ICanvasRenderingContext.md#setlinedash)
- [setTransform](ICanvasRenderingContext.md#settransform)
- [stroke](ICanvasRenderingContext.md#stroke)
- [strokeRect](ICanvasRenderingContext.md#strokerect)
- [strokeText](ICanvasRenderingContext.md#stroketext)
- [translate](ICanvasRenderingContext.md#translate)

## Properties

### canvas

• `Readonly` **canvas**: [`ICanvas`](ICanvas.md)

canvas is a read-only reference to ICanvas.

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:177

___

### fillStyle

• **fillStyle**: `string` \| [`ICanvasGradient`](ICanvasGradient.md)

Color or style to use inside shapes. Default #000 (black).

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:142

___

### font

• **font**: `string`

Font setting. Default value 10px sans-serif.

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:132

___

### globalAlpha

• **globalAlpha**: `number`

Alpha value that is applied to shapes and images before they are composited onto the canvas. Default 1.0 (opaque).

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:147

___

### lineJoin

• **lineJoin**: `string`

Defines the type of corners where two lines meet. Possible values: round, bevel, miter (default).

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:122

___

### lineWidth

• **lineWidth**: `number`

Width of lines. Default 1.0.

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:172

___

### miterLimit

• **miterLimit**: `number`

Miter limit ratio. Default 10.

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:127

___

### shadowBlur

• **shadowBlur**: `number`

Specifies the blurring effect. Default: 0.

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:157

___

### shadowColor

• **shadowColor**: `string`

Color of the shadow. Default: fully-transparent black.

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:152

___

### shadowOffsetX

• **shadowOffsetX**: `number`

Horizontal distance the shadow will be offset. Default: 0.

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:162

___

### shadowOffsetY

• **shadowOffsetY**: `number`

Vertical distance the shadow will be offset. Default: 0.

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:167

___

### strokeStyle

• **strokeStyle**: `string`

Color or style to use for the lines around shapes. Default #000 (black).

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:137

## Methods

### arc

▸ **arc**(`x`, `y`, `radius`, `startAngle`, `endAngle`, `anticlockwise?`): `void`

Adds a circular arc to the current path.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | The horizontal coordinate of the arc's center. |
| `y` | `number` | The vertical coordinate of the arc's center. |
| `radius` | `number` | The arc's radius. Must be positive. |
| `startAngle` | `number` | The angle at which the arc starts in radians, measured from the positive x-axis. |
| `endAngle` | `number` | The angle at which the arc ends in radians, measured from the positive x-axis. |
| `anticlockwise?` | `boolean` | An optional Boolean. If true, draws the arc counter-clockwise between the start and end angles. The default is false (clockwise). |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:267

___

### beginPath

▸ **beginPath**(): `void`

Starts a new path by emptying the list of sub-paths. Call this method when you want to create a new path.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:272

___

### clearRect

▸ **clearRect**(`x`, `y`, `width`, `height`): `void`

Sets all pixels in the rectangle defined by starting point (x, y) and size (width, height) to transparent black, erasing any previously drawn content.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | The x-axis coordinate of the rectangle's starting point. |
| `y` | `number` | The y-axis coordinate of the rectangle's starting point. |
| `width` | `number` | The rectangle's width. Positive values are to the right, and negative to the left. |
| `height` | `number` | The rectangle's height. Positive values are down, and negative are up. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:186

___

### clip

▸ **clip**(): `void`

Creates a clipping path from the current sub-paths. Everything drawn after clip() is called appears inside the clipping path only.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:248

___

### closePath

▸ **closePath**(): `void`

Causes the point of the pen to move back to the start of the current sub-path. It tries to draw a straight line from the current point to the start.
If the shape has already been closed or has only one point, this function does nothing.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:278

___

### createLinearGradient

▸ **createLinearGradient**(`x0`, `y0`, `x1`, `y1`): [`ICanvasGradient`](ICanvasGradient.md)

Creates a linear gradient along the line given by the coordinates represented by the parameters.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x0` | `number` | The x-axis coordinate of the start point. |
| `y0` | `number` | The y-axis coordinate of the start point. |
| `x1` | `number` | The x-axis coordinate of the end point. |
| `y1` | `number` | The y-axis coordinate of the end point. |

#### Returns

[`ICanvasGradient`](ICanvasGradient.md)

ICanvasGradient A linear ICanvasGradient initialized with the specified line.

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:394

___

### drawImage

▸ **drawImage**(`image`, `sx`, `sy`, `sWidth`, `sHeight`, `dx`, `dy`, `dWidth`, `dHeight`): `void`

Draws the specified image. This method is available in multiple formats, providing a great deal of flexibility in its use.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `image` | `any` | An element to draw into the context. |
| `sx` | `number` | The x-axis coordinate of the top left corner of the sub-rectangle of the source image to draw into the destination context. |
| `sy` | `number` | The y-axis coordinate of the top left corner of the sub-rectangle of the source image to draw into the destination context. |
| `sWidth` | `number` | The width of the sub-rectangle of the source image to draw into the destination context. If not specified, the entire rectangle from the coordinates specified by sx and sy to the bottom-right corner of the image is used. |
| `sHeight` | `number` | The height of the sub-rectangle of the source image to draw into the destination context. |
| `dx` | `number` | The x-axis coordinate in the destination canvas at which to place the top-left corner of the source image. |
| `dy` | `number` | The y-axis coordinate in the destination canvas at which to place the top-left corner of the source image. |
| `dWidth` | `number` | The width to draw the image in the destination canvas. This allows scaling of the drawn image. If not specified, the image is not scaled in width when drawn. |
| `dHeight` | `number` | The height to draw the image in the destination canvas. This allows scaling of the drawn image. If not specified, the image is not scaled in height when drawn. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:333

▸ **drawImage**(`image`, `dx`, `dy`, `dWidth`, `dHeight`): `void`

Draws the specified image. This method is available in multiple formats, providing a great deal of flexibility in its use.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `image` | `any` | An element to draw into the context. |
| `dx` | `number` | The x-axis coordinate in the destination canvas at which to place the top-left corner of the source image. |
| `dy` | `number` | The y-axis coordinate in the destination canvas at which to place the top-left corner of the source image. |
| `dWidth` | `number` | The width to draw the image in the destination canvas. This allows scaling of the drawn image. If not specified, the image is not scaled in width when drawn. |
| `dHeight` | `number` | The height to draw the image in the destination canvas. This allows scaling of the drawn image. If not specified, the image is not scaled in height when drawn. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:342

▸ **drawImage**(`image`, `dx`, `dy`): `void`

Draws the specified image. This method is available in multiple formats, providing a great deal of flexibility in its use.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `image` | `any` | An element to draw into the context. |
| `dx` | `number` | The x-axis coordinate in the destination canvas at which to place the top-left corner of the source image. |
| `dy` | `number` | The y-axis coordinate in the destination canvas at which to place the top-left corner of the source image. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:350

___

### fill

▸ **fill**(): `void`

Fills the current sub-paths with the current fill style.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:318

___

### fillRect

▸ **fillRect**(`x`, `y`, `width`, `height`): `void`

Draws a filled rectangle at (x, y) position whose size is determined by width and height.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | The x-axis coordinate of the rectangle's starting point. |
| `y` | `number` | The y-axis coordinate of the rectangle's starting point. |
| `width` | `number` | The rectangle's width. Positive values are to the right, and negative to the left. |
| `height` | `number` | The rectangle's height. Positive values are down, and negative are up. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:205

___

### fillText

▸ **fillText**(`text`, `x`, `y`, `maxWidth?`): `void`

Draws (fills) a given text at the given (x, y) position.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `text` | `string` | A String specifying the text string to render into the context. The text is rendered using the settings specified by font, textAlign, textBaseline, and direction. |
| `x` | `number` | The x-axis coordinate of the point at which to begin drawing the text, in pixels. |
| `y` | `number` | The y-axis coordinate of the baseline on which to begin drawing the text, in pixels. |
| `maxWidth?` | `number` | The maximum number of pixels wide the text may be once rendered. If not specified, there is no limit to the width of the text. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:375

___

### getImageData

▸ **getImageData**(`sx`, `sy`, `sw`, `sh`): `ImageData`

Returns an ImageData object representing the underlying pixel data for the area of the canvas denoted by the rectangle which starts at (sx, sy) and has an sw width and sh height.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sx` | `number` | The x-axis coordinate of the top-left corner of the rectangle from which the ImageData will be extracted. |
| `sy` | `number` | The y-axis coordinate of the top-left corner of the rectangle from which the ImageData will be extracted. |
| `sw` | `number` | The width of the rectangle from which the ImageData will be extracted. Positive values are to the right, and negative to the left. |
| `sh` | `number` | The height of the rectangle from which the ImageData will be extracted. Positive values are down, and negative are up. |

#### Returns

`ImageData`

ImageData An ImageData object containing the image data for the rectangle of the canvas specified.

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:360

___

### lineTo

▸ **lineTo**(`x`, `y`): `void`

Connects the last point in the current sub-path to the specified (x, y) coordinates with a straight line.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | The x-axis coordinate of the line's end point. |
| `y` | `number` | The y-axis coordinate of the line's end point. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:292

___

### measureText

▸ **measureText**(`text`): [`ITextMetrics`](ITextMetrics.md)

Returns a TextMetrics object.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `text` | `string` | The text String to measure. |

#### Returns

[`ITextMetrics`](ITextMetrics.md)

ITextMetrics A ITextMetrics object.

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:308

___

### moveTo

▸ **moveTo**(`x`, `y`): `void`

Moves the starting point of a new sub-path to the (x, y) coordinates.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | The x-axis (horizontal) coordinate of the point. |
| `y` | `number` | The y-axis (vertical) coordinate of the point. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:285

___

### putImageData

▸ **putImageData**(`imageData`, `dx`, `dy`): `void`

Paints data from the given ImageData object onto the bitmap. If a dirty rectangle is provided, only the pixels from that rectangle are painted.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `imageData` | `ImageData` | An ImageData object containing the array of pixel values. |
| `dx` | `number` | Horizontal position (x coordinate) at which to place the image data in the destination canvas. |
| `dy` | `number` | Vertical position (y coordinate) at which to place the image data in the destination canvas. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:256

___

### quadraticCurveTo

▸ **quadraticCurveTo**(`cpx`, `cpy`, `x`, `y`): `void`

Adds a quadratic Bézier curve to the current path.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `cpx` | `number` | The x-axis coordinate of the control point. |
| `cpy` | `number` | The y-axis coordinate of the control point. |
| `x` | `number` | The x-axis coordinate of the end point. |
| `y` | `number` | The y-axis coordinate of the end point. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:301

___

### rect

▸ **rect**(`x`, `y`, `width`, `height`): `void`

Creates a path for a rectangle at position (x, y) with a size that is determined by width and height.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | The x-axis coordinate of the rectangle's starting point. |
| `y` | `number` | The y-axis coordinate of the rectangle's starting point. |
| `width` | `number` | The rectangle's width. Positive values are to the right, and negative to the left. |
| `height` | `number` | The rectangle's height. Positive values are down, and negative are up. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:243

___

### restore

▸ **restore**(): `void`

Restores the drawing style state to the last element on the 'state stack' saved by save().

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:196

___

### rotate

▸ **rotate**(`angle`): `void`

Adds a rotation to the transformation matrix. The angle argument represents a clockwise rotation angle and is expressed in radians.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `angle` | `number` | The rotation angle, clockwise in radians. You can use degree * Math.PI / 180 to calculate a radian from a degree. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:218

___

### save

▸ **save**(): `void`

Saves the current drawing style state using a stack so you can revert any change you make to it using restore().

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:191

___

### scale

▸ **scale**(`x`, `y`): `void`

Adds a scaling transformation to the canvas units by x horizontally and by y vertically.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | Scaling factor in the horizontal direction. A negative value flips pixels across the vertical axis. A value of 1 results in no horizontal scaling. |
| `y` | `number` | Scaling factor in the vertical direction. A negative value flips pixels across the horizontal axis. A value of 1 results in no vertical scaling. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:212

___

### setLineDash

▸ **setLineDash**(`segments`): `void`

Sets the current line dash pattern.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `segments` | `number`[] | An Array of numbers that specify distances to alternately draw a line and a gap (in coordinate space units). |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:366

___

### setTransform

▸ **setTransform**(`a`, `b`, `c`, `d`, `e`, `f`): `void`

Resets the current transform to matrix composed with a, b, c, d, e, f.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `a` | `number` | Horizontal scaling. A value of 1 results in no scaling. |
| `b` | `number` | Vertical skewing. |
| `c` | `number` | Horizontal skewing. |
| `d` | `number` | Vertical scaling. A value of 1 results in no scaling. |
| `e` | `number` | Horizontal translation (moving). |
| `f` | `number` | Vertical translation (moving). |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:405

___

### stroke

▸ **stroke**(): `void`

Strokes the current sub-paths with the current stroke style.

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:313

___

### strokeRect

▸ **strokeRect**(`x`, `y`, `width`, `height`): `void`

Paints a rectangle which has a starting point at (x, y) and has a w width and an h height onto the canvas, using the current stroke style.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | The x-axis coordinate of the rectangle's starting point. |
| `y` | `number` | The y-axis coordinate of the rectangle's starting point. |
| `width` | `number` | The rectangle's width. Positive values are to the right, and negative to the left. |
| `height` | `number` | The rectangle's height. Positive values are down, and negative are up. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:234

___

### strokeText

▸ **strokeText**(`text`, `x`, `y`, `maxWidth?`): `void`

Draws (strokes) a given text at the given (x, y) position.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `text` | `string` | A String specifying the text string to render into the context. The text is rendered using the settings specified by font, textAlign, textBaseline, and direction. |
| `x` | `number` | The x-axis coordinate of the point at which to begin drawing the text, in pixels. |
| `y` | `number` | The y-axis coordinate of the baseline on which to begin drawing the text, in pixels. |
| `maxWidth?` | `number` | The maximum number of pixels wide the text may be once rendered. If not specified, there is no limit to the width of the text. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:384

___

### translate

▸ **translate**(`x`, `y`): `void`

Adds a translation transformation by moving the canvas and its origin x horizontally and y vertically on the grid.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | Distance to move in the horizontal direction. Positive values are to the right, and negative to the left. |
| `y` | `number` | Distance to move in the vertical direction. Positive values are down, and negative are up. |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Engines/ICanvas.ts:225
