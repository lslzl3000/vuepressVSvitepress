[@dev/core](../README.md) / [Exports](../modules.md) / IWebXRDomOverlayOptions

# Interface: IWebXRDomOverlayOptions

Options for DOM Overlay feature

## Table of contents

### Properties

- [element](IWebXRDomOverlayOptions.md#element)
- [supressXRSelectEvents](IWebXRDomOverlayOptions.md#supressxrselectevents)

## Properties

### element

• **element**: `string` \| `Element`

DOM Element or document query selector string for overlay.

NOTE: UA may make this element background transparent in XR.

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRDOMOverlay.ts:16

___

### supressXRSelectEvents

• `Optional` **supressXRSelectEvents**: `boolean`

Supress XR Select events on container element (DOM blocks interaction to scene).

#### Defined in

https://github.com/babylon.js/core/src/XR/features/WebXRDOMOverlay.ts:20
