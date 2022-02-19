[metamask-controllers-main-src-gas-2](../README.md) › [Globals](../globals.md) › ["ControllerMessenger"](../modules/_controllermessenger_.md) › [RestrictedControllerMessenger](_controllermessenger_.restrictedcontrollermessenger.md)

# Class: RestrictedControllerMessenger ‹**N, Action, Event, AllowedAction, AllowedEvent**›

A restricted controller messenger.

This acts as a wrapper around the controller messenger instance that restricts access to actions
and events.

## Type parameters

▪ **N**: *string*

The namespace for this messenger. Typically this is the name of the controller or
module that this messenger has been created for. The authority to publish events and register
actions under this namespace is granted to this restricted messenger instance.

▪ **Action**: *[ActionConstraint](../modules/_controllermessenger_.md#actionconstraint)*

A type union of all Action types.

▪ **Event**: *[EventConstraint](../modules/_controllermessenger_.md#eventconstraint)*

A type union of all Event types.

▪ **AllowedAction**: *string*

A type union of the 'type' string for any allowed actions.

▪ **AllowedEvent**: *string*

A type union of the 'type' string for any allowed events.

## Hierarchy

* **RestrictedControllerMessenger**

## Index

### Constructors

* [constructor](_controllermessenger_.restrictedcontrollermessenger.md#constructor)

### Properties

* [allowedActions](_controllermessenger_.restrictedcontrollermessenger.md#private-allowedactions)
* [allowedEvents](_controllermessenger_.restrictedcontrollermessenger.md#private-allowedevents)
* [controllerMessenger](_controllermessenger_.restrictedcontrollermessenger.md#private-controllermessenger)
* [controllerName](_controllermessenger_.restrictedcontrollermessenger.md#private-controllername)

### Methods

* [call](_controllermessenger_.restrictedcontrollermessenger.md#call)
* [clearEventSubscriptions](_controllermessenger_.restrictedcontrollermessenger.md#cleareventsubscriptions)
* [publish](_controllermessenger_.restrictedcontrollermessenger.md#publish)
* [registerActionHandler](_controllermessenger_.restrictedcontrollermessenger.md#registeractionhandler)
* [subscribe](_controllermessenger_.restrictedcontrollermessenger.md#subscribe)
* [unregisterActionHandler](_controllermessenger_.restrictedcontrollermessenger.md#unregisteractionhandler)
* [unsubscribe](_controllermessenger_.restrictedcontrollermessenger.md#unsubscribe)

## Constructors

###  constructor

\+ **new RestrictedControllerMessenger**(`__namedParameters`: object): *[RestrictedControllerMessenger](_controllermessenger_.restrictedcontrollermessenger.md)*

Defined in ControllerMessenger.ts:101

Constructs a restricted controller messenger

The provided allowlists grant the ability to call the listed actions and subscribe to the
listed events. The "name" provided grants ownership of any actions and events under that
namespace. Ownership allows registering actions and publishing events, as well as
unregistering actions and clearing event subscriptions.

**Parameters:**

▪ **__namedParameters**: *object*

Name | Type |
------ | ------ |
`allowedActions` | AllowedAction[] |
`allowedEvents` | AllowedEvent[] |
`controllerMessenger` | [ControllerMessenger](_controllermessenger_.controllermessenger.md)‹[ActionConstraint](../modules/_controllermessenger_.md#actionconstraint), [EventConstraint](../modules/_controllermessenger_.md#eventconstraint)› |
`name` | N |

**Returns:** *[RestrictedControllerMessenger](_controllermessenger_.restrictedcontrollermessenger.md)*

## Properties

### `Private` allowedActions

• **allowedActions**: *AllowedAction[] | null*

Defined in ControllerMessenger.ts:99

___

### `Private` allowedEvents

• **allowedEvents**: *AllowedEvent[] | null*

Defined in ControllerMessenger.ts:101

___

### `Private` controllerMessenger

• **controllerMessenger**: *[ControllerMessenger](_controllermessenger_.controllermessenger.md)‹[ActionConstraint](../modules/_controllermessenger_.md#actionconstraint), [EventConstraint](../modules/_controllermessenger_.md#eventconstraint)›*

Defined in ControllerMessenger.ts:92

___

### `Private` controllerName

• **controllerName**: *N*

Defined in ControllerMessenger.ts:97

## Methods

###  call

▸ **call**‹**T**›(`action`: T, ...`params`: [ExtractActionParameters](../modules/_controllermessenger_.md#extractactionparameters)‹Action, T›): *[ExtractActionResponse](../modules/_controllermessenger_.md#extractactionresponse)‹Action, T›*

Defined in ControllerMessenger.ts:199

Call an action.

This function will call the action handler corresponding to the given action type, passing
along any parameters given.

The action type being called must be on the action allowlist.

**`throws`** Will throw when no handler has been registered for the given type.

**Type parameters:**

▪ **T**: *AllowedAction & string*

A type union of allowed Action type strings.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`action` | T | The action type. This is a unqiue identifier for this action. |
`...params` | [ExtractActionParameters](../modules/_controllermessenger_.md#extractactionparameters)‹Action, T› | The action parameters. These must match the type of the parameters of the registered action handler. |

**Returns:** *[ExtractActionResponse](../modules/_controllermessenger_.md#extractactionresponse)‹Action, T›*

The action return value.

___

###  clearEventSubscriptions

▸ **clearEventSubscriptions**‹**E**›(`event`: E): *void*

Defined in ControllerMessenger.ts:332

Clear subscriptions for a specific event.

This will remove all subscribed handlers for this event.

The event type being cleared *must* be in the current namespace.

**Type parameters:**

▪ **E**: *[Namespaced](../modules/_controllermessenger_.md#namespaced)‹N, Event["type"]›*

A type union of Event type strings that are namespaced by N.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`event` | E | The event type. This is a unique identifier for this event. |

**Returns:** *void*

___

###  publish

▸ **publish**‹**E**›(`event`: E, ...`payload`: [ExtractEventPayload](../modules/_controllermessenger_.md#extracteventpayload)‹Event, E›): *void*

Defined in ControllerMessenger.ts:224

Publish an event.

Publishes the given payload to all subscribers of the given event type.

The event type being published *must* be in the current namespace.

**Type parameters:**

▪ **E**: *[Namespaced](../modules/_controllermessenger_.md#namespaced)‹N, Event["type"]›*

A type union of Event type strings that are namespaced by N.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`event` | E | The event type. This is a unique identifier for this event. |
`...payload` | [ExtractEventPayload](../modules/_controllermessenger_.md#extracteventpayload)‹Event, E› | The event payload. The type of the parameters for each event handler must match the type of this payload. |

**Returns:** *void*

___

###  registerActionHandler

▸ **registerActionHandler**‹**T**›(`action`: T, `handler`: [ActionHandler](../modules/_controllermessenger_.md#actionhandler)‹Action, T›): *void*

Defined in ControllerMessenger.ts:151

Register an action handler.

This will make the registered function available to call via the `call` method.

The action type this handler is registered under *must* be in the current namespace.

**`throws`** Will throw when a handler has been registered for this action type already.

**Type parameters:**

▪ **T**: *[Namespaced](../modules/_controllermessenger_.md#namespaced)‹N, Action["type"]›*

A type union of Action type strings that are namespaced by N.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`action` | T | The action type. This is a unqiue identifier for this action. |
`handler` | [ActionHandler](../modules/_controllermessenger_.md#actionhandler)‹Action, T› | The action handler. This function gets called when the `call` method is invoked with the given action type. |

**Returns:** *void*

___

###  subscribe

▸ **subscribe**‹**E**›(`eventType`: E, `handler`: [ExtractEventHandler](../modules/_controllermessenger_.md#extracteventhandler)‹Event, E›): *void*

Defined in ControllerMessenger.ts:249

Subscribe to an event.

Registers the given function as an event handler for the given event type.

The event type being subscribed to must be on the event allowlist.

**Type parameters:**

▪ **E**: *AllowedEvent & string*

A type union of Event type strings.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`eventType` | E | The event type. This is a unique identifier for this event. |
`handler` | [ExtractEventHandler](../modules/_controllermessenger_.md#extracteventhandler)‹Event, E› | The event handler. The type of the parameters for this event handler must match the type of the payload for this event type. |

**Returns:** *void*

▸ **subscribe**‹**E**, **V**›(`eventType`: E, `handler`: [SelectorEventHandler](../modules/_controllermessenger_.md#selectoreventhandler)‹V›, `selector`: [SelectorFunction](../modules/_controllermessenger_.md#selectorfunction)‹[ExtractEventPayload](../modules/_controllermessenger_.md#extracteventpayload)‹Event, E›, V›): *void*

Defined in ControllerMessenger.ts:273

Subscribe to an event, with a selector.

Registers the given handler function as an event handler for the given
event type. When an event is published, its payload is first passed to the
selector. The event handler is only called if the selector's return value
differs from its last known return value.

The event type being subscribed to must be on the event allowlist.

**Type parameters:**

▪ **E**: *AllowedEvent & string*

A type union of Event type strings.

▪ **V**

The selector return value.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`eventType` | E | The event type. This is a unique identifier for this event. |
`handler` | [SelectorEventHandler](../modules/_controllermessenger_.md#selectoreventhandler)‹V› | The event handler. The type of the parameters for this event handler must match the return type of the selector. |
`selector` | [SelectorFunction](../modules/_controllermessenger_.md#selectorfunction)‹[ExtractEventPayload](../modules/_controllermessenger_.md#extracteventpayload)‹Event, E›, V› | The selector function used to select relevant data from the event payload. The type of the parameters for this selector must match the type of the payload for this event type. |

**Returns:** *void*

___

###  unregisterActionHandler

▸ **unregisterActionHandler**‹**T**›(`action`: T): *void*

Defined in ControllerMessenger.ts:174

Unregister an action handler.

This will prevent this action from being called.

The action type being unregistered *must* be in the current namespace.

**Type parameters:**

▪ **T**: *[Namespaced](../modules/_controllermessenger_.md#namespaced)‹N, Action["type"]›*

A type union of Action type strings that are namespaced by N.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`action` | T | The action type. This is a unqiue identifier for this action. |

**Returns:** *void*

___

###  unsubscribe

▸ **unsubscribe**‹**E**›(`event`: E, `handler`: [ExtractEventHandler](../modules/_controllermessenger_.md#extracteventhandler)‹Event, E›): *void*

Defined in ControllerMessenger.ts:309

Unsubscribe from an event.

Unregisters the given function as an event handler for the given event.

The event type being unsubscribed to must be on the event allowlist.

**`throws`** Will throw when the given event handler is not registered for this event.

**`template`** A type union of allowed Event type strings.

**Type parameters:**

▪ **E**: *AllowedEvent & string*

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`event` | E | The event type. This is a unique identifier for this event. |
`handler` | [ExtractEventHandler](../modules/_controllermessenger_.md#extracteventhandler)‹Event, E› | The event handler to unregister. |

**Returns:** *void*
