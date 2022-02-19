[ethereum-gas-reference](../README.md) › [Globals](../globals.md) › ["GasFeeController"](_gasfeecontroller_.md)

# Module: "GasFeeController"

## Index

### Classes

* [GasFeeController](../classes/_gasfeecontroller_.gasfeecontroller.md)

### Type aliases

* [Eip1559GasFee](_gasfeecontroller_.md#eip1559gasfee)
* [EstimatedGasFeeTimeBounds](_gasfeecontroller_.md#estimatedgasfeetimebounds)
* [EthGasPriceEstimate](_gasfeecontroller_.md#ethgaspriceestimate)
* [EthGasPriceEstimateType](_gasfeecontroller_.md#ethgaspriceestimatetype)
* [FeeMarketEstimateType](_gasfeecontroller_.md#feemarketestimatetype)
* [FetchGasFeeEstimateOptions](_gasfeecontroller_.md#fetchgasfeeestimateoptions)
* [GasEstimateType](_gasfeecontroller_.md#gasestimatetype)
* [GasFeeEstimates](_gasfeecontroller_.md#gasfeeestimates)
* [GasFeeMessenger](_gasfeecontroller_.md#gasfeemessenger)
* [GasFeeState](_gasfeecontroller_.md#gasfeestate)
* [GasFeeStateChange](_gasfeecontroller_.md#gasfeestatechange)
* [GasFeeStateEthGasPrice](_gasfeecontroller_.md#gasfeestateethgasprice)
* [GasFeeStateFeeMarket](_gasfeecontroller_.md#gasfeestatefeemarket)
* [GasFeeStateLegacy](_gasfeecontroller_.md#gasfeestatelegacy)
* [GasFeeStateNoEstimates](_gasfeecontroller_.md#gasfeestatenoestimates)
* [GetGasFeeState](_gasfeecontroller_.md#getgasfeestate)
* [LegacyEstimateType](_gasfeecontroller_.md#legacyestimatetype)
* [LegacyGasPriceEstimate](_gasfeecontroller_.md#legacygaspriceestimate)
* [NoEstimateType](_gasfeecontroller_.md#noestimatetype)
* [unknownString](_gasfeecontroller_.md#unknownstring)

### Variables

* [GAS_FEE_API](_gasfeecontroller_.md#const-gas_fee_api)
* [LEGACY_GAS_PRICES_API_URL](_gasfeecontroller_.md#const-legacy_gas_prices_api_url)
* [currentAccountIsEIP1559Compatible](_gasfeecontroller_.md#const-currentaccountiseip1559compatible)
* [currentNetworkIsEIP1559Compatible](_gasfeecontroller_.md#const-currentnetworkiseip1559compatible)
* [gasFeeCalculations](_gasfeecontroller_.md#const-gasfeecalculations)
* [name](_gasfeecontroller_.md#const-name)
* [provider](_gasfeecontroller_.md#const-provider)

### Object literals

* [GAS_ESTIMATE_TYPES](_gasfeecontroller_.md#const-gas_estimate_types)
* [defaultState](_gasfeecontroller_.md#const-defaultstate)
* [metadata](_gasfeecontroller_.md#const-metadata)

## Type aliases

###  Eip1559GasFee

Ƭ **Eip1559GasFee**: *object*

Defined in GasFeeController.ts:103

**`property`** minWaitTimeEstimate - The fastest the transaction will take, in milliseconds

**`property`** maxWaitTimeEstimate - The slowest the transaction will take, in milliseconds

**`property`** suggestedMaxPriorityFeePerGas - A suggested "tip", a GWEI hex number

**`property`** suggestedMaxFeePerGas - A suggested max fee, the most a user will pay. a GWEI hex number

#### Type declaration:

* **maxWaitTimeEstimate**: *number*

* **minWaitTimeEstimate**: *number*

* **suggestedMaxFeePerGas**: *string*

* **suggestedMaxPriorityFeePerGas**: *string*

___

###  EstimatedGasFeeTimeBounds

Ƭ **EstimatedGasFeeTimeBounds**: *object*

Defined in GasFeeController.ts:59

#### Type declaration:

* **lowerTimeBound**: *number | null*

* **upperTimeBound**: *number | [unknownString](_gasfeecontroller_.md#unknownstring)*

___

###  EthGasPriceEstimate

Ƭ **EthGasPriceEstimate**: *object*

Defined in GasFeeController.ts:73

**`property`** gasPrice - A GWEI dec string

#### Type declaration:

* **gasPrice**: *string*

___

###  EthGasPriceEstimateType

Ƭ **EthGasPriceEstimateType**: *"eth_gasPrice"*

Defined in GasFeeController.ts:35

___

###  FeeMarketEstimateType

Ƭ **FeeMarketEstimateType**: *"fee-market"*

Defined in GasFeeController.ts:26

___

###  FetchGasFeeEstimateOptions

Ƭ **FetchGasFeeEstimateOptions**: *object*

Defined in GasFeeController.ts:165

#### Type declaration:

* **shouldUpdateState**? : *boolean*

___

###  GasEstimateType

Ƭ **GasEstimateType**: *[FeeMarketEstimateType](_gasfeecontroller_.md#feemarketestimatetype) | [EthGasPriceEstimateType](_gasfeecontroller_.md#ethgaspriceestimatetype) | [LegacyEstimateType](_gasfeecontroller_.md#legacyestimatetype) | [NoEstimateType](_gasfeecontroller_.md#noestimatetype)*

Defined in GasFeeController.ts:53

___

###  GasFeeEstimates

Ƭ **GasFeeEstimates**: *object*

Defined in GasFeeController.ts:122

**`property`** low - A GasFee for a minimum necessary combination of tip and maxFee

**`property`** medium - A GasFee for a recommended combination of tip and maxFee

**`property`** high - A GasFee for a high combination of tip and maxFee

**`property`** estimatedBaseFee - An estimate of what the base fee will be for the pending/next block. A GWEI dec number

**`property`** networkCongestion - A normalized number that can be used to gauge the congestion
level of the network, with 0 meaning not congested and 1 meaning extremely congested

#### Type declaration:

* **baseFeeTrend**: *"up" | "down" | "level"*

* **estimatedBaseFee**: *string*

* **high**: *[Eip1559GasFee](_gasfeecontroller_.md#eip1559gasfee)*

* **historicalBaseFeeRange**: *[string, string]*

* **historicalPriorityFeeRange**: *[string, string]*

* **latestPriorityFeeRange**: *[string, string]*

* **low**: *[Eip1559GasFee](_gasfeecontroller_.md#eip1559gasfee)*

* **medium**: *[Eip1559GasFee](_gasfeecontroller_.md#eip1559gasfee)*

* **networkCongestion**: *number*

* **priorityFeeTrend**: *"up" | "down" | "level"*

___

###  GasFeeMessenger

Ƭ **GasFeeMessenger**: *[RestrictedControllerMessenger](../classes/_controllermessenger_.restrictedcontrollermessenger.md)‹typeof name, [GetGasFeeState](_gasfeecontroller_.md#getgasfeestate), [GasFeeStateChange](_gasfeecontroller_.md#gasfeestatechange), never, never›*

Defined in GasFeeController.ts:194

___

###  GasFeeState

Ƭ **GasFeeState**: *[GasFeeStateEthGasPrice](_gasfeecontroller_.md#gasfeestateethgasprice) | [GasFeeStateFeeMarket](_gasfeecontroller_.md#gasfeestatefeemarket) | [GasFeeStateLegacy](_gasfeecontroller_.md#gasfeestatelegacy) | [GasFeeStateNoEstimates](_gasfeecontroller_.md#gasfeestatenoestimates)*

Defined in GasFeeController.ts:176

**`property`** gasFeeEstimates - Gas fee estimate data based on new EIP-1559 properties

**`property`** estimatedGasFeeTimeBounds - Estimates representing the minimum and maximum

___

###  GasFeeStateChange

Ƭ **GasFeeStateChange**: *object*

Defined in GasFeeController.ts:184

#### Type declaration:

* **type**: **

___

###  GasFeeStateEthGasPrice

Ƭ **GasFeeStateEthGasPrice**: *object*

Defined in GasFeeController.ts:141

#### Type declaration:

* **estimatedGasFeeTimeBounds**: *Record‹string, never›*

* **gasEstimateType**: *[EthGasPriceEstimateType](_gasfeecontroller_.md#ethgaspriceestimatetype)*

* **gasFeeEstimates**: *[EthGasPriceEstimate](_gasfeecontroller_.md#ethgaspriceestimate)*

___

###  GasFeeStateFeeMarket

Ƭ **GasFeeStateFeeMarket**: *object*

Defined in GasFeeController.ts:147

#### Type declaration:

* **estimatedGasFeeTimeBounds**: *[EstimatedGasFeeTimeBounds](_gasfeecontroller_.md#estimatedgasfeetimebounds) | Record‹string, never›*

* **gasEstimateType**: *[FeeMarketEstimateType](_gasfeecontroller_.md#feemarketestimatetype)*

* **gasFeeEstimates**: *[GasFeeEstimates](_gasfeecontroller_.md#gasfeeestimates)*

___

###  GasFeeStateLegacy

Ƭ **GasFeeStateLegacy**: *object*

Defined in GasFeeController.ts:153

#### Type declaration:

* **estimatedGasFeeTimeBounds**: *Record‹string, never›*

* **gasEstimateType**: *[LegacyEstimateType](_gasfeecontroller_.md#legacyestimatetype)*

* **gasFeeEstimates**: *[LegacyGasPriceEstimate](_gasfeecontroller_.md#legacygaspriceestimate)*

___

###  GasFeeStateNoEstimates

Ƭ **GasFeeStateNoEstimates**: *object*

Defined in GasFeeController.ts:159

#### Type declaration:

* **estimatedGasFeeTimeBounds**: *Record‹string, never›*

* **gasEstimateType**: *[NoEstimateType](_gasfeecontroller_.md#noestimatetype)*

* **gasFeeEstimates**: *Record‹string, never›*

___

###  GetGasFeeState

Ƭ **GetGasFeeState**: *object*

Defined in GasFeeController.ts:189

#### Type declaration:

* **type**: **

___

###  LegacyEstimateType

Ƭ **LegacyEstimateType**: *"legacy"*

Defined in GasFeeController.ts:30

___

###  LegacyGasPriceEstimate

Ƭ **LegacyGasPriceEstimate**: *object*

Defined in GasFeeController.ts:87

**`property`** high - gasPrice, in decimal gwei string format, suggested for fast inclusion

**`property`** medium - gasPrice, in decimal gwei string format, suggested for avg inclusion

**`property`** low - gasPrice, in decimal gwei string format, suggested for slow inclusion

#### Type declaration:

* **high**: *string*

* **low**: *string*

* **medium**: *string*

___

###  NoEstimateType

Ƭ **NoEstimateType**: *"none"*

Defined in GasFeeController.ts:38

___

###  unknownString

Ƭ **unknownString**: *"unknown"*

Defined in GasFeeController.ts:22

## Variables

### `Const` GAS_FEE_API

• **GAS_FEE_API**: *"https://mock-gas-server.herokuapp.com/"* = "https://mock-gas-server.herokuapp.com/"

Defined in GasFeeController.ts:19

___

### `Const` LEGACY_GAS_PRICES_API_URL

• **LEGACY_GAS_PRICES_API_URL**: *"https://api.metaswap.codefi.network/gasPrices"* = `https://api.metaswap.codefi.network/gasPrices`

Defined in GasFeeController.ts:20

___

### `Const` currentAccountIsEIP1559Compatible

• **currentAccountIsEIP1559Compatible**: *any* = this.getCurrentAccountEIP1559Compatibility?.() ?? true

Defined in GasFeeController.ts:462

___

### `Const` currentNetworkIsEIP1559Compatible

• **currentNetworkIsEIP1559Compatible**: *any* = await this.getCurrentNetworkEIP1559Compatibility()

Defined in GasFeeController.ts:460

___

### `Const` gasFeeCalculations

• **gasFeeCalculations**: *[GasFeeState](_gasfeecontroller_.md#gasfeestate)* = await determineGasFeeCalculations({
      isEIP1559Compatible,
      isLegacyGasAPICompatible,
      fetchGasEstimates,
      fetchGasEstimatesUrl: this.EIP1559APIEndpoint.replace(
        '<chain_id>',
        `${chainId}`,
      ),
      fetchGasEstimatesViaEthFeeHistory,
      fetchLegacyGasPriceEstimates,
      fetchLegacyGasPriceEstimatesUrl: this.legacyAPIEndpoint.replace(
        '<chain_id>',
        `${chainId}`,
      ),
      fetchEthGasPriceEstimate,
      calculateTimeEstimate,
      clientId: this.clientId,
      ethQuery: this.ethQuery,
    })

Defined in GasFeeController.ts:381

___

### `Const` name

• **name**: *"GasFeeController"* = "GasFeeController"

Defined in GasFeeController.ts:182

___

### `Const` provider

• **provider**: *any* = getProvider()

Defined in GasFeeController.ts:309

## Object literals

### `Const` GAS_ESTIMATE_TYPES

### ▪ **GAS_ESTIMATE_TYPES**: *object*

Defined in GasFeeController.ts:46

Indicates which type of gasEstimate the controller is currently returning.
This is useful as a way of asserting that the shape of gasEstimates matches
expectations. NONE is a special case indicating that no previous gasEstimate
has been fetched.

###  ETH_GASPRICE

• **ETH_GASPRICE**: *"eth_gasPrice"* = 'eth_gasPrice' as EthGasPriceEstimateType

Defined in GasFeeController.ts:49

###  FEE_MARKET

• **FEE_MARKET**: *"fee-market"* = 'fee-market' as FeeMarketEstimateType

Defined in GasFeeController.ts:47

###  LEGACY

• **LEGACY**: *"legacy"* = 'legacy' as LegacyEstimateType

Defined in GasFeeController.ts:48

###  NONE

• **NONE**: *"none"* = 'none' as NoEstimateType

Defined in GasFeeController.ts:50

___

### `Const` defaultState

### ▪ **defaultState**: *object*

Defined in GasFeeController.ts:202

###  estimatedGasFeeTimeBounds

• **estimatedGasFeeTimeBounds**: *object*

Defined in GasFeeController.ts:204

#### Type declaration:

###  gasEstimateType

• **gasEstimateType**: *"none"* = GAS_ESTIMATE_TYPES.NONE

Defined in GasFeeController.ts:205

###  gasFeeEstimates

• **gasFeeEstimates**: *object*

Defined in GasFeeController.ts:203

#### Type declaration:

___

### `Const` metadata

### ▪ **metadata**: *object*

Defined in GasFeeController.ts:135

▪ **estimatedGasFeeTimeBounds**: *object*

Defined in GasFeeController.ts:137

* **anonymous**: *boolean* = false

* **persist**: *boolean* = true

▪ **gasEstimateType**: *object*

Defined in GasFeeController.ts:138

* **anonymous**: *boolean* = false

* **persist**: *boolean* = true

▪ **gasFeeEstimates**: *object*

Defined in GasFeeController.ts:136

* **anonymous**: *boolean* = false

* **persist**: *boolean* = true
