[@dev/core](../README.md) / [Exports](../modules.md) / ComputePressureObserverWrapper

# Class: ComputePressureObserverWrapper

A wrapper for the experimental compute pressure api which allows a callback to be called whenever certain thresholds are met.

## Table of contents

### Constructors

- [constructor](ComputePressureObserverWrapper.md#constructor)

### Properties

- [\_observer](ComputePressureObserverWrapper.md#_observer)

### Accessors

- [IsAvailable](ComputePressureObserverWrapper.md#isavailable)

### Methods

- [observe](ComputePressureObserverWrapper.md#observe)
- [unobserve](ComputePressureObserverWrapper.md#unobserve)

## Constructors

### constructor

• **new ComputePressureObserverWrapper**(`callback`, `thresholds`)

A compute pressure observer will call this callback, whenever these thresholds are met.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callback` | (`update`: [`IComputePressureData`](../interfaces/IComputePressureData.md)) => `void` | The callback that is called whenever thresholds are met. |
| `thresholds` | [`IComputePressureThresholds`](../interfaces/IComputePressureThresholds.md) | An object containing the thresholds used to decide what value to to return for each update property (average of start and end of a threshold boundary). |

#### Defined in

packages/dev/core/src/Misc/computePressure.ts:13

## Properties

### \_observer

• `Private` **\_observer**: `any`

#### Defined in

packages/dev/core/src/Misc/computePressure.ts:7

## Accessors

### IsAvailable

• `Static` `get` **IsAvailable**(): `boolean`

Returns true if ComputePressureObserver is available for use, false otherwise.

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Misc/computePressure.ts:22

## Methods

### observe

▸ **observe**(): `void`

Method that must be called to begin observing changes, and triggering callbacks.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/computePressure.ts:29

___

### unobserve

▸ **unobserve**(): `void`

Method that must be called to stop observing changes and triggering callbacks (cleanup function).

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/computePressure.ts:39
