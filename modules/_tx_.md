[metamask-controllers-main-src-gas-2](../README.md) › [Globals](../globals.md) › ["Tx"](_tx_.md)

# Module: "Tx"

## Index

### Enumerations

* [TransactionStatus](../enums/_tx_.transactionstatus.md)
* [WalletDevice](../enums/_tx_.walletdevice.md)

### Classes

* [TransactionController](../classes/_tx_.transactioncontroller.md)

### Interfaces

* [EtherscanTransactionMeta](../interfaces/_tx_.etherscantransactionmeta.md)
* [FeeMarketEIP1559Values](../interfaces/_tx_.feemarketeip1559values.md)
* [FetchAllOptions](../interfaces/_tx_.fetchalloptions.md)
* [GasPriceValue](../interfaces/_tx_.gaspricevalue.md)
* [MethodData](../interfaces/_tx_.methoddata.md)
* [Result](../interfaces/_tx_.result.md)
* [Transaction](../interfaces/_tx_.transaction.md)
* [TransactionConfig](../interfaces/_tx_.transactionconfig.md)
* [TransactionState](../interfaces/_tx_.transactionstate.md)

### Type aliases

* [TransactionMeta](_tx_.md#transactionmeta)
* [TransactionMetaBase](_tx_.md#transactionmetabase)

### Variables

* [CANCEL_RATE](_tx_.md#const-cancel_rate)
* [HARDFORK](_tx_.md#const-hardfork)
* [SPEED_UP_RATE](_tx_.md#const-speed_up_rate)
* [hub](_tx_.md#const-hub)
* [name](_tx_.md#const-name)

## Type aliases

###  TransactionMeta

Ƭ **TransactionMeta**: *object & [TransactionMetaBase](_tx_.md#transactionmetabase) | object & [TransactionMetaBase](_tx_.md#transactionmetabase)*

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

* **deviceConfirmedOn**? : *[WalletDevice](../enums/_tx_.walletdevice.md)*

* **id**: *string*

* **isTransfer**? : *boolean*

* **networkID**? : *string*

* **origin**? : *string*

* **rawTransaction**? : *string*

* **time**: *number*

* **toSmartContract**? : *boolean*

* **transaction**: *[Transaction](../interfaces/_tx_.transaction.md)*

* **transactionHash**? : *string*

* **transferInformation**(): *object*

  * **contractAddress**: *string*

  * **decimals**: *number*

  * **symbol**: *string*

* **verifiedOnBlockchain**? : *boolean*

## Variables

### `Const` CANCEL_RATE

• **CANCEL_RATE**: *1.5* = 1.5

Defined in Tx.ts:255

Multiplier used to determine a transaction's increased gas fee during cancellation

___

### `Const` HARDFORK

• **HARDFORK**: *"london"* = "london"

Defined in Tx.ts:31

___

### `Const` SPEED_UP_RATE

• **SPEED_UP_RATE**: *1.1* = 1.1

Defined in Tx.ts:260

Multiplier used to determine a transaction's increased gas fee during speed up

___

### `Const` hub

• **hub**: *EventEmitter‹›* = new EventEmitter()

Defined in Tx.ts:36

EventEmitter instance used to listen to specific transactional events

___

### `Const` name

• **name**: *"TransactionController"* = "TransactionController"

Defined in Tx.ts:41

Name of this controller used during composition
