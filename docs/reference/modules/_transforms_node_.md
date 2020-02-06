[slate](../README.md) › [Globals](../globals.md) › ["transforms/node"](_transforms_node_.md)

# External module: "transforms/node"

## Index

### Functions

* [deleteRange](_transforms_node_.md#const-deleterange)
* [matchPath](_transforms_node_.md#const-matchpath)

### Object literals

* [NodeTransforms](_transforms_node_.md#const-nodetransforms)

## Functions

### `Const` deleteRange

▸ **deleteRange**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `range`: [Range](../interfaces/_interfaces_range_.range.md)): *[Point](../interfaces/_interfaces_point_.point.md) | null*

*Defined in [transforms/node.ts:848](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/transforms/node.ts#L848)*

Convert a range into a point by deleting it's content.

**Parameters:**

Name | Type |
------ | ------ |
`editor` | [Editor](../interfaces/_interfaces_editor_.editor.md) |
`range` | [Range](../interfaces/_interfaces_range_.range.md) |

**Returns:** *[Point](../interfaces/_interfaces_point_.point.md) | null*

___

### `Const` matchPath

▸ **matchPath**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `path`: [Path](_interfaces_path_.md#path)): *function*

*Defined in [transforms/node.ts:859](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/transforms/node.ts#L859)*

**Parameters:**

Name | Type |
------ | ------ |
`editor` | [Editor](../interfaces/_interfaces_editor_.editor.md) |
`path` | [Path](_interfaces_path_.md#path) |

**Returns:** *function*

▸ (`node`: [Node](_interfaces_node_.md#node)): *boolean*

**Parameters:**

Name | Type |
------ | ------ |
`node` | [Node](_interfaces_node_.md#node) |

## Object literals

### `Const` NodeTransforms

### ▪ **NodeTransforms**: *object*

*Defined in [transforms/node.ts:13](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/transforms/node.ts#L13)*

###  insertNodes

▸ **insertNodes**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `nodes`: [Node](_interfaces_node_.md#node) | [Node](_interfaces_node_.md#node)[], `options`: object): *void*

*Defined in [transforms/node.ts:18](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/transforms/node.ts#L18)*

Insert nodes at a specific location in the Editor.

**Parameters:**

▪ **editor**: *[Editor](../interfaces/_interfaces_editor_.editor.md)*

▪ **nodes**: *[Node](_interfaces_node_.md#node) | [Node](_interfaces_node_.md#node)[]*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`at?` | [Location](_interfaces_location_.md#location) |
`hanging?` | boolean |
`match?` | function |
`mode?` | "highest" &#124; "lowest" |
`select?` | boolean |
`voids?` | boolean |

**Returns:** *void*

###  liftNodes

▸ **liftNodes**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `options`: object): *void*

*Defined in [transforms/node.ts:136](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/transforms/node.ts#L136)*

Lift nodes at a specific location upwards in the document tree, splitting
their parent in two if necessary.

**Parameters:**

▪ **editor**: *[Editor](../interfaces/_interfaces_editor_.editor.md)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`at?` | [Location](_interfaces_location_.md#location) |
`match?` | function |
`mode?` | "all" &#124; "highest" &#124; "lowest" |
`voids?` | boolean |

**Returns:** *void*

###  mergeNodes

▸ **mergeNodes**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `options`: object): *void*

*Defined in [transforms/node.ts:199](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/transforms/node.ts#L199)*

Merge a node at a location with the previous node of the same depth,
removing any empty containing nodes after the merge if necessary.

**Parameters:**

▪ **editor**: *[Editor](../interfaces/_interfaces_editor_.editor.md)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`at?` | [Location](_interfaces_location_.md#location) |
`hanging?` | boolean |
`match?` | function |
`mode?` | "highest" &#124; "lowest" |
`voids?` | boolean |

**Returns:** *void*

###  moveNodes

▸ **moveNodes**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `options`: object): *void*

*Defined in [transforms/node.ts:338](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/transforms/node.ts#L338)*

Move the nodes at a location to a new location.

**Parameters:**

▪ **editor**: *[Editor](../interfaces/_interfaces_editor_.editor.md)*

▪ **options**: *object*

Name | Type |
------ | ------ |
`at?` | [Location](_interfaces_location_.md#location) |
`match?` | function |
`mode?` | "all" &#124; "highest" &#124; "lowest" |
`to` | [Path](_interfaces_path_.md#path) |
`voids?` | boolean |

**Returns:** *void*

###  removeNodes

▸ **removeNodes**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `options`: object): *void*

*Defined in [transforms/node.ts:388](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/transforms/node.ts#L388)*

Remove the nodes at a specific location in the document.

**Parameters:**

▪ **editor**: *[Editor](../interfaces/_interfaces_editor_.editor.md)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`at?` | [Location](_interfaces_location_.md#location) |
`hanging?` | boolean |
`match?` | function |
`mode?` | "highest" &#124; "lowest" |
`voids?` | boolean |

**Returns:** *void*

###  setNodes

▸ **setNodes**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `props`: Partial‹[Node](_interfaces_node_.md#node)›, `options`: object): *void*

*Defined in [transforms/node.ts:434](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/transforms/node.ts#L434)*

Set new properties on the nodes at a location.

**Parameters:**

▪ **editor**: *[Editor](../interfaces/_interfaces_editor_.editor.md)*

▪ **props**: *Partial‹[Node](_interfaces_node_.md#node)›*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`at?` | [Location](_interfaces_location_.md#location) |
`hanging?` | boolean |
`match?` | function |
`mode?` | "all" &#124; "highest" &#124; "lowest" |
`split?` | boolean |
`voids?` | boolean |

**Returns:** *void*

###  splitNodes

▸ **splitNodes**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `options`: object): *void*

*Defined in [transforms/node.ts:533](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/transforms/node.ts#L533)*

Split the nodes at a specific location.

**Parameters:**

▪ **editor**: *[Editor](../interfaces/_interfaces_editor_.editor.md)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`always?` | boolean |
`at?` | [Location](_interfaces_location_.md#location) |
`height?` | number |
`match?` | function |
`mode?` | "highest" &#124; "lowest" |
`voids?` | boolean |

**Returns:** *void*

###  unsetNodes

▸ **unsetNodes**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `props`: string | string[], `options`: object): *void*

*Defined in [transforms/node.ts:661](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/transforms/node.ts#L661)*

Unset properties on the nodes at a location.

**Parameters:**

▪ **editor**: *[Editor](../interfaces/_interfaces_editor_.editor.md)*

▪ **props**: *string | string[]*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`at?` | [Location](_interfaces_location_.md#location) |
`match?` | function |
`mode?` | "all" &#124; "highest" &#124; "lowest" |
`split?` | boolean |
`voids?` | boolean |

**Returns:** *void*

###  unwrapNodes

▸ **unwrapNodes**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `options`: object): *void*

*Defined in [transforms/node.ts:690](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/transforms/node.ts#L690)*

Unwrap the nodes at a location from a parent node, splitting the parent if
necessary to ensure that only the content in the range is unwrapped.

**Parameters:**

▪ **editor**: *[Editor](../interfaces/_interfaces_editor_.editor.md)*

▪ **options**: *object*

Name | Type |
------ | ------ |
`at?` | [Location](_interfaces_location_.md#location) |
`match?` | function |
`mode?` | "all" &#124; "highest" &#124; "lowest" |
`split?` | boolean |
`voids?` | boolean |

**Returns:** *void*

###  wrapNodes

▸ **wrapNodes**(`editor`: [Editor](../interfaces/_interfaces_editor_.editor.md), `element`: [Element](../interfaces/_interfaces_element_.element.md), `options`: object): *void*

*Defined in [transforms/node.ts:749](https://github.com/horacioh/slate/blob/b3461bd5/packages/slate/src/transforms/node.ts#L749)*

Wrap the nodes at a location in a new container node, splitting the edges
of the range first to ensure that only the content in the range is wrapped.

**Parameters:**

▪ **editor**: *[Editor](../interfaces/_interfaces_editor_.editor.md)*

▪ **element**: *[Element](../interfaces/_interfaces_element_.element.md)*

▪`Default value`  **options**: *object*= {}

Name | Type |
------ | ------ |
`at?` | [Location](_interfaces_location_.md#location) |
`match?` | function |
`mode?` | "all" &#124; "highest" &#124; "lowest" |
`split?` | boolean |
`voids?` | boolean |

**Returns:** *void*
