[@dev/core](../README.md) / [Exports](../modules.md) / PerfCounter

# Class: PerfCounter

This class is used to track a performance counter which is number based.
The user has access to many properties which give statistics of different nature.

The implementer can track two kinds of Performance Counter: time and count.
For time you can optionally call fetchNewFrame() to notify the start of a new frame to monitor, then call beginMonitoring() to start and endMonitoring() to record the lapsed time. endMonitoring takes a newFrame parameter for you to specify if the monitored time should be set for a new frame or accumulated to the current frame being monitored.
For count you first have to call fetchNewFrame() to notify the start of a new frame to monitor, then call addCount() how many time required to increment the count value you monitor.

## Table of contents

### Constructors

- [constructor](PerfCounter.md#constructor)

### Properties

- [\_average](PerfCounter.md#_average)
- [\_current](PerfCounter.md#_current)
- [\_lastSecAccumulated](PerfCounter.md#_lastsecaccumulated)
- [\_lastSecAverage](PerfCounter.md#_lastsecaverage)
- [\_lastSecTime](PerfCounter.md#_lastsectime)
- [\_lastSecValueCount](PerfCounter.md#_lastsecvaluecount)
- [\_max](PerfCounter.md#_max)
- [\_min](PerfCounter.md#_min)
- [\_startMonitoringTime](PerfCounter.md#_startmonitoringtime)
- [\_totalAccumulated](PerfCounter.md#_totalaccumulated)
- [\_totalValueCount](PerfCounter.md#_totalvaluecount)
- [Enabled](PerfCounter.md#enabled)

### Accessors

- [average](PerfCounter.md#average)
- [count](PerfCounter.md#count)
- [current](PerfCounter.md#current)
- [lastSecAverage](PerfCounter.md#lastsecaverage)
- [max](PerfCounter.md#max)
- [min](PerfCounter.md#min)
- [total](PerfCounter.md#total)

### Methods

- [\_fetchResult](PerfCounter.md#_fetchresult)
- [addCount](PerfCounter.md#addcount)
- [beginMonitoring](PerfCounter.md#beginmonitoring)
- [endMonitoring](PerfCounter.md#endmonitoring)
- [fetchNewFrame](PerfCounter.md#fetchnewframe)

## Constructors

### constructor

• **new PerfCounter**()

Creates a new counter

#### Defined in

packages/dev/core/src/Misc/perfCounter.ts:69

## Properties

### \_average

• `Private` **\_average**: `number`

#### Defined in

packages/dev/core/src/Misc/perfCounter.ts:161

___

### \_current

• `Private` **\_current**: `number`

#### Defined in

packages/dev/core/src/Misc/perfCounter.ts:162

___

### \_lastSecAccumulated

• `Private` **\_lastSecAccumulated**: `number`

#### Defined in

packages/dev/core/src/Misc/perfCounter.ts:166

___

### \_lastSecAverage

• `Private` **\_lastSecAverage**: `number`

#### Defined in

packages/dev/core/src/Misc/perfCounter.ts:165

___

### \_lastSecTime

• `Private` **\_lastSecTime**: `number`

#### Defined in

packages/dev/core/src/Misc/perfCounter.ts:167

___

### \_lastSecValueCount

• `Private` **\_lastSecValueCount**: `number`

#### Defined in

packages/dev/core/src/Misc/perfCounter.ts:168

___

### \_max

• `Private` **\_max**: `number`

#### Defined in

packages/dev/core/src/Misc/perfCounter.ts:160

___

### \_min

• `Private` **\_min**: `number`

#### Defined in

packages/dev/core/src/Misc/perfCounter.ts:159

___

### \_startMonitoringTime

• `Private` **\_startMonitoringTime**: `number`

#### Defined in

packages/dev/core/src/Misc/perfCounter.ts:158

___

### \_totalAccumulated

• `Private` **\_totalAccumulated**: `number`

#### Defined in

packages/dev/core/src/Misc/perfCounter.ts:164

___

### \_totalValueCount

• `Private` **\_totalValueCount**: `number`

#### Defined in

packages/dev/core/src/Misc/perfCounter.ts:163

___

### Enabled

▪ `Static` **Enabled**: `boolean` = `true`

Gets or sets a global boolean to turn on and off all the counters

#### Defined in

packages/dev/core/src/Misc/perfCounter.ts:15

## Accessors

### average

• `get` **average**(): `number`

Returns the average value since the performance counter is running

#### Returns

`number`

#### Defined in

packages/dev/core/src/Misc/perfCounter.ts:34

___

### count

• `get` **count**(): `number`

Gets the total value count

#### Returns

`number`

#### Defined in

packages/dev/core/src/Misc/perfCounter.ts:62

___

### current

• `get` **current**(): `number`

Returns the current value

#### Returns

`number`

#### Defined in

packages/dev/core/src/Misc/perfCounter.ts:48

___

### lastSecAverage

• `get` **lastSecAverage**(): `number`

Returns the average value of the last second the counter was monitored

#### Returns

`number`

#### Defined in

packages/dev/core/src/Misc/perfCounter.ts:41

___

### max

• `get` **max**(): `number`

Returns the biggest value ever

#### Returns

`number`

#### Defined in

packages/dev/core/src/Misc/perfCounter.ts:27

___

### min

• `get` **min**(): `number`

Returns the smallest value ever

#### Returns

`number`

#### Defined in

packages/dev/core/src/Misc/perfCounter.ts:20

___

### total

• `get` **total**(): `number`

Gets the accumulated total

#### Returns

`number`

#### Defined in

packages/dev/core/src/Misc/perfCounter.ts:55

## Methods

### \_fetchResult

▸ `Private` **_fetchResult**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/perfCounter.ts:139

___

### addCount

▸ **addCount**(`newCount`, `fetchResult`): `void`

Call this method to monitor a count of something (e.g. mesh drawn in viewport count)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newCount` | `number` | the count value to add to the monitored count |
| `fetchResult` | `boolean` | true when it's the last time in the frame you add to the counter and you wish to update the statistics properties (min/max/average), false if you only want to update statistics. |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/perfCounter.ts:98

___

### beginMonitoring

▸ **beginMonitoring**(): `void`

Start monitoring this performance counter

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/perfCounter.ts:111

___

### endMonitoring

▸ **endMonitoring**(`newFrame?`): `void`

Compute the time lapsed since the previous beginMonitoring() call.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `newFrame` | `boolean` | `true` | true by default to fetch the result and monitor a new frame, if false the time monitored will be added to the current frame counter |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/perfCounter.ts:122

___

### fetchNewFrame

▸ **fetchNewFrame**(): `void`

Call this method to start monitoring a new frame.
This scenario is typically used when you accumulate monitoring time many times for a single frame, you call this method at the start of the frame, then beginMonitoring to start recording and endMonitoring(false) to accumulated the recorded time to the PerfCounter or addCount() to accumulate a monitored count.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/perfCounter.ts:87
