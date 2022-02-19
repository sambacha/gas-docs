[ethereum-gas-reference](../README.md) › [Globals](../globals.md) › ["util"](_util_.md)

# Module: "util"

## Index

### Variables

* [hexRe](_util_.md#const-hexre)

### Functions

* [BNToHex](_util_.md#bntohex)
* [convertPriceToDecimal](_util_.md#const-convertpricetodecimal)
* [fractionBN](_util_.md#fractionbn)
* [fromHex](_util_.md#fromhex)
* [getBuyURL](_util_.md#getbuyurl)
* [getEtherscanApiUrl](_util_.md#getetherscanapiurl)
* [getIncreasedPriceFromExisting](_util_.md#const-getincreasedpricefromexisting)
* [getIncreasedPriceHex](_util_.md#const-getincreasedpricehex)
* [gweiDecToWEIBN](_util_.md#gweidectoweibn)
* [handleFetch](_util_.md#handlefetch)
* [handleTransactionFetch](_util_.md#handletransactionfetch)
* [hexToBN](_util_.md#hextobn)
* [hexToText](_util_.md#hextotext)
* [isEIP1559Transaction](_util_.md#const-iseip1559transaction)
* [isFeeMarketEIP1559Values](_util_.md#const-isfeemarketeip1559values)
* [isGasPriceValue](_util_.md#const-isgaspricevalue)
* [isValidHexAddress](_util_.md#isvalidhexaddress)
* [normalizeEnsName](_util_.md#normalizeensname)
* [normalizeMessageData](_util_.md#normalizemessagedata)
* [normalizeTransaction](_util_.md#normalizetransaction)
* [query](_util_.md#query)
* [safelyExecute](_util_.md#safelyexecute)
* [safelyExecuteWithTimeout](_util_.md#safelyexecutewithtimeout)
* [successfulFetch](_util_.md#successfulfetch)
* [timeoutFetch](_util_.md#timeoutfetch)
* [toChecksumHexAddress](_util_.md#tochecksumhexaddress)
* [toHex](_util_.md#tohex)
* [validateGasValues](_util_.md#const-validategasvalues)
* [validateMinimumIncrease](_util_.md#validateminimumincrease)
* [validateSignMessageData](_util_.md#validatesignmessagedata)
* [validateTransaction](_util_.md#validatetransaction)
* [validateTypedSignMessageDataV1](_util_.md#validatetypedsignmessagedatav1)
* [validateTypedSignMessageDataV3](_util_.md#validatetypedsignmessagedatav3)
* [weiHexToGweiDec](_util_.md#weihextogweidec)

### Object literals

* [NORMALIZERS](_util_.md#const-normalizers)

## Variables

### `Const` hexRe

• **hexRe**: *RegExp‹›* = /^[0-9A-Fa-f]+$/gu

Defined in util.ts:28

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

### `Const` convertPriceToDecimal

▸ **convertPriceToDecimal**(`value`: string | undefined): *number*

Defined in util.ts:703

**Parameters:**

Name | Type |
------ | ------ |
`value` | string &#124; undefined |

**Returns:** *number*

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

▸ **handleTransactionFetch**(`networkType`: string, `address`: string, `txHistoryLimit`: number, `opt?`: [FetchAllOptions](../interfaces/_tx_.fetchalloptions.md)): *Promise‹[object, object]›*

Defined in util.ts:185

Handles the fetch of incoming transactions.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`networkType` | string | Network type of desired network. |
`address` | string | Address to get the transactions from. |
`txHistoryLimit` | number | The maximum number of transactions to fetch. |
`opt?` | [FetchAllOptions](../interfaces/_tx_.fetchalloptions.md) | Object that can contain fromBlock and Etherscan service API key. |

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

▸ **isEIP1559Transaction**(`transaction`: [Transaction](../interfaces/_tx_.transaction.md)): *boolean*

Defined in util.ts:694

Checks if a transaction is EIP-1559 by checking for the existence of
maxFeePerGas and maxPriorityFeePerGas within its parameters.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`transaction` | [Transaction](../interfaces/_tx_.transaction.md) | Transaction object to add. |

**Returns:** *boolean*

Boolean that is true if the transaction is EIP-1559 (has maxFeePerGas and maxPriorityFeePerGas), otherwise returns false.

___

### `Const` isFeeMarketEIP1559Values

▸ **isFeeMarketEIP1559Values**(`gasValues?`: [GasPriceValue](../interfaces/_tx_.gaspricevalue.md) | [FeeMarketEIP1559Values](../interfaces/_tx_.feemarketeip1559values.md)): *gasValues is FeeMarketEIP1559Values*

Defined in util.ts:729

**Parameters:**

Name | Type |
------ | ------ |
`gasValues?` | [GasPriceValue](../interfaces/_tx_.gaspricevalue.md) &#124; [FeeMarketEIP1559Values](../interfaces/_tx_.feemarketeip1559values.md) |

**Returns:** *gasValues is FeeMarketEIP1559Values*

___

### `Const` isGasPriceValue

▸ **isGasPriceValue**(`gasValues?`: [GasPriceValue](../interfaces/_tx_.gaspricevalue.md) | [FeeMarketEIP1559Values](../interfaces/_tx_.feemarketeip1559values.md)): *gasValues is GasPriceValue*

Defined in util.ts:735

**Parameters:**

Name | Type |
------ | ------ |
`gasValues?` | [GasPriceValue](../interfaces/_tx_.gaspricevalue.md) &#124; [FeeMarketEIP1559Values](../interfaces/_tx_.feemarketeip1559values.md) |

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

▸ **normalizeTransaction**(`transaction`: [Transaction](../interfaces/_tx_.transaction.md)): *[Transaction](../interfaces/_tx_.transaction.md)*

Defined in util.ts:301

Normalizes properties on a Transaction object.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`transaction` | [Transaction](../interfaces/_tx_.transaction.md) | Transaction object to normalize. |

**Returns:** *[Transaction](../interfaces/_tx_.transaction.md)*

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

### `Const` validateGasValues

▸ **validateGasValues**(`gasValues`: [GasPriceValue](../interfaces/_tx_.gaspricevalue.md) | [FeeMarketEIP1559Values](../interfaces/_tx_.feemarketeip1559values.md)): *void*

Defined in util.ts:716

**Parameters:**

Name | Type |
------ | ------ |
`gasValues` | [GasPriceValue](../interfaces/_tx_.gaspricevalue.md) &#124; [FeeMarketEIP1559Values](../interfaces/_tx_.feemarketeip1559values.md) |

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

▸ **validateSignMessageData**(`messageData`: [PersonalMessageParams](../interfaces/_message_manager_personalmessagemanager_.personalmessageparams.md) | [MessageParams](../interfaces/_message_manager_messagemanager_.messageparams.md)): *void*

Defined in util.ts:498

Validates a PersonalMessageParams and MessageParams objects for required properties and throws in
the event of any validation error.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`messageData` | [PersonalMessageParams](../interfaces/_message_manager_personalmessagemanager_.personalmessageparams.md) &#124; [MessageParams](../interfaces/_message_manager_messagemanager_.messageparams.md) | PersonalMessageParams object to validate.  |

**Returns:** *void*

___

###  validateTransaction

▸ **validateTransaction**(`transaction`: [Transaction](../interfaces/_tx_.transaction.md)): *void*

Defined in util.ts:420

Validates a Transaction object for required properties and throws in
the event of any validation error.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`transaction` | [Transaction](../interfaces/_tx_.transaction.md) | Transaction object to validate.  |

**Returns:** *void*

___

###  validateTypedSignMessageDataV1

▸ **validateTypedSignMessageDataV1**(`messageData`: [TypedMessageParams](../interfaces/_message_manager_typedmessagemanager_.typedmessageparams.md)): *void*

Defined in util.ts:517

Validates a TypedMessageParams object for required properties and throws in
the event of any validation error for eth_signTypedMessage_V1.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`messageData` | [TypedMessageParams](../interfaces/_message_manager_typedmessagemanager_.typedmessageparams.md) | TypedMessageParams object to validate.  |

**Returns:** *void*

___

###  validateTypedSignMessageDataV3

▸ **validateTypedSignMessageDataV3**(`messageData`: [TypedMessageParams](../interfaces/_message_manager_typedmessagemanager_.typedmessageparams.md)): *void*

Defined in util.ts:550

Validates a TypedMessageParams object for required properties and throws in
the event of any validation error for eth_signTypedMessage_V3.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`messageData` | [TypedMessageParams](../interfaces/_message_manager_typedmessagemanager_.typedmessageparams.md) | TypedMessageParams object to validate.  |

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
