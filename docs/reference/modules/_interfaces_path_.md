[slate](../README.md) › [Globals](../globals.md) › ["interfaces/path"](_interfaces_path_.md)

# External module: "interfaces/path"

## Index

### Type aliases

* [Path](_interfaces_path_.md#path)

### Object literals

* [Path](_interfaces_path_.md#const-path)

## Type aliases

###  Path

Ƭ **Path**: *number[]*

*Defined in [interfaces/path.ts:10](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/path.ts#L10)*

`Path` arrays are a list of indexes that describe a node's exact position in
a Slate node tree. Although they are usually relative to the root `Editor`
object, they can be relative to any `Node` object.

## Object literals

### `Const` Path

### ▪ **Path**: *object*

*Defined in [interfaces/path.ts:12](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/path.ts#L12)*

###  ancestors

▸ **ancestors**(`path`: [Path](_interfaces_path_.md#path), `options`: object): *[Path](_interfaces_path_.md#path)[]*

*Defined in [interfaces/path.ts:20](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/path.ts#L20)*

Get a list of ancestor paths for a given path.

The paths are sorted from deepest to shallowest ancestor. However, if the
`reverse: true` option is passed, they are reversed.

**Parameters:**

▪ **path**: *[Path](_interfaces_path_.md#path)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`reverse?` | boolean |

**Returns:** *[Path](_interfaces_path_.md#path)[]*

###  common

▸ **common**(`path`: [Path](_interfaces_path_.md#path), `another`: [Path](_interfaces_path_.md#path)): *[Path](_interfaces_path_.md#path)*

*Defined in [interfaces/path.ts:37](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/path.ts#L37)*

Get the common ancestor path of two paths.

**Parameters:**

Name | Type |
------ | ------ |
`path` | [Path](_interfaces_path_.md#path) |
`another` | [Path](_interfaces_path_.md#path) |

**Returns:** *[Path](_interfaces_path_.md#path)*

###  compare

▸ **compare**(`path`: [Path](_interfaces_path_.md#path), `another`: [Path](_interfaces_path_.md#path)): *-1 | 0 | 1*

*Defined in [interfaces/path.ts:63](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/path.ts#L63)*

Compare a path to another, returning an integer indicating whether the path
was before, at, or after the other.

Note: Two paths of unequal length can still receive a `0` result if one is
directly above or below the other. If you want exact matching, use
[Path.equals](_interfaces_path_.md#equals) instead.

**Parameters:**

Name | Type |
------ | ------ |
`path` | [Path](_interfaces_path_.md#path) |
`another` | [Path](_interfaces_path_.md#path) |

**Returns:** *-1 | 0 | 1*

###  endsAfter

▸ **endsAfter**(`path`: [Path](_interfaces_path_.md#path), `another`: [Path](_interfaces_path_.md#path)): *boolean*

*Defined in [interfaces/path.ts:78](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/path.ts#L78)*

Check if a path ends after one of the indexes in another.

**Parameters:**

Name | Type |
------ | ------ |
`path` | [Path](_interfaces_path_.md#path) |
`another` | [Path](_interfaces_path_.md#path) |

**Returns:** *boolean*

###  endsAt

▸ **endsAt**(`path`: [Path](_interfaces_path_.md#path), `another`: [Path](_interfaces_path_.md#path)): *boolean*

*Defined in [interfaces/path.ts:91](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/path.ts#L91)*

Check if a path ends at one of the indexes in another.

**Parameters:**

Name | Type |
------ | ------ |
`path` | [Path](_interfaces_path_.md#path) |
`another` | [Path](_interfaces_path_.md#path) |

**Returns:** *boolean*

###  endsBefore

▸ **endsBefore**(`path`: [Path](_interfaces_path_.md#path), `another`: [Path](_interfaces_path_.md#path)): *boolean*

*Defined in [interfaces/path.ts:102](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/path.ts#L102)*

Check if a path ends before one of the indexes in another.

**Parameters:**

Name | Type |
------ | ------ |
`path` | [Path](_interfaces_path_.md#path) |
`another` | [Path](_interfaces_path_.md#path) |

**Returns:** *boolean*

###  equals

▸ **equals**(`path`: [Path](_interfaces_path_.md#path), `another`: [Path](_interfaces_path_.md#path)): *boolean*

*Defined in [interfaces/path.ts:115](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/path.ts#L115)*

Check if a path is exactly equal to another.

**Parameters:**

Name | Type |
------ | ------ |
`path` | [Path](_interfaces_path_.md#path) |
`another` | [Path](_interfaces_path_.md#path) |

**Returns:** *boolean*

###  isAfter

▸ **isAfter**(`path`: [Path](_interfaces_path_.md#path), `another`: [Path](_interfaces_path_.md#path)): *boolean*

*Defined in [interfaces/path.ts:125](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/path.ts#L125)*

Check if a path is after another.

**Parameters:**

Name | Type |
------ | ------ |
`path` | [Path](_interfaces_path_.md#path) |
`another` | [Path](_interfaces_path_.md#path) |

**Returns:** *boolean*

###  isAncestor

▸ **isAncestor**(`path`: [Path](_interfaces_path_.md#path), `another`: [Path](_interfaces_path_.md#path)): *boolean*

*Defined in [interfaces/path.ts:133](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/path.ts#L133)*

Check if a path is an ancestor of another.

**Parameters:**

Name | Type |
------ | ------ |
`path` | [Path](_interfaces_path_.md#path) |
`another` | [Path](_interfaces_path_.md#path) |

**Returns:** *boolean*

###  isBefore

▸ **isBefore**(`path`: [Path](_interfaces_path_.md#path), `another`: [Path](_interfaces_path_.md#path)): *boolean*

*Defined in [interfaces/path.ts:141](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/path.ts#L141)*

Check if a path is before another.

**Parameters:**

Name | Type |
------ | ------ |
`path` | [Path](_interfaces_path_.md#path) |
`another` | [Path](_interfaces_path_.md#path) |

**Returns:** *boolean*

###  isChild

▸ **isChild**(`path`: [Path](_interfaces_path_.md#path), `another`: [Path](_interfaces_path_.md#path)): *boolean*

*Defined in [interfaces/path.ts:149](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/path.ts#L149)*

Check if a path is a child of another.

**Parameters:**

Name | Type |
------ | ------ |
`path` | [Path](_interfaces_path_.md#path) |
`another` | [Path](_interfaces_path_.md#path) |

**Returns:** *boolean*

###  isCommon

▸ **isCommon**(`path`: [Path](_interfaces_path_.md#path), `another`: [Path](_interfaces_path_.md#path)): *boolean*

*Defined in [interfaces/path.ts:159](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/path.ts#L159)*

Check if a path is equal to or an ancestor of another.

**Parameters:**

Name | Type |
------ | ------ |
`path` | [Path](_interfaces_path_.md#path) |
`another` | [Path](_interfaces_path_.md#path) |

**Returns:** *boolean*

###  isDescendant

▸ **isDescendant**(`path`: [Path](_interfaces_path_.md#path), `another`: [Path](_interfaces_path_.md#path)): *boolean*

*Defined in [interfaces/path.ts:167](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/path.ts#L167)*

Check if a path is a descendant of another.

**Parameters:**

Name | Type |
------ | ------ |
`path` | [Path](_interfaces_path_.md#path) |
`another` | [Path](_interfaces_path_.md#path) |

**Returns:** *boolean*

###  isParent

▸ **isParent**(`path`: [Path](_interfaces_path_.md#path), `another`: [Path](_interfaces_path_.md#path)): *boolean*

*Defined in [interfaces/path.ts:175](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/path.ts#L175)*

Check if a path is the parent of another.

**Parameters:**

Name | Type |
------ | ------ |
`path` | [Path](_interfaces_path_.md#path) |
`another` | [Path](_interfaces_path_.md#path) |

**Returns:** *boolean*

###  isPath

▸ **isPath**(`value`: any): *value is Path*

*Defined in [interfaces/path.ts:185](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/path.ts#L185)*

Check is a value implements the `Path` interface.

**Parameters:**

Name | Type |
------ | ------ |
`value` | any |

**Returns:** *value is Path*

###  isSibling

▸ **isSibling**(`path`: [Path](_interfaces_path_.md#path), `another`: [Path](_interfaces_path_.md#path)): *boolean*

*Defined in [interfaces/path.ts:196](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/path.ts#L196)*

Check if a path is a sibling of another.

**Parameters:**

Name | Type |
------ | ------ |
`path` | [Path](_interfaces_path_.md#path) |
`another` | [Path](_interfaces_path_.md#path) |

**Returns:** *boolean*

###  levels

▸ **levels**(`path`: [Path](_interfaces_path_.md#path), `options`: object): *[Path](_interfaces_path_.md#path)[]*

*Defined in [interfaces/path.ts:216](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/path.ts#L216)*

Get a list of paths at every level down to a path. Note: this is the same
as `Path.ancestors`, but including the path itself.

The paths are sorted from shallowest to deepest. However, if the `reverse:
true` option is passed, they are reversed.

**Parameters:**

▪ **path**: *[Path](_interfaces_path_.md#path)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`reverse?` | boolean |

**Returns:** *[Path](_interfaces_path_.md#path)[]*

###  next

▸ **next**(`path`: [Path](_interfaces_path_.md#path)): *[Path](_interfaces_path_.md#path)*

*Defined in [interfaces/path.ts:240](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/path.ts#L240)*

Given a path, get the path to the next sibling node.

**Parameters:**

Name | Type |
------ | ------ |
`path` | [Path](_interfaces_path_.md#path) |

**Returns:** *[Path](_interfaces_path_.md#path)*

###  parent

▸ **parent**(`path`: [Path](_interfaces_path_.md#path)): *[Path](_interfaces_path_.md#path)*

*Defined in [interfaces/path.ts:255](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/path.ts#L255)*

Given a path, return a new path referring to the parent node above it.

**Parameters:**

Name | Type |
------ | ------ |
`path` | [Path](_interfaces_path_.md#path) |

**Returns:** *[Path](_interfaces_path_.md#path)*

###  previous

▸ **previous**(`path`: [Path](_interfaces_path_.md#path)): *[Path](_interfaces_path_.md#path)*

*Defined in [interfaces/path.ts:267](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/path.ts#L267)*

Given a path, get the path to the previous sibling node.

**Parameters:**

Name | Type |
------ | ------ |
`path` | [Path](_interfaces_path_.md#path) |

**Returns:** *[Path](_interfaces_path_.md#path)*

###  relative

▸ **relative**(`path`: [Path](_interfaces_path_.md#path), `ancestor`: [Path](_interfaces_path_.md#path)): *[Path](_interfaces_path_.md#path)*

*Defined in [interfaces/path.ts:289](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/path.ts#L289)*

Get a path relative to an ancestor.

**Parameters:**

Name | Type |
------ | ------ |
`path` | [Path](_interfaces_path_.md#path) |
`ancestor` | [Path](_interfaces_path_.md#path) |

**Returns:** *[Path](_interfaces_path_.md#path)*

###  transform

▸ **transform**(`path`: [Path](_interfaces_path_.md#path), `operation`: [Operation](_interfaces_operation_.md#operation), `options`: object): *[Path](_interfaces_path_.md#path) | null*

*Defined in [interfaces/path.ts:303](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/interfaces/path.ts#L303)*

Transform a path by an operation.

**Parameters:**

▪ **path**: *[Path](_interfaces_path_.md#path)*

▪ **operation**: *[Operation](_interfaces_operation_.md#operation)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`affinity?` | "forward" &#124; "backward" &#124; null |

**Returns:** *[Path](_interfaces_path_.md#path) | null*
