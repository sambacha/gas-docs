[ethereum-gas-reference](../README.md) › [Globals](../globals.md) › [ControllerMessenger](controllermessenger.md)

# Class: ControllerMessenger ‹**Action, Event**›

A messaging system for controllers.

The controller messenger allows registering functions as 'actions' that can be called elsewhere,
and it allows publishing and subscribing to events. Both actions and events are identified by
unique strings.

## Type parameters

▪ **Action**: *[ActionConstraint](../globals.md#actionconstraint)*

A type union of all Action types.

▪ **Event**: *[EventConstraint](../globals.md#eventconstraint)*

A type union of all Event types.

## Hierarchy

* **ControllerMessenger**

## Index

### Properties

* [actions](controllermessenger.md#private-actions)
* [eventPayloadCache](controllermessenger.md#private-eventpayloadcache)
* [events](controllermessenger.md#private-events)

### Methods

* [call](controllermessenger.md#call)
* [clearActions](controllermessenger.md#clearactions)
* [clearEventSubscriptions](controllermessenger.md#cleareventsubscriptions)
* [clearSubscriptions](controllermessenger.md#clearsubscriptions)
* [getRestricted](controllermessenger.md#getrestricted)
* [publish](controllermessenger.md#publish)
* [registerActionHandler](controllermessenger.md#registeractionhandler)
* [subscribe](controllermessenger.md#subscribe)
* [unregisterActionHandler](controllermessenger.md#unregisteractionhandler)
* [unsubscribe](controllermessenger.md#unsubscribe)

## Properties

### `Private` actions

• **actions**: *Map‹Action["type"], unknown›* = new Map<Action['type'], unknown>()

Defined in ControllerMessenger.ts:357

___

### `Private` eventPayloadCache

• **eventPayloadCache**: *Map‹[GenericEventHandler](../globals.md#genericeventhandler), unknown›* = new Map<
    GenericEventHandler,
    unknown | undefined
  >()

Defined in ControllerMessenger.ts:364

A cache of selector return values for their respective handlers.

___

### `Private` events

• **events**: *Map‹Event["type"], [EventSubscriptionMap](../globals.md#eventsubscriptionmap)›* = new Map<Event['type'], EventSubscriptionMap>()

Defined in ControllerMessenger.ts:359

## Methods

###  call

▸ **call**‹**T**›(`actionType`: T, ...`params`: [ExtractActionParameters](../globals.md#extractactionparameters)‹Action, T›): *[ExtractActionResponse](../globals.md#extractactionresponse)‹Action, T›*

Defined in ControllerMessenger.ts:426

Call an action.

This function will call the action handler corresponding to the given action type, passing
along any parameters given.

**`throws`** Will throw when no handler has been registered for the given type.

**Type parameters:**

▪ **T**: *Action["type"]*

A type union of Action type strings.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`actionType` | T | The action type. This is a unqiue identifier for this action. |
`...params` | [ExtractActionParameters](../globals.md#extractactionparameters)‹Action, T› | The action parameters. These must match the type of the parameters of the registered action handler. |

**Returns:** *[ExtractActionResponse](../globals.md#extractactionresponse)‹Action, T›*

The action return value.

___

###  clearActions

▸ **clearActions**(): *void*

Defined in ControllerMessenger.ts:409

Unregister all action handlers.

This prevents all actions from being called.

**Returns:** *void*

___

###  clearEventSubscriptions

▸ **clearEventSubscriptions**‹**E**›(`eventType`: E): *void*

Defined in ControllerMessenger.ts:558

Clear subscriptions for a specific event.

This will remove all subscribed handlers for this event.

**Type parameters:**

▪ **E**: *Event["type"]*

A type union of Event type strings.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`eventType` | E | The event type. This is a unique identifier for this event. |

**Returns:** *void*

___

###  clearSubscriptions

▸ **clearSubscriptions**(): *void*

Defined in ControllerMessenger.ts:567

Clear all subscriptions.

This will remove all subscribed handlers for all events.

**Returns:** *void*

___

###  getRestricted

▸ **getRestricted**‹**N**, **AllowedAction**, **AllowedEvent**›(`__namedParameters`: object): *[RestrictedControllerMessenger](restrictedcontrollermessenger.md)‹N, [NarrowToNamespace](../globals.md#narrowtonamespace)‹Action, N› | [NarrowToAllowed](../globals.md#narrowtoallowed)‹Action, AllowedAction›, [NarrowToNamespace](../globals.md#narrowtonamespace)‹Event, N› | [NarrowToAllowed](../globals.md#narrowtoallowed)‹Event, AllowedEvent›, AllowedAction, AllowedEvent›*

Defined in ControllerMessenger.ts:595

Get a restricted controller messenger

Returns a wrapper around the controller messenger instance that restricts access to actions
and events. The provided allowlists grant the ability to call the listed actions and subscribe
to the listed events. The "name" provided grants ownership of any actions and events under
that namespace. Ownership allows registering actions and publishing events, as well as
unregistering actions and clearing event subscriptions.

**Type parameters:**

▪ **N**: *string*

The namespace for this messenger. Typically this is the name of the controller or
module that this messenger has been created for. The authority to publish events and register
actions under this namespace is granted to this restricted messenger instance.

▪ **AllowedAction**: *string*

A type union of the 'type' string for any allowed actions.

▪ **AllowedEvent**: *string*

A type union of the 'type' string for any allowed events.

**Parameters:**

▪ **__namedParameters**: *object*

Name | Type |
------ | ------ |
`allowedActions` | Extract‹Action["type"], AllowedAction›[] |
`allowedEvents` | Extract‹Event["type"], AllowedEvent›[] |
`name` | N |

**Returns:** *[RestrictedControllerMessenger](restrictedcontrollermessenger.md)‹N, [NarrowToNamespace](../globals.md#narrowtonamespace)‹Action, N› | [NarrowToAllowed](../globals.md#narrowtoallowed)‹Action, AllowedAction›, [NarrowToNamespace](../globals.md#narrowtonamespace)‹Event, N› | [NarrowToAllowed](../globals.md#narrowtoallowed)‹Event, AllowedEvent›, AllowedAction, AllowedEvent›*

The restricted controller messenger.

___

###  publish

▸ **publish**‹**E**›(`eventType`: E, ...`payload`: [ExtractEventPayload](../globals.md#extracteventpayload)‹Event, E›): *void*

Defined in ControllerMessenger.ts:447

Publish an event.

Publishes the given payload to all subscribers of the given event type.

**Type parameters:**

▪ **E**: *Event["type"]*

A type union of Event type strings.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`eventType` | E | The event type. This is a unique identifier for this event. |
`...payload` | [ExtractEventPayload](../globals.md#extracteventpayload)‹Event, E› | The event payload. The type of the parameters for each event handler must match the type of this payload. |

**Returns:** *void*

___

###  registerActionHandler

▸ **registerActionHandler**‹**T**›(`actionType`: T, `handler`: [ActionHandler](../globals.md#actionhandler)‹Action, T›): *void*

Defined in ControllerMessenger.ts:380

Register an action handler.

This will make the registered function available to call via the `call` method.

**`throws`** Will throw when a handler has been registered for this action type already.

**Type parameters:**

▪ **T**: *Action["type"]*

A type union of Action type strings.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`actionType` | T | The action type. This is a unqiue identifier for this action. |
`handler` | [ActionHandler](../globals.md#actionhandler)‹Action, T› | The action handler. This function gets called when the `call` method is invoked with the given action type. |

**Returns:** *void*

___

###  subscribe

▸ **subscribe**‹**E**›(`eventType`: E, `handler`: [ExtractEventHandler](../globals.md#extracteventhandler)‹Event, E›): *void*

Defined in ControllerMessenger.ts:480

Subscribe to an event.

Registers the given function as an event handler for the given event type.

**Type parameters:**

▪ **E**: *Event["type"]*

A type union of Event type strings.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`eventType` | E | The event type. This is a unique identifier for this event. |
`handler` | [ExtractEventHandler](../globals.md#extracteventhandler)‹Event, E› | The event handler. The type of the parameters for this event handler must match the type of the payload for this event type. |

**Returns:** *void*

▸ **subscribe**‹**E**, **V**›(`eventType`: E, `handler`: [SelectorEventHandler](../globals.md#selectoreventhandler)‹V›, `selector`: [SelectorFunction](../globals.md#selectorfunction)‹[ExtractEventPayload](../globals.md#extracteventpayload)‹Event, E›, V›): *void*

Defined in ControllerMessenger.ts:502

Subscribe to an event, with a selector.

Registers the given handler function as an event handler for the given
event type. When an event is published, its payload is first passed to the
selector. The event handler is only called if the selector's return value
differs from its last known return value.

**Type parameters:**

▪ **E**: *Event["type"]*

A type union of Event type strings.

▪ **V**

The selector return value.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`eventType` | E | The event type. This is a unique identifier for this event. |
`handler` | [SelectorEventHandler](../globals.md#selectoreventhandler)‹V› | The event handler. The type of the parameters for this event handler must match the return type of the selector. |
`selector` | [SelectorFunction](../globals.md#selectorfunction)‹[ExtractEventPayload](../globals.md#extracteventpayload)‹Event, E›, V› | The selector function used to select relevant data from the event payload. The type of the parameters for this selector must match the type of the payload for this event type. |

**Returns:** *void*

___

###  unregisterActionHandler

▸ **unregisterActionHandler**‹**T**›(`actionType`: T): *void*

Defined in ControllerMessenger.ts:400

Unregister an action handler.

This will prevent this action from being called.

**Type parameters:**

▪ **T**: *Action["type"]*

A type union of Action type strings.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`actionType` | T | The action type. This is a unqiue identifier for this action. |

**Returns:** *void*

___

###  unsubscribe

▸ **unsubscribe**‹**E**›(`eventType`: E, `handler`: [ExtractEventHandler](../globals.md#extracteventhandler)‹Event, E›): *void*

Defined in ControllerMessenger.ts:532

Unsubscribe from an event.

Unregisters the given function as an event handler for the given event.

**`throws`** Will throw when the given event handler is not registered for this event.

**Type parameters:**

▪ **E**: *Event["type"]*

A type union of Event type strings.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`eventType` | E | The event type. This is a unique identifier for this event. |
`handler` | [ExtractEventHandler](../globals.md#extracteventhandler)‹Event, E› | The event handler to unregister. |

**Returns:** *void*
