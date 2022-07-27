[@dev/core](../README.md) / [Exports](../modules.md) / WebRequest

# Class: WebRequest

Extended version of XMLHttpRequest with support for customizations (headers, ...)

## Implements

- `IWebRequest`

## Table of contents

### Constructors

- [constructor](WebRequest.md#constructor)

### Properties

- [\_requestURL](WebRequest.md#_requesturl)
- [\_xhr](WebRequest.md#_xhr)
- [CustomRequestHeaders](WebRequest.md#customrequestheaders)
- [CustomRequestModifiers](WebRequest.md#customrequestmodifiers)
- [SkipRequestModificationForBabylonCDN](WebRequest.md#skiprequestmodificationforbabyloncdn)

### Accessors

- [onprogress](WebRequest.md#onprogress)
- [readyState](WebRequest.md#readystate)
- [response](WebRequest.md#response)
- [responseText](WebRequest.md#responsetext)
- [responseType](WebRequest.md#responsetype)
- [responseURL](WebRequest.md#responseurl)
- [status](WebRequest.md#status)
- [statusText](WebRequest.md#statustext)
- [timeout](WebRequest.md#timeout)

### Methods

- [\_injectCustomRequestHeaders](WebRequest.md#_injectcustomrequestheaders)
- [\_shouldSkipRequestModifications](WebRequest.md#_shouldskiprequestmodifications)
- [abort](WebRequest.md#abort)
- [getResponseHeader](WebRequest.md#getresponseheader)
- [open](WebRequest.md#open)
- [send](WebRequest.md#send)
- [setRequestHeader](WebRequest.md#setrequestheader)

## Constructors

### constructor

• **new WebRequest**()

## Properties

### \_requestURL

• `Private` **\_requestURL**: `string` = `""`

#### Defined in

packages/dev/core/src/Misc/webRequest.ts:38

___

### \_xhr

• `Private` `Readonly` **\_xhr**: `XMLHttpRequest`

#### Defined in

packages/dev/core/src/Misc/webRequest.ts:23

___

### CustomRequestHeaders

▪ `Static` **CustomRequestHeaders**: `Object` = `{}`

Custom HTTP Request Headers to be sent with XMLHttpRequests
i.e. when loading files, where the server/service expects an Authorization header

#### Index signature

▪ [key: `string`]: `string`

#### Defined in

packages/dev/core/src/Misc/webRequest.ts:29

___

### CustomRequestModifiers

▪ `Static` **CustomRequestModifiers**: (`request`: `XMLHttpRequest`, `url`: `string`) => `void`[]

Add callback functions in this array to update all the requests before they get sent to the network

#### Defined in

packages/dev/core/src/Misc/webRequest.ts:34

___

### SkipRequestModificationForBabylonCDN

▪ `Static` **SkipRequestModificationForBabylonCDN**: `boolean` = `true`

#### Defined in

packages/dev/core/src/Misc/webRequest.ts:36

## Accessors

### onprogress

• `get` **onprogress**(): ``null`` \| (`this`: `XMLHttpRequest`, `ev`: `ProgressEvent``EventTarget`) => `any`

Gets or sets a function to be called when loading progress changes

#### Returns

``null`` \| (`this`: `XMLHttpRequest`, `ev`: `ProgressEvent``EventTarget`) => `any`

#### Defined in

packages/dev/core/src/Misc/webRequest.ts:59

• `set` **onprogress**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | ``null`` \| (`this`: `XMLHttpRequest`, `ev`: `ProgressEvent``EventTarget`) => `any` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/webRequest.ts:63

___

### readyState

• `get` **readyState**(): `number`

Returns client's state

#### Returns

`number`

#### Defined in

packages/dev/core/src/Misc/webRequest.ts:70

___

### response

• `get` **response**(): `any`

Returns client's response

#### Returns

`any`

#### Defined in

packages/dev/core/src/Misc/webRequest.ts:91

___

### responseText

• `get` **responseText**(): `string`

Returns client's response as text

#### Returns

`string`

#### Defined in

packages/dev/core/src/Misc/webRequest.ts:105

___

### responseType

• `get` **responseType**(): `XMLHttpRequestResponseType`

Gets or sets the expected response type

#### Returns

`XMLHttpRequestResponseType`

#### Defined in

packages/dev/core/src/Misc/webRequest.ts:112

• `set` **responseType**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `XMLHttpRequestResponseType` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/webRequest.ts:116

___

### responseURL

• `get` **responseURL**(): `string`

Returns client's response url

#### Returns

`string`

#### Implementation of

IWebRequest.responseURL

#### Defined in

packages/dev/core/src/Misc/webRequest.ts:98

___

### status

• `get` **status**(): `number`

Returns client's status

#### Returns

`number`

#### Implementation of

IWebRequest.status

#### Defined in

packages/dev/core/src/Misc/webRequest.ts:77

___

### statusText

• `get` **statusText**(): `string`

Returns client's status as a text

#### Returns

`string`

#### Implementation of

IWebRequest.statusText

#### Defined in

packages/dev/core/src/Misc/webRequest.ts:84

___

### timeout

• `get` **timeout**(): `number`

Gets or sets the timeout value in milliseconds

#### Returns

`number`

#### Defined in

packages/dev/core/src/Misc/webRequest.ts:123

• `set` **timeout**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/webRequest.ts:127

## Methods

### \_injectCustomRequestHeaders

▸ `Private` **_injectCustomRequestHeaders**(): `void`

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/webRequest.ts:40

___

### \_shouldSkipRequestModifications

▸ `Private` **_shouldSkipRequestModifications**(`url`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `url` | `string` |

#### Returns

`boolean`

#### Defined in

packages/dev/core/src/Misc/webRequest.ts:52

___

### abort

▸ **abort**(): `void`

Cancels any network activity

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/webRequest.ts:154

___

### getResponseHeader

▸ **getResponseHeader**(`name`): [`Nullable`](../modules.md#nullable)`string`

Get the string containing the text of a particular header's value.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | The name of the header |

#### Returns

[`Nullable`](../modules.md#nullable)`string`

The string containing the text of the given header name

#### Defined in

packages/dev/core/src/Misc/webRequest.ts:206

___

### open

▸ **open**(`method`, `url`): `void`

Sets the request method, request URL

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `method` | `string` | defines the method to use (GET, POST, etc..) |
| `url` | `string` | defines the url to connect with |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/webRequest.ts:175

___

### send

▸ **send**(`body?`): `void`

Initiates the request. The optional argument provides the request body. The argument is ignored if request method is GET or HEAD

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `body?` | ``null`` \| `Document` \| `XMLHttpRequestBodyInit` | defines an optional request body |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/webRequest.ts:162

___

### setRequestHeader

▸ **setRequestHeader**(`name`, `value`): `void`

Sets the value of a request header.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | The name of the header whose value is to be set |
| `value` | `string` | The value to set as the body of the header |

#### Returns

`void`

#### Defined in

packages/dev/core/src/Misc/webRequest.ts:197
