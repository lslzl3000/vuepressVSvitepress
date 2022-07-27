[@dev/core](../README.md) / [Exports](../modules.md) / ShadowGeneratorSceneComponent

# Class: ShadowGeneratorSceneComponent

Defines the shadow generator component responsible to manage any shadow generators
in a given scene.

## Implements

- [`ISceneSerializableComponent`](../interfaces/ISceneSerializableComponent.md)

## Table of contents

### Constructors

- [constructor](ShadowGeneratorSceneComponent.md#constructor)

### Properties

- [name](ShadowGeneratorSceneComponent.md#name)
- [scene](ShadowGeneratorSceneComponent.md#scene)

### Methods

- [\_gatherRenderTargets](ShadowGeneratorSceneComponent.md#_gatherrendertargets)
- [addFromContainer](ShadowGeneratorSceneComponent.md#addfromcontainer)
- [dispose](ShadowGeneratorSceneComponent.md#dispose)
- [rebuild](ShadowGeneratorSceneComponent.md#rebuild)
- [register](ShadowGeneratorSceneComponent.md#register)
- [removeFromContainer](ShadowGeneratorSceneComponent.md#removefromcontainer)
- [serialize](ShadowGeneratorSceneComponent.md#serialize)

## Constructors

### constructor

• **new ShadowGeneratorSceneComponent**(`scene`)

Creates a new instance of the component for the given scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `scene` | [`Scene`](Scene.md) | Defines the scene to register the component in |

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGeneratorSceneComponent.ts:44

## Properties

### name

• `Readonly` **name**: ``"ShadowGenerator"``

The component name helpful to identify the component in the list of scene components.

#### Implementation of

[ISceneSerializableComponent](../interfaces/ISceneSerializableComponent.md).[name](../interfaces/ISceneSerializableComponent.md#name)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGeneratorSceneComponent.ts:33

___

### scene

• **scene**: [`Scene`](Scene.md)

The scene the component belongs to.

#### Implementation of

[ISceneSerializableComponent](../interfaces/ISceneSerializableComponent.md).[scene](../interfaces/ISceneSerializableComponent.md#scene)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGeneratorSceneComponent.ts:38

## Methods

### \_gatherRenderTargets

▸ `Private` **_gatherRenderTargets**(`renderTargets`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `renderTargets` | [`SmartArrayNoDuplicate`](SmartArrayNoDuplicate.md)[`RenderTargetTexture`](RenderTargetTexture.md) |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGeneratorSceneComponent.ts:106

___

### addFromContainer

▸ **addFromContainer**(`container`): `void`

Adds all the elements from the container to the scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `container` | [`AbstractScene`](AbstractScene.md) | the container holding the elements |

#### Returns

`void`

#### Implementation of

[ISceneSerializableComponent](../interfaces/ISceneSerializableComponent.md).[addFromContainer](../interfaces/ISceneSerializableComponent.md#addfromcontainer)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGeneratorSceneComponent.ts:84

___

### dispose

▸ **dispose**(): `void`

Rebuilds the elements related to this component in case of
context lost for instance.

#### Returns

`void`

#### Implementation of

[ISceneSerializableComponent](../interfaces/ISceneSerializableComponent.md).[dispose](../interfaces/ISceneSerializableComponent.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGeneratorSceneComponent.ts:102

___

### rebuild

▸ **rebuild**(): `void`

Rebuilds the elements related to this component in case of
context lost for instance.

#### Returns

`void`

#### Implementation of

[ISceneSerializableComponent](../interfaces/ISceneSerializableComponent.md).[rebuild](../interfaces/ISceneSerializableComponent.md#rebuild)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGeneratorSceneComponent.ts:59

___

### register

▸ **register**(): `void`

Registers the component in a given scene

#### Returns

`void`

#### Implementation of

[ISceneSerializableComponent](../interfaces/ISceneSerializableComponent.md).[register](../interfaces/ISceneSerializableComponent.md#register)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGeneratorSceneComponent.ts:51

___

### removeFromContainer

▸ **removeFromContainer**(`container`, `dispose?`): `void`

Removes all the elements in the container from the scene

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `container` | [`AbstractScene`](AbstractScene.md) | contains the elements to remove |
| `dispose?` | `boolean` | if the removed element should be disposed (default: false) |

#### Returns

`void`

#### Implementation of

[ISceneSerializableComponent](../interfaces/ISceneSerializableComponent.md).[removeFromContainer](../interfaces/ISceneSerializableComponent.md#removefromcontainer)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGeneratorSceneComponent.ts:94

___

### serialize

▸ **serialize**(`serializationObject`): `void`

Serializes the component data to the specified json object

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `serializationObject` | `any` | The object to serialize to |

#### Returns

`void`

#### Implementation of

[ISceneSerializableComponent](../interfaces/ISceneSerializableComponent.md).[serialize](../interfaces/ISceneSerializableComponent.md#serialize)

#### Defined in

https://github.com/babylon.js/core/src/Lights/Shadows/shadowGeneratorSceneComponent.ts:67
