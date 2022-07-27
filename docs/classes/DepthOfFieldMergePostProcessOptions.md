[@dev/core](../README.md) / [Exports](../modules.md) / DepthOfFieldMergePostProcessOptions

# Class: DepthOfFieldMergePostProcessOptions

Options to be set when merging outputs from the default pipeline.

## Table of contents

### Constructors

- [constructor](DepthOfFieldMergePostProcessOptions.md#constructor)

### Properties

- [bloom](DepthOfFieldMergePostProcessOptions.md#bloom)
- [depthOfField](DepthOfFieldMergePostProcessOptions.md#depthoffield)
- [originalFromInput](DepthOfFieldMergePostProcessOptions.md#originalfrominput)

## Constructors

### constructor

• **new DepthOfFieldMergePostProcessOptions**()

## Properties

### bloom

• `Optional` **bloom**: `Object`

Parameters to perform the merge of bloom effect

#### Type declaration

| Name | Type |
| :------ | :------ |
| `blurred` | [`PostProcess`](PostProcess.md) |
| `weight` | `number` |

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/depthOfFieldMergePostProcess.ts:29

___

### depthOfField

• `Optional` **depthOfField**: `Object`

Parameters to perform the merge of the depth of field effect

#### Type declaration

| Name | Type |
| :------ | :------ |
| `blurSteps` | [`PostProcess`](PostProcess.md)[] |
| `circleOfConfusion` | [`PostProcess`](PostProcess.md) |

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/depthOfFieldMergePostProcess.ts:22

___

### originalFromInput

• **originalFromInput**: [`PostProcess`](PostProcess.md)

The original image to merge on top of

#### Defined in

https://github.com/babylon.js/core/src/PostProcesses/depthOfFieldMergePostProcess.ts:18
