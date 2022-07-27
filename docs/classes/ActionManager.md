[@dev/core](../README.md) / [Exports](../modules.md) / ActionManager

# Class: ActionManager

Action Manager manages all events to be triggered on a given mesh or the global scene.
A single scene can have many Action Managers to handle predefined actions on specific meshes.

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions

## Hierarchy

- [`AbstractActionManager`](AbstractActionManager.md)

  ↳ **`ActionManager`**

## Table of contents

### Constructors

- [constructor](ActionManager.md#constructor)

### Properties

- [\_scene](ActionManager.md#_scene)
- [actions](ActionManager.md#actions)
- [hoverCursor](ActionManager.md#hovercursor)
- [isRecursive](ActionManager.md#isrecursive)
- [NothingTrigger](ActionManager.md#nothingtrigger)
- [OnCenterPickTrigger](ActionManager.md#oncenterpicktrigger)
- [OnDoublePickTrigger](ActionManager.md#ondoublepicktrigger)
- [OnEveryFrameTrigger](ActionManager.md#oneveryframetrigger)
- [OnIntersectionEnterTrigger](ActionManager.md#onintersectionentertrigger)
- [OnIntersectionExitTrigger](ActionManager.md#onintersectionexittrigger)
- [OnKeyDownTrigger](ActionManager.md#onkeydowntrigger)
- [OnKeyUpTrigger](ActionManager.md#onkeyuptrigger)
- [OnLeftPickTrigger](ActionManager.md#onleftpicktrigger)
- [OnLongPressTrigger](ActionManager.md#onlongpresstrigger)
- [OnPickDownTrigger](ActionManager.md#onpickdowntrigger)
- [OnPickOutTrigger](ActionManager.md#onpickouttrigger)
- [OnPickTrigger](ActionManager.md#onpicktrigger)
- [OnPickUpTrigger](ActionManager.md#onpickuptrigger)
- [OnPointerOutTrigger](ActionManager.md#onpointerouttrigger)
- [OnPointerOverTrigger](ActionManager.md#onpointerovertrigger)
- [OnRightPickTrigger](ActionManager.md#onrightpicktrigger)
- [Triggers](ActionManager.md#triggers)

### Accessors

- [hasPickTriggers](ActionManager.md#haspicktriggers)
- [hasPointerTriggers](ActionManager.md#haspointertriggers)
- [HasPickTriggers](ActionManager.md#haspicktriggers-1)
- [HasTriggers](ActionManager.md#hastriggers)

### Methods

- [dispose](ActionManager.md#dispose)
- [getScene](ActionManager.md#getscene)
- [hasSpecificTrigger](ActionManager.md#hasspecifictrigger)
- [hasSpecificTriggers](ActionManager.md#hasspecifictriggers)
- [hasSpecificTriggers2](ActionManager.md#hasspecifictriggers2)
- [processTrigger](ActionManager.md#processtrigger)
- [registerAction](ActionManager.md#registeraction)
- [serialize](ActionManager.md#serialize)
- [unregisterAction](ActionManager.md#unregisteraction)
- [GetTriggerName](ActionManager.md#gettriggername)
- [HasSpecificTrigger](ActionManager.md#hasspecifictrigger-1)
- [Parse](ActionManager.md#parse)

## Constructors

### constructor

• **new ActionManager**(`scene?`)

Creates a new action manager

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene?` | [`Nullable`](../modules.md#nullable)[`Scene`](Scene.md) | defines the hosting scene |

#### Overrides

[AbstractActionManager](AbstractActionManager.md).[constructor](AbstractActionManager.md#constructor)

#### Defined in

packages/dev/core/src/Actions/actionManager.ts:133

## Properties

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/Actions/actionManager.ts:127

___

### actions

• **actions**: [`IAction`](../interfaces/IAction.md)[]

Gets the list of actions

#### Inherited from

[AbstractActionManager](AbstractActionManager.md).[actions](AbstractActionManager.md#actions)

#### Defined in

packages/dev/core/src/Actions/abstractActionManager.ts:20

___

### hoverCursor

• **hoverCursor**: `string` = `""`

Gets the cursor to use when hovering items

#### Inherited from

[AbstractActionManager](AbstractActionManager.md).[hoverCursor](AbstractActionManager.md#hovercursor)

#### Defined in

packages/dev/core/src/Actions/abstractActionManager.ts:17

___

### isRecursive

• **isRecursive**: `boolean` = `false`

Gets or sets a boolean indicating that the manager is recursive meaning that it can trigger action from children

#### Inherited from

[AbstractActionManager](AbstractActionManager.md).[isRecursive](AbstractActionManager.md#isrecursive)

#### Defined in

packages/dev/core/src/Actions/abstractActionManager.ts:25

___

### NothingTrigger

▪ `Static` `Readonly` **NothingTrigger**: ``0``

Nothing

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions#triggers

#### Defined in

packages/dev/core/src/Actions/actionManager.ts:29

___

### OnCenterPickTrigger

▪ `Static` `Readonly` **OnCenterPickTrigger**: ``4``

On center pick

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions#triggers

#### Defined in

packages/dev/core/src/Actions/actionManager.ts:53

___

### OnDoublePickTrigger

▪ `Static` `Readonly` **OnDoublePickTrigger**: ``6``

On double pick

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions#triggers

#### Defined in

packages/dev/core/src/Actions/actionManager.ts:65

___

### OnEveryFrameTrigger

▪ `Static` `Readonly` **OnEveryFrameTrigger**: ``11``

On every frame

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions#triggers

#### Defined in

packages/dev/core/src/Actions/actionManager.ts:101

___

### OnIntersectionEnterTrigger

▪ `Static` `Readonly` **OnIntersectionEnterTrigger**: ``12``

On intersection enter

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions#triggers

#### Defined in

packages/dev/core/src/Actions/actionManager.ts:106

___

### OnIntersectionExitTrigger

▪ `Static` `Readonly` **OnIntersectionExitTrigger**: ``13``

On intersection exit

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions#triggers

#### Defined in

packages/dev/core/src/Actions/actionManager.ts:112

___

### OnKeyDownTrigger

▪ `Static` `Readonly` **OnKeyDownTrigger**: ``14``

On key down

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions#triggers

#### Defined in

packages/dev/core/src/Actions/actionManager.ts:118

___

### OnKeyUpTrigger

▪ `Static` `Readonly` **OnKeyUpTrigger**: ``15``

On key up

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions#triggers

#### Defined in

packages/dev/core/src/Actions/actionManager.ts:124

___

### OnLeftPickTrigger

▪ `Static` `Readonly` **OnLeftPickTrigger**: ``2``

On left pick

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions#triggers

#### Defined in

packages/dev/core/src/Actions/actionManager.ts:41

___

### OnLongPressTrigger

▪ `Static` `Readonly` **OnLongPressTrigger**: ``8``

On long press

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions#triggers

#### Defined in

packages/dev/core/src/Actions/actionManager.ts:83

___

### OnPickDownTrigger

▪ `Static` `Readonly` **OnPickDownTrigger**: ``5``

On pick down

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions#triggers

#### Defined in

packages/dev/core/src/Actions/actionManager.ts:59

___

### OnPickOutTrigger

▪ `Static` `Readonly` **OnPickOutTrigger**: ``16``

On pick out.
This trigger will only be raised if you also declared a OnPickDown

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions#triggers

#### Defined in

packages/dev/core/src/Actions/actionManager.ts:77

___

### OnPickTrigger

▪ `Static` `Readonly` **OnPickTrigger**: ``1``

On pick

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions#triggers

#### Defined in

packages/dev/core/src/Actions/actionManager.ts:35

___

### OnPickUpTrigger

▪ `Static` `Readonly` **OnPickUpTrigger**: ``7``

On pick up

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions#triggers

#### Defined in

packages/dev/core/src/Actions/actionManager.ts:71

___

### OnPointerOutTrigger

▪ `Static` `Readonly` **OnPointerOutTrigger**: ``10``

On pointer out

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions#triggers

#### Defined in

packages/dev/core/src/Actions/actionManager.ts:95

___

### OnPointerOverTrigger

▪ `Static` `Readonly` **OnPointerOverTrigger**: ``9``

On pointer over

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions#triggers

#### Defined in

packages/dev/core/src/Actions/actionManager.ts:89

___

### OnRightPickTrigger

▪ `Static` `Readonly` **OnRightPickTrigger**: ``3``

On right pick

**`See`**

https://doc.babylonjs.com/how_to/how_to_use_actions#triggers

#### Defined in

packages/dev/core/src/Actions/actionManager.ts:47

___

### Triggers

▪ `Static` **Triggers**: `Object` = `{}`

Gets the list of active triggers

#### Index signature

▪ [key: `string`]: `number`

#### Inherited from

[AbstractActionManager](AbstractActionManager.md).[Triggers](AbstractActionManager.md#triggers)

#### Defined in

packages/dev/core/src/Actions/abstractActionManager.ts:14

## Accessors

### hasPickTriggers

• `get` **hasPickTriggers**(): `boolean`

Does this action manager has pick triggers

#### Returns

`boolean`

#### Overrides

AbstractActionManager.hasPickTriggers

#### Defined in

packages/dev/core/src/Actions/actionManager.ts:251

___

### hasPointerTriggers

• `get` **hasPointerTriggers**(): `boolean`

Does this action manager has pointer triggers

#### Returns

`boolean`

#### Overrides

AbstractActionManager.hasPointerTriggers

#### Defined in

packages/dev/core/src/Actions/actionManager.ts:236

___

### HasPickTriggers

• `Static` `get` **HasPickTriggers**(): `boolean`

Does exist one action manager with at least one pick trigger

#### Returns

`boolean`

#### Inherited from

AbstractActionManager.HasPickTriggers

#### Defined in

packages/dev/core/src/Actions/abstractActionManager.ts:109

___

### HasTriggers

• `Static` `get` **HasTriggers**(): `boolean`

Does exist one action manager with at least one trigger

#### Returns

`boolean`

#### Inherited from

AbstractActionManager.HasTriggers

#### Defined in

packages/dev/core/src/Actions/abstractActionManager.ts:97

## Methods

### dispose

▸ **dispose**(): `void`

Releases all associated resources

#### Returns

`void`

#### Overrides

[AbstractActionManager](AbstractActionManager.md).[dispose](AbstractActionManager.md#dispose)

#### Defined in

packages/dev/core/src/Actions/actionManager.ts:149

___

### getScene

▸ **getScene**(): [`Scene`](Scene.md)

Gets hosting scene

#### Returns

[`Scene`](Scene.md)

the hosting scene

#### Defined in

packages/dev/core/src/Actions/actionManager.ts:169

___

### hasSpecificTrigger

▸ **hasSpecificTrigger**(`trigger`, `parameterPredicate?`): `boolean`

Does this action manager handles actions of a given trigger

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `trigger` | `number` | defines the trigger to be tested |
| `parameterPredicate?` | (`parameter`: `any`) => `boolean` | defines an optional predicate to filter triggers by parameter |

#### Returns

`boolean`

whether the trigger is handled

#### Overrides

[AbstractActionManager](AbstractActionManager.md).[hasSpecificTrigger](AbstractActionManager.md#hasspecifictrigger)

#### Defined in

packages/dev/core/src/Actions/actionManager.ts:215

___

### hasSpecificTriggers

▸ **hasSpecificTriggers**(`triggers`): `boolean`

Does this action manager handles actions of any of the given triggers

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `triggers` | `number`[] | defines the triggers to be tested |

#### Returns

`boolean`

a boolean indicating whether one (or more) of the triggers is handled

#### Overrides

[AbstractActionManager](AbstractActionManager.md).[hasSpecificTriggers](AbstractActionManager.md#hasspecifictriggers)

#### Defined in

packages/dev/core/src/Actions/actionManager.ts:178

___

### hasSpecificTriggers2

▸ **hasSpecificTriggers2**(`triggerA`, `triggerB`): `boolean`

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

#### Overrides

[AbstractActionManager](AbstractActionManager.md).[hasSpecificTriggers2](AbstractActionManager.md#hasspecifictriggers2)

#### Defined in

packages/dev/core/src/Actions/actionManager.ts:197

___

### processTrigger

▸ **processTrigger**(`trigger`, `evt?`): `void`

Process a specific trigger

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `trigger` | `number` | defines the trigger to process |
| `evt?` | [`IActionEvent`](../interfaces/IActionEvent.md) | defines the event details to be processed |

#### Returns

`void`

#### Overrides

[AbstractActionManager](AbstractActionManager.md).[processTrigger](AbstractActionManager.md#processtrigger)

#### Defined in

packages/dev/core/src/Actions/actionManager.ts:314

___

### registerAction

▸ **registerAction**(`action`): [`Nullable`](../modules.md#nullable)[`IAction`](../interfaces/IAction.md)

Registers an action to this action manager

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `action` | [`IAction`](../interfaces/IAction.md) | defines the action to be registered |

#### Returns

[`Nullable`](../modules.md#nullable)[`IAction`](../interfaces/IAction.md)

the action amended (prepared) after registration

#### Overrides

[AbstractActionManager](AbstractActionManager.md).[registerAction](AbstractActionManager.md#registeraction)

#### Defined in

packages/dev/core/src/Actions/actionManager.ts:268

___

### serialize

▸ **serialize**(`name`): `any`

Serialize this manager to a JSON object

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the property name to store this manager |

#### Returns

`any`

a JSON representation of this manager

#### Overrides

[AbstractActionManager](AbstractActionManager.md).[serialize](AbstractActionManager.md#serialize)

#### Defined in

packages/dev/core/src/Actions/actionManager.ts:375

___

### unregisterAction

▸ **unregisterAction**(`action`): `Boolean`

Unregisters an action to this action manager

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `action` | [`IAction`](../interfaces/IAction.md) | defines the action to be unregistered |

#### Returns

`Boolean`

a boolean indicating whether the action has been unregistered

#### Overrides

[AbstractActionManager](AbstractActionManager.md).[unregisterAction](AbstractActionManager.md#unregisteraction)

#### Defined in

packages/dev/core/src/Actions/actionManager.ts:295

___

### GetTriggerName

▸ `Static` **GetTriggerName**(`trigger`): `string`

Get a trigger name by index

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `trigger` | `number` | defines the trigger index |

#### Returns

`string`

a trigger name

#### Defined in

packages/dev/core/src/Actions/actionManager.ts:634

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

#### Inherited from

[AbstractActionManager](AbstractActionManager.md).[HasSpecificTrigger](AbstractActionManager.md#hasspecifictrigger-1)

#### Defined in

packages/dev/core/src/Actions/abstractActionManager.ts:126

___

### Parse

▸ `Static` **Parse**(`parsedActions`, `object`, `scene`): `void`

Creates a new ActionManager from a JSON data

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `parsedActions` | `any` | defines the JSON data to read from |
| `object` | [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md) | defines the hosting mesh |
| `scene` | [`Scene`](Scene.md) | defines the hosting scene |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Actions/actionManager.ts:424
