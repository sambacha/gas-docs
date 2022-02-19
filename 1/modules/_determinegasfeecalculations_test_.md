[ethereum-gas-reference](../README.md) › [Globals](../globals.md) › ["determineGasFeeCalculations.test"](_determinegasfeecalculations_test_.md)

# Module: "determineGasFeeCalculations.test"

## Index

### Variables

* [mockedCalculateTimeEstimate](_determinegasfeecalculations_test_.md#const-mockedcalculatetimeestimate)
* [mockedFetchEthGasPriceEstimate](_determinegasfeecalculations_test_.md#const-mockedfetchethgaspriceestimate)
* [mockedFetchGasEstimates](_determinegasfeecalculations_test_.md#const-mockedfetchgasestimates)
* [mockedFetchGasEstimatesViaEthFeeHistory](_determinegasfeecalculations_test_.md#const-mockedfetchgasestimatesviaethfeehistory)
* [mockedFetchLegacyGasPriceEstimates](_determinegasfeecalculations_test_.md#const-mockedfetchlegacygaspriceestimates)

### Functions

* [buildMockDataForCalculateTimeEstimate](_determinegasfeecalculations_test_.md#buildmockdataforcalculatetimeestimate)
* [buildMockDataForFetchEthGasPriceEstimate](_determinegasfeecalculations_test_.md#buildmockdataforfetchethgaspriceestimate)
* [buildMockDataForFetchGasEstimates](_determinegasfeecalculations_test_.md#buildmockdataforfetchgasestimates)
* [buildMockDataForFetchLegacyGasPriceEstimates](_determinegasfeecalculations_test_.md#buildmockdataforfetchlegacygaspriceestimates)

## Variables

### `Const` mockedCalculateTimeEstimate

• **mockedCalculateTimeEstimate**: *any* = mocked(calculateTimeEstimate, true)

Defined in determineGasFeeCalculations.test.ts:27

___

### `Const` mockedFetchEthGasPriceEstimate

• **mockedFetchEthGasPriceEstimate**: *any* = mocked(fetchEthGasPriceEstimate, true)

Defined in determineGasFeeCalculations.test.ts:26

___

### `Const` mockedFetchGasEstimates

• **mockedFetchGasEstimates**: *any* = mocked(fetchGasEstimates, true)

Defined in determineGasFeeCalculations.test.ts:21

___

### `Const` mockedFetchGasEstimatesViaEthFeeHistory

• **mockedFetchGasEstimatesViaEthFeeHistory**: *any* = mocked(
  fetchGasEstimatesViaEthFeeHistory,
  true,
)

Defined in determineGasFeeCalculations.test.ts:28

___

### `Const` mockedFetchLegacyGasPriceEstimates

• **mockedFetchLegacyGasPriceEstimates**: *any* = mocked(
  fetchLegacyGasPriceEstimates,
  true,
)

Defined in determineGasFeeCalculations.test.ts:22

## Functions

###  buildMockDataForCalculateTimeEstimate

▸ **buildMockDataForCalculateTimeEstimate**(): *[EstimatedGasFeeTimeBounds](_gasfeecontroller_.md#estimatedgasfeetimebounds)*

Defined in determineGasFeeCalculations.test.ts:105

Builds mock data for the `calculateTimeEstimate` function. All of the data here is filled in to
make the gas fee estimation code function in a way that represents a reasonably happy path; it
does not necessarily match the real world.

**Returns:** *[EstimatedGasFeeTimeBounds](_gasfeecontroller_.md#estimatedgasfeetimebounds)*

The mock data.

___

###  buildMockDataForFetchEthGasPriceEstimate

▸ **buildMockDataForFetchEthGasPriceEstimate**(): *[EthGasPriceEstimate](_gasfeecontroller_.md#ethgaspriceestimate)*

Defined in determineGasFeeCalculations.test.ts:92

Builds mock data for the `fetchEthGasPriceEstimate` function. All of the data here is filled in
to make the gas fee estimation code function in a way that represents a reasonably happy path; it
does not necessarily match the real world.

**Returns:** *[EthGasPriceEstimate](_gasfeecontroller_.md#ethgaspriceestimate)*

The mock data.

___

###  buildMockDataForFetchGasEstimates

▸ **buildMockDataForFetchGasEstimates**(): *[GasFeeEstimates](_gasfeecontroller_.md#gasfeeestimates)*

Defined in determineGasFeeCalculations.test.ts:40

Builds mock data for the `fetchGasEstimates` function. All of the data here is filled in to make
the gas fee estimation code function in a way that represents a reasonably happy path; it does
not necessarily match the real world.

**Returns:** *[GasFeeEstimates](_gasfeecontroller_.md#gasfeeestimates)*

The mock data.

___

###  buildMockDataForFetchLegacyGasPriceEstimates

▸ **buildMockDataForFetchLegacyGasPriceEstimates**(): *[LegacyGasPriceEstimate](_gasfeecontroller_.md#legacygaspriceestimate)*

Defined in determineGasFeeCalculations.test.ts:77

Builds mock data for the `fetchLegacyGasPriceEstimates` function. All of the data here is filled
in to make the gas fee estimation code function in a way that represents a reasonably happy path;
it does not necessarily match the real world.

**Returns:** *[LegacyGasPriceEstimate](_gasfeecontroller_.md#legacygaspriceestimate)*

The mock data.
