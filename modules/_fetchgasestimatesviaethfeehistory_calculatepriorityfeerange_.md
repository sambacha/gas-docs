[metamask-controllers-main-src-gas-2](../README.md) › [Globals](../globals.md) › ["fetchGasEstimatesViaEthFeeHistory/calculatePriorityFeeRange"](_fetchgasestimatesviaethfeehistory_calculatepriorityfeerange_.md)

# Module: "fetchGasEstimatesViaEthFeeHistory/calculatePriorityFeeRange"

## Index

### Functions

* [calculatePriorityFeeRange](_fetchgasestimatesviaethfeehistory_calculatepriorityfeerange_.md#calculatepriorityfeerange)

## Functions

###  calculatePriorityFeeRange

▸ **calculatePriorityFeeRange**(`blocks`: [ExistingFeeHistoryBlock](_fetchblockfeehistory_.md#existingfeehistoryblock)‹10 | 95›[]): *[FeeRange](_fetchgasestimatesviaethfeehistory_types_.md#feerange)*

Defined in fetchGasEstimatesViaEthFeeHistory/calculatePriorityFeeRange.ts:16

Calculates reasonable minimum and maximum values for priority fees over the last 200 blocks.
Although some priority fees may be 0, these are discarded as they are not useful for suggestion
purposes.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`blocks` | [ExistingFeeHistoryBlock](_fetchblockfeehistory_.md#existingfeehistoryblock)‹10 &#124; 95›[] | A set of blocks populated with data for priority fee percentiles 10 and 95, obtained via [BlockFeeHistoryDatasetFetcher](../classes/_fetchgasestimatesviaethfeehistory_blockfeehistorydatasetfetcher_.blockfeehistorydatasetfetcher.md). |

**Returns:** *[FeeRange](_fetchgasestimatesviaethfeehistory_types_.md#feerange)*

The range.
