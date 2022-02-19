[ethereum-gas-reference](../README.md) › [Globals](../globals.md) › ["fetchGasEstimatesViaEthFeeHistory/medianOf"](_fetchgasestimatesviaethfeehistory_medianof_.md)

# Module: "fetchGasEstimatesViaEthFeeHistory/medianOf"

## Index

### Functions

* [medianOf](_fetchgasestimatesviaethfeehistory_medianof_.md#medianof)

## Functions

###  medianOf

▸ **medianOf**(`numbers`: BN[]): *BN*

Defined in fetchGasEstimatesViaEthFeeHistory/medianOf.ts:10

Finds the median among a list of numbers. Note that this is different from the implementation
in the MetaSwap API, as we want to hold to using BN as much as possible.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`numbers` | BN[] | A list of numbers, as BNs. Will be sorted automatically if unsorted. |

**Returns:** *BN*

The median number.
