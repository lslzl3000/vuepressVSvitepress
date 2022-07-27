[@dev/core](../README.md) / [Exports](../modules.md) / IWebXRFeaturePoint

# Interface: IWebXRFeaturePoint

A babylon interface for a "WebXR" feature point.
Represents the position and confidence value of a given feature point.

## Table of contents

### Properties

- [confidenceValue](IWebXRFeaturePoint.md#confidencevalue)
- [position](IWebXRFeaturePoint.md#position)

## Properties

### confidenceValue

• **confidenceValue**: `number`

Represents the confidence value of the feature point in world space. 0 being least confident, and 1 being most confident.

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRFeaturePointSystem.ts:19

___

### position

• **position**: [`Vector3`](../classes/Vector3.md)

Represents the position of the feature point in world space.

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRFeaturePointSystem.ts:15
