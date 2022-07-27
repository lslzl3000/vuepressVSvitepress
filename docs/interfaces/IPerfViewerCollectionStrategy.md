[@dev/core](../README.md) / [Exports](../modules.md) / IPerfViewerCollectionStrategy

# Interface: IPerfViewerCollectionStrategy

Defines the general structure of what is necessary for a collection strategy.

## Table of contents

### Properties

- [dispose](IPerfViewerCollectionStrategy.md#dispose)
- [getData](IPerfViewerCollectionStrategy.md#getdata)
- [id](IPerfViewerCollectionStrategy.md#id)

## Properties

### dispose

• **dispose**: () => `void`

#### Type declaration

▸ (): `void`

Function which does any necessary cleanup. Called when performanceViewerCollector.dispose() is called.

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/PerformanceViewer/performanceViewerCollectionStrategies.ts:21

___

### getData

• **getData**: () => `number`

#### Type declaration

▸ (): `number`

Function which gets the data for the strategy.

##### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/Misc/PerformanceViewer/performanceViewerCollectionStrategies.ts:17

___

### id

• **id**: `string`

The id of the strategy.

#### Defined in

https://github.com/babylon.js/core/src/Misc/PerformanceViewer/performanceViewerCollectionStrategies.ts:13
