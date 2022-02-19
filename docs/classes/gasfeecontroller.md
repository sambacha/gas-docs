[ethereum-gas-reference](../README.md) › [Globals](../globals.md) › [GasFeeController](gasfeecontroller.md)

# Class: GasFeeController

Controller that retrieves gas fee estimate data and polls for updated data on a set interval

## Hierarchy

* BaseController‹typeof name, [GasFeeState](../globals.md#gasfeestate), [GasFeeMessenger](../globals.md#gasfeemessenger)›

  ↳ **GasFeeController**

## Index

### Constructors

* [constructor](gasfeecontroller.md#constructor)

### Properties

* [EIP1559APIEndpoint](gasfeecontroller.md#private-eip1559apiendpoint)
* [clientId](gasfeecontroller.md#private-optional-clientid)
* [currentChainId](gasfeecontroller.md#private-currentchainid)
* [ethQuery](gasfeecontroller.md#private-ethquery)
* [getChainId](gasfeecontroller.md#private-getchainid)
* [getCurrentAccountEIP1559Compatibility](gasfeecontroller.md#private-getcurrentaccounteip1559compatibility)
* [getCurrentNetworkEIP1559Compatibility](gasfeecontroller.md#private-getcurrentnetworkeip1559compatibility)
* [getCurrentNetworkLegacyGasAPICompatibility](gasfeecontroller.md#private-getcurrentnetworklegacygasapicompatibility)
* [intervalDelay](gasfeecontroller.md#private-intervaldelay)
* [intervalId](gasfeecontroller.md#private-optional-intervalid)
* [legacyAPIEndpoint](gasfeecontroller.md#private-legacyapiendpoint)
* [messagingSystem](gasfeecontroller.md#protected-messagingsystem)
* [metadata](gasfeecontroller.md#readonly-metadata)
* [name](gasfeecontroller.md#readonly-name)
* [pollTokens](gasfeecontroller.md#private-polltokens)
* [subscribe](gasfeecontroller.md#readonly-subscribe)

### Accessors

* [state](gasfeecontroller.md#state)

### Methods

* [destroy](gasfeecontroller.md#protected-destroy)
* [update](gasfeecontroller.md#protected-update)

## Constructors

###  constructor

\+ **new GasFeeController**(`__namedParameters`: object): *[GasFeeController](gasfeecontroller.md)*

*Overrides void*

Defined in GasFeeController.ts:238

Creates a GasFeeController instance.

**Parameters:**

▪ **__namedParameters**: *object*

Name | Type | Default |
------ | ------ | ------ |
`EIP1559APIEndpoint` | any | GAS_FEE_API |
`clientId` | any | - |
`getChainId` | function | - |
`getCurrentAccountEIP1559Compatibility` | function | - |
`getCurrentNetworkEIP1559Compatibility` | function | - |
`getCurrentNetworkLegacyGasAPICompatibility` | function | - |
`getProvider` | any | - |
`interval` | number | 15000 |
`legacyAPIEndpoint` | any | LEGACY_GAS_PRICES_API_URL |
`messenger` | [GasFeeMessenger](../globals.md#gasfeemessenger) | - |
`onNetworkStateChange` | any | - |
`state` | [GasFeeState](../globals.md#gasfeestate) | - |

**Returns:** *[GasFeeController](gasfeecontroller.md)*

## Properties

### `Private` EIP1559APIEndpoint

• **EIP1559APIEndpoint**: *string*

Defined in GasFeeController.ts:224

___

### `Private` `Optional` clientId

• **clientId**? : *string*

Defined in GasFeeController.ts:238

___

### `Private` currentChainId

• **currentChainId**: *any*

Defined in GasFeeController.ts:234

___

### `Private` ethQuery

• **ethQuery**: *any*

Defined in GasFeeController.ts:236

___

### `Private` getChainId

• **getChainId**: *any*

Defined in GasFeeController.ts:232

___

### `Private` getCurrentAccountEIP1559Compatibility

• **getCurrentAccountEIP1559Compatibility**: *any*

Defined in GasFeeController.ts:230

___

### `Private` getCurrentNetworkEIP1559Compatibility

• **getCurrentNetworkEIP1559Compatibility**: *any*

Defined in GasFeeController.ts:226

___

### `Private` getCurrentNetworkLegacyGasAPICompatibility

• **getCurrentNetworkLegacyGasAPICompatibility**: *any*

Defined in GasFeeController.ts:228

___

### `Private` intervalDelay

• **intervalDelay**: *any*

Defined in GasFeeController.ts:218

___

### `Private` `Optional` intervalId

• **intervalId**? : *Timeout*

Defined in GasFeeController.ts:216

___

### `Private` legacyAPIEndpoint

• **legacyAPIEndpoint**: *string*

Defined in GasFeeController.ts:222

___

### `Protected` messagingSystem

• **messagingSystem**: *[GasFeeMessenger](../globals.md#gasfeemessenger)*

*Inherited from [BaseController](basecontroller.md).[messagingSystem](basecontroller.md#protected-messagingsystem)*

Defined in BaseControllerV2.ts:82

___

### `Readonly` metadata

• **metadata**: *[StateMetadata](../globals.md#statemetadata)‹[GasFeeState](../globals.md#gasfeestate)›*

*Inherited from [BaseController](basecontroller.md).[metadata](basecontroller.md#readonly-metadata)*

Defined in BaseControllerV2.ts:91

___

### `Readonly` name

• **name**: *typeof name*

*Inherited from [GasFeeController](gasfeecontroller.md).[name](gasfeecontroller.md#readonly-name)*

Defined in BaseControllerV2.ts:89

The name of the controller.

This is used by the ComposableController to construct a composed application state.

___

### `Private` pollTokens

• **pollTokens**: *Set‹string›*

Defined in GasFeeController.ts:220

___

### `Readonly` subscribe

• **subscribe**: *never*

*Inherited from [GasFeeController](gasfeecontroller.md).[subscribe](gasfeecontroller.md#readonly-subscribe)*

Defined in BaseControllerV2.ts:99

The existence of the `subscribe` property is how the ComposableController detects whether a
controller extends the old BaseController or the new one. We set it to `never` here to ensure
this property is never used for new BaseController-based controllers, to ensure the
ComposableController never mistakes them for an older style controller.

## Accessors

###  state

• **get state**(): *S*

*Inherited from [GasFeeController](gasfeecontroller.md).[state](gasfeecontroller.md#state)*

Defined in BaseControllerV2.ts:138

Retrieves current controller state.

**Returns:** *S*

The current state.

• **set state**(`_`: S): *void*

*Inherited from [GasFeeController](gasfeecontroller.md).[state](gasfeecontroller.md#state)*

Defined in BaseControllerV2.ts:142

Retrieves current controller state.

**Parameters:**

Name | Type |
------ | ------ |
`_` | S |

**Returns:** *void*

The current state.

## Methods

### `Protected` destroy

▸ **destroy**(): *void*

*Inherited from [BaseController](basecontroller.md).[destroy](basecontroller.md#protected-destroy)*

Defined in BaseControllerV2.ts:185

Prepares the controller for garbage collection. This should be extended
by any subclasses to clean up any additional connections or events.

The only cleanup performed here is to remove listeners. While technically
this is not required to ensure this instance is garbage collected, it at
least ensures this instance won't be responsible for preventing the
listeners from being garbage collected.

**Returns:** *void*

___

### `Protected` update

▸ **update**(`callback`: function): *void*

*Inherited from [GasFeeController](gasfeecontroller.md).[update](gasfeecontroller.md#protected-update)*

Defined in BaseControllerV2.ts:157

Updates controller state. Accepts a callback that is passed a draft copy
of the controller state. If a value is returned, it is set as the new
state. Otherwise, any changes made within that callback to the draft are
applied to the controller state.

**Parameters:**

▪ **callback**: *function*

Callback for updating state, passed a draft state
object. Return a new state object or mutate the draft to update state.

▸ (`state`: Draft‹[GasFeeState](../globals.md#gasfeestate)›): *void | [GasFeeState](../globals.md#gasfeestate)*

**Parameters:**

Name | Type |
------ | ------ |
`state` | Draft‹[GasFeeState](../globals.md#gasfeestate)› |

**Returns:** *void*
