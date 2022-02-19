[ethereum-gas-reference](../README.md) › [Globals](../globals.md) › ["message-manager/TypedMessageManager"](../modules/_message_manager_typedmessagemanager_.md) › [TypedMessageParams](_message_manager_typedmessagemanager_.typedmessageparams.md)

# Interface: TypedMessageParams

**`property`** data - A hex string conversion of the raw buffer or an object containing data of the signature
request depending on version

**`property`** from - Address to sign this message from

**`property`** origin? - Added for request origin identification

## Hierarchy

* [AbstractMessageParams](_message_manager_abstractmessagemanager_.abstractmessageparams.md)

  ↳ **TypedMessageParams**

## Index

### Properties

* [data](_message_manager_typedmessagemanager_.typedmessageparams.md#data)
* [from](_message_manager_typedmessagemanager_.typedmessageparams.md#from)
* [origin](_message_manager_typedmessagemanager_.typedmessageparams.md#optional-origin)

## Properties

###  data

• **data**: *Record‹string, unknown›[] | string*

Defined in message-manager/TypedMessageManager.ts:46

___

###  from

• **from**: *string*

*Inherited from [AbstractMessageParams](_message_manager_abstractmessagemanager_.abstractmessageparams.md).[from](_message_manager_abstractmessagemanager_.abstractmessageparams.md#from)*

Defined in message-manager/AbstractMessageManager.ts:39

___

### `Optional` origin

• **origin**? : *string*

*Inherited from [AbstractMessageParams](_message_manager_abstractmessagemanager_.abstractmessageparams.md).[origin](_message_manager_abstractmessagemanager_.abstractmessageparams.md#optional-origin)*

Defined in message-manager/AbstractMessageManager.ts:40
