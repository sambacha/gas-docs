[ethereum-gas-reference](../README.md) › [Globals](../globals.md) › ["fetchBlockFeeHistory.test"](_fetchblockfeehistory_test_.md)

# Module: "fetchBlockFeeHistory.test"

## Index

### Variables

* [mockedQuery](_fetchblockfeehistory_test_.md#const-mockedquery)

### Functions

* [times](_fetchblockfeehistory_test_.md#times)

## Variables

### `Const` mockedQuery

• **mockedQuery**: *any* = mocked(query, true)

Defined in fetchBlockFeeHistory.test.ts:15

## Functions

###  times

▸ **times**‹**T**›(`n`: number, `fn`: function): *T[]*

Defined in fetchBlockFeeHistory.test.ts:24

Calls the given function the given number of times, collecting the results from each call.

**Type parameters:**

▪ **T**

**Parameters:**

▪ **n**: *number*

The number of times you want to call the function.

▪ **fn**: *function*

The function to call.

▸ (`n`: number): *T*

**Parameters:**

Name | Type |
------ | ------ |
`n` | number |

**Returns:** *T[]*

An array of values gleaned from the results of each call to the function.
