[@dev/core](../README.md) / [Exports](../modules.md) / EngineFactory

# Class: EngineFactory

Helper class to create the best engine depending on the current hardware

## Table of contents

### Constructors

- [constructor](EngineFactory.md#constructor)

### Methods

- [CreateAsync](EngineFactory.md#createasync)

## Constructors

### constructor

• **new EngineFactory**()

## Methods

### CreateAsync

▸ `Static` **CreateAsync**(`canvas`, `options`): `Promise`[`Engine`](Engine.md)

Creates an engine based on the capabilities of the underlying hardware

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `canvas` | `HTMLCanvasElement` | Defines the canvas to use to display the result |
| `options` | `any` | Defines the options passed to the engine to create the context dependencies |

#### Returns

`Promise`[`Engine`](Engine.md)

a promise that resolves with the created engine

#### Defined in

packages/dev/core/src/Engines/engineFactory.ts:15
