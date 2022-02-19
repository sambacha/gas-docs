[metamask-controllers-main-src-gas-2](../README.md) › [Globals](../globals.md) › ["message-manager/AbstractMessageManager.test"](_message_manager_abstractmessagemanager_test_.md)

# Module: "message-manager/AbstractMessageManager.test"

## Index

### Classes

* [AbstractTestManager](../classes/_message_manager_abstractmessagemanager_test_.abstracttestmanager.md)

### Variables

* [from](_message_manager_abstractmessagemanager_test_.md#const-from)
* [messageData](_message_manager_abstractmessagemanager_test_.md#const-messagedata)
* [messageId](_message_manager_abstractmessagemanager_test_.md#const-messageid)
* [messageStatus](_message_manager_abstractmessagemanager_test_.md#const-messagestatus)
* [messageTime](_message_manager_abstractmessagemanager_test_.md#const-messagetime)
* [messageType](_message_manager_abstractmessagemanager_test_.md#const-messagetype)
* [typedMessage](_message_manager_abstractmessagemanager_test_.md#const-typedmessage)

## Variables

### `Const` from

• **from**: *"0x0123"* = "0x0123"

Defined in message-manager/AbstractMessageManager.test.ts:38

___

### `Const` messageData

• **messageData**: *object[]* = typedMessage

Defined in message-manager/AbstractMessageManager.test.ts:42

___

### `Const` messageId

• **messageId**: *"1"* = "1"

Defined in message-manager/AbstractMessageManager.test.ts:37

___

### `Const` messageStatus

• **messageStatus**: *"unapproved"* = "unapproved"

Defined in message-manager/AbstractMessageManager.test.ts:40

___

### `Const` messageTime

• **messageTime**: *number* = Date.now()

Defined in message-manager/AbstractMessageManager.test.ts:39

___

### `Const` messageType

• **messageType**: *"eth_signTypedData"* = "eth_signTypedData"

Defined in message-manager/AbstractMessageManager.test.ts:41

___

### `Const` typedMessage

• **typedMessage**: *object[]* = [
  {
    name: 'Message',
    type: 'string',
    value: 'Hi, Alice!',
  },
  {
    name: 'A number',
    type: 'uint32',
    value: '1337',
  },
]

Defined in message-manager/AbstractMessageManager.test.ts:25
