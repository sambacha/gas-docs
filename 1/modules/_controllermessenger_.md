[ethereum-gas-reference](../README.md) › [Globals](../globals.md) › ["ControllerMessenger"](_controllermessenger_.md)

# Module: "ControllerMessenger"

## Index

### Classes

* [ControllerMessenger](../classes/_controllermessenger_.controllermessenger.md)
* [RestrictedControllerMessenger](../classes/_controllermessenger_.restrictedcontrollermessenger.md)

### Type aliases

* [ActionConstraint](_controllermessenger_.md#actionconstraint)
* [ActionHandler](_controllermessenger_.md#actionhandler)
* [EventConstraint](_controllermessenger_.md#eventconstraint)
* [EventSubscriptionMap](_controllermessenger_.md#eventsubscriptionmap)
* [ExtractActionParameters](_controllermessenger_.md#extractactionparameters)
* [ExtractActionResponse](_controllermessenger_.md#extractactionresponse)
* [ExtractEventHandler](_controllermessenger_.md#extracteventhandler)
* [ExtractEventPayload](_controllermessenger_.md#extracteventpayload)
* [GenericEventHandler](_controllermessenger_.md#genericeventhandler)
* [Namespaced](_controllermessenger_.md#namespaced)
* [NarrowToAllowed](_controllermessenger_.md#narrowtoallowed)
* [NarrowToNamespace](_controllermessenger_.md#narrowtonamespace)
* [SelectorEventHandler](_controllermessenger_.md#selectoreventhandler)
* [SelectorFunction](_controllermessenger_.md#selectorfunction)

## Type aliases

###  ActionConstraint

Ƭ **ActionConstraint**: *object*

Defined in ControllerMessenger.ts:36

#### Type declaration:

* **handler**(): *function*

  * (...`args`: any): *unknown*

* **type**: *string*

___

###  ActionHandler

Ƭ **ActionHandler**: *function*

Defined in ControllerMessenger.ts:1

#### Type declaration:

▸ (...`args`: [ExtractActionParameters](_controllermessenger_.md#extractactionparameters)‹Action, ActionType›): *[ExtractActionResponse](_controllermessenger_.md#extractactionresponse)‹Action, ActionType›*

**Parameters:**

Name | Type |
------ | ------ |
`...args` | [ExtractActionParameters](_controllermessenger_.md#extractactionparameters)‹Action, ActionType› |

___

###  EventConstraint

Ƭ **EventConstraint**: *object*

Defined in ControllerMessenger.ts:40

#### Type declaration:

* **payload**: *unknown[]*

* **type**: *string*

___

###  EventSubscriptionMap

Ƭ **EventSubscriptionMap**: *Map‹[GenericEventHandler](_controllermessenger_.md#genericeventhandler) | [SelectorEventHandler](_controllermessenger_.md#selectoreventhandler)‹unknown›, [SelectorFunction](_controllermessenger_.md#selectorfunction)‹any, unknown› | undefined›*

Defined in ControllerMessenger.ts:42

___

###  ExtractActionParameters

Ƭ **ExtractActionParameters**: *Action extends object ? H : never*

Defined in ControllerMessenger.ts:4

___

###  ExtractActionResponse

Ƭ **ExtractActionResponse**: *Action extends object ? H : never*

Defined in ControllerMessenger.ts:10

___

###  ExtractEventHandler

Ƭ **ExtractEventHandler**: *Event extends object ? P extends unknown[] ? function : never : never*

Defined in ControllerMessenger.ts:17

___

###  ExtractEventPayload

Ƭ **ExtractEventPayload**: *Event extends object ? P : never*

Defined in ControllerMessenger.ts:22

___

###  GenericEventHandler

Ƭ **GenericEventHandler**: *function*

Defined in ControllerMessenger.ts:26

#### Type declaration:

▸ (...`args`: unknown[]): *void*

**Parameters:**

Name | Type |
------ | ------ |
`...args` | unknown[] |

___

###  Namespaced

Ƭ **Namespaced**: *T extends  ?  : *

Defined in ControllerMessenger.ts:55

A namespaced string

This type verifies that the string T is prefixed by the string Name followed by a colon.

___

###  NarrowToAllowed

Ƭ **NarrowToAllowed**: *T extends object ? T : never*

Defined in ControllerMessenger.ts:65

___

###  NarrowToNamespace

Ƭ **NarrowToNamespace**: *T extends object ?  : *

Defined in ControllerMessenger.ts:59

___

###  SelectorEventHandler

Ƭ **SelectorEventHandler**: *function*

Defined in ControllerMessenger.ts:31

#### Type declaration:

▸ (`newValue`: SelectorReturnValue, `previousValue`: SelectorReturnValue | undefined): *void*

**Parameters:**

Name | Type |
------ | ------ |
`newValue` | SelectorReturnValue |
`previousValue` | SelectorReturnValue &#124; undefined |

___

###  SelectorFunction

Ƭ **SelectorFunction**: *function*

Defined in ControllerMessenger.ts:28

#### Type declaration:

▸ (...`args`: Args): *ReturnValue*

**Parameters:**

Name | Type |
------ | ------ |
`...args` | Args |
