[@dev/core](../README.md) / [Exports](../modules.md) / AdvancedTimer

# Class: AdvancedTimerT

An advanced implementation of a timer class

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | `any` |

## Implements

- [`IDisposable`](../interfaces/IDisposable.md)

## Table of contents

### Constructors

- [constructor](AdvancedTimer.md#constructor)

### Properties

- [\_breakCondition](AdvancedTimer.md#_breakcondition)
- [\_breakOnNextTick](AdvancedTimer.md#_breakonnexttick)
- [\_contextObservable](AdvancedTimer.md#_contextobservable)
- [\_observableParameters](AdvancedTimer.md#_observableparameters)
- [\_observer](AdvancedTimer.md#_observer)
- [\_startTime](AdvancedTimer.md#_starttime)
- [\_state](AdvancedTimer.md#_state)
- [\_timeToEnd](AdvancedTimer.md#_timetoend)
- [\_timer](AdvancedTimer.md#_timer)
- [onEachCountObservable](AdvancedTimer.md#oneachcountobservable)
- [onStateChangedObservable](AdvancedTimer.md#onstatechangedobservable)
- [onTimerAbortedObservable](AdvancedTimer.md#ontimerabortedobservable)
- [onTimerEndedObservable](AdvancedTimer.md#ontimerendedobservable)

### Accessors

- [breakCondition](AdvancedTimer.md#breakcondition)

### Methods

- [\_setState](AdvancedTimer.md#_setstate)
- [\_stop](AdvancedTimer.md#_stop)
- [\_tick](AdvancedTimer.md#_tick)
- [clearObservables](AdvancedTimer.md#clearobservables)
- [dispose](AdvancedTimer.md#dispose)
- [start](AdvancedTimer.md#start)
- [stop](AdvancedTimer.md#stop)

## Constructors

### constructor

• **new AdvancedTimer**`T`(`options`)

Will construct a new advanced timer based on the options provided. Timer will not start until start() is called.

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | `any` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | [`ITimerOptions`](../interfaces/ITimerOptions.md)`T` | construction options for this advanced timer |

#### Defined in

packages/dev/core/src/Misc/timer.ts:167

## Properties

### \_breakCondition

• `Private` **\_breakCondition**: (`data`: [`ITimerData`](../interfaces/ITimerData.md)`T`) => `boolean`

#### Type declaration

▸ (`data`): `boolean`

##### Parameters

| Name | Type |
| :------ | :------ |
| `data` | [`ITimerData`](../interfaces/ITimerData.md)`T` |

##### Returns

`boolean`

#### Defined in

packages/dev/core/src/Misc/timer.ts:159

___

### \_breakOnNextTick

• `Private` **\_breakOnNextTick**: `boolean` = `false`

#### Defined in

packages/dev/core/src/Misc/timer.ts:161

___

### \_contextObservable

• `Private` **\_contextObservable**: [`Observable`](Observable.md)`T`

#### Defined in

packages/dev/core/src/Misc/timer.ts:150

___

### \_observableParameters

• `Private` **\_observableParameters**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `insertFirst?` | `boolean` |
| `mask?` | `number` |
| `scope?` | `any` |

#### Defined in

packages/dev/core/src/Misc/timer.ts:151

___

### \_observer

• `Private` **\_observer**: [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)`T` = `null`

#### Defined in

packages/dev/core/src/Misc/timer.ts:149

___

### \_startTime

• `Private` **\_startTime**: `number`

#### Defined in

packages/dev/core/src/Misc/timer.ts:156

___

### \_state

• `Private` **\_state**: [`TimerState`](../enums/TimerState.md)

#### Defined in

packages/dev/core/src/Misc/timer.ts:158

___

### \_timeToEnd

• `Private` **\_timeToEnd**: `number`

#### Defined in

packages/dev/core/src/Misc/timer.ts:160

___

### \_timer

• `Private` **\_timer**: `number`

#### Defined in

packages/dev/core/src/Misc/timer.ts:157

___

### onEachCountObservable

• **onEachCountObservable**: [`Observable`](Observable.md)[`ITimerData`](../interfaces/ITimerData.md)`T`

Will notify each time the timer calculates the remaining time

#### Defined in

packages/dev/core/src/Misc/timer.ts:135

___

### onStateChangedObservable

• **onStateChangedObservable**: [`Observable`](Observable.md)[`TimerState`](../enums/TimerState.md)

Will trigger when the timer state has changed

#### Defined in

packages/dev/core/src/Misc/timer.ts:147

___

### onTimerAbortedObservable

• **onTimerAbortedObservable**: [`Observable`](Observable.md)[`ITimerData`](../interfaces/ITimerData.md)`T`

Will trigger when the timer was aborted due to the break condition

#### Defined in

packages/dev/core/src/Misc/timer.ts:139

___

### onTimerEndedObservable

• **onTimerEndedObservable**: [`Observable`](Observable.md)[`ITimerData`](../interfaces/ITimerData.md)`T`

Will trigger when the timer ended successfully

#### Defined in

packages/dev/core/src/Misc/timer.ts:143

## Accessors

### breakCondition

• `set` **breakCondition**(`predicate`): `void`

set a breaking condition for this timer. Default is to never break during count

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `predicate` | (`data`: [`ITimerData`](../interfaces/ITimerData.md)`T`) => `boolean` | the new break condition. Returns true to break, false otherwise |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/timer.ts:188

## Methods

### \_setState

▸ `Private` **_setState**(`newState`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `newState` | [`TimerState`](../enums/TimerState.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/timer.ts:238

___

### \_stop

▸ `Private` **_stop**(`data`, `aborted?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `data` | [`ITimerData`](../interfaces/ITimerData.md)`T` | `undefined` |
| `aborted` | `boolean` | `false` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/timer.ts:261

___

### \_tick

▸ `Private` **_tick**(`payload`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `payload` | `T` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/timer.ts:243

___

### clearObservables

▸ **clearObservables**(): `void`

Reset ALL associated observables in this advanced timer

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/timer.ts:195

___

### dispose

▸ **dispose**(): `void`

Dispose this timer, clearing all resources

#### Returns

`void`

#### Implementation of

[IDisposable](../interfaces/IDisposable.md).[dispose](../interfaces/IDisposable.md#dispose)

#### Defined in

packages/dev/core/src/Misc/timer.ts:231

___

### start

▸ **start**(`timeToEnd?`): `void`

Will start a new iteration of this timer. Only one instance of this timer can run at a time.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `timeToEnd` | `number` | how much time to measure until timer ended |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/timer.ts:207

___

### stop

▸ **stop**(): `void`

Will force a stop on the next tick.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/timer.ts:221
