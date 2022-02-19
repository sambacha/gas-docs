[ethereum-gas-reference](../README.md) › [Globals](../globals.md) › ["BaseController"](../modules/_basecontroller_.md) › [BaseController](_basecontroller_.basecontroller.md)

# Class: BaseController ‹**C, S**›

Controller class that provides configuration, state management, and subscriptions

## Type parameters

▪ **C**: *[BaseConfig](../interfaces/_basecontroller_.baseconfig.md)*

▪ **S**: *[BaseState](../interfaces/_basecontroller_.basestate.md)*

## Hierarchy

* **BaseController**

  ↳ [TestController](_basecontroller_test_.testcontroller.md)

  ↳ [AbstractMessageManager](_message_manager_abstractmessagemanager_.abstractmessagemanager.md)

  ↳ [NetworkController](_networkcontroller_.networkcontroller.md)

## Index

### Constructors

* [constructor](_basecontroller_.basecontroller.md#constructor)

### Properties

* [defaultConfig](_basecontroller_.basecontroller.md#defaultconfig)
* [defaultState](_basecontroller_.basecontroller.md#defaultstate)
* [disabled](_basecontroller_.basecontroller.md#disabled)
* [initialConfig](_basecontroller_.basecontroller.md#private-readonly-initialconfig)
* [initialState](_basecontroller_.basecontroller.md#private-readonly-initialstate)
* [internalConfig](_basecontroller_.basecontroller.md#private-internalconfig)
* [internalListeners](_basecontroller_.basecontroller.md#private-internallisteners)
* [internalState](_basecontroller_.basecontroller.md#private-internalstate)
* [name](_basecontroller_.basecontroller.md#name)

### Accessors

* [config](_basecontroller_.basecontroller.md#config)
* [state](_basecontroller_.basecontroller.md#state)

### Methods

* [configure](_basecontroller_.basecontroller.md#configure)
* [initialize](_basecontroller_.basecontroller.md#protected-initialize)
* [notify](_basecontroller_.basecontroller.md#notify)
* [subscribe](_basecontroller_.basecontroller.md#subscribe)
* [unsubscribe](_basecontroller_.basecontroller.md#unsubscribe)
* [update](_basecontroller_.basecontroller.md#update)

## Constructors

###  constructor

\+ **new BaseController**(`config`: Partial‹C›, `state`: Partial‹S›): *[BaseController](_basecontroller_.basecontroller.md)*

Defined in BaseController.ts:58

Creates a BaseController instance. Both initial state and initial
configuration options are merged with defaults upon initialization.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`config` | Partial‹C› | {} as C | Initial options used to configure this controller. |
`state` | Partial‹S› | {} as S | Initial state to set on this controller.  |

**Returns:** *[BaseController](_basecontroller_.basecontroller.md)*

## Properties

###  defaultConfig

• **defaultConfig**: *C* = {} as C

Defined in BaseController.ts:33

Default options used to configure this controller

___

###  defaultState

• **defaultState**: *S* = {} as S

Defined in BaseController.ts:38

Default state set on this controller

___

###  disabled

• **disabled**: *boolean* = false

Defined in BaseController.ts:43

Determines if listeners are notified of state changes

___

### `Private` `Readonly` initialConfig

• **initialConfig**: *C*

Defined in BaseController.ts:50

___

### `Private` `Readonly` initialState

• **initialState**: *S*

Defined in BaseController.ts:52

___

### `Private` internalConfig

• **internalConfig**: *C* = this.defaultConfig

Defined in BaseController.ts:54

___

### `Private` internalListeners

• **internalListeners**: *[Listener](../modules/_basecontroller_.md#listener)‹S›[]* = []

Defined in BaseController.ts:58

___

### `Private` internalState

• **internalState**: *S* = this.defaultState

Defined in BaseController.ts:56

___

###  name

• **name**: *string* = "BaseController"

Defined in BaseController.ts:48

Name of this controller used during composition

## Accessors

###  config

• **get config**(): *C*

Defined in BaseController.ts:93

Retrieves current controller configuration options.

**Returns:** *C*

The current configuration.

___

###  state

• **get state**(): *S*

Defined in BaseController.ts:102

Retrieves current controller state.

**Returns:** *S*

The current state.

## Methods

###  configure

▸ **configure**(`config`: Partial‹C›, `overwrite`: boolean, `fullUpdate`: boolean): *void*

Defined in BaseController.ts:113

Updates controller configuration.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`config` | Partial‹C› | - | New configuration options. |
`overwrite` | boolean | false | Overwrite config instead of merging. |
`fullUpdate` | boolean | true | Boolean that defines if the update is partial or not.  |

**Returns:** *void*

___

### `Protected` initialize

▸ **initialize**(): *this*

Defined in BaseController.ts:80

Enables the controller. This sets each config option as a member
variable on this instance and triggers any defined setters. This
also sets initial state and triggers any listeners.

**Returns:** *this*

This controller instance.

___

###  notify

▸ **notify**(): *void*

Defined in BaseController.ts:138

Notifies all subscribed listeners of current state.

**Returns:** *void*

___

###  subscribe

▸ **subscribe**(`listener`: [Listener](../modules/_basecontroller_.md#listener)‹S›): *void*

Defined in BaseController.ts:153

Adds new listener to be notified of state changes.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`listener` | [Listener](../modules/_basecontroller_.md#listener)‹S› | The callback triggered when state changes.  |

**Returns:** *void*

___

###  unsubscribe

▸ **unsubscribe**(`listener`: [Listener](../modules/_basecontroller_.md#listener)‹S›): *boolean*

Defined in BaseController.ts:163

Removes existing listener from receiving state changes.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`listener` | [Listener](../modules/_basecontroller_.md#listener)‹S› | The callback to remove. |

**Returns:** *boolean*

`true` if a listener is found and unsubscribed.

___

###  update

▸ **update**(`state`: Partial‹S›, `overwrite`: boolean): *void*

Defined in BaseController.ts:175

Updates controller state.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`state` | Partial‹S› | - | The new state. |
`overwrite` | boolean | false | Overwrite state instead of merging.  |

**Returns:** *void*
