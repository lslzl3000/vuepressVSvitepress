[@dev/core](../README.md) / [Exports](../modules.md) / Sprite

# Class: Sprite

Class used to represent a sprite

**`See`**

https://doc.babylonjs.com/babylon101/sprites

## Hierarchy

- `ThinSprite`

  ↳ **`Sprite`**

## Implements

- [`IAnimatable`](../interfaces/IAnimatable.md)

## Table of contents

### Constructors

- [constructor](Sprite.md#constructor)

### Properties

- [\_delay](Sprite.md#_delay)
- [\_fromIndex](Sprite.md#_fromindex)
- [\_loopAnimation](Sprite.md#_loopanimation)
- [\_manager](Sprite.md#_manager)
- [\_onAnimationEnd](Sprite.md#_onanimationend)
- [\_toIndex](Sprite.md#_toindex)
- [actionManager](Sprite.md#actionmanager)
- [angle](Sprite.md#angle)
- [animations](Sprite.md#animations)
- [cellIndex](Sprite.md#cellindex)
- [cellRef](Sprite.md#cellref)
- [color](Sprite.md#color)
- [disposeWhenFinishedAnimating](Sprite.md#disposewhenfinishedanimating)
- [height](Sprite.md#height)
- [invertU](Sprite.md#invertu)
- [invertV](Sprite.md#invertv)
- [isPickable](Sprite.md#ispickable)
- [isVisible](Sprite.md#isvisible)
- [name](Sprite.md#name)
- [onDisposeObservable](Sprite.md#ondisposeobservable)
- [position](Sprite.md#position)
- [uniqueId](Sprite.md#uniqueid)
- [useAlphaForPicking](Sprite.md#usealphaforpicking)
- [width](Sprite.md#width)

### Accessors

- [animationStarted](Sprite.md#animationstarted)
- [delay](Sprite.md#delay)
- [fromIndex](Sprite.md#fromindex)
- [loopAnimation](Sprite.md#loopanimation)
- [manager](Sprite.md#manager)
- [size](Sprite.md#size)
- [toIndex](Sprite.md#toindex)

### Methods

- [\_endAnimation](Sprite.md#_endanimation)
- [dispose](Sprite.md#dispose)
- [getClassName](Sprite.md#getclassname)
- [playAnimation](Sprite.md#playanimation)
- [serialize](Sprite.md#serialize)
- [stopAnimation](Sprite.md#stopanimation)
- [Parse](Sprite.md#parse)

## Constructors

### constructor

• **new Sprite**(`name`, `manager`)

Creates a new Sprite

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | defines the name |
| `manager` | [`ISpriteManager`](../interfaces/ISpriteManager.md) | defines the manager |

#### Overrides

ThinSprite.constructor

#### Defined in

packages/dev/core/src/Sprites/sprite.ts:72

## Properties

### \_delay

• `Protected` **\_delay**: `number` = `0`

#### Inherited from

ThinSprite.\_delay

#### Defined in

packages/dev/core/src/Sprites/thinSprite.ts:71

___

### \_fromIndex

• `Protected` **\_fromIndex**: `number` = `0`

#### Inherited from

ThinSprite.\_fromIndex

#### Defined in

packages/dev/core/src/Sprites/thinSprite.ts:69

___

### \_loopAnimation

• `Protected` **\_loopAnimation**: `boolean` = `false`

#### Inherited from

ThinSprite.\_loopAnimation

#### Defined in

packages/dev/core/src/Sprites/thinSprite.ts:68

___

### \_manager

• `Private` **\_manager**: [`ISpriteManager`](../interfaces/ISpriteManager.md)

#### Defined in

packages/dev/core/src/Sprites/sprite.ts:40

___

### \_onAnimationEnd

• `Private` **\_onAnimationEnd**: [`Nullable`](../modules.md#nullable)() => `void` = `null`

#### Defined in

packages/dev/core/src/Sprites/sprite.ts:41

___

### \_toIndex

• `Protected` **\_toIndex**: `number` = `0`

#### Inherited from

ThinSprite.\_toIndex

#### Defined in

packages/dev/core/src/Sprites/thinSprite.ts:70

___

### actionManager

• **actionManager**: [`Nullable`](../modules.md#nullable)[`ActionManager`](ActionManager.md)

Gets or sets the associated action manager

#### Defined in

packages/dev/core/src/Sprites/sprite.ts:33

___

### angle

• **angle**: `number` = `0`

Gets or sets rotation angle

#### Inherited from

ThinSprite.angle

#### Defined in

packages/dev/core/src/Sprites/thinSprite.ts:23

___

### animations

• **animations**: [`Nullable`](../modules.md#nullable)[`Animation`](Animation.md)[]

Gets the list of attached animations

#### Implementation of

[IAnimatable](../interfaces/IAnimatable.md).[animations](../interfaces/IAnimatable.md#animations)

#### Defined in

packages/dev/core/src/Sprites/sprite.ts:24

___

### cellIndex

• **cellIndex**: `number`

Gets or sets the cell index in the sprite sheet

#### Inherited from

ThinSprite.cellIndex

#### Defined in

packages/dev/core/src/Sprites/thinSprite.ts:11

___

### cellRef

• **cellRef**: `string`

Gets or sets the cell reference in the sprite sheet, uses sprite's filename when added to sprite sheet

#### Inherited from

ThinSprite.cellRef

#### Defined in

packages/dev/core/src/Sprites/thinSprite.ts:13

___

### color

• **color**: [`Color4`](Color4.md)

Gets or sets the main color

#### Overrides

ThinSprite.color

#### Defined in

packages/dev/core/src/Sprites/sprite.ts:20

___

### disposeWhenFinishedAnimating

• **disposeWhenFinishedAnimating**: `boolean`

Gets or sets a boolean indicating that this sprite should be disposed after animation ends

#### Defined in

packages/dev/core/src/Sprites/sprite.ts:22

___

### height

• **height**: `number` = `1.0`

Gets or sets the height

#### Inherited from

ThinSprite.height

#### Defined in

packages/dev/core/src/Sprites/thinSprite.ts:21

___

### invertU

• **invertU**: `boolean` = `false`

Gets or sets a boolean indicating if UV coordinates should be inverted in U axis

#### Inherited from

ThinSprite.invertU

#### Defined in

packages/dev/core/src/Sprites/thinSprite.ts:25

___

### invertV

• **invertV**: `boolean` = `false`

Gets or sets a boolean indicating if UV coordinates should be inverted in B axis

#### Inherited from

ThinSprite.invertV

#### Defined in

packages/dev/core/src/Sprites/thinSprite.ts:27

___

### isPickable

• **isPickable**: `boolean` = `false`

Gets or sets a boolean indicating if the sprite can be picked

#### Defined in

packages/dev/core/src/Sprites/sprite.ts:26

___

### isVisible

• **isVisible**: `boolean` = `true`

Gets or sets a boolean indicating if the sprite is visible (renderable). Default is true

#### Inherited from

ThinSprite.isVisible

#### Defined in

packages/dev/core/src/Sprites/thinSprite.ts:29

___

### name

• **name**: `string`

#### Defined in

packages/dev/core/src/Sprites/sprite.ts:74

___

### onDisposeObservable

• **onDisposeObservable**: [`Observable`](Observable.md)[`Sprite`](Sprite.md)

An event triggered when the control has been disposed

#### Defined in

packages/dev/core/src/Sprites/sprite.ts:38

___

### position

• **position**: [`Vector3`](Vector3.md)

Gets or sets the current world position

#### Overrides

ThinSprite.position

#### Defined in

packages/dev/core/src/Sprites/sprite.ts:18

___

### uniqueId

• **uniqueId**: `number`

Gets or sets the unique id of the sprite

#### Defined in

packages/dev/core/src/Sprites/sprite.ts:58

___

### useAlphaForPicking

• **useAlphaForPicking**: `boolean` = `false`

Gets or sets a boolean indicating that sprite texture alpha will be used for precise picking (false by default)

#### Defined in

packages/dev/core/src/Sprites/sprite.ts:28

___

### width

• **width**: `number` = `1.0`

Gets or sets the width

#### Inherited from

ThinSprite.width

#### Defined in

packages/dev/core/src/Sprites/thinSprite.ts:19

## Accessors

### animationStarted

• `get` **animationStarted**(): `boolean`

Returns a boolean indicating if the animation is started

#### Returns

`boolean`

#### Inherited from

ThinSprite.animationStarted

#### Defined in

packages/dev/core/src/Sprites/thinSprite.ts:34

___

### delay

• `get` **delay**(): `number`

Gets or sets the delay between cell changes (setting it will restart the animation)

#### Returns

`number`

#### Overrides

ThinSprite.delay

#### Defined in

packages/dev/core/src/Sprites/sprite.ts:119

• `set` **delay**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Overrides

ThinSprite.delay

#### Defined in

packages/dev/core/src/Sprites/sprite.ts:122

___

### fromIndex

• `get` **fromIndex**(): `number`

Gets or sets the initial key for the animation (setting it will restart the animation)

#### Returns

`number`

#### Overrides

ThinSprite.fromIndex

#### Defined in

packages/dev/core/src/Sprites/sprite.ts:95

• `set` **fromIndex**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Overrides

ThinSprite.fromIndex

#### Defined in

packages/dev/core/src/Sprites/sprite.ts:98

___

### loopAnimation

• `get` **loopAnimation**(): `boolean`

Gets or sets a boolean indicating if the animation is looping (setting it will restart the animation)

#### Returns

`boolean`

#### Overrides

ThinSprite.loopAnimation

#### Defined in

packages/dev/core/src/Sprites/sprite.ts:111

• `set` **loopAnimation**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Overrides

ThinSprite.loopAnimation

#### Defined in

packages/dev/core/src/Sprites/sprite.ts:114

___

### manager

• `get` **manager**(): [`ISpriteManager`](../interfaces/ISpriteManager.md)

Gets the manager of this sprite

#### Returns

[`ISpriteManager`](../interfaces/ISpriteManager.md)

#### Defined in

packages/dev/core/src/Sprites/sprite.ts:63

___

### size

• `get` **size**(): `number`

Gets or sets the sprite size

#### Returns

`number`

#### Defined in

packages/dev/core/src/Sprites/sprite.ts:46

• `set` **size**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Sprites/sprite.ts:50

___

### toIndex

• `get` **toIndex**(): `number`

Gets or sets the end key for the animation (setting it will restart the animation)

#### Returns

`number`

#### Overrides

ThinSprite.toIndex

#### Defined in

packages/dev/core/src/Sprites/sprite.ts:103

• `set` **toIndex**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Overrides

ThinSprite.toIndex

#### Defined in

packages/dev/core/src/Sprites/sprite.ts:106

## Methods

### \_endAnimation

▸ `Private` **_endAnimation**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Sprites/sprite.ts:140

___

### dispose

▸ **dispose**(): `void`

Release associated resources

#### Returns

`void`

#### Defined in

packages/dev/core/src/Sprites/sprite.ts:150

___

### getClassName

▸ **getClassName**(): `string`

Returns the string "Sprite"

#### Returns

`string`

"Sprite"

#### Defined in

packages/dev/core/src/Sprites/sprite.ts:90

___

### playAnimation

▸ **playAnimation**(`from`, `to`, `loop`, `delay`, `onAnimationEnd?`): `void`

Starts an animation

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `from` | `number` | `undefined` | defines the initial key |
| `to` | `number` | `undefined` | defines the end key |
| `loop` | `boolean` | `undefined` | defines if the animation must loop |
| `delay` | `number` | `undefined` | defines the start delay (in ms) |
| `onAnimationEnd` | [`Nullable`](../modules.md#nullable)() => `void` | `null` | defines a callback to call when animation ends |

#### Returns

`void`

#### Overrides

ThinSprite.playAnimation

#### Defined in

packages/dev/core/src/Sprites/sprite.ts:134

___

### serialize

▸ **serialize**(): `any`

Serializes the sprite to a JSON object

#### Returns

`any`

the JSON object

#### Defined in

packages/dev/core/src/Sprites/sprite.ts:166

___

### stopAnimation

▸ **stopAnimation**(): `void`

Stops current animation (if any)

#### Returns

`void`

#### Inherited from

ThinSprite.stopAnimation

#### Defined in

packages/dev/core/src/Sprites/thinSprite.ts:113

___

### Parse

▸ `Static` **Parse**(`parsedSprite`, `manager`): [`Sprite`](Sprite.md)

Parses a JSON object to create a new sprite

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `parsedSprite` | `any` | The JSON object to parse |
| `manager` | [`SpriteManager`](SpriteManager.md) | defines the hosting manager |

#### Returns

[`Sprite`](Sprite.md)

the new sprite

#### Defined in

packages/dev/core/src/Sprites/sprite.ts:199
