[@dev/core](../README.md) / [Exports](../modules.md) / DirectionalLightFrustumViewer

# Class: DirectionalLightFrustumViewer

Class used to render a debug view of the frustum for a directional light

**`See`**

https://playground.babylonjs.com/#7EFGSG#4

**`Since`**

5.0.0

## Table of contents

### Constructors

- [constructor](DirectionalLightFrustumViewer.md#constructor)

### Properties

- [\_blLinesPoints](DirectionalLightFrustumViewer.md#_bllinespoints)
- [\_bottomPlaneVertices](DirectionalLightFrustumViewer.md#_bottomplanevertices)
- [\_brLinesPoints](DirectionalLightFrustumViewer.md#_brlinespoints)
- [\_camera](DirectionalLightFrustumViewer.md#_camera)
- [\_farLinesPoints](DirectionalLightFrustumViewer.md#_farlinespoints)
- [\_farPlaneVertices](DirectionalLightFrustumViewer.md#_farplanevertices)
- [\_inverseViewMatrix](DirectionalLightFrustumViewer.md#_inverseviewmatrix)
- [\_leftPlaneVertices](DirectionalLightFrustumViewer.md#_leftplanevertices)
- [\_light](DirectionalLightFrustumViewer.md#_light)
- [\_lightHelperFrustumMeshes](DirectionalLightFrustumViewer.md#_lighthelperfrustummeshes)
- [\_nearLinesPoints](DirectionalLightFrustumViewer.md#_nearlinespoints)
- [\_nearPlaneVertices](DirectionalLightFrustumViewer.md#_nearplanevertices)
- [\_oldAutoCalc](DirectionalLightFrustumViewer.md#_oldautocalc)
- [\_oldDirection](DirectionalLightFrustumViewer.md#_olddirection)
- [\_oldMaxZ](DirectionalLightFrustumViewer.md#_oldmaxz)
- [\_oldMinZ](DirectionalLightFrustumViewer.md#_oldminz)
- [\_oldPosition](DirectionalLightFrustumViewer.md#_oldposition)
- [\_rightPlaneVertices](DirectionalLightFrustumViewer.md#_rightplanevertices)
- [\_rootNode](DirectionalLightFrustumViewer.md#_rootnode)
- [\_scene](DirectionalLightFrustumViewer.md#_scene)
- [\_showLines](DirectionalLightFrustumViewer.md#_showlines)
- [\_showPlanes](DirectionalLightFrustumViewer.md#_showplanes)
- [\_tlLinesPoints](DirectionalLightFrustumViewer.md#_tllinespoints)
- [\_topPlaneVertices](DirectionalLightFrustumViewer.md#_topplanevertices)
- [\_trLinesPoints](DirectionalLightFrustumViewer.md#_trlinespoints)
- [\_transparency](DirectionalLightFrustumViewer.md#_transparency)
- [\_visible](DirectionalLightFrustumViewer.md#_visible)

### Accessors

- [showLines](DirectionalLightFrustumViewer.md#showlines)
- [showPlanes](DirectionalLightFrustumViewer.md#showplanes)
- [transparency](DirectionalLightFrustumViewer.md#transparency)

### Methods

- [\_createGeometry](DirectionalLightFrustumViewer.md#_creategeometry)
- [\_getInvertViewMatrix](DirectionalLightFrustumViewer.md#_getinvertviewmatrix)
- [dispose](DirectionalLightFrustumViewer.md#dispose)
- [hide](DirectionalLightFrustumViewer.md#hide)
- [show](DirectionalLightFrustumViewer.md#show)
- [update](DirectionalLightFrustumViewer.md#update)

## Constructors

### constructor

• **new DirectionalLightFrustumViewer**(`light`, `camera`)

Creates a new frustum viewer

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `light` | [`DirectionalLight`](DirectionalLight.md) | directional light to display the frustum for |
| `camera` | [`Camera`](Camera.md) | camera used to retrieve the minZ / maxZ values if the shadowMinZ/shadowMaxZ values of the light are not setup |

#### Defined in

packages/dev/core/src/Debug/directionalLightFrustumViewer.ts:104

## Properties

### \_blLinesPoints

• `Private` **\_blLinesPoints**: [`Vector3`](Vector3.md)[]

#### Defined in

packages/dev/core/src/Debug/directionalLightFrustumViewer.ts:33

___

### \_bottomPlaneVertices

• `Private` **\_bottomPlaneVertices**: `number`[]

#### Defined in

packages/dev/core/src/Debug/directionalLightFrustumViewer.ts:40

___

### \_brLinesPoints

• `Private` **\_brLinesPoints**: [`Vector3`](Vector3.md)[]

#### Defined in

packages/dev/core/src/Debug/directionalLightFrustumViewer.ts:31

___

### \_camera

• `Private` **\_camera**: [`Camera`](Camera.md)

#### Defined in

packages/dev/core/src/Debug/directionalLightFrustumViewer.ts:21

___

### \_farLinesPoints

• `Private` **\_farLinesPoints**: [`Vector3`](Vector3.md)[]

#### Defined in

packages/dev/core/src/Debug/directionalLightFrustumViewer.ts:29

___

### \_farPlaneVertices

• `Private` **\_farPlaneVertices**: `number`[]

#### Defined in

packages/dev/core/src/Debug/directionalLightFrustumViewer.ts:36

___

### \_inverseViewMatrix

• `Private` **\_inverseViewMatrix**: [`Matrix`](Matrix.md)

#### Defined in

packages/dev/core/src/Debug/directionalLightFrustumViewer.ts:22

___

### \_leftPlaneVertices

• `Private` **\_leftPlaneVertices**: `number`[]

#### Defined in

packages/dev/core/src/Debug/directionalLightFrustumViewer.ts:38

___

### \_light

• `Private` **\_light**: [`DirectionalLight`](DirectionalLight.md)

#### Defined in

packages/dev/core/src/Debug/directionalLightFrustumViewer.ts:20

___

### \_lightHelperFrustumMeshes

• `Private` **\_lightHelperFrustumMeshes**: [`Mesh`](Mesh.md)[]

#### Defined in

packages/dev/core/src/Debug/directionalLightFrustumViewer.ts:26

___

### \_nearLinesPoints

• `Private` **\_nearLinesPoints**: [`Vector3`](Vector3.md)[]

#### Defined in

packages/dev/core/src/Debug/directionalLightFrustumViewer.ts:28

___

### \_nearPlaneVertices

• `Private` **\_nearPlaneVertices**: `number`[]

#### Defined in

packages/dev/core/src/Debug/directionalLightFrustumViewer.ts:35

___

### \_oldAutoCalc

• `Private` **\_oldAutoCalc**: `boolean`

#### Defined in

packages/dev/core/src/Debug/directionalLightFrustumViewer.ts:44

___

### \_oldDirection

• `Private` **\_oldDirection**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Debug/directionalLightFrustumViewer.ts:43

___

### \_oldMaxZ

• `Private` **\_oldMaxZ**: `number`

#### Defined in

packages/dev/core/src/Debug/directionalLightFrustumViewer.ts:46

___

### \_oldMinZ

• `Private` **\_oldMinZ**: `number`

#### Defined in

packages/dev/core/src/Debug/directionalLightFrustumViewer.ts:45

___

### \_oldPosition

• `Private` **\_oldPosition**: [`Vector3`](Vector3.md)

#### Defined in

packages/dev/core/src/Debug/directionalLightFrustumViewer.ts:42

___

### \_rightPlaneVertices

• `Private` **\_rightPlaneVertices**: `number`[]

#### Defined in

packages/dev/core/src/Debug/directionalLightFrustumViewer.ts:37

___

### \_rootNode

• `Private` **\_rootNode**: [`TransformNode`](TransformNode.md)

#### Defined in

packages/dev/core/src/Debug/directionalLightFrustumViewer.ts:25

___

### \_scene

• `Private` **\_scene**: [`Scene`](Scene.md)

#### Defined in

packages/dev/core/src/Debug/directionalLightFrustumViewer.ts:19

___

### \_showLines

• `Private` **\_showLines**: `boolean` = `true`

#### Defined in

packages/dev/core/src/Debug/directionalLightFrustumViewer.ts:63

___

### \_showPlanes

• `Private` **\_showPlanes**: `boolean` = `true`

#### Defined in

packages/dev/core/src/Debug/directionalLightFrustumViewer.ts:81

___

### \_tlLinesPoints

• `Private` **\_tlLinesPoints**: [`Vector3`](Vector3.md)[]

#### Defined in

packages/dev/core/src/Debug/directionalLightFrustumViewer.ts:32

___

### \_topPlaneVertices

• `Private` **\_topPlaneVertices**: `number`[]

#### Defined in

packages/dev/core/src/Debug/directionalLightFrustumViewer.ts:39

___

### \_trLinesPoints

• `Private` **\_trLinesPoints**: [`Vector3`](Vector3.md)[]

#### Defined in

packages/dev/core/src/Debug/directionalLightFrustumViewer.ts:30

___

### \_transparency

• `Private` **\_transparency**: `number` = `0.3`

#### Defined in

packages/dev/core/src/Debug/directionalLightFrustumViewer.ts:48

___

### \_visible

• `Private` **\_visible**: `boolean`

#### Defined in

packages/dev/core/src/Debug/directionalLightFrustumViewer.ts:23

## Accessors

### showLines

• `get` **showLines**(): `boolean`

true to display the edges of the frustum

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Debug/directionalLightFrustumViewer.ts:67

• `set` **showLines**(`show`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `show` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Debug/directionalLightFrustumViewer.ts:71

___

### showPlanes

• `get` **showPlanes**(): `boolean`

true to display the planes of the frustum

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Debug/directionalLightFrustumViewer.ts:85

• `set` **showPlanes**(`show`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `show` | `boolean` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Debug/directionalLightFrustumViewer.ts:89

___

### transparency

• `get` **transparency**(): `number`

Gets or sets the transparency of the frustum planes

#### Returns

`number`

#### Defined in

packages/dev/core/src/Debug/directionalLightFrustumViewer.ts:52

• `set` **transparency**(`alpha`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `alpha` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Debug/directionalLightFrustumViewer.ts:56

## Methods

### \_createGeometry

▸ `Protected` **_createGeometry**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Debug/directionalLightFrustumViewer.ts:246

___

### \_getInvertViewMatrix

▸ `Protected` **_getInvertViewMatrix**(): [`Matrix`](Matrix.md)

#### Returns

[`Matrix`](Matrix.md)

#### Defined in

packages/dev/core/src/Debug/directionalLightFrustumViewer.ts:346

___

### dispose

▸ **dispose**(): `void`

Dispose of the class / remove the frustum view

#### Returns

`void`

#### Defined in

packages/dev/core/src/Debug/directionalLightFrustumViewer.ts:238

___

### hide

▸ **hide**(): `void`

Hides the frustum

#### Returns

`void`

#### Defined in

packages/dev/core/src/Debug/directionalLightFrustumViewer.ts:129

___

### show

▸ **show**(): `void`

Shows the frustum

#### Returns

`void`

#### Defined in

packages/dev/core/src/Debug/directionalLightFrustumViewer.ts:118

___

### update

▸ **update**(): `void`

Updates the frustum.
Call this method to update the frustum view if the light has changed position/direction

#### Returns

`void`

#### Defined in

packages/dev/core/src/Debug/directionalLightFrustumViewer.ts:140
