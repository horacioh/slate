
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

___

###  current

• **current**: *[Path](../modules/_interfaces_path_.md#path) | null*

## Methods

###  unref

▸ **unref**(): *[Path](../modules/_interfaces_path_.md#path) | null*

**Returns:** *[Path](../modules/_interfaces_path_.md#path) | null*
