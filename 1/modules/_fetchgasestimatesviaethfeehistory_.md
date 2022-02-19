[ethereum-gas-reference](../README.md) › [Globals](../globals.md) › ["fetchGasEstimatesViaEthFeeHistory"](_fetchgasestimatesviaethfeehistory_.md)

# Module: "fetchGasEstimatesViaEthFeeHistory"

## Index

### Functions

* [fetchGasEstimatesViaEthFeeHistory](_fetchgasestimatesviaethfeehistory_.md#fetchgasestimatesviaethfeehistory)

## Functions

###  fetchGasEstimatesViaEthFeeHistory

▸ **fetchGasEstimatesViaEthFeeHistory**(`ethQuery`: [EthQuery](_fetchgasestimatesviaethfeehistory_types_.md#ethquery)): *Promise‹[GasFeeEstimates](_gasfeecontroller_.md#gasfeeestimates)›*

Defined in fetchGasEstimatesViaEthFeeHistory.ts:29

Generates gas fee estimates based on gas fees that have been used in the recent past so that
those estimates can be displayed to users.

To produce the estimates, the last 5 blocks are read from the network, and for each block, the
priority fees for transactions at the 10th, 20th, and 30th percentiles are also read (here
"percentile" signifies the level at which those transactions contribute to the overall gas used
for the block, where higher percentiles correspond to higher fees). This information is used to
calculate reasonable max priority and max fees for three different priority levels (higher
priority = higher fee).

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`ethQuery` | [EthQuery](_fetchgasestimatesviaethfeehistory_types_.md#ethquery) | An EthQuery instance. |

**Returns:** *Promise‹[GasFeeEstimates](_gasfeecontroller_.md#gasfeeestimates)›*

Base and priority fee estimates, categorized by priority level, as well as an estimate
for the next block's base fee.
