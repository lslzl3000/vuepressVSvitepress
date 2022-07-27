[@dev/core](../README.md) / [Exports](../modules.md) / DebugLayer

# Class: DebugLayer

The debug layer (aka Inspector) is the go to tool in order to better understand
what is happening in your scene

**`See`**

https://doc.babylonjs.com/features/playground_debuglayer

## Table of contents

### Constructors

- [constructor](DebugLayer.md#constructor)

### Properties

- [BJSINSPECTOR](DebugLayer.md#bjsinspector)
- [\_onPropertyChangedObservable](DebugLayer.md#_onpropertychangedobservable)
- [\_onSelectionChangedObservable](DebugLayer.md#_onselectionchangedobservable)
- [\_scene](DebugLayer.md#_scene)
- [InspectorURL](DebugLayer.md#inspectorurl)

### Accessors

- [onPropertyChangedObservable](DebugLayer.md#onpropertychangedobservable)
- [onSelectionChangedObservable](DebugLayer.md#onselectionchangedobservable)

### Methods

- [\_createInspector](DebugLayer.md#_createinspector)
- [\_getGlobalInspector](DebugLayer.md#_getglobalinspector)
- [hide](DebugLayer.md#hide)
- [isVisible](DebugLayer.md#isvisible)
- [select](DebugLayer.md#select)
- [setAsActiveScene](DebugLayer.md#setasactivescene)
- [show](DebugLayer.md#show)

## Constructors

### constructor

• **new DebugLayer**(`scene?`)

Instantiates a new debug layer.
The debug layer (aka Inspector) is the go to tool in order to better understand
what is happening in your scene

**`See`**

https://doc.babylonjs.com/features/playground_debuglayer

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene?` | [`Scene`](Scene.md) | Defines the scene to inspect |

#### Defined in

packages/dev/core/src/Debug/debugLayer.ts:199

## Properties

### BJSINSPECTOR

• `Private` **BJSINSPECTOR**: `any`

#### Defined in

packages/dev/core/src/Debug/debugLayer.ts:158

___

### \_onPropertyChangedObservable

• `Private` `Optional` **\_onPropertyChangedObservable**: [`Observable`](Observable.md){ `initialValue`: `any` ; `object`: `any` ; `property`: `string` ; `value`: `any`  }

#### Defined in

packages/dev/core/src/Debug/debugLayer.ts:160

___

### \_onSelectionChangedObservable

• `Private` `Optional` **\_onSelectionChangedObservable**: [`Observable`](Observable.md)`any`

#### Defined in

packages/dev/core/src/Debug/debugLayer.ts:176

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/Debug/debugLayer.ts:155

___

### InspectorURL

▪ `Static` **InspectorURL**: `string`

Define the url to get the inspector script from.
By default it uses the babylonjs CDN.

**`Ignore Naming`**

#### Defined in

packages/dev/core/src/Debug/debugLayer.ts:153

## Accessors

### onPropertyChangedObservable

• `get` **onPropertyChangedObservable**(): `any`

Observable triggered when a property is changed through the inspector.

#### Returns

`any`

#### Defined in

packages/dev/core/src/Debug/debugLayer.ts:164

___

### onSelectionChangedObservable

• `get` **onSelectionChangedObservable**(): `any`

Observable triggered when the selection is changed through the inspector.

#### Returns

`any`

#### Defined in

packages/dev/core/src/Debug/debugLayer.ts:180

## Methods

### \_createInspector

▸ `Private` **_createInspector**(`config?`): `void`

Creates the inspector window.

#### Parameters

| Name | Type |
| :------ | :------ |
| `config?` | `Partial`[`IInspectorOptions`](../interfaces/IInspectorOptions.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Debug/debugLayer.ts:216

___

### \_getGlobalInspector

▸ `Private` **_getGlobalInspector**(): `any`

Get the inspector from bundle or global

#### Returns

`any`

#### Defined in

packages/dev/core/src/Debug/debugLayer.ts:271

___

### hide

▸ **hide**(): `void`

Hide the inspector and close its window.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Debug/debugLayer.ts:296

___

### isVisible

▸ **isVisible**(): `boolean`

Get if the inspector is visible or not.

#### Returns

`boolean`

true if visible otherwise, false

#### Defined in

packages/dev/core/src/Debug/debugLayer.ts:289

___

### select

▸ **select**(`entity`, `lineContainerTitles?`): `void`

Select a specific entity in the scene explorer and highlight a specific block in that entity property grid

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `entity` | `any` | defines the entity to select |
| `lineContainerTitles?` | `string` \| `string`[] | defines the specific blocks to highlight (could be a string or an array of strings) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Debug/debugLayer.ts:257

___

### setAsActiveScene

▸ **setAsActiveScene**(): `void`

Update the scene in the inspector

#### Returns

`void`

#### Defined in

packages/dev/core/src/Debug/debugLayer.ts:305

___

### show

▸ **show**(`config?`): `Promise`[`DebugLayer`](DebugLayer.md)

Launch the debugLayer.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `config?` | [`IInspectorOptions`](../interfaces/IInspectorOptions.md) | Define the configuration of the inspector |

#### Returns

`Promise`[`DebugLayer`](DebugLayer.md)

a promise fulfilled when the debug layer is visible

#### Defined in

packages/dev/core/src/Debug/debugLayer.ts:316
