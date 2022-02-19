[ethereum-gas-reference](../README.md) › [Globals](../globals.md) › [TransactionController](transactioncontroller.md)

# Class: TransactionController

Controller responsible for submitting and managing transactions

## Hierarchy

* any

  ↳ **TransactionController**

## Index

### Properties

* [ethQuery](transactioncontroller.md#private-ethquery)
* [handle](transactioncontroller.md#private-optional-handle)
* [mutex](transactioncontroller.md#private-mutex)
* [registry](transactioncontroller.md#private-registry)

### Methods

* [stopTransaction](transactioncontroller.md#stoptransaction)

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

▸ **stopTransaction**(`transactionID`: string, `gasValues?`: [GasPriceValue](../interfaces/gaspricevalue.md) | [FeeMarketEIP1559Values](../interfaces/feemarketeip1559values.md)): *Promise‹void›*

Defined in Tx.ts:284

Attempts to cancel a transaction based on its ID by setting its status to "rejected"
and emitting a `<tx.id>:finished` hub event.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`transactionID` | string | The ID of the transaction to cancel. |
`gasValues?` | [GasPriceValue](../interfaces/gaspricevalue.md) &#124; [FeeMarketEIP1559Values](../interfaces/feemarketeip1559values.md) | The gas values to use for the cancellation transation.  |

**Returns:** *Promise‹void›*
