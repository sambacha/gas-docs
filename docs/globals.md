[ethereum-gas-reference](README.md) › [Globals](globals.md)

# ethereum-gas-reference

## Index

### Enumerations

* [NetworksChainId](enums/networkschainid.md)
* [TransactionStatus](enums/transactionstatus.md)
* [WalletDevice](enums/walletdevice.md)

### Classes

* [BaseController](classes/basecontroller.md)
* [BlockFeeHistoryDatasetFetcher](classes/blockfeehistorydatasetfetcher.md)
* [ControllerMessenger](classes/controllermessenger.md)
* [GasFeeController](classes/gasfeecontroller.md)
* [NetworkController](classes/networkcontroller.md)
* [RestrictedControllerMessenger](classes/restrictedcontrollermessenger.md)
* [TransactionController](classes/transactioncontroller.md)

### Interfaces

* [BaseConfig](interfaces/baseconfig.md)
* [BaseState](interfaces/basestate.md)
* [Block](interfaces/block.md)
* [EtherscanTransactionMeta](interfaces/etherscantransactionmeta.md)
* [FeeMarketEIP1559Values](interfaces/feemarketeip1559values.md)
* [FetchAllOptions](interfaces/fetchalloptions.md)
* [GasPriceValue](interfaces/gaspricevalue.md)
* [MethodData](interfaces/methoddata.md)
* [NetworkConfig](interfaces/networkconfig.md)
* [NetworkProperties](interfaces/networkproperties.md)
* [NetworkState](interfaces/networkstate.md)
* [ProviderConfig](interfaces/providerconfig.md)
* [Result](interfaces/result.md)
* [StatePropertyMetadata](interfaces/statepropertymetadata.md)
* [Transaction](interfaces/transaction.md)
* [TransactionConfig](interfaces/transactionconfig.md)
* [TransactionState](interfaces/transactionstate.md)

### Type aliases

