[ethereum-gas-reference](../README.md) › [Globals](../globals.md) › ["fetchGasEstimatesViaEthFeeHistory/BlockFeeHistoryDatasetFetcher"](../modules/_fetchgasestimatesviaethfeehistory_blockfeehistorydatasetfetcher_.md) › [BlockFeeHistoryDatasetFetcher](_fetchgasestimatesviaethfeehistory_blockfeehistorydatasetfetcher_.blockfeehistorydatasetfetcher.md)

# Class: BlockFeeHistoryDatasetFetcher

## Hierarchy

* **BlockFeeHistoryDatasetFetcher**

## Index

### Constructors

* [constructor](_fetchgasestimatesviaethfeehistory_blockfeehistorydatasetfetcher_.blockfeehistorydatasetfetcher.md#constructor)

### Properties

* [endBlockNumber](_fetchgasestimatesviaethfeehistory_blockfeehistorydatasetfetcher_.blockfeehistorydatasetfetcher.md#private-endblocknumber)
* [ethQuery](_fetchgasestimatesviaethfeehistory_blockfeehistorydatasetfetcher_.blockfeehistorydatasetfetcher.md#private-ethquery)

### Methods

* [fetchExcludingNextBlock](_fetchgasestimatesviaethfeehistory_blockfeehistorydatasetfetcher_.blockfeehistorydatasetfetcher.md#private-fetchexcludingnextblock)
* [fetchIncludingNextBlock](_fetchgasestimatesviaethfeehistory_blockfeehistorydatasetfetcher_.blockfeehistorydatasetfetcher.md#private-fetchincludingnextblock)
* [forAll](_fetchgasestimatesviaethfeehistory_blockfeehistorydatasetfetcher_.blockfeehistorydatasetfetcher.md#forall)
* [forLatestWithNextBlock](_fetchgasestimatesviaethfeehistory_blockfeehistorydatasetfetcher_.blockfeehistorydatasetfetcher.md#forlatestwithnextblock)
* [forLongRange](_fetchgasestimatesviaethfeehistory_blockfeehistorydatasetfetcher_.blockfeehistorydatasetfetcher.md#forlongrange)
* [forMediumRange](_fetchgasestimatesviaethfeehistory_blockfeehistorydatasetfetcher_.blockfeehistorydatasetfetcher.md#formediumrange)
* [forSmallRange](_fetchgasestimatesviaethfeehistory_blockfeehistorydatasetfetcher_.blockfeehistorydatasetfetcher.md#forsmallrange)
* [forTinyRange](_fetchgasestimatesviaethfeehistory_blockfeehistorydatasetfetcher_.blockfeehistorydatasetfetcher.md#fortinyrange)

## Constructors

###  constructor

\+ **new BlockFeeHistoryDatasetFetcher**(`__namedParameters`: object): *[BlockFeeHistoryDatasetFetcher](_fetchgasestimatesviaethfeehistory_blockfeehistorydatasetfetcher_.blockfeehistorydatasetfetcher.md)*

Defined in fetchGasEstimatesViaEthFeeHistory/BlockFeeHistoryDatasetFetcher.ts:12

**Parameters:**

▪ **__namedParameters**: *object*

Name | Type |
------ | ------ |
`endBlockNumber` | BN‹› |
`ethQuery` | [EthQuery](../modules/_fetchgasestimatesviaethfeehistory_types_.md#ethquery) |

**Returns:** *[BlockFeeHistoryDatasetFetcher](_fetchgasestimatesviaethfeehistory_blockfeehistorydatasetfetcher_.blockfeehistorydatasetfetcher.md)*

## Properties

### `Private` endBlockNumber

• **endBlockNumber**: *BN*

Defined in fetchGasEstimatesViaEthFeeHistory/BlockFeeHistoryDatasetFetcher.ts:12

___

### `Private` ethQuery

• **ethQuery**: *[EthQuery](../modules/_fetchgasestimatesviaethfeehistory_types_.md#ethquery)*

Defined in fetchGasEstimatesViaEthFeeHistory/BlockFeeHistoryDatasetFetcher.ts:10

## Methods

### `Private` fetchExcludingNextBlock

▸ **fetchExcludingNextBlock**‹**T**›(`args`: object): *Promise‹[ExistingFeeHistoryBlock](../modules/_fetchblockfeehistory_.md#existingfeehistoryblock)‹T›[]›*

Defined in fetchGasEstimatesViaEthFeeHistory/BlockFeeHistoryDatasetFetcher.ts:81

**Type parameters:**

▪ **T**: *number*

**Parameters:**

▪ **args**: *object*

Name | Type |
------ | ------ |
`endBlock?` | BN |
`numberOfBlocks` | number |
`percentiles?` | T[] |

**Returns:** *Promise‹[ExistingFeeHistoryBlock](../modules/_fetchblockfeehistory_.md#existingfeehistoryblock)‹T›[]›*

___

### `Private` fetchIncludingNextBlock

▸ **fetchIncludingNextBlock**‹**T**›(`args`: object): *Promise‹[FeeHistoryBlock](../modules/_fetchblockfeehistory_.md#feehistoryblock)‹T›[]›*

Defined in fetchGasEstimatesViaEthFeeHistory/BlockFeeHistoryDatasetFetcher.ts:93

**Type parameters:**

▪ **T**: *number*

**Parameters:**

▪ **args**: *object*

Name | Type |
------ | ------ |
`endBlock?` | BN |
`numberOfBlocks` | number |
`percentiles?` | T[] |

**Returns:** *Promise‹[FeeHistoryBlock](../modules/_fetchblockfeehistory_.md#feehistoryblock)‹T›[]›*

___

###  forAll

▸ **forAll**(): *Promise‹object›*

Defined in fetchGasEstimatesViaEthFeeHistory/BlockFeeHistoryDatasetFetcher.ts:25

**Returns:** *Promise‹object›*

___

###  forLatestWithNextBlock

▸ **forLatestWithNextBlock**(): *Promise‹[FeeHistoryBlock](../modules/_fetchblockfeehistory_.md#feehistoryblock)‹10 | 95›[]›*

Defined in fetchGasEstimatesViaEthFeeHistory/BlockFeeHistoryDatasetFetcher.ts:74

**Returns:** *Promise‹[FeeHistoryBlock](../modules/_fetchblockfeehistory_.md#feehistoryblock)‹10 | 95›[]›*

___

###  forLongRange

▸ **forLongRange**(): *Promise‹[ExistingFeeHistoryBlock](../modules/_fetchblockfeehistory_.md#existingfeehistoryblock)‹number›[]›*

Defined in fetchGasEstimatesViaEthFeeHistory/BlockFeeHistoryDatasetFetcher.ts:49

**Returns:** *Promise‹[ExistingFeeHistoryBlock](../modules/_fetchblockfeehistory_.md#existingfeehistoryblock)‹number›[]›*

___

###  forMediumRange

▸ **forMediumRange**(): *Promise‹[ExistingFeeHistoryBlock](../modules/_fetchblockfeehistory_.md#existingfeehistoryblock)‹10 | 95›[]›*

Defined in fetchGasEstimatesViaEthFeeHistory/BlockFeeHistoryDatasetFetcher.ts:53

**Returns:** *Promise‹[ExistingFeeHistoryBlock](../modules/_fetchblockfeehistory_.md#existingfeehistoryblock)‹10 | 95›[]›*

___

###  forSmallRange

▸ **forSmallRange**(): *Promise‹[ExistingFeeHistoryBlock](../modules/_fetchblockfeehistory_.md#existingfeehistoryblock)‹10 | 20 | 30›[]›*

Defined in fetchGasEstimatesViaEthFeeHistory/BlockFeeHistoryDatasetFetcher.ts:60

**Returns:** *Promise‹[ExistingFeeHistoryBlock](../modules/_fetchblockfeehistory_.md#existingfeehistoryblock)‹10 | 20 | 30›[]›*

___

###  forTinyRange

▸ **forTinyRange**(): *Promise‹[ExistingFeeHistoryBlock](../modules/_fetchblockfeehistory_.md#existingfeehistoryblock)‹50›[]›*

Defined in fetchGasEstimatesViaEthFeeHistory/BlockFeeHistoryDatasetFetcher.ts:67

**Returns:** *Promise‹[ExistingFeeHistoryBlock](../modules/_fetchblockfeehistory_.md#existingfeehistoryblock)‹50›[]›*
