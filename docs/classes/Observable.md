[@dev/core](../README.md) / [Exports](../modules.md) / Observable

# Class: ObservableT

The Observable class is a simple implementation of the Observable pattern.

There's one slight particularity though: a given Observable can notify its observer using a particular mask value, only the Observers registered with this mask value will be notified.
This enable a more fine grained execution without having to rely on multiple different Observable objects.
For instance you may have a given Observable that have four different types of notifications: Move (mask = 0x01), Stop (mask = 0x02), Turn Right (mask = 0X04), Turn Left (mask = 0X08).
A given observer can register itself with only Move and Stop (mask = 0x03), then it will only be notified when one of these two occurs and will never be for Turn Left/Right.

## Type parameters

| Name |
| :------ |
| `T` |

## Table of contents

### Constructors

- [constructor](Observable.md#constructor)

### Properties

- [\_coroutineScheduler](Observable.md#_coroutinescheduler)
- [\_coroutineSchedulerDispose](Observable.md#_coroutineschedulerdispose)
- [\_eventState](Observable.md#_eventstate)
- [\_observers](Observable.md#_observers)
- [\_onObserverAdded](Observable.md#_onobserveradded)

### Accessors

- [observers](Observable.md#observers)

### Methods

- [\_deferUnregister](Observable.md#_deferunregister)
- [\_remove](Observable.md#_remove)
- [add](Observable.md#add)
- [addOnce](Observable.md#addonce)
- [cancelAllCoroutines](Observable.md#cancelallcoroutines)
- [clear](Observable.md#clear)
- [clone](Observable.md#clone)
- [hasObservers](Observable.md#hasobservers)
- [hasSpecificMask](Observable.md#hasspecificmask)
- [makeObserverBottomPriority](Observable.md#makeobserverbottompriority)
- [makeObserverTopPriority](Observable.md#makeobservertoppriority)
- [notifyObserver](Observable.md#notifyobserver)
- [notifyObservers](Observable.md#notifyobservers)
- [notifyObserversWithPromise](Observable.md#notifyobserverswithpromise)
- [remove](Observable.md#remove)
- [removeCallback](Observable.md#removecallback)
- [runCoroutineAsync](Observable.md#runcoroutineasync)
- [FromPromise](Observable.md#frompromise)

## Constructors

### constructor

• **new Observable**`T`(`onObserverAdded?`)

Creates a new observable

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `onObserverAdded?` | (`observer`: [`Observer`](Observer.md)`T`) => `void` | defines a callback to call when a new observer is added |

#### Defined in

https://github.com/babylon.js/core/src/Misc/observable.ts:195

## Properties

### \_coroutineScheduler

• `Optional` **\_coroutineScheduler**: `CoroutineScheduler``void`

Internal observable-based coroutine scheduler instance.

#### Defined in

https://github.com/babylon.js/core/src/Misc/observableCoroutine.ts:37

___

### \_coroutineSchedulerDispose

• `Optional` **\_coroutineSchedulerDispose**: () => `void`

#### Type declaration

▸ (): `void`

Internal disposal method for observable-based coroutine scheduler instance.

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/observableCoroutine.ts:42

___

### \_eventState

• `Private` **\_eventState**: [`EventState`](EventState.md)

#### Defined in

https://github.com/babylon.js/core/src/Misc/observable.ts:156

___

### \_observers

• `Private` **\_observers**: [`Observer`](Observer.md)`T`[]

#### Defined in

https://github.com/babylon.js/core/src/Misc/observable.ts:154

___

### \_onObserverAdded

• `Private` **\_onObserverAdded**: [`Nullable`](../modules.md#nullable)(`observer`: [`Observer`](Observer.md)`T`) => `void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/observable.ts:158

## Accessors

### observers

• `get` **observers**(): [`Observer`](Observer.md)`T`[]

Gets the list of observers

#### Returns

[`Observer`](Observer.md)`T`[]

#### Defined in

https://github.com/babylon.js/core/src/Misc/observable.ts:187

## Methods

### \_deferUnregister

▸ `Private` **_deferUnregister**(`observer`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `observer` | [`Observer`](Observer.md)`T` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/observable.ts:289

___

### \_remove

▸ `Private` **_remove**(`observer`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `observer` | [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)`T` |

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Misc/observable.ts:299

___

### add

▸ **add**(`callback`, `mask?`, `insertFirst?`, `scope?`, `unregisterOnFirstCall?`): [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)`T`

Create a new Observer with the specified callback

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `callback` | (`eventData`: `T`, `eventState`: [`EventState`](EventState.md)) => `void` | `undefined` | the callback that will be executed for that Observer |
| `mask` | `number` | `-1` | the mask used to filter observers |
| `insertFirst` | `boolean` | `false` | if true the callback will be inserted at the first position, hence executed before the others ones. If false (default behavior) the callback will be inserted at the last position, executed after all the others already present. |
| `scope` | `any` | `null` | optional scope for the callback to be called from |
| `unregisterOnFirstCall` | `boolean` | `false` | defines if the observer as to be unregistered after the next notification |

#### Returns

[`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)`T`

the new observer created for the callback

#### Defined in

https://github.com/babylon.js/core/src/Misc/observable.ts:212

___

### addOnce

▸ **addOnce**(`callback`): [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)`T`

Create a new Observer with the specified callback and unregisters after the next notification

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callback` | (`eventData`: `T`, `eventState`: [`EventState`](EventState.md)) => `void` | the callback that will be executed for that Observer |

#### Returns

[`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)`T`

the new observer created for the callback

#### Defined in

https://github.com/babylon.js/core/src/Misc/observable.ts:244

___

### cancelAllCoroutines

▸ **cancelAllCoroutines**(): `void`

Cancels all coroutines currently running on this observable

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/observableCoroutine.ts:54

___

### clear

▸ **clear**(): `void`

Clear the list of observers

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/observable.ts:473

___

### clone

▸ **clone**(): [`Observable`](Observable.md)`T`

Clone the current observable

#### Returns

[`Observable`](Observable.md)`T`

a new observable

#### Defined in

https://github.com/babylon.js/core/src/Misc/observable.ts:482

___

### hasObservers

▸ **hasObservers**(): `boolean`

Gets a boolean indicating if the observable has at least one observer

#### Returns

`boolean`

true is the Observable has at least one Observer registered

#### Defined in

https://github.com/babylon.js/core/src/Misc/observable.ts:466

___

### hasSpecificMask

▸ **hasSpecificMask**(`mask?`): `boolean`

Does this observable handles observer registered with a given mask

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `mask` | `number` | `-1` | defines the mask to be tested |

#### Returns

`boolean`

whether or not one observer registered with the given mask is handled

#### Defined in

https://github.com/babylon.js/core/src/Misc/observable.ts:495

___

### makeObserverBottomPriority

▸ **makeObserverBottomPriority**(`observer`): `void`

Moves the observable to the bottom of the observer list making it get called last when notified

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `observer` | [`Observer`](Observer.md)`T` | the observer to move |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/observable.ts:327

___

### makeObserverTopPriority

▸ **makeObserverTopPriority**(`observer`): `void`

Moves the observable to the top of the observer list making it get called first when notified

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `observer` | [`Observer`](Observer.md)`T` | the observer to move |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/observable.ts:318

___

### notifyObserver

▸ **notifyObserver**(`observer`, `eventData`, `mask?`): `void`

Notify a specific observer

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `observer` | [`Observer`](Observer.md)`T` | `undefined` | defines the observer to notify |
| `eventData` | `T` | `undefined` | defines the data to be sent to each callback |
| `mask` | `number` | `-1` | is used to filter observers defaults to -1 |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/observable.ts:446

___

### notifyObservers

▸ **notifyObservers**(`eventData`, `mask?`, `target?`, `currentTarget?`, `userInfo?`): `boolean`

Notify all Observers by calling their respective callback with the given data
Will return true if all observers were executed, false if an observer set skipNextObservers to true, then prevent the subsequent ones to execute

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `eventData` | `T` | `undefined` | defines the data to send to all observers |
| `mask` | `number` | `-1` | defines the mask of the current notification (observers with incompatible mask (ie mask & observer.mask === 0) will not be notified) |
| `target?` | `any` | `undefined` | defines the original target of the state |
| `currentTarget?` | `any` | `undefined` | defines the current target of the state |
| `userInfo?` | `any` | `undefined` | defines any user info to send to observers |

#### Returns

`boolean`

false if the complete observer chain was not processed (because one observer set the skipNextObservers to true)

#### Defined in

https://github.com/babylon.js/core/src/Misc/observable.ts:342

___

### notifyObserversWithPromise

▸ **notifyObserversWithPromise**(`eventData`, `mask?`, `target?`, `currentTarget?`, `userInfo?`): `Promise``T`

Calling this will execute each callback, expecting it to be a promise or return a value.
If at any point in the chain one function fails, the promise will fail and the execution will not continue.
This is useful when a chain of events (sometimes async events) is needed to initialize a certain object
and it is crucial that all callbacks will be executed.
The order of the callbacks is kept, callbacks are not executed parallel.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `eventData` | `T` | `undefined` | The data to be sent to each callback |
| `mask` | `number` | `-1` | is used to filter observers defaults to -1 |
| `target?` | `any` | `undefined` | defines the callback target (see EventState) |
| `currentTarget?` | `any` | `undefined` | defines he current object in the bubbling phase |
| `userInfo?` | `any` | `undefined` | defines any user info to send to observers |

#### Returns

`Promise``T`

will return a Promise than resolves when all callbacks executed successfully.

#### Defined in

https://github.com/babylon.js/core/src/Misc/observable.ts:392

___

### remove

▸ **remove**(`observer`): `boolean`

Remove an Observer from the Observable object

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `observer` | [`Nullable`](../modules.md#nullable)[`Observer`](Observer.md)`T` | the instance of the Observer to remove |

#### Returns

`boolean`

false if it doesn't belong to this Observable

#### Defined in

https://github.com/babylon.js/core/src/Misc/observable.ts:253

___

### removeCallback

▸ **removeCallback**(`callback`, `scope?`): `boolean`

Remove a callback from the Observable object

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callback` | (`eventData`: `T`, `eventState`: [`EventState`](EventState.md)) => `void` | the callback to remove |
| `scope?` | `any` | optional scope. If used only the callbacks with this scope will be removed |

#### Returns

`boolean`

false if it doesn't belong to this Observable

#### Defined in

https://github.com/babylon.js/core/src/Misc/observable.ts:274

___

### runCoroutineAsync

▸ **runCoroutineAsync**(`coroutine`): `Promise``void`

Runs a coroutine asynchronously on this observable

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `coroutine` | `AsyncCoroutine``void` | the iterator resulting from having started the coroutine |

#### Returns

`Promise``void`

a promise which will be resolved when the coroutine finishes or rejected if the coroutine is cancelled

#### Defined in

https://github.com/babylon.js/core/src/Misc/observableCoroutine.ts:49

___

### FromPromise

▸ `Static` **FromPromise**`T`, `E`(`promise`, `onErrorObservable?`): [`Observable`](Observable.md)`T`

Create an observable from a Promise.

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | `T` |
| `E` | `Error` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `promise` | `Promise``T` | a promise to observe for fulfillment. |
| `onErrorObservable?` | [`Observable`](Observable.md)`E` | an observable to notify if a promise was rejected. |

#### Returns

[`Observable`](Observable.md)`T`

the new Observable

#### Defined in

https://github.com/babylon.js/core/src/Misc/observable.ts:166
