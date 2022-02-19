[metamask-controllers-main-src-gas-2](../README.md) › [Globals](../globals.md) › ["transaction/TransactionController.test"](_transaction_transactioncontroller_test_.md)

# Module: "transaction/TransactionController.test"

## Index

### Variables

* [ETHER_TRANSACTION_HASH](_transaction_transactioncontroller_test_.md#const-ether_transaction_hash)
* [ETH_TRANSACTIONS](_transaction_transactioncontroller_test_.md#const-eth_transactions)
* [MAINNET_PROVIDER](_transaction_transactioncontroller_test_.md#const-mainnet_provider)
* [PROVIDER](_transaction_transactioncontroller_test_.md#const-provider)
* [TOKEN_TRANSACTIONS](_transaction_transactioncontroller_test_.md#const-token_transactions)
* [TOKEN_TRANSACTION_HASH](_transaction_transactioncontroller_test_.md#const-token_transaction_hash)
* [TRANSACTIONS_IN_STATE](_transaction_transactioncontroller_test_.md#const-transactions_in_state)
* [TRANSACTIONS_IN_STATE_WITH_OUTDATED_GAS_DATA](_transaction_transactioncontroller_test_.md#const-transactions_in_state_with_outdated_gas_data)
* [TRANSACTIONS_IN_STATE_WITH_OUTDATED_STATUS](_transaction_transactioncontroller_test_.md#const-transactions_in_state_with_outdated_status)
* [TRANSACTIONS_IN_STATE_WITH_OUTDATED_STATUS_AND_GAS_DATA](_transaction_transactioncontroller_test_.md#const-transactions_in_state_with_outdated_status_and_gas_data)
* [globalAny](_transaction_transactioncontroller_test_.md#const-globalany)

### Functions

* [mockFetch](_transaction_transactioncontroller_test_.md#mockfetch)
* [mockFetchs](_transaction_transactioncontroller_test_.md#mockfetchs)

### Object literals

* [ETH_TX_HISTORY_DATA](_transaction_transactioncontroller_test_.md#const-eth_tx_history_data)
* [ETH_TX_HISTORY_DATA_FROM_BLOCK](_transaction_transactioncontroller_test_.md#const-eth_tx_history_data_from_block)
* [ETH_TX_HISTORY_DATA_ROPSTEN_NO_TRANSACTIONS_FOUND](_transaction_transactioncontroller_test_.md#const-eth_tx_history_data_ropsten_no_transactions_found)
* [MOCK_CUSTOM_NETWORK](_transaction_transactioncontroller_test_.md#const-mock_custom_network)
* [MOCK_FETCH_TX_HISTORY_DATA_ERROR](_transaction_transactioncontroller_test_.md#const-mock_fetch_tx_history_data_error)
* [MOCK_FETCH_TX_HISTORY_DATA_OK](_transaction_transactioncontroller_test_.md#const-mock_fetch_tx_history_data_ok)
* [MOCK_MAINNET_NETWORK](_transaction_transactioncontroller_test_.md#const-mock_mainnet_network)
* [MOCK_NETWORK](_transaction_transactioncontroller_test_.md#const-mock_network)
* [MOCK_NETWORK_CUSTOM](_transaction_transactioncontroller_test_.md#const-mock_network_custom)
* [MOCK_NETWORK_WITHOUT_CHAIN_ID](_transaction_transactioncontroller_test_.md#const-mock_network_without_chain_id)
* [MOCK_PRFERENCES](_transaction_transactioncontroller_test_.md#const-mock_prferences)
* [TOKEN_TX_HISTORY_DATA](_transaction_transactioncontroller_test_.md#const-token_tx_history_data)
* [TOKEN_TX_HISTORY_DATA_FROM_BLOCK](_transaction_transactioncontroller_test_.md#const-token_tx_history_data_from_block)
* [mockFlags](_transaction_transactioncontroller_test_.md#const-mockflags)

## Variables

### `Const` ETHER_TRANSACTION_HASH

• **ETHER_TRANSACTION_HASH**: *"0xa9d17df83756011ea63e1f0ca50a6627df7cac9806809e36680fcf4e88cb9dae"* = "0xa9d17df83756011ea63e1f0ca50a6627df7cac9806809e36680fcf4e88cb9dae"

Defined in transaction/TransactionController.test.ts:179

___

### `Const` ETH_TRANSACTIONS

• **ETH_TRANSACTIONS**: *(object | object)[]* = ethTxsMock(ETHER_TRANSACTION_HASH)

Defined in transaction/TransactionController.test.ts:182

___

### `Const` MAINNET_PROVIDER

• **MAINNET_PROVIDER**: *any* = new HttpProvider(
  'https://mainnet.infura.io/v3/341eacb578dd44a1a049cbc5f6fd4035',
)

Defined in transaction/TransactionController.test.ts:115

___

### `Const` PROVIDER

• **PROVIDER**: *any* = new HttpProvider(
  'https://ropsten.infura.io/v3/341eacb578dd44a1a049cbc5f6fd4035',
)

Defined in transaction/TransactionController.test.ts:112

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

• **TRANSACTIONS_IN_STATE**: *[TransactionMeta](_tx_.md#transactionmeta)[]* = txsInStateMock(
  ETHER_TRANSACTION_HASH,
  TOKEN_TRANSACTION_HASH,
)

Defined in transaction/TransactionController.test.ts:186

___

### `Const` TRANSACTIONS_IN_STATE_WITH_OUTDATED_GAS_DATA

• **TRANSACTIONS_IN_STATE_WITH_OUTDATED_GAS_DATA**: *[TransactionMeta](_tx_.md#transactionmeta)[]* = txsInStateWithOutdatedGasDataMock(
    ETHER_TRANSACTION_HASH,
    TOKEN_TRANSACTION_HASH,
  )

Defined in transaction/TransactionController.test.ts:197

___

### `Const` TRANSACTIONS_IN_STATE_WITH_OUTDATED_STATUS

• **TRANSACTIONS_IN_STATE_WITH_OUTDATED_STATUS**: *[TransactionMeta](_tx_.md#transactionmeta)[]* = txsInStateWithOutdatedStatusMock(
    ETHER_TRANSACTION_HASH,
    TOKEN_TRANSACTION_HASH,
  )

Defined in transaction/TransactionController.test.ts:191

___

### `Const` TRANSACTIONS_IN_STATE_WITH_OUTDATED_STATUS_AND_GAS_DATA

• **TRANSACTIONS_IN_STATE_WITH_OUTDATED_STATUS_AND_GAS_DATA**: *[TransactionMeta](_tx_.md#transactionmeta)[]* = txsInStateWithOutdatedStatusAndGasDataMock(
    ETHER_TRANSACTION_HASH,
    TOKEN_TRANSACTION_HASH,
  )

Defined in transaction/TransactionController.test.ts:203

___

### `Const` globalAny

• **globalAny**: *any* = global

Defined in transaction/TransactionController.test.ts:22

## Functions

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

### `Const` mockFlags

### ▪ **mockFlags**: *object*

Defined in transaction/TransactionController.test.ts:24

###  estimateGas

• **estimateGas**: *null* = null

Defined in transaction/TransactionController.test.ts:25
