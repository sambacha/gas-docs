[metamask-controllers-main-src-gas-2](../README.md) › [Globals](../globals.md) › ["fetchGasEstimatesViaEthFeeHistory/calculatePriorityFeeTrend"](_fetchgasestimatesviaethfeehistory_calculatepriorityfeetrend_.md)

# Module: "fetchGasEstimatesViaEthFeeHistory/calculatePriorityFeeTrend"

## Index

### Functions

* [calculatePriorityFeeTrend](_fetchgasestimatesviaethfeehistory_calculatepriorityfeetrend_.md#calculatepriorityfeetrend)

## Functions

###  calculatePriorityFeeTrend

▸ **calculatePriorityFeeTrend**(`blocks`: [ExistingFeeHistoryBlock](_fetchblockfeehistory_.md#existingfeehistoryblock)‹50›[]): *"up" | "down" | "level"*

Defined in fetchGasEstimatesViaEthFeeHistory/calculatePriorityFeeTrend.ts:11

Given a collection of blocks, returns an indicator of whether the base fee is moving up, down, or
holding steady, based on comparing the last base fee in the collection to the first.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`blocks` | [ExistingFeeHistoryBlock](_fetchblockfeehistory_.md#existingfeehistoryblock)‹50›[] | A set of blocks obtained via [BlockFeeHistoryDatasetFetcher](../classes/_fetchgasestimatesviaethfeehistory_blockfeehistorydatasetfetcher_.blockfeehistorydatasetfetcher.md). |

**Returns:** *"up" | "down" | "level"*

The indicator ("up", "down", or "level").
