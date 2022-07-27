[@dev/core](../README.md) / [Exports](../modules.md) / WebXRControllerComponent

# Class: WebXRControllerComponent

This class represents a single component (for example button or thumbstick) of a motion controller

## Implements

- [`IDisposable`](../interfaces/IDisposable.md)

## Table of contents

### Constructors

- [constructor](WebXRControllerComponent.md#constructor)

### Properties

- [\_axes](WebXRControllerComponent.md#_axes)
- [\_changes](WebXRControllerComponent.md#_changes)
- [\_currentValue](WebXRControllerComponent.md#_currentvalue)
- [\_hasChanges](WebXRControllerComponent.md#_haschanges)
- [\_pressed](WebXRControllerComponent.md#_pressed)
- [\_touched](WebXRControllerComponent.md#_touched)
- [id](WebXRControllerComponent.md#id)
- [onAxisValueChangedObservable](WebXRControllerComponent.md#onaxisvaluechangedobservable)
- [onButtonStateChangedObservable](WebXRControllerComponent.md#onbuttonstatechangedobservable)
- [type](WebXRControllerComponent.md#type)
- [BUTTON\_TYPE](WebXRControllerComponent.md#button_type)
- [SQUEEZE\_TYPE](WebXRControllerComponent.md#squeeze_type)
- [THUMBSTICK\_TYPE](WebXRControllerComponent.md#thumbstick_type)
- [TOUCHPAD\_TYPE](WebXRControllerComponent.md#touchpad_type)
- [TRIGGER\_TYPE](WebXRControllerComponent.md#trigger_type)

### Accessors

- [axes](WebXRControllerComponent.md#axes)
- [changes](WebXRControllerComponent.md#changes)
- [hasChanges](WebXRControllerComponent.md#haschanges)
- [pressed](WebXRControllerComponent.md#pressed)
- [touched](WebXRControllerComponent.md#touched)
- [value](WebXRControllerComponent.md#value)

### Methods

- [dispose](WebXRControllerComponent.md#dispose)
- [isAxes](WebXRControllerComponent.md#isaxes)
- [isButton](WebXRControllerComponent.md#isbutton)
- [update](WebXRControllerComponent.md#update)

## Constructors

### constructor

• **new WebXRControllerComponent**(`id`, `type`, `_buttonIndex?`, `_axesIndices?`)

Creates a new component for a motion controller.
It is created by the motion controller itself

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `id` | `string` | `undefined` | the id of this component |
| `type` | [`MotionControllerComponentType`](../modules.md#motioncontrollercomponenttype) | `undefined` | the type of the component |
| `_buttonIndex` | `number` | `-1` | index in the buttons array of the gamepad |
| `_axesIndices` | `number`[] | `[]` | indices of the values in the axes array of the gamepad |

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRControllerComponent.ts:109

## Properties

### \_axes

• `Private` **\_axes**: [`IWebXRMotionControllerAxesValue`](../interfaces/IWebXRMotionControllerAxesValue.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRControllerComponent.ts:58

___

### \_changes

• `Private` **\_changes**: [`IWebXRMotionControllerComponentChanges`](../interfaces/IWebXRMotionControllerComponentChanges.md) = `{}`

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRControllerComponent.ts:62

___

### \_currentValue

• `Private` **\_currentValue**: `number` = `0`

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRControllerComponent.ts:63

___

### \_hasChanges

• `Private` **\_hasChanges**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRControllerComponent.ts:64

___

### \_pressed

• `Private` **\_pressed**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRControllerComponent.ts:65

___

### \_touched

• `Private` **\_touched**: `boolean` = `false`

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRControllerComponent.ts:66

___

### id

• **id**: `string`

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRControllerComponent.ts:113

___

### onAxisValueChangedObservable

• **onAxisValueChangedObservable**: [`Observable`](Observable.md){ `x`: `number` ; `y`: `number`  }

If axes are available for this component (like a touchpad or thumbstick) the observers will be notified when
the axes data changes

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRControllerComponent.ts:93

___

### onButtonStateChangedObservable

• **onButtonStateChangedObservable**: [`Observable`](Observable.md)[`WebXRControllerComponent`](WebXRControllerComponent.md)

Observers registered here will be triggered when the state of a button changes
State change is either pressed / touched / value

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRControllerComponent.ts:98

___

### type

• **type**: [`MotionControllerComponentType`](../modules.md#motioncontrollercomponenttype)

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRControllerComponent.ts:117

___

### BUTTON\_TYPE

▪ `Static` **BUTTON\_TYPE**: [`MotionControllerComponentType`](../modules.md#motioncontrollercomponenttype) = `"button"`

button component type

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRControllerComponent.ts:71

___

### SQUEEZE\_TYPE

▪ `Static` **SQUEEZE\_TYPE**: [`MotionControllerComponentType`](../modules.md#motioncontrollercomponenttype) = `"squeeze"`

squeeze component type

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRControllerComponent.ts:75

___

### THUMBSTICK\_TYPE

▪ `Static` **THUMBSTICK\_TYPE**: [`MotionControllerComponentType`](../modules.md#motioncontrollercomponenttype) = `"thumbstick"`

Thumbstick component type

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRControllerComponent.ts:79

___

### TOUCHPAD\_TYPE

▪ `Static` **TOUCHPAD\_TYPE**: [`MotionControllerComponentType`](../modules.md#motioncontrollercomponenttype) = `"touchpad"`

Touchpad component type

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRControllerComponent.ts:83

___

### TRIGGER\_TYPE

▪ `Static` **TRIGGER\_TYPE**: [`MotionControllerComponentType`](../modules.md#motioncontrollercomponenttype) = `"trigger"`

trigger component type

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRControllerComponent.ts:87

## Accessors

### axes

• `get` **axes**(): [`IWebXRMotionControllerAxesValue`](../interfaces/IWebXRMotionControllerAxesValue.md)

The current axes data. If this component has no axes it will still return an object { x: 0, y: 0 }

#### Returns

[`IWebXRMotionControllerAxesValue`](../interfaces/IWebXRMotionControllerAxesValue.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRControllerComponent.ts:125

___

### changes

• `get` **changes**(): [`IWebXRMotionControllerComponentChanges`](../interfaces/IWebXRMotionControllerComponentChanges.md)

Get the changes. Elements will be populated only if they changed with their previous and current value

#### Returns

[`IWebXRMotionControllerComponentChanges`](../interfaces/IWebXRMotionControllerComponentChanges.md)

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRControllerComponent.ts:132

___

### hasChanges

• `get` **hasChanges**(): `boolean`

Return whether or not the component changed the last frame

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRControllerComponent.ts:139

___

### pressed

• `get` **pressed**(): `boolean`

is the button currently pressed

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRControllerComponent.ts:146

___

### touched

• `get` **touched**(): `boolean`

is the button currently touched

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRControllerComponent.ts:153

___

### value

• `get` **value**(): `number`

Get the current value of this component

#### Returns

`number`

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRControllerComponent.ts:160

## Methods

### dispose

▸ **dispose**(): `void`

Dispose this component

#### Returns

`void`

#### Implementation of

[IDisposable](../interfaces/IDisposable.md).[dispose](../interfaces/IDisposable.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRControllerComponent.ts:167

___

### isAxes

▸ **isAxes**(): `boolean`

Are there axes correlating to this component

#### Returns

`boolean`

true is axes data is available

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRControllerComponent.ts:176

___

### isButton

▸ **isButton**(): `boolean`

Is this component a button (hence - pressable)

#### Returns

`boolean`

true if can be pressed

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRControllerComponent.ts:184

___

### update

▸ **update**(`nativeController`): `void`

update this component using the gamepad object it is in. Called on every frame

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `nativeController` | [`IMinimalMotionControllerObject`](../interfaces/IMinimalMotionControllerObject.md) | the native gamepad controller object |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/XR/motionController/webXRControllerComponent.ts:192
