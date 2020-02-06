[slate](../README.md) › [Globals](../globals.md) › ["interfaces/path-ref"](../modules/_interfaces_path_ref_.md) › [PathRef](_interfaces_path_ref_.pathref.md)

# Interface: PathRef

`PathRef` objects keep a specific path in a document synced over time as new
operations are applied to the editor. You can access their `current` property
at any time for the up-to-date path value.

## Hierarchy

* **PathRef**

## Index

### Properties

* [affinity](_interfaces_path_ref_.pathref.md#affinity)
* [current](_interfaces_path_ref_.pathref.md#current)

### Methods

* [unref](_interfaces_path_ref_.pathref.md#unref)

## Properties

###  affinity

• **affinity**: *"forward" | "backward" | null*

*Defined in [interfaces/path-ref.ts:11](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/path-ref.ts#L11)*

___

###  current

• **current**: *[Path](../modules/_interfaces_path_.md#path) | null*

*Defined in [interfaces/path-ref.ts:10](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/path-ref.ts#L10)*

## Methods

###  unref

▸ **unref**(): *[Path](../modules/_interfaces_path_.md#path) | null*

*Defined in [interfaces/path-ref.ts:12](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/path-ref.ts#L12)*

**Returns:** *[Path](../modules/_interfaces_path_.md#path) | null*
