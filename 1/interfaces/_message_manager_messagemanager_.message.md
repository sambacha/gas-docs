[ethereum-gas-reference](../README.md) › [Globals](../globals.md) › ["message-manager/MessageManager"](../modules/_message_manager_messagemanager_.md) › [Message](_message_manager_messagemanager_.message.md)

# Interface: Message

**`property`** id - An id to track and identify the message object

**`property`** messageParams - The parameters to pass to the eth_sign method once the signature request is approved

**`property`** type - The json-prc signing method for which a signature request has been made.
A 'Message' which always has a 'eth_sign' type

**`property`** rawSig - Raw data of the signature request

## Hierarchy

* [AbstractMessage](_message_manager_abstractmessagemanager_.abstractmessage.md)

  ↳ **Message**

## Index

### Properties

* [id](_message_manager_messagemanager_.message.md#id)
* [messageParams](_message_manager_messagemanager_.message.md#messageparams)
* [rawSig](_message_manager_messagemanager_.message.md#optional-rawsig)
* [status](_message_manager_messagemanager_.message.md#status)
* [time](_message_manager_messagemanager_.message.md#time)
* [type](_message_manager_messagemanager_.message.md#type)

## Properties

###  id

• **id**: *string*

*Inherited from [AbstractMessage](_message_manager_abstractmessagemanager_.abstractmessage.md).[id](_message_manager_abstractmessagemanager_.abstractmessage.md#id)*

Defined in message-manager/AbstractMessageManager.ts:24

___

###  messageParams

• **messageParams**: *[MessageParams](_message_manager_messagemanager_.messageparams.md)*

Defined in message-manager/MessageManager.ts:23

___

### `Optional` rawSig

• **rawSig**? : *string*

*Inherited from [AbstractMessage](_message_manager_abstractmessagemanager_.abstractmessage.md).[rawSig](_message_manager_abstractmessagemanager_.abstractmessage.md#optional-rawsig)*

Defined in message-manager/AbstractMessageManager.ts:28

___

###  status

• **status**: *string*

*Inherited from [AbstractMessage](_message_manager_abstractmessagemanager_.abstractmessage.md).[status](_message_manager_abstractmessagemanager_.abstractmessage.md#status)*

Defined in message-manager/AbstractMessageManager.ts:26

___

###  time

• **time**: *number*

*Inherited from [AbstractMessage](_message_manager_abstractmessagemanager_.abstractmessage.md).[time](_message_manager_abstractmessagemanager_.abstractmessage.md#time)*

Defined in message-manager/AbstractMessageManager.ts:25

___

###  type

• **type**: *string*

*Inherited from [AbstractMessage](_message_manager_abstractmessagemanager_.abstractmessage.md).[type](_message_manager_abstractmessagemanager_.abstractmessage.md#type)*

Defined in message-manager/AbstractMessageManager.ts:27
