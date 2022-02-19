[metamask-controllers-main-src-gas-2](../README.md) › [Globals](../globals.md) › ["BaseControllerV2"](../modules/_basecontrollerv2_.md) › [BaseController](_basecontrollerv2_.basecontroller.md)

# Class: BaseController ‹**N, S, messenger**›

Controller class that provides state management, subscriptions, and state metadata

## Type parameters

▪ **N**: *string*

▪ **S**: *Record‹string, [Json](../modules/_basecontrollerv2_.md#json)›*

▪ **messenger**: *[RestrictedControllerMessenger](_controllermessenger_.restrictedcontrollermessenger.md)‹N, any, any, string, string›*

## Hierarchy

* **BaseController**

  ↳ [GasFeeController](_gasfeecontroller_.gasfeecontroller.md)

## Index

### Constructors

* [constructor](_basecontrollerv2_.basecontroller.md#constructor)

### Properties

* [internalState](_basecontrollerv2_.basecontroller.md#private-internalstate)
* [messagingSystem](_basecontrollerv2_.basecontroller.md#protected-messagingsystem)
* [metadata](_basecontrollerv2_.basecontroller.md#readonly-metadata)
* [name](_basecontrollerv2_.basecontroller.md#readonly-name)
* [subscribe](_basecontrollerv2_.basecontroller.md#readonly-subscribe)

### Accessors

* [state](_basecontrollerv2_.basecontroller.md#state)

### Methods

* [destroy](_basecontrollerv2_.basecontroller.md#protected-destroy)
* [update](_basecontrollerv2_.basecontroller.md#protected-update)

## Constructors

###  constructor

\+ **new BaseController**(`__namedParameters`: object): *[BaseController](_basecontrollerv2_.basecontroller.md)*

Defined in BaseControllerV2.ts:99

Creates a BaseController instance.

**Parameters:**

▪ **__namedParameters**: *object*

Name | Type |
------ | ------ |
`messenger` | messenger |
`metadata` | [StateMetadata](../modules/_basecontrollerv2_.md#statemetadata)‹S› |
`name` | N |
`state` | S |

**Returns:** *[BaseController](_basecontrollerv2_.basecontroller.md)*

## Properties

### `Private` internalState

• **internalState**: *S*

Defined in BaseControllerV2.ts:80

___

### `Protected` messagingSystem

• **messagingSystem**: *messenger*

Defined in BaseControllerV2.ts:82

___

### `Readonly` metadata

• **metadata**: *[StateMetadata](../modules/_basecontrollerv2_.md#statemetadata)‹S›*

Defined in BaseControllerV2.ts:91

___

### `Readonly` name

• **name**: *N*

Defined in BaseControllerV2.ts:89

The name of the controller.

This is used by the ComposableController to construct a composed application state.

___

### `Readonly` subscribe

• **subscribe**: *never*

Defined in BaseControllerV2.ts:99

The existence of the `subscribe` property is how the ComposableController detects whether a
controller extends the old BaseController or the new one. We set it to `never` here to ensure
this property is never used for new BaseController-based controllers, to ensure the
ComposableController never mistakes them for an older style controller.

## Accessors

###  state

• **get state**(): *S*

Defined in BaseControllerV2.ts:138

Retrieves current controller state.

**Returns:** *S*

The current state.

• **set state**(`_`: S): *void*

Defined in BaseControllerV2.ts:142

Retrieves current controller state.

**Parameters:**

Name | Type |
------ | ------ |
`_` | S |

**Returns:** *void*

The current state.

## Methods

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

### `Protected` update

▸ **update**(`callback`: function): *void*

Defined in BaseControllerV2.ts:157

Updates controller state. Accepts a callback that is passed a draft copy
of the controller state. If a value is returned, it is set as the new
state. Otherwise, any changes made within that callback to the draft are
applied to the controller state.

**Parameters:**

▪ **callback**: *function*

Callback for updating state, passed a draft state
object. Return a new state object or mutate the draft to update state.

▸ (`state`: Draft‹S›): *void | S*

**Parameters:**

Name | Type |
------ | ------ |
`state` | Draft‹S› |

**Returns:** *void*
