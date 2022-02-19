[ethereum-gas-reference](../README.md) › [Globals](../globals.md) › ["fetchGasEstimatesViaEthFeeHistory/calculateBaseFeeTrend"](_fetchgasestimatesviaethfeehistory_calculatebasefeetrend_.md)

# Module: "fetchGasEstimatesViaEthFeeHistory/calculateBaseFeeTrend"

## Index

### Functions

* [calculateBaseFeeTrend](_fetchgasestimatesviaethfeehistory_calculatebasefeetrend_.md#calculatebasefeetrend)

## Functions

###  calculateBaseFeeTrend

▸ **calculateBaseFeeTrend**‹**Percentile**›(`blocks`: [FeeHistoryBlock](_fetchblockfeehistory_.md#feehistoryblock)‹Percentile›[]): *"up" | "down" | "level"*

Defined in fetchGasEstimatesViaEthFeeHistory/calculateBaseFeeTrend.ts:10

Given a collection of blocks, returns an indicator of whether the base fee is moving up, down, or
holding steady, based on comparing the last base fee in the collection to the first.

**Type parameters:**

▪ **Percentile**: *number*

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`blocks` | [FeeHistoryBlock](_fetchblockfeehistory_.md#feehistoryblock)‹Percentile›[] | A set of blocks obtained via [BlockFeeHistoryDatasetFetcher](../classes/_fetchgasestimatesviaethfeehistory_blockfeehistorydatasetfetcher_.blockfeehistorydatasetfetcher.md). |

**Returns:** *"up" | "down" | "level"*

The indicator ("up", "down", or "level").
