[ethereum-gas-reference](../README.md) › [Globals](../globals.md) › ["message-manager/MessageManager"](../modules/_message_manager_messagemanager_.md) › [MessageParamsMetamask](_message_manager_messagemanager_.messageparamsmetamask.md)

# Interface: MessageParamsMetamask

**`property`** metamaskId - Added for tracking and identification within MetaMask

**`property`** data - A hex string conversion of the raw buffer data of the signature request

**`property`** from - Address to sign this message from

**`property`** origin? - Added for request origin identification

## Hierarchy

  ↳ [AbstractMessageParamsMetamask](_message_manager_abstractmessagemanager_.abstractmessageparamsmetamask.md)

  ↳ **MessageParamsMetamask**

## Index

### Properties

* [data](_message_manager_messagemanager_.messageparamsmetamask.md#data)
* [from](_message_manager_messagemanager_.messageparamsmetamask.md#from)
* [metamaskId](_message_manager_messagemanager_.messageparamsmetamask.md#optional-metamaskid)
* [origin](_message_manager_messagemanager_.messageparamsmetamask.md#optional-origin)

## Properties

###  data

• **data**: *string*

Defined in message-manager/MessageManager.ts:49

___

###  from

• **from**: *string*

*Inherited from [AbstractMessageParams](_message_manager_abstractmessagemanager_.abstractmessageparams.md).[from](_message_manager_abstractmessagemanager_.abstractmessageparams.md#from)*

Defined in message-manager/AbstractMessageManager.ts:39

___

### `Optional` metamaskId

• **metamaskId**? : *string*

*Inherited from [AbstractMessageParamsMetamask](_message_manager_abstractmessagemanager_.abstractmessageparamsmetamask.md).[metamaskId](_message_manager_abstractmessagemanager_.abstractmessageparamsmetamask.md#optional-metamaskid)*

Defined in message-manager/AbstractMessageManager.ts:53

___

### `Optional` origin

• **origin**? : *string*

*Inherited from [AbstractMessageParams](_message_manager_abstractmessagemanager_.abstractmessageparams.md).[origin](_message_manager_abstractmessagemanager_.abstractmessageparams.md#optional-origin)*

Defined in message-manager/AbstractMessageManager.ts:40
