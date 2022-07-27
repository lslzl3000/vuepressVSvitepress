[@dev/core](../README.md) / [Exports](../modules.md) / WebXRFeaturesManager

# Class: WebXRFeaturesManager

The WebXR features manager is responsible of enabling or disabling features required for the current XR session.
It is mainly used in AR sessions.

A feature can have a version that is defined by Babylon (and does not correspond with the webxr version).

## Implements

- [`IDisposable`](../interfaces/IDisposable.md)

## Table of contents

### Constructors

- [constructor](WebXRFeaturesManager.md#constructor)

### Properties

- [\_features](WebXRFeaturesManager.md#_features)
- [\_AvailableFeatures](WebXRFeaturesManager.md#_availablefeatures)
- [\_ConflictingFeatures](WebXRFeaturesManager.md#_conflictingfeatures)

### Methods

- [\_extendXRSessionInitObject](WebXRFeaturesManager.md#_extendxrsessioninitobject)
- [attachFeature](WebXRFeaturesManager.md#attachfeature)
- [detachFeature](WebXRFeaturesManager.md#detachfeature)
- [disableFeature](WebXRFeaturesManager.md#disablefeature)
- [dispose](WebXRFeaturesManager.md#dispose)
- [enableFeature](WebXRFeaturesManager.md#enablefeature)
- [getEnabledFeature](WebXRFeaturesManager.md#getenabledfeature)
- [getEnabledFeatures](WebXRFeaturesManager.md#getenabledfeatures)
- [AddWebXRFeature](WebXRFeaturesManager.md#addwebxrfeature)
- [ConstructFeature](WebXRFeaturesManager.md#constructfeature)
- [GetAvailableFeatures](WebXRFeaturesManager.md#getavailablefeatures)
- [GetAvailableVersions](WebXRFeaturesManager.md#getavailableversions)
- [GetLatestVersionOfFeature](WebXRFeaturesManager.md#getlatestversionoffeature)
- [GetStableVersionOfFeature](WebXRFeaturesManager.md#getstableversionoffeature)

## Constructors

### constructor

• **new WebXRFeaturesManager**(`_xrSessionManager`)

constructs a new features manages.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `_xrSessionManager` | [`WebXRSessionManager`](WebXRSessionManager.md) | an instance of WebXRSessionManager |

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRFeaturesManager.ts:183

## Properties

### \_features

• `Private` **\_features**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: { `enabled`: `boolean` ; `featureImplementation`: [`IWebXRFeature`](../interfaces/IWebXRFeature.md) ; `required`: `boolean` ; `version`: `number`  }

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRFeaturesManager.ts:161

___

### \_AvailableFeatures

▪ `Static` `Private` `Readonly` **\_AvailableFeatures**: `Object` = `{}`

#### Index signature

▪ [name: `string`]: { `[version: number]`: [`WebXRFeatureConstructor`](../modules.md#webxrfeatureconstructor); `latest`: `number` ; `stable`: `number`  }

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRFeaturesManager.ts:153

___

### \_ConflictingFeatures

▪ `Static` `Private` `Readonly` **\_ConflictingFeatures**: `Object`

The key is the feature to check and the value is the feature that conflicts.

#### Index signature

▪ [key: `string`]: `string`

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRFeaturesManager.ts:173

## Methods

### \_extendXRSessionInitObject

▸ **_extendXRSessionInitObject**(`xrSessionInit`): `Promise``XRSessionInit`

This function will extend the session creation configuration object with enabled features.
If, for example, the anchors feature is enabled, it will be automatically added to the optional or required features list,
according to the defined "required" variable, provided during enableFeature call

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `xrSessionInit` | `XRSessionInit` | the xr Session init object to extend |

#### Returns

`Promise``XRSessionInit`

an extended XRSessionInit object

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRFeaturesManager.ts:454

___

### attachFeature

▸ **attachFeature**(`featureName`): `void`

Attach a feature to the current session. Mainly used when session started to start the feature effect.
Can be used during a session to start a feature

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `featureName` | `string` | the name of feature to attach |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRFeaturesManager.ts:286

___

### detachFeature

▸ **detachFeature**(`featureName`): `void`

Can be used inside a session or when the session ends to detach a specific feature

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `featureName` | `string` | the name of the feature to detach |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRFeaturesManager.ts:297

___

### disableFeature

▸ **disableFeature**(`featureName`): `boolean`

Used to disable an already-enabled feature
The feature will be disposed and will be recreated once enabled.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `featureName` | `string` \| { `Name`: `string`  } | the feature to disable |

#### Returns

`boolean`

true if disable was successful

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRFeaturesManager.ts:311

___

### dispose

▸ **dispose**(): `void`

dispose this features manager

#### Returns

`void`

#### Implementation of

[IDisposable](../interfaces/IDisposable.md).[dispose](../interfaces/IDisposable.md#dispose)

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRFeaturesManager.ts:327

___

### enableFeature

▸ **enableFeature**(`featureName`, `version?`, `moduleOptions?`, `attachIfPossible?`, `required?`): [`IWebXRFeature`](../interfaces/IWebXRFeature.md)

Enable a feature using its name and a version. This will enable it in the scene, and will be responsible to attach it when the session starts.
If used twice, the old version will be disposed and a new one will be constructed. This way you can re-enable with different configuration.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `featureName` | `string` \| { `Name`: `string`  } | `undefined` | the name of the feature to load or the class of the feature |
| `version` | `string` \| `number` | `"latest"` | optional version to load. if not provided the latest version will be enabled |
| `moduleOptions` | `any` | `{}` | options provided to the module. Ses the module documentation / constructor |
| `attachIfPossible` | `boolean` | `true` | if set to true (default) the feature will be automatically attached, if it is currently possible |
| `required` | `boolean` | `true` | is this feature required to the app. If set to true the session init will fail if the feature is not available. |

#### Returns

[`IWebXRFeature`](../interfaces/IWebXRFeature.md)

a new constructed feature or throws an error if feature not found or conflicts with another enabled feature.

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRFeaturesManager.ts:344

___

### getEnabledFeature

▸ **getEnabledFeature**(`featureName`): [`IWebXRFeature`](../interfaces/IWebXRFeature.md)

get the implementation of an enabled feature.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `featureName` | `string` | the name of the feature to load |

#### Returns

[`IWebXRFeature`](../interfaces/IWebXRFeature.md)

the feature class, if found

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRFeaturesManager.ts:434

___

### getEnabledFeatures

▸ **getEnabledFeatures**(): `string`[]

Get the list of enabled features

#### Returns

`string`[]

an array of enabled features

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRFeaturesManager.ts:442

___

### AddWebXRFeature

▸ `Static` **AddWebXRFeature**(`featureName`, `constructorFunction`, `version?`, `stable?`): `void`

Used to register a module. After calling this function a developer can use this feature in the scene.
Mainly used internally.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `featureName` | `string` | `undefined` | the name of the feature to register |
| `constructorFunction` | [`WebXRFeatureConstructor`](../modules.md#webxrfeatureconstructor) | `undefined` | the function used to construct the module |
| `version` | `number` | `1` | the (babylon) version of the module |
| `stable` | `boolean` | `false` | is that a stable version of this module |

#### Returns

`void`

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRFeaturesManager.ts:215

___

### ConstructFeature

▸ `Static` **ConstructFeature**(`featureName`, `version?`, `xrSessionManager`, `options?`): () => [`IWebXRFeature`](../interfaces/IWebXRFeature.md)

Returns a constructor of a specific feature.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `featureName` | `string` | `undefined` | the name of the feature to construct |
| `version` | `number` | `1` | the version of the feature to load |
| `xrSessionManager` | [`WebXRSessionManager`](WebXRSessionManager.md) | `undefined` | the xrSessionManager. Used to construct the module |
| `options?` | `any` | `undefined` | optional options provided to the module. |

#### Returns

`fn`

a function that, when called, will return a new instance of this feature

▸ (): [`IWebXRFeature`](../interfaces/IWebXRFeature.md)

Returns a constructor of a specific feature.

##### Returns

[`IWebXRFeature`](../interfaces/IWebXRFeature.md)

a function that, when called, will return a new instance of this feature

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRFeaturesManager.ts:235

___

### GetAvailableFeatures

▸ `Static` **GetAvailableFeatures**(): `string`[]

Can be used to return the list of features currently registered

#### Returns

`string`[]

an Array of available features

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRFeaturesManager.ts:250

___

### GetAvailableVersions

▸ `Static` **GetAvailableVersions**(`featureName`): `string`[]

Gets the versions available for a specific feature

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `featureName` | `string` | the name of the feature |

#### Returns

`string`[]

an array with the available versions

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRFeaturesManager.ts:259

___

### GetLatestVersionOfFeature

▸ `Static` **GetLatestVersionOfFeature**(`featureName`): `number`

Return the latest unstable version of this feature

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `featureName` | `string` | the name of the feature to search |

#### Returns

`number`

the version number. if not found will return -1

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRFeaturesManager.ts:268

___

### GetStableVersionOfFeature

▸ `Static` **GetStableVersionOfFeature**(`featureName`): `number`

Return the latest stable version of this feature

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `featureName` | `string` | the name of the feature to search |

#### Returns

`number`

the version number. if not found will return -1

#### Defined in

https://github.com/babylon.js/core/src/XR/webXRFeaturesManager.ts:277
