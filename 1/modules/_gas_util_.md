[ethereum-gas-reference](../README.md) › [Globals](../globals.md) › ["gas-util"](_gas_util_.md)

# Module: "gas-util"

## Index

### Functions

* [calculateTimeEstimate](_gas_util_.md#calculatetimeestimate)
* [fetchEthGasPriceEstimate](_gas_util_.md#fetchethgaspriceestimate)
* [fetchGasEstimates](_gas_util_.md#fetchgasestimates)
* [fetchLegacyGasPriceEstimates](_gas_util_.md#fetchlegacygaspriceestimates)
* [makeClientIdHeader](_gas_util_.md#const-makeclientidheader)
* [normalizeGWEIDecimalNumbers](_gas_util_.md#normalizegweidecimalnumbers)

## Functions

###  calculateTimeEstimate

▸ **calculateTimeEstimate**(`maxPriorityFeePerGas`: string, `maxFeePerGas`: string, `gasFeeEstimates`: [GasFeeEstimates](_gasfeecontroller_.md#gasfeeestimates)): *[EstimatedGasFeeTimeBounds](_gasfeecontroller_.md#estimatedgasfeetimebounds)*

Defined in gas-util.ts:130

Estimate the time it will take for a transaction to be confirmed.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`maxPriorityFeePerGas` | string | The max priority fee per gas. |
`maxFeePerGas` | string | The max fee per gas. |
`gasFeeEstimates` | [GasFeeEstimates](_gasfeecontroller_.md#gasfeeestimates) | The gas fee estimates. |

**Returns:** *[EstimatedGasFeeTimeBounds](_gasfeecontroller_.md#estimatedgasfeetimebounds)*

The estimated lower and upper bounds for when this transaction will be confirmed.

___

###  fetchEthGasPriceEstimate

▸ **fetchEthGasPriceEstimate**(`ethQuery`: any): *Promise‹[EthGasPriceEstimate](_gasfeecontroller_.md#ethgaspriceestimate)›*

Defined in gas-util.ts:113

Get a gas price estimate from the network using the `eth_gasPrice` method.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`ethQuery` | any | The EthQuery instance to call the network with. |

**Returns:** *Promise‹[EthGasPriceEstimate](_gasfeecontroller_.md#ethgaspriceestimate)›*

A gas price estimate.

___

###  fetchGasEstimates

▸ **fetchGasEstimates**(`url`: string, `clientId?`: string): *Promise‹[GasFeeEstimates](_gasfeecontroller_.md#gasfeeestimates)›*

Defined in gas-util.ts:32

Fetch gas estimates from the given URL.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`url` | string | The gas estimate URL. |
`clientId?` | string | The client ID used to identify to the API who is asking for estimates. |

**Returns:** *Promise‹[GasFeeEstimates](_gasfeecontroller_.md#gasfeeestimates)›*

The gas estimates.

___

###  fetchLegacyGasPriceEstimates

▸ **fetchLegacyGasPriceEstimates**(`url`: string, `clientId?`: string): *Promise‹[LegacyGasPriceEstimate](_gasfeecontroller_.md#legacygaspriceestimate)›*

Defined in gas-util.ts:86

Hit the legacy MetaSwaps gasPrices estimate api and return the low, medium
high values from that API.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`url` | string | The URL to fetch gas price estimates from. |
`clientId?` | string | The client ID used to identify to the API who is asking for estimates. |

**Returns:** *Promise‹[LegacyGasPriceEstimate](_gasfeecontroller_.md#legacygaspriceestimate)›*

The gas price estimates.

___

### `Const` makeClientIdHeader

▸ **makeClientIdHeader**(`clientId`: string): *object*

Defined in gas-util.ts:11

**Parameters:**

Name | Type |
------ | ------ |
`clientId` | string |

**Returns:** *object*

* **X-Client-Id**: *string* = clientId

___

###  normalizeGWEIDecimalNumbers

▸ **normalizeGWEIDecimalNumbers**(`n`: string | number): *any*

Defined in gas-util.ts:19

Convert a decimal GWEI value to a decimal string rounded to the nearest WEI.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`n` | string &#124; number | The input GWEI amount, as a decimal string or a number. |

**Returns:** *any*

The decimal string GWEI amount.
