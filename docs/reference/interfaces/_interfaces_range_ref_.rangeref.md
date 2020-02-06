
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

___

###  current

• **current**: *[Range](_interfaces_range_.range.md) | null*

## Methods

###  unref

▸ **unref**(): *[Range](_interfaces_range_.range.md) | null*

**Returns:** *[Range](_interfaces_range_.range.md) | null*
