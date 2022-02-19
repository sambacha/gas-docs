[metamask-controllers-main-src-gas-2](../README.md) › [Globals](../globals.md) › ["fetchGasEstimatesViaEthFeeHistory/calculateNetworkCongestion"](_fetchgasestimatesviaethfeehistory_calculatenetworkcongestion_.md)

# Module: "fetchGasEstimatesViaEthFeeHistory/calculateNetworkCongestion"

## Index

### Functions

* [fetchNetworkCongestionLevel](_fetchgasestimatesviaethfeehistory_calculatenetworkcongestion_.md#fetchnetworkcongestionlevel)

## Functions

###  fetchNetworkCongestionLevel

▸ **fetchNetworkCongestionLevel**(`blocks`: [FeeHistoryBlock](_fetchblockfeehistory_.md#feehistoryblock)‹never›[]): *number*

Defined in fetchGasEstimatesViaEthFeeHistory/calculateNetworkCongestion.ts:14

Calculates the approximate normalized ranking of the latest base fee in the given blocks among
the entirety of the blocks. That is, sorts all of the base fees, then finds the rank of the first
base fee that meets or exceeds the latest base fee among the base fees. The result is the rank
normalized as a number between 0 and 1, where 0 means that the latest base fee is the least of
all and 1 means that the latest base fee is the greatest of all. This can ultimately be used to
render a visualization of the status of the network for users.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`blocks` | [FeeHistoryBlock](_fetchblockfeehistory_.md#feehistoryblock)‹never›[] | A set of blocks obtained via [BlockFeeHistoryDatasetFetcher](../classes/_fetchgasestimatesviaethfeehistory_blockfeehistorydatasetfetcher_.blockfeehistorydatasetfetcher.md). |

**Returns:** *number*

A number between 0 and 1.
