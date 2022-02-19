[ethereum-gas-reference](../README.md) › [Globals](../globals.md) › [NetworkState](networkstate.md)

# Interface: NetworkState

**`property`** network - Network ID as per net_version

**`property`** isCustomNetwork - Identifies if the network is a custom network

**`property`** provider - RPC URL and network name provider settings

## Hierarchy

* [BaseState](basestate.md)

  ↳ **NetworkState**

## Index

### Properties

* [isCustomNetwork](networkstate.md#iscustomnetwork)
* [name](networkstate.md#optional-name)
* [network](networkstate.md#network)
* [properties](networkstate.md#properties)
* [provider](networkstate.md#provider)

## Properties

###  isCustomNetwork

• **isCustomNetwork**: *boolean*

Defined in NetworkController.ts:83

___

### `Optional` name

• **name**? : *string*

*Inherited from [BaseState](basestate.md).[name](basestate.md#optional-name)*

Defined in BaseController.ts:23

___

###  network

• **network**: *string*

Defined in NetworkController.ts:82

___

###  properties

• **properties**: *[NetworkProperties](networkproperties.md)*

Defined in NetworkController.ts:85

___

###  provider

• **provider**: *[ProviderConfig](providerconfig.md)*

Defined in NetworkController.ts:84
