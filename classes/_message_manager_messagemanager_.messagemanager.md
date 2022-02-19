[metamask-controllers-main-src-gas-2](../README.md) › [Globals](../globals.md) › ["message-manager/MessageManager"](../modules/_message_manager_messagemanager_.md) › [MessageManager](_message_manager_messagemanager_.messagemanager.md)

# Class: MessageManager

Controller in charge of managing - storing, adding, removing, updating - Messages.

## Hierarchy

  ↳ [AbstractMessageManager](_message_manager_abstractmessagemanager_.abstractmessagemanager.md)‹[Message](../interfaces/_message_manager_messagemanager_.message.md), [MessageParams](../interfaces/_message_manager_messagemanager_.messageparams.md), [MessageParamsMetamask](../interfaces/_message_manager_messagemanager_.messageparamsmetamask.md)›

  ↳ **MessageManager**

## Index

### Constructors

* [constructor](_message_manager_messagemanager_.messagemanager.md#constructor)

### Properties

* [defaultConfig](_message_manager_messagemanager_.messagemanager.md#defaultconfig)
* [defaultState](_message_manager_messagemanager_.messagemanager.md#defaultstate)
* [disabled](_message_manager_messagemanager_.messagemanager.md#disabled)
* [hub](_message_manager_messagemanager_.messagemanager.md#hub)
* [messages](_message_manager_messagemanager_.messagemanager.md#protected-messages)
* [name](_message_manager_messagemanager_.messagemanager.md#name)

### Accessors

* [config](_message_manager_messagemanager_.messagemanager.md#config)
* [state](_message_manager_messagemanager_.messagemanager.md#state)

### Methods

* [addMessage](_message_manager_messagemanager_.messagemanager.md#addmessage)
* [addUnapprovedMessage](_message_manager_messagemanager_.messagemanager.md#addunapprovedmessage)
* [addUnapprovedMessageAsync](_message_manager_messagemanager_.messagemanager.md#addunapprovedmessageasync)
* [approveMessage](_message_manager_messagemanager_.messagemanager.md#approvemessage)
* [configure](_message_manager_messagemanager_.messagemanager.md#configure)
* [getMessage](_message_manager_messagemanager_.messagemanager.md#getmessage)
* [getUnapprovedMessages](_message_manager_messagemanager_.messagemanager.md#getunapprovedmessages)
* [getUnapprovedMessagesCount](_message_manager_messagemanager_.messagemanager.md#getunapprovedmessagescount)
* [initialize](_message_manager_messagemanager_.messagemanager.md#protected-initialize)
* [notify](_message_manager_messagemanager_.messagemanager.md#notify)
* [prepMessageForSigning](_message_manager_messagemanager_.messagemanager.md#prepmessageforsigning)
* [rejectMessage](_message_manager_messagemanager_.messagemanager.md#rejectmessage)
* [saveMessageList](_message_manager_messagemanager_.messagemanager.md#protected-savemessagelist)
* [setMessageStatus](_message_manager_messagemanager_.messagemanager.md#protected-setmessagestatus)
* [setMessageStatusApproved](_message_manager_messagemanager_.messagemanager.md#setmessagestatusapproved)
* [setMessageStatusSigned](_message_manager_messagemanager_.messagemanager.md#setmessagestatussigned)
* [subscribe](_message_manager_messagemanager_.messagemanager.md#subscribe)
* [unsubscribe](_message_manager_messagemanager_.messagemanager.md#unsubscribe)
* [update](_message_manager_messagemanager_.messagemanager.md#update)
* [updateMessage](_message_manager_messagemanager_.messagemanager.md#protected-updatemessage)

## Constructors

###  constructor

\+ **new MessageManager**(`config?`: Partial‹[BaseConfig](../interfaces/_basecontroller_.baseconfig.md)›, `state?`: Partial‹[MessageManagerState](../interfaces/_message_manager_abstractmessagemanager_.messagemanagerstate.md)‹[Message](../interfaces/_message_manager_messagemanager_.message.md)››): *[MessageManager](_message_manager_messagemanager_.messagemanager.md)*

*Inherited from [AbstractMessageManager](_message_manager_abstractmessagemanager_.abstractmessagemanager.md).[constructor](_message_manager_abstractmessagemanager_.abstractmessagemanager.md#constructor)*

*Overrides [BaseController](_basecontroller_.basecontroller.md).[constructor](_basecontroller_.basecontroller.md#constructor)*

Defined in message-manager/AbstractMessageManager.ts:132

Creates an AbstractMessageManager instance.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`config?` | Partial‹[BaseConfig](../interfaces/_basecontroller_.baseconfig.md)› | Initial options used to configure this controller. |
`state?` | Partial‹[MessageManagerState](../interfaces/_message_manager_abstractmessagemanager_.messagemanagerstate.md)‹[Message](../interfaces/_message_manager_messagemanager_.message.md)›› | Initial state to set on this controller.  |

**Returns:** *[MessageManager](_message_manager_messagemanager_.messagemanager.md)*

## Properties

###  defaultConfig

• **defaultConfig**: *[BaseConfig](../interfaces/_basecontroller_.baseconfig.md)* = {} as C

*Inherited from [BaseController](_basecontroller_.basecontroller.md).[defaultConfig](_basecontroller_.basecontroller.md#defaultconfig)*

Defined in BaseController.ts:33

Default options used to configure this controller

___

###  defaultState

• **defaultState**: *[MessageManagerState](../interfaces/_message_manager_abstractmessagemanager_.messagemanagerstate.md)‹[Message](../interfaces/_message_manager_messagemanager_.message.md)›* = {} as S

*Inherited from [BaseController](_basecontroller_.basecontroller.md).[defaultState](_basecontroller_.basecontroller.md#defaultstate)*

Defined in BaseController.ts:38

Default state set on this controller

___

###  disabled

• **disabled**: *boolean* = false

*Inherited from [BaseController](_basecontroller_.basecontroller.md).[disabled](_basecontroller_.basecontroller.md#disabled)*

Defined in BaseController.ts:43

Determines if listeners are notified of state changes

___

###  hub

• **hub**: *EventEmitter‹›* = new EventEmitter()

*Inherited from [AbstractMessageManager](_message_manager_abstractmessagemanager_.abstractmessagemanager.md).[hub](_message_manager_abstractmessagemanager_.abstractmessagemanager.md#hub)*

Defined in message-manager/AbstractMessageManager.ts:127

EventEmitter instance used to listen to specific message events

___

### `Protected` messages

• **messages**: *[Message](../interfaces/_message_manager_messagemanager_.message.md)[]*

*Inherited from [AbstractMessageManager](_message_manager_abstractmessagemanager_.abstractmessagemanager.md).[messages](_message_manager_abstractmessagemanager_.abstractmessagemanager.md#protected-messages)*

Defined in message-manager/AbstractMessageManager.ts:77

___

###  name

• **name**: *string* = "MessageManager"

*Overrides [AbstractMessageManager](_message_manager_abstractmessagemanager_.abstractmessagemanager.md).[name](_message_manager_abstractmessagemanager_.abstractmessagemanager.md#name)*

Defined in message-manager/MessageManager.ts:63

Name of this controller used during composition

## Accessors

###  config

• **get config**(): *C*

*Inherited from [BaseController](_basecontroller_.basecontroller.md).[config](_basecontroller_.basecontroller.md#config)*

Defined in BaseController.ts:93

Retrieves current controller configuration options.

**Returns:** *C*

The current configuration.

___

###  state

• **get state**(): *S*

*Inherited from [BaseController](_basecontroller_.basecontroller.md).[state](_basecontroller_.basecontroller.md#state)*

Defined in BaseController.ts:102

Retrieves current controller state.

**Returns:** *S*

The current state.

## Methods

###  addMessage

▸ **addMessage**(`message`: [Message](../interfaces/_message_manager_messagemanager_.message.md)): *void*

*Inherited from [AbstractMessageManager](_message_manager_abstractmessagemanager_.abstractmessagemanager.md).[addMessage](_message_manager_abstractmessagemanager_.abstractmessagemanager.md#addmessage)*

Defined in message-manager/AbstractMessageManager.ts:182

Adds a passed Message to this.messages, and calls this.saveMessageList() to save
the unapproved Messages from that list to this.messages.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`message` | [Message](../interfaces/_message_manager_messagemanager_.message.md) | The Message to add to this.messages.  |

**Returns:** *void*

___

###  addUnapprovedMessage

▸ **addUnapprovedMessage**(`messageParams`: [MessageParams](../interfaces/_message_manager_messagemanager_.messageparams.md), `req?`: [OriginalRequest](../interfaces/_message_manager_abstractmessagemanager_.originalrequest.md)): *string*

Defined in message-manager/MessageManager.ts:113

Creates a new Message with an 'unapproved' status using the passed messageParams.
this.addMessage is called to add the new Message to this.messages, and to save the
unapproved Messages.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`messageParams` | [MessageParams](../interfaces/_message_manager_messagemanager_.messageparams.md) | The params for the eth_sign call to be made after the message is approved. |
`req?` | [OriginalRequest](../interfaces/_message_manager_abstractmessagemanager_.originalrequest.md) | The original request object possibly containing the origin. |

**Returns:** *string*

The id of the newly created message.

___

###  addUnapprovedMessageAsync

▸ **addUnapprovedMessageAsync**(`messageParams`: [MessageParams](../interfaces/_message_manager_messagemanager_.messageparams.md), `req?`: [OriginalRequest](../interfaces/_message_manager_abstractmessagemanager_.originalrequest.md)): *Promise‹string›*

Defined in message-manager/MessageManager.ts:73

Creates a new Message with an 'unapproved' status using the passed messageParams.
this.addMessage is called to add the new Message to this.messages, and to save the unapproved Messages.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`messageParams` | [MessageParams](../interfaces/_message_manager_messagemanager_.messageparams.md) | The params for the eth_sign call to be made after the message is approved. |
`req?` | [OriginalRequest](../interfaces/_message_manager_abstractmessagemanager_.originalrequest.md) | The original request object possibly containing the origin. |

**Returns:** *Promise‹string›*

Promise resolving to the raw data of the signature request.

___

###  approveMessage

▸ **approveMessage**(`messageParams`: [MessageParamsMetamask](../interfaces/_message_manager_messagemanager_.messageparamsmetamask.md)): *Promise‹[MessageParams](../interfaces/_message_manager_messagemanager_.messageparams.md)›*

*Inherited from [AbstractMessageManager](_message_manager_abstractmessagemanager_.abstractmessagemanager.md).[approveMessage](_message_manager_abstractmessagemanager_.abstractmessagemanager.md#approvemessage)*

Defined in message-manager/AbstractMessageManager.ts:206

Approves a Message. Sets the message status via a call to this.setMessageStatusApproved,
and returns a promise with any the message params modified for proper signing.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`messageParams` | [MessageParamsMetamask](../interfaces/_message_manager_messagemanager_.messageparamsmetamask.md) | The messageParams to be used when signing method is called, plus data added by MetaMask. |

**Returns:** *Promise‹[MessageParams](../interfaces/_message_manager_messagemanager_.messageparams.md)›*

Promise resolving to the messageParams with the metamaskId property removed.

___

###  configure

▸ **configure**(`config`: Partial‹[BaseConfig](../interfaces/_basecontroller_.baseconfig.md)›, `overwrite`: boolean, `fullUpdate`: boolean): *void*

*Inherited from [BaseController](_basecontroller_.basecontroller.md).[configure](_basecontroller_.basecontroller.md#configure)*

Defined in BaseController.ts:113

Updates controller configuration.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`config` | Partial‹[BaseConfig](../interfaces/_basecontroller_.baseconfig.md)› | - | New configuration options. |
`overwrite` | boolean | false | Overwrite config instead of merging. |
`fullUpdate` | boolean | true | Boolean that defines if the update is partial or not.  |

**Returns:** *void*

___

###  getMessage

▸ **getMessage**(`messageId`: string): *M*

*Inherited from [AbstractMessageManager](_message_manager_abstractmessagemanager_.abstractmessagemanager.md).[getMessage](_message_manager_abstractmessagemanager_.abstractmessagemanager.md#getmessage)*

Defined in message-manager/AbstractMessageManager.ts:194

Returns a specified Message.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`messageId` | string | The id of the Message to get. |

**Returns:** *M*

The Message with the id that matches the passed messageId, or undefined
if no Message has that id.

___

###  getUnapprovedMessages

▸ **getUnapprovedMessages**(): *object*

*Inherited from [AbstractMessageManager](_message_manager_abstractmessagemanager_.abstractmessagemanager.md).[getUnapprovedMessages](_message_manager_abstractmessagemanager_.abstractmessagemanager.md#getunapprovedmessages)*

Defined in message-manager/AbstractMessageManager.ts:167

A getter for the 'unapproved' Messages in state messages.

**Returns:** *object*

An index of Message ids to Messages, for all 'unapproved' Messages in this.messages.

* \[ **key**: *string*\]: [Message](../interfaces/_message_manager_messagemanager_.message.md)

___

###  getUnapprovedMessagesCount

▸ **getUnapprovedMessagesCount**(): *number*

*Inherited from [AbstractMessageManager](_message_manager_abstractmessagemanager_.abstractmessagemanager.md).[getUnapprovedMessagesCount](_message_manager_abstractmessagemanager_.abstractmessagemanager.md#getunapprovedmessagescount)*

Defined in message-manager/AbstractMessageManager.ts:158

A getter for the number of 'unapproved' Messages in this.messages.

**Returns:** *number*

The number of 'unapproved' Messages in this.messages.

___

### `Protected` initialize

▸ **initialize**(): *this*

*Inherited from [BaseController](_basecontroller_.basecontroller.md).[initialize](_basecontroller_.basecontroller.md#protected-initialize)*

Defined in BaseController.ts:80

Enables the controller. This sets each config option as a member
variable on this instance and triggers any defined setters. This
also sets initial state and triggers any listeners.

**Returns:** *this*

This controller instance.

___

###  notify

▸ **notify**(): *void*

*Inherited from [BaseController](_basecontroller_.basecontroller.md).[notify](_basecontroller_.basecontroller.md#notify)*

Defined in BaseController.ts:138

Notifies all subscribed listeners of current state.

**Returns:** *void*

___

###  prepMessageForSigning

▸ **prepMessageForSigning**(`messageParams`: [MessageParamsMetamask](../interfaces/_message_manager_messagemanager_.messageparamsmetamask.md)): *Promise‹[MessageParams](../interfaces/_message_manager_messagemanager_.messageparams.md)›*

*Overrides [AbstractMessageManager](_message_manager_abstractmessagemanager_.abstractmessagemanager.md).[prepMessageForSigning](_message_manager_abstractmessagemanager_.abstractmessagemanager.md#abstract-prepmessageforsigning)*

Defined in message-manager/MessageManager.ts:141

Removes the metamaskId property from passed messageParams and returns a promise which
resolves the updated messageParams.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`messageParams` | [MessageParamsMetamask](../interfaces/_message_manager_messagemanager_.messageparamsmetamask.md) | The messageParams to modify. |

**Returns:** *Promise‹[MessageParams](../interfaces/_message_manager_messagemanager_.messageparams.md)›*

Promise resolving to the messageParams with the metamaskId property removed.

___

###  rejectMessage

▸ **rejectMessage**(`messageId`: string): *void*

*Inherited from [AbstractMessageManager](_message_manager_abstractmessagemanager_.abstractmessagemanager.md).[rejectMessage](_message_manager_abstractmessagemanager_.abstractmessagemanager.md#rejectmessage)*

Defined in message-manager/AbstractMessageManager.ts:255

Sets a Message status to 'rejected' via a call to this.setMessageStatus.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`messageId` | string | The id of the Message to reject.  |

**Returns:** *void*

___

### `Protected` saveMessageList

▸ **saveMessageList**(): *void*

*Inherited from [AbstractMessageManager](_message_manager_abstractmessagemanager_.abstractmessagemanager.md).[saveMessageList](_message_manager_abstractmessagemanager_.abstractmessagemanager.md#protected-savemessagelist)*

Defined in message-manager/AbstractMessageManager.ts:83

Saves the unapproved messages, and their count to state.

**Returns:** *void*

___

### `Protected` setMessageStatus

▸ **setMessageStatus**(`messageId`: string, `status`: string): *void*

*Inherited from [AbstractMessageManager](_message_manager_abstractmessagemanager_.abstractmessagemanager.md).[setMessageStatus](_message_manager_abstractmessagemanager_.abstractmessagemanager.md#protected-setmessagestatus)*

Defined in message-manager/AbstractMessageManager.ts:96

Updates the status of a Message in this.messages.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`messageId` | string | The id of the Message to update. |
`status` | string | The new status of the Message.  |

**Returns:** *void*

___

###  setMessageStatusApproved

▸ **setMessageStatusApproved**(`messageId`: string): *void*

*Inherited from [AbstractMessageManager](_message_manager_abstractmessagemanager_.abstractmessagemanager.md).[setMessageStatusApproved](_message_manager_abstractmessagemanager_.abstractmessagemanager.md#setmessagestatusapproved)*

Defined in message-manager/AbstractMessageManager.ts:218

Sets a Message status to 'approved' via a call to this.setMessageStatus.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`messageId` | string | The id of the Message to approve.  |

**Returns:** *void*

___

###  setMessageStatusSigned

▸ **setMessageStatusSigned**(`messageId`: string, `rawSig`: string): *void*

*Inherited from [AbstractMessageManager](_message_manager_abstractmessagemanager_.abstractmessagemanager.md).[setMessageStatusSigned](_message_manager_abstractmessagemanager_.abstractmessagemanager.md#setmessagestatussigned)*

Defined in message-manager/AbstractMessageManager.ts:230

Sets a Message status to 'signed' via a call to this.setMessageStatus and updates
that Message in this.messages by adding the raw signature data of the signature
request to the Message.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`messageId` | string | The id of the Message to sign. |
`rawSig` | string | The raw data of the signature request.  |

**Returns:** *void*

___

###  subscribe

▸ **subscribe**(`listener`: [Listener](../modules/_basecontroller_.md#listener)‹[MessageManagerState](../interfaces/_message_manager_abstractmessagemanager_.messagemanagerstate.md)‹[Message](../interfaces/_message_manager_messagemanager_.message.md)››): *void*

*Inherited from [BaseController](_basecontroller_.basecontroller.md).[subscribe](_basecontroller_.basecontroller.md#subscribe)*

Defined in BaseController.ts:153

Adds new listener to be notified of state changes.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`listener` | [Listener](../modules/_basecontroller_.md#listener)‹[MessageManagerState](../interfaces/_message_manager_abstractmessagemanager_.messagemanagerstate.md)‹[Message](../interfaces/_message_manager_messagemanager_.message.md)›› | The callback triggered when state changes.  |

**Returns:** *void*

___

###  unsubscribe

▸ **unsubscribe**(`listener`: [Listener](../modules/_basecontroller_.md#listener)‹[MessageManagerState](../interfaces/_message_manager_abstractmessagemanager_.messagemanagerstate.md)‹[Message](../interfaces/_message_manager_messagemanager_.message.md)››): *boolean*

*Inherited from [BaseController](_basecontroller_.basecontroller.md).[unsubscribe](_basecontroller_.basecontroller.md#unsubscribe)*

Defined in BaseController.ts:163

Removes existing listener from receiving state changes.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`listener` | [Listener](../modules/_basecontroller_.md#listener)‹[MessageManagerState](../interfaces/_message_manager_abstractmessagemanager_.messagemanagerstate.md)‹[Message](../interfaces/_message_manager_messagemanager_.message.md)›› | The callback to remove. |

**Returns:** *boolean*

`true` if a listener is found and unsubscribed.

___

###  update

▸ **update**(`state`: Partial‹[MessageManagerState](../interfaces/_message_manager_abstractmessagemanager_.messagemanagerstate.md)‹[Message](../interfaces/_message_manager_messagemanager_.message.md)››, `overwrite`: boolean): *void*

*Inherited from [BaseController](_basecontroller_.basecontroller.md).[update](_basecontroller_.basecontroller.md#update)*

Defined in BaseController.ts:175

Updates controller state.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`state` | Partial‹[MessageManagerState](../interfaces/_message_manager_abstractmessagemanager_.messagemanagerstate.md)‹[Message](../interfaces/_message_manager_messagemanager_.message.md)›› | - | The new state. |
`overwrite` | boolean | false | Overwrite state instead of merging.  |

**Returns:** *void*

___

### `Protected` updateMessage

▸ **updateMessage**(`message`: [Message](../interfaces/_message_manager_messagemanager_.message.md)): *void*

*Inherited from [AbstractMessageManager](_message_manager_abstractmessagemanager_.abstractmessagemanager.md).[updateMessage](_message_manager_abstractmessagemanager_.abstractmessagemanager.md#protected-updatemessage)*

Defined in message-manager/AbstractMessageManager.ts:115

Sets a Message in this.messages to the passed Message if the ids are equal.
Then saves the unapprovedMessage list to storage.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`message` | [Message](../interfaces/_message_manager_messagemanager_.message.md) | A Message that will replace an existing Message (with the id) in this.messages.  |

**Returns:** *void*
