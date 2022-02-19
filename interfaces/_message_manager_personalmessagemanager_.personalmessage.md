[metamask-controllers-main-src-gas-2](../README.md) › [Globals](../globals.md) › ["message-manager/PersonalMessageManager"](../modules/_message_manager_personalmessagemanager_.md) › [PersonalMessage](_message_manager_personalmessagemanager_.personalmessage.md)

# Interface: PersonalMessage

**`property`** id - An id to track and identify the message object

**`property`** messageParams - The parameters to pass to the personal_sign method once the signature request is approved

**`property`** type - The json-prc signing method for which a signature request has been made.
A 'Message' which always has a 'personal_sign' type

**`property`** rawSig - Raw data of the signature request

## Hierarchy

* [AbstractMessage](_message_manager_abstractmessagemanager_.abstractmessage.md)

  ↳ **PersonalMessage**

## Index

### Properties

* [id](_message_manager_personalmessagemanager_.personalmessage.md#id)
* [messageParams](_message_manager_personalmessagemanager_.personalmessage.md#messageparams)
* [rawSig](_message_manager_personalmessagemanager_.personalmessage.md#optional-rawsig)
* [status](_message_manager_personalmessagemanager_.personalmessage.md#status)
* [time](_message_manager_personalmessagemanager_.personalmessage.md#time)
* [type](_message_manager_personalmessagemanager_.personalmessage.md#type)

## Properties

###  id

• **id**: *string*

*Inherited from [AbstractMessage](_message_manager_abstractmessagemanager_.abstractmessage.md).[id](_message_manager_abstractmessagemanager_.abstractmessage.md#id)*

Defined in message-manager/AbstractMessageManager.ts:24

___

###  messageParams

• **messageParams**: *[PersonalMessageParams](_message_manager_personalmessagemanager_.personalmessageparams.md)*

Defined in message-manager/PersonalMessageManager.ts:23

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
