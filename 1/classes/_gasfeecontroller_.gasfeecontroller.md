[ethereum-gas-reference](../README.md) › [Globals](../globals.md) › ["GasFeeController"](../modules/_gasfeecontroller_.md) › [GasFeeController](_gasfeecontroller_.gasfeecontroller.md)

# Class: GasFeeController

Controller that retrieves gas fee estimate data and polls for updated data on a set interval

## Hierarchy

* [BaseController](_basecontrollerv2_.basecontroller.md)‹typeof name, [GasFeeState](../modules/_gasfeecontroller_.md#gasfeestate), [GasFeeMessenger](../modules/_gasfeecontroller_.md#gasfeemessenger)›

  ↳ **GasFeeController**

## Index

### Constructors

* [constructor](_gasfeecontroller_.gasfeecontroller.md#constructor)

### Properties

* [EIP1559APIEndpoint](_gasfeecontroller_.gasfeecontroller.md#private-eip1559apiendpoint)
* [clientId](_gasfeecontroller_.gasfeecontroller.md#private-optional-clientid)
* [currentChainId](_gasfeecontroller_.gasfeecontroller.md#private-currentchainid)
* [ethQuery](_gasfeecontroller_.gasfeecontroller.md#private-ethquery)
* [getChainId](_gasfeecontroller_.gasfeecontroller.md#private-getchainid)
* [getCurrentAccountEIP1559Compatibility](_gasfeecontroller_.gasfeecontroller.md#private-getcurrentaccounteip1559compatibility)
* [getCurrentNetworkEIP1559Compatibility](_gasfeecontroller_.gasfeecontroller.md#private-getcurrentnetworkeip1559compatibility)
* [getCurrentNetworkLegacyGasAPICompatibility](_gasfeecontroller_.gasfeecontroller.md#private-getcurrentnetworklegacygasapicompatibility)
* [intervalDelay](_gasfeecontroller_.gasfeecontroller.md#private-intervaldelay)
* [intervalId](_gasfeecontroller_.gasfeecontroller.md#private-optional-intervalid)
* [legacyAPIEndpoint](_gasfeecontroller_.gasfeecontroller.md#private-legacyapiendpoint)
* [messagingSystem](_gasfeecontroller_.gasfeecontroller.md#protected-messagingsystem)
* [metadata](_gasfeecontroller_.gasfeecontroller.md#readonly-metadata)
* [name](_gasfeecontroller_.gasfeecontroller.md#readonly-name)
* [pollTokens](_gasfeecontroller_.gasfeecontroller.md#private-polltokens)
* [subscribe](_gasfeecontroller_.gasfeecontroller.md#readonly-subscribe)

### Accessors

* [state](_gasfeecontroller_.gasfeecontroller.md#state)

### Methods

* [destroy](_gasfeecontroller_.gasfeecontroller.md#protected-destroy)
* [update](_gasfeecontroller_.gasfeecontroller.md#protected-update)

## Constructors

###  constructor

\+ **new GasFeeController**(`__namedParameters`: object): *[GasFeeController](_gasfeecontroller_.gasfeecontroller.md)*

*Overrides [BaseController](_basecontrollerv2_.basecontroller.md).[constructor](_basecontrollerv2_.basecontroller.md#constructor)*

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
`messenger` | [GasFeeMessenger](../modules/_gasfeecontroller_.md#gasfeemessenger) | - |
`onNetworkStateChange` | any | - |
`state` | [GasFeeState](../modules/_gasfeecontroller_.md#gasfeestate) | - |

**Returns:** *[GasFeeController](_gasfeecontroller_.gasfeecontroller.md)*

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

• **messagingSystem**: *[GasFeeMessenger](../modules/_gasfeecontroller_.md#gasfeemessenger)*

*Inherited from [BaseController](_basecontrollerv2_.basecontroller.md).[messagingSystem](_basecontrollerv2_.basecontroller.md#protected-messagingsystem)*

Defined in BaseControllerV2.ts:82

___

### `Readonly` metadata

• **metadata**: *[StateMetadata](../modules/_basecontrollerv2_.md#statemetadata)‹[GasFeeState](../modules/_gasfeecontroller_.md#gasfeestate)›*

*Inherited from [BaseController](_basecontrollerv2_.basecontroller.md).[metadata](_basecontrollerv2_.basecontroller.md#readonly-metadata)*

Defined in BaseControllerV2.ts:91

___

### `Readonly` name

• **name**: *typeof name*

*Inherited from [BaseController](_basecontrollerv2_.basecontroller.md).[name](_basecontrollerv2_.basecontroller.md#readonly-name)*

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

*Inherited from [BaseController](_basecontrollerv2_.basecontroller.md).[subscribe](_basecontrollerv2_.basecontroller.md#readonly-subscribe)*

Defined in BaseControllerV2.ts:99

The existence of the `subscribe` property is how the ComposableController detects whether a
controller extends the old BaseController or the new one. We set it to `never` here to ensure
this property is never used for new BaseController-based controllers, to ensure the
ComposableController never mistakes them for an older style controller.

## Accessors

###  state

• **get state**(): *S*

*Inherited from [BaseController](_basecontrollerv2_.basecontroller.md).[state](_basecontrollerv2_.basecontroller.md#state)*

Defined in BaseControllerV2.ts:138

Retrieves current controller state.

**Returns:** *S*

The current state.

• **set state**(`_`: S): *void*

*Inherited from [BaseController](_basecontrollerv2_.basecontroller.md).[state](_basecontrollerv2_.basecontroller.md#state)*

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

*Inherited from [BaseController](_basecontrollerv2_.basecontroller.md).[destroy](_basecontrollerv2_.basecontroller.md#protected-destroy)*

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

*Inherited from [BaseController](_basecontrollerv2_.basecontroller.md).[update](_basecontrollerv2_.basecontroller.md#protected-update)*

Defined in BaseControllerV2.ts:157

Updates controller state. Accepts a callback that is passed a draft copy
of the controller state. If a value is returned, it is set as the new
state. Otherwise, any changes made within that callback to the draft are
applied to the controller state.

**Parameters:**

▪ **callback**: *function*

Callback for updating state, passed a draft state
object. Return a new state object or mutate the draft to update state.

▸ (`state`: Draft‹[GasFeeState](../modules/_gasfeecontroller_.md#gasfeestate)›): *void | [GasFeeState](../modules/_gasfeecontroller_.md#gasfeestate)*

**Parameters:**

Name | Type |
------ | ------ |
`state` | Draft‹[GasFeeState](../modules/_gasfeecontroller_.md#gasfeestate)› |

**Returns:** *void*
