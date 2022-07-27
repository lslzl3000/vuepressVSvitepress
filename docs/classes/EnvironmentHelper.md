[@dev/core](../README.md) / [Exports](../modules.md) / EnvironmentHelper

# Class: EnvironmentHelper

The Environment helper class can be used to add a fully featured none expensive background to your scene.
It includes by default a skybox and a ground relying on the BackgroundMaterial.
It also helps with the default setup of your imageProcessing configuration.

## Table of contents

### Constructors

- [constructor](EnvironmentHelper.md#constructor)

### Properties

- [\_ground](EnvironmentHelper.md#_ground)
- [\_groundMaterial](EnvironmentHelper.md#_groundmaterial)
- [\_groundMirror](EnvironmentHelper.md#_groundmirror)
- [\_groundTexture](EnvironmentHelper.md#_groundtexture)
- [\_options](EnvironmentHelper.md#_options)
- [\_rootMesh](EnvironmentHelper.md#_rootmesh)
- [\_scene](EnvironmentHelper.md#_scene)
- [\_skybox](EnvironmentHelper.md#_skybox)
- [\_skyboxMaterial](EnvironmentHelper.md#_skyboxmaterial)
- [\_skyboxTexture](EnvironmentHelper.md#_skyboxtexture)
- [onErrorObservable](EnvironmentHelper.md#onerrorobservable)
- [\_EnvironmentTextureCDNUrl](EnvironmentHelper.md#_environmenttexturecdnurl)
- [\_GroundTextureCDNUrl](EnvironmentHelper.md#_groundtexturecdnurl)
- [\_SkyboxTextureCDNUrl](EnvironmentHelper.md#_skyboxtexturecdnurl)

### Accessors

- [ground](EnvironmentHelper.md#ground)
- [groundMaterial](EnvironmentHelper.md#groundmaterial)
- [groundMirror](EnvironmentHelper.md#groundmirror)
- [groundMirrorRenderList](EnvironmentHelper.md#groundmirrorrenderlist)
- [groundTexture](EnvironmentHelper.md#groundtexture)
- [rootMesh](EnvironmentHelper.md#rootmesh)
- [skybox](EnvironmentHelper.md#skybox)
- [skyboxMaterial](EnvironmentHelper.md#skyboxmaterial)
- [skyboxTexture](EnvironmentHelper.md#skyboxtexture)

### Methods

- [\_errorHandler](EnvironmentHelper.md#_errorhandler)
- [\_getSceneSize](EnvironmentHelper.md#_getscenesize)
- [\_setupBackground](EnvironmentHelper.md#_setupbackground)
- [\_setupEnvironmentTexture](EnvironmentHelper.md#_setupenvironmenttexture)
- [\_setupGround](EnvironmentHelper.md#_setupground)
- [\_setupGroundDiffuseTexture](EnvironmentHelper.md#_setupgrounddiffusetexture)
- [\_setupGroundMaterial](EnvironmentHelper.md#_setupgroundmaterial)
- [\_setupGroundMirrorTexture](EnvironmentHelper.md#_setupgroundmirrortexture)
- [\_setupImageProcessing](EnvironmentHelper.md#_setupimageprocessing)
- [\_setupMirrorInGroundMaterial](EnvironmentHelper.md#_setupmirroringroundmaterial)
- [\_setupSkybox](EnvironmentHelper.md#_setupskybox)
- [\_setupSkyboxMaterial](EnvironmentHelper.md#_setupskyboxmaterial)
- [\_setupSkyboxReflectionTexture](EnvironmentHelper.md#_setupskyboxreflectiontexture)
- [dispose](EnvironmentHelper.md#dispose)
- [setMainColor](EnvironmentHelper.md#setmaincolor)
- [updateOptions](EnvironmentHelper.md#updateoptions)
- [\_GetDefaultOptions](EnvironmentHelper.md#_getdefaultoptions)

## Constructors

### constructor

• **new EnvironmentHelper**(`options`, `scene`)

constructor

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | `Partial`[`IEnvironmentHelperOptions`](../interfaces/IEnvironmentHelperOptions.md) | Defines the options we want to customize the helper |
| `scene` | [`Scene`](Scene.md) | The scene to add the material to |

#### Defined in

packages/dev/core/src/Helpers/environmentHelper.ts:340

## Properties

### \_ground

• `Private` **\_ground**: [`Nullable`](../modules.md#nullable)[`Mesh`](Mesh.md)

#### Defined in

packages/dev/core/src/Helpers/environmentHelper.ts:280

___

### \_groundMaterial

• `Private` **\_groundMaterial**: [`Nullable`](../modules.md#nullable)[`BackgroundMaterial`](BackgroundMaterial.md)

#### Defined in

packages/dev/core/src/Helpers/environmentHelper.ts:315

___

### \_groundMirror

• `Private` **\_groundMirror**: [`Nullable`](../modules.md#nullable)[`MirrorTexture`](MirrorTexture.md)

#### Defined in

packages/dev/core/src/Helpers/environmentHelper.ts:296

___

### \_groundTexture

• `Private` **\_groundTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

#### Defined in

packages/dev/core/src/Helpers/environmentHelper.ts:288

___

### \_options

• `Private` **\_options**: [`IEnvironmentHelperOptions`](../interfaces/IEnvironmentHelperOptions.md)

#### Defined in

packages/dev/core/src/Helpers/environmentHelper.ts:327

___

### \_rootMesh

• `Private` **\_rootMesh**: [`Mesh`](Mesh.md)

#### Defined in

packages/dev/core/src/Helpers/environmentHelper.ts:248

___

### \_scene

• `Private` `Readonly` **\_scene**: [`Scene`](Scene.md)

Stores the creation options.

#### Defined in

packages/dev/core/src/Helpers/environmentHelper.ts:326

___

### \_skybox

• `Private` **\_skybox**: [`Nullable`](../modules.md#nullable)[`Mesh`](Mesh.md)

#### Defined in

packages/dev/core/src/Helpers/environmentHelper.ts:256

___

### \_skyboxMaterial

• `Private` **\_skyboxMaterial**: [`Nullable`](../modules.md#nullable)[`BackgroundMaterial`](BackgroundMaterial.md)

#### Defined in

packages/dev/core/src/Helpers/environmentHelper.ts:272

___

### \_skyboxTexture

• `Private` **\_skyboxTexture**: [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

#### Defined in

packages/dev/core/src/Helpers/environmentHelper.ts:264

___

### onErrorObservable

• **onErrorObservable**: [`Observable`](Observable.md){ `exception?`: `any` ; `message?`: `string`  }

This observable will be notified with any error during the creation of the environment,
mainly texture creation errors.

#### Defined in

packages/dev/core/src/Helpers/environmentHelper.ts:333

___

### \_EnvironmentTextureCDNUrl

▪ `Static` `Private` **\_EnvironmentTextureCDNUrl**: `string` = `"https://assets.babylonjs.com/environments/environmentSpecular.env"`

Default environment texture URL.

#### Defined in

packages/dev/core/src/Helpers/environmentHelper.ts:206

___

### \_GroundTextureCDNUrl

▪ `Static` `Private` **\_GroundTextureCDNUrl**: `string` = `"https://assets.babylonjs.com/environments/backgroundGround.png"`

Default ground texture URL.

#### Defined in

packages/dev/core/src/Helpers/environmentHelper.ts:196

___

### \_SkyboxTextureCDNUrl

▪ `Static` `Private` **\_SkyboxTextureCDNUrl**: `string` = `"https://assets.babylonjs.com/environments/backgroundSkybox.dds"`

Default skybox texture URL.

#### Defined in

packages/dev/core/src/Helpers/environmentHelper.ts:201

## Accessors

### ground

• `get` **ground**(): [`Nullable`](../modules.md#nullable)[`Mesh`](Mesh.md)

Gets the ground mesh created by the helper.

#### Returns

[`Nullable`](../modules.md#nullable)[`Mesh`](Mesh.md)

#### Defined in

packages/dev/core/src/Helpers/environmentHelper.ts:284

___

### groundMaterial

• `get` **groundMaterial**(): [`Nullable`](../modules.md#nullable)[`BackgroundMaterial`](BackgroundMaterial.md)

Gets the ground material created by the helper.

#### Returns

[`Nullable`](../modules.md#nullable)[`BackgroundMaterial`](BackgroundMaterial.md)

#### Defined in

packages/dev/core/src/Helpers/environmentHelper.ts:319

___

### groundMirror

• `get` **groundMirror**(): [`Nullable`](../modules.md#nullable)[`MirrorTexture`](MirrorTexture.md)

Gets the ground mirror created by the helper.

#### Returns

[`Nullable`](../modules.md#nullable)[`MirrorTexture`](MirrorTexture.md)

#### Defined in

packages/dev/core/src/Helpers/environmentHelper.ts:300

___

### groundMirrorRenderList

• `get` **groundMirrorRenderList**(): [`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)[]

Gets the ground mirror render list to helps pushing the meshes
you wish in the ground reflection.

#### Returns

[`Nullable`](../modules.md#nullable)[`AbstractMesh`](AbstractMesh.md)[]

#### Defined in

packages/dev/core/src/Helpers/environmentHelper.ts:308

___

### groundTexture

• `get` **groundTexture**(): [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Gets the ground texture created by the helper.

#### Returns

[`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

#### Defined in

packages/dev/core/src/Helpers/environmentHelper.ts:292

___

### rootMesh

• `get` **rootMesh**(): [`Mesh`](Mesh.md)

Gets the root mesh created by the helper.

#### Returns

[`Mesh`](Mesh.md)

#### Defined in

packages/dev/core/src/Helpers/environmentHelper.ts:252

___

### skybox

• `get` **skybox**(): [`Nullable`](../modules.md#nullable)[`Mesh`](Mesh.md)

Gets the skybox created by the helper.

#### Returns

[`Nullable`](../modules.md#nullable)[`Mesh`](Mesh.md)

#### Defined in

packages/dev/core/src/Helpers/environmentHelper.ts:260

___

### skyboxMaterial

• `get` **skyboxMaterial**(): [`Nullable`](../modules.md#nullable)[`BackgroundMaterial`](BackgroundMaterial.md)

Gets the skybox material created by the helper.

#### Returns

[`Nullable`](../modules.md#nullable)[`BackgroundMaterial`](BackgroundMaterial.md)

#### Defined in

packages/dev/core/src/Helpers/environmentHelper.ts:276

___

### skyboxTexture

• `get` **skyboxTexture**(): [`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

Gets the skybox texture created by the helper.

#### Returns

[`Nullable`](../modules.md#nullable)[`BaseTexture`](BaseTexture.md)

#### Defined in

packages/dev/core/src/Helpers/environmentHelper.ts:268

## Methods

### \_errorHandler

▸ `Private` **_errorHandler**(`message?`, `exception?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `message?` | `string` |
| `exception?` | `any` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Helpers/environmentHelper.ts:694

___

### \_getSceneSize

▸ `Private` **_getSceneSize**(): `ISceneSize`

Get the scene sizes according to the setup.

#### Returns

`ISceneSize`

#### Defined in

packages/dev/core/src/Helpers/environmentHelper.ts:495

___

### \_setupBackground

▸ `Private` **_setupBackground**(): `void`

Setup the background according to the specified options.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Helpers/environmentHelper.ts:463

___

### \_setupEnvironmentTexture

▸ `Private` **_setupEnvironmentTexture**(): `void`

Setup the environment texture according to the specified options.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Helpers/environmentHelper.ts:446

___

### \_setupGround

▸ `Private` **_setupGround**(`sceneSize`): `void`

Setup the ground according to the specified options.

#### Parameters

| Name | Type |
| :------ | :------ |
| `sceneSize` | `ISceneSize` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Helpers/environmentHelper.ts:535

___

### \_setupGroundDiffuseTexture

▸ `Private` **_setupGroundDiffuseTexture**(): `void`

Setup the ground diffuse texture according to the specified options.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Helpers/environmentHelper.ts:570

___

### \_setupGroundMaterial

▸ `Private` **_setupGroundMaterial**(): `void`

Setup the ground material according to the specified options.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Helpers/environmentHelper.ts:551

___

### \_setupGroundMirrorTexture

▸ `Private` **_setupGroundMirrorTexture**(`sceneSize`): `void`

Setup the ground mirror texture according to the specified options.

#### Parameters

| Name | Type |
| :------ | :------ |
| `sceneSize` | `ISceneSize` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Helpers/environmentHelper.ts:594

___

### \_setupImageProcessing

▸ `Private` **_setupImageProcessing**(): `void`

Setup the image processing according to the specified options.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Helpers/environmentHelper.ts:434

___

### \_setupMirrorInGroundMaterial

▸ `Private` **_setupMirrorInGroundMaterial**(): `void`

Setup the ground to receive the mirror texture.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Helpers/environmentHelper.ts:629

___

### \_setupSkybox

▸ `Private` **_setupSkybox**(`sceneSize`): `void`

Setup the skybox according to the specified options.

#### Parameters

| Name | Type |
| :------ | :------ |
| `sceneSize` | `ISceneSize` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Helpers/environmentHelper.ts:643

___

### \_setupSkyboxMaterial

▸ `Private` **_setupSkyboxMaterial**(): `void`

Setup the skybox material according to the specified options.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Helpers/environmentHelper.ts:656

___

### \_setupSkyboxReflectionTexture

▸ `Private` **_setupSkyboxReflectionTexture**(): `void`

Setup the skybox reflection texture according to the specified options.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Helpers/environmentHelper.ts:674

___

### dispose

▸ **dispose**(): `void`

Dispose all the elements created by the Helper.

#### Returns

`void`

#### Defined in

packages/dev/core/src/Helpers/environmentHelper.ts:701

___

### setMainColor

▸ **setMainColor**(`color`): `void`

Sets the primary color of all the available elements.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `color` | [`Color3`](Color3.md) | the main color to affect to the ground and the background |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Helpers/environmentHelper.ts:417

___

### updateOptions

▸ **updateOptions**(`options`): `void`

Updates the background according to the new options

#### Parameters

| Name | Type |
| :------ | :------ |
| `options` | `Partial`[`IEnvironmentHelperOptions`](../interfaces/IEnvironmentHelperOptions.md) |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Helpers/environmentHelper.ts:356

___

### \_GetDefaultOptions

▸ `Static` `Private` **_GetDefaultOptions**(): [`IEnvironmentHelperOptions`](../interfaces/IEnvironmentHelperOptions.md)

Creates the default options for the helper.

#### Returns

[`IEnvironmentHelperOptions`](../interfaces/IEnvironmentHelperOptions.md)

#### Defined in

packages/dev/core/src/Helpers/environmentHelper.ts:211
