[@dev/core](../README.md) / [Exports](../modules.md) / AbstractActionManager

# Class: AbstractActionManager

Abstract class used to decouple action Manager from scene and meshes.
Do not instantiate.

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions

## Hierarchy

- **`AbstractActionManager`**

  ↳ [`ActionManager`](ActionManager.md)

## Implements

- [`IDisposable`](../interfaces/IDisposable.md)

## Table of contents

### Constructors

- [constructor](AbstractActionManager.md#constructor)

### Properties

- [actions](AbstractActionManager.md#actions)
- [hoverCursor](AbstractActionManager.md#hovercursor)
- [isRecursive](AbstractActionManager.md#isrecursive)
- [Triggers](AbstractActionManager.md#triggers)

### Accessors

- [hasPickTriggers](AbstractActionManager.md#haspicktriggers)
- [hasPointerTriggers](AbstractActionManager.md#haspointertriggers)
- [HasPickTriggers](AbstractActionManager.md#haspicktriggers-1)
- [HasTriggers](AbstractActionManager.md#hastriggers)

### Methods

- [dispose](AbstractActionManager.md#dispose)
- [hasSpecificTrigger](AbstractActionManager.md#hasspecifictrigger)
- [hasSpecificTriggers](AbstractActionManager.md#hasspecifictriggers)
- [hasSpecificTriggers2](AbstractActionManager.md#hasspecifictriggers2)
- [processTrigger](AbstractActionManager.md#processtrigger)
- [registerAction](AbstractActionManager.md#registeraction)
- [serialize](AbstractActionManager.md#serialize)
- [unregisterAction](AbstractActionManager.md#unregisteraction)
- [HasSpecificTrigger](AbstractActionManager.md#hasspecifictrigger-1)

## Constructors

### constructor

• **new AbstractActionManager**()

## Properties

### actions

• **actions**: [`IAction`](../interfaces/IAction.md)[]

Gets the list of actions

#### Defined in

https://github.com/babylon.js/core/src/Actions/abstractActionManager.ts:20

___

### hoverCursor

• **hoverCursor**: `string` = `""`

Gets the cursor to use when hovering items

#### Defined in

https://github.com/babylon.js/core/src/Actions/abstractActionManager.ts:17

___

### isRecursive

• **isRecursive**: `boolean` = `false`

Gets or sets a boolean indicating that the manager is recursive meaning that it can trigger action from children

#### Defined in

https://github.com/babylon.js/core/src/Actions/abstractActionManager.ts:25

___

### Triggers

▪ `Static` **Triggers**: `Object` = `{}`

Gets the list of active triggers

#### Index signature

▪ [key: `string`]: `number`

#### Defined in

https://github.com/babylon.js/core/src/Actions/abstractActionManager.ts:14

## Accessors

### hasPickTriggers

• `Abstract` `get` **hasPickTriggers**(): `boolean`

Does this action manager has pick triggers

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Actions/abstractActionManager.ts:40

___

### hasPointerTriggers

• `Abstract` `get` **hasPointerTriggers**(): `boolean`

Does this action manager has pointer triggers

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Actions/abstractActionManager.ts:35

___

### HasPickTriggers

• `Static` `get` **HasPickTriggers**(): `boolean`

Does exist one action manager with at least one pick trigger

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Actions/abstractActionManager.ts:109

___

### HasTriggers

• `Static` `get` **HasTriggers**(): `boolean`

Does exist one action manager with at least one trigger

#### Returns

`boolean`

#### Defined in

https://github.com/babylon.js/core/src/Actions/abstractActionManager.ts:97

## Methods

### dispose

▸ `Abstract` **dispose**(): `void`

Releases all associated resources

#### Returns

`void`

#### Implementation of

[IDisposable](../interfaces/IDisposable.md).[dispose](../interfaces/IDisposable.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Actions/abstractActionManager.ts:30

___

### hasSpecificTrigger

▸ `Abstract` **hasSpecificTrigger**(`trigger`, `parameterPredicate?`): `boolean`

Does this action manager handles actions of a given trigger

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `trigger` | `number` | defines the trigger to be tested |
| `parameterPredicate?` | (`parameter`: `any`) => `boolean` | defines an optional predicate to filter triggers by parameter |

#### Returns

`boolean`

whether the trigger is handled

#### Defined in

https://github.com/babylon.js/core/src/Actions/abstractActionManager.ts:71

___

### hasSpecificTriggers

▸ `Abstract` **hasSpecificTriggers**(`triggers`): `boolean`

Does this action manager handles actions of any of the given triggers

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `triggers` | `number`[] | defines the triggers to be tested |

#### Returns

`boolean`

a boolean indicating whether one (or more) of the triggers is handled

#### Defined in

https://github.com/babylon.js/core/src/Actions/abstractActionManager.ts:54

___

### hasSpecificTriggers2

▸ `Abstract` **hasSpecificTriggers2**(`triggerA`, `triggerB`): `boolean`

Does this action manager handles actions of any of the given triggers. This function takes two arguments for
speed.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `triggerA` | `number` | defines the trigger to be tested |
| `triggerB` | `number` | defines the trigger to be tested |

#### Returns

`boolean`

a boolean indicating whether one (or more) of the triggers is handled

#### Defined in

https://github.com/babylon.js/core/src/Actions/abstractActionManager.ts:63

___

### processTrigger

▸ `Abstract` **processTrigger**(`trigger`, `evt?`): `void`

Process a specific trigger

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `trigger` | `number` | defines the trigger to process |
| `evt?` | [`IActionEvent`](../interfaces/IActionEvent.md) | defines the event details to be processed |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Actions/abstractActionManager.ts:47

___

### registerAction

▸ `Abstract` **registerAction**(`action`): [`Nullable`](../modules.md#nullable)[`IAction`](../interfaces/IAction.md)

Registers an action to this action manager

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `action` | [`IAction`](../interfaces/IAction.md) | defines the action to be registered |

#### Returns

[`Nullable`](../modules.md#nullable)[`IAction`](../interfaces/IAction.md)

the action amended (prepared) after registration

#### Defined in

https://github.com/babylon.js/core/src/Actions/abstractActionManager.ts:85

___

### serialize

▸ `Abstract` **serialize**(`name`): `any`

Serialize this manager to a JSON object

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the property name to store this manager |

#### Returns

`any`

a JSON representation of this manager

#### Defined in

https://github.com/babylon.js/core/src/Actions/abstractActionManager.ts:78

___

### unregisterAction

▸ `Abstract` **unregisterAction**(`action`): `Boolean`

Unregisters an action to this action manager

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `action` | [`IAction`](../interfaces/IAction.md) | defines the action to be unregistered |

#### Returns

`Boolean`

a boolean indicating whether the action has been unregistered

#### Defined in

https://github.com/babylon.js/core/src/Actions/abstractActionManager.ts:92

___

### HasSpecificTrigger

▸ `Static` **HasSpecificTrigger**(`trigger`): `boolean`

Does exist one action manager that handles actions of a given trigger

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `trigger` | `number` | defines the trigger to be tested |

#### Returns

`boolean`

a boolean indicating whether the trigger is handled by at least one action manager

#### Defined in

https://github.com/babylon.js/core/src/Actions/abstractActionManager.ts:126
