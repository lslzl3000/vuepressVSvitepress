[@dev/core](../README.md) / [Exports](../modules.md) / AxesViewer

# Class: AxesViewer

The Axes viewer will show 3 axes in a specific point in space

**`See`**

https://doc.babylonjs.com/toolsAndResources/utilities/World_Axes

## Hierarchy

- **`AxesViewer`**

  ↳ [`BoneAxesViewer`](BoneAxesViewer.md)

## Table of contents

### Constructors

- [constructor](AxesViewer.md#constructor)

### Properties

- [\_instanced](AxesViewer.md#_instanced)
- [\_scaleLinesFactor](AxesViewer.md#_scalelinesfactor)
- [\_xAxis](AxesViewer.md#_xaxis)
- [\_yAxis](AxesViewer.md#_yaxis)
- [\_zAxis](AxesViewer.md#_zaxis)
- [scaleLines](AxesViewer.md#scalelines)
- [scene](AxesViewer.md#scene)

### Accessors

- [xAxis](AxesViewer.md#xaxis)
- [yAxis](AxesViewer.md#yaxis)
- [zAxis](AxesViewer.md#zaxis)

### Methods

- [createInstance](AxesViewer.md#createinstance)
- [dispose](AxesViewer.md#dispose)
- [update](AxesViewer.md#update)
- [\_SetRenderingGroupId](AxesViewer.md#_setrenderinggroupid)

## Constructors

### constructor

• **new AxesViewer**(`scene?`, `scaleLines?`, `renderingGroupId?`, `xAxis?`, `yAxis?`, `zAxis?`, `lineThickness?`)

Creates a new AxesViewer

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `scene?` | [`Scene`](Scene.md) | `undefined` | defines the hosting scene |
| `scaleLines` | `number` | `1` | defines a number used to scale line length (1 by default) |
| `renderingGroupId` | [`Nullable`](../modules.md#nullable)`number` | `2` | defines a number used to set the renderingGroupId of the meshes (2 by default) |
| `xAxis?` | [`TransformNode`](TransformNode.md) | `undefined` | defines the node hierarchy used to render the x-axis |
| `yAxis?` | [`TransformNode`](TransformNode.md) | `undefined` | defines the node hierarchy used to render the y-axis |
| `zAxis?` | [`TransformNode`](TransformNode.md) | `undefined` | defines the node hierarchy used to render the z-axis |
| `lineThickness` | `number` | `1` | The line thickness to use when creating the arrow. defaults to 1. |

#### Defined in

packages/dev/core/src/Debug/axesViewer.ts:56

## Properties

### \_instanced

• `Private` **\_instanced**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Debug/axesViewer.ts:19

___

### \_scaleLinesFactor

• `Private` **\_scaleLinesFactor**: `number` = `4`

#### Defined in

packages/dev/core/src/Debug/axesViewer.ts:18

___

### \_xAxis

• `Private` **\_xAxis**: [`TransformNode`](TransformNode.md)

#### Defined in

packages/dev/core/src/Debug/axesViewer.ts:15

___

### \_yAxis

• `Private` **\_yAxis**: [`TransformNode`](TransformNode.md)

#### Defined in

packages/dev/core/src/Debug/axesViewer.ts:16

___

### \_zAxis

• `Private` **\_zAxis**: [`TransformNode`](TransformNode.md)

#### Defined in

packages/dev/core/src/Debug/axesViewer.ts:17

___

### scaleLines

• **scaleLines**: `number` = `1`

Gets or sets a number used to scale line length

#### Defined in

packages/dev/core/src/Debug/axesViewer.ts:29

___

### scene

• **scene**: [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) = `null`

Gets the hosting scene

#### Defined in

packages/dev/core/src/Debug/axesViewer.ts:24

## Accessors

### xAxis

• `get` **xAxis**(): [`TransformNode`](TransformNode.md)

Gets the node hierarchy used to render x-axis

#### Returns

[`TransformNode`](TransformNode.md)

#### Defined in

packages/dev/core/src/Debug/axesViewer.ts:32

___

### yAxis

• `get` **yAxis**(): [`TransformNode`](TransformNode.md)

Gets the node hierarchy used to render y-axis

#### Returns

[`TransformNode`](TransformNode.md)

#### Defined in

packages/dev/core/src/Debug/axesViewer.ts:37

___

### zAxis

• `get` **zAxis**(): [`TransformNode`](TransformNode.md)

Gets the node hierarchy used to render z-axis

#### Returns

[`TransformNode`](TransformNode.md)

#### Defined in

packages/dev/core/src/Debug/axesViewer.ts:42

## Methods

### createInstance

▸ **createInstance**(): [`AxesViewer`](AxesViewer.md)

Creates an instance of this axes viewer.

#### Returns

[`AxesViewer`](AxesViewer.md)

a new axes viewer with instanced meshes

#### Defined in

packages/dev/core/src/Debug/axesViewer.ts:126

___

### dispose

▸ **dispose**(): `void`

Releases resources

#### Returns

`void`

#### Defined in

packages/dev/core/src/Debug/axesViewer.ts:136

___

### update

▸ **update**(`position`, `xaxis`, `yaxis`, `zaxis`): `void`

Force the viewer to update

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `position` | [`Vector3`](Vector3.md) | defines the position of the viewer |
| `xaxis` | [`Vector3`](Vector3.md) | defines the x axis of the viewer |
| `yaxis` | [`Vector3`](Vector3.md) | defines the y axis of the viewer |
| `zaxis` | [`Vector3`](Vector3.md) | defines the z axis of the viewer |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Debug/axesViewer.ts:108

___

### \_SetRenderingGroupId

▸ `Static` `Private` **_SetRenderingGroupId**(`node`, `id`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `node` | [`TransformNode`](TransformNode.md) |
| `id` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Debug/axesViewer.ts:152
