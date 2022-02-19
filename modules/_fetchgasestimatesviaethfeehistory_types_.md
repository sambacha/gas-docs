[metamask-controllers-main-src-gas-2](../README.md) › [Globals](../globals.md) › ["fetchGasEstimatesViaEthFeeHistory/types"](_fetchgasestimatesviaethfeehistory_types_.md)

# Module: "fetchGasEstimatesViaEthFeeHistory/types"

## Index

### Type aliases

* [EthBlock](_fetchgasestimatesviaethfeehistory_types_.md#ethblock)
* [EthQuery](_fetchgasestimatesviaethfeehistory_types_.md#ethquery)
* [FeeRange](_fetchgasestimatesviaethfeehistory_types_.md#feerange)

## Type aliases

###  EthBlock

Ƭ **EthBlock**: *object*

Defined in fetchGasEstimatesViaEthFeeHistory/types.ts:3

#### Type declaration:

* **baseFeePerGas**: *BN*

* **number**: *BN*

___

###  EthQuery

Ƭ **EthQuery**: *object*

Defined in fetchGasEstimatesViaEthFeeHistory/types.ts:8

#### Type declaration:

* **getBlockByNumber**(): *function*

  * (`blockNumber`: BN | "latest" | "earliest" | "pending"): *Promise‹[EthBlock](_fetchgasestimatesviaethfeehistory_types_.md#ethblock)›*

___

###  FeeRange

Ƭ **FeeRange**: *[string, string]*

Defined in fetchGasEstimatesViaEthFeeHistory/types.ts:14
