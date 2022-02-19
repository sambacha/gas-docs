[ethereum-gas-reference](../README.md) › [Globals](../globals.md) › ["message-manager/TypedMessageManager"](../modules/_message_manager_typedmessagemanager_.md) › [TypedMessage](_message_manager_typedmessagemanager_.typedmessage.md)

# Interface: TypedMessage

**`property`** id - An id to track and identify the message object

**`property`** error - Error corresponding to eth_signTypedData error in failure case

**`property`** messageParams - The parameters to pass to the eth_signTypedData method once
the signature request is approved

**`property`** type - The json-prc signing method for which a signature request has been made.
A 'TypedMessage' which always has a 'eth_signTypedData' type

**`property`** rawSig - Raw data of the signature request

## Hierarchy

* [AbstractMessage](_message_manager_abstractmessagemanager_.abstractmessage.md)

  ↳ **TypedMessage**

## Index

### Properties

* [error](_message_manager_typedmessagemanager_.typedmessage.md#optional-error)
* [id](_message_manager_typedmessagemanager_.typedmessage.md#id)
* [messageParams](_message_manager_typedmessagemanager_.typedmessage.md#messageparams)
* [rawSig](_message_manager_typedmessagemanager_.typedmessage.md#optional-rawsig)
* [status](_message_manager_typedmessagemanager_.typedmessage.md#status)
* [time](_message_manager_typedmessagemanager_.typedmessage.md#time)
* [type](_message_manager_typedmessagemanager_.typedmessage.md#type)

## Properties

### `Optional` error

• **error**? : *string*

Defined in message-manager/TypedMessageManager.ts:28

___

###  id

• **id**: *string*

*Inherited from [AbstractMessage](_message_manager_abstractmessagemanager_.abstractmessage.md).[id](_message_manager_abstractmessagemanager_.abstractmessage.md#id)*

Defined in message-manager/AbstractMessageManager.ts:24

___

###  messageParams

• **messageParams**: *[TypedMessageParams](_message_manager_typedmessagemanager_.typedmessageparams.md)*

Defined in message-manager/TypedMessageManager.ts:29

___

### `Optional` rawSig

• **rawSig**? : *string*

*Overrides [AbstractMessage](_message_manager_abstractmessagemanager_.abstractmessage.md).[rawSig](_message_manager_abstractmessagemanager_.abstractmessage.md#optional-rawsig)*

Defined in message-manager/TypedMessageManager.ts:33

___

###  status

• **status**: *string*

*Overrides [AbstractMessage](_message_manager_abstractmessagemanager_.abstractmessage.md).[status](_message_manager_abstractmessagemanager_.abstractmessage.md#status)*

Defined in message-manager/TypedMessageManager.ts:31

___

###  time

• **time**: *number*

*Overrides [AbstractMessage](_message_manager_abstractmessagemanager_.abstractmessage.md).[time](_message_manager_abstractmessagemanager_.abstractmessage.md#time)*

Defined in message-manager/TypedMessageManager.ts:30

___

###  type

• **type**: *string*

*Overrides [AbstractMessage](_message_manager_abstractmessagemanager_.abstractmessage.md).[type](_message_manager_abstractmessagemanager_.abstractmessage.md#type)*

Defined in message-manager/TypedMessageManager.ts:32
