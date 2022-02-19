[metamask-controllers-main-src-gas-2](../README.md) › [Globals](../globals.md) › ["determineGasFeeCalculations"](_determinegasfeecalculations_.md)

# Module: "determineGasFeeCalculations"

## Index

### Functions

* [determineGasFeeCalculations](_determinegasfeecalculations_.md#determinegasfeecalculations)

## Functions

###  determineGasFeeCalculations

▸ **determineGasFeeCalculations**(`__namedParameters`: object): *Promise‹GasFeeCalculations›*

Defined in determineGasFeeCalculations.ts:36

Obtains a set of max base and priority fee estimates along with time estimates so that we
can present them to users when they are sending transactions or making swaps.

**Parameters:**

▪ **__namedParameters**: *object*

Name | Type |
------ | ------ |
`calculateTimeEstimate` | function |
`clientId` | string |
`ethQuery` | any |
`fetchEthGasPriceEstimate` | function |
`fetchGasEstimates` | function |
`fetchGasEstimatesUrl` | string |
`fetchGasEstimatesViaEthFeeHistory` | function |
`fetchLegacyGasPriceEstimates` | function |
`fetchLegacyGasPriceEstimatesUrl` | string |
`isEIP1559Compatible` | boolean |
`isLegacyGasAPICompatible` | boolean |

**Returns:** *Promise‹GasFeeCalculations›*

The gas fee calculations.
