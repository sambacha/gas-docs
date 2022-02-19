[ethereum-gas-reference](../README.md) › [Globals](../globals.md) › ["getGasEstimatesViaEthFeeHistory"](_getgasestimatesviaethfeehistory_.md)

# Module: "getGasEstimatesViaEthFeeHistory"

## Index

### Type aliases

* [EthQuery](_getgasestimatesviaethfeehistory_.md#ethquery)
* [Percentile](_getgasestimatesviaethfeehistory_.md#percentile)
* [PriorityLevel](_getgasestimatesviaethfeehistory_.md#prioritylevel)

### Variables

* [NUMBER_OF_HISTORICAL_BLOCKS_TO_FETCH](_getgasestimatesviaethfeehistory_.md#const-number_of_historical_blocks_to_fetch)
* [NUMBER_OF_RECENT_BLOCKS_TO_FETCH](_getgasestimatesviaethfeehistory_.md#const-number_of_recent_blocks_to_fetch)
* [PRIORITY_LEVELS](_getgasestimatesviaethfeehistory_.md#const-priority_levels)
* [PRIORITY_LEVEL_PERCENTILES](_getgasestimatesviaethfeehistory_.md#const-priority_level_percentiles)

### Functions

* [calculateGasEstimatesForAllPriorityLevels](_getgasestimatesviaethfeehistory_.md#calculategasestimatesforallprioritylevels)
* [calculateGasEstimatesForPriorityLevel](_getgasestimatesviaethfeehistory_.md#calculategasestimatesforprioritylevel)
* [calculateNetworkCongestionLevelFrom](_getgasestimatesviaethfeehistory_.md#calculatenetworkcongestionlevelfrom)
* [fetchGasEstimatesViaEthFeeHistory](_getgasestimatesviaethfeehistory_.md#fetchgasestimatesviaethfeehistory)
* [medianOf](_getgasestimatesviaethfeehistory_.md#medianof)

### Object literals

* [SETTINGS_BY_PRIORITY_LEVEL](_getgasestimatesviaethfeehistory_.md#const-settings_by_priority_level)

## Type aliases

###  EthQuery

Ƭ **EthQuery**: *any*

Defined in getGasEstimatesViaEthFeeHistory.ts:9

___

###  Percentile

Ƭ **Percentile**: *typeof PRIORITY_LEVEL_PERCENTILES[number]*

Defined in getGasEstimatesViaEthFeeHistory.ts:11

___

###  PriorityLevel

Ƭ **PriorityLevel**: *typeof PRIORITY_LEVELS[number]*

Defined in getGasEstimatesViaEthFeeHistory.ts:10

## Variables

### `Const` NUMBER_OF_HISTORICAL_BLOCKS_TO_FETCH

• **NUMBER_OF_HISTORICAL_BLOCKS_TO_FETCH**: *20000* = 20000

Defined in getGasEstimatesViaEthFeeHistory.ts:13

___

### `Const` NUMBER_OF_RECENT_BLOCKS_TO_FETCH

• **NUMBER_OF_RECENT_BLOCKS_TO_FETCH**: *5* = 5

Defined in getGasEstimatesViaEthFeeHistory.ts:14

___

### `Const` PRIORITY_LEVELS

• **PRIORITY_LEVELS**: *["low", "medium", "high"]* = ['low', 'medium', 'high'] as const

Defined in getGasEstimatesViaEthFeeHistory.ts:15

___

### `Const` PRIORITY_LEVEL_PERCENTILES

• **PRIORITY_LEVEL_PERCENTILES**: *[10, 20, 30]* = [10, 20, 30] as const

Defined in getGasEstimatesViaEthFeeHistory.ts:16

## Functions

###  calculateGasEstimatesForAllPriorityLevels

▸ **calculateGasEstimatesForAllPriorityLevels**(`blocks`: [Block](../interfaces/_networkcontroller_.block.md)‹[Percentile](_getgasestimatesviaethfeehistory_.md#percentile)›[]): *Pick‹[GasFeeEstimates](_gasfeecontroller_.md#gasfeeestimates), [PriorityLevel](_getgasestimatesviaethfeehistory_.md#prioritylevel)›*

Defined in getGasEstimatesViaEthFeeHistory.ts:115

Calculates a set of estimates suitable for different priority levels based on the data returned
by `eth_feeHistory`.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`blocks` | [Block](../interfaces/_networkcontroller_.block.md)‹[Percentile](_getgasestimatesviaethfeehistory_.md#percentile)›[] | A set of blocks as obtained from [fetchBlockFeeHistory](_fetchblockfeehistory_.md#fetchblockfeehistory). |

**Returns:** *Pick‹[GasFeeEstimates](_gasfeecontroller_.md#gasfeeestimates), [PriorityLevel](_getgasestimatesviaethfeehistory_.md#prioritylevel)›*

The estimates.

___

###  calculateGasEstimatesForPriorityLevel

▸ **calculateGasEstimatesForPriorityLevel**(`priorityLevel`: [PriorityLevel](_getgasestimatesviaethfeehistory_.md#prioritylevel), `blocks`: [Block](../interfaces/_networkcontroller_.block.md)‹[Percentile](_getgasestimatesviaethfeehistory_.md#percentile)›[]): *[Eip1559GasFee](_gasfeecontroller_.md#eip1559gasfee)*

Defined in getGasEstimatesViaEthFeeHistory.ts:73

Calculates a set of estimates assigned to a particular priority level based on the data returned
by `eth_feeHistory`.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`priorityLevel` | [PriorityLevel](_getgasestimatesviaethfeehistory_.md#prioritylevel) | The level of fees that dictates how soon a transaction may go through ("low", "medium", or "high"). |
`blocks` | [Block](../interfaces/_networkcontroller_.block.md)‹[Percentile](_getgasestimatesviaethfeehistory_.md#percentile)›[] | A set of blocks as obtained from [fetchBlockFeeHistory](_fetchblockfeehistory_.md#fetchblockfeehistory). |

**Returns:** *[Eip1559GasFee](_gasfeecontroller_.md#eip1559gasfee)*

The estimates.

___

###  calculateNetworkCongestionLevelFrom

▸ **calculateNetworkCongestionLevelFrom**(`blocks`: [Block](../interfaces/_networkcontroller_.block.md)‹[Percentile](_getgasestimatesviaethfeehistory_.md#percentile)›[]): *Promise‹number›*

Defined in getGasEstimatesViaEthFeeHistory.ts:138

Calculates the approximate normalized ranking of the latest base fee in the given blocks among
the entirety of the blocks. That is, sorts all of the base fees, then finds the rank of the first
base fee that meets or exceeds the latest base fee among the base fees. The result is the rank
normalized as a number between 0 and 1, where 0 means that the latest base fee is the least of
all and 1 means that the latest base fee is the greatest of all. This can ultimately be used to
render a visualization of the status of the network for users.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`blocks` | [Block](../interfaces/_networkcontroller_.block.md)‹[Percentile](_getgasestimatesviaethfeehistory_.md#percentile)›[] | A set of blocks as obtained from [fetchBlockFeeHistory](_fetchblockfeehistory_.md#fetchblockfeehistory). |

**Returns:** *Promise‹number›*

A promise of a number between 0 and 1.

___

###  fetchGasEstimatesViaEthFeeHistory

▸ **fetchGasEstimatesViaEthFeeHistory**(`ethQuery`: [EthQuery](_getgasestimatesviaethfeehistory_.md#ethquery)): *Promise‹[GasFeeEstimates](_gasfeecontroller_.md#gasfeeestimates)›*

Defined in getGasEstimatesViaEthFeeHistory.ts:168

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
`ethQuery` | [EthQuery](_getgasestimatesviaethfeehistory_.md#ethquery) | An EthQuery instance. |

**Returns:** *Promise‹[GasFeeEstimates](_gasfeecontroller_.md#gasfeeestimates)›*

Base and priority fee estimates, categorized by priority level, as well as an estimate
for the next block's base fee.

___

###  medianOf

▸ **medianOf**(`numbers`: BN[]): *BN*

Defined in getGasEstimatesViaEthFeeHistory.ts:57

Finds the median among a list of numbers. Note that this is different from the implementation
in the MetaSwap API, as we want to hold to using BN as much as possible.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`numbers` | BN[] | A list of numbers, as BNs. Will be sorted automatically if unsorted. |

**Returns:** *BN*

The median number.

## Object literals

### `Const` SETTINGS_BY_PRIORITY_LEVEL

### ▪ **SETTINGS_BY_PRIORITY_LEVEL**: *object*

Defined in getGasEstimatesViaEthFeeHistory.ts:17

▪ **high**: *object*

Defined in getGasEstimatesViaEthFeeHistory.ts:38

* **baseFeePercentageMultiplier**: *BN‹›* = new BN(125)

* **minSuggestedMaxPriorityFeePerGas**: *BN‹›* = new BN(2_000_000_000)

* **percentile**: *10 | 20 | 30* = 30 as Percentile

* **priorityFeePercentageMultiplier**: *BN‹›* = new BN(98)

* **estimatedWaitTimes**: *object*

  * **maxWaitTimeEstimate**: *number* = 60000

  * **minWaitTimeEstimate**: *number* = 15000

▪ **low**: *object*

Defined in getGasEstimatesViaEthFeeHistory.ts:18

* **baseFeePercentageMultiplier**: *BN‹›* = new BN(110)

* **minSuggestedMaxPriorityFeePerGas**: *BN‹›* = new BN(1_000_000_000)

* **percentile**: *10 | 20 | 30* = 10 as Percentile

* **priorityFeePercentageMultiplier**: *BN‹›* = new BN(94)

* **estimatedWaitTimes**: *object*

  * **maxWaitTimeEstimate**: *number* = 30000

  * **minWaitTimeEstimate**: *number* = 15000

▪ **medium**: *object*

Defined in getGasEstimatesViaEthFeeHistory.ts:28

* **baseFeePercentageMultiplier**: *BN‹›* = new BN(120)

* **minSuggestedMaxPriorityFeePerGas**: *BN‹›* = new BN(1_500_000_000)

* **percentile**: *10 | 20 | 30* = 20 as Percentile

* **priorityFeePercentageMultiplier**: *BN‹›* = new BN(97)

* **estimatedWaitTimes**: *object*

  * **maxWaitTimeEstimate**: *number* = 45000

  * **minWaitTimeEstimate**: *number* = 15000
