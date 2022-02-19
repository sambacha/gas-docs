[metamask-controllers-main-src-gas-2](../README.md) › [Globals](../globals.md) › ["fetchBlockFeeHistory"](_fetchblockfeehistory_.md)

# Module: "fetchBlockFeeHistory"

## Index

### Type aliases

* [EthFeeHistoryResponse](_fetchblockfeehistory_.md#ethfeehistoryresponse)
* [EthQuery](_fetchblockfeehistory_.md#ethquery)
* [ExistingFeeHistoryBlock](_fetchblockfeehistory_.md#existingfeehistoryblock)
* [ExtractPercentileFrom](_fetchblockfeehistory_.md#extractpercentilefrom)
* [FeeHistoryBlock](_fetchblockfeehistory_.md#feehistoryblock)
* [NextFeeHistoryBlock](_fetchblockfeehistory_.md#nextfeehistoryblock)
* [RequestChunkSpecifier](_fetchblockfeehistory_.md#requestchunkspecifier)

### Variables

* [MAX_NUMBER_OF_BLOCKS_PER_ETH_FEE_HISTORY_CALL](_fetchblockfeehistory_.md#const-max_number_of_blocks_per_eth_fee_history_call)

### Functions

* [buildExistingFeeHistoryBlock](_fetchblockfeehistory_.md#buildexistingfeehistoryblock)
* [buildNextFeeHistoryBlock](_fetchblockfeehistory_.md#buildnextfeehistoryblock)
* [determineRequestChunkSpecifiers](_fetchblockfeehistory_.md#determinerequestchunkspecifiers)
* [fetchBlockFeeHistory](_fetchblockfeehistory_.md#fetchblockfeehistory)
* [makeRequestForChunk](_fetchblockfeehistory_.md#makerequestforchunk)

## Type aliases

###  EthFeeHistoryResponse

Ƭ **EthFeeHistoryResponse**: *object*

Defined in fetchBlockFeeHistory.ts:31

**`property`** oldestBlock - The id of the oldest block (in hex format) in the range of blocks
requested.

**`property`** baseFeePerGas - Base fee per gas for each block in the range of blocks requested.

**`property`** gasUsedRatio - A number between 0 and 1 that represents the gas used vs. gas limit for
each block in the range of blocks requested.

**`property`** reward - The priority fee at the percentiles requested for each block in the range of
blocks requested.

#### Type declaration:

* **baseFeePerGas**: *string[]*

* **gasUsedRatio**: *number[]*

* **oldestBlock**: *string*

* **reward**? : *string[][]*

___

###  EthQuery

Ƭ **EthQuery**: *any*

Defined in fetchBlockFeeHistory.ts:4

___

###  ExistingFeeHistoryBlock

Ƭ **ExistingFeeHistoryBlock**: *object*

Defined in fetchBlockFeeHistory.ts:51

**`property`** number - The number of the block, as a BN.

**`property`** baseFeePerGas - The base fee per gas for the block in WEI, as a BN.

**`property`** gasUsedRatio - A number between 0 and 1 that represents the ratio between the gas paid
for the block and its set gas limit.

**`property`** priorityFeesByPercentile - The priority fees paid for the transactions in the block
that occurred at particular levels at which those transactions contributed to the overall gas
used for the block, indexed by those percentiles. (See docs for [fetchBlockFeeHistory](_fetchblockfeehistory_.md#fetchblockfeehistory) for more
on how this works.)

#### Type declaration:

* **baseFeePerGas**: *BN*

* **gasUsedRatio**: *number*

* **number**: *BN*

* **priorityFeesByPercentile**: *Record‹Percentile, BN›*

___

###  ExtractPercentileFrom

Ƭ **ExtractPercentileFrom**: *T extends FeeHistoryBlock‹infer P›[] ? P : never*

Defined in fetchBlockFeeHistory.ts:93

___

###  FeeHistoryBlock

Ƭ **FeeHistoryBlock**: *[ExistingFeeHistoryBlock](_fetchblockfeehistory_.md#existingfeehistoryblock)‹Percentile› | [NextFeeHistoryBlock](_fetchblockfeehistory_.md#nextfeehistoryblock)*

Defined in fetchBlockFeeHistory.ts:83

**`property`** number - The number of the block, as a BN.

**`property`** baseFeePerGas - The base fee per gas for the block in WEI, as a BN.

**`property`** gasUsedRatio - A number between 0 and 1 that represents the ratio between the gas paid
for the block and its set gas limit.

**`property`** priorityFeesByPercentile - The priority fees paid for the transactions in the block
that occurred at particular levels at which those transactions contributed to the overall gas
used for the block, indexed by those percentiles. (See docs for [fetchBlockFeeHistory](_fetchblockfeehistory_.md#fetchblockfeehistory) for more
on how this works.)

___

###  NextFeeHistoryBlock

Ƭ **NextFeeHistoryBlock**: *object*

Defined in fetchBlockFeeHistory.ts:65

**`property`** number - The number of the block, as a BN.

**`property`** baseFeePerGas - The estimated base fee per gas for the block in WEI, as a BN.

#### Type declaration:

* **baseFeePerGas**: *BN*

* **number**: *BN*

___

###  RequestChunkSpecifier

Ƭ **RequestChunkSpecifier**: *object*

Defined in fetchBlockFeeHistory.ts:13

**`property`** blockCount - The number of blocks requested.

**`property`** endBlockNumber - The number of the block at the end of the requested range.

#### Type declaration:

* **endBlockNumber**: *BN*

* **numberOfBlocks**: *number*

## Variables

### `Const` MAX_NUMBER_OF_BLOCKS_PER_ETH_FEE_HISTORY_CALL

• **MAX_NUMBER_OF_BLOCKS_PER_ETH_FEE_HISTORY_CALL**: *1024* = 1024

Defined in fetchBlockFeeHistory.ts:97

## Functions

###  buildExistingFeeHistoryBlock

▸ **buildExistingFeeHistoryBlock**‹**Percentile**›(`__namedParameters`: object): *[ExistingFeeHistoryBlock](_fetchblockfeehistory_.md#existingfeehistoryblock)‹Percentile›*

Defined in fetchBlockFeeHistory.ts:198

Builds an ExistingFeeHistoryBlock.

**Type parameters:**

▪ **Percentile**: *number*

**Parameters:**

▪ **__namedParameters**: *object*

Name | Type |
------ | ------ |
`baseFeePerGas` | BN‹› |
`blockIndex` | number |
`gasUsedRatios` | number[] |
`number` | BN‹› |
`percentiles` | ReadonlyArray‹Percentile› |
`priorityFeePercentileGroups` | string[][] |

**Returns:** *[ExistingFeeHistoryBlock](_fetchblockfeehistory_.md#existingfeehistoryblock)‹Percentile›*

The ExistingFeeHistoryBlock.

___

###  buildNextFeeHistoryBlock

▸ **buildNextFeeHistoryBlock**(`__namedParameters`: object): *object*

Defined in fetchBlockFeeHistory.ts:239

Builds a NextFeeHistoryBlock.

**Parameters:**

▪ **__namedParameters**: *object*

Name | Type |
------ | ------ |
`baseFeePerGas` | BN‹› |
`number` | BN‹› |

**Returns:** *object*

The NextFeeHistoryBlock.

* **baseFeePerGas**: *BN‹›*

* **gasUsedRatio**: *null* = null

* **number**: *BN‹›*

* **priorityFeesByPercentile**: *null* = null

___

###  determineRequestChunkSpecifiers

▸ **determineRequestChunkSpecifiers**(`endBlockNumber`: BN, `totalNumberOfBlocks`: number): *[RequestChunkSpecifier](_fetchblockfeehistory_.md#requestchunkspecifier)[]*

Defined in fetchBlockFeeHistory.ts:336

Divides a block range (specified by a range size and the end of the range) into chunks based on
the maximum number of blocks that `eth_feeHistory` can return in a single call.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`endBlockNumber` | BN | The final block in the complete desired block range after all `eth_feeHistory` requests have been made. |
`totalNumberOfBlocks` | number | The total number of desired blocks after all `eth_feeHistory` requests have been made. |

**Returns:** *[RequestChunkSpecifier](_fetchblockfeehistory_.md#requestchunkspecifier)[]*

A set of arguments that can be used to make requests to `eth_feeHistory` in order to
retrieve all of the requested blocks, sorted from oldest block to newest block.

___

###  fetchBlockFeeHistory

▸ **fetchBlockFeeHistory**‹**Percentile**›(`__namedParameters`: object): *Promise‹[FeeHistoryBlock](_fetchblockfeehistory_.md#feehistoryblock)‹Percentile›[]›*

Defined in fetchBlockFeeHistory.ts:132

Uses `eth_feeHistory` (an EIP-1559 feature) to obtain information about gas fees from a range of
blocks that have occurred recently on a network.

To learn more, see these resources:

- <https://infura.io/docs/ethereum#operation/eth_feeHistory>
- <https://github.com/zsfelfoldi/feehistory/blob/main/docs/feeHistory.md>
- <https://github.com/ethereum/go-ethereum/blob/57a3fab8a75eeb9c2f4fab770b73b51b9fe672c5/eth/gasprice/feehistory.go#L180>
- <https://github.com/ethereum/EIPs/blob/master/EIPS/eip-1559.md>
- <https://gas-api.metaswap.codefi.network/testFeeHistory>

**Type parameters:**

▪ **Percentile**: *number*

**Parameters:**

▪ **__namedParameters**: *object*

Name | Type | Default |
------ | ------ | ------ |
`ethQuery` | any | - |
`givenEndBlock` | BN‹› &#124; "latest" | "latest" |
`givenPercentiles` | ReadonlyArray‹Percentile› | [] |
`includeNextBlock` | boolean | false |
`totalNumberOfBlocks` | number | - |

**Returns:** *Promise‹[FeeHistoryBlock](_fetchblockfeehistory_.md#feehistoryblock)‹Percentile›[]›*

The list of blocks and their fee data, sorted from oldest to newest.

___

###  makeRequestForChunk

▸ **makeRequestForChunk**‹**Percentile**›(`__namedParameters`: object): *Promise‹[FeeHistoryBlock](_fetchblockfeehistory_.md#feehistoryblock)‹Percentile›[]›*

Defined in fetchBlockFeeHistory.ts:269

Uses eth_feeHistory to request historical data about a group of blocks (max size 1024).

**Type parameters:**

▪ **Percentile**: *number*

**Parameters:**

▪ **__namedParameters**: *object*

Name | Type |
------ | ------ |
`endBlockNumber` | BN‹› |
`ethQuery` | any |
`includeNextBlock` | boolean |
`numberOfBlocks` | number |
`percentiles` | ReadonlyArray‹Percentile› |

**Returns:** *Promise‹[FeeHistoryBlock](_fetchblockfeehistory_.md#feehistoryblock)‹Percentile›[]›*

A list of block data.