* [ActionConstraint](globals.md#actionconstraint)
* [ActionHandler](globals.md#actionhandler)
* [Eip1559GasFee](globals.md#eip1559gasfee)
* [EstimatedGasFeeTimeBounds](globals.md#estimatedgasfeetimebounds)
* [EthBlock](globals.md#ethblock)
* [EthFeeHistoryResponse](globals.md#ethfeehistoryresponse)
* [EthGasPriceEstimate](globals.md#ethgaspriceestimate)
* [EthGasPriceEstimateType](globals.md#ethgaspriceestimatetype)
* [EthQuery](globals.md#ethquery)
* [EventConstraint](globals.md#eventconstraint)
* [EventSubscriptionMap](globals.md#eventsubscriptionmap)
* [ExistingFeeHistoryBlock](globals.md#existingfeehistoryblock)
* [ExtractActionParameters](globals.md#extractactionparameters)
* [ExtractActionResponse](globals.md#extractactionresponse)
* [ExtractEventHandler](globals.md#extracteventhandler)
* [ExtractEventPayload](globals.md#extracteventpayload)
* [ExtractPercentileFrom](globals.md#extractpercentilefrom)
* [FeeHistoryBlock](globals.md#feehistoryblock)
* [FeeMarketEstimateType](globals.md#feemarketestimatetype)
* [FeeRange](globals.md#feerange)
* [FetchGasFeeEstimateOptions](globals.md#fetchgasfeeestimateoptions)
* [GasEstimateType](globals.md#gasestimatetype)
* [GasFeeEstimates](globals.md#gasfeeestimates)
* [GasFeeMessenger](globals.md#gasfeemessenger)
* [GasFeeState](globals.md#gasfeestate)
* [GasFeeStateChange](globals.md#gasfeestatechange)
* [GasFeeStateEthGasPrice](globals.md#gasfeestateethgasprice)
* [GasFeeStateFeeMarket](globals.md#gasfeestatefeemarket)
* [GasFeeStateLegacy](globals.md#gasfeestatelegacy)
* [GasFeeStateNoEstimates](globals.md#gasfeestatenoestimates)
* [GenericEventHandler](globals.md#genericeventhandler)
* [GetGasFeeState](globals.md#getgasfeestate)
* [Json](globals.md#json)
* [LegacyEstimateType](globals.md#legacyestimatetype)
* [LegacyGasPriceEstimate](globals.md#legacygaspriceestimate)
* [Listener](globals.md#listener)
* [Namespaced](globals.md#namespaced)
* [NarrowToAllowed](globals.md#narrowtoallowed)
* [NarrowToNamespace](globals.md#narrowtonamespace)
* [NetworkType](globals.md#networktype)
* [NextFeeHistoryBlock](globals.md#nextfeehistoryblock)
* [NoEstimateType](globals.md#noestimatetype)
* [Percentile](globals.md#percentile)
* [PriorityLevel](globals.md#prioritylevel)
* [RequestChunkSpecifier](globals.md#requestchunkspecifier)
* [SelectorEventHandler](globals.md#selectoreventhandler)
* [SelectorFunction](globals.md#selectorfunction)
* [StateDeriver](globals.md#statederiver)
* [StateMetadata](globals.md#statemetadata)
* [TransactionMeta](globals.md#transactionmeta)
* [TransactionMetaBase](globals.md#transactionmetabase)
* [unknownString](globals.md#unknownstring)

### Variables

* [CANCEL_RATE](globals.md#const-cancel_rate)
* [ERC1155](globals.md#const-erc1155)
* [ERC1155_INTERFACE_ID](globals.md#const-erc1155_interface_id)
* [ERC1155_METADATA_URI_INTERFACE_ID](globals.md#const-erc1155_metadata_uri_interface_id)
* [ERC1155_TOKEN_RECEIVER_INTERFACE_ID](globals.md#const-erc1155_token_receiver_interface_id)
* [ERC20](globals.md#const-erc20)
* [ERC721](globals.md#const-erc721)
* [ERC721_ENUMERABLE_INTERFACE_ID](globals.md#const-erc721_enumerable_interface_id)
* [ERC721_INTERFACE_ID](globals.md#const-erc721_interface_id)
* [ERC721_METADATA_INTERFACE_ID](globals.md#const-erc721_metadata_interface_id)
* [ETHER_TRANSACTION_HASH](globals.md#const-ether_transaction_hash)
* [ETH_TRANSACTIONS](globals.md#const-eth_transactions)
* [FALL_BACK_VS_CURRENCY](globals.md#const-fall_back_vs_currency)
* [GAS_FEE_API](globals.md#const-gas_fee_api)
* [GWEI](globals.md#const-gwei)
* [HARDFORK](globals.md#const-hardfork)
* [IPFS_DEFAULT_GATEWAY_URL](globals.md#const-ipfs_default_gateway_url)
* [LEGACY_GAS_PRICES_API_URL](globals.md#const-legacy_gas_prices_api_url)
* [LOCALHOST_RPC_URL](globals.md#const-localhost_rpc_url)
* [MAINNET](globals.md#const-mainnet)
* [MAINNET_PROVIDER](globals.md#const-mainnet_provider)
* [MAX_NUMBER_OF_BLOCKS_PER_ETH_FEE_HISTORY_CALL](globals.md#const-max_number_of_blocks_per_eth_fee_history_call)
* [NUMBER_OF_HISTORICAL_BLOCKS_TO_FETCH](globals.md#const-number_of_historical_blocks_to_fetch)
* [NUMBER_OF_RECENT_BLOCKS_TO_FETCH](globals.md#const-number_of_recent_blocks_to_fetch)
* [PRIORITY_LEVELS](globals.md#const-priority_levels)
* [PRIORITY_LEVEL_PERCENTILES](globals.md#const-priority_level_percentiles)
* [PROVIDER](globals.md#const-provider)
* [RINKEBY_CHAIN_ID](globals.md#const-rinkeby_chain_id)
* [RPC](globals.md#const-rpc)
* [SPEED_UP_RATE](globals.md#const-speed_up_rate)
* [TOKEN_TRANSACTIONS](globals.md#const-token_transactions)
* [TOKEN_TRANSACTION_HASH](globals.md#const-token_transaction_hash)
* [TRANSACTIONS_IN_STATE](globals.md#const-transactions_in_state)
* [TRANSACTIONS_IN_STATE_WITH_OUTDATED_GAS_DATA](globals.md#const-transactions_in_state_with_outdated_gas_data)
* [TRANSACTIONS_IN_STATE_WITH_OUTDATED_STATUS](globals.md#const-transactions_in_state_with_outdated_status)
* [TRANSACTIONS_IN_STATE_WITH_OUTDATED_STATUS_AND_GAS_DATA](globals.md#const-transactions_in_state_with_outdated_status_and_gas_data)
* [currentAccountIsEIP1559Compatible](globals.md#const-currentaccountiseip1559compatible)
* [currentNetworkIsEIP1559Compatible](globals.md#const-currentnetworkiseip1559compatible)
* [gasFeeCalculations](globals.md#const-gasfeecalculations)
* [globalAny](globals.md#const-globalany)
* [hexRe](globals.md#const-hexre)
* [hub](globals.md#const-hub)
* [name](globals.md#const-name)
* [provider](globals.md#const-provider)

### Functions

* [BNToHex](globals.md#bntohex)
* [buildExistingFeeHistoryBlock](globals.md#buildexistingfeehistoryblock)
* [buildNextFeeHistoryBlock](globals.md#buildnextfeehistoryblock)
* [calculateBaseFeeRange](globals.md#calculatebasefeerange)
* [calculateBaseFeeTrend](globals.md#calculatebasefeetrend)
* [calculateEstimatesForPriorityLevel](globals.md#calculateestimatesforprioritylevel)
* [calculateGasEstimatesForAllPriorityLevels](globals.md#calculategasestimatesforallprioritylevels)
* [calculateGasEstimatesForPriorityLevel](globals.md#calculategasestimatesforprioritylevel)
* [calculateGasFeeEstimatesForPriorityLevels](globals.md#calculategasfeeestimatesforprioritylevels)
* [calculateNetworkCongestionLevelFrom](globals.md#calculatenetworkcongestionlevelfrom)
* [calculatePriorityFeeRange](globals.md#calculatepriorityfeerange)
* [calculatePriorityFeeTrend](globals.md#calculatepriorityfeetrend)
* [calculateTimeEstimate](globals.md#calculatetimeestimate)
* [convertPriceToDecimal](globals.md#const-convertpricetodecimal)
* [deriveStateFromMetadata](globals.md#derivestatefrommetadata)
* [determineGasFeeCalculations](globals.md#determinegasfeecalculations)
* [determineRequestChunkSpecifiers](globals.md#determinerequestchunkspecifiers)
* [ethTxsMock](globals.md#const-ethtxsmock)
* [fetchBlockFeeHistory](globals.md#fetchblockfeehistory)
* [fetchEthGasPriceEstimate](globals.md#fetchethgaspriceestimate)
* [fetchGasEstimates](globals.md#fetchgasestimates)
* [fetchGasEstimatesViaEthFeeHistory](globals.md#fetchgasestimatesviaethfeehistory)
* [fetchLatestBlock](globals.md#fetchlatestblock)
* [fetchLegacyGasPriceEstimates](globals.md#fetchlegacygaspriceestimates)
* [fetchNetworkCongestionLevel](globals.md#fetchnetworkcongestionlevel)
* [fractionBN](globals.md#fractionbn)
* [fromHex](globals.md#fromhex)
* [getAnonymizedState](globals.md#getanonymizedstate)
* [getBuyURL](globals.md#getbuyurl)
* [getEtherscanApiUrl](globals.md#getetherscanapiurl)
* [getIncreasedPriceFromExisting](globals.md#const-getincreasedpricefromexisting)
* [getIncreasedPriceHex](globals.md#const-getincreasedpricehex)
* [getPersistentState](globals.md#getpersistentstate)
* [gweiDecToWEIBN](globals.md#gweidectoweibn)
* [handleFetch](globals.md#handlefetch)
* [handleTransactionFetch](globals.md#handletransactionfetch)
* [hexToBN](globals.md#hextobn)
* [hexToText](globals.md#hextotext)
* [isEIP1559Transaction](globals.md#const-iseip1559transaction)
* [isFeeMarketEIP1559Values](globals.md#const-isfeemarketeip1559values)
* [isGasPriceValue](globals.md#const-isgaspricevalue)
* [isValidHexAddress](globals.md#isvalidhexaddress)
* [makeClientIdHeader](globals.md#const-makeclientidheader)
* [makeRequestForChunk](globals.md#makerequestforchunk)
* [medianOf](globals.md#medianof)
* [mockFetch](globals.md#mockfetch)
* [mockFetchs](globals.md#mockfetchs)
* [normalizeEnsName](globals.md#normalizeensname)
* [normalizeGWEIDecimalNumbers](globals.md#normalizegweidecimalnumbers)
* [normalizeMessageData](globals.md#normalizemessagedata)
* [normalizeTransaction](globals.md#normalizetransaction)
* [query](globals.md#query)
* [safelyExecute](globals.md#safelyexecute)
* [safelyExecuteWithTimeout](globals.md#safelyexecutewithtimeout)
* [successfulFetch](globals.md#successfulfetch)
* [timeoutFetch](globals.md#timeoutfetch)
* [toChecksumHexAddress](globals.md#tochecksumhexaddress)
* [toHex](globals.md#tohex)
* [tokenTxsMock](globals.md#const-tokentxsmock)
* [txsInStateMock](globals.md#const-txsinstatemock)
* [txsInStateWithOutdatedGasDataMock](globals.md#const-txsinstatewithoutdatedgasdatamock)
* [txsInStateWithOutdatedStatusAndGasDataMock](globals.md#const-txsinstatewithoutdatedstatusandgasdatamock)
* [txsInStateWithOutdatedStatusMock](globals.md#const-txsinstatewithoutdatedstatusmock)
* [validateGasValues](globals.md#const-validategasvalues)
* [validateMinimumIncrease](globals.md#validateminimumincrease)
* [validateSignMessageData](globals.md#validatesignmessagedata)
* [validateTransaction](globals.md#validatetransaction)
* [validateTypedSignMessageDataV1](globals.md#validatetypedsignmessagedatav1)
* [validateTypedSignMessageDataV3](globals.md#validatetypedsignmessagedatav3)
* [weiHexToGweiDec](globals.md#weihextogweidec)

### Object literals

* [ETH_TX_HISTORY_DATA](globals.md#const-eth_tx_history_data)
* [ETH_TX_HISTORY_DATA_FROM_BLOCK](globals.md#const-eth_tx_history_data_from_block)
* [ETH_TX_HISTORY_DATA_ROPSTEN_NO_TRANSACTIONS_FOUND](globals.md#const-eth_tx_history_data_ropsten_no_transactions_found)
* [GAS_ESTIMATE_TYPES](globals.md#const-gas_estimate_types)
* [MOCK_CUSTOM_NETWORK](globals.md#const-mock_custom_network)
* [MOCK_FETCH_TX_HISTORY_DATA_ERROR](globals.md#const-mock_fetch_tx_history_data_error)
* [MOCK_FETCH_TX_HISTORY_DATA_OK](globals.md#const-mock_fetch_tx_history_data_ok)
* [MOCK_MAINNET_NETWORK](globals.md#const-mock_mainnet_network)
* [MOCK_NETWORK](globals.md#const-mock_network)
* [MOCK_NETWORK_CUSTOM](globals.md#const-mock_network_custom)
* [MOCK_NETWORK_WITHOUT_CHAIN_ID](globals.md#const-mock_network_without_chain_id)
* [MOCK_PRFERENCES](globals.md#const-mock_prferences)
* [NORMALIZERS](globals.md#const-normalizers)
* [SETTINGS_BY_PRIORITY_LEVEL](globals.md#const-settings_by_priority_level)
* [TOKEN_TX_HISTORY_DATA](globals.md#const-token_tx_history_data)
* [TOKEN_TX_HISTORY_DATA_FROM_BLOCK](globals.md#const-token_tx_history_data_from_block)
* [defaultState](globals.md#const-defaultstate)
* [metadata](globals.md#const-metadata)
* [mockFlags](globals.md#const-mockflags)

## Type aliases

###  ActionConstraint

Ƭ **ActionConstraint**: *object*

Defined in ControllerMessenger.ts:36

#### Type declaration:

* **handler**(): *function*

  * (...`args`: any): *unknown*

* **type**: *string*

___

###  ActionHandler

Ƭ **ActionHandler**: *function*

Defined in ControllerMessenger.ts:1

#### Type declaration:

▸ (...`args`: [ExtractActionParameters](globals.md#extractactionparameters)‹Action, ActionType›): *[ExtractActionResponse](globals.md#extractactionresponse)‹Action, ActionType›*

**Parameters:**

Name | Type |
------ | ------ |
`...args` | [ExtractActionParameters](globals.md#extractactionparameters)‹Action, ActionType› |

___

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

* **upperTimeBound**: *number | [unknownString](globals.md#unknownstring)*

___

###  EthBlock

Ƭ **EthBlock**: *object*

Defined in fetchGasEstimatesViaEthFeeHistory/types.ts:3

#### Type declaration:

* **baseFeePerGas**: *BN*

* **number**: *BN*

___

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

###  EthQuery

Ƭ **EthQuery**: *any*

Defined in fetchGasEstimatesViaEthFeeHistory/types.ts:8

Defined in fetchBlockFeeHistory.ts:4

Defined in getGasEstimatesViaEthFeeHistory.ts:9

___

###  EventConstraint

Ƭ **EventConstraint**: *object*

Defined in ControllerMessenger.ts:40

#### Type declaration:

* **payload**: *unknown[]*

* **type**: *string*

___

###  EventSubscriptionMap

Ƭ **EventSubscriptionMap**: *Map‹[GenericEventHandler](globals.md#genericeventhandler) | [SelectorEventHandler](globals.md#selectoreventhandler)‹unknown›, [SelectorFunction](globals.md#selectorfunction)‹any, unknown› | undefined›*

Defined in ControllerMessenger.ts:42

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
used for the block, indexed by those percentiles. (See docs for [fetchBlockFeeHistory](globals.md#fetchblockfeehistory) for more
on how this works.)

#### Type declaration:

* **baseFeePerGas**: *BN*

* **gasUsedRatio**: *number*

* **number**: *BN*

* **priorityFeesByPercentile**: *Record‹Percentile, BN›*

___

###  ExtractActionParameters

Ƭ **ExtractActionParameters**: *Action extends object ? H : never*

Defined in ControllerMessenger.ts:4

___

###  ExtractActionResponse

Ƭ **ExtractActionResponse**: *Action extends object ? H : never*

Defined in ControllerMessenger.ts:10

___

###  ExtractEventHandler

Ƭ **ExtractEventHandler**: *Event extends object ? P extends unknown[] ? function : never : never*

Defined in ControllerMessenger.ts:17

___

###  ExtractEventPayload

Ƭ **ExtractEventPayload**: *Event extends object ? P : never*

Defined in ControllerMessenger.ts:22

___

###  ExtractPercentileFrom

Ƭ **ExtractPercentileFrom**: *T extends FeeHistoryBlock‹infer P›[] ? P : never*

Defined in fetchBlockFeeHistory.ts:93

___

###  FeeHistoryBlock

Ƭ **FeeHistoryBlock**: *[ExistingFeeHistoryBlock](globals.md#existingfeehistoryblock)‹Percentile› | [NextFeeHistoryBlock](globals.md#nextfeehistoryblock)*

Defined in fetchBlockFeeHistory.ts:83

**`property`** number - The number of the block, as a BN.

**`property`** baseFeePerGas - The base fee per gas for the block in WEI, as a BN.

**`property`** gasUsedRatio - A number between 0 and 1 that represents the ratio between the gas paid
for the block and its set gas limit.

**`property`** priorityFeesByPercentile - The priority fees paid for the transactions in the block
that occurred at particular levels at which those transactions contributed to the overall gas
used for the block, indexed by those percentiles. (See docs for [fetchBlockFeeHistory](globals.md#fetchblockfeehistory) for more
on how this works.)

___

###  FeeMarketEstimateType

Ƭ **FeeMarketEstimateType**: *"fee-market"*

Defined in GasFeeController.ts:26

___

###  FeeRange

Ƭ **FeeRange**: *[string, string]*

Defined in fetchGasEstimatesViaEthFeeHistory/types.ts:14

___

###  FetchGasFeeEstimateOptions

Ƭ **FetchGasFeeEstimateOptions**: *object*

Defined in GasFeeController.ts:165

#### Type declaration:

* **shouldUpdateState**? : *boolean*

___

###  GasEstimateType

Ƭ **GasEstimateType**: *[FeeMarketEstimateType](globals.md#feemarketestimatetype) | [EthGasPriceEstimateType](globals.md#ethgaspriceestimatetype) | [LegacyEstimateType](globals.md#legacyestimatetype) | [NoEstimateType](globals.md#noestimatetype)*

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

* **high**: *[Eip1559GasFee](globals.md#eip1559gasfee)*

* **historicalBaseFeeRange**: *[string, string]*

* **historicalPriorityFeeRange**: *[string, string]*

* **latestPriorityFeeRange**: *[string, string]*

* **low**: *[Eip1559GasFee](globals.md#eip1559gasfee)*

* **medium**: *[Eip1559GasFee](globals.md#eip1559gasfee)*

* **networkCongestion**: *number*

* **priorityFeeTrend**: *"up" | "down" | "level"*

___

###  GasFeeMessenger

Ƭ **GasFeeMessenger**: *[RestrictedControllerMessenger](classes/restrictedcontrollermessenger.md)‹typeof name, [GetGasFeeState](globals.md#getgasfeestate), [GasFeeStateChange](globals.md#gasfeestatechange), never, never›*

Defined in GasFeeController.ts:194

___

###  GasFeeState

Ƭ **GasFeeState**: *[GasFeeStateEthGasPrice](globals.md#gasfeestateethgasprice) | [GasFeeStateFeeMarket](globals.md#gasfeestatefeemarket) | [GasFeeStateLegacy](globals.md#gasfeestatelegacy) | [GasFeeStateNoEstimates](globals.md#gasfeestatenoestimates)*

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

* **gasEstimateType**: *[EthGasPriceEstimateType](globals.md#ethgaspriceestimatetype)*

* **gasFeeEstimates**: *[EthGasPriceEstimate](globals.md#ethgaspriceestimate)*

___

###  GasFeeStateFeeMarket

Ƭ **GasFeeStateFeeMarket**: *object*

Defined in GasFeeController.ts:147

#### Type declaration:

* **estimatedGasFeeTimeBounds**: *[EstimatedGasFeeTimeBounds](globals.md#estimatedgasfeetimebounds) | Record‹string, never›*

* **gasEstimateType**: *[FeeMarketEstimateType](globals.md#feemarketestimatetype)*

* **gasFeeEstimates**: *[GasFeeEstimates](globals.md#gasfeeestimates)*

___

###  GasFeeStateLegacy

Ƭ **GasFeeStateLegacy**: *object*

Defined in GasFeeController.ts:153

#### Type declaration:

* **estimatedGasFeeTimeBounds**: *Record‹string, never›*

* **gasEstimateType**: *[LegacyEstimateType](globals.md#legacyestimatetype)*

* **gasFeeEstimates**: *[LegacyGasPriceEstimate](globals.md#legacygaspriceestimate)*

___

###  GasFeeStateNoEstimates

Ƭ **GasFeeStateNoEstimates**: *object*

Defined in GasFeeController.ts:159

#### Type declaration:

* **estimatedGasFeeTimeBounds**: *Record‹string, never›*

* **gasEstimateType**: *[NoEstimateType](globals.md#noestimatetype)*

* **gasFeeEstimates**: *Record‹string, never›*

___

###  GenericEventHandler

Ƭ **GenericEventHandler**: *function*

Defined in ControllerMessenger.ts:26

#### Type declaration:

▸ (...`args`: unknown[]): *void*

**Parameters:**

Name | Type |
------ | ------ |
`...args` | unknown[] |

___

###  GetGasFeeState

Ƭ **GetGasFeeState**: *object*

Defined in GasFeeController.ts:189

#### Type declaration:

* **type**: **

___

###  Json

Ƭ **Json**: *null | boolean | number | string | [Json](globals.md#json)[] | object*

Defined in BaseControllerV2.ts:64

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

###  Listener

Ƭ **Listener**: *function*

Defined in BaseController.ts:4

Defined in BaseControllerV2.ts:25

State change callbacks
A state change listener.

This function will get called for each state change, and is given a copy of
the new state along with a set of patches describing the changes since the
last update.

**`param`** The new controller state.

**`param`** A list of patches describing any changes (see here for more
information: https://immerjs.github.io/immer/docs/patches)

#### Type declaration:

▸ (`state`: T, `patches`: Patch[]): *void*

**Parameters:**

Name | Type |
------ | ------ |
`state` | T |
`patches` | Patch[] |

___

###  Namespaced

Ƭ **Namespaced**: *T extends  ?  : *

Defined in ControllerMessenger.ts:55

A namespaced string

This type verifies that the string T is prefixed by the string Name followed by a colon.

___

###  NarrowToAllowed

Ƭ **NarrowToAllowed**: *T extends object ? T : never*

Defined in ControllerMessenger.ts:65

___

###  NarrowToNamespace

Ƭ **NarrowToNamespace**: *T extends object ?  : *

Defined in ControllerMessenger.ts:59

___

###  NetworkType

Ƭ **NetworkType**: *"kovan" | "localhost" | "mainnet" | "rinkeby" | "goerli" | "ropsten" | "rpc" | "optimism" | "optimismTest"*

Defined in NetworkController.ts:12

Human-readable network name

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

###  NoEstimateType

Ƭ **NoEstimateType**: *"none"*

Defined in GasFeeController.ts:38

___

###  Percentile

Ƭ **Percentile**: *typeof PRIORITY_LEVEL_PERCENTILES[number]*

Defined in fetchGasEstimatesViaEthFeeHistory/calculateGasFeeEstimatesForPriorityLevels.ts:9

Defined in getGasEstimatesViaEthFeeHistory.ts:11

___

###  PriorityLevel

Ƭ **PriorityLevel**: *typeof PRIORITY_LEVELS[number]*

Defined in fetchGasEstimatesViaEthFeeHistory/calculateGasFeeEstimatesForPriorityLevels.ts:8

Defined in getGasEstimatesViaEthFeeHistory.ts:10

___

###  RequestChunkSpecifier

Ƭ **RequestChunkSpecifier**: *object*

Defined in fetchBlockFeeHistory.ts:13

**`property`** blockCount - The number of blocks requested.

**`property`** endBlockNumber - The number of the block at the end of the requested range.

#### Type declaration:

* **endBlockNumber**: *BN*

* **numberOfBlocks**: *number*

___

###  SelectorEventHandler

Ƭ **SelectorEventHandler**: *function*

Defined in ControllerMessenger.ts:31

#### Type declaration:

▸ (`newValue`: SelectorReturnValue, `previousValue`: SelectorReturnValue | undefined): *void*

**Parameters:**

Name | Type |
------ | ------ |
`newValue` | SelectorReturnValue |
`previousValue` | SelectorReturnValue &#124; undefined |

___

###  SelectorFunction

Ƭ **SelectorFunction**: *function*

Defined in ControllerMessenger.ts:28

#### Type declaration:

▸ (...`args`: Args): *ReturnValue*

**Parameters:**

Name | Type |
------ | ------ |
`...args` | Args |

___

###  StateDeriver

Ƭ **StateDeriver**: *function*

Defined in BaseControllerV2.ts:36

An function to derive state.

This function will accept one piece of the controller state (one property),
and will return some derivation of that state.

**`param`** A piece of controller state.

**`returns`** Something derived from controller state.

#### Type declaration:

▸ (`value`: T): *[Json](globals.md#json)*

**Parameters:**

Name | Type |
------ | ------ |
`value` | T |

___

###  StateMetadata

Ƭ **StateMetadata**: *object*

Defined in BaseControllerV2.ts:44

State metadata.

This metadata describes which parts of state should be persisted, and how to
get an anonymized representation of the state.

#### Type declaration:

___

###  TransactionMeta

Ƭ **TransactionMeta**: *object & [TransactionMetaBase](globals.md#transactionmetabase) | object & [TransactionMetaBase](globals.md#transactionmetabase)*

Defined in Tx.ts:164

**`property`** error - Synthesized error information for failed transactions

**`property`** id - Generated UUID associated with this transaction

**`property`** networkID - Network code as per EIP-155 for this transaction

**`property`** origin - Origin this transaction was sent from

**`property`** deviceConfirmedOn - string to indicate what device the transaction was confirmed

**`property`** rawTransaction - Hex representation of the underlying transaction

**`property`** status - String status of this transaction

**`property`** time - Timestamp associated with this transaction

**`property`** toSmartContract - Whether transaction recipient is a smart contract

**`property`** transaction - Underlying Transaction object

**`property`** transactionHash - Hash of a successful transaction

**`property`** blockNumber - Number of the block where the transaction has been included

___

###  TransactionMetaBase

Ƭ **TransactionMetaBase**: *object*

Defined in Tx.ts:126

#### Type declaration:

* **blockNumber**? : *string*

* **chainId**? : *string*

* **deviceConfirmedOn**? : *[WalletDevice](enums/walletdevice.md)*

* **id**: *string*

* **isTransfer**? : *boolean*

* **networkID**? : *string*

* **origin**? : *string*

* **rawTransaction**? : *string*

* **time**: *number*

* **toSmartContract**? : *boolean*

* **transaction**: *[Transaction](interfaces/transaction.md)*

* **transactionHash**? : *string*

* **transferInformation**(): *object*

  * **contractAddress**: *string*

  * **decimals**: *number*

  * **symbol**: *string*

* **verifiedOnBlockchain**? : *boolean*

___

###  unknownString

Ƭ **unknownString**: *"unknown"*

Defined in GasFeeController.ts:22

## Variables

### `Const` CANCEL_RATE

• **CANCEL_RATE**: *1.5* = 1.5

Defined in Tx.ts:255

Multiplier used to determine a transaction's increased gas fee during cancellation

___

### `Const` ERC1155

• **ERC1155**: *"ERC1155"* = "ERC1155"

Defined in constants.ts:11

___

### `Const` ERC1155_INTERFACE_ID

• **ERC1155_INTERFACE_ID**: *"0xd9b67a26"* = "0xd9b67a26"

Defined in constants.ts:18

___

### `Const` ERC1155_METADATA_URI_INTERFACE_ID

• **ERC1155_METADATA_URI_INTERFACE_ID**: *"0x0e89341c"* = "0x0e89341c"

Defined in constants.ts:19

___

### `Const` ERC1155_TOKEN_RECEIVER_INTERFACE_ID

• **ERC1155_TOKEN_RECEIVER_INTERFACE_ID**: *"0x4e2312e0"* = "0x4e2312e0"

Defined in constants.ts:20

___

### `Const` ERC20

• **ERC20**: *"ERC20"* = "ERC20"

Defined in constants.ts:12

___

### `Const` ERC721

• **ERC721**: *"ERC721"* = "ERC721"

Defined in constants.ts:10

___

### `Const` ERC721_ENUMERABLE_INTERFACE_ID

• **ERC721_ENUMERABLE_INTERFACE_ID**: *"0x780e9d63"* = "0x780e9d63"

Defined in constants.ts:17

___

### `Const` ERC721_INTERFACE_ID

• **ERC721_INTERFACE_ID**: *"0x80ac58cd"* = "0x80ac58cd"

Defined in constants.ts:15

___

### `Const` ERC721_METADATA_INTERFACE_ID

• **ERC721_METADATA_INTERFACE_ID**: *"0x5b5e139f"* = "0x5b5e139f"

Defined in constants.ts:16

___

### `Const` ETHER_TRANSACTION_HASH

• **ETHER_TRANSACTION_HASH**: *"0xa9d17df83756011ea63e1f0ca50a6627df7cac9806809e36680fcf4e88cb9dae"* = "0xa9d17df83756011ea63e1f0ca50a6627df7cac9806809e36680fcf4e88cb9dae"

Defined in transaction/TransactionController.test.ts:179

___

### `Const` ETH_TRANSACTIONS

• **ETH_TRANSACTIONS**: *(object | object)[]* = ethTxsMock(ETHER_TRANSACTION_HASH)

Defined in transaction/TransactionController.test.ts:182

___

### `Const` FALL_BACK_VS_CURRENCY

• **FALL_BACK_VS_CURRENCY**: *"ETH"* = "ETH"

Defined in constants.ts:3

___

### `Const` GAS_FEE_API

• **GAS_FEE_API**: *"https://mock-gas-server.herokuapp.com/"* = "https://mock-gas-server.herokuapp.com/"

Defined in GasFeeController.ts:19

___

### `Const` GWEI

• **GWEI**: *"gwei"* = "gwei"

Defined in constants.ts:23

___

### `Const` HARDFORK

• **HARDFORK**: *"london"* = "london"

Defined in Tx.ts:31

___

### `Const` IPFS_DEFAULT_GATEWAY_URL

• **IPFS_DEFAULT_GATEWAY_URL**: *"https://cloudflare-ipfs.com/ipfs/"* = "https://cloudflare-ipfs.com/ipfs/"

Defined in constants.ts:4

___

### `Const` LEGACY_GAS_PRICES_API_URL

• **LEGACY_GAS_PRICES_API_URL**: *"https://api.metaswap.codefi.network/gasPrices"* = `https://api.metaswap.codefi.network/gasPrices`

Defined in GasFeeController.ts:20

___

### `Const` LOCALHOST_RPC_URL

• **LOCALHOST_RPC_URL**: *"http://localhost:8545"* = "http://localhost:8545"

Defined in NetworkController.ts:88

___

### `Const` MAINNET

• **MAINNET**: *"mainnet"* = "mainnet"

Defined in constants.ts:1

___

### `Const` MAINNET_PROVIDER

• **MAINNET_PROVIDER**: *any* = new HttpProvider(
  'https://mainnet.infura.io/v3/341eacb578dd44a1a049cbc5f6fd4035',
)

Defined in transaction/TransactionController.test.ts:115

___

### `Const` MAX_NUMBER_OF_BLOCKS_PER_ETH_FEE_HISTORY_CALL

• **MAX_NUMBER_OF_BLOCKS_PER_ETH_FEE_HISTORY_CALL**: *1024* = 1024

Defined in fetchBlockFeeHistory.ts:97

___

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

Defined in fetchGasEstimatesViaEthFeeHistory/calculateGasFeeEstimatesForPriorityLevels.ts:11

Defined in getGasEstimatesViaEthFeeHistory.ts:15

___

### `Const` PRIORITY_LEVEL_PERCENTILES

• **PRIORITY_LEVEL_PERCENTILES**: *[10, 20, 30]* = [10, 20, 30] as const

Defined in fetchGasEstimatesViaEthFeeHistory/calculateGasFeeEstimatesForPriorityLevels.ts:12

Defined in getGasEstimatesViaEthFeeHistory.ts:16

___

### `Const` PROVIDER

• **PROVIDER**: *any* = new HttpProvider(
  'https://ropsten.infura.io/v3/341eacb578dd44a1a049cbc5f6fd4035',
)

Defined in transaction/TransactionController.test.ts:112

___

### `Const` RINKEBY_CHAIN_ID

• **RINKEBY_CHAIN_ID**: *"4"* = "4"

Defined in constants.ts:7

___

### `Const` RPC

• **RPC**: *"rpc"* = "rpc"

Defined in constants.ts:2

___

### `Const` SPEED_UP_RATE

• **SPEED_UP_RATE**: *1.1* = 1.1

Defined in Tx.ts:260

Multiplier used to determine a transaction's increased gas fee during speed up

___

### `Const` TOKEN_TRANSACTIONS

• **TOKEN_TRANSACTIONS**: *object[]* = tokenTxsMock(TOKEN_TRANSACTION_HASH)

Defined in transaction/TransactionController.test.ts:184

___

### `Const` TOKEN_TRANSACTION_HASH

• **TOKEN_TRANSACTION_HASH**: *"0x01d1cebeab9da8d887b36000c25fa175737e150f193ea37d5bb66347d834e999"* = "0x01d1cebeab9da8d887b36000c25fa175737e150f193ea37d5bb66347d834e999"

Defined in transaction/TransactionController.test.ts:177

___

### `Const` TRANSACTIONS_IN_STATE

• **TRANSACTIONS_IN_STATE**: *[TransactionMeta](globals.md#transactionmeta)[]* = txsInStateMock(
  ETHER_TRANSACTION_HASH,
  TOKEN_TRANSACTION_HASH,
)

Defined in transaction/TransactionController.test.ts:186

___

### `Const` TRANSACTIONS_IN_STATE_WITH_OUTDATED_GAS_DATA

• **TRANSACTIONS_IN_STATE_WITH_OUTDATED_GAS_DATA**: *[TransactionMeta](globals.md#transactionmeta)[]* = txsInStateWithOutdatedGasDataMock(
    ETHER_TRANSACTION_HASH,
    TOKEN_TRANSACTION_HASH,
  )

Defined in transaction/TransactionController.test.ts:197

___

### `Const` TRANSACTIONS_IN_STATE_WITH_OUTDATED_STATUS

• **TRANSACTIONS_IN_STATE_WITH_OUTDATED_STATUS**: *[TransactionMeta](globals.md#transactionmeta)[]* = txsInStateWithOutdatedStatusMock(
    ETHER_TRANSACTION_HASH,
    TOKEN_TRANSACTION_HASH,
  )

Defined in transaction/TransactionController.test.ts:191

___

### `Const` TRANSACTIONS_IN_STATE_WITH_OUTDATED_STATUS_AND_GAS_DATA

• **TRANSACTIONS_IN_STATE_WITH_OUTDATED_STATUS_AND_GAS_DATA**: *[TransactionMeta](globals.md#transactionmeta)[]* = txsInStateWithOutdatedStatusAndGasDataMock(
    ETHER_TRANSACTION_HASH,
    TOKEN_TRANSACTION_HASH,
  )

Defined in transaction/TransactionController.test.ts:203

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

• **gasFeeCalculations**: *[GasFeeState](globals.md#gasfeestate)* = await determineGasFeeCalculations({
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

### `Const` globalAny

• **globalAny**: *any* = global

Defined in transaction/TransactionController.test.ts:22

___

### `Const` hexRe

• **hexRe**: *RegExp‹›* = /^[0-9A-Fa-f]+$/gu

Defined in util.ts:28

___

### `Const` hub

• **hub**: *EventEmitter‹›* = new EventEmitter()

Defined in Tx.ts:36

EventEmitter instance used to listen to specific transactional events

___

### `Const` name

• **name**: *"GasFeeController"* = "GasFeeController"

Defined in Tx.ts:41

Defined in GasFeeController.ts:182

Name of this controller used during composition

___

### `Const` provider

• **provider**: *any* = getProvider()

Defined in GasFeeController.ts:309

## Functions

###  BNToHex

▸ **BNToHex**(`inputBn`: any): *string*

Defined in util.ts:51

Converts a BN object to a hex string with a '0x' prefix.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`inputBn` | any | BN instance to convert to a hex string. |

**Returns:** *string*

A '0x'-prefixed hex string.

___

###  buildExistingFeeHistoryBlock

▸ **buildExistingFeeHistoryBlock**‹**Percentile**›(`__namedParameters`: object): *[ExistingFeeHistoryBlock](globals.md#existingfeehistoryblock)‹Percentile›*

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

**Returns:** *[ExistingFeeHistoryBlock](globals.md#existingfeehistoryblock)‹Percentile›*

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

###  calculateBaseFeeRange

▸ **calculateBaseFeeRange**‹**Percentile**›(`blocks`: [FeeHistoryBlock](globals.md#feehistoryblock)‹Percentile›[]): *[FeeRange](globals.md#feerange)*

Defined in fetchGasEstimatesViaEthFeeHistory/calculateBaseFeeRange.ts:12

Calculates reasonable minimum and maximum values for base fees over the last 200 blocks.

**Type parameters:**

▪ **Percentile**: *number*

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`blocks` | [FeeHistoryBlock](globals.md#feehistoryblock)‹Percentile›[] | A set of blocks obtained via [BlockFeeHistoryDatasetFetcher](classes/blockfeehistorydatasetfetcher.md). |

**Returns:** *[FeeRange](globals.md#feerange)*

The ranges.

___

###  calculateBaseFeeTrend

▸ **calculateBaseFeeTrend**‹**Percentile**›(`blocks`: [FeeHistoryBlock](globals.md#feehistoryblock)‹Percentile›[]): *"up" | "down" | "level"*

Defined in fetchGasEstimatesViaEthFeeHistory/calculateBaseFeeTrend.ts:10

Given a collection of blocks, returns an indicator of whether the base fee is moving up, down, or
holding steady, based on comparing the last base fee in the collection to the first.

**Type parameters:**

▪ **Percentile**: *number*

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`blocks` | [FeeHistoryBlock](globals.md#feehistoryblock)‹Percentile›[] | A set of blocks obtained via [BlockFeeHistoryDatasetFetcher](classes/blockfeehistorydatasetfetcher.md). |

**Returns:** *"up" | "down" | "level"*

The indicator ("up", "down", or "level").

___

###  calculateEstimatesForPriorityLevel

▸ **calculateEstimatesForPriorityLevel**(`priorityLevel`: [PriorityLevel](globals.md#prioritylevel), `blocks`: [ExistingFeeHistoryBlock](globals.md#existingfeehistoryblock)‹Percentile›[]): *[Eip1559GasFee](globals.md#eip1559gasfee)*

Defined in fetchGasEstimatesViaEthFeeHistory/calculateGasFeeEstimatesForPriorityLevels.ts:55

Calculates a set of estimates assigned to a particular priority level based on the data returned
by `eth_feeHistory`.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`priorityLevel` | [PriorityLevel](globals.md#prioritylevel) | The level of fees that dictates how soon a transaction may go through ("low", "medium", or "high"). |
`blocks` | [ExistingFeeHistoryBlock](globals.md#existingfeehistoryblock)‹Percentile›[] | A set of blocks as obtained from [fetchBlockFeeHistory](globals.md#fetchblockfeehistory). |

**Returns:** *[Eip1559GasFee](globals.md#eip1559gasfee)*

The estimates.

___

###  calculateGasEstimatesForAllPriorityLevels

▸ **calculateGasEstimatesForAllPriorityLevels**(`blocks`: [Block](interfaces/block.md)‹Percentile›[]): *Pick‹[GasFeeEstimates](globals.md#gasfeeestimates), [PriorityLevel](globals.md#prioritylevel)›*

Defined in getGasEstimatesViaEthFeeHistory.ts:115

Calculates a set of estimates suitable for different priority levels based on the data returned
by `eth_feeHistory`.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`blocks` | [Block](interfaces/block.md)‹Percentile›[] | A set of blocks as obtained from [fetchBlockFeeHistory](globals.md#fetchblockfeehistory). |

**Returns:** *Pick‹[GasFeeEstimates](globals.md#gasfeeestimates), [PriorityLevel](globals.md#prioritylevel)›*

The estimates.

___

###  calculateGasEstimatesForPriorityLevel

▸ **calculateGasEstimatesForPriorityLevel**(`priorityLevel`: [PriorityLevel](globals.md#prioritylevel), `blocks`: [Block](interfaces/block.md)‹Percentile›[]): *[Eip1559GasFee](globals.md#eip1559gasfee)*

Defined in getGasEstimatesViaEthFeeHistory.ts:73

Calculates a set of estimates assigned to a particular priority level based on the data returned
by `eth_feeHistory`.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`priorityLevel` | [PriorityLevel](globals.md#prioritylevel) | The level of fees that dictates how soon a transaction may go through ("low", "medium", or "high"). |
`blocks` | [Block](interfaces/block.md)‹Percentile›[] | A set of blocks as obtained from [fetchBlockFeeHistory](globals.md#fetchblockfeehistory). |

**Returns:** *[Eip1559GasFee](globals.md#eip1559gasfee)*

The estimates.

___

###  calculateGasFeeEstimatesForPriorityLevels

▸ **calculateGasFeeEstimatesForPriorityLevels**(`blocks`: [ExistingFeeHistoryBlock](globals.md#existingfeehistoryblock)‹Percentile›[]): *Pick‹[GasFeeEstimates](globals.md#gasfeeestimates), [PriorityLevel](globals.md#prioritylevel)›*

Defined in fetchGasEstimatesViaEthFeeHistory/calculateGasFeeEstimatesForPriorityLevels.ts:97

Calculates a set of estimates suitable for different priority levels based on the data returned
by `eth_feeHistory`.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`blocks` | [ExistingFeeHistoryBlock](globals.md#existingfeehistoryblock)‹Percentile›[] | A set of blocks populated with data for priority fee percentiles 10, 20, and 30, obtained via [BlockFeeHistoryDatasetFetcher](classes/blockfeehistorydatasetfetcher.md). |

**Returns:** *Pick‹[GasFeeEstimates](globals.md#gasfeeestimates), [PriorityLevel](globals.md#prioritylevel)›*

The estimates.

___

###  calculateNetworkCongestionLevelFrom

▸ **calculateNetworkCongestionLevelFrom**(`blocks`: [Block](interfaces/block.md)‹Percentile›[]): *Promise‹number›*

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
`blocks` | [Block](interfaces/block.md)‹Percentile›[] | A set of blocks as obtained from [fetchBlockFeeHistory](globals.md#fetchblockfeehistory). |

**Returns:** *Promise‹number›*

A promise of a number between 0 and 1.

___

###  calculatePriorityFeeRange

▸ **calculatePriorityFeeRange**(`blocks`: [ExistingFeeHistoryBlock](globals.md#existingfeehistoryblock)‹10 | 95›[]): *[FeeRange](globals.md#feerange)*

Defined in fetchGasEstimatesViaEthFeeHistory/calculatePriorityFeeRange.ts:16

Calculates reasonable minimum and maximum values for priority fees over the last 200 blocks.
Although some priority fees may be 0, these are discarded as they are not useful for suggestion
purposes.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`blocks` | [ExistingFeeHistoryBlock](globals.md#existingfeehistoryblock)‹10 &#124; 95›[] | A set of blocks populated with data for priority fee percentiles 10 and 95, obtained via [BlockFeeHistoryDatasetFetcher](classes/blockfeehistorydatasetfetcher.md). |

**Returns:** *[FeeRange](globals.md#feerange)*

The range.

___

###  calculatePriorityFeeTrend

▸ **calculatePriorityFeeTrend**(`blocks`: [ExistingFeeHistoryBlock](globals.md#existingfeehistoryblock)‹50›[]): *"up" | "down" | "level"*

Defined in fetchGasEstimatesViaEthFeeHistory/calculatePriorityFeeTrend.ts:11

Given a collection of blocks, returns an indicator of whether the base fee is moving up, down, or
holding steady, based on comparing the last base fee in the collection to the first.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`blocks` | [ExistingFeeHistoryBlock](globals.md#existingfeehistoryblock)‹50›[] | A set of blocks obtained via [BlockFeeHistoryDatasetFetcher](classes/blockfeehistorydatasetfetcher.md). |

**Returns:** *"up" | "down" | "level"*

The indicator ("up", "down", or "level").

___

###  calculateTimeEstimate

▸ **calculateTimeEstimate**(`maxPriorityFeePerGas`: string, `maxFeePerGas`: string, `gasFeeEstimates`: [GasFeeEstimates](globals.md#gasfeeestimates)): *[EstimatedGasFeeTimeBounds](globals.md#estimatedgasfeetimebounds)*

Defined in gas-util.ts:130

Estimate the time it will take for a transaction to be confirmed.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`maxPriorityFeePerGas` | string | The max priority fee per gas. |
`maxFeePerGas` | string | The max fee per gas. |
`gasFeeEstimates` | [GasFeeEstimates](globals.md#gasfeeestimates) | The gas fee estimates. |

**Returns:** *[EstimatedGasFeeTimeBounds](globals.md#estimatedgasfeetimebounds)*

The estimated lower and upper bounds for when this transaction will be confirmed.

___

### `Const` convertPriceToDecimal

▸ **convertPriceToDecimal**(`value`: string | undefined): *number*

Defined in util.ts:703

**Parameters:**

Name | Type |
------ | ------ |
`value` | string &#124; undefined |

**Returns:** *number*

___

###  deriveStateFromMetadata

▸ **deriveStateFromMetadata**‹**S**›(`state`: S, `metadata`: [StateMetadata](globals.md#statemetadata)‹S›, `metadataProperty`: "anonymous" | "persist"): *Record‹string, [Json](globals.md#json)›*

Defined in BaseControllerV2.ts:232

Use the metadata to derive state according to the given metadata property.

**Type parameters:**

▪ **S**: *Record‹string, [Json](globals.md#json)›*

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`state` | S | The full controller state. |
`metadata` | [StateMetadata](globals.md#statemetadata)‹S› | The controller metadata. |
`metadataProperty` | "anonymous" &#124; "persist" | The metadata property to use to derive state. |

**Returns:** *Record‹string, [Json](globals.md#json)›*

The metadata-derived controller state.

___

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

___

###  determineRequestChunkSpecifiers

▸ **determineRequestChunkSpecifiers**(`endBlockNumber`: BN, `totalNumberOfBlocks`: number): *[RequestChunkSpecifier](globals.md#requestchunkspecifier)[]*

Defined in fetchBlockFeeHistory.ts:336

Divides a block range (specified by a range size and the end of the range) into chunks based on
the maximum number of blocks that `eth_feeHistory` can return in a single call.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`endBlockNumber` | BN | The final block in the complete desired block range after all `eth_feeHistory` requests have been made. |
`totalNumberOfBlocks` | number | The total number of desired blocks after all `eth_feeHistory` requests have been made. |

**Returns:** *[RequestChunkSpecifier](globals.md#requestchunkspecifier)[]*

A set of arguments that can be used to make requests to `eth_feeHistory` in order to
retrieve all of the requested blocks, sorted from oldest block to newest block.

___

### `Const` ethTxsMock

▸ **ethTxsMock**(`ethTxHash`: string): *(object | object)[]*

Defined in transaction/mocks/txsMock.ts:3

**Parameters:**

Name | Type |
------ | ------ |
`ethTxHash` | string |

**Returns:** *(object | object)[]*

___

###  fetchBlockFeeHistory

▸ **fetchBlockFeeHistory**‹**Percentile**›(`__namedParameters`: object): *Promise‹[FeeHistoryBlock](globals.md#feehistoryblock)‹Percentile›[]›*

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

**Returns:** *Promise‹[FeeHistoryBlock](globals.md#feehistoryblock)‹Percentile›[]›*

The list of blocks and their fee data, sorted from oldest to newest.

___

###  fetchEthGasPriceEstimate

▸ **fetchEthGasPriceEstimate**(`ethQuery`: any): *Promise‹[EthGasPriceEstimate](globals.md#ethgaspriceestimate)›*

Defined in gas-util.ts:113

Get a gas price estimate from the network using the `eth_gasPrice` method.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`ethQuery` | any | The EthQuery instance to call the network with. |

**Returns:** *Promise‹[EthGasPriceEstimate](globals.md#ethgaspriceestimate)›*

A gas price estimate.

___

###  fetchGasEstimates

▸ **fetchGasEstimates**(`url`: string, `clientId?`: string): *Promise‹[GasFeeEstimates](globals.md#gasfeeestimates)›*

Defined in gas-util.ts:32

Fetch gas estimates from the given URL.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`url` | string | The gas estimate URL. |
`clientId?` | string | The client ID used to identify to the API who is asking for estimates. |

**Returns:** *Promise‹[GasFeeEstimates](globals.md#gasfeeestimates)›*

The gas estimates.

___

###  fetchGasEstimatesViaEthFeeHistory

▸ **fetchGasEstimatesViaEthFeeHistory**(`ethQuery`: [EthQuery](globals.md#ethquery)): *Promise‹[GasFeeEstimates](globals.md#gasfeeestimates)›*

Defined in fetchGasEstimatesViaEthFeeHistory.ts:29

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
`ethQuery` | [EthQuery](globals.md#ethquery) | An EthQuery instance. |

**Returns:** *Promise‹[GasFeeEstimates](globals.md#gasfeeestimates)›*

Base and priority fee estimates, categorized by priority level, as well as an estimate
for the next block's base fee.

___

###  fetchLatestBlock

▸ **fetchLatestBlock**(`ethQuery`: [EthQuery](globals.md#ethquery), `includeFullTransactionData`: boolean): *Promise‹[EthBlock](globals.md#ethblock)›*

Defined in fetchGasEstimatesViaEthFeeHistory/fetchLatestBlock.ts:12

Returns information about the latest completed block.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`ethQuery` | [EthQuery](globals.md#ethquery) | - | An EthQuery instance |
`includeFullTransactionData` | boolean | false | Whether or not to include all data for transactions as opposed to merely hashes. False by default. |

**Returns:** *Promise‹[EthBlock](globals.md#ethblock)›*

The block.

___

###  fetchLegacyGasPriceEstimates

▸ **fetchLegacyGasPriceEstimates**(`url`: string, `clientId?`: string): *Promise‹[LegacyGasPriceEstimate](globals.md#legacygaspriceestimate)›*

Defined in gas-util.ts:86

Hit the legacy MetaSwaps gasPrices estimate api and return the low, medium
high values from that API.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`url` | string | The URL to fetch gas price estimates from. |
`clientId?` | string | The client ID used to identify to the API who is asking for estimates. |

**Returns:** *Promise‹[LegacyGasPriceEstimate](globals.md#legacygaspriceestimate)›*

The gas price estimates.

___

###  fetchNetworkCongestionLevel

▸ **fetchNetworkCongestionLevel**(`blocks`: [FeeHistoryBlock](globals.md#feehistoryblock)‹never›[]): *number*

Defined in fetchGasEstimatesViaEthFeeHistory/calculateNetworkCongestion.ts:14

Calculates the approximate normalized ranking of the latest base fee in the given blocks among
the entirety of the blocks. That is, sorts all of the base fees, then finds the rank of the first
base fee that meets or exceeds the latest base fee among the base fees. The result is the rank
normalized as a number between 0 and 1, where 0 means that the latest base fee is the least of
all and 1 means that the latest base fee is the greatest of all. This can ultimately be used to
render a visualization of the status of the network for users.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`blocks` | [FeeHistoryBlock](globals.md#feehistoryblock)‹never›[] | A set of blocks obtained via [BlockFeeHistoryDatasetFetcher](classes/blockfeehistorydatasetfetcher.md). |

**Returns:** *number*

A number between 0 and 1.

___

###  fractionBN

▸ **fractionBN**(`targetBN`: any, `numerator`: number | string, `denominator`: number | string): *any*

Defined in util.ts:63

Used to multiply a BN by a fraction.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`targetBN` | any | Number to multiply by a fraction. |
`numerator` | number &#124; string | Numerator of the fraction multiplier. |
`denominator` | number &#124; string | Denominator of the fraction multiplier. |

**Returns:** *any*

Product of the multiplication.

___

###  fromHex

▸ **fromHex**(`value`: string | BN): *BN*

Defined in util.ts:272

Parses a hex string and converts it into a number that can be operated on in a bignum-safe,
base-10 way.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`value` | string &#124; BN | A base-16 number encoded as a string. |

**Returns:** *BN*

The number as a BN object in base-16 mode.

___

###  getAnonymizedState

▸ **getAnonymizedState**‹**S**›(`state`: S, `metadata`: [StateMetadata](globals.md#statemetadata)‹S›): *Record‹string, [Json](globals.md#json)›*

Defined in BaseControllerV2.ts:203

Returns an anonymized representation of the controller state.

By "anonymized" we mean that it should not contain any information that could be personally
identifiable.

**Type parameters:**

▪ **S**: *Record‹string, [Json](globals.md#json)›*

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`state` | S | The controller state. |
`metadata` | [StateMetadata](globals.md#statemetadata)‹S› | The controller state metadata, which describes how to derive the anonymized state. |

**Returns:** *Record‹string, [Json](globals.md#json)›*

The anonymized controller state.

___

###  getBuyURL

▸ **getBuyURL**(`networkCode`: string, `address?`: string, `amount`: number): *string | undefined*

Defined in util.ts:128

Return a URL that can be used to obtain ETH for a given network.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`networkCode` | string | "1" | Network code of desired network. |
`address?` | string | - | Address to deposit obtained ETH. |
`amount` | number | 5 | How much ETH is desired. |

**Returns:** *string | undefined*

URL to buy ETH based on network.

___

###  getEtherscanApiUrl

▸ **getEtherscanApiUrl**(`networkType`: string, `urlParams`: any): *string*

Defined in util.ts:156

Return a URL that can be used to fetch ETH transactions.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`networkType` | string | Network type of desired network. |
`urlParams` | any | The parameters used to construct the URL. |

**Returns:** *string*

URL to fetch the access the endpoint.

___

### `Const` getIncreasedPriceFromExisting

▸ **getIncreasedPriceFromExisting**(`value`: string | undefined, `rate`: number): *string*

Defined in util.ts:709

**Parameters:**

Name | Type |
------ | ------ |
`value` | string &#124; undefined |
`rate` | number |

**Returns:** *string*

___

### `Const` getIncreasedPriceHex

▸ **getIncreasedPriceHex**(`value`: number, `rate`: number): *string*

Defined in util.ts:706

**Parameters:**

Name | Type |
------ | ------ |
`value` | number |
`rate` | number |

**Returns:** *string*

___

###  getPersistentState

▸ **getPersistentState**‹**S**›(`state`: S, `metadata`: [StateMetadata](globals.md#statemetadata)‹S›): *Record‹string, [Json](globals.md#json)›*

Defined in BaseControllerV2.ts:217

Returns the subset of state that should be persisted.

**Type parameters:**

▪ **S**: *Record‹string, [Json](globals.md#json)›*

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`state` | S | The controller state. |
`metadata` | [StateMetadata](globals.md#statemetadata)‹S› | The controller state metadata, which describes which pieces of state should be persisted. |

**Returns:** *Record‹string, [Json](globals.md#json)›*

The subset of controller state that should be persisted.

___

###  gweiDecToWEIBN

▸ **gweiDecToWEIBN**(`n`: number | string): *any*

Defined in util.ts:79

Used to convert a base-10 number from GWEI to WEI. Can handle numbers with decimal parts.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`n` | number &#124; string | The base 10 number to convert to WEI. |

**Returns:** *any*

The number in WEI, as a BN.

___

###  handleFetch

▸ **handleFetch**(`request`: string, `options?`: RequestInit): *Promise‹any›*

Defined in util.ts:606

Execute fetch and return object response.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`request` | string | The request information. |
`options?` | RequestInit | The fetch options. |

**Returns:** *Promise‹any›*

The fetch response JSON data.

___

###  handleTransactionFetch

▸ **handleTransactionFetch**(`networkType`: string, `address`: string, `txHistoryLimit`: number, `opt?`: [FetchAllOptions](interfaces/fetchalloptions.md)): *Promise‹[object, object]›*

Defined in util.ts:185

Handles the fetch of incoming transactions.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`networkType` | string | Network type of desired network. |
`address` | string | Address to get the transactions from. |
`txHistoryLimit` | number | The maximum number of transactions to fetch. |
`opt?` | [FetchAllOptions](interfaces/fetchalloptions.md) | Object that can contain fromBlock and Etherscan service API key. |

**Returns:** *Promise‹[object, object]›*

Responses for both ETH and ERC20 token transactions.

___

###  hexToBN

▸ **hexToBN**(`inputHex`: string): *BN‹›*

Defined in util.ts:244

Converts a hex string to a BN object.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`inputHex` | string | Number represented as a hex string. |

**Returns:** *BN‹›*

A BN instance.

___

###  hexToText

▸ **hexToText**(`hex`: string): *string*

Defined in util.ts:254

A helper function that converts hex data to human readable string.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`hex` | string | The hex string to convert to string. |

**Returns:** *string*

A human readable string conversion.

___

### `Const` isEIP1559Transaction

▸ **isEIP1559Transaction**(`transaction`: [Transaction](interfaces/transaction.md)): *boolean*

Defined in util.ts:694

Checks if a transaction is EIP-1559 by checking for the existence of
maxFeePerGas and maxPriorityFeePerGas within its parameters.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`transaction` | [Transaction](interfaces/transaction.md) | Transaction object to add. |

**Returns:** *boolean*

Boolean that is true if the transaction is EIP-1559 (has maxFeePerGas and maxPriorityFeePerGas), otherwise returns false.

___

### `Const` isFeeMarketEIP1559Values

▸ **isFeeMarketEIP1559Values**(`gasValues?`: [GasPriceValue](interfaces/gaspricevalue.md) | [FeeMarketEIP1559Values](interfaces/feemarketeip1559values.md)): *gasValues is FeeMarketEIP1559Values*

Defined in util.ts:729

**Parameters:**

Name | Type |
------ | ------ |
`gasValues?` | [GasPriceValue](interfaces/gaspricevalue.md) &#124; [FeeMarketEIP1559Values](interfaces/feemarketeip1559values.md) |

**Returns:** *gasValues is FeeMarketEIP1559Values*

___

### `Const` isGasPriceValue

▸ **isGasPriceValue**(`gasValues?`: [GasPriceValue](interfaces/gaspricevalue.md) | [FeeMarketEIP1559Values](interfaces/feemarketeip1559values.md)): *gasValues is GasPriceValue*

Defined in util.ts:735

**Parameters:**

Name | Type |
------ | ------ |
`gasValues?` | [GasPriceValue](interfaces/gaspricevalue.md) &#124; [FeeMarketEIP1559Values](interfaces/feemarketeip1559values.md) |

**Returns:** *gasValues is GasPriceValue*

___

###  isValidHexAddress

▸ **isValidHexAddress**(`possibleAddress`: string, `__namedParameters`: object): *boolean*

Defined in util.ts:400

Validates that the input is a hex address. This utility method is a thin
wrapper around ethereumjs-util.isValidAddress, with the exception that it
does not throw an error when provided values that are not hex strings. In
addition, and by default, this method will return true for hex strings that
meet the length requirement of a hex address, but are not prefixed with `0x`
Finally, if the mixedCaseUseChecksum flag is true and a mixed case string is
provided this method will validate it has the proper checksum formatting.

**Parameters:**

▪ **possibleAddress**: *string*

Input parameter to check against.

▪`Default value`  **__namedParameters**: *object*= {}

Name | Type | Default |
------ | ------ | ------ |
`allowNonPrefixed` | boolean | true |

**Returns:** *boolean*

Whether or not the input is a valid hex address.

___

### `Const` makeClientIdHeader

▸ **makeClientIdHeader**(`clientId`: string): *object*

Defined in gas-util.ts:11

**Parameters:**

Name | Type |
------ | ------ |
`clientId` | string |

**Returns:** *object*

* **X-Client-Id**: *string* = clientId

___

###  makeRequestForChunk

▸ **makeRequestForChunk**‹**Percentile**›(`__namedParameters`: object): *Promise‹[FeeHistoryBlock](globals.md#feehistoryblock)‹Percentile›[]›*

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

**Returns:** *Promise‹[FeeHistoryBlock](globals.md#feehistoryblock)‹Percentile›[]›*

A list of block data.

___

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

___

###  mockFetch

▸ **mockFetch**(`data`: any): *any*

Defined in transaction/TransactionController.test.ts:87

Create a mock implementation of `fetch` that always returns the same data.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`data` | any | The mock data to return. |

**Returns:** *any*

The mock `fetch` implementation.

___

###  mockFetchs

▸ **mockFetchs**(`data`: any): *any*

Defined in transaction/TransactionController.test.ts:102

Create a mock implementation of `fetch` that returns different mock data for each URL.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`data` | any | A map of mock data, keyed by URL. |

**Returns:** *any*

The mock `fetch` implementation.

___

###  normalizeEnsName

▸ **normalizeEnsName**(`ensName`: string): *string | null*

Defined in util.ts:641

Normalizes the given ENS name.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`ensName` | string | The ENS name. |

**Returns:** *string | null*

The normalized ENS name string.

___

###  normalizeGWEIDecimalNumbers

▸ **normalizeGWEIDecimalNumbers**(`n`: string | number): *any*

Defined in gas-util.ts:19

Convert a decimal GWEI value to a decimal string rounded to the nearest WEI.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`n` | string &#124; number | The input GWEI amount, as a decimal string or a number. |

**Returns:** *any*

The decimal string GWEI amount.

___

###  normalizeMessageData

▸ **normalizeMessageData**(`data`: string): *string*

Defined in util.ts:480

A helper function that converts rawmessageData buffer data to a hex, or just returns the data if
it is already formatted as a hex.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`data` | string | The buffer data to convert to a hex. |

**Returns:** *string*

A hex string conversion of the buffer data.

___

###  normalizeTransaction

▸ **normalizeTransaction**(`transaction`: [Transaction](interfaces/transaction.md)): *[Transaction](interfaces/transaction.md)*

Defined in util.ts:301

Normalizes properties on a Transaction object.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`transaction` | [Transaction](interfaces/transaction.md) | Transaction object to normalize. |

**Returns:** *[Transaction](interfaces/transaction.md)*

Normalized Transaction object.

___

###  query

▸ **query**(`ethQuery`: any, `method`: string, `args`: any[]): *Promise‹any›*

Defined in util.ts:665

Wrapper method to handle EthQuery requests.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`ethQuery` | any | - | EthQuery object initialized with a provider. |
`method` | string | - | Method to request. |
`args` | any[] | [] | Arguments to send. |

**Returns:** *Promise‹any›*

Promise resolving the request.

___

###  safelyExecute

▸ **safelyExecute**(`operation`: function, `logError`: boolean, `retry?`: function): *Promise‹any›*

Defined in util.ts:320

Execute and return an asynchronous operation without throwing errors.

**Parameters:**

▪ **operation**: *function*

Function returning a Promise.

▸ (): *Promise‹any›*

▪`Default value`  **logError**: *boolean*= false

Determines if the error should be logged.

▪`Optional`  **retry**: *function*

Function called if an error is caught.

▸ (`error`: Error): *void*

**Parameters:**

Name | Type |
------ | ------ |
`error` | Error |

**Returns:** *Promise‹any›*

Promise resolving to the result of the async operation.

___

###  safelyExecuteWithTimeout

▸ **safelyExecuteWithTimeout**(`operation`: function, `logError`: boolean, `timeout`: number): *Promise‹any›*

Defined in util.ts:345

Execute and return an asynchronous operation with a timeout.

**Parameters:**

▪ **operation**: *function*

Function returning a Promise.

▸ (): *Promise‹any›*

▪`Default value`  **logError**: *boolean*= false

Determines if the error should be logged.

▪`Default value`  **timeout**: *number*= 500

Timeout to fail the operation.

**Returns:** *Promise‹any›*

Promise resolving to the result of the async operation.

___

###  successfulFetch

▸ **successfulFetch**(`request`: string, `options?`: RequestInit): *Promise‹Response›*

Defined in util.ts:589

Execute fetch and verify that the response was successful.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`request` | string | Request information. |
`options?` | RequestInit | Fetch options. |

**Returns:** *Promise‹Response›*

The fetch response.

___

###  timeoutFetch

▸ **timeoutFetch**(`url`: string, `options?`: RequestInit, `timeout`: number): *Promise‹Response›*

Defined in util.ts:620

Fetch that fails after timeout.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`url` | string | - | Url to fetch. |
`options?` | RequestInit | - | Options to send with the request. |
`timeout` | number | 500 | Timeout to fail request. |

**Returns:** *Promise‹Response›*

Promise resolving the request.

___

###  toChecksumHexAddress

▸ **toChecksumHexAddress**(`address`: string): *string*

Defined in util.ts:374

Convert an address to a checksummed hexidecimal address.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`address` | string | The address to convert. |

**Returns:** *string*

A 0x-prefixed hexidecimal checksummed address.

___

###  toHex

▸ **toHex**(`value`: number | string | BN): *string*

Defined in util.ts:285

Converts an integer to a hexadecimal representation.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`value` | number &#124; string &#124; BN | An integer, an integer encoded as a base-10 string, or a BN. |

**Returns:** *string*

The integer encoded as a hex string.

___

### `Const` tokenTxsMock

▸ **tokenTxsMock**(`tokenTxHash`: string): *object[]*

Defined in transaction/mocks/txsMock.ts:81

**Parameters:**

Name | Type |
------ | ------ |
`tokenTxHash` | string |

**Returns:** *object[]*

___

### `Const` txsInStateMock

▸ **txsInStateMock**(`ethTxHash`: string, `tokenTxHash`: string): *[TransactionMeta](globals.md#transactionmeta)[]*

Defined in transaction/mocks/txsMock.ts:370

**Parameters:**

Name | Type |
------ | ------ |
`ethTxHash` | string |
`tokenTxHash` | string |

**Returns:** *[TransactionMeta](globals.md#transactionmeta)[]*

___

### `Const` txsInStateWithOutdatedGasDataMock

▸ **txsInStateWithOutdatedGasDataMock**(`ethTxHash`: string, `tokenTxHash`: string): *[TransactionMeta](globals.md#transactionmeta)[]*

Defined in transaction/mocks/txsMock.ts:454

**Parameters:**

Name | Type |
------ | ------ |
`ethTxHash` | string |
`tokenTxHash` | string |

**Returns:** *[TransactionMeta](globals.md#transactionmeta)[]*

___

### `Const` txsInStateWithOutdatedStatusAndGasDataMock

▸ **txsInStateWithOutdatedStatusAndGasDataMock**(`ethTxHash`: string, `tokenTxHash`: string): *[TransactionMeta](globals.md#transactionmeta)[]*

Defined in transaction/mocks/txsMock.ts:496

**Parameters:**

Name | Type |
------ | ------ |
`ethTxHash` | string |
`tokenTxHash` | string |

**Returns:** *[TransactionMeta](globals.md#transactionmeta)[]*

___

### `Const` txsInStateWithOutdatedStatusMock

▸ **txsInStateWithOutdatedStatusMock**(`ethTxHash`: string, `tokenTxHash`: string): *[TransactionMeta](globals.md#transactionmeta)[]*

Defined in transaction/mocks/txsMock.ts:412

**Parameters:**

Name | Type |
------ | ------ |
`ethTxHash` | string |
`tokenTxHash` | string |

**Returns:** *[TransactionMeta](globals.md#transactionmeta)[]*

___

### `Const` validateGasValues

▸ **validateGasValues**(`gasValues`: [GasPriceValue](interfaces/gaspricevalue.md) | [FeeMarketEIP1559Values](interfaces/feemarketeip1559values.md)): *void*

Defined in util.ts:716

**Parameters:**

Name | Type |
------ | ------ |
`gasValues` | [GasPriceValue](interfaces/gaspricevalue.md) &#124; [FeeMarketEIP1559Values](interfaces/feemarketeip1559values.md) |

**Returns:** *void*

___

###  validateMinimumIncrease

▸ **validateMinimumIncrease**(`proposed`: string, `min`: string): *string*

Defined in util.ts:748

Validates that the proposed value is greater than or equal to the minimum value.

**`throws`** Will throw if the proposed value is too low.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`proposed` | string | The proposed value. |
`min` | string | The minimum value. |

**Returns:** *string*

The proposed value.

___

###  validateSignMessageData

▸ **validateSignMessageData**(`messageData`: PersonalMessageParams | MessageParams): *void*

Defined in util.ts:498

Validates a PersonalMessageParams and MessageParams objects for required properties and throws in
the event of any validation error.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`messageData` | PersonalMessageParams &#124; MessageParams | PersonalMessageParams object to validate.  |

**Returns:** *void*

___

###  validateTransaction

▸ **validateTransaction**(`transaction`: [Transaction](interfaces/transaction.md)): *void*

Defined in util.ts:420

Validates a Transaction object for required properties and throws in
the event of any validation error.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`transaction` | [Transaction](interfaces/transaction.md) | Transaction object to validate.  |

**Returns:** *void*

___

###  validateTypedSignMessageDataV1

▸ **validateTypedSignMessageDataV1**(`messageData`: TypedMessageParams): *void*

Defined in util.ts:517

Validates a TypedMessageParams object for required properties and throws in
the event of any validation error for eth_signTypedMessage_V1.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`messageData` | TypedMessageParams | TypedMessageParams object to validate.  |

**Returns:** *void*

___

###  validateTypedSignMessageDataV3

▸ **validateTypedSignMessageDataV3**(`messageData`: TypedMessageParams): *void*

Defined in util.ts:550

Validates a TypedMessageParams object for required properties and throws in
the event of any validation error for eth_signTypedMessage_V3.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`messageData` | TypedMessageParams | TypedMessageParams object to validate.  |

**Returns:** *void*

___

###  weiHexToGweiDec

▸ **weiHexToGweiDec**(`hex`: string): *any*

Defined in util.ts:115

Used to convert values from wei hex format to dec gwei format.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`hex` | string | The value in hex wei. |

**Returns:** *any*

The value in dec gwei as string.

## Object literals

### `Const` ETH_TX_HISTORY_DATA

### ▪ **ETH_TX_HISTORY_DATA**: *object*

Defined in transaction/TransactionController.test.ts:209

###  message

• **message**: *string* = "OK"

Defined in transaction/TransactionController.test.ts:210

###  result

• **result**: *(object | object)[]* = ETH_TRANSACTIONS

Defined in transaction/TransactionController.test.ts:211

###  status

• **status**: *string* = "1"

Defined in transaction/TransactionController.test.ts:212

___

### `Const` ETH_TX_HISTORY_DATA_FROM_BLOCK

### ▪ **ETH_TX_HISTORY_DATA_FROM_BLOCK**: *object*

Defined in transaction/TransactionController.test.ts:215

###  message

• **message**: *string* = "OK"

Defined in transaction/TransactionController.test.ts:216

###  result

• **result**: *(object | object)[]* = [ETH_TRANSACTIONS[0], ETH_TRANSACTIONS[1]]

Defined in transaction/TransactionController.test.ts:217

###  status

• **status**: *string* = "1"

Defined in transaction/TransactionController.test.ts:218

___

### `Const` ETH_TX_HISTORY_DATA_ROPSTEN_NO_TRANSACTIONS_FOUND

### ▪ **ETH_TX_HISTORY_DATA_ROPSTEN_NO_TRANSACTIONS_FOUND**: *object*

Defined in transaction/TransactionController.test.ts:233

###  message

• **message**: *string* = "No transactions found"

Defined in transaction/TransactionController.test.ts:234

###  result

• **result**: *undefined[]* = []

Defined in transaction/TransactionController.test.ts:235

###  status

• **status**: *string* = "0"

Defined in transaction/TransactionController.test.ts:236

___

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

### `Const` MOCK_CUSTOM_NETWORK

### ▪ **MOCK_CUSTOM_NETWORK**: *object*

Defined in transaction/TransactionController.test.ts:163

###  getProvider

▸ **getProvider**(): *any*

Defined in transaction/TransactionController.test.ts:164

**Returns:** *any*

###  subscribe

▸ **subscribe**(): *any*

Defined in transaction/TransactionController.test.ts:174

**Returns:** *any*

▪ **state**: *object*

Defined in transaction/TransactionController.test.ts:165

* **isCustomNetwork**: *boolean* = true

* **network**: *string* = "80001"

* **properties**: *object*

  * **isEIP1559Compatible**: *boolean* = false

* **provider**: *object*

  * **chainId**: *string* = "80001"

  * **type**: *any* = 'rpc' as NetworkType

___

### `Const` MOCK_FETCH_TX_HISTORY_DATA_ERROR

### ▪ **MOCK_FETCH_TX_HISTORY_DATA_ERROR**: *object*

Defined in transaction/TransactionController.test.ts:258

###  status

• **status**: *string* = "0"

Defined in transaction/TransactionController.test.ts:259

___

### `Const` MOCK_FETCH_TX_HISTORY_DATA_OK

### ▪ **MOCK_FETCH_TX_HISTORY_DATA_OK**: *object*

Defined in transaction/TransactionController.test.ts:239

###  https://api-ropsten.etherscan.io/api?module=account&address=0x6bf137f335ea1b8f193b8f6ea92561a60d23a207&offset=2&order=desc&action=tokentx&tag=latest&page=1

• **https://api-ropsten.etherscan.io/api?module=account&address=0x6bf137f335ea1b8f193b8f6ea92561a60d23a207&offset=2&order=desc&action=tokentx&tag=latest&page=1**: *object* = ETH_TX_HISTORY_DATA_ROPSTEN_NO_TRANSACTIONS_FOUND

Defined in transaction/TransactionController.test.ts:252

#### Type declaration:

* **message**: *string* = "No transactions found"

* **result**: *undefined[]* = []

* **status**: *string* = "0"

###  https://api-ropsten.etherscan.io/api?module=account&address=0x6bf137f335ea1b8f193b8f6ea92561a60d23a207&offset=2&order=desc&action=txlist&tag=latest&page=1

• **https://api-ropsten.etherscan.io/api?module=account&address=0x6bf137f335ea1b8f193b8f6ea92561a60d23a207&offset=2&order=desc&action=txlist&tag=latest&page=1**: *object* = ETH_TX_HISTORY_DATA

Defined in transaction/TransactionController.test.ts:254

#### Type declaration:

* **message**: *string* = "OK"

* **result**: *(object | object)[]* = ETH_TRANSACTIONS

* **status**: *string* = "1"

###  https://api-ropsten.etherscan.io/api?module=account&address=0x6bf137f335ea1b8f193b8f6ea92561a60d23a207&offset=40&order=desc&action=tokentx&tag=latest&page=1

• **https://api-ropsten.etherscan.io/api?module=account&address=0x6bf137f335ea1b8f193b8f6ea92561a60d23a207&offset=40&order=desc&action=tokentx&tag=latest&page=1**: *object* = ETH_TX_HISTORY_DATA_ROPSTEN_NO_TRANSACTIONS_FOUND

Defined in transaction/TransactionController.test.ts:240

#### Type declaration:

* **message**: *string* = "No transactions found"

* **result**: *undefined[]* = []

* **status**: *string* = "0"

###  https://api-ropsten.etherscan.io/api?module=account&address=0x6bf137f335ea1b8f193b8f6ea92561a60d23a207&offset=40&order=desc&action=txlist&tag=latest&page=1

• **https://api-ropsten.etherscan.io/api?module=account&address=0x6bf137f335ea1b8f193b8f6ea92561a60d23a207&offset=40&order=desc&action=txlist&tag=latest&page=1**: *object* = ETH_TX_HISTORY_DATA

Defined in transaction/TransactionController.test.ts:248

#### Type declaration:

* **message**: *string* = "OK"

* **result**: *(object | object)[]* = ETH_TRANSACTIONS

* **status**: *string* = "1"

###  https://api.etherscan.io/api?module=account&address=0x6bf137f335ea1b8f193b8f6ea92561a60d23a207&offset=40&order=desc&action=tokentx&tag=latest&page=1

• **https://api.etherscan.io/api?module=account&address=0x6bf137f335ea1b8f193b8f6ea92561a60d23a207&offset=40&order=desc&action=tokentx&tag=latest&page=1**: *object* = TOKEN_TX_HISTORY_DATA

Defined in transaction/TransactionController.test.ts:242

#### Type declaration:

* **message**: *string* = "OK"

* **result**: *object[]* = TOKEN_TRANSACTIONS

* **status**: *string* = "1"

###  https://api.etherscan.io/api?module=account&address=0x6bf137f335ea1b8f193b8f6ea92561a60d23a207&offset=40&order=desc&action=txlist&tag=latest&page=1

• **https://api.etherscan.io/api?module=account&address=0x6bf137f335ea1b8f193b8f6ea92561a60d23a207&offset=40&order=desc&action=txlist&tag=latest&page=1**: *object* = ETH_TX_HISTORY_DATA

Defined in transaction/TransactionController.test.ts:246

#### Type declaration:

* **message**: *string* = "OK"

* **result**: *(object | object)[]* = ETH_TRANSACTIONS

* **status**: *string* = "1"

###  https://api.etherscan.io/api?module=account&address=0x6bf137f335ea1b8f193b8f6ea92561a60d23a207&startBlock=999&offset=40&order=desc&action=tokentx&tag=latest&page=1

• **https://api.etherscan.io/api?module=account&address=0x6bf137f335ea1b8f193b8f6ea92561a60d23a207&startBlock=999&offset=40&order=desc&action=tokentx&tag=latest&page=1**: *object* = TOKEN_TX_HISTORY_DATA_FROM_BLOCK

Defined in transaction/TransactionController.test.ts:244

#### Type declaration:

* **message**: *string* = "OK"

* **result**: *object[]* = [TOKEN_TRANSACTIONS[0]]

* **status**: *string* = "1"

###  https://api.etherscan.io/api?module=account&address=0x6bf137f335ea1b8f193b8f6ea92561a60d23a207&startBlock=999&offset=40&order=desc&action=txlist&tag=latest&page=1

• **https://api.etherscan.io/api?module=account&address=0x6bf137f335ea1b8f193b8f6ea92561a60d23a207&startBlock=999&offset=40&order=desc&action=txlist&tag=latest&page=1**: *object* = ETH_TX_HISTORY_DATA_FROM_BLOCK

Defined in transaction/TransactionController.test.ts:250

#### Type declaration:

* **message**: *string* = "OK"

* **result**: *(object | object)[]* = [ETH_TRANSACTIONS[0], ETH_TRANSACTIONS[1]]

* **status**: *string* = "1"

___

### `Const` MOCK_MAINNET_NETWORK

### ▪ **MOCK_MAINNET_NETWORK**: *object*

Defined in transaction/TransactionController.test.ts:150

###  getProvider

▸ **getProvider**(): *any*

Defined in transaction/TransactionController.test.ts:151

**Returns:** *any*

###  subscribe

▸ **subscribe**(): *any*

Defined in transaction/TransactionController.test.ts:161

**Returns:** *any*

▪ **state**: *object*

Defined in transaction/TransactionController.test.ts:152

* **isCustomNetwork**: *boolean* = false

* **network**: *string* = "1"

* **properties**: *object*

  * **isEIP1559Compatible**: *boolean* = false

* **provider**: *object*

  * **chainId**: *any* = NetworksChainId.mainnet

  * **type**: *any* = 'mainnet' as NetworkType

___

### `Const` MOCK_NETWORK

### ▪ **MOCK_NETWORK**: *object*

Defined in transaction/TransactionController.test.ts:118

###  getProvider

▸ **getProvider**(): *any*

Defined in transaction/TransactionController.test.ts:119

**Returns:** *any*

###  subscribe

▸ **subscribe**(): *any*

Defined in transaction/TransactionController.test.ts:129

**Returns:** *any*

▪ **state**: *object*

Defined in transaction/TransactionController.test.ts:120

* **isCustomNetwork**: *boolean* = false

* **network**: *string* = "3"

* **properties**: *object*

  * **isEIP1559Compatible**: *boolean* = false

* **provider**: *object*

  * **chainId**: *any* = NetworksChainId.ropsten

  * **type**: *any* = 'ropsten' as NetworkType

___

### `Const` MOCK_NETWORK_CUSTOM

### ▪ **MOCK_NETWORK_CUSTOM**: *object*

Defined in transaction/TransactionController.test.ts:131

###  getProvider

▸ **getProvider**(): *any*

Defined in transaction/TransactionController.test.ts:132

**Returns:** *any*

###  subscribe

▸ **subscribe**(): *any*

Defined in transaction/TransactionController.test.ts:142

**Returns:** *any*

▪ **state**: *object*

Defined in transaction/TransactionController.test.ts:133

* **isCustomNetwork**: *boolean* = true

* **network**: *string* = "10"

* **properties**: *object*

  * **isEIP1559Compatible**: *boolean* = false

* **provider**: *object*

  * **chainId**: *any* = NetworksChainId.optimism

  * **type**: *any* = 'optimism' as NetworkType

___

### `Const` MOCK_NETWORK_WITHOUT_CHAIN_ID

### ▪ **MOCK_NETWORK_WITHOUT_CHAIN_ID**: *object*

Defined in transaction/TransactionController.test.ts:144

###  isCustomNetwork

• **isCustomNetwork**: *boolean* = false

Defined in transaction/TransactionController.test.ts:146

###  getProvider

▸ **getProvider**(): *any*

Defined in transaction/TransactionController.test.ts:145

**Returns:** *any*

###  subscribe

▸ **subscribe**(): *any*

Defined in transaction/TransactionController.test.ts:148

**Returns:** *any*

▪ **state**: *object*

Defined in transaction/TransactionController.test.ts:147

* **network**: *string* = "3"

* **provider**: *object*

  * **type**: *any* = 'ropsten' as NetworkType

___

### `Const` MOCK_PRFERENCES

### ▪ **MOCK_PRFERENCES**: *object*

Defined in transaction/TransactionController.test.ts:111

▪ **state**: *object*

Defined in transaction/TransactionController.test.ts:111

* **selectedAddress**: *string* = "foo"

___

### `Const` NORMALIZERS

### ▪ **NORMALIZERS**: *object*

Defined in util.ts:30

###  data

▸ **data**(`data`: string): *string*

Defined in util.ts:31

**Parameters:**

Name | Type |
------ | ------ |
`data` | string |

**Returns:** *string*

###  estimatedBaseFee

▸ **estimatedBaseFee**(`maxPriorityFeePerGas`: string): *string*

Defined in util.ts:41

**Parameters:**

Name | Type |
------ | ------ |
`maxPriorityFeePerGas` | string |

**Returns:** *string*

###  from

▸ **from**(`from`: string): *string*

Defined in util.ts:32

**Parameters:**

Name | Type |
------ | ------ |
`from` | string |

**Returns:** *string*

###  gas

▸ **gas**(`gas`: string): *string*

Defined in util.ts:33

**Parameters:**

Name | Type |
------ | ------ |
`gas` | string |

**Returns:** *string*

###  gasPrice

▸ **gasPrice**(`gasPrice`: string): *string*

Defined in util.ts:34

**Parameters:**

Name | Type |
------ | ------ |
`gasPrice` | string |

**Returns:** *string*

###  maxFeePerGas

▸ **maxFeePerGas**(`maxFeePerGas`: string): *string*

Defined in util.ts:38

**Parameters:**

Name | Type |
------ | ------ |
`maxFeePerGas` | string |

**Returns:** *string*

###  maxPriorityFeePerGas

▸ **maxPriorityFeePerGas**(`maxPriorityFeePerGas`: string): *string*

Defined in util.ts:39

**Parameters:**

Name | Type |
------ | ------ |
`maxPriorityFeePerGas` | string |

**Returns:** *string*

###  nonce

▸ **nonce**(`nonce`: string): *string*

Defined in util.ts:35

**Parameters:**

Name | Type |
------ | ------ |
`nonce` | string |

**Returns:** *string*

###  to

▸ **to**(`to`: string): *string*

Defined in util.ts:36

**Parameters:**

Name | Type |
------ | ------ |
`to` | string |

**Returns:** *string*

###  value

▸ **value**(`value`: string): *string*

Defined in util.ts:37

**Parameters:**

Name | Type |
------ | ------ |
`value` | string |

**Returns:** *string*

___

### `Const` SETTINGS_BY_PRIORITY_LEVEL

### ▪ **SETTINGS_BY_PRIORITY_LEVEL**: *object*

Defined in fetchGasEstimatesViaEthFeeHistory/calculateGasFeeEstimatesForPriorityLevels.ts:13

Defined in getGasEstimatesViaEthFeeHistory.ts:17

▪ **high**: *object*

Defined in fetchGasEstimatesViaEthFeeHistory/calculateGasFeeEstimatesForPriorityLevels.ts:34

Defined in getGasEstimatesViaEthFeeHistory.ts:38

* **baseFeePercentageMultiplier**: *BN‹›* = new BN(125)

* **minSuggestedMaxPriorityFeePerGas**: *BN‹›* = new BN(2_000_000_000)

* **percentile**: *10 | 20 | 30* = 30 as Percentile

* **priorityFeePercentageMultiplier**: *BN‹›* = new BN(98)

* **estimatedWaitTimes**: *object*

  * **maxWaitTimeEstimate**: *number* = 60000

  * **minWaitTimeEstimate**: *number* = 15000

▪ **low**: *object*

Defined in fetchGasEstimatesViaEthFeeHistory/calculateGasFeeEstimatesForPriorityLevels.ts:14

Defined in getGasEstimatesViaEthFeeHistory.ts:18

* **baseFeePercentageMultiplier**: *BN‹›* = new BN(110)

* **minSuggestedMaxPriorityFeePerGas**: *BN‹›* = new BN(1_000_000_000)

* **percentile**: *10 | 20 | 30* = 10 as Percentile

* **priorityFeePercentageMultiplier**: *BN‹›* = new BN(94)

* **estimatedWaitTimes**: *object*

  * **maxWaitTimeEstimate**: *number* = 30000

  * **minWaitTimeEstimate**: *number* = 15000

▪ **medium**: *object*

Defined in fetchGasEstimatesViaEthFeeHistory/calculateGasFeeEstimatesForPriorityLevels.ts:24

Defined in getGasEstimatesViaEthFeeHistory.ts:28

* **baseFeePercentageMultiplier**: *BN‹›* = new BN(120)

* **minSuggestedMaxPriorityFeePerGas**: *BN‹›* = new BN(1_500_000_000)

* **percentile**: *10 | 20 | 30* = 20 as Percentile

* **priorityFeePercentageMultiplier**: *BN‹›* = new BN(97)

* **estimatedWaitTimes**: *object*

  * **maxWaitTimeEstimate**: *number* = 45000

  * **minWaitTimeEstimate**: *number* = 15000

___

### `Const` TOKEN_TX_HISTORY_DATA

### ▪ **TOKEN_TX_HISTORY_DATA**: *object*

Defined in transaction/TransactionController.test.ts:221

###  message

• **message**: *string* = "OK"

Defined in transaction/TransactionController.test.ts:222

###  result

• **result**: *object[]* = TOKEN_TRANSACTIONS

Defined in transaction/TransactionController.test.ts:223

###  status

• **status**: *string* = "1"

Defined in transaction/TransactionController.test.ts:224

___

### `Const` TOKEN_TX_HISTORY_DATA_FROM_BLOCK

### ▪ **TOKEN_TX_HISTORY_DATA_FROM_BLOCK**: *object*

Defined in transaction/TransactionController.test.ts:227

###  message

• **message**: *string* = "OK"

Defined in transaction/TransactionController.test.ts:228

###  result

• **result**: *object[]* = [TOKEN_TRANSACTIONS[0]]

Defined in transaction/TransactionController.test.ts:229

###  status

• **status**: *string* = "1"

Defined in transaction/TransactionController.test.ts:230

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

___

### `Const` mockFlags

### ▪ **mockFlags**: *object*

Defined in transaction/TransactionController.test.ts:24

###  estimateGas

• **estimateGas**: *null* = null

Defined in transaction/TransactionController.test.ts:25
