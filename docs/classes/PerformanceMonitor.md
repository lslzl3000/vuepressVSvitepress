[@dev/core](../README.md) / [Exports](../modules.md) / PerformanceMonitor

# Class: PerformanceMonitor

Performance monitor tracks rolling average frame-time and frame-time variance over a user defined sliding-window

## Table of contents

### Constructors

- [constructor](PerformanceMonitor.md#constructor)

### Properties

- [\_enabled](PerformanceMonitor.md#_enabled)
- [\_lastFrameTimeMs](PerformanceMonitor.md#_lastframetimems)
- [\_rollingFrameTime](PerformanceMonitor.md#_rollingframetime)

### Accessors

- [averageFPS](PerformanceMonitor.md#averagefps)
- [averageFrameTime](PerformanceMonitor.md#averageframetime)
- [averageFrameTimeVariance](PerformanceMonitor.md#averageframetimevariance)
- [instantaneousFPS](PerformanceMonitor.md#instantaneousfps)
- [instantaneousFrameTime](PerformanceMonitor.md#instantaneousframetime)
- [isEnabled](PerformanceMonitor.md#isenabled)
- [isSaturated](PerformanceMonitor.md#issaturated)

### Methods

- [disable](PerformanceMonitor.md#disable)
- [enable](PerformanceMonitor.md#enable)
- [reset](PerformanceMonitor.md#reset)
- [sampleFrame](PerformanceMonitor.md#sampleframe)

## Constructors

### constructor

• **new PerformanceMonitor**(`frameSampleSize?`)

constructor

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `frameSampleSize` | `number` | `30` | The number of samples required to saturate the sliding window |

#### Defined in

packages/dev/core/src/Misc/performanceMonitor.ts:16

## Properties

### \_enabled

• `Private` **\_enabled**: `boolean` = `true`

#### Defined in

packages/dev/core/src/Misc/performanceMonitor.ts:8

___

### \_lastFrameTimeMs

• `Private` **\_lastFrameTimeMs**: [`Nullable`](../modules.md#nullable)`number`

#### Defined in

packages/dev/core/src/Misc/performanceMonitor.ts:10

___

### \_rollingFrameTime

• `Private` **\_rollingFrameTime**: [`RollingAverage`](RollingAverage.md)

#### Defined in

packages/dev/core/src/Misc/performanceMonitor.ts:9

## Accessors

### averageFPS

• `get` **averageFPS**(): `number`

Returns the average framerate in frames per second over the sliding window (or the subset of frames sampled so far)

#### Returns

`number`

#### Defined in

packages/dev/core/src/Misc/performanceMonitor.ts:61

___

### averageFrameTime

• `get` **averageFrameTime**(): `number`

Returns the average frame time in milliseconds over the sliding window (or the subset of frames sampled so far)

#### Returns

`number`

#### Defined in

packages/dev/core/src/Misc/performanceMonitor.ts:40

___

### averageFrameTimeVariance

• `get` **averageFrameTimeVariance**(): `number`

Returns the variance frame time in milliseconds over the sliding window (or the subset of frames sampled so far)

#### Returns

`number`

#### Defined in

packages/dev/core/src/Misc/performanceMonitor.ts:47

___

### instantaneousFPS

• `get` **instantaneousFPS**(): `number`

Returns the average framerate in frames per second using the most recent frame time

#### Returns

`number`

#### Defined in

packages/dev/core/src/Misc/performanceMonitor.ts:68

___

### instantaneousFrameTime

• `get` **instantaneousFrameTime**(): `number`

Returns the frame time of the most recent frame

#### Returns

`number`

#### Defined in

packages/dev/core/src/Misc/performanceMonitor.ts:54

___

### isEnabled

• `get` **isEnabled**(): `boolean`

Returns true if sampling is enabled

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Misc/performanceMonitor.ts:105

___

### isSaturated

• `get` **isSaturated**(): `boolean`

Returns true if enough samples have been taken to completely fill the sliding window

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Misc/performanceMonitor.ts:81

## Methods

### disable

▸ **disable**(): `void`

Disables contributions to the sliding window sample set
Samples will not be interpolated over the disabled period

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/performanceMonitor.ts:96

___

### enable

▸ **enable**(): `void`

Enables contributions to the sliding window sample set

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/performanceMonitor.ts:88

___

### reset

▸ **reset**(): `void`

Resets performance monitor

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/performanceMonitor.ts:112

___

### sampleFrame

▸ **sampleFrame**(`timeMs?`): `void`

Samples current frame

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `timeMs` | `number` | `PrecisionDate.Now` | A timestamp in milliseconds of the current frame to compare with other frames |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/performanceMonitor.ts:24
