[ethereum-gas-reference](../README.md) › [Globals](../globals.md) › [BaseController](basecontroller.md)

# Class: BaseController ‹**C, S, N, S, messenger**›

Controller class that provides configuration, state management, and subscriptions
Controller class that provides state management, subscriptions, and state metadata

## Type parameters

▪ **C**: *[BaseConfig](../interfaces/baseconfig.md)*

▪ **S**: *[BaseState](../interfaces/basestate.md)*

▪ **N**: *string*

▪ **S**: *Record‹string, [Json](../globals.md#json)›*

▪ **messenger**: *[RestrictedControllerMessenger](restrictedcontrollermessenger.md)‹N, any, any, string, string›*

## Hierarchy

* **BaseController**

  ↳ [NetworkController](networkcontroller.md)

## Index

### Constructors

* [constructor](basecontroller.md#constructor)

### Properties

* [defaultConfig](basecontroller.md#defaultconfig)
* [defaultState](basecontroller.md#defaultstate)
* [disabled](basecontroller.md#disabled)
* [initialConfig](basecontroller.md#private-readonly-initialconfig)
* [initialState](basecontroller.md#private-readonly-initialstate)
* [internalConfig](basecontroller.md#private-internalconfig)
* [internalListeners](basecontroller.md#private-internallisteners)
* [internalState](basecontroller.md#private-internalstate)
* [messagingSystem](basecontroller.md#protected-messagingsystem)
* [metadata](basecontroller.md#readonly-metadata)
* [name](basecontroller.md#name)

### Accessors

* [config](basecontroller.md#config)
* [state](basecontroller.md#state)

### Methods

* [configure](basecontroller.md#configure)
* [destroy](basecontroller.md#protected-destroy)
* [initialize](basecontroller.md#protected-initialize)
* [notify](basecontroller.md#notify)
* [subscribe](basecontroller.md#subscribe)
* [unsubscribe](basecontroller.md#unsubscribe)
* [update](basecontroller.md#update)

## Constructors

###  constructor

\+ **new BaseController**(`config`: Partial‹C›, `state`: Partial‹S›): *[BaseController](basecontroller.md)*

Defined in BaseController.ts:58

Creates a BaseController instance. Both initial state and initial
configuration options are merged with defaults upon initialization.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`config` | Partial‹C› | {} as C | Initial options used to configure this controller. |
`state` | Partial‹S› | {} as S | Initial state to set on this controller.  |

**Returns:** *[BaseController](basecontroller.md)*

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

• **internalListeners**: *[Listener](../globals.md#listener)‹S›[]* = []

Defined in BaseController.ts:58

___

### `Private` internalState

• **internalState**: *S* = this.defaultState

Defined in BaseController.ts:56

Defined in BaseControllerV2.ts:80

___

### `Protected` messagingSystem

• **messagingSystem**: *messenger*

Defined in BaseControllerV2.ts:82

___

### `Readonly` metadata

• **metadata**: *[StateMetadata](../globals.md#statemetadata)‹S›*

Defined in BaseControllerV2.ts:91

___

###  name

• **name**: *N* = "BaseController"

Defined in BaseController.ts:48

Defined in BaseControllerV2.ts:89

Name of this controller used during composition
The name of the controller.

This is used by the ComposableController to construct a composed application state.

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

Defined in BaseControllerV2.ts:138

Retrieves current controller state.

**Returns:** *S*

The current state.

• **set state**(`_`: S): *void*

Defined in BaseControllerV2.ts:142

Retrieves current controller state.
Retrieves current controller state.

**Parameters:**

Name | Type |
------ | ------ |
`_` | S |

**Returns:** *void*

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

### `Protected` destroy

▸ **destroy**(): *void*

Defined in BaseControllerV2.ts:185

Prepares the controller for garbage collection. This should be extended
by any subclasses to clean up any additional connections or events.

The only cleanup performed here is to remove listeners. While technically
this is not required to ensure this instance is garbage collected, it at
least ensures this instance won't be responsible for preventing the
listeners from being garbage collected.

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

▸ **subscribe**(`listener`: [Listener](../globals.md#listener)‹S›): *void*

Defined in BaseController.ts:153

Adds new listener to be notified of state changes.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`listener` | [Listener](../globals.md#listener)‹S› | The callback triggered when state changes.  |

**Returns:** *void*

___

###  unsubscribe

▸ **unsubscribe**(`listener`: [Listener](../globals.md#listener)‹S›): *boolean*

Defined in BaseController.ts:163

Removes existing listener from receiving state changes.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`listener` | [Listener](../globals.md#listener)‹S› | The callback to remove. |

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
