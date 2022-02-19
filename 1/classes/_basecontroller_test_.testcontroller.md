[ethereum-gas-reference](../README.md) › [Globals](../globals.md) › ["BaseController.test"](../modules/_basecontroller_test_.md) › [TestController](_basecontroller_test_.testcontroller.md)

# Class: TestController

## Hierarchy

* [BaseController](_basecontroller_.basecontroller.md)‹[BaseConfig](../interfaces/_basecontroller_.baseconfig.md), [BaseState](../interfaces/_basecontroller_.basestate.md)›

  ↳ **TestController**

## Index

### Constructors

* [constructor](_basecontroller_test_.testcontroller.md#constructor)

### Properties

* [defaultConfig](_basecontroller_test_.testcontroller.md#defaultconfig)
* [defaultState](_basecontroller_test_.testcontroller.md#defaultstate)
* [disabled](_basecontroller_test_.testcontroller.md#disabled)
* [name](_basecontroller_test_.testcontroller.md#name)

### Accessors

* [config](_basecontroller_test_.testcontroller.md#config)
* [state](_basecontroller_test_.testcontroller.md#state)

### Methods

* [configure](_basecontroller_test_.testcontroller.md#configure)
* [initialize](_basecontroller_test_.testcontroller.md#protected-initialize)
* [notify](_basecontroller_test_.testcontroller.md#notify)
* [subscribe](_basecontroller_test_.testcontroller.md#subscribe)
* [unsubscribe](_basecontroller_test_.testcontroller.md#unsubscribe)
* [update](_basecontroller_test_.testcontroller.md#update)

## Constructors

###  constructor

\+ **new TestController**(`config?`: [BaseConfig](../interfaces/_basecontroller_.baseconfig.md), `state?`: [BaseState](../interfaces/_basecontroller_.basestate.md)): *[TestController](_basecontroller_test_.testcontroller.md)*

*Overrides [BaseController](_basecontroller_.basecontroller.md).[constructor](_basecontroller_.basecontroller.md#constructor)*

Defined in BaseController.test.ts:7

**Parameters:**

Name | Type |
------ | ------ |
`config?` | [BaseConfig](../interfaces/_basecontroller_.baseconfig.md) |
`state?` | [BaseState](../interfaces/_basecontroller_.basestate.md) |

**Returns:** *[TestController](_basecontroller_test_.testcontroller.md)*

## Properties

###  defaultConfig

• **defaultConfig**: *[BaseConfig](../interfaces/_basecontroller_.baseconfig.md)* = {} as C

*Inherited from [BaseController](_basecontroller_.basecontroller.md).[defaultConfig](_basecontroller_.basecontroller.md#defaultconfig)*

Defined in BaseController.ts:33

Default options used to configure this controller

___

###  defaultState

• **defaultState**: *[BaseState](../interfaces/_basecontroller_.basestate.md)* = {} as S

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

###  name

• **name**: *string* = "BaseController"

*Inherited from [BaseController](_basecontroller_.basecontroller.md).[name](_basecontroller_.basecontroller.md#name)*

Defined in BaseController.ts:48

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

###  subscribe

▸ **subscribe**(`listener`: [Listener](../modules/_basecontroller_.md#listener)‹[BaseState](../interfaces/_basecontroller_.basestate.md)›): *void*

*Inherited from [BaseController](_basecontroller_.basecontroller.md).[subscribe](_basecontroller_.basecontroller.md#subscribe)*

Defined in BaseController.ts:153

Adds new listener to be notified of state changes.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`listener` | [Listener](../modules/_basecontroller_.md#listener)‹[BaseState](../interfaces/_basecontroller_.basestate.md)› | The callback triggered when state changes.  |

**Returns:** *void*

___

###  unsubscribe

▸ **unsubscribe**(`listener`: [Listener](../modules/_basecontroller_.md#listener)‹[BaseState](../interfaces/_basecontroller_.basestate.md)›): *boolean*

*Inherited from [BaseController](_basecontroller_.basecontroller.md).[unsubscribe](_basecontroller_.basecontroller.md#unsubscribe)*

Defined in BaseController.ts:163

Removes existing listener from receiving state changes.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`listener` | [Listener](../modules/_basecontroller_.md#listener)‹[BaseState](../interfaces/_basecontroller_.basestate.md)› | The callback to remove. |

**Returns:** *boolean*

`true` if a listener is found and unsubscribed.

___

###  update

▸ **update**(`state`: Partial‹[BaseState](../interfaces/_basecontroller_.basestate.md)›, `overwrite`: boolean): *void*

*Inherited from [BaseController](_basecontroller_.basecontroller.md).[update](_basecontroller_.basecontroller.md#update)*

Defined in BaseController.ts:175

Updates controller state.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`state` | Partial‹[BaseState](../interfaces/_basecontroller_.basestate.md)› | - | The new state. |
`overwrite` | boolean | false | Overwrite state instead of merging.  |

**Returns:** *void*
