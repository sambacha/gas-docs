[ethereum-gas-reference](../README.md) › [Globals](../globals.md) › ["BaseControllerV2"](../modules/_basecontrollerv2_.md) › [StatePropertyMetadata](_basecontrollerv2_.statepropertymetadata.md)

# Interface: StatePropertyMetadata ‹**T**›

Metadata for a single state property

**`property`** persist - Indicates whether this property should be persisted
(`true` for persistent, `false` for transient), or is set to a function
that derives the persistent state from the state.

**`property`** anonymous - Indicates whether this property is already anonymous,
(`true` for anonymous, `false` if it has potential to be personally
identifiable), or is set to a function that returns an anonymized
representation of this state.

## Type parameters

▪ **T**: *[Json](../modules/_basecontrollerv2_.md#json)*

## Hierarchy

* **StatePropertyMetadata**

## Index

### Properties

* [anonymous](_basecontrollerv2_.statepropertymetadata.md#anonymous)
* [persist](_basecontrollerv2_.statepropertymetadata.md#persist)

## Properties

###  anonymous

• **anonymous**: *boolean | [StateDeriver](../modules/_basecontrollerv2_.md#statederiver)‹T›*

Defined in BaseControllerV2.ts:61

___

###  persist

• **persist**: *boolean | [StateDeriver](../modules/_basecontrollerv2_.md#statederiver)‹T›*

Defined in BaseControllerV2.ts:60
