[slate](../README.md) › [Globals](../globals.md) › ["interfaces/point-ref"](../modules/_interfaces_point_ref_.md) › [PointRef](_interfaces_point_ref_.pointref.md)

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

*Defined in [interfaces/point-ref.ts:11](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/point-ref.ts#L11)*

___

###  current

• **current**: *[Point](_interfaces_point_.point.md) | null*

*Defined in [interfaces/point-ref.ts:10](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/point-ref.ts#L10)*

## Methods

###  unref

▸ **unref**(): *[Point](_interfaces_point_.point.md) | null*

*Defined in [interfaces/point-ref.ts:12](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/point-ref.ts#L12)*

**Returns:** *[Point](_interfaces_point_.point.md) | null*
