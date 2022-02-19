[ethereum-gas-reference](../README.md) › [Globals](../globals.md) › ["GasFeeController.test"](_gasfeecontroller_test_.md)

# Module: "GasFeeController.test"

## Index

### Variables

* [mockedDetermineGasFeeCalculations](_gasfeecontroller_test_.md#const-mockeddeterminegasfeecalculations)
* [name](_gasfeecontroller_test_.md#const-name)

### Functions

* [buildMockGasFeeStateEthGasPrice](_gasfeecontroller_test_.md#buildmockgasfeestateethgasprice)
* [buildMockGasFeeStateFeeMarket](_gasfeecontroller_test_.md#buildmockgasfeestatefeemarket)
* [buildMockGasFeeStateLegacy](_gasfeecontroller_test_.md#buildmockgasfeestatelegacy)
* [getRestrictedMessenger](_gasfeecontroller_test_.md#getrestrictedmessenger)

## Variables

### `Const` mockedDetermineGasFeeCalculations

• **mockedDetermineGasFeeCalculations**: *any* = mocked(
  determineGasFeeCalculations,
  true,
)

Defined in GasFeeController.test.ts:18

___

### `Const` name

• **name**: *"GasFeeController"* = "GasFeeController"

Defined in GasFeeController.test.ts:23

## Functions

###  buildMockGasFeeStateEthGasPrice

▸ **buildMockGasFeeStateEthGasPrice**(`__namedParameters`: object): *[GasFeeStateEthGasPrice](_gasfeecontroller_.md#gasfeestateethgasprice)*

Defined in GasFeeController.test.ts:132

Builds mock gas fee state that would typically be generated for the case in which eth_gasPrice is
used to fetch estimates. This data is merely intended to fit the GasFeeStateEthGasPrice type and
does not represent any real-world scenario.

**Parameters:**

▪`Default value`  **__namedParameters**: *object*= {}

Name | Type | Default |
------ | ------ | ------ |
`modifier` | number | 1 |

**Returns:** *[GasFeeStateEthGasPrice](_gasfeecontroller_.md#gasfeestateethgasprice)*

The mock data.

___

###  buildMockGasFeeStateFeeMarket

▸ **buildMockGasFeeStateFeeMarket**(`__namedParameters`: object): *[GasFeeStateFeeMarket](_gasfeecontroller_.md#gasfeestatefeemarket)*

Defined in GasFeeController.test.ts:55

Builds mock gas fee state that would typically be generated for an EIP-1559-compatible network.
This data is merely intended to fit the GasFeeStateFeeMarket type and does not represent any
real-world scenario.

**Parameters:**

▪`Default value`  **__namedParameters**: *object*= {}

Name | Type | Default |
------ | ------ | ------ |
`modifier` | number | 1 |

**Returns:** *[GasFeeStateFeeMarket](_gasfeecontroller_.md#gasfeestatefeemarket)*

The mock data.

___

###  buildMockGasFeeStateLegacy

▸ **buildMockGasFeeStateLegacy**(`__namedParameters`: object): *[GasFeeStateLegacy](_gasfeecontroller_.md#gasfeestatelegacy)*

Defined in GasFeeController.test.ts:110

Builds mock gas fee state that would typically be generated for an non-EIP-1559-compatible
network. This data is merely intended to fit the GasFeeStateLegacy type and does not represent
any real-world scenario.

**Parameters:**

▪`Default value`  **__namedParameters**: *object*= {}

Name | Type | Default |
------ | ------ | ------ |
`modifier` | number | 1 |

**Returns:** *[GasFeeStateLegacy](_gasfeecontroller_.md#gasfeestatelegacy)*

The mock data.

___

###  getRestrictedMessenger

▸ **getRestrictedMessenger**(): *any*

Defined in GasFeeController.test.ts:30

Constructs a restricted controller messenger.

**Returns:** *any*

A restricted controller messenger.
