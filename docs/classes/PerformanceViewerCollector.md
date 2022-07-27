[@dev/core](../README.md) / [Exports](../modules.md) / PerformanceViewerCollector

# Class: PerformanceViewerCollector

The collector class handles the collection and storage of data into the appropriate array.
The collector also handles notifying any observers of any updates.

## Table of contents

### Constructors

- [constructor](PerformanceViewerCollector.md#constructor)

### Properties

- [\_customEventObservable](PerformanceViewerCollector.md#_customeventobservable)
- [\_datasetMeta](PerformanceViewerCollector.md#_datasetmeta)
- [\_eventRestoreSet](PerformanceViewerCollector.md#_eventrestoreset)
- [\_hasLoadedData](PerformanceViewerCollector.md#_hasloadeddata)
- [\_isStarted](PerformanceViewerCollector.md#_isstarted)
- [\_startingTimestamp](PerformanceViewerCollector.md#_startingtimestamp)
- [\_strategies](PerformanceViewerCollector.md#_strategies)
- [datasetObservable](PerformanceViewerCollector.md#datasetobservable)
- [datasets](PerformanceViewerCollector.md#datasets)
- [metadataObservable](PerformanceViewerCollector.md#metadataobservable)

### Accessors

- [hasLoadedData](PerformanceViewerCollector.md#hasloadeddata)
- [isStarted](PerformanceViewerCollector.md#isstarted)
- [NumberOfPointsOffset](PerformanceViewerCollector.md#numberofpointsoffset)
- [SliceDataOffset](PerformanceViewerCollector.md#slicedataoffset)

### Methods

- [\_collectDataAtFrame](PerformanceViewerCollector.md#_collectdataatframe)
- [\_getHexColorFromId](PerformanceViewerCollector.md#_gethexcolorfromid)
- [\_restoreStringEvents](PerformanceViewerCollector.md#_restorestringevents)
- [addCollectionStrategies](PerformanceViewerCollector.md#addcollectionstrategies)
- [clear](PerformanceViewerCollector.md#clear)
- [dispose](PerformanceViewerCollector.md#dispose)
- [exportDataToCsv](PerformanceViewerCollector.md#exportdatatocsv)
- [getCurrentSlice](PerformanceViewerCollector.md#getcurrentslice)
- [loadFromFileData](PerformanceViewerCollector.md#loadfromfiledata)
- [registerEvent](PerformanceViewerCollector.md#registerevent)
- [sendEvent](PerformanceViewerCollector.md#sendevent)
- [start](PerformanceViewerCollector.md#start)
- [stop](PerformanceViewerCollector.md#stop)
- [updateMetadata](PerformanceViewerCollector.md#updatemetadata)

## Constructors

### constructor

• **new PerformanceViewerCollector**(`_scene`, `_enabledStrategyCallbacks?`)

Handles the creation of a performance viewer collector.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `_scene` | [`Scene`](Scene.md) | the scene to collect on. |
| `_enabledStrategyCallbacks?` | `IPerformanceViewerStrategyParameter`[] | the list of data to collect with callbacks for initialization purposes. |

#### Defined in

packages/dev/core/src/Misc/PerformanceViewer/performanceViewerCollector.ts:94

## Properties

### \_customEventObservable

• `Private` `Readonly` **\_customEventObservable**: [`Observable`](Observable.md)[`IPerfCustomEvent`](../interfaces/IPerfCustomEvent.md)

#### Defined in

packages/dev/core/src/Misc/PerformanceViewer/performanceViewerCollector.ts:58

___

### \_datasetMeta

• `Private` **\_datasetMeta**: `Map``string`, [`IPerfMetadata`](../interfaces/IPerfMetadata.md)

#### Defined in

packages/dev/core/src/Misc/PerformanceViewer/performanceViewerCollector.ts:53

___

### \_eventRestoreSet

• `Private` `Readonly` **\_eventRestoreSet**: `Set``string`

#### Defined in

packages/dev/core/src/Misc/PerformanceViewer/performanceViewerCollector.ts:59

___

### \_hasLoadedData

• `Private` **\_hasLoadedData**: `boolean`

#### Defined in

packages/dev/core/src/Misc/PerformanceViewer/performanceViewerCollector.ts:56

___

### \_isStarted

• `Private` **\_isStarted**: `boolean`

#### Defined in

packages/dev/core/src/Misc/PerformanceViewer/performanceViewerCollector.ts:57

___

### \_startingTimestamp

• `Private` **\_startingTimestamp**: `number`

#### Defined in

packages/dev/core/src/Misc/PerformanceViewer/performanceViewerCollector.ts:55

___

### \_strategies

• `Private` **\_strategies**: `Map``string`, [`IPerfViewerCollectionStrategy`](../interfaces/IPerfViewerCollectionStrategy.md)

#### Defined in

packages/dev/core/src/Misc/PerformanceViewer/performanceViewerCollector.ts:54

___

### datasetObservable

• `Readonly` **datasetObservable**: [`Observable`](Observable.md)`number`[]

An observable you can attach to get deltas in the dataset. Subscribing to this will increase memory consumption slightly, and may hurt performance due to increased garbage collection needed.
Updates of slices will be of the form [timestamp, numberOfPoints, value1, value2...].

#### Defined in

packages/dev/core/src/Misc/PerformanceViewer/performanceViewerCollector.ts:69

___

### datasets

• `Readonly` **datasets**: [`IPerfDatasets`](../interfaces/IPerfDatasets.md)

Datastructure containing the collected datasets. Warning: you should not modify the values in here, data will be of the form [timestamp, numberOfPoints, value1, value2..., timestamp, etc...]

#### Defined in

packages/dev/core/src/Misc/PerformanceViewer/performanceViewerCollector.ts:64

___

### metadataObservable

• `Readonly` **metadataObservable**: [`Observable`](Observable.md)`Map``string`, [`IPerfMetadata`](../interfaces/IPerfMetadata.md)

An observable you can attach to get the most updated map of metadatas.

#### Defined in

packages/dev/core/src/Misc/PerformanceViewer/performanceViewerCollector.ts:73

## Accessors

### hasLoadedData

• `get` **hasLoadedData**(): `boolean`

Accessor which lets the caller know if the performance collector has data loaded from a file or not!
Call clear() to reset this value.

#### Returns

`boolean`

true if the data is loaded from a file, false otherwise.

#### Defined in

packages/dev/core/src/Misc/PerformanceViewer/performanceViewerCollector.ts:358

___

### isStarted

• `get` **isStarted**(): `boolean`

Returns if the perf collector has been started or not.

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Misc/PerformanceViewer/performanceViewerCollector.ts:525

___

### NumberOfPointsOffset

• `Static` `get` **NumberOfPointsOffset**(): `number`

The offset for the value of the number of points inside a slice.

#### Returns

`number`

#### Defined in

packages/dev/core/src/Misc/PerformanceViewer/performanceViewerCollector.ts:85

___

### SliceDataOffset

• `Static` `get` **SliceDataOffset**(): `number`

The offset for when actual data values start appearing inside a slice.

#### Returns

`number`

#### Defined in

packages/dev/core/src/Misc/PerformanceViewer/performanceViewerCollector.ts:78

## Methods

### \_collectDataAtFrame

▸ `Private` **_collectDataAtFrame**(): `void`

Collects data for every dataset by using the appropriate strategy. This is called every frame.
This method will then notify all observers with the latest slice.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/PerformanceViewer/performanceViewerCollector.ts:247

___

### \_getHexColorFromId

▸ `Private` **_getHexColorFromId**(`id`): `string`

Gets a 6 character hexcode representing the colour from a passed in string.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | the string to get a hex code for. |

#### Returns

`string`

a hexcode hashed from the id.

#### Defined in

packages/dev/core/src/Misc/PerformanceViewer/performanceViewerCollector.ts:225

___

### \_restoreStringEvents

▸ `Private` **_restoreStringEvents**(): `void`

This event restores all custom string events if necessary.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/PerformanceViewer/performanceViewerCollector.ts:181

___

### addCollectionStrategies

▸ **addCollectionStrategies**(...`strategyCallbacks`): `void`

This method adds additional collection strategies for data collection purposes.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `...strategyCallbacks` | `IPerformanceViewerStrategyParameter`[] | the list of data to collect with callbacks. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/PerformanceViewer/performanceViewerCollector.ts:193

___

### clear

▸ **clear**(`preserveStringEventsRestore?`): `void`

Completely clear, data, ids, and strategies saved to this performance collector.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `preserveStringEventsRestore?` | `boolean` | if it should preserve the string events, by default will clear string events registered when called. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/PerformanceViewer/performanceViewerCollector.ts:339

___

### dispose

▸ **dispose**(): `void`

Disposes of the object

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/PerformanceViewer/performanceViewerCollector.ts:532

___

### exportDataToCsv

▸ **exportDataToCsv**(): `void`

Exports the datasets inside of the collector to a csv.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/PerformanceViewer/performanceViewerCollector.ts:460

___

### getCurrentSlice

▸ **getCurrentSlice**(): `void`

Collects and then sends the latest slice to any observers by using the appropriate strategy when the user wants.
The slice will be of the form [timestamp, numberOfPoints, value1, value2...]
This method does not add onto the collected data accessible via the datasets variable.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/PerformanceViewer/performanceViewerCollector.ts:294

___

### loadFromFileData

▸ **loadFromFileData**(`data`, `keepDatasetMeta?`): `boolean`

Given a string containing file data, this function parses the file data into the datasets object.
It returns a boolean to indicate if this object was successfully loaded with the data.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `string` | string content representing the file data. |
| `keepDatasetMeta?` | `boolean` | if it should use reuse the existing dataset metadata |

#### Returns

`boolean`

true if the data was successfully loaded, false otherwise.

#### Defined in

packages/dev/core/src/Misc/PerformanceViewer/performanceViewerCollector.ts:369

___

### registerEvent

▸ **registerEvent**(`name`, `forceUpdate?`, `category?`): `undefined` \| [`IPerfCustomEvent`](../interfaces/IPerfCustomEvent.md)

Registers a custom string event which will be callable via sendEvent. This method returns an event object which will contain the id of the event.
The user can set a value optionally, which will be used in the sendEvent method. If the value is set, we will record this value at the end of each frame,
if not we will increment our counter and record the value of the counter at the end of each frame. The value recorded is 0 if no sendEvent method is called, within a frame.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | The name of the event to register |
| `forceUpdate?` | `boolean` | if the code should force add an event, and replace the last one. |
| `category?` | `string` | the category for that event |

#### Returns

`undefined` \| [`IPerfCustomEvent`](../interfaces/IPerfCustomEvent.md)

The event registered, used in sendEvent

#### Defined in

packages/dev/core/src/Misc/PerformanceViewer/performanceViewerCollector.ts:120

___

### sendEvent

▸ **sendEvent**(`event`): `void`

Lets the perf collector handle an event, occurences or event value depending on if the event.value params is set.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `event` | [`IPerfCustomEvent`](../interfaces/IPerfCustomEvent.md) | the event to handle an occurence for |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/PerformanceViewer/performanceViewerCollector.ts:174

___

### start

▸ **start**(`shouldPreserve?`): `void`

Starts the realtime collection of data.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `shouldPreserve?` | `boolean` | optional boolean param, if set will preserve the dataset between calls of start. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/PerformanceViewer/performanceViewerCollector.ts:501

___

### stop

▸ **stop**(): `void`

Stops the collection of data.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/PerformanceViewer/performanceViewerCollector.ts:517

___

### updateMetadata

▸ **updateMetadata**`T`(`id`, `prop`, `value`): `void`

Updates a property for a dataset's metadata with the value provided.

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends keyof [`IPerfMetadata`](../interfaces/IPerfMetadata.md) |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | the id of the dataset which needs its metadata updated. |
| `prop` | `T` | the property to update. |
| `value` | [`IPerfMetadata`](../interfaces/IPerfMetadata.md)[`T`] | the value to update the property with. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/PerformanceViewer/performanceViewerCollector.ts:323
