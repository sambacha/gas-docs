[ethereum-gas-reference](../README.md) › [Globals](../globals.md) › [TransactionConfig](transactionconfig.md)

# Interface: TransactionConfig

**`property`** interval - Polling interval used to fetch new currency rate

**`property`** provider - Provider used to create a new underlying EthQuery instance

**`property`** sign - Method used to sign transactions

## Hierarchy

* any

  ↳ **TransactionConfig**

## Index

### Properties

* [interval](transactionconfig.md#interval)
* [sign](transactionconfig.md#optional-sign)
* [txHistoryLimit](transactionconfig.md#txhistorylimit)

## Properties

###  interval

• **interval**: *number*

Defined in Tx.ts:223

___

### `Optional` sign

• **sign**? : *function*

Defined in Tx.ts:224

#### Type declaration:

▸ (`transaction`: [Transaction](transaction.md), `from`: string): *Promise‹any›*

**Parameters:**

Name | Type |
------ | ------ |
`transaction` | [Transaction](transaction.md) |
`from` | string |

___

###  txHistoryLimit

• **txHistoryLimit**: *number*

Defined in Tx.ts:225
