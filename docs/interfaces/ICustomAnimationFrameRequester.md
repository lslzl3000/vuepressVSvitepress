[@dev/core](../README.md) / [Exports](../modules.md) / ICustomAnimationFrameRequester

# Interface: ICustomAnimationFrameRequester

Interface for any object that can request an animation frame

## Table of contents

### Properties

- [renderFunction](ICustomAnimationFrameRequester.md#renderfunction)
- [requestAnimationFrame](ICustomAnimationFrameRequester.md#requestanimationframe)
- [requestID](ICustomAnimationFrameRequester.md#requestid)

## Properties

### renderFunction

• `Optional` **renderFunction**: `Function`

This function will be called when the render loop is ready. If this is not populated, the engine's renderloop function will be called

#### Defined in

https://github.com/babylon.js/core/src/Misc/customAnimationFrameRequester.ts:8

___

### requestAnimationFrame

• **requestAnimationFrame**: `Function`

Called to request the next frame to render to

**`See`**

https://developer.mozilla.org/en-US/docs/Web/API/window/requestAnimationFrame

#### Defined in

https://github.com/babylon.js/core/src/Misc/customAnimationFrameRequester.ts:13

___

### requestID

• `Optional` **requestID**: `number`

You can pass this value to cancelAnimationFrame() to cancel the refresh callback request

**`See`**

https://developer.mozilla.org/en-US/docs/Web/API/window/requestAnimationFrame#Return_value

#### Defined in

https://github.com/babylon.js/core/src/Misc/customAnimationFrameRequester.ts:18
