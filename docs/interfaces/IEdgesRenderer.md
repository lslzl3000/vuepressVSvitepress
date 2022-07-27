[@dev/core](../README.md) / [Exports](../modules.md) / IEdgesRenderer

# Interface: IEdgesRenderer

Defines the minimum contract an Edges renderer should follow.

## Hierarchy

- [`IDisposable`](IDisposable.md)

  ↳ **`IEdgesRenderer`**

## Implemented by

- [`EdgesRenderer`](../classes/EdgesRenderer.md)

## Table of contents

### Properties

- [customInstances](IEdgesRenderer.md#custominstances)
- [isEnabled](IEdgesRenderer.md#isenabled)

### Methods

- [dispose](IEdgesRenderer.md#dispose)
- [isReady](IEdgesRenderer.md#isready)
- [render](IEdgesRenderer.md#render)

## Properties

### customInstances

• **customInstances**: [`SmartArray`](../classes/SmartArray.md)[`Matrix`](../classes/Matrix.md)

List of instances to render in case the source mesh has instances

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:133

___

### isEnabled

• **isEnabled**: `boolean`

Gets or sets a boolean indicating if the edgesRenderer is active

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:117

## Methods

### dispose

▸ **dispose**(): `void`

Releases all held resources

#### Returns

`void`

#### Inherited from

[IDisposable](IDisposable.md).[dispose](IDisposable.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/scene.ts:103

___

### isReady

▸ **isReady**(): `boolean`

Checks whether or not the edges renderer is ready to render.

#### Returns

`boolean`

true if ready, otherwise false.

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:128

___

### render

▸ **render**(): `void`

Renders the edges of the attached mesh,

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Rendering/edgesRenderer.ts:122
