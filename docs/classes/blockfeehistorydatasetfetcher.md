[ethereum-gas-reference](../README.md) › [Globals](../globals.md) › [BlockFeeHistoryDatasetFetcher](blockfeehistorydatasetfetcher.md)

# Class: BlockFeeHistoryDatasetFetcher

## Hierarchy

* **BlockFeeHistoryDatasetFetcher**

## Index

### Constructors

* [constructor](blockfeehistorydatasetfetcher.md#constructor)

### Properties

* [endBlockNumber](blockfeehistorydatasetfetcher.md#private-endblocknumber)
* [ethQuery](blockfeehistorydatasetfetcher.md#private-ethquery)

### Methods

* [fetchExcludingNextBlock](blockfeehistorydatasetfetcher.md#private-fetchexcludingnextblock)
* [fetchIncludingNextBlock](blockfeehistorydatasetfetcher.md#private-fetchincludingnextblock)
* [forAll](blockfeehistorydatasetfetcher.md#forall)
* [forLatestWithNextBlock](blockfeehistorydatasetfetcher.md#forlatestwithnextblock)
* [forLongRange](blockfeehistorydatasetfetcher.md#forlongrange)
* [forMediumRange](blockfeehistorydatasetfetcher.md#formediumrange)
* [forSmallRange](blockfeehistorydatasetfetcher.md#forsmallrange)
* [forTinyRange](blockfeehistorydatasetfetcher.md#fortinyrange)

## Constructors

###  constructor

\+ **new BlockFeeHistoryDatasetFetcher**(`__namedParameters`: object): *[BlockFeeHistoryDatasetFetcher](blockfeehistorydatasetfetcher.md)*

Defined in fetchGasEstimatesViaEthFeeHistory/BlockFeeHistoryDatasetFetcher.ts:12

**Parameters:**

▪ **__namedParameters**: *object*

Name | Type |
------ | ------ |
`endBlockNumber` | BN‹› |
`ethQuery` | [EthQuery](../globals.md#ethquery) |

**Returns:** *[BlockFeeHistoryDatasetFetcher](blockfeehistorydatasetfetcher.md)*

## Properties

### `Private` endBlockNumber

• **endBlockNumber**: *BN*

Defined in fetchGasEstimatesViaEthFeeHistory/BlockFeeHistoryDatasetFetcher.ts:12

___

### `Private` ethQuery

• **ethQuery**: *[EthQuery](../globals.md#ethquery)*

Defined in fetchGasEstimatesViaEthFeeHistory/BlockFeeHistoryDatasetFetcher.ts:10

## Methods

### `Private` fetchExcludingNextBlock

▸ **fetchExcludingNextBlock**‹**T**›(`args`: object): *Promise‹[ExistingFeeHistoryBlock](../globals.md#existingfeehistoryblock)‹T›[]›*

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

**Returns:** *Promise‹[ExistingFeeHistoryBlock](../globals.md#existingfeehistoryblock)‹T›[]›*

___

### `Private` fetchIncludingNextBlock

▸ **fetchIncludingNextBlock**‹**T**›(`args`: object): *Promise‹[FeeHistoryBlock](../globals.md#feehistoryblock)‹T›[]›*

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

**Returns:** *Promise‹[FeeHistoryBlock](../globals.md#feehistoryblock)‹T›[]›*

___

###  forAll

▸ **forAll**(): *Promise‹object›*

Defined in fetchGasEstimatesViaEthFeeHistory/BlockFeeHistoryDatasetFetcher.ts:25

**Returns:** *Promise‹object›*

___

###  forLatestWithNextBlock

▸ **forLatestWithNextBlock**(): *Promise‹[FeeHistoryBlock](../globals.md#feehistoryblock)‹10 | 95›[]›*

Defined in fetchGasEstimatesViaEthFeeHistory/BlockFeeHistoryDatasetFetcher.ts:74

**Returns:** *Promise‹[FeeHistoryBlock](../globals.md#feehistoryblock)‹10 | 95›[]›*

___

###  forLongRange

▸ **forLongRange**(): *Promise‹[ExistingFeeHistoryBlock](../globals.md#existingfeehistoryblock)‹number›[]›*

Defined in fetchGasEstimatesViaEthFeeHistory/BlockFeeHistoryDatasetFetcher.ts:49

**Returns:** *Promise‹[ExistingFeeHistoryBlock](../globals.md#existingfeehistoryblock)‹number›[]›*

___

###  forMediumRange

▸ **forMediumRange**(): *Promise‹[ExistingFeeHistoryBlock](../globals.md#existingfeehistoryblock)‹10 | 95›[]›*

Defined in fetchGasEstimatesViaEthFeeHistory/BlockFeeHistoryDatasetFetcher.ts:53

**Returns:** *Promise‹[ExistingFeeHistoryBlock](../globals.md#existingfeehistoryblock)‹10 | 95›[]›*

___

###  forSmallRange

▸ **forSmallRange**(): *Promise‹[ExistingFeeHistoryBlock](../globals.md#existingfeehistoryblock)‹10 | 20 | 30›[]›*

Defined in fetchGasEstimatesViaEthFeeHistory/BlockFeeHistoryDatasetFetcher.ts:60

**Returns:** *Promise‹[ExistingFeeHistoryBlock](../globals.md#existingfeehistoryblock)‹10 | 20 | 30›[]›*

___

###  forTinyRange

▸ **forTinyRange**(): *Promise‹[ExistingFeeHistoryBlock](../globals.md#existingfeehistoryblock)‹50›[]›*

Defined in fetchGasEstimatesViaEthFeeHistory/BlockFeeHistoryDatasetFetcher.ts:67

**Returns:** *Promise‹[ExistingFeeHistoryBlock](../globals.md#existingfeehistoryblock)‹50›[]›*
