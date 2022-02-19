[ethereum-gas-reference](../README.md) › [Globals](../globals.md) › ["message-manager/TypedMessageManager"](../modules/_message_manager_typedmessagemanager_.md) › [TypedMessageParamsMetamask](_message_manager_typedmessagemanager_.typedmessageparamsmetamask.md)

# Interface: TypedMessageParamsMetamask

**`property`** metamaskId - Added for tracking and identification within MetaMask

**`property`** data - A hex string conversion of the raw buffer or an object containing data of the signature
request depending on version

**`property`** error? - Added for message errored

**`property`** from - Address to sign this message from

**`property`** origin? - Added for request origin identification

**`property`** version - Compatibility version EIP712

## Hierarchy

  ↳ [AbstractMessageParamsMetamask](_message_manager_abstractmessagemanager_.abstractmessageparamsmetamask.md)

  ↳ **TypedMessageParamsMetamask**

## Index

### Properties

* [data](_message_manager_typedmessagemanager_.typedmessageparamsmetamask.md#data)
* [error](_message_manager_typedmessagemanager_.typedmessageparamsmetamask.md#optional-error)
* [from](_message_manager_typedmessagemanager_.typedmessageparamsmetamask.md#from)
* [metamaskId](_message_manager_typedmessagemanager_.typedmessageparamsmetamask.md#optional-metamaskid)
* [origin](_message_manager_typedmessagemanager_.typedmessageparamsmetamask.md#optional-origin)
* [version](_message_manager_typedmessagemanager_.typedmessageparamsmetamask.md#optional-version)

## Properties

###  data

• **data**: *Record‹string, unknown›[] | string*

Defined in message-manager/TypedMessageManager.ts:64

___

### `Optional` error

• **error**? : *string*

Defined in message-manager/TypedMessageManager.ts:66

___

###  from

• **from**: *string*

*Inherited from [AbstractMessageParams](_message_manager_abstractmessagemanager_.abstractmessageparams.md).[from](_message_manager_abstractmessagemanager_.abstractmessageparams.md#from)*

Defined in message-manager/AbstractMessageManager.ts:39

___

### `Optional` metamaskId

• **metamaskId**? : *string*

*Overrides [AbstractMessageParamsMetamask](_message_manager_abstractmessagemanager_.abstractmessageparamsmetamask.md).[metamaskId](_message_manager_abstractmessagemanager_.abstractmessageparamsmetamask.md#optional-metamaskid)*

Defined in message-manager/TypedMessageManager.ts:65

___

### `Optional` origin

• **origin**? : *string*

*Inherited from [AbstractMessageParams](_message_manager_abstractmessagemanager_.abstractmessageparams.md).[origin](_message_manager_abstractmessagemanager_.abstractmessageparams.md#optional-origin)*

Defined in message-manager/AbstractMessageManager.ts:40

___

### `Optional` version

• **version**? : *string*

Defined in message-manager/TypedMessageManager.ts:67
