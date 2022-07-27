[@dev/core](../README.md) / [Exports](../modules.md) / Logger

# Class: Logger

Logger used throughout the application to allow configuration of
the log level required for the messages.

## Table of contents

### Constructors

- [constructor](Logger.md#constructor)

### Properties

- [AllLogLevel](Logger.md#allloglevel)
- [Error](Logger.md#error)
- [ErrorLogLevel](Logger.md#errorloglevel)
- [Log](Logger.md#log)
- [MessageLimitReached](Logger.md#messagelimitreached)
- [MessageLogLevel](Logger.md#messageloglevel)
- [NoneLogLevel](Logger.md#noneloglevel)
- [OnNewCacheEntry](Logger.md#onnewcacheentry)
- [Warn](Logger.md#warn)
- [WarningLogLevel](Logger.md#warningloglevel)
- [\_LogCache](Logger.md#_logcache)
- [\_LogLimitOutputs](Logger.md#_loglimitoutputs)
- [errorsCount](Logger.md#errorscount)

### Accessors

- [LogCache](Logger.md#logcache)
- [LogLevels](Logger.md#loglevels)

### Methods

- [ClearLogCache](Logger.md#clearlogcache)
- [\_AddLogEntry](Logger.md#_addlogentry)
- [\_CheckLimit](Logger.md#_checklimit)
- [\_ErrorDisabled](Logger.md#_errordisabled)
- [\_ErrorEnabled](Logger.md#_errorenabled)
- [\_FormatMessage](Logger.md#_formatmessage)
- [\_GenerateLimitMessage](Logger.md#_generatelimitmessage)
- [\_LogDisabled](Logger.md#_logdisabled)
- [\_LogEnabled](Logger.md#_logenabled)
- [\_WarnDisabled](Logger.md#_warndisabled)
- [\_WarnEnabled](Logger.md#_warnenabled)

## Constructors

### constructor

• **new Logger**()

## Properties

### AllLogLevel

▪ `Static` `Readonly` **AllLogLevel**: ``7``

All logs

#### Defined in

https://github.com/babylon.js/core/src/Misc/logger.ts:25

___

### Error

▪ `Static` **Error**: (`message`: `string`, `limit?`: `number`) => `void` = `Logger._ErrorEnabled`

#### Type declaration

▸ (`message`, `limit?`): `void`

Write an error message to the console

##### Parameters

| Name | Type |
| :------ | :------ |
| `message` | `string` |
| `limit?` | `number` |

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/logger.ts:161

___

### ErrorLogLevel

▪ `Static` `Readonly` **ErrorLogLevel**: ``4``

Only error logs

#### Defined in

https://github.com/babylon.js/core/src/Misc/logger.ts:21

___

### Log

▪ `Static` **Log**: (`message`: `string`, `limit?`: `number`) => `void` = `Logger._LogEnabled`

#### Type declaration

▸ (`message`, `limit?`): `void`

Log a message to the console

##### Parameters

| Name | Type |
| :------ | :------ |
| `message` | `string` |
| `limit?` | `number` |

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/logger.ts:151

___

### MessageLimitReached

▪ `Static` **MessageLimitReached**: `string` = `"Too many %TYPE%s (%LIMIT%), no more %TYPE%s will be reported for this message."`

Message to display when a message has been logged too many times

#### Defined in

https://github.com/babylon.js/core/src/Misc/logger.ts:30

___

### MessageLogLevel

▪ `Static` `Readonly` **MessageLogLevel**: ``1``

Only message logs

#### Defined in

https://github.com/babylon.js/core/src/Misc/logger.ts:13

___

### NoneLogLevel

▪ `Static` `Readonly` **NoneLogLevel**: ``0``

No log

#### Defined in

https://github.com/babylon.js/core/src/Misc/logger.ts:9

___

### OnNewCacheEntry

▪ `Static` **OnNewCacheEntry**: (`entry`: `string`) => `void`

#### Type declaration

▸ (`entry`): `void`

Callback called when a new log is added

##### Parameters

| Name | Type |
| :------ | :------ |
| `entry` | `string` |

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/logger.ts:45

___

### Warn

▪ `Static` **Warn**: (`message`: `string`, `limit?`: `number`) => `void` = `Logger._WarnEnabled`

#### Type declaration

▸ (`message`, `limit?`): `void`

Write a warning message to the console

##### Parameters

| Name | Type |
| :------ | :------ |
| `message` | `string` |
| `limit?` | `number` |

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/logger.ts:156

___

### WarningLogLevel

▪ `Static` `Readonly` **WarningLogLevel**: ``2``

Only warning logs

#### Defined in

https://github.com/babylon.js/core/src/Misc/logger.ts:17

___

### \_LogCache

▪ `Static` `Private` **\_LogCache**: `string` = `""`

#### Defined in

https://github.com/babylon.js/core/src/Misc/logger.ts:32

___

### \_LogLimitOutputs

▪ `Static` `Private` **\_LogLimitOutputs**: `Object` = `{}`

#### Index signature

▪ [message: `string`]: { `current`: `number` ; `limit`: `number`  }

#### Defined in

https://github.com/babylon.js/core/src/Misc/logger.ts:33

___

### errorsCount

▪ `Static` **errorsCount**: `number` = `0`

Gets a value indicating the number of loading errors

**`Ignorenaming`**

#### Defined in

https://github.com/babylon.js/core/src/Misc/logger.ts:40

## Accessors

### LogCache

• `Static` `get` **LogCache**(): `string`

Gets current log cache (list of logs)

#### Returns

`string`

#### Defined in

https://github.com/babylon.js/core/src/Misc/logger.ts:166

___

### LogLevels

• `Static` `set` **LogLevels**(`level`): `void`

Sets the current log level (MessageLogLevel / WarningLogLevel / ErrorLogLevel)

#### Parameters

| Name | Type |
| :------ | :------ |
| `level` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/logger.ts:182

## Methods

### ClearLogCache

▸ `Static` **ClearLogCache**(): `void`

Clears the log cache

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/logger.ts:173

___

### \_AddLogEntry

▸ `Static` `Private` **_AddLogEntry**(`entry`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `entry` | `string` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/logger.ts:78

___

### \_CheckLimit

▸ `Static` `Private` **_CheckLimit**(`message`, `limit`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `message` | `string` |
| `limit` | `number` |

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Misc/logger.ts:47

___

### \_ErrorDisabled

▸ `Static` `Private` **_ErrorDisabled**(`message`, `limit?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `message` | `string` |
| `limit?` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/logger.ts:130

___

### \_ErrorEnabled

▸ `Static` `Private` **_ErrorEnabled**(`message`, `limit?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `message` | `string` |
| `limit?` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/logger.ts:133

___

### \_FormatMessage

▸ `Static` `Private` **_FormatMessage**(`message`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `message` | `string` |

#### Returns

`string`

#### Defined in

https://github.com/babylon.js/core/src/Misc/logger.ts:86

___

### \_GenerateLimitMessage

▸ `Static` `Private` **_GenerateLimitMessage**(`message`, `messageType`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `message` | `string` |
| `messageType` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/logger.ts:58

___

### \_LogDisabled

▸ `Static` `Private` **_LogDisabled**(`message`, `limit?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `message` | `string` |
| `limit?` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/logger.ts:94

___

### \_LogEnabled

▸ `Static` `Private` **_LogEnabled**(`message`, `limit?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `message` | `string` |
| `limit?` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/logger.ts:97

___

### \_WarnDisabled

▸ `Static` `Private` **_WarnDisabled**(`message`, `limit?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `message` | `string` |
| `limit?` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/logger.ts:112

___

### \_WarnEnabled

▸ `Static` `Private` **_WarnEnabled**(`message`, `limit?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `message` | `string` |
| `limit?` | `number` |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/logger.ts:115
