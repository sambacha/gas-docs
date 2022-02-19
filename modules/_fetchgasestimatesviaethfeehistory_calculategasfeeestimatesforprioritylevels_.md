[metamask-controllers-main-src-gas-2](../README.md) › [Globals](../globals.md) › ["fetchGasEstimatesViaEthFeeHistory/calculateGasFeeEstimatesForPriorityLevels"](_fetchgasestimatesviaethfeehistory_calculategasfeeestimatesforprioritylevels_.md)

# Module: "fetchGasEstimatesViaEthFeeHistory/calculateGasFeeEstimatesForPriorityLevels"

## Index

### Type aliases

* [Percentile](_fetchgasestimatesviaethfeehistory_calculategasfeeestimatesforprioritylevels_.md#percentile)
* [PriorityLevel](_fetchgasestimatesviaethfeehistory_calculategasfeeestimatesforprioritylevels_.md#prioritylevel)

### Variables

* [PRIORITY_LEVELS](_fetchgasestimatesviaethfeehistory_calculategasfeeestimatesforprioritylevels_.md#const-priority_levels)
* [PRIORITY_LEVEL_PERCENTILES](_fetchgasestimatesviaethfeehistory_calculategasfeeestimatesforprioritylevels_.md#const-priority_level_percentiles)

### Functions

* [calculateEstimatesForPriorityLevel](_fetchgasestimatesviaethfeehistory_calculategasfeeestimatesforprioritylevels_.md#calculateestimatesforprioritylevel)
* [calculateGasFeeEstimatesForPriorityLevels](_fetchgasestimatesviaethfeehistory_calculategasfeeestimatesforprioritylevels_.md#calculategasfeeestimatesforprioritylevels)

### Object literals

* [SETTINGS_BY_PRIORITY_LEVEL](_fetchgasestimatesviaethfeehistory_calculategasfeeestimatesforprioritylevels_.md#const-settings_by_priority_level)

## Type aliases

###  Percentile

Ƭ **Percentile**: *typeof PRIORITY_LEVEL_PERCENTILES[number]*

Defined in fetchGasEstimatesViaEthFeeHistory/calculateGasFeeEstimatesForPriorityLevels.ts:9

___

###  PriorityLevel

Ƭ **PriorityLevel**: *typeof PRIORITY_LEVELS[number]*

Defined in fetchGasEstimatesViaEthFeeHistory/calculateGasFeeEstimatesForPriorityLevels.ts:8

## Variables

### `Const` PRIORITY_LEVELS

• **PRIORITY_LEVELS**: *["low", "medium", "high"]* = ['low', 'medium', 'high'] as const

Defined in fetchGasEstimatesViaEthFeeHistory/calculateGasFeeEstimatesForPriorityLevels.ts:11

___

### `Const` PRIORITY_LEVEL_PERCENTILES

• **PRIORITY_LEVEL_PERCENTILES**: *[10, 20, 30]* = [10, 20, 30] as const

Defined in fetchGasEstimatesViaEthFeeHistory/calculateGasFeeEstimatesForPriorityLevels.ts:12

## Functions

###  calculateEstimatesForPriorityLevel

▸ **calculateEstimatesForPriorityLevel**(`priorityLevel`: [PriorityLevel](_fetchgasestimatesviaethfeehistory_calculategasfeeestimatesforprioritylevels_.md#prioritylevel), `blocks`: [ExistingFeeHistoryBlock](_fetchblockfeehistory_.md#existingfeehistoryblock)‹[Percentile](_fetchgasestimatesviaethfeehistory_calculategasfeeestimatesforprioritylevels_.md#percentile)›[]): *[Eip1559GasFee](_gasfeecontroller_.md#eip1559gasfee)*

Defined in fetchGasEstimatesViaEthFeeHistory/calculateGasFeeEstimatesForPriorityLevels.ts:55

Calculates a set of estimates assigned to a particular priority level based on the data returned
by `eth_feeHistory`.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`priorityLevel` | [PriorityLevel](_fetchgasestimatesviaethfeehistory_calculategasfeeestimatesforprioritylevels_.md#prioritylevel) | The level of fees that dictates how soon a transaction may go through ("low", "medium", or "high"). |
`blocks` | [ExistingFeeHistoryBlock](_fetchblockfeehistory_.md#existingfeehistoryblock)‹[Percentile](_fetchgasestimatesviaethfeehistory_calculategasfeeestimatesforprioritylevels_.md#percentile)›[] | A set of blocks as obtained from [fetchBlockFeeHistory](_fetchblockfeehistory_.md#fetchblockfeehistory). |

**Returns:** *[Eip1559GasFee](_gasfeecontroller_.md#eip1559gasfee)*

The estimates.

___

###  calculateGasFeeEstimatesForPriorityLevels

▸ **calculateGasFeeEstimatesForPriorityLevels**(`blocks`: [ExistingFeeHistoryBlock](_fetchblockfeehistory_.md#existingfeehistoryblock)‹[Percentile](_fetchgasestimatesviaethfeehistory_calculategasfeeestimatesforprioritylevels_.md#percentile)›[]): *Pick‹[GasFeeEstimates](_gasfeecontroller_.md#gasfeeestimates), [PriorityLevel](_fetchgasestimatesviaethfeehistory_calculategasfeeestimatesforprioritylevels_.md#prioritylevel)›*

Defined in fetchGasEstimatesViaEthFeeHistory/calculateGasFeeEstimatesForPriorityLevels.ts:97

Calculates a set of estimates suitable for different priority levels based on the data returned
by `eth_feeHistory`.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`blocks` | [ExistingFeeHistoryBlock](_fetchblockfeehistory_.md#existingfeehistoryblock)‹[Percentile](_fetchgasestimatesviaethfeehistory_calculategasfeeestimatesforprioritylevels_.md#percentile)›[] | A set of blocks populated with data for priority fee percentiles 10, 20, and 30, obtained via [BlockFeeHistoryDatasetFetcher](../classes/_fetchgasestimatesviaethfeehistory_blockfeehistorydatasetfetcher_.blockfeehistorydatasetfetcher.md). |

**Returns:** *Pick‹[GasFeeEstimates](_gasfeecontroller_.md#gasfeeestimates), [PriorityLevel](_fetchgasestimatesviaethfeehistory_calculategasfeeestimatesforprioritylevels_.md#prioritylevel)›*

The estimates.

## Object literals

### `Const` SETTINGS_BY_PRIORITY_LEVEL

### ▪ **SETTINGS_BY_PRIORITY_LEVEL**: *object*

Defined in fetchGasEstimatesViaEthFeeHistory/calculateGasFeeEstimatesForPriorityLevels.ts:13

▪ **high**: *object*

Defined in fetchGasEstimatesViaEthFeeHistory/calculateGasFeeEstimatesForPriorityLevels.ts:34

* **baseFeePercentageMultiplier**: *BN‹›* = new BN(125)

* **minSuggestedMaxPriorityFeePerGas**: *BN‹›* = new BN(2_000_000_000)

* **percentile**: *10 | 20 | 30* = 30 as Percentile

* **priorityFeePercentageMultiplier**: *BN‹›* = new BN(98)

* **estimatedWaitTimes**: *object*

  * **maxWaitTimeEstimate**: *number* = 60000

  * **minWaitTimeEstimate**: *number* = 15000

▪ **low**: *object*

Defined in fetchGasEstimatesViaEthFeeHistory/calculateGasFeeEstimatesForPriorityLevels.ts:14

* **baseFeePercentageMultiplier**: *BN‹›* = new BN(110)

* **minSuggestedMaxPriorityFeePerGas**: *BN‹›* = new BN(1_000_000_000)

* **percentile**: *10 | 20 | 30* = 10 as Percentile

* **priorityFeePercentageMultiplier**: *BN‹›* = new BN(94)

* **estimatedWaitTimes**: *object*

  * **maxWaitTimeEstimate**: *number* = 30000

  * **minWaitTimeEstimate**: *number* = 15000

▪ **medium**: *object*

Defined in fetchGasEstimatesViaEthFeeHistory/calculateGasFeeEstimatesForPriorityLevels.ts:24

* **baseFeePercentageMultiplier**: *BN‹›* = new BN(120)

* **minSuggestedMaxPriorityFeePerGas**: *BN‹›* = new BN(1_500_000_000)

* **percentile**: *10 | 20 | 30* = 20 as Percentile

* **priorityFeePercentageMultiplier**: *BN‹›* = new BN(97)

* **estimatedWaitTimes**: *object*

  * **maxWaitTimeEstimate**: *number* = 45000

  * **minWaitTimeEstimate**: *number* = 15000
