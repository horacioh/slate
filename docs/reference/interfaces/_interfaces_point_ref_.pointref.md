
# Interface: PointRef

`PointRef` objects keep a specific point in a document synced over time as new
operations are applied to the editor. You can access their `current` property
at any time for the up-to-date point value.

## Hierarchy

* **PointRef**

## Index

### Properties

* [affinity](_interfaces_point_ref_.pointref.md#affinity)
* [current](_interfaces_point_ref_.pointref.md#current)

### Methods

* [unref](_interfaces_point_ref_.pointref.md#unref)

## Properties

###  affinity

• **affinity**: *"forward" | "backward" | null*

___

###  current

• **current**: *[Point](_interfaces_point_.point.md) | null*

## Methods

###  unref

▸ **unref**(): *[Point](_interfaces_point_.point.md) | null*

**Returns:** *[Point](_interfaces_point_.point.md) | null*
