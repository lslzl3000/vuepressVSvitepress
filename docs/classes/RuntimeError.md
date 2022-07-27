[@dev/core](../README.md) / [Exports](../modules.md) / RuntimeError

# Class: RuntimeError

Application runtime error

## Hierarchy

- `BaseError`

  ↳ **`RuntimeError`**

## Table of contents

### Constructors

- [constructor](RuntimeError.md#constructor)

### Properties

- [errorCode](RuntimeError.md#errorcode)
- [innerError](RuntimeError.md#innererror)
- [message](RuntimeError.md#message)
- [name](RuntimeError.md#name)
- [stack](RuntimeError.md#stack)
- [\_setPrototypeOf](RuntimeError.md#_setprototypeof)
- [prepareStackTrace](RuntimeError.md#preparestacktrace)
- [stackTraceLimit](RuntimeError.md#stacktracelimit)

### Methods

- [captureStackTrace](RuntimeError.md#capturestacktrace)

## Constructors

### constructor

• **new RuntimeError**(`message`, `errorCode`, `innerError?`)

Creates a new RuntimeError

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` | defines the message of the error |
| `errorCode` | [`ErrorCodesType`](../modules.md#errorcodestype) | the error code |
| `innerError?` | `Error` | the error that caused the outer error |

#### Overrides

BaseError.constructor

#### Defined in

https://github.com/babylon.js/core/src/Misc/error.ts:75

## Properties

### errorCode

• **errorCode**: [`ErrorCodesType`](../modules.md#errorcodestype)

The error code

#### Defined in

https://github.com/babylon.js/core/src/Misc/error.ts:62

___

### innerError

• `Optional` **innerError**: `Error`

The error that caused this outer error

#### Defined in

https://github.com/babylon.js/core/src/Misc/error.ts:67

___

### message

• **message**: `string`

#### Inherited from

BaseError.message

#### Defined in

node_modules/typescript/lib/lib.es5.d.ts:1023

___

### name

• **name**: `string`

#### Inherited from

BaseError.name

#### Defined in

node_modules/typescript/lib/lib.es5.d.ts:1022

___

### stack

• `Optional` **stack**: `string`

#### Inherited from

BaseError.stack

#### Defined in

node_modules/typescript/lib/lib.es5.d.ts:1024

___

### \_setPrototypeOf

▪ `Static` `Protected` **\_setPrototypeOf**: (`o`: `any`, `proto`: ``null`` \| `object`) => `any`

#### Type declaration

▸ (`o`, `proto`): `any`

##### Parameters

| Name | Type |
| :------ | :------ |
| `o` | `any` |
| `proto` | ``null`` \| `object` |

##### Returns

`any`

#### Inherited from

BaseError.\_setPrototypeOf

#### Defined in

https://github.com/babylon.js/core/src/Misc/error.ts:12

___

### prepareStackTrace

▪ `Static` `Optional` **prepareStackTrace**: (`err`: `Error`, `stackTraces`: `CallSite`[]) => `any`

#### Type declaration

▸ (`err`, `stackTraces`): `any`

Optional override for formatting stack traces

**`See`**

https://v8.dev/docs/stack-trace-api#customizing-stack-traces

##### Parameters

| Name | Type |
| :------ | :------ |
| `err` | `Error` |
| `stackTraces` | `CallSite`[] |

##### Returns

`any`

#### Inherited from

BaseError.prepareStackTrace

#### Defined in

node_modules/@types/node/globals.d.ts:11

___

### stackTraceLimit

▪ `Static` **stackTraceLimit**: `number`

#### Inherited from

BaseError.stackTraceLimit

#### Defined in

node_modules/@types/node/globals.d.ts:13

## Methods

### captureStackTrace

▸ `Static` **captureStackTrace**(`targetObject`, `constructorOpt?`): `void`

Create .stack property on a target object

#### Parameters

| Name | Type |
| :------ | :------ |
| `targetObject` | `object` |
| `constructorOpt?` | `Function` |

#### Returns

`void`

#### Inherited from

BaseError.captureStackTrace

#### Defined in

node_modules/@types/node/globals.d.ts:4
