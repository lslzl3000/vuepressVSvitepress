[@dev/core](../README.md) / [Exports](../modules.md) / IWebXRAnchor

# Interface: IWebXRAnchor

A babylon container for an XR Anchor

## Table of contents

### Properties

- [attachedNode](IWebXRAnchor.md#attachednode)
- [id](IWebXRAnchor.md#id)
- [transformationMatrix](IWebXRAnchor.md#transformationmatrix)
- [xrAnchor](IWebXRAnchor.md#xranchor)

### Methods

- [remove](IWebXRAnchor.md#remove)

## Properties

### attachedNode

• `Optional` **attachedNode**: [`TransformNode`](../classes/TransformNode.md)

if defined, this object will be constantly updated by the anchor's position and rotation

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRAnchorSystem.ts:46

___

### id

• **id**: `number`

A babylon-assigned ID for this anchor

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRAnchorSystem.ts:33

___

### transformationMatrix

• **transformationMatrix**: [`Matrix`](../classes/Matrix.md)

Transformation matrix to apply to an object attached to this anchor

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRAnchorSystem.ts:37

___

### xrAnchor

• **xrAnchor**: `XRAnchor`

The native anchor object

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRAnchorSystem.ts:41

## Methods

### remove

▸ **remove**(): `void`

Remove this anchor from the scene

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRAnchorSystem.ts:51
