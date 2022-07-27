[@dev/core](../README.md) / [Exports](../modules.md) / AssetsProgressEvent

# Class: AssetsProgressEvent

Class used to share progress information about assets loading

## Implements

- [`IAssetsProgressEvent`](../interfaces/IAssetsProgressEvent.md)

## Table of contents

### Constructors

- [constructor](AssetsProgressEvent.md#constructor)

### Properties

- [remainingCount](AssetsProgressEvent.md#remainingcount)
- [task](AssetsProgressEvent.md#task)
- [totalCount](AssetsProgressEvent.md#totalcount)

## Constructors

### constructor

• **new AssetsProgressEvent**(`remainingCount`, `totalCount`, `task`)

Creates a AssetsProgressEvent

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `remainingCount` | `number` | defines the number of remaining tasks to process |
| `totalCount` | `number` | defines the total number of tasks |
| `task` | [`AbstractAssetTask`](AbstractAssetTask.md) | defines the task that was just processed |

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:216

## Properties

### remainingCount

• **remainingCount**: `number`

Defines the number of remaining tasks to process

#### Implementation of

[IAssetsProgressEvent](../interfaces/IAssetsProgressEvent.md).[remainingCount](../interfaces/IAssetsProgressEvent.md#remainingcount)

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:200

___

### task

• **task**: [`AbstractAssetTask`](AbstractAssetTask.md)

Defines the task that was just processed

#### Implementation of

[IAssetsProgressEvent](../interfaces/IAssetsProgressEvent.md).[task](../interfaces/IAssetsProgressEvent.md#task)

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:208

___

### totalCount

• **totalCount**: `number`

Defines the total number of tasks

#### Implementation of

[IAssetsProgressEvent](../interfaces/IAssetsProgressEvent.md).[totalCount](../interfaces/IAssetsProgressEvent.md#totalcount)

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:204
