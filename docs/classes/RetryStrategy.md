[@dev/core](../README.md) / [Exports](../modules.md) / RetryStrategy

# Class: RetryStrategy

Class used to define a retry strategy when error happens while loading assets

## Table of contents

### Constructors

- [constructor](RetryStrategy.md#constructor)

### Methods

- [ExponentialBackoff](RetryStrategy.md#exponentialbackoff)

## Constructors

### constructor

• **new RetryStrategy**()

## Methods

### ExponentialBackoff

▸ `Static` **ExponentialBackoff**(`maxRetries?`, `baseInterval?`): (`url`: `string`, `request`: [`WebRequest`](WebRequest.md), `retryIndex`: `number`) => `number`

Function used to defines an exponential back off strategy

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `maxRetries` | `number` | `3` | defines the maximum number of retries (3 by default) |
| `baseInterval` | `number` | `500` | defines the interval between retries |

#### Returns

`fn`

the strategy function to use

▸ (`url`, `request`, `retryIndex`): `number`

##### Parameters

| Name | Type |
| :------ | :------ |
| `url` | `string` |
| `request` | [`WebRequest`](WebRequest.md) |
| `retryIndex` | `number` |

##### Returns

`number`

#### Defined in

packages/dev/core/src/Misc/retryStrategy.ts:13
