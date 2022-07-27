[@dev/core](../README.md) / [Exports](../modules.md) / IEditablePropertyOption

# Interface: IEditablePropertyOption

Interface that defines the options available for an editable property

## Table of contents

### Properties

- [max](IEditablePropertyOption.md#max)
- [min](IEditablePropertyOption.md#min)
- [notifiers](IEditablePropertyOption.md#notifiers)
- [options](IEditablePropertyOption.md#options)

## Properties

### max

• `Optional` **max**: `number`

max value

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialDecorator.ts:36

___

### min

• `Optional` **min**: `number`

min value

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialDecorator.ts:34

___

### notifiers

• `Optional` **notifiers**: `Object`

notifiers: indicates which actions to take when the property is changed

#### Type declaration

| Name | Type | Description |
| :------ | :------ | :------ |
| `activatePreviewCommand?` | `boolean` | the onPreviewCommandActivated observer of the preview manager should be triggered |
| `callback?` | (`scene`: [`Scene`](../classes/Scene.md)) => `void` | a callback to trigger |
| `rebuild?` | `boolean` | the material should be rebuilt |
| `update?` | `boolean` | the preview should be updated |

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialDecorator.ts:38

___

### options

• `Optional` **options**: [`IEditablePropertyListOption`](IEditablePropertyListOption.md)[]

list of the options for a variable of type list

#### Defined in

https://github.com/babylon.js/core/src/Materials/Node/nodeMaterialDecorator.ts:49
