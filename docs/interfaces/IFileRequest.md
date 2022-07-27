[@dev/core](../README.md) / [Exports](../modules.md) / IFileRequest

# Interface: IFileRequest

File request interface

## Table of contents

### Properties

- [abort](IFileRequest.md#abort)
- [onCompleteObservable](IFileRequest.md#oncompleteobservable)

## Properties

### abort

• **abort**: () => `void`

#### Type declaration

▸ (): `void`

Aborts the request for a file.

##### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Misc/fileRequest.ts:15

___

### onCompleteObservable

• **onCompleteObservable**: [`Observable`](../classes/Observable.md)[`IFileRequest`](IFileRequest.md)

Raised when the request is complete (success or error).

#### Defined in

https://github.com/babylon.js/core/src/Misc/fileRequest.ts:10
