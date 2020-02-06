
# External module: "interfaces/path"

## Index

### Type aliases

* [Path](_interfaces_path_.md#path)

### Object literals

* [Path](_interfaces_path_.md#const-path)

## Type aliases

###  Path

Ƭ **Path**: *number[]*

`Path` arrays are a list of indexes that describe a node's exact position in
a Slate node tree. Although they are usually relative to the root `Editor`
object, they can be relative to any `Node` object.

## Object literals

### `Const` Path

### ▪ **Path**: *object*

###  ancestors

▸ **ancestors**(`path`: [Path](_interfaces_path_.md#path), `options`: object): *[Path](_interfaces_path_.md#path)[]*

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

Get the common ancestor path of two paths.

**Parameters:**

Name | Type |
------ | ------ |
`path` | [Path](_interfaces_path_.md#path) |
`another` | [Path](_interfaces_path_.md#path) |

**Returns:** *[Path](_interfaces_path_.md#path)*

###  compare

▸ **compare**(`path`: [Path](_interfaces_path_.md#path), `another`: [Path](_interfaces_path_.md#path)): *-1 | 0 | 1*

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

Check if a path ends after one of the indexes in another.

**Parameters:**

Name | Type |
------ | ------ |
`path` | [Path](_interfaces_path_.md#path) |
`another` | [Path](_interfaces_path_.md#path) |

**Returns:** *boolean*

###  endsAt

▸ **endsAt**(`path`: [Path](_interfaces_path_.md#path), `another`: [Path](_interfaces_path_.md#path)): *boolean*

Check if a path ends at one of the indexes in another.

**Parameters:**

Name | Type |
------ | ------ |
`path` | [Path](_interfaces_path_.md#path) |
`another` | [Path](_interfaces_path_.md#path) |

**Returns:** *boolean*

###  endsBefore

▸ **endsBefore**(`path`: [Path](_interfaces_path_.md#path), `another`: [Path](_interfaces_path_.md#path)): *boolean*

Check if a path ends before one of the indexes in another.

**Parameters:**

Name | Type |
------ | ------ |
`path` | [Path](_interfaces_path_.md#path) |
`another` | [Path](_interfaces_path_.md#path) |

**Returns:** *boolean*

###  equals

▸ **equals**(`path`: [Path](_interfaces_path_.md#path), `another`: [Path](_interfaces_path_.md#path)): *boolean*

Check if a path is exactly equal to another.

**Parameters:**

Name | Type |
------ | ------ |
`path` | [Path](_interfaces_path_.md#path) |
`another` | [Path](_interfaces_path_.md#path) |

**Returns:** *boolean*

###  isAfter

▸ **isAfter**(`path`: [Path](_interfaces_path_.md#path), `another`: [Path](_interfaces_path_.md#path)): *boolean*

Check if a path is after another.

**Parameters:**

Name | Type |
------ | ------ |
`path` | [Path](_interfaces_path_.md#path) |
`another` | [Path](_interfaces_path_.md#path) |

**Returns:** *boolean*

###  isAncestor

▸ **isAncestor**(`path`: [Path](_interfaces_path_.md#path), `another`: [Path](_interfaces_path_.md#path)): *boolean*

Check if a path is an ancestor of another.

**Parameters:**

Name | Type |
------ | ------ |
`path` | [Path](_interfaces_path_.md#path) |
`another` | [Path](_interfaces_path_.md#path) |

**Returns:** *boolean*

###  isBefore

▸ **isBefore**(`path`: [Path](_interfaces_path_.md#path), `another`: [Path](_interfaces_path_.md#path)): *boolean*

Check if a path is before another.

**Parameters:**

Name | Type |
------ | ------ |
`path` | [Path](_interfaces_path_.md#path) |
`another` | [Path](_interfaces_path_.md#path) |

**Returns:** *boolean*

###  isChild

▸ **isChild**(`path`: [Path](_interfaces_path_.md#path), `another`: [Path](_interfaces_path_.md#path)): *boolean*

Check if a path is a child of another.

**Parameters:**

Name | Type |
------ | ------ |
`path` | [Path](_interfaces_path_.md#path) |
`another` | [Path](_interfaces_path_.md#path) |

**Returns:** *boolean*

###  isCommon

▸ **isCommon**(`path`: [Path](_interfaces_path_.md#path), `another`: [Path](_interfaces_path_.md#path)): *boolean*

Check if a path is equal to or an ancestor of another.

**Parameters:**

Name | Type |
------ | ------ |
`path` | [Path](_interfaces_path_.md#path) |
`another` | [Path](_interfaces_path_.md#path) |

**Returns:** *boolean*

###  isDescendant

▸ **isDescendant**(`path`: [Path](_interfaces_path_.md#path), `another`: [Path](_interfaces_path_.md#path)): *boolean*

Check if a path is a descendant of another.

**Parameters:**

Name | Type |
------ | ------ |
`path` | [Path](_interfaces_path_.md#path) |
`another` | [Path](_interfaces_path_.md#path) |

**Returns:** *boolean*

###  isParent

▸ **isParent**(`path`: [Path](_interfaces_path_.md#path), `another`: [Path](_interfaces_path_.md#path)): *boolean*

Check if a path is the parent of another.

**Parameters:**

Name | Type |
------ | ------ |
`path` | [Path](_interfaces_path_.md#path) |
`another` | [Path](_interfaces_path_.md#path) |

**Returns:** *boolean*

###  isPath

▸ **isPath**(`value`: any): *value is Path*

Check is a value implements the `Path` interface.

**Parameters:**

Name | Type |
------ | ------ |
`value` | any |

**Returns:** *value is Path*

###  isSibling

▸ **isSibling**(`path`: [Path](_interfaces_path_.md#path), `another`: [Path](_interfaces_path_.md#path)): *boolean*

Check if a path is a sibling of another.

**Parameters:**

Name | Type |
------ | ------ |
`path` | [Path](_interfaces_path_.md#path) |
`another` | [Path](_interfaces_path_.md#path) |

**Returns:** *boolean*

###  levels

▸ **levels**(`path`: [Path](_interfaces_path_.md#path), `options`: object): *[Path](_interfaces_path_.md#path)[]*

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

Given a path, get the path to the next sibling node.

**Parameters:**

Name | Type |
------ | ------ |
`path` | [Path](_interfaces_path_.md#path) |

**Returns:** *[Path](_interfaces_path_.md#path)*

###  parent

▸ **parent**(`path`: [Path](_interfaces_path_.md#path)): *[Path](_interfaces_path_.md#path)*

Given a path, return a new path referring to the parent node above it.

**Parameters:**

Name | Type |
------ | ------ |
`path` | [Path](_interfaces_path_.md#path) |

**Returns:** *[Path](_interfaces_path_.md#path)*

###  previous

▸ **previous**(`path`: [Path](_interfaces_path_.md#path)): *[Path](_interfaces_path_.md#path)*

Given a path, get the path to the previous sibling node.

**Parameters:**

Name | Type |
------ | ------ |
`path` | [Path](_interfaces_path_.md#path) |

**Returns:** *[Path](_interfaces_path_.md#path)*

###  relative

▸ **relative**(`path`: [Path](_interfaces_path_.md#path), `ancestor`: [Path](_interfaces_path_.md#path)): *[Path](_interfaces_path_.md#path)*

Get a path relative to an ancestor.

**Parameters:**

Name | Type |
------ | ------ |
`path` | [Path](_interfaces_path_.md#path) |
`ancestor` | [Path](_interfaces_path_.md#path) |

**Returns:** *[Path](_interfaces_path_.md#path)*

###  transform

▸ **transform**(`path`: [Path](_interfaces_path_.md#path), `operation`: [Operation](_interfaces_operation_.md#operation), `options`: object): *[Path](_interfaces_path_.md#path) | null*

Transform a path by an operation.

**Parameters:**

▪ **path**: *[Path](_interfaces_path_.md#path)*

▪ **operation**: *[Operation](_interfaces_operation_.md#operation)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`affinity?` | "forward" &#124; "backward" &#124; null |

**Returns:** *[Path](_interfaces_path_.md#path) | null*
