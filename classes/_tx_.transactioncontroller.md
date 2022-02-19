[metamask-controllers-main-src-gas-2](../README.md) › [Globals](../globals.md) › ["Tx"](../modules/_tx_.md) › [TransactionController](_tx_.transactioncontroller.md)

# Class: TransactionController

Controller responsible for submitting and managing transactions

## Hierarchy

* any

  ↳ **TransactionController**

## Index

### Properties

* [ethQuery](_tx_.transactioncontroller.md#private-ethquery)
* [handle](_tx_.transactioncontroller.md#private-optional-handle)
* [mutex](_tx_.transactioncontroller.md#private-mutex)
* [registry](_tx_.transactioncontroller.md#private-registry)

### Methods

* [stopTransaction](_tx_.transactioncontroller.md#stoptransaction)

## Properties

### `Private` ethQuery

• **ethQuery**: *any*

Defined in Tx.ts:269

___

### `Private` `Optional` handle

• **handle**? : *Timer*

Defined in Tx.ts:273

___

### `Private` mutex

• **mutex**: *Mutex‹›* = new Mutex()

Defined in Tx.ts:275

___

### `Private` registry

• **registry**: *any*

Defined in Tx.ts:271

## Methods

###  stopTransaction

▸ **stopTransaction**(`transactionID`: string, `gasValues?`: [GasPriceValue](../interfaces/_tx_.gaspricevalue.md) | [FeeMarketEIP1559Values](../interfaces/_tx_.feemarketeip1559values.md)): *Promise‹void›*

Defined in Tx.ts:284

Attempts to cancel a transaction based on its ID by setting its status to "rejected"
and emitting a `<tx.id>:finished` hub event.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`transactionID` | string | The ID of the transaction to cancel. |
`gasValues?` | [GasPriceValue](../interfaces/_tx_.gaspricevalue.md) &#124; [FeeMarketEIP1559Values](../interfaces/_tx_.feemarketeip1559values.md) | The gas values to use for the cancellation transation.  |

**Returns:** *Promise‹void›*
