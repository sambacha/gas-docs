[ethereum-gas-reference](../README.md) › [Globals](../globals.md) › ["gas-util.test"](_gas_util_test_.md)

# Module: "gas-util.test"

## Index

### Variables

* [mockEIP1559ApiResponses](_gas_util_test_.md#const-mockeip1559apiresponses)

## Variables

### `Const` mockEIP1559ApiResponses

• **mockEIP1559ApiResponses**: *object[]* = [
  {
    low: {
      minWaitTimeEstimate: 120000,
      maxWaitTimeEstimate: 300000,
      suggestedMaxPriorityFeePerGas: '1',
      suggestedMaxFeePerGas: '35',
    },
    medium: {
      minWaitTimeEstimate: 0,
      maxWaitTimeEstimate: 30000,
      suggestedMaxPriorityFeePerGas: '2',
      suggestedMaxFeePerGas: '40',
    },
    high: {
      minWaitTimeEstimate: 0,
      maxWaitTimeEstimate: 15000,
      suggestedMaxPriorityFeePerGas: '3',
      suggestedMaxFeePerGas: '60',
    },
    estimatedBaseFee: '30',
  },
  {
    low: {
      minWaitTimeEstimate: 180000,
      maxWaitTimeEstimate: 360000,
      suggestedMaxPriorityFeePerGas: '1.0000000162',
      suggestedMaxFeePerGas: '40',
    },
    medium: {
      minWaitTimeEstimate: 15000,
      maxWaitTimeEstimate: 60000,
      suggestedMaxPriorityFeePerGas: '1.0000000160000028',
      suggestedMaxFeePerGas: '45',
    },
    high: {
      minWaitTimeEstimate: 0,
      maxWaitTimeEstimate: 15000,
      suggestedMaxPriorityFeePerGas: '3',
      suggestedMaxFeePerGas: '1.000000016522',
    },
    estimatedBaseFee: '32.000000016522',
  },
]

Defined in gas-util.test.ts:8
