[@dev/core](../README.md) / [Exports](../modules.md) / NodeMaterialOptimizer

# Class: NodeMaterialOptimizer

Root class for all node material optimizers

## Table of contents

### Constructors

- [constructor](NodeMaterialOptimizer.md#constructor)

### Methods

- [optimize](NodeMaterialOptimizer.md#optimize)

## Constructors

### constructor

• **new NodeMaterialOptimizer**()

## Methods

### optimize

▸ **optimize**(`_vertexOutputNodes`, `_fragmentOutputNodes`): `void`

Function used to optimize a NodeMaterial graph

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `_vertexOutputNodes` | [`NodeMaterialBlock`](NodeMaterialBlock.md)[] | defines the list of output nodes for the vertex shader |
| `_fragmentOutputNodes` | [`NodeMaterialBlock`](NodeMaterialBlock.md)[] | defines the list of output nodes for the fragment shader |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/Optimizers/nodeMaterialOptimizer.ts:12
