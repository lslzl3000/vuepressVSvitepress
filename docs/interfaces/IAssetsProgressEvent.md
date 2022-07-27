[@dev/core](../README.md) / [Exports](../modules.md) / IAssetsProgressEvent

# Interface: IAssetsProgressEvent

Define the interface used by progress events raised during assets loading

## Implemented by

- [`AssetsProgressEvent`](../classes/AssetsProgressEvent.md)

## Table of contents

### Properties

- [remainingCount](IAssetsProgressEvent.md#remainingcount)
- [task](IAssetsProgressEvent.md#task)
- [totalCount](IAssetsProgressEvent.md#totalcount)

## Properties

### remainingCount

• **remainingCount**: `number`

Defines the number of remaining tasks to process

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:182

___

### task

• **task**: [`AbstractAssetTask`](../classes/AbstractAssetTask.md)

Defines the task that was just processed

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:190

___

### totalCount

• **totalCount**: `number`

Defines the total number of tasks

#### Defined in

https://github.com/babylon.js/core/src/Misc/assetsManager.ts:186
