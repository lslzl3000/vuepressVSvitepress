[@dev/core](../README.md) / [Exports](../modules.md) / ITimerOptions

# Interface: ITimerOptionsT

Construction options for a timer

## Type parameters

| Name |
| :------ |
| `T` |

## Table of contents

### Properties

- [breakCondition](ITimerOptions.md#breakcondition)
- [contextObservable](ITimerOptions.md#contextobservable)
- [observableParameters](ITimerOptions.md#observableparameters)
- [onAborted](ITimerOptions.md#onaborted)
- [onEnded](ITimerOptions.md#onended)
- [onTick](ITimerOptions.md#ontick)
- [timeout](ITimerOptions.md#timeout)

## Properties

### breakCondition

• `Optional` **breakCondition**: (`data?`: [`ITimerData`](ITimerData.md)`T`) => `boolean`

#### Type declaration

▸ (`data?`): `boolean`

An optional break condition that will stop the times prematurely. In this case onEnded will not be triggered!

##### Parameters

| Name | Type |
| :------ | :------ |
| `data?` | [`ITimerData`](ITimerData.md)`T` |

##### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Misc/timer.ts:31

___

### contextObservable

• **contextObservable**: [`Observable`](../classes/Observable.md)`T`

The context observable is used to calculate time deltas and provides the context of the timer's callbacks. Will usually be OnBeforeRenderObservable.
Countdown calculation is done ONLY when the observable is notifying its observers, meaning that if
you choose an observable that doesn't trigger too often, the wait time might extend further than the requested max time

#### Defined in

https://github.com/babylon.js/core/src/Misc/timer.ts:19

___

### observableParameters

• `Optional` **observableParameters**: `Object`

Optional parameters when adding an observer to the observable

#### Type declaration

| Name | Type |
| :------ | :------ |
| `insertFirst?` | `boolean` |
| `mask?` | `number` |
| `scope?` | `any` |

#### Defined in

https://github.com/babylon.js/core/src/Misc/timer.ts:23

___

### onAborted

• `Optional` **onAborted**: (`data`: [`ITimerData`](ITimerData.md)`any`) => `void`

#### Type declaration

▸ (`data`): `void`

Will be triggered when the break condition has met (prematurely ended)

##### Parameters

| Name | Type |
| :------ | :------ |
| `data` | [`ITimerData`](ITimerData.md)`any` |

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/timer.ts:39

___

### onEnded

• `Optional` **onEnded**: (`data`: [`ITimerData`](ITimerData.md)`any`) => `void`

#### Type declaration

▸ (`data`): `void`

Will be triggered when the time condition has met

##### Parameters

| Name | Type |
| :------ | :------ |
| `data` | [`ITimerData`](ITimerData.md)`any` |

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/timer.ts:35

___

### onTick

• `Optional` **onTick**: (`data`: [`ITimerData`](ITimerData.md)`any`) => `void`

#### Type declaration

▸ (`data`): `void`

Optional function to execute on each tick (or count)

##### Parameters

| Name | Type |
| :------ | :------ |
| `data` | [`ITimerData`](ITimerData.md)`any` |

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/timer.ts:43

___

### timeout

• **timeout**: `number`

Time-to-end

#### Defined in

https://github.com/babylon.js/core/src/Misc/timer.ts:13
