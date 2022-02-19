[ethereum-gas-reference](../README.md) › [Globals](../globals.md) › ["message-manager/AbstractMessageManager"](../modules/_message_manager_abstractmessagemanager_.md) › [MessageManagerState](_message_manager_abstractmessagemanager_.messagemanagerstate.md)

# Interface: MessageManagerState ‹**M**›

**`property`** unapprovedMessages - A collection of all Messages in the 'unapproved' state

**`property`** unapprovedMessagesCount - The count of all Messages in this.unapprovedMessages

## Type parameters

▪ **M**: *[AbstractMessage](_message_manager_abstractmessagemanager_.abstractmessage.md)*

## Hierarchy

* [BaseState](_basecontroller_.basestate.md)

  ↳ **MessageManagerState**

## Index

### Properties

* [name](_message_manager_abstractmessagemanager_.messagemanagerstate.md#optional-name)
* [unapprovedMessages](_message_manager_abstractmessagemanager_.messagemanagerstate.md#unapprovedmessages)
* [unapprovedMessagesCount](_message_manager_abstractmessagemanager_.messagemanagerstate.md#unapprovedmessagescount)

## Properties

### `Optional` name

• **name**? : *string*

*Inherited from [BaseState](_basecontroller_.basestate.md).[name](_basecontroller_.basestate.md#optional-name)*

Defined in BaseController.ts:23

___

###  unapprovedMessages

• **unapprovedMessages**: *object*

Defined in message-manager/AbstractMessageManager.ts:65

#### Type declaration:

* \[ **key**: *string*\]: M

___

###  unapprovedMessagesCount

• **unapprovedMessagesCount**: *number*

Defined in message-manager/AbstractMessageManager.ts:66
