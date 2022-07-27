[@dev/core](../README.md) / [Exports](../modules.md) / BoneAxesViewer

# Class: BoneAxesViewer

The BoneAxesViewer will attach 3 axes to a specific bone of a specific mesh

**`See`**

demo here: https://www.babylonjs-playground.com/#0DE8F4#8

## Hierarchy

- [`AxesViewer`](AxesViewer.md)

  ↳ **`BoneAxesViewer`**

## Table of contents

### Constructors

- [constructor](BoneAxesViewer.md#constructor)

### Properties

- [bone](BoneAxesViewer.md#bone)
- [mesh](BoneAxesViewer.md#mesh)
- [pos](BoneAxesViewer.md#pos)
- [scaleLines](BoneAxesViewer.md#scalelines)
- [scene](BoneAxesViewer.md#scene)
- [xaxis](BoneAxesViewer.md#xaxis)
- [yaxis](BoneAxesViewer.md#yaxis)
- [zaxis](BoneAxesViewer.md#zaxis)

### Accessors

- [xAxis](BoneAxesViewer.md#xaxis-1)
- [yAxis](BoneAxesViewer.md#yaxis-1)
- [zAxis](BoneAxesViewer.md#zaxis-1)

### Methods

- [createInstance](BoneAxesViewer.md#createinstance)
- [dispose](BoneAxesViewer.md#dispose)
- [update](BoneAxesViewer.md#update)

## Constructors

### constructor

• **new BoneAxesViewer**(`scene`, `bone`, `mesh`, `scaleLines?`)

Creates a new BoneAxesViewer

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | `undefined` | defines the hosting scene |
| `bone` | [`Bone`](Bone.md) | `undefined` | defines the target bone |
| `mesh` | [`Mesh`](Mesh.md) | `undefined` | defines the target mesh |
| `scaleLines` | `number` | `1` | defines a scaling factor for line length (1 by default) |

#### Overrides

[AxesViewer](AxesViewer.md).[constructor](AxesViewer.md#constructor)

#### Defined in

packages/dev/core/src/Debug/boneAxesViewer.ts:39

## Properties

### bone

• **bone**: [`Nullable`](../modules.md#nullable)[`Bone`](Bone.md)

Gets or sets the target bone where to display the axes viewer

#### Defined in

packages/dev/core/src/Debug/boneAxesViewer.ts:21

___

### mesh

• **mesh**: [`Nullable`](../modules.md#nullable)[`Mesh`](Mesh.md)

Gets or sets the target mesh where to display the axes viewer

#### Defined in

packages/dev/core/src/Debug/boneAxesViewer.ts:17

___

### pos

• **pos**: [`Vector3`](Vector3.md)

Gets current position

#### Defined in

packages/dev/core/src/Debug/boneAxesViewer.ts:24

___

### scaleLines

• **scaleLines**: `number` = `1`

Gets or sets a number used to scale line length

#### Inherited from

[AxesViewer](AxesViewer.md).[scaleLines](AxesViewer.md#scalelines)

#### Defined in

packages/dev/core/src/Debug/axesViewer.ts:29

___

### scene

• **scene**: [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) = `null`

Gets the hosting scene

#### Inherited from

[AxesViewer](AxesViewer.md).[scene](AxesViewer.md#scene)

#### Defined in

packages/dev/core/src/Debug/axesViewer.ts:24

___

### xaxis

• **xaxis**: [`Vector3`](Vector3.md)

Gets direction of X axis

#### Defined in

packages/dev/core/src/Debug/boneAxesViewer.ts:26

___

### yaxis

• **yaxis**: [`Vector3`](Vector3.md)

Gets direction of Y axis

#### Defined in

packages/dev/core/src/Debug/boneAxesViewer.ts:28

___

### zaxis

• **zaxis**: [`Vector3`](Vector3.md)

Gets direction of Z axis

#### Defined in

packages/dev/core/src/Debug/boneAxesViewer.ts:30

## Accessors

### xAxis

• `get` **xAxis**(): [`TransformNode`](TransformNode.md)

Gets the node hierarchy used to render x-axis

#### Returns

[`TransformNode`](TransformNode.md)

#### Inherited from

AxesViewer.xAxis

#### Defined in

packages/dev/core/src/Debug/axesViewer.ts:32

___

### yAxis

• `get` **yAxis**(): [`TransformNode`](TransformNode.md)

Gets the node hierarchy used to render y-axis

#### Returns

[`TransformNode`](TransformNode.md)

#### Inherited from

AxesViewer.yAxis

#### Defined in

packages/dev/core/src/Debug/axesViewer.ts:37

___

### zAxis

• `get` **zAxis**(): [`TransformNode`](TransformNode.md)

Gets the node hierarchy used to render z-axis

#### Returns

[`TransformNode`](TransformNode.md)

#### Inherited from

AxesViewer.zAxis

#### Defined in

packages/dev/core/src/Debug/axesViewer.ts:42

## Methods

### createInstance

▸ **createInstance**(): [`AxesViewer`](AxesViewer.md)

Creates an instance of this axes viewer.

#### Returns

[`AxesViewer`](AxesViewer.md)

a new axes viewer with instanced meshes

#### Inherited from

[AxesViewer](AxesViewer.md).[createInstance](AxesViewer.md#createinstance)

#### Defined in

packages/dev/core/src/Debug/axesViewer.ts:126

___

### dispose

▸ **dispose**(): `void`

Releases resources

#### Returns

`void`

#### Overrides

[AxesViewer](AxesViewer.md).[dispose](AxesViewer.md#dispose)

#### Defined in

packages/dev/core/src/Debug/boneAxesViewer.ts:64

___

### update

▸ **update**(): `void`

Force the viewer to update

#### Returns

`void`

#### Overrides

[AxesViewer](AxesViewer.md).[update](AxesViewer.md#update)

#### Defined in

packages/dev/core/src/Debug/boneAxesViewer.ts:49
