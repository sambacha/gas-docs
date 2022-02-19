[ethereum-gas-reference](../README.md) › [Globals](../globals.md) › [StatePropertyMetadata](statepropertymetadata.md)

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

▪ **T**: *[Json](../globals.md#json)*

## Hierarchy

* **StatePropertyMetadata**

## Index

### Properties

* [anonymous](statepropertymetadata.md#anonymous)
* [persist](statepropertymetadata.md#persist)

## Properties

###  anonymous

• **anonymous**: *boolean | [StateDeriver](../globals.md#statederiver)‹T›*

Defined in BaseControllerV2.ts:61

___

###  persist

• **persist**: *boolean | [StateDeriver](../globals.md#statederiver)‹T›*

Defined in BaseControllerV2.ts:60
