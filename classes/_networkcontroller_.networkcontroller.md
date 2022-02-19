[metamask-controllers-main-src-gas-2](../README.md) › [Globals](../globals.md) › ["NetworkController"](../modules/_networkcontroller_.md) › [NetworkController](_networkcontroller_.networkcontroller.md)

# Class: NetworkController

Controller that creates and manages an Ethereum network provider

## Hierarchy

* [BaseController](_basecontroller_.basecontroller.md)‹[NetworkConfig](../interfaces/_networkcontroller_.networkconfig.md), [NetworkState](../interfaces/_networkcontroller_.networkstate.md)›

  ↳ **NetworkController**

## Index

### Constructors

* [constructor](_networkcontroller_.networkcontroller.md#constructor)

### Properties

* [defaultConfig](_networkcontroller_.networkcontroller.md#defaultconfig)
* [defaultState](_networkcontroller_.networkcontroller.md#defaultstate)
* [disabled](_networkcontroller_.networkcontroller.md#disabled)
* [ethQuery](_networkcontroller_.networkcontroller.md#private-ethquery)
* [internalProviderConfig](_networkcontroller_.networkcontroller.md#private-internalproviderconfig)
* [mutex](_networkcontroller_.networkcontroller.md#private-mutex)
* [name](_networkcontroller_.networkcontroller.md#name)
* [provider](_networkcontroller_.networkcontroller.md#provider)

### Accessors

* [config](_networkcontroller_.networkcontroller.md#config)
* [providerConfig](_networkcontroller_.networkcontroller.md#providerconfig)
* [state](_networkcontroller_.networkcontroller.md#state)

### Methods

* [configure](_networkcontroller_.networkcontroller.md#configure)
* [getEIP1559Compatibility](_networkcontroller_.networkcontroller.md#geteip1559compatibility)
* [getIsCustomNetwork](_networkcontroller_.networkcontroller.md#private-getiscustomnetwork)
* [initialize](_networkcontroller_.networkcontroller.md#protected-initialize)
* [initializeProvider](_networkcontroller_.networkcontroller.md#private-initializeprovider)
* [lookupNetwork](_networkcontroller_.networkcontroller.md#lookupnetwork)
* [notify](_networkcontroller_.networkcontroller.md#notify)
* [refreshNetwork](_networkcontroller_.networkcontroller.md#private-refreshnetwork)
* [registerProvider](_networkcontroller_.networkcontroller.md#private-registerprovider)
* [safelyStopProvider](_networkcontroller_.networkcontroller.md#private-safelystopprovider)
* [setProviderType](_networkcontroller_.networkcontroller.md#setprovidertype)
* [setRpcTarget](_networkcontroller_.networkcontroller.md#setrpctarget)
* [setupInfuraProvider](_networkcontroller_.networkcontroller.md#private-setupinfuraprovider)
* [setupStandardProvider](_networkcontroller_.networkcontroller.md#private-setupstandardprovider)
* [subscribe](_networkcontroller_.networkcontroller.md#subscribe)
* [unsubscribe](_networkcontroller_.networkcontroller.md#unsubscribe)
* [update](_networkcontroller_.networkcontroller.md#update)
* [updateProvider](_networkcontroller_.networkcontroller.md#private-updateprovider)
* [verifyNetwork](_networkcontroller_.networkcontroller.md#private-verifynetwork)

## Constructors

###  constructor

\+ **new NetworkController**(`config?`: Partial‹[NetworkConfig](../interfaces/_networkcontroller_.networkconfig.md)›, `state?`: Partial‹[NetworkState](../interfaces/_networkcontroller_.networkstate.md)›): *[NetworkController](_networkcontroller_.networkcontroller.md)*

*Overrides [BaseController](_basecontroller_.basecontroller.md).[constructor](_basecontroller_.basecontroller.md#constructor)*

Defined in NetworkController.ts:218

Creates a NetworkController instance.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`config?` | Partial‹[NetworkConfig](../interfaces/_networkcontroller_.networkconfig.md)› | Initial options used to configure this controller. |
`state?` | Partial‹[NetworkState](../interfaces/_networkcontroller_.networkstate.md)› | Initial state to set on this controller.  |

**Returns:** *[NetworkController](_networkcontroller_.networkcontroller.md)*

## Properties

###  defaultConfig

• **defaultConfig**: *[NetworkConfig](../interfaces/_networkcontroller_.networkconfig.md)* = {} as C

*Inherited from [BaseController](_basecontroller_.basecontroller.md).[defaultConfig](_basecontroller_.basecontroller.md#defaultconfig)*

Defined in BaseController.ts:33

Default options used to configure this controller

___

###  defaultState

• **defaultState**: *[NetworkState](../interfaces/_networkcontroller_.networkstate.md)* = {} as S

*Inherited from [BaseController](_basecontroller_.basecontroller.md).[defaultState](_basecontroller_.basecontroller.md#defaultstate)*

Defined in BaseController.ts:38

Default state set on this controller

___

###  disabled

• **disabled**: *boolean* = false

*Inherited from [BaseController](_basecontroller_.basecontroller.md).[disabled](_basecontroller_.basecontroller.md#disabled)*

Defined in BaseController.ts:43

Determines if listeners are notified of state changes

___

### `Private` ethQuery

• **ethQuery**: *any*

Defined in NetworkController.ts:97

___

### `Private` internalProviderConfig

• **internalProviderConfig**: *[ProviderConfig](../interfaces/_networkcontroller_.providerconfig.md)* = {} as ProviderConfig

Defined in NetworkController.ts:99

___

### `Private` mutex

• **mutex**: *Mutex‹›* = new Mutex()

Defined in NetworkController.ts:101

___

###  name

• **name**: *string* = "NetworkController"

*Overrides [BaseController](_basecontroller_.basecontroller.md).[name](_basecontroller_.basecontroller.md#name)*

Defined in NetworkController.ts:213

Name of this controller used during composition

___

###  provider

• **provider**: *any*

Defined in NetworkController.ts:218

Ethereum provider object for the current network

## Accessors

###  config

• **get config**(): *C*

*Inherited from [BaseController](_basecontroller_.basecontroller.md).[config](_basecontroller_.basecontroller.md#config)*

Defined in BaseController.ts:93

Retrieves current controller configuration options.

**Returns:** *C*

The current configuration.

___

###  providerConfig

• **get providerConfig**(): *[ProviderConfig](../interfaces/_networkcontroller_.providerconfig.md)*

Defined in NetworkController.ts:253

Sets a new configuration for web3-provider-engine.

The web3-provider-engine configuration.

**Returns:** *[ProviderConfig](../interfaces/_networkcontroller_.providerconfig.md)*

• **set providerConfig**(`providerConfig`: [ProviderConfig](../interfaces/_networkcontroller_.providerconfig.md)): *void*

Defined in NetworkController.ts:245

Sets a new configuration for web3-provider-engine.

TODO: Replace this wth a method.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`providerConfig` | [ProviderConfig](../interfaces/_networkcontroller_.providerconfig.md) | The web3-provider-engine configuration.  |

**Returns:** *void*

___

###  state

• **get state**(): *S*

*Inherited from [BaseController](_basecontroller_.basecontroller.md).[state](_basecontroller_.basecontroller.md#state)*

Defined in BaseController.ts:102

Retrieves current controller state.

**Returns:** *S*

The current state.

## Methods

###  configure

▸ **configure**(`config`: Partial‹[NetworkConfig](../interfaces/_networkcontroller_.networkconfig.md)›, `overwrite`: boolean, `fullUpdate`: boolean): *void*

*Inherited from [BaseController](_basecontroller_.basecontroller.md).[configure](_basecontroller_.basecontroller.md#configure)*

Defined in BaseController.ts:113

Updates controller configuration.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`config` | Partial‹[NetworkConfig](../interfaces/_networkcontroller_.networkconfig.md)› | - | New configuration options. |
`overwrite` | boolean | false | Overwrite config instead of merging. |
`fullUpdate` | boolean | true | Boolean that defines if the update is partial or not.  |

**Returns:** *void*

___

###  getEIP1559Compatibility

▸ **getEIP1559Compatibility**(): *Promise‹unknown›*

Defined in NetworkController.ts:317

**Returns:** *Promise‹unknown›*

___

### `Private` getIsCustomNetwork

▸ **getIsCustomNetwork**(`chainId?`: string): *boolean*

Defined in NetworkController.ts:164

**Parameters:**

Name | Type |
------ | ------ |
`chainId?` | string |

**Returns:** *boolean*

___

### `Protected` initialize

▸ **initialize**(): *this*

*Inherited from [BaseController](_basecontroller_.basecontroller.md).[initialize](_basecontroller_.basecontroller.md#protected-initialize)*

Defined in BaseController.ts:80

Enables the controller. This sets each config option as a member
variable on this instance and triggers any defined setters. This
also sets initial state and triggers any listeners.

**Returns:** *this*

This controller instance.

___

### `Private` initializeProvider

▸ **initializeProvider**(`type`: [NetworkType](../modules/_networkcontroller_.md#networktype), `rpcTarget?`: string, `chainId?`: string, `ticker?`: string, `nickname?`: string): *void*

Defined in NetworkController.ts:103

**Parameters:**

Name | Type |
------ | ------ |
`type` | [NetworkType](../modules/_networkcontroller_.md#networktype) |
`rpcTarget?` | string |
`chainId?` | string |
`ticker?` | string |
`nickname?` | string |

**Returns:** *void*

___

###  lookupNetwork

▸ **lookupNetwork**(): *Promise‹void›*

Defined in NetworkController.ts:260

Refreshes the current network code.

**Returns:** *Promise‹void›*

___

###  notify

▸ **notify**(): *void*

*Inherited from [BaseController](_basecontroller_.basecontroller.md).[notify](_basecontroller_.basecontroller.md#notify)*

Defined in BaseController.ts:138

Notifies all subscribed listeners of current state.

**Returns:** *void*

___

### `Private` refreshNetwork

▸ **refreshNetwork**(): *void*

Defined in NetworkController.ts:133

**Returns:** *void*

___

### `Private` registerProvider

▸ **registerProvider**(): *void*

Defined in NetworkController.ts:140

**Returns:** *void*

___

### `Private` safelyStopProvider

▸ **safelyStopProvider**(`provider`: any): *void*

Defined in NetworkController.ts:200

**Parameters:**

Name | Type |
------ | ------ |
`provider` | any |

**Returns:** *void*

___

###  setProviderType

▸ **setProviderType**(`type`: [NetworkType](../modules/_networkcontroller_.md#networktype)): *void*

Defined in NetworkController.ts:282

Convenience method to update provider network type settings.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`type` | [NetworkType](../modules/_networkcontroller_.md#networktype) | Human readable network name.  |

**Returns:** *void*

___

###  setRpcTarget

▸ **setRpcTarget**(`rpcTarget`: string, `chainId`: string, `ticker?`: string, `nickname?`: string): *void*

Defined in NetworkController.ts:302

Convenience method to update provider RPC settings.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`rpcTarget` | string | The RPC endpoint URL. |
`chainId` | string | The chain ID as per EIP-155. |
`ticker?` | string | The currency ticker. |
`nickname?` | string | Personalized network name.  |

**Returns:** *void*

___

### `Private` setupInfuraProvider

▸ **setupInfuraProvider**(`type`: [NetworkType](../modules/_networkcontroller_.md#networktype)): *void*

Defined in NetworkController.ts:145

**Parameters:**

Name | Type |
------ | ------ |
`type` | [NetworkType](../modules/_networkcontroller_.md#networktype) |

**Returns:** *void*

___

### `Private` setupStandardProvider

▸ **setupStandardProvider**(`rpcTarget`: string, `chainId?`: string, `ticker?`: string, `nickname?`: string): *void*

Defined in NetworkController.ts:175

**Parameters:**

Name | Type |
------ | ------ |
`rpcTarget` | string |
`chainId?` | string |
`ticker?` | string |
`nickname?` | string |

**Returns:** *void*

___

###  subscribe

▸ **subscribe**(`listener`: [Listener](../modules/_basecontroller_.md#listener)‹[NetworkState](../interfaces/_networkcontroller_.networkstate.md)›): *void*

*Inherited from [BaseController](_basecontroller_.basecontroller.md).[subscribe](_basecontroller_.basecontroller.md#subscribe)*

Defined in BaseController.ts:153

Adds new listener to be notified of state changes.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`listener` | [Listener](../modules/_basecontroller_.md#listener)‹[NetworkState](../interfaces/_networkcontroller_.networkstate.md)› | The callback triggered when state changes.  |

**Returns:** *void*

___

###  unsubscribe

▸ **unsubscribe**(`listener`: [Listener](../modules/_basecontroller_.md#listener)‹[NetworkState](../interfaces/_networkcontroller_.networkstate.md)›): *boolean*

*Inherited from [BaseController](_basecontroller_.basecontroller.md).[unsubscribe](_basecontroller_.basecontroller.md#unsubscribe)*

Defined in BaseController.ts:163

Removes existing listener from receiving state changes.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`listener` | [Listener](../modules/_basecontroller_.md#listener)‹[NetworkState](../interfaces/_networkcontroller_.networkstate.md)› | The callback to remove. |

**Returns:** *boolean*

`true` if a listener is found and unsubscribed.

___

###  update

▸ **update**(`state`: Partial‹[NetworkState](../interfaces/_networkcontroller_.networkstate.md)›, `overwrite`: boolean): *void*

*Inherited from [BaseController](_basecontroller_.basecontroller.md).[update](_basecontroller_.basecontroller.md#update)*

Defined in BaseController.ts:175

Updates controller state.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`state` | Partial‹[NetworkState](../interfaces/_networkcontroller_.networkstate.md)› | - | The new state. |
`overwrite` | boolean | false | Overwrite state instead of merging.  |

**Returns:** *void*

___

### `Private` updateProvider

▸ **updateProvider**(`provider`: any): *void*

Defined in NetworkController.ts:194

**Parameters:**

Name | Type |
------ | ------ |
`provider` | any |

**Returns:** *void*

___

### `Private` verifyNetwork

▸ **verifyNetwork**(): *void*

Defined in NetworkController.ts:206

**Returns:** *void*
