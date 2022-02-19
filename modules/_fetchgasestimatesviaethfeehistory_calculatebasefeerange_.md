[metamask-controllers-main-src-gas-2](../README.md) › [Globals](../globals.md) › ["fetchGasEstimatesViaEthFeeHistory/calculateBaseFeeRange"](_fetchgasestimatesviaethfeehistory_calculatebasefeerange_.md)

# Module: "fetchGasEstimatesViaEthFeeHistory/calculateBaseFeeRange"

## Index

### Functions

* [calculateBaseFeeRange](_fetchgasestimatesviaethfeehistory_calculatebasefeerange_.md#calculatebasefeerange)

## Functions

###  calculateBaseFeeRange

▸ **calculateBaseFeeRange**‹**Percentile**›(`blocks`: [FeeHistoryBlock](_fetchblockfeehistory_.md#feehistoryblock)‹Percentile›[]): *[FeeRange](_fetchgasestimatesviaethfeehistory_types_.md#feerange)*

Defined in fetchGasEstimatesViaEthFeeHistory/calculateBaseFeeRange.ts:12

Calculates reasonable minimum and maximum values for base fees over the last 200 blocks.

**Type parameters:**

▪ **Percentile**: *number*

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`blocks` | [FeeHistoryBlock](_fetchblockfeehistory_.md#feehistoryblock)‹Percentile›[] | A set of blocks obtained via [BlockFeeHistoryDatasetFetcher](../classes/_fetchgasestimatesviaethfeehistory_blockfeehistorydatasetfetcher_.blockfeehistorydatasetfetcher.md). |

**Returns:** *[FeeRange](_fetchgasestimatesviaethfeehistory_types_.md#feerange)*

The ranges.
