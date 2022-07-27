[@dev/core](../README.md) / [Exports](../modules.md) / IComputePressureThresholds

# Interface: IComputePressureThresholds

An interface defining the shape of the thresholds parameter in the experimental compute pressure api

## Table of contents

### Properties

- [cpuSpeedThresholds](IComputePressureThresholds.md#cpuspeedthresholds)
- [cpuUtilizationThresholds](IComputePressureThresholds.md#cpuutilizationthresholds)

## Properties

### cpuSpeedThresholds

• **cpuSpeedThresholds**: `number`[]

Thresholds to make buckets out of for the cpu speed, the average between the start and end points of a threshold will be returned to the callback.
0.5 represents base speed.

#### Defined in

https://github.com/babylon.js/core/src/Misc/computePressure.ts:56

___

### cpuUtilizationThresholds

• **cpuUtilizationThresholds**: `number`[]

Thresholds to make buckets out of for the cpu utilization, the average between the start and end points of a threshold will be returned to the callback.

#### Defined in

https://github.com/babylon.js/core/src/Misc/computePressure.ts:51
