[metamask-controllers-main-src-gas-2](../README.md) › [Globals](../globals.md) › ["message-manager/AbstractMessageManager"](../modules/_message_manager_abstractmessagemanager_.md) › [AbstractMessage](_message_manager_abstractmessagemanager_.abstractmessage.md)

# Interface: AbstractMessage

**`property`** id - An id to track and identify the message object

**`property`** type - The json-prc signing method for which a signature request has been made.
A 'Message' which always has a signing type

**`property`** rawSig - Raw data of the signature request

## Hierarchy

* **AbstractMessage**

  ↳ [Message](_message_manager_messagemanager_.message.md)

  ↳ [PersonalMessage](_message_manager_personalmessagemanager_.personalmessage.md)

  ↳ [TypedMessage](_message_manager_typedmessagemanager_.typedmessage.md)

## Index

### Properties

* [id](_message_manager_abstractmessagemanager_.abstractmessage.md#id)
* [rawSig](_message_manager_abstractmessagemanager_.abstractmessage.md#optional-rawsig)
* [status](_message_manager_abstractmessagemanager_.abstractmessage.md#status)
* [time](_message_manager_abstractmessagemanager_.abstractmessage.md#time)
* [type](_message_manager_abstractmessagemanager_.abstractmessage.md#type)

## Properties

###  id

• **id**: *string*

Defined in message-manager/AbstractMessageManager.ts:24

___

### `Optional` rawSig

• **rawSig**? : *string*

Defined in message-manager/AbstractMessageManager.ts:28

___

###  status

• **status**: *string*

Defined in message-manager/AbstractMessageManager.ts:26

___

###  time

• **time**: *number*

Defined in message-manager/AbstractMessageManager.ts:25

___

###  type

• **type**: *string*

Defined in message-manager/AbstractMessageManager.ts:27
