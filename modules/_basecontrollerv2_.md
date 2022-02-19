[metamask-controllers-main-src-gas-2](../README.md) › [Globals](../globals.md) › ["BaseControllerV2"](_basecontrollerv2_.md)

# Module: "BaseControllerV2"

## Index

### Classes

* [BaseController](../classes/_basecontrollerv2_.basecontroller.md)

### Interfaces

* [StatePropertyMetadata](../interfaces/_basecontrollerv2_.statepropertymetadata.md)

### Type aliases

* [Json](_basecontrollerv2_.md#json)
* [Listener](_basecontrollerv2_.md#listener)
* [StateDeriver](_basecontrollerv2_.md#statederiver)
* [StateMetadata](_basecontrollerv2_.md#statemetadata)

### Functions

* [deriveStateFromMetadata](_basecontrollerv2_.md#derivestatefrommetadata)
* [getAnonymizedState](_basecontrollerv2_.md#getanonymizedstate)
* [getPersistentState](_basecontrollerv2_.md#getpersistentstate)

## Type aliases

###  Json

Ƭ **Json**: *null | boolean | number | string | [Json](_basecontrollerv2_.md#json)[] | object*

Defined in BaseControllerV2.ts:64

___

###  Listener

Ƭ **Listener**: *function*

Defined in BaseControllerV2.ts:25

A state change listener.

This function will get called for each state change, and is given a copy of
the new state along with a set of patches describing the changes since the
last update.

**`param`** The new controller state.

**`param`** A list of patches describing any changes (see here for more
information: https://immerjs.github.io/immer/docs/patches)

#### Type declaration:

▸ (`state`: T, `patches`: Patch[]): *void*

**Parameters:**

Name | Type |
------ | ------ |
`state` | T |
`patches` | Patch[] |

___

###  StateDeriver

Ƭ **StateDeriver**: *function*

Defined in BaseControllerV2.ts:36

An function to derive state.

This function will accept one piece of the controller state (one property),
and will return some derivation of that state.

**`param`** A piece of controller state.

**`returns`** Something derived from controller state.

#### Type declaration:

▸ (`value`: T): *[Json](_basecontrollerv2_.md#json)*

**Parameters:**

Name | Type |
------ | ------ |
`value` | T |

___

###  StateMetadata

Ƭ **StateMetadata**: *object*

Defined in BaseControllerV2.ts:44

State metadata.

This metadata describes which parts of state should be persisted, and how to
get an anonymized representation of the state.

#### Type declaration:

## Functions

###  deriveStateFromMetadata

▸ **deriveStateFromMetadata**‹**S**›(`state`: S, `metadata`: [StateMetadata](_basecontrollerv2_.md#statemetadata)‹S›, `metadataProperty`: "anonymous" | "persist"): *Record‹string, [Json](_basecontrollerv2_.md#json)›*

Defined in BaseControllerV2.ts:232

Use the metadata to derive state according to the given metadata property.

**Type parameters:**

▪ **S**: *Record‹string, [Json](_basecontrollerv2_.md#json)›*

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`state` | S | The full controller state. |
`metadata` | [StateMetadata](_basecontrollerv2_.md#statemetadata)‹S› | The controller metadata. |
`metadataProperty` | "anonymous" &#124; "persist" | The metadata property to use to derive state. |

**Returns:** *Record‹string, [Json](_basecontrollerv2_.md#json)›*

The metadata-derived controller state.

___

###  getAnonymizedState

▸ **getAnonymizedState**‹**S**›(`state`: S, `metadata`: [StateMetadata](_basecontrollerv2_.md#statemetadata)‹S›): *Record‹string, [Json](_basecontrollerv2_.md#json)›*

Defined in BaseControllerV2.ts:203

Returns an anonymized representation of the controller state.

By "anonymized" we mean that it should not contain any information that could be personally
identifiable.

**Type parameters:**

▪ **S**: *Record‹string, [Json](_basecontrollerv2_.md#json)›*

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`state` | S | The controller state. |
`metadata` | [StateMetadata](_basecontrollerv2_.md#statemetadata)‹S› | The controller state metadata, which describes how to derive the anonymized state. |

**Returns:** *Record‹string, [Json](_basecontrollerv2_.md#json)›*

The anonymized controller state.

___

###  getPersistentState

▸ **getPersistentState**‹**S**›(`state`: S, `metadata`: [StateMetadata](_basecontrollerv2_.md#statemetadata)‹S›): *Record‹string, [Json](_basecontrollerv2_.md#json)›*

Defined in BaseControllerV2.ts:217

Returns the subset of state that should be persisted.

**Type parameters:**

▪ **S**: *Record‹string, [Json](_basecontrollerv2_.md#json)›*

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`state` | S | The controller state. |
`metadata` | [StateMetadata](_basecontrollerv2_.md#statemetadata)‹S› | The controller state metadata, which describes which pieces of state should be persisted. |

**Returns:** *Record‹string, [Json](_basecontrollerv2_.md#json)›*

The subset of controller state that should be persisted.
