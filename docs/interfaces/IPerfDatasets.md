[@dev/core](../README.md) / [Exports](../modules.md) / IPerfDatasets

# Interface: IPerfDatasets

Defines the shape of a collection of datasets that our graphing service uses for drawing purposes.

## Table of contents

### Properties

- [data](IPerfDatasets.md#data)
- [ids](IPerfDatasets.md#ids)
- [startingIndices](IPerfDatasets.md#startingindices)

## Properties

### data

• **data**: [`DynamicFloat32Array`](../classes/DynamicFloat32Array.md)

The data to be processed by the performance graph. Each slice will be of the form of [timestamp, numberOfPoints, value1, value2...]

#### Defined in

https://github.com/babylon.js/core/src/Misc/interfaces/iPerfViewer.ts:15

___

### ids

• **ids**: `string`[]

The ids of our dataset.

#### Defined in

https://github.com/babylon.js/core/src/Misc/interfaces/iPerfViewer.ts:10

___

### startingIndices

• **startingIndices**: [`DynamicFloat32Array`](../classes/DynamicFloat32Array.md)

A list of starting indices for each slice of data collected. Used for fast access of an arbitrary slice inside the data array.

#### Defined in

https://github.com/babylon.js/core/src/Misc/interfaces/iPerfViewer.ts:20
