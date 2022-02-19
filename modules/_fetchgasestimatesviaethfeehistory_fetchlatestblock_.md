[metamask-controllers-main-src-gas-2](../README.md) › [Globals](../globals.md) › ["fetchGasEstimatesViaEthFeeHistory/fetchLatestBlock"](_fetchgasestimatesviaethfeehistory_fetchlatestblock_.md)

# Module: "fetchGasEstimatesViaEthFeeHistory/fetchLatestBlock"

## Index

### Functions

* [fetchLatestBlock](_fetchgasestimatesviaethfeehistory_fetchlatestblock_.md#fetchlatestblock)

## Functions

###  fetchLatestBlock

▸ **fetchLatestBlock**(`ethQuery`: [EthQuery](_fetchgasestimatesviaethfeehistory_types_.md#ethquery), `includeFullTransactionData`: boolean): *Promise‹[EthBlock](_fetchgasestimatesviaethfeehistory_types_.md#ethblock)›*

Defined in fetchGasEstimatesViaEthFeeHistory/fetchLatestBlock.ts:12

Returns information about the latest completed block.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`ethQuery` | [EthQuery](_fetchgasestimatesviaethfeehistory_types_.md#ethquery) | - | An EthQuery instance |
`includeFullTransactionData` | boolean | false | Whether or not to include all data for transactions as opposed to merely hashes. False by default. |

**Returns:** *Promise‹[EthBlock](_fetchgasestimatesviaethfeehistory_types_.md#ethblock)›*

The block.
