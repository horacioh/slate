[slate](../README.md) › [Globals](../globals.md) › ["interfaces/range-ref"](../modules/_interfaces_range_ref_.md) › [RangeRef](_interfaces_range_ref_.rangeref.md)

# Interface: RangeRef

`RangeRef` objects keep a specific range in a document synced over time as new
operations are applied to the editor. You can access their `current` property
at any time for the up-to-date range value.

## Hierarchy

* **RangeRef**

## Index

### Properties

* [affinity](_interfaces_range_ref_.rangeref.md#affinity)
* [current](_interfaces_range_ref_.rangeref.md#current)

### Methods

* [unref](_interfaces_range_ref_.rangeref.md#unref)

## Properties

###  affinity

• **affinity**: *"forward" | "backward" | "outward" | "inward" | null*

*Defined in [interfaces/range-ref.ts:11](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/range-ref.ts#L11)*

___

###  current

• **current**: *[Range](_interfaces_range_.range.md) | null*

*Defined in [interfaces/range-ref.ts:10](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/range-ref.ts#L10)*

## Methods

###  unref

▸ **unref**(): *[Range](_interfaces_range_.range.md) | null*

*Defined in [interfaces/range-ref.ts:12](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/range-ref.ts#L12)*

**Returns:** *[Range](_interfaces_range_.range.md) | null*
